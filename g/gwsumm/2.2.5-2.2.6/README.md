# Comparing `tmp/gwsumm-2.2.5.tar.gz` & `tmp/gwsumm-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwsumm-2.2.5.tar", last modified: Thu Apr 18 16:16:55 2024, max compression
+gzip compressed data, was "gwsumm-2.2.6.tar", last modified: Fri Apr 19 17:50:55 2024, max compression
```

## Comparing `gwsumm-2.2.5.tar` & `gwsumm-2.2.6.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.799503 gwsumm-2.2.5/
--rw-r--r--   0 egoetz     (501) staff       (20)      319 2023-11-01 22:18:02.000000 gwsumm-2.2.5/.codeclimate.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      184 2020-04-07 19:56:04.000000 gwsumm-2.2.5/.codecov.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      126 2023-11-01 22:18:02.000000 gwsumm-2.2.5/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)       32 2020-04-07 19:56:04.000000 gwsumm-2.2.5/.gitattributes
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.699010 gwsumm-2.2.5/.github/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.711514 gwsumm-2.2.5/.github/workflows/
--rw-r--r--   0 egoetz     (501) staff       (20)     3579 2024-03-26 21:53:27.000000 gwsumm-2.2.5/.github/workflows/build.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      765 2024-03-26 21:53:27.000000 gwsumm-2.2.5/.github/workflows/lint.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      259 2023-11-01 22:18:02.000000 gwsumm-2.2.5/.gitignore
--rw-r--r--   0 egoetz     (501) staff       (20)      645 2024-03-25 16:15:43.000000 gwsumm-2.2.5/.readthedocs.yaml
--rw-r--r--   0 egoetz     (501) staff       (20)     2667 2021-03-09 19:10:52.000000 gwsumm-2.2.5/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2020-04-07 19:56:04.000000 gwsumm-2.2.5/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       94 2023-11-01 22:18:02.000000 gwsumm-2.2.5/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-18 16:16:55.798589 gwsumm-2.2.5/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2358 2022-01-25 22:56:26.000000 gwsumm-2.2.5/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.720148 gwsumm-2.2.5/docs/
--rw-r--r--   0 egoetz     (501) staff       (20)     6810 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/Makefile
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.699534 gwsumm-2.2.5/docs/_static/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.720975 gwsumm-2.2.5/docs/_static/css/
--rw-r--r--   0 egoetz     (501) staff       (20)     4997 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_static/css/custom.css
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.721783 gwsumm-2.2.5/docs/_templates/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.722880 gwsumm-2.2.5/docs/_templates/autoclass/
--rw-r--r--   0 egoetz     (501) staff       (20)      928 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autoclass/class.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.725624 gwsumm-2.2.5/docs/_templates/autosummary/
--rw-r--r--   0 egoetz     (501) staff       (20)      170 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autosummary/base.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1167 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      703 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      303 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/_templates/layout.html
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.726865 gwsumm-2.2.5/docs/api/
--rw-r--r--   0 egoetz     (501) staff       (20)       64 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/api/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      537 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/automation.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1427 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/cli.rst
--rw-r--r--   0 egoetz     (501) staff       (20)    10467 2023-11-01 22:18:02.000000 gwsumm-2.2.5/docs/conf.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.729685 gwsumm-2.2.5/docs/configuration/
--rw-r--r--   0 egoetz     (501) staff       (20)    12488 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/data.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1887 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/format.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      908 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     3433 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/configuration/tabs.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      555 2024-03-25 16:02:23.000000 gwsumm-2.2.5/docs/environment.yml
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.731211 gwsumm-2.2.5/docs/examples/
--rw-r--r--   0 egoetz     (501) staff       (20)    22257 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/examples/first.png
--rw-r--r--   0 egoetz     (501) staff       (20)    95352 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/examples/imc.png
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.732590 gwsumm-2.2.5/docs/images/
--rw-r--r--   0 egoetz     (501) staff       (20)   710629 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/images/screenshot.png
--rw-r--r--   0 egoetz     (501) staff       (20)     2948 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     6701 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/make.bat
--rw-r--r--   0 egoetz     (501) staff       (20)       28 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/modes.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2864 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/overview.rst
--rw-r--r--   0 egoetz     (501) staff       (20)       79 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/plots.rst
--rw-r--r--   0 egoetz     (501) staff       (20)      100 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/states.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.738832 gwsumm-2.2.5/docs/tabs/
--rw-r--r--   0 egoetz     (501) staff       (20)       53 2020-04-07 19:56:04.000000 gwsumm-2.2.5/docs/tabs/api.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     1458 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/tabs/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2368 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/tabs/modes.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2202 2023-11-01 16:21:08.000000 gwsumm-2.2.5/docs/tabs/websites.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.747158 gwsumm-2.2.5/gwsumm/
--rw-r--r--   0 egoetz     (501) staff       (20)     1326 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    28701 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16826 2024-04-17 23:14:02.000000 gwsumm-2.2.5/gwsumm/archive.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20413 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12777 2024-04-17 23:14:02.000000 gwsumm-2.2.5/gwsumm/channels.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.750606 gwsumm-2.2.5/gwsumm/config/
--rw-r--r--   0 egoetz     (501) staff       (20)    14290 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/config/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3229 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/config/defaults.ini
--rw-r--r--   0 egoetz     (501) staff       (20)      423 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/config/matplotlib.ini
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.756105 gwsumm-2.2.5/gwsumm/data/
--rw-r--r--   0 egoetz     (501) staff       (20)     2098 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/data/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20054 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/data/coherence.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8781 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/data/mathutils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7322 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/data/range.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16530 2024-04-05 20:16:32.000000 gwsumm-2.2.5/gwsumm/data/spectral.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32307 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/data/timeseries.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5424 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/data/utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1263 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/globalv.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.758475 gwsumm-2.2.5/gwsumm/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1268 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/html/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6402 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/html/bootstrap.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8700 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/html/html5.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2591 2024-04-18 16:13:50.000000 gwsumm-2.2.5/gwsumm/html/static.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.760724 gwsumm-2.2.5/gwsumm/html/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      798 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/html/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4297 2024-04-04 18:06:28.000000 gwsumm-2.2.5/gwsumm/html/tests/test_bootstrap.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6577 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/html/tests/test_html5.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1940 2024-03-26 21:53:27.000000 gwsumm-2.2.5/gwsumm/html/tests/test_static.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2116 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/io.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3832 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/mode.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.768868 gwsumm-2.2.5/gwsumm/plot/
--rw-r--r--   0 egoetz     (501) staff       (20)     2834 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/plot/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    37328 2024-04-05 20:16:32.000000 gwsumm-2.2.5/gwsumm/plot/builtin.py
--rw-r--r--   0 egoetz     (501) staff       (20)    27119 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/plot/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.770800 gwsumm-2.2.5/gwsumm/plot/guardian/
--rw-r--r--   0 egoetz     (501) staff       (20)      911 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6353 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7919 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.772053 gwsumm-2.2.5/gwsumm/plot/guardian/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2903 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/guardian/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8243 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/plot/mixins.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8000 2023-11-02 17:15:14.000000 gwsumm-2.2.5/gwsumm/plot/noisebudget.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14079 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/plot/range.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2023 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/plot/registry.py
--rw-r--r--   0 egoetz     (501) staff       (20)    58958 2024-03-19 23:14:10.000000 gwsumm-2.2.5/gwsumm/plot/segments.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6023 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/plot/sei.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.774206 gwsumm-2.2.5/gwsumm/plot/triggers/
--rw-r--r--   0 egoetz     (501) staff       (20)     1014 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/triggers/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9012 2022-12-20 19:28:31.000000 gwsumm-2.2.5/gwsumm/plot/triggers/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    21921 2023-11-02 17:15:14.000000 gwsumm-2.2.5/gwsumm/plot/triggers/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.775874 gwsumm-2.2.5/gwsumm/plot/triggers/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/triggers/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3902 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/plot/triggers/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4987 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/plot/utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12722 2024-01-25 21:39:34.000000 gwsumm-2.2.5/gwsumm/segments.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.778413 gwsumm-2.2.5/gwsumm/state/
--rw-r--r--   0 egoetz     (501) staff       (20)     2023 2023-05-22 17:31:39.000000 gwsumm-2.2.5/gwsumm/state/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2034 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/state/all.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12603 2023-11-01 16:21:08.000000 gwsumm-2.2.5/gwsumm/state/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3034 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/state/registry.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.788515 gwsumm-2.2.5/gwsumm/tabs/
--rw-r--r--   0 egoetz     (501) staff       (20)     1506 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    29472 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/builtin.py
--rw-r--r--   0 egoetz     (501) staff       (20)    36826 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/tabs/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    39853 2024-03-26 21:53:27.000000 gwsumm-2.2.5/gwsumm/tabs/data.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15759 2024-01-31 17:20:38.000000 gwsumm-2.2.5/gwsumm/tabs/etg.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10248 2022-01-25 22:56:26.000000 gwsumm-2.2.5/gwsumm/tabs/fscan.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10332 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tabs/gracedb.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14124 2024-03-26 21:53:27.000000 gwsumm-2.2.5/gwsumm/tabs/guardian.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9258 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/management.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3611 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tabs/misc.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2107 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/registry.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16837 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tabs/sei.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4984 2022-09-15 15:47:20.000000 gwsumm-2.2.5/gwsumm/tabs/stamp.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.795407 gwsumm-2.2.5/gwsumm/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      790 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1170 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/common.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4780 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_archive.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4855 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4208 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_channels.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8768 2023-11-01 22:18:02.000000 gwsumm-2.2.5/gwsumm/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8903 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_data.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1803 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_mode.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10913 2024-02-09 21:54:30.000000 gwsumm-2.2.5/gwsumm/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4393 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_tabs.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3782 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16412 2024-03-19 23:14:10.000000 gwsumm-2.2.5/gwsumm/triggers.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1032 2020-04-07 19:56:04.000000 gwsumm-2.2.5/gwsumm/units.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6446 2021-03-09 19:10:52.000000 gwsumm-2.2.5/gwsumm/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-18 16:16:55.796074 gwsumm-2.2.5/gwsumm.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2986 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      204 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      410 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        7 2024-04-18 16:16:55.000000 gwsumm-2.2.5/gwsumm.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     2891 2024-04-18 16:13:50.000000 gwsumm-2.2.5/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-18 16:16:55.799671 gwsumm-2.2.5/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.584441 gwsumm-2.2.6/
+-rw-r--r--   0 egoetz     (501) staff       (20)      319 2023-11-01 22:18:02.000000 gwsumm-2.2.6/.codeclimate.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2020-04-07 19:56:04.000000 gwsumm-2.2.6/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      126 2023-11-01 22:18:02.000000 gwsumm-2.2.6/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       32 2020-04-07 19:56:04.000000 gwsumm-2.2.6/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.474945 gwsumm-2.2.6/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.488413 gwsumm-2.2.6/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3579 2024-03-26 21:53:27.000000 gwsumm-2.2.6/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      765 2024-03-26 21:53:27.000000 gwsumm-2.2.6/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      259 2023-11-01 22:18:02.000000 gwsumm-2.2.6/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      645 2024-03-25 16:15:43.000000 gwsumm-2.2.6/.readthedocs.yaml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2667 2021-03-09 19:10:52.000000 gwsumm-2.2.6/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2020-04-07 19:56:04.000000 gwsumm-2.2.6/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       94 2023-11-01 22:18:02.000000 gwsumm-2.2.6/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-19 17:50:55.583681 gwsumm-2.2.6/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2358 2022-01-25 22:56:26.000000 gwsumm-2.2.6/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.497569 gwsumm-2.2.6/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6810 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.475383 gwsumm-2.2.6/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.498164 gwsumm-2.2.6/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.498663 gwsumm-2.2.6/docs/_templates/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.499194 gwsumm-2.2.6/docs/_templates/autoclass/
+-rw-r--r--   0 egoetz     (501) staff       (20)      928 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/_templates/autoclass/class.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.501103 gwsumm-2.2.6/docs/_templates/autosummary/
+-rw-r--r--   0 egoetz     (501) staff       (20)      170 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1167 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      703 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      303 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/_templates/layout.html
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.501800 gwsumm-2.2.6/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       64 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      537 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/automation.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1427 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/cli.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10467 2023-11-01 22:18:02.000000 gwsumm-2.2.6/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.505105 gwsumm-2.2.6/docs/configuration/
+-rw-r--r--   0 egoetz     (501) staff       (20)    12488 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/configuration/data.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1887 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/configuration/format.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      908 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/configuration/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     3433 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/configuration/tabs.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      555 2024-03-25 16:02:23.000000 gwsumm-2.2.6/docs/environment.yml
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.507331 gwsumm-2.2.6/docs/examples/
+-rw-r--r--   0 egoetz     (501) staff       (20)    22257 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/examples/first.png
+-rw-r--r--   0 egoetz     (501) staff       (20)    95352 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/examples/imc.png
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.509072 gwsumm-2.2.6/docs/images/
+-rw-r--r--   0 egoetz     (501) staff       (20)   710629 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/images/screenshot.png
+-rw-r--r--   0 egoetz     (501) staff       (20)     2948 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     6701 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/make.bat
+-rw-r--r--   0 egoetz     (501) staff       (20)       28 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/modes.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2864 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/overview.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)       79 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/plots.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)      100 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/states.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.515696 gwsumm-2.2.6/docs/tabs/
+-rw-r--r--   0 egoetz     (501) staff       (20)       53 2020-04-07 19:56:04.000000 gwsumm-2.2.6/docs/tabs/api.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     1458 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/tabs/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2368 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/tabs/modes.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2202 2023-11-01 16:21:08.000000 gwsumm-2.2.6/docs/tabs/websites.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.528481 gwsumm-2.2.6/gwsumm/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1326 2023-11-01 22:18:02.000000 gwsumm-2.2.6/gwsumm/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    28701 2023-11-01 16:21:08.000000 gwsumm-2.2.6/gwsumm/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-19 17:50:55.000000 gwsumm-2.2.6/gwsumm/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16826 2024-04-17 23:14:02.000000 gwsumm-2.2.6/gwsumm/archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20413 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12777 2024-04-17 23:14:02.000000 gwsumm-2.2.6/gwsumm/channels.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.533975 gwsumm-2.2.6/gwsumm/config/
+-rw-r--r--   0 egoetz     (501) staff       (20)    14290 2023-11-01 22:18:02.000000 gwsumm-2.2.6/gwsumm/config/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3229 2023-11-01 22:18:02.000000 gwsumm-2.2.6/gwsumm/config/defaults.ini
+-rw-r--r--   0 egoetz     (501) staff       (20)      423 2023-11-01 22:18:02.000000 gwsumm-2.2.6/gwsumm/config/matplotlib.ini
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.540670 gwsumm-2.2.6/gwsumm/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2098 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/data/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20054 2024-04-18 16:13:50.000000 gwsumm-2.2.6/gwsumm/data/coherence.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8781 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/data/mathutils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7322 2024-04-18 16:13:50.000000 gwsumm-2.2.6/gwsumm/data/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16530 2024-04-05 20:16:32.000000 gwsumm-2.2.6/gwsumm/data/spectral.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32307 2023-11-01 16:21:08.000000 gwsumm-2.2.6/gwsumm/data/timeseries.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5424 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/data/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1263 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/globalv.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.543507 gwsumm-2.2.6/gwsumm/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1268 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/html/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6402 2024-04-18 16:13:50.000000 gwsumm-2.2.6/gwsumm/html/bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8700 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/html/html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2591 2024-04-19 17:49:54.000000 gwsumm-2.2.6/gwsumm/html/static.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.546216 gwsumm-2.2.6/gwsumm/html/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      798 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/html/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4297 2024-04-04 18:06:28.000000 gwsumm-2.2.6/gwsumm/html/tests/test_bootstrap.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6577 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/html/tests/test_html5.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1940 2024-03-26 21:53:27.000000 gwsumm-2.2.6/gwsumm/html/tests/test_static.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2116 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/io.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3832 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/mode.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.554813 gwsumm-2.2.6/gwsumm/plot/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2834 2024-02-09 21:54:30.000000 gwsumm-2.2.6/gwsumm/plot/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    37328 2024-04-05 20:16:32.000000 gwsumm-2.2.6/gwsumm/plot/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    27119 2024-02-09 21:54:30.000000 gwsumm-2.2.6/gwsumm/plot/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.556601 gwsumm-2.2.6/gwsumm/plot/guardian/
+-rw-r--r--   0 egoetz     (501) staff       (20)      911 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/guardian/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6353 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/guardian/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7919 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/guardian/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.557735 gwsumm-2.2.6/gwsumm/plot/guardian/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/guardian/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2903 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/guardian/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8243 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/plot/mixins.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8000 2023-11-02 17:15:14.000000 gwsumm-2.2.6/gwsumm/plot/noisebudget.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14079 2024-02-09 21:54:30.000000 gwsumm-2.2.6/gwsumm/plot/range.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/plot/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    58958 2024-03-19 23:14:10.000000 gwsumm-2.2.6/gwsumm/plot/segments.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6023 2023-11-01 16:21:08.000000 gwsumm-2.2.6/gwsumm/plot/sei.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.559890 gwsumm-2.2.6/gwsumm/plot/triggers/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1014 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/triggers/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9012 2022-12-20 19:28:31.000000 gwsumm-2.2.6/gwsumm/plot/triggers/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    21921 2023-11-02 17:15:14.000000 gwsumm-2.2.6/gwsumm/plot/triggers/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.561641 gwsumm-2.2.6/gwsumm/plot/triggers/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      807 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/triggers/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3902 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/plot/triggers/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4987 2023-11-01 22:18:02.000000 gwsumm-2.2.6/gwsumm/plot/utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12722 2024-01-25 21:39:34.000000 gwsumm-2.2.6/gwsumm/segments.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.564466 gwsumm-2.2.6/gwsumm/state/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2023 2023-05-22 17:31:39.000000 gwsumm-2.2.6/gwsumm/state/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2034 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/state/all.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12603 2023-11-01 16:21:08.000000 gwsumm-2.2.6/gwsumm/state/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3034 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/state/registry.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.573924 gwsumm-2.2.6/gwsumm/tabs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1506 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/tabs/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    29472 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/tabs/builtin.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    36826 2023-11-01 22:18:02.000000 gwsumm-2.2.6/gwsumm/tabs/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    39853 2024-03-26 21:53:27.000000 gwsumm-2.2.6/gwsumm/tabs/data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15759 2024-01-31 17:20:38.000000 gwsumm-2.2.6/gwsumm/tabs/etg.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10248 2022-01-25 22:56:26.000000 gwsumm-2.2.6/gwsumm/tabs/fscan.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10332 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tabs/gracedb.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14124 2024-03-26 21:53:27.000000 gwsumm-2.2.6/gwsumm/tabs/guardian.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9258 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/tabs/management.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3611 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tabs/misc.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2107 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/tabs/registry.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16837 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/tabs/sei.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4984 2022-09-15 15:47:20.000000 gwsumm-2.2.6/gwsumm/tabs/stamp.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.581076 gwsumm-2.2.6/gwsumm/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      790 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1170 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/common.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4780 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/test_archive.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4855 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4208 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/test_channels.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8768 2023-11-01 22:18:02.000000 gwsumm-2.2.6/gwsumm/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8903 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/test_data.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1803 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/test_mode.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10913 2024-02-09 21:54:30.000000 gwsumm-2.2.6/gwsumm/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4393 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/test_tabs.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3782 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16412 2024-03-19 23:14:10.000000 gwsumm-2.2.6/gwsumm/triggers.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1032 2020-04-07 19:56:04.000000 gwsumm-2.2.6/gwsumm/units.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6446 2021-03-09 19:10:52.000000 gwsumm-2.2.6/gwsumm/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-19 17:50:55.581809 gwsumm-2.2.6/gwsumm.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4764 2024-04-19 17:50:55.000000 gwsumm-2.2.6/gwsumm.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2986 2024-04-19 17:50:55.000000 gwsumm-2.2.6/gwsumm.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-19 17:50:55.000000 gwsumm-2.2.6/gwsumm.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      204 2024-04-19 17:50:55.000000 gwsumm-2.2.6/gwsumm.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      410 2024-04-19 17:50:55.000000 gwsumm-2.2.6/gwsumm.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        7 2024-04-19 17:50:55.000000 gwsumm-2.2.6/gwsumm.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     2891 2024-04-19 17:49:54.000000 gwsumm-2.2.6/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-19 17:50:55.584597 gwsumm-2.2.6/setup.cfg
```

### Comparing `gwsumm-2.2.5/.github/workflows/build.yml` & `gwsumm-2.2.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/.github/workflows/lint.yml` & `gwsumm-2.2.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/.readthedocs.yaml` & `gwsumm-2.2.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/CONTRIBUTING.md` & `gwsumm-2.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/LICENSE` & `gwsumm-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/PKG-INFO` & `gwsumm-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.2.5
+Version: 2.2.6
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwsumm.readthedocs.io
 Project-URL: Source Code, https://github.com/gwpy/gwsumm
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.0
 Requires-Dist: gwdatafind>=1.1.1
