# Comparing `tmp/kilosort-4.0.4.tar.gz` & `tmp/kilosort-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilosort-4.0.4.tar", last modified: Sat Apr 13 21:11:55 2024, max compression
+gzip compressed data, was "kilosort-4.0.5.tar", last modified: Fri Apr 19 18:45:04 2024, max compression
```

## Comparing `kilosort-4.0.4.tar` & `kilosort-4.0.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.791759 kilosort-4.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.775759 kilosort-4.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.775759 kilosort-4.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/installation_issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/other.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.775759 kilosort-4.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-13 21:11:45.000000 kilosort-4.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-13 21:11:45.000000 kilosort-4.0.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-13 21:11:45.000000 kilosort-4.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 21:11:45.000000 kilosort-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-13 21:11:55.791759 kilosort-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-13 21:11:45.000000 kilosort-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.779759 kilosort-4.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/drift.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/gui_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/hardware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/multi_shank.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.779759 kilosort-4.0.4/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/basic_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/load_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/make_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.783758 kilosort-4.0.4/kilosort/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/CCG.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/clustering_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/datashift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.787758 kilosort-4.0.4/kilosort/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/data_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/header_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/message_log_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/minor_gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/probe_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/run_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/sanity_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/settings_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/run_kilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/swarmsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/template_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/wTEMP.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.787758 kilosort-4.0.4/kilosort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-13 21:11:45.000000 kilosort-4.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:11:55.791759 kilosort-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-13 21:11:45.000000 kilosort-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.787758 kilosort-4.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_full_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-13 21:11:45.000000 kilosort-4.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.359928 kilosort-4.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.343928 kilosort-4.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/installation_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/ISSUE_TEMPLATE/other.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-19 18:44:55.000000 kilosort-4.0.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-19 18:44:55.000000 kilosort-4.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-19 18:44:55.000000 kilosort-4.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-19 18:44:55.000000 kilosort-4.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 18:44:55.000000 kilosort-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-19 18:45:04.359928 kilosort-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-19 18:44:55.000000 kilosort-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/drift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/gui_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/hardware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/multi_shank.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.347928 kilosort-4.0.5/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/basic_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/load_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/make_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 18:44:55.000000 kilosort-4.0.5/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.351928 kilosort-4.0.5/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/CCG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/clustering_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/datashift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.355928 kilosort-4.0.5/kilosort/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/data_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/header_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/message_log_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/minor_gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/probe_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/run_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/sanity_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/settings_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/gui/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36575 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/run_kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/swarmsplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/template_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-19 18:44:55.000000 kilosort-4.0.5/kilosort/wTEMP.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.359928 kilosort-4.0.5/kilosort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 18:45:04.000000 kilosort-4.0.5/kilosort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 18:44:55.000000 kilosort-4.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:45:04.359928 kilosort-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-19 18:44:55.000000 kilosort-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:45:04.359928 kilosort-4.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_full_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-19 18:44:55.000000 kilosort-4.0.5/tests/test_spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 18:44:55.000000 kilosort-4.0.5/tox.ini
```

### Comparing `kilosort-4.0.4/.github/ISSUE_TEMPLATE/bug_report.yml` & `kilosort-4.0.5/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/.github/ISSUE_TEMPLATE/feature_request.yml` & `kilosort-4.0.5/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/.github/ISSUE_TEMPLATE/installation_issue.yml` & `kilosort-4.0.5/.github/ISSUE_TEMPLATE/installation_issue.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/.github/workflows/test_and_deploy.yml` & `kilosort-4.0.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/.gitignore` & `kilosort-4.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/.readthedocs.yml` & `kilosort-4.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/CODE_OF_CONDUCT.md` & `kilosort-4.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/LICENSE` & `kilosort-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/PKG-INFO` & `kilosort-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.4
+Version: 4.0.5
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kilosort-4.0.4/README.md` & `kilosort-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/Makefile` & `kilosort-4.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/conf.py` & `kilosort-4.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/drift.rst` & `kilosort-4.0.5/docs/drift.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/gui_guide.rst` & `kilosort-4.0.5/docs/gui_guide.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/hardware.rst` & `kilosort-4.0.5/docs/hardware.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/index.rst` & `kilosort-4.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/make.bat` & `kilosort-4.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/multi_shank.rst` & `kilosort-4.0.5/docs/multi_shank.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/parameters.rst` & `kilosort-4.0.5/docs/parameters.rst`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 ``x_centers``
 -------------
 The number of x-positions to use when determining centers for template groupings. Specifically, this is the number of centroids to look for when using k-means to cluster the x-positions for the probe. In most cases you should not need to specify this. However, **for probes with contacts arranged in a 2D grid**, we recommend setting ``x_centers`` such that centers are placed every 200-300um so that there are not too many templates in each group. For example, for an array that is 2000um in width, try ``x_centers = 10``. If contacts are very densely spaced, you may need to use a higher value for better performance.
 
 
 ``duplicate_spike_bins``
 ------------------------
-After sorting has finished, spikes that occur within this number of bins of each other, from the same unit, are assumed to be artifacts and removed. The default of 15 bins corresponds to 0.5ms for a sampling rate of 30000hz. If your sampling rate is different, you may need to increase or decrease this accordingly. If you see otherwise good neurons with large peaks around 0ms when viewing correlograms in Phy, increasing this value can help remove those artifacts.
+After sorting has finished, spikes that occur within this number of bins of each other, from the same unit, are assumed to be artifacts and removed. The default of 7 bins corresponds to approximately 0.25ms for a sampling rate of 30000hz. If your sampling rate is different, you may need to increase or decrease this accordingly. If you see otherwise good neurons with large peaks around 0ms when viewing correlograms in Phy, increasing this value can help remove those artifacts.
 
 **Warning!!!** Do not increase this value beyond 0.5ms as it will interfere with the ACG and CCG refractory period estimations (which normally ignores the central 1ms of the correlogram).
```

