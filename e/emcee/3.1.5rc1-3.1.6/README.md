# Comparing `tmp/emcee-3.1.5rc1.tar.gz` & `tmp/emcee-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emcee-3.1.5rc1.tar", last modified: Wed Apr 10 20:13:49 2024, max compression
+gzip compressed data, was "emcee-3.1.6.tar", last modified: Fri Apr 19 09:50:06 2024, max compression
```

## Comparing `emcee-3.1.5rc1.tar` & `emcee-3.1.6.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/VISION.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/binder/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/binder/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/_static/line/
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-data.png
--rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-least-squares.png
--rw-r--r--   0 runner    (1001) docker     (127)    34934 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-max-likelihood.png
--rw-r--r--   0 runner    (1001) docker     (127)    67232 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-mcmc.png
--rw-r--r--   0 runner    (1001) docker     (127)   404073 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-time.png
--rw-r--r--   0 runner    (1001) docker     (127)   126982 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-triangle.png
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo-sidebar.png
--rw-r--r--   0 runner    (1001) docker     (127)   150797 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo.pxm
--rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo2.png
--rw-r--r--   0 runner    (1001) docker     (127)   240605 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo2.pxm
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/fix_internal_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.290466 emcee-3.1.5rc1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)   515948 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/autocorr.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   865248 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1100525 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/monitor.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   245392 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/moves.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/parallel.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/tutorial_rst.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/docs/user/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/autocorr.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/backends.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/blobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/moves.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/sampler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/document/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    66184 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/aastex.cls
--rw-r--r--   0 runner    (1001) docker     (127)    41540 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/ms.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/document/plots/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/plots/oned.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/plots/plot_acor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/joss/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/make_latex.sh
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.tex
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2376 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.278466 emcee-3.1.5rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.298467 emcee-3.1.5rc1/src/emcee/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/autocorr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.298467 emcee-3.1.5rc1/src/emcee/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee/emcee_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25923 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/interruptible_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/moves/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/de.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/de_snooker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/mh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/move.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/red_blue.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/stretch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/walk.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/pbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/ptsampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_de.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_de_snooker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_longdouble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_stretch.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_autocorr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_blobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_stretch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.431932 emcee-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 09:49:57.000000 emcee-3.1.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.407933 emcee-3.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-19 09:49:57.000000 emcee-3.1.6/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 09:49:57.000000 emcee-3.1.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.407933 emcee-3.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-19 09:49:57.000000 emcee-3.1.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 09:49:57.000000 emcee-3.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 09:49:57.000000 emcee-3.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 09:49:57.000000 emcee-3.1.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 09:49:57.000000 emcee-3.1.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-19 09:49:57.000000 emcee-3.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-19 09:49:57.000000 emcee-3.1.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-19 09:49:57.000000 emcee-3.1.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-19 09:49:57.000000 emcee-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 09:49:57.000000 emcee-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-19 09:50:06.431932 emcee-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-19 09:49:57.000000 emcee-3.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 09:49:57.000000 emcee-3.1.6/VISION.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.407933 emcee-3.1.6/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 09:49:57.000000 emcee-3.1.6/binder/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.411933 emcee-3.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.411933 emcee-3.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.411933 emcee-3.1.6/docs/_static/line/
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/line/line-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/line/line-least-squares.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34934 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/line/line-max-likelihood.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67232 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/line/line-mcmc.png
+-rw-r--r--   0 runner    (1001) docker     (127)   404073 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/line/line-time.png
+-rw-r--r--   0 runner    (1001) docker     (127)   126982 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/line/line-triangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/logo-sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (127)   150797 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/logo.pxm
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/logo2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   240605 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/_static/logo2.pxm
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/fix_internal_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.419932 emcee-3.1.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   515948 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/tutorials/autocorr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   865248 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/tutorials/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1100525 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/tutorials/monitor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   245392 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/tutorials/moves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/tutorials/parallel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/tutorials/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/tutorials/tutorial_rst.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.419932 emcee-3.1.6/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/autocorr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/blobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/moves.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-19 09:49:57.000000 emcee-3.1.6/docs/user/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.419932 emcee-3.1.6/document/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 09:49:57.000000 emcee-3.1.6/document/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-19 09:49:57.000000 emcee-3.1.6/document/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    66184 2024-04-19 09:49:57.000000 emcee-3.1.6/document/aastex.cls
+-rw-r--r--   0 runner    (1001) docker     (127)    41540 2024-04-19 09:49:57.000000 emcee-3.1.6/document/ms.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.419932 emcee-3.1.6/document/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-19 09:49:57.000000 emcee-3.1.6/document/plots/oned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 09:49:57.000000 emcee-3.1.6/document/plots/plot_acor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.419932 emcee-3.1.6/joss/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 09:49:57.000000 emcee-3.1.6/joss/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-04-19 09:49:57.000000 emcee-3.1.6/joss/make_latex.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-19 09:49:57.000000 emcee-3.1.6/joss/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-19 09:49:57.000000 emcee-3.1.6/joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-19 09:49:57.000000 emcee-3.1.6/joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-19 09:49:57.000000 emcee-3.1.6/joss/paper.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 09:49:57.000000 emcee-3.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:50:06.431932 emcee-3.1.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2376 2024-04-19 09:49:57.000000 emcee-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.403933 emcee-3.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.423932 emcee-3.1.6/src/emcee/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/autocorr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.423932 emcee-3.1.6/src/emcee/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/backends/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 09:50:06.000000 emcee-3.1.6/src/emcee/emcee_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26186 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/interruptible_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.427932 emcee-3.1.6/src/emcee/moves/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/de_snooker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/mh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/red_blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/moves/walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/pbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/ptsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.427932 emcee-3.1.6/src/emcee/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.427932 emcee-3.1.6/src/emcee/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_de_snooker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_longdouble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/integration/test_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.431932 emcee-3.1.6/src/emcee/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/test_autocorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/test_blobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/tests/unit/test_stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 09:49:57.000000 emcee-3.1.6/src/emcee/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:50:06.431932 emcee-3.1.6/src/emcee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-19 09:50:06.000000 emcee-3.1.6/src/emcee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-19 09:50:06.000000 emcee-3.1.6/src/emcee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:50:06.000000 emcee-3.1.6/src/emcee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:50:06.000000 emcee-3.1.6/src/emcee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 09:50:06.000000 emcee-3.1.6/src/emcee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 09:50:06.000000 emcee-3.1.6/src/emcee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 09:49:57.000000 emcee-3.1.6/tox.ini
```

### Comparing `emcee-3.1.5rc1/.github/ISSUE_TEMPLATE.md` & `emcee-3.1.6/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/.github/workflows/tests.yml` & `emcee-3.1.6/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -45,34 +45,39 @@
           python -m coverage xml -i
           python -m coveralls --service=github
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           COVERALLS_PARALLEL: true
           COVERALLS_FLAG_NAME: ${{ matrix.python-version }}-${{ matrix.os }}
 