-Requires-Dist: gwdetchar>=2.2.5
+Requires-Dist: gwdetchar>=2.2.6
 Requires-Dist: gwpy>=2.0.0
 Requires-Dist: gwtrigfind
 Requires-Dist: lalsuite
 Requires-Dist: ligo-segments
 Requires-Dist: lscsoft-glue>=1.60.0
 Requires-Dist: lxml
 Requires-Dist: markdown
```

### Comparing `gwsumm-2.2.5/README.rst` & `gwsumm-2.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/Makefile` & `gwsumm-2.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/_static/css/custom.css` & `gwsumm-2.2.6/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/_templates/autoclass/class.rst` & `gwsumm-2.2.6/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/_templates/autosummary/class.rst` & `gwsumm-2.2.6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/_templates/autosummary/module.rst` & `gwsumm-2.2.6/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/automation.rst` & `gwsumm-2.2.6/docs/automation.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/cli.rst` & `gwsumm-2.2.6/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/conf.py` & `gwsumm-2.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/configuration/data.rst` & `gwsumm-2.2.6/docs/configuration/data.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/configuration/format.rst` & `gwsumm-2.2.6/docs/configuration/format.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/configuration/index.rst` & `gwsumm-2.2.6/docs/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/configuration/tabs.rst` & `gwsumm-2.2.6/docs/configuration/tabs.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/environment.yml` & `gwsumm-2.2.6/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/examples/first.png` & `gwsumm-2.2.6/docs/examples/first.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/examples/imc.png` & `gwsumm-2.2.6/docs/examples/imc.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/images/screenshot.png` & `gwsumm-2.2.6/docs/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/index.rst` & `gwsumm-2.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/make.bat` & `gwsumm-2.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/overview.rst` & `gwsumm-2.2.6/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/tabs/index.rst` & `gwsumm-2.2.6/docs/tabs/index.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/tabs/modes.rst` & `gwsumm-2.2.6/docs/tabs/modes.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/docs/tabs/websites.rst` & `gwsumm-2.2.6/docs/tabs/websites.rst`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/__init__.py` & `gwsumm-2.2.6/gwsumm/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/__main__.py` & `gwsumm-2.2.6/gwsumm/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/archive.py` & `gwsumm-2.2.6/gwsumm/archive.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/batch.py` & `gwsumm-2.2.6/gwsumm/batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/channels.py` & `gwsumm-2.2.6/gwsumm/channels.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/config/__init__.py` & `gwsumm-2.2.6/gwsumm/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/config/defaults.ini` & `gwsumm-2.2.6/gwsumm/config/defaults.ini`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/data/__init__.py` & `gwsumm-2.2.6/gwsumm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/data/coherence.py` & `gwsumm-2.2.6/gwsumm/data/coherence.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/data/mathutils.py` & `gwsumm-2.2.6/gwsumm/data/mathutils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/data/range.py` & `gwsumm-2.2.6/gwsumm/data/range.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/data/spectral.py` & `gwsumm-2.2.6/gwsumm/data/spectral.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/data/timeseries.py` & `gwsumm-2.2.6/gwsumm/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/data/utils.py` & `gwsumm-2.2.6/gwsumm/data/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/globalv.py` & `gwsumm-2.2.6/gwsumm/globalv.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/html/__init__.py` & `gwsumm-2.2.6/gwsumm/html/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/html/bootstrap.py` & `gwsumm-2.2.6/gwsumm/html/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/html/html5.py` & `gwsumm-2.2.6/gwsumm/html/html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/html/static.py` & `gwsumm-2.2.6/gwsumm/html/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 # build collection of CSS resources
 CSS = OrderedDict((
     ('font-awesome', 'https://cdnjs.cloudflare.com/ajax/libs/'
                      'font-awesome/6.5.1/css/fontawesome.min.css'),
     ('font-awesome-solid', 'https://cdnjs.cloudflare.com/ajax/libs/'
                            'font-awesome/6.5.1/css/solid.min.css'),
-    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.5/'
+    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.6/'
                     'lib/gwbootstrap.min.css'),
 ))
 
 # build collection of javascript resources
 JS = OrderedDict((
     ('jquery', 'https://code.jquery.com/jquery-3.7.1.min.js'),
     ('jquery-ui', 'https://code.jquery.com/ui/1.13.2/jquery-ui.min.js'),
@@ -47,15 +47,15 @@
     ('bootstrap', 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/'
                   'dist/js/bootstrap.bundle.min.js'),
     ('fancybox', 'https://cdn.jsdelivr.net/npm/@fancyapps/ui@5.0/'
                  'dist/fancybox/fancybox.umd.js'),
     ('datepicker', 'https://cdnjs.cloudflare.com/ajax/libs/'
                    'bootstrap-datepicker/1.9.0/js/'
                    'bootstrap-datepicker.min.js'),
-    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.5/'
+    ('gwbootstrap', 'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.6/'
                     'lib/gwbootstrap-extra.min.js'),
 ))
 
 
 # -- utilities ----------------------------------------------------------------
 
 def get_css():