### Comparing `kilosort-4.0.4/docs/tutorials/basic_example.ipynb` & `kilosort-4.0.5/docs/tutorials/basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/tutorials/load_data.ipynb` & `kilosort-4.0.5/docs/tutorials/load_data.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/docs/tutorials/make_probe.ipynb` & `kilosort-4.0.5/docs/tutorials/make_probe.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/CCG.py` & `kilosort-4.0.5/kilosort/CCG.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/bench.py` & `kilosort-4.0.5/kilosort/bench.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/clustering_qr.py` & `kilosort-4.0.5/kilosort/clustering_qr.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,35 +236,41 @@
     if k is not None:
         # Use this as the input for k-means, either a number of centers
         # or initial guesses.
         approx_centers = k
     else:
         # NOTE: This automated method does not work well for 2D array probes.
         #       We recommend specifying `x_centers` manually for that case.
-        dminx = ops['dminx']
+
+        # Originally bin_width was set equal to `dminx`, but decided it's better
+        # to not couple this behavior with that setting. A bin size of 50 microns
+        # seems to work well for NP1 and 2, tetrodes, and 2D arrays. We can make
+        # this a parameter later on if it becomes a problem.
+        bin_width = 50
         min_x = ops['xc'].min()
         max_x = ops['xc'].max()
 
         # Make histogram of x-positions with bin size roughly equal to dminx,
         # with a bit of padding on either end of the probe so that peaks can be
         # detected at edges.
-        num_bins = int((max_x-min_x)/(dminx)) + 4
-        bins = np.linspace(min_x - dminx*2, max_x + dminx*2, num_bins)
+        num_bins = int((max_x-min_x)/(bin_width)) + 4
+        bins = np.linspace(min_x - bin_width*2, max_x + bin_width*2, num_bins)
         hist, edges = np.histogram(ops['xc'], bins=bins)
         # Apply smoothing to make peak-finding simpler.
         smoothed = gaussian_filter(hist, sigma=0.5)
         peaks, _ = find_peaks(smoothed)
         # peaks are indices, translate back to position in microns
         approx_centers = [edges[p] for p in peaks]
+
         # Use these as initial guesses for centroids in k-means to get
         # a more accurate value for the actual centers. Or, if there's only 1,
         # just look for one centroid.
         if len(approx_centers) == 1: approx_centers = 1
 
-    centers, distortion = kmeans(ops['xc'], approx_centers)
+    centers, distortion = kmeans(ops['xc'], approx_centers, seed=5330)
 
     # TODO: Maybe use distortion to raise warning if it seems too large?
     # "The mean (non-squared) Euclidean distance between the observations passed
     #  and the centroids generated. Note the difference to the standard definition
     #  of distortion in the context of the k-means algorithm, which is the sum of
     #  the squared distances."