-  leading_edge:
+  numpy_edge:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version: ["3.12"]
+        numpy-version: ["numpy>=2.0.0rc1"]
         os: ["ubuntu-latest"]
+        include:
+          - python-version: "3.9"
+            numpy-version: "numpy<1.25"
+            os: "ubuntu-latest"
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install pip install pytest "numpy>=2.0.0rc1"
+          python -m pip install pip install pytest "${{ matrix.numpy-version }}"
           python -m pip install -e.
       - name: Run tests
         run: pytest
 
   coverage:
     needs: tests
     runs-on: ubuntu-latest
```

### Comparing `emcee-3.1.5rc1/CODE_OF_CONDUCT.md` & `emcee-3.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/CONTRIBUTING.md` & `emcee-3.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/HISTORY.rst` & `emcee-3.1.6/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/LICENSE` & `emcee-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/PKG-INFO` & `emcee-3.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emcee
-Version: 3.1.5rc1
+Version: 3.1.6
 Summary: The Python ensemble sampling toolkit for MCMC
 Home-page: https://emcee.readthedocs.io
 Author: Daniel Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Maintainer: Daniel Foreman-Mackey
 Maintainer-email: foreman.mackey@gmail.com
 License: MIT
```

### Comparing `emcee-3.1.5rc1/README.rst` & `emcee-3.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/Makefile` & `emcee-3.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/favicon.png` & `emcee-3.1.6/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/line/line-data.png` & `emcee-3.1.6/docs/_static/line/line-data.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/line/line-least-squares.png` & `emcee-3.1.6/docs/_static/line/line-least-squares.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/line/line-max-likelihood.png` & `emcee-3.1.6/docs/_static/line/line-max-likelihood.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/line/line-mcmc.png` & `emcee-3.1.6/docs/_static/line/line-mcmc.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/line/line-time.png` & `emcee-3.1.6/docs/_static/line/line-time.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/line/line-triangle.png` & `emcee-3.1.6/docs/_static/line/line-triangle.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/logo-sidebar.png` & `emcee-3.1.6/docs/_static/logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/logo.pxm` & `emcee-3.1.6/docs/_static/logo.pxm`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/logo2.png` & `emcee-3.1.6/docs/_static/logo2.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/_static/logo2.pxm` & `emcee-3.1.6/docs/_static/logo2.pxm`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/conf.py` & `emcee-3.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/index.rst` & `emcee-3.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/tutorials/autocorr.ipynb` & `emcee-3.1.6/docs/tutorials/autocorr.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/tutorials/line.ipynb` & `emcee-3.1.6/docs/tutorials/line.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/tutorials/monitor.ipynb` & `emcee-3.1.6/docs/tutorials/monitor.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/tutorials/moves.ipynb` & `emcee-3.1.6/docs/tutorials/moves.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/tutorials/parallel.ipynb` & `emcee-3.1.6/docs/tutorials/parallel.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/tutorials/quickstart.ipynb` & `emcee-3.1.6/docs/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/tutorials/tutorial_rst.tpl` & `emcee-3.1.6/docs/tutorials/tutorial_rst.tpl`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/user/backends.rst` & `emcee-3.1.6/docs/user/backends.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/user/blobs.rst` & `emcee-3.1.6/docs/user/blobs.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/user/faq.rst` & `emcee-3.1.6/docs/user/faq.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/user/install.rst` & `emcee-3.1.6/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/user/moves.rst` & `emcee-3.1.6/docs/user/moves.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/docs/user/upgrade.rst` & `emcee-3.1.6/docs/user/upgrade.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/document/aastex.cls` & `emcee-3.1.6/document/aastex.cls`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/document/ms.tex` & `emcee-3.1.6/document/ms.tex`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/document/plots/oned.py` & `emcee-3.1.6/document/plots/oned.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/joss/make_latex.sh` & `emcee-3.1.6/joss/make_latex.sh`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/joss/metadata.yaml` & `emcee-3.1.6/joss/metadata.yaml`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/joss/paper.bib` & `emcee-3.1.6/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/joss/paper.md` & `emcee-3.1.6/joss/paper.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/joss/paper.tex` & `emcee-3.1.6/joss/paper.tex`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/pyproject.toml` & `emcee-3.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/setup.py` & `emcee-3.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/__init__.py` & `emcee-3.1.6/src/emcee/__init__.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/autocorr.py` & `emcee-3.1.6/src/emcee/autocorr.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/backends/backend.py` & `emcee-3.1.6/src/emcee/backends/backend.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/backends/hdf.py` & `emcee-3.1.6/src/emcee/backends/hdf.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/ensemble.py` & `emcee-3.1.6/src/emcee/ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 
 try:
     from collections.abc import Iterable
 except ImportError:
     # for py2.7, will be an Exception in 3.8
     from collections import Iterable
 