```

### Comparing `gwsumm-2.2.5/gwsumm/html/tests/__init__.py` & `gwsumm-2.2.6/gwsumm/html/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/html/tests/test_bootstrap.py` & `gwsumm-2.2.6/gwsumm/html/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/html/tests/test_html5.py` & `gwsumm-2.2.6/gwsumm/html/tests/test_html5.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/html/tests/test_static.py` & `gwsumm-2.2.6/gwsumm/html/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/io.py` & `gwsumm-2.2.6/gwsumm/io.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/mode.py` & `gwsumm-2.2.6/gwsumm/mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/__init__.py` & `gwsumm-2.2.6/gwsumm/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/builtin.py` & `gwsumm-2.2.6/gwsumm/plot/builtin.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/core.py` & `gwsumm-2.2.6/gwsumm/plot/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/guardian/__init__.py` & `gwsumm-2.2.6/gwsumm/plot/guardian/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/guardian/__main__.py` & `gwsumm-2.2.6/gwsumm/plot/guardian/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/guardian/core.py` & `gwsumm-2.2.6/gwsumm/plot/guardian/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/guardian/tests/__init__.py` & `gwsumm-2.2.6/gwsumm/plot/guardian/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/guardian/tests/test_main.py` & `gwsumm-2.2.6/gwsumm/plot/guardian/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/mixins.py` & `gwsumm-2.2.6/gwsumm/plot/mixins.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/noisebudget.py` & `gwsumm-2.2.6/gwsumm/plot/noisebudget.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/range.py` & `gwsumm-2.2.6/gwsumm/plot/range.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/registry.py` & `gwsumm-2.2.6/gwsumm/plot/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/segments.py` & `gwsumm-2.2.6/gwsumm/plot/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/sei.py` & `gwsumm-2.2.6/gwsumm/plot/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/triggers/__init__.py` & `gwsumm-2.2.6/gwsumm/plot/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/triggers/__main__.py` & `gwsumm-2.2.6/gwsumm/plot/triggers/__main__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/triggers/core.py` & `gwsumm-2.2.6/gwsumm/plot/triggers/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/triggers/tests/__init__.py` & `gwsumm-2.2.6/gwsumm/plot/triggers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/triggers/tests/test_main.py` & `gwsumm-2.2.6/gwsumm/plot/triggers/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/plot/utils.py` & `gwsumm-2.2.6/gwsumm/plot/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/segments.py` & `gwsumm-2.2.6/gwsumm/segments.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/state/__init__.py` & `gwsumm-2.2.6/gwsumm/state/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/state/all.py` & `gwsumm-2.2.6/gwsumm/state/all.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/state/core.py` & `gwsumm-2.2.6/gwsumm/state/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/state/registry.py` & `gwsumm-2.2.6/gwsumm/state/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/__init__.py` & `gwsumm-2.2.6/gwsumm/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/builtin.py` & `gwsumm-2.2.6/gwsumm/tabs/builtin.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/core.py` & `gwsumm-2.2.6/gwsumm/tabs/core.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/data.py` & `gwsumm-2.2.6/gwsumm/tabs/data.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/etg.py` & `gwsumm-2.2.6/gwsumm/tabs/etg.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/fscan.py` & `gwsumm-2.2.6/gwsumm/tabs/fscan.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/gracedb.py` & `gwsumm-2.2.6/gwsumm/tabs/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/guardian.py` & `gwsumm-2.2.6/gwsumm/tabs/guardian.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/management.py` & `gwsumm-2.2.6/gwsumm/tabs/management.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/misc.py` & `gwsumm-2.2.6/gwsumm/tabs/misc.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/registry.py` & `gwsumm-2.2.6/gwsumm/tabs/registry.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/sei.py` & `gwsumm-2.2.6/gwsumm/tabs/sei.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tabs/stamp.py` & `gwsumm-2.2.6/gwsumm/tabs/stamp.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/__init__.py` & `gwsumm-2.2.6/gwsumm/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/common.py` & `gwsumm-2.2.6/gwsumm/tests/common.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_archive.py` & `gwsumm-2.2.6/gwsumm/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_batch.py` & `gwsumm-2.2.6/gwsumm/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_channels.py` & `gwsumm-2.2.6/gwsumm/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_config.py` & `gwsumm-2.2.6/gwsumm/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_data.py` & `gwsumm-2.2.6/gwsumm/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_mode.py` & `gwsumm-2.2.6/gwsumm/tests/test_mode.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_plot.py` & `gwsumm-2.2.6/gwsumm/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_tabs.py` & `gwsumm-2.2.6/gwsumm/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/tests/test_utils.py` & `gwsumm-2.2.6/gwsumm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/triggers.py` & `gwsumm-2.2.6/gwsumm/triggers.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/units.py` & `gwsumm-2.2.6/gwsumm/units.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm/utils.py` & `gwsumm-2.2.6/gwsumm/utils.py`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/gwsumm.egg-info/PKG-INFO` & `gwsumm-2.2.6/gwsumm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsumm
-Version: 2.2.5
+Version: 2.2.6
 Summary: A python toolbox used by the LIGO Scientific Collaboration for detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwsumm.readthedocs.io
 Project-URL: Source Code, https://github.com/gwpy/gwsumm
 Project-URL: Bug Tracker, https://github.com/gwpy/gwsumm/issues
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: astropy>=3.0.0
 Requires-Dist: gwdatafind>=1.1.1
-Requires-Dist: gwdetchar>=2.2.5
+Requires-Dist: gwdetchar>=2.2.6
 Requires-Dist: gwpy>=2.0.0
 Requires-Dist: gwtrigfind
 Requires-Dist: lalsuite
 Requires-Dist: ligo-segments
 Requires-Dist: lscsoft-glue>=1.60.0
 Requires-Dist: lxml
 Requires-Dist: markdown
```

### Comparing `gwsumm-2.2.5/gwsumm.egg-info/SOURCES.txt` & `gwsumm-2.2.6/gwsumm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwsumm-2.2.5/pyproject.toml` & `gwsumm-2.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   "Topic :: Scientific/Engineering :: Astronomy",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 dependencies = [
   "astropy >=3.0.0",
   "gwdatafind >=1.1.1",
-  "gwdetchar >=2.2.5",
+  "gwdetchar >=2.2.6",
   "gwpy >=2.0.0",
   "gwtrigfind",
   "lalsuite",
   "ligo-segments",
   "lscsoft-glue >=1.60.0",
   "lxml",
   "markdown",
```