```

### Comparing `kilosort-4.0.4/kilosort/datashift.py` & `kilosort-4.0.5/kilosort/datashift.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/__init__.py` & `kilosort-4.0.5/kilosort/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/converter.py` & `kilosort-4.0.5/kilosort/gui/converter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/data_view_box.py` & `kilosort-4.0.5/kilosort/gui/data_view_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/header_box.py` & `kilosort-4.0.5/kilosort/gui/header_box.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import webbrowser
+
 from kilosort import __version__
 from kilosort.gui.minor_gui_elements import help_popup_text, controls_popup_text
 from qtpy import QtCore, QtGui, QtWidgets
 
 
 class HeaderBox(QtWidgets.QWidget):
     def __init__(self, parent):
@@ -28,19 +30,19 @@
             self.show_plots_check.setCheckState(QtCore.Qt.CheckState.Unchecked)
         self.show_plots_check.clicked.connect(self.check_show_plots)
 
         # TODO: connect the button clicks to open something in browser instead?
         #       like the paper and/or wiki.
         self.controls_button = QtWidgets.QPushButton("Controls")
         self.controls_button.setToolTip(controls_popup_text)
-        #self.controls_button.clicked.connect(self.show_controls_popup)
+        self.controls_button.clicked.connect(self.open_controls_link)
 
         self.help_button = QtWidgets.QPushButton("Help")
         self.help_button.setToolTip(help_popup_text)
-        #self.help_button.clicked.connect(self.show_help_popup)
+        self.help_button.clicked.connect(self.open_help_link)
 
         self.reset_gui_button = QtWidgets.QPushButton("Reset GUI")
         
         self.clear_cache_button = QtWidgets.QPushButton("Clear Cache")
         self.clear_cache_button.clicked.connect(self.clear_cache)
 
         # self.layout.addWidget(self.kilosort_text)
@@ -64,8 +66,16 @@
     def check_show_plots(self):
         self.gui.show_plots = self.show_plots_check.isChecked()
         self.gui.qt_settings.setValue('show_plots', self.gui.show_plots)
 
     @QtCore.Slot()
     def clear_cache(self):
         self.gui.qt_settings.clear()
-        
+        
+    @QtCore.Slot()
+    def open_controls_link(self):
+        webbrowser.open('https://kilosort.readthedocs.io/en/latest/gui_guide.html')
+        
+
+    @QtCore.Slot()
+    def open_help_link(self):
+        webbrowser.open('https://github.com/MouseLand/Kilosort/issues')
```

### Comparing `kilosort-4.0.4/kilosort/gui/launch.py` & `kilosort-4.0.5/kilosort/gui/launch.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/logger.py` & `kilosort-4.0.5/kilosort/gui/logger.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/main.py` & `kilosort-4.0.5/kilosort/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,14 +327,20 @@
         yc = self.probe_layout["yc"]
         nskip = self.params["nskip"]
         data_dtype = self.params["data_dtype"]
         tmin = self.params['tmin']
         tmax = self.params['tmax']
         artifact = self.params['artifact_threshold']
 