+try:
+    # Try to import from numpy.exceptions (available in NumPy 1.25 and later)
+    from numpy.exceptions import VisibleDeprecationWarning
+except ImportError:
+    # Fallback to the top-level numpy import (for older versions)
+    from numpy import VisibleDeprecationWarning
+
 
 class EnsembleSampler(object):
     """An ensemble MCMC sampler
 
     If you are upgrading from an earlier version of emcee, you might notice
     that some arguments are now deprecated. The parameters that control the
     proposals have been moved to the :ref:`moves-user` interface (``a`` and
@@ -507,15 +514,15 @@
             # Get the blobs dtype
             if self.blobs_dtype is not None:
                 dt = self.blobs_dtype
             else:
                 try:
                     with warnings.catch_warnings(record=True):
                         warnings.simplefilter(
-                            "error", np.exceptions.VisibleDeprecationWarning
+                            "error", VisibleDeprecationWarning
                         )
                         try:
                             dt = np.atleast_1d(blob[0]).dtype
                         except Warning:
                             deprecation_warning(
                                 "You have provided blobs that are not all the "
                                 "same shape or size. This means they must be "
```

### Comparing `emcee-3.1.5rc1/src/emcee/moves/de.py` & `emcee-3.1.6/src/emcee/moves/de.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/de_snooker.py` & `emcee-3.1.6/src/emcee/moves/de_snooker.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/gaussian.py` & `emcee-3.1.6/src/emcee/moves/gaussian.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/kde.py` & `emcee-3.1.6/src/emcee/moves/kde.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/mh.py` & `emcee-3.1.6/src/emcee/moves/mh.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/move.py` & `emcee-3.1.6/src/emcee/moves/move.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/red_blue.py` & `emcee-3.1.6/src/emcee/moves/red_blue.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/stretch.py` & `emcee-3.1.6/src/emcee/moves/stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/moves/walk.py` & `emcee-3.1.6/src/emcee/moves/walk.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/pbar.py` & `emcee-3.1.6/src/emcee/pbar.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/state.py` & `emcee-3.1.6/src/emcee/state.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/integration/test_gaussian.py` & `emcee-3.1.6/src/emcee/tests/integration/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/integration/test_kde.py` & `emcee-3.1.6/src/emcee/tests/integration/test_kde.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/integration/test_longdouble.py` & `emcee-3.1.6/src/emcee/tests/integration/test_longdouble.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/integration/test_proposal.py` & `emcee-3.1.6/src/emcee/tests/integration/test_proposal.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/integration/test_stretch.py` & `emcee-3.1.6/src/emcee/tests/integration/test_stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/unit/test_autocorr.py` & `emcee-3.1.6/src/emcee/tests/unit/test_autocorr.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/unit/test_backends.py` & `emcee-3.1.6/src/emcee/tests/unit/test_backends.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/unit/test_blobs.py` & `emcee-3.1.6/src/emcee/tests/unit/test_blobs.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/unit/test_ensemble.py` & `emcee-3.1.6/src/emcee/tests/unit/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/unit/test_sampler.py` & `emcee-3.1.6/src/emcee/tests/unit/test_sampler.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/unit/test_state.py` & `emcee-3.1.6/src/emcee/tests/unit/test_state.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/tests/unit/test_stretch.py` & `emcee-3.1.6/src/emcee/tests/unit/test_stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee/utils.py` & `emcee-3.1.6/src/emcee/utils.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5rc1/src/emcee.egg-info/PKG-INFO` & `emcee-3.1.6/src/emcee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emcee
-Version: 3.1.5rc1
+Version: 3.1.6
 Summary: The Python ensemble sampling toolkit for MCMC
 Home-page: https://emcee.readthedocs.io
 Author: Daniel Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Maintainer: Daniel Foreman-Mackey
 Maintainer-email: foreman.mackey@gmail.com
 License: MIT
```

### Comparing `emcee-3.1.5rc1/src/emcee.egg-info/SOURCES.txt` & `emcee-3.1.6/src/emcee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