+        if chan_map.max() >= n_channels:
+            raise ValueError(
+                f'Largest value of chanMap exceeds channel count of data, '
+                'make sure chanMap is 0-indexed.'
+            )
+
         binary_file = BinaryFiltered(
             filename=self.data_path,
             n_chan_bin=n_channels,
             fs=sample_rate,
             chan_map=chan_map,
             device=self.device,
             dtype=data_dtype,
```

### Comparing `kilosort-4.0.4/kilosort/gui/message_log_box.py` & `kilosort-4.0.5/kilosort/gui/message_log_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/minor_gui_elements.py` & `kilosort-4.0.5/kilosort/gui/minor_gui_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         buttons = [self.check_button, self.okay_button, self.cancel_button]
 
         error_label_size_policy = self.error_label.sizePolicy()
         error_label_size_policy.setVerticalPolicy(QtWidgets.QSizePolicy.Maximum)
         error_label_size_policy.setRetainSizeWhenHidden(True)
         self.error_label.setSizePolicy(error_label_size_policy)
         error_label_palette = self.error_label.palette()
-        error_label_palette.setColor(QtGui.QPalette.Foreground, QtGui.QColor("red"))
+        error_label_palette.setColor(QtGui.QPalette.WindowText, QtGui.QColor("red"))
         self.error_label.setPalette(error_label_palette)
         self.error_label.hide()
 
         for field in self.input_list:
             field.textChanged.connect(self.set_values_as_unchecked)
 
         widget_list = [
@@ -244,13 +244,13 @@
 """
 
 help_popup_text = """
 Welcome to Kilosort4!
 
 ##### Documentation #####
 For documentation of the underlying algorithm or the GUI, please visit https://github.com/MouseLand/Kilosort/
-or https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1.
+or read the paper at https://www.nature.com/articles/s41592-024-02232-7.
 
 ##### Troubleshooting #####
 1. Click 'Reset GUI' to clear any GUI problems or strange errors. If the problem persists, try 'Clear Cache' and restarting Kilosort. 
-2. If the problem persists, visit https://github.com/MouseLand/kilosort and create an issue there with as much detail about the problem as possible.  
+2. If the problem persists, visit https://github.com/MouseLand/Kilosort/issues/ and ask for assistance there with as much detail about the problem as possible.  
 """
```

### Comparing `kilosort-4.0.4/kilosort/gui/palettes.py` & `kilosort-4.0.5/kilosort/gui/palettes.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/probe_view_box.py` & `kilosort-4.0.5/kilosort/gui/probe_view_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
         self.active_layout = None
         self.kcoords = None
         self.xc = None
         self.yc = None
         self.xcup = None
         self.ycup = None
+        self.xcent_pos = None
+        self.ycent_pos = None
         self.total_channels = None
         self.channel_map = None
         self.channel_map_dict = {}
         self.channel_spots = None
         self.template_spots = None
         self.center_spots = None
 
@@ -76,16 +78,17 @@
         self.set_active_layout(probe, template_args)
         self.update_probe_view()
 
     def set_active_layout(self, probe, template_args):
         self.active_layout = probe
         self.kcoords = self.active_layout["kcoords"]
         self.xc, self.yc = self.active_layout["xc"], self.active_layout["yc"]
-        self.xcup, self.ycup, self.ops = self.get_template_spots(*template_args)
-        self.xcent_pos, self.ycent_pos = self.get_center_spots()
+        if self.template_toggle.isChecked() or self.center_toggle.isChecked():
+            self.xcup, self.ycup, self.ops = self.get_template_spots(*template_args)
+            self.xcent_pos, self.ycent_pos = self.get_center_spots()
         self.channel_map_dict = {}
         for ind, (xc, yc) in enumerate(zip(self.xc, self.yc)):
             self.channel_map_dict[(xc, yc)] = ind
         self.total_channels = self.active_layout["n_chan"]
         self.channel_map = self.active_layout["chanMap"]
 
     def get_template_spots(self, nC, dmin, dminx, max_dist, x_centers, device):
```

### Comparing `kilosort-4.0.4/kilosort/gui/run_box.py` & `kilosort-4.0.5/kilosort/gui/run_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/sanity_plots.py` & `kilosort-4.0.5/kilosort/gui/sanity_plots.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/settings_box.py` & `kilosort-4.0.5/kilosort/gui/settings_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/gui/sorter.py` & `kilosort-4.0.5/kilosort/gui/sorter.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,19 +85,19 @@
             self.Wall0 = Wall0
             self.wPCA = torch.clone(ops['wPCA'].cpu()).numpy()
             self.clu0 = clu0
             self.plotDataReady.emit('diagnostics')
 
             clu, Wall = cluster_spikes(st, tF, ops, self.device, bfile, tic0=tic0,
                                        progress_bar=self.progress_bar)
-            ops, similar_templates, is_ref, est_contam_rate = \
+            ops, similar_templates, is_ref, est_contam_rate, kept_spikes = \
                 save_sorting(ops, results_dir, st, clu, tF, Wall, bfile.imin, tic0)
 
             self.ops = ops
-            self.st = st
-            self.clu = clu
-            self.tF = tF
+            self.st = st[kept_spikes]
+            self.clu = clu[kept_spikes]
+            self.tF = tF[kept_spikes]
             self.is_refractory = is_ref
             self.plotDataReady.emit('probe')
 
             logger.info(f"Spike sorting output saved in\n{results_dir}")
             self.finishedSpikesort.emit(self.context)
```

### Comparing `kilosort-4.0.4/kilosort/hierarchical.py` & `kilosort-4.0.5/kilosort/hierarchical.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/io.py` & `kilosort-4.0.5/kilosort/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
     # Remove cached .phy results if present from running Phy on a previous
     # version of results in the same directory.
     phy_cache_path = Path(results_dir / '.phy')
     if phy_cache_path.is_dir():
         shutil.rmtree(phy_cache_path)
 
-    return results_dir, similar_templates, is_ref, est_contam_rate
+    return results_dir, similar_templates, is_ref, est_contam_rate, kept_spikes
 
 
 def save_ops(ops, results_dir=None):
     """Save intermediate `ops` dictionary to `results_dir/ops.npy`."""
 
     if results_dir is None:
         results_dir = Path(ops['data_dir']) / 'kilosort4'
```

### Comparing `kilosort-4.0.4/kilosort/parameters.py` & `kilosort-4.0.5/kilosort/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,15 @@
             """
     },
 
 
     ### POSTPROCESSING
     'duplicate_spike_bins': {
         'gui_name': 'duplicate spike bins', 'type': int, 'min': 0, 'max': np.inf,
-        'exclude': [], 'default': 15, 'step': 'postprocessing',
+        'exclude': [], 'default': 7, 'step': 'postprocessing',
         'description':
             """
             Number of bins for which subsequent spikes from the same cluster are
             assumed to be artifacts. A value of 0 disables this step.
             """
     },
 }
```

### Comparing `kilosort-4.0.4/kilosort/postprocessing.py` & `kilosort-4.0.5/kilosort/postprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/preprocessing.py` & `kilosort-4.0.5/kilosort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/run_kilosort.py` & `kilosort-4.0.5/kilosort/run_kilosort.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,20 @@
             device = torch.device('cpu')
 
     # NOTE: Also modifies settings in-place
     filename, data_dir, results_dir, probe = \
         set_files(settings, filename, probe, probe_name, data_dir, results_dir)
     ops = initialize_ops(settings, probe, data_dtype, do_CAR, invert_sign, device)
 
+    if probe['chanMap'].max() >= settings['n_chan_bin']:
+        raise ValueError(
+            f'Largest value of chanMap exceeds channel count of data, '
+             'make sure chanMap is 0-indexed.'
+        )
+
     # Set preprocessing and drift correction parameters
     ops = compute_preprocessing(ops, device, tic0=tic0, file_object=file_object)
     np.random.seed(1)
     torch.cuda.manual_seed_all(1)
     torch.random.manual_seed(1)
     ops, bfile, st0 = compute_drift_correction(
         ops, device, tic0=tic0, progress_bar=progress_bar,
@@ -138,19 +144,20 @@
     io.save_ops(ops, results_dir)
 
     # Sort spikes and save results
     st, tF, _, _ = detect_spikes(ops, device, bfile, tic0=tic0,
                                  progress_bar=progress_bar)
     clu, Wall = cluster_spikes(st, tF, ops, device, bfile, tic0=tic0,
                                progress_bar=progress_bar)
-    ops, similar_templates, is_ref, est_contam_rate = \
+    ops, similar_templates, is_ref, est_contam_rate, kept_spikes = \
         save_sorting(ops, results_dir, st, clu, tF, Wall, bfile.imin, tic0,
                      save_extra_vars=save_extra_vars)
 
-    return ops, st, clu, tF, Wall, similar_templates, is_ref, est_contam_rate
+    return ops, st, clu, tF, Wall, similar_templates, \
+           is_ref, est_contam_rate, kept_spikes
 
 
 def set_files(settings, filename, probe, probe_name, data_dir, results_dir):
     """Parse file and directory information for data, probe, and results."""
 
     # Check for filename 
     filename = settings.get('filename', None) if filename is None else filename 
@@ -465,15 +472,16 @@
     similar_templates : np.ndarray
     is_ref : np.ndarray
     est_contam_rate : np.ndarray
     
     """
 
     print('\nSaving to phy and computing refractory periods')
-    results_dir, similar_templates, is_ref, est_contam_rate = io.save_to_phy(
+    results_dir, similar_templates, is_ref, est_contam_rate, kept_spikes = \
+        io.save_to_phy(
             st, clu, tF, Wall, ops['probe'], ops, imin, results_dir=results_dir,
             data_dtype=ops['data_dtype'], save_extra_vars=save_extra_vars
             )
     print(f'{int(is_ref.sum())} units found with good refractory periods')
     
     runtime = time.time()-tic0
     seconds = runtime % 60
@@ -482,15 +490,15 @@
     mins = mins % 60
     print(f'\nTotal runtime: {runtime:.2f}s = {int(hrs):02d}:' +
           f'{int(mins):02d}:{round(seconds)} h:m:s')
     ops['runtime'] = runtime 
 
     io.save_ops(ops, results_dir)
 
-    return ops, similar_templates, is_ref, est_contam_rate
+    return ops, similar_templates, is_ref, est_contam_rate, kept_spikes
 
 
 def load_sorting(results_dir, device=None, load_extra_vars=False):
     if device is None:
         if torch.cuda.is_available():
             device = torch.device('cuda')
         else:
```

### Comparing `kilosort-4.0.4/kilosort/simulation.py` & `kilosort-4.0.5/kilosort/simulation.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/spikedetect.py` & `kilosort-4.0.5/kilosort/spikedetect.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/swarmsplitter.py` & `kilosort-4.0.5/kilosort/swarmsplitter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/template_matching.py` & `kilosort-4.0.5/kilosort/template_matching.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/utils.py` & `kilosort-4.0.5/kilosort/utils.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort/wTEMP.npz` & `kilosort-4.0.5/kilosort/wTEMP.npz`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/kilosort.egg-info/PKG-INFO` & `kilosort-4.0.5/kilosort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.4
+Version: 4.0.5
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kilosort-4.0.4/kilosort.egg-info/SOURCES.txt` & `kilosort-4.0.5/kilosort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/setup.py` & `kilosort-4.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/tests/conftest.py` & `kilosort-4.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/tests/test_clustering.py` & `kilosort-4.0.5/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/tests/test_dtype.py` & `kilosort-4.0.5/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/tests/test_full_pipeline.py` & `kilosort-4.0.5/tests/test_full_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
 # Use `pytest --runslow` option to include this in tests.
 @pytest.mark.slow
 def test_pipeline(data_directory, results_directory, saved_ops, torch_device, capture_mgr):
     bin_file = data_directory / 'ZFM-02370_mini.imec0.ap.short.bin'
     with pytest.raises(ValueError):
         # Should result in an error, since `n_chan_bin` isn't specified.
-        ops, st, clu, _, _, _, _, _ = run_kilosort(
+        ops, st, clu, _, _, _, _, _, kept_spikes = run_kilosort(
             settings={}, filename=bin_file, device=torch_device,
             probe_name='neuropixPhase3B1_kilosortChanMap.mat',
             )
 
     with capture_mgr.global_and_fixture_disabled():
         print('\nStarting run_kilosort test...')
-        ops, st, clu, _, _, _, _, _ = run_kilosort(
+        ops, st, clu, _, _, _, _, _, kept_spikes = run_kilosort(
             filename=bin_file, device=torch_device,
             settings={'n_chan_bin': 385},
             probe_name='neuropixPhase3B1_kilosortChanMap.mat',
             )
 
-    st = st[:,0]  # only first column is spike times, that's all that gets saved
+    st = st[kept_spikes,0]  # only first column is spike times
+    clu = clu[kept_spikes]
         
     # Check that spike times and spike cluster assignments match
     st_load = np.load(results_directory / 'spike_times.npy')
     clu_load = np.load(results_directory / 'spike_clusters.npy')
     saved_yblk = saved_ops['yblk']
     saved_dshift = saved_ops['dshift']
     saved_iKxx = saved_ops['iKxx']
```

### Comparing `kilosort-4.0.4/tests/test_io.py` & `kilosort-4.0.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/tests/test_parameters.py` & `kilosort-4.0.5/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/tests/test_preprocessing.py` & `kilosort-4.0.5/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.4/tox.ini` & `kilosort-4.0.5/tox.ini`

 * *Files identical despite different names*

