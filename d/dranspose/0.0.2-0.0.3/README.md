# Comparing `tmp/dranspose-0.0.2.tar.gz` & `tmp/dranspose-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dranspose-0.0.2.tar", last modified: Mon Jan  8 16:47:44 2024, max compression
+gzip compressed data, was "dranspose-0.0.3.tar", last modified: Fri Apr 19 08:25:47 2024, max compression
```

## Comparing `dranspose-0.0.2.tar` & `dranspose-0.0.3.tar`

### file list

```diff
@@ -1,131 +1,175 @@
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.358728 dranspose-0.0.2/
--rw-r--r--   0 feleng    (1000) feleng    (1000)      157 2024-01-08 10:04:19.000000 dranspose-0.0.2/.flake8
--rw-r--r--   0 feleng    (1000) feleng    (1000)      101 2023-12-04 22:59:46.000000 dranspose-0.0.2/.gitignore
--rw-r--r--   0 feleng    (1000) feleng    (1000)      460 2023-12-20 14:11:19.000000 dranspose-0.0.2/.gitlab-ci.yml
--rw-r--r--   0 feleng    (1000) feleng    (1000)      640 2024-01-08 10:11:03.000000 dranspose-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 feleng    (1000) feleng    (1000)      103 2023-11-14 09:28:43.000000 dranspose-0.0.2/Dockerfile
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1072 2023-12-03 13:40:04.000000 dranspose-0.0.2/LICENSE
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1676 2024-01-08 16:47:44.358728 dranspose-0.0.2/PKG-INFO
--rw-r--r--   0 feleng    (1000) feleng    (1000)      601 2023-12-04 23:34:21.000000 dranspose-0.0.2/README.md
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.348728 dranspose-0.0.2/docs/
--rw-r--r--   0 feleng    (1000) feleng    (1000)       48 2023-11-29 16:34:31.000000 dranspose-0.0.2/docs/.gitignore
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.348728 dranspose-0.0.2/docs/applications/
--rw-r--r--   0 feleng    (1000) feleng    (1000)     5210 2023-12-04 23:34:21.000000 dranspose-0.0.2/docs/applications/overview.md
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.348728 dranspose-0.0.2/docs/deployment/
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1926 2023-12-01 20:06:45.000000 dranspose-0.0.2/docs/deployment/capturing.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1240 2023-12-04 23:34:21.000000 dranspose-0.0.2/docs/deployment/kubernetes.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)      383 2023-12-03 13:23:04.000000 dranspose-0.0.2/docs/index.md
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/docs/poster-2024-01-15/
--rw-r--r--   0 feleng    (1000) feleng    (1000)        6 2024-01-08 07:32:42.000000 dranspose-0.0.2/docs/poster-2024-01-15/.gitignore
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/docs/poster-2024-01-15/logo/
--rw-r--r--   0 feleng    (1000) feleng    (1000)    42506 2024-01-08 07:22:29.000000 dranspose-0.0.2/docs/poster-2024-01-15/logo/lulogo.pdf
--rw-r--r--   0 feleng    (1000) feleng    (1000)    15700 2024-01-08 16:42:48.000000 dranspose-0.0.2/docs/poster-2024-01-15/logo/maxivlogo.pdf
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3744 2024-01-08 07:22:29.000000 dranspose-0.0.2/docs/poster-2024-01-15/lutheme.sty
--rw-r--r--   0 feleng    (1000) feleng    (1000)    11408 2024-01-08 16:43:19.000000 dranspose-0.0.2/docs/poster-2024-01-15/main.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)      421 2024-01-08 10:38:48.000000 dranspose-0.0.2/docs/poster-2024-01-15/reducer.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)    30338 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposter.cls
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2134 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterBackgroundstyles.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)     8363 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterBlockstyles.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1537 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterColorpalettes.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)     6502 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterColorstyles.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)    10868 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterInnerblockstyles.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2747 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterLayoutthemes.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)     7851 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterNotestyles.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)     6372 2024-01-08 10:10:53.000000 dranspose-0.0.2/docs/poster-2024-01-15/tikzposterTitlestyles.tex
--rw-r--r--   0 feleng    (1000) feleng    (1000)      509 2024-01-08 10:38:38.000000 dranspose-0.0.2/docs/poster-2024-01-15/values.yaml
--rw-r--r--   0 feleng    (1000) feleng    (1000)      186 2024-01-08 12:58:14.000000 dranspose-0.0.2/docs/poster-2024-01-15/viewer.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)      418 2024-01-08 10:36:34.000000 dranspose-0.0.2/docs/poster-2024-01-15/worker.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/docs/reference/
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/docs/reference/internals/
--rw-r--r--   0 feleng    (1000) feleng    (1000)       27 2023-12-01 16:17:01.000000 dranspose-0.0.2/docs/reference/internals/distributed_service.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)       22 2023-12-01 16:28:29.000000 dranspose-0.0.2/docs/reference/internals/ingester.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)      172 2023-12-01 20:28:06.000000 dranspose-0.0.2/docs/reference/middlewares.md
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/docs/reference/protocols/
--rw-r--r--   0 feleng    (1000) feleng    (1000)       26 2023-12-01 20:08:24.000000 dranspose-0.0.2/docs/reference/protocols/contrast.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)       44 2023-12-01 20:34:01.000000 dranspose-0.0.2/docs/reference/protocols/events.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)       26 2023-12-01 20:24:40.000000 dranspose-0.0.2/docs/reference/protocols/xspress.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)     4805 2023-12-04 23:34:21.000000 dranspose-0.0.2/docs/reference/trigger_map.md
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/docs/seminar-2023-11-30/
--rw-r--r--   0 feleng    (1000) feleng    (1000)    20633 2023-12-04 23:34:21.000000 dranspose-0.0.2/docs/seminar-2023-11-30/main.tex
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/docs/tutorials/
--rw-r--r--   0 feleng    (1000) feleng    (1000)       78 2023-12-01 18:48:27.000000 dranspose-0.0.2/docs/tutorials/ingesters.md
--rw-r--r--   0 feleng    (1000) feleng    (1000)      696 2023-12-04 23:34:21.000000 dranspose-0.0.2/docs/tutorials/viewers.md
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.352062 dranspose-0.0.2/dranspose/
--rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2023-11-14 07:32:03.000000 dranspose-0.0.2/dranspose/__init__.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     7583 2023-12-21 13:05:27.000000 dranspose-0.0.2/dranspose/cli.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)    16424 2023-12-22 20:25:16.000000 dranspose-0.0.2/dranspose/controller.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.355395 dranspose-0.0.2/dranspose/data/
--rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2023-11-17 18:33:57.000000 dranspose-0.0.2/dranspose/data/__init__.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2947 2023-12-06 18:59:00.000000 dranspose-0.0.2/dranspose/data/contrast.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)      401 2023-12-12 15:36:22.000000 dranspose-0.0.2/dranspose/data/sardana.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)      610 2023-12-04 19:21:30.000000 dranspose-0.0.2/dranspose/data/stream1.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2202 2023-12-02 02:08:51.000000 dranspose-0.0.2/dranspose/data/xspress3.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3099 2023-12-22 15:28:48.000000 dranspose-0.0.2/dranspose/debug_worker.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     6639 2023-12-22 15:28:48.000000 dranspose-0.0.2/dranspose/distributed.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3647 2023-12-22 15:28:48.000000 dranspose-0.0.2/dranspose/event.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.355395 dranspose-0.0.2/dranspose/helpers/
--rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2023-12-02 19:35:38.000000 dranspose-0.0.2/dranspose/helpers/__init__.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2118 2023-12-04 23:02:40.000000 dranspose-0.0.2/dranspose/helpers/jsonpath_slice_ext.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)      915 2023-12-22 15:28:48.000000 dranspose-0.0.2/dranspose/helpers/utils.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)    10884 2023-12-21 13:11:37.000000 dranspose-0.0.2/dranspose/ingester.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.355395 dranspose-0.0.2/dranspose/ingesters/
--rw-r--r--   0 feleng    (1000) feleng    (1000)      582 2023-12-19 13:39:13.000000 dranspose-0.0.2/dranspose/ingesters/__init__.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3866 2023-12-21 13:12:46.000000 dranspose-0.0.2/dranspose/ingesters/http_sardana.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2594 2023-12-19 13:27:47.000000 dranspose-0.0.2/dranspose/ingesters/tcp_positioncap.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2789 2023-12-22 10:40:17.000000 dranspose-0.0.2/dranspose/ingesters/zmqpull_single.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2905 2023-12-19 09:28:08.000000 dranspose-0.0.2/dranspose/ingesters/zmqsub_contrast.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3152 2023-12-19 09:28:08.000000 dranspose-0.0.2/dranspose/ingesters/zmqsub_xspress3.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     8169 2023-12-22 19:32:45.000000 dranspose-0.0.2/dranspose/mapping.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.355395 dranspose-0.0.2/dranspose/middlewares/
--rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2023-11-30 19:37:04.000000 dranspose-0.0.2/dranspose/middlewares/__init__.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)      685 2023-12-04 23:00:45.000000 dranspose-0.0.2/dranspose/middlewares/contrast.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1074 2023-12-04 19:29:00.000000 dranspose-0.0.2/dranspose/middlewares/stream1.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1810 2023-12-04 23:00:30.000000 dranspose-0.0.2/dranspose/middlewares/xspress.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)      630 2023-12-08 09:57:46.000000 dranspose-0.0.2/dranspose/parameters.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     6024 2023-12-21 10:07:14.000000 dranspose-0.0.2/dranspose/protocol.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     5838 2023-12-21 13:46:37.000000 dranspose-0.0.2/dranspose/reducer.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2529 2023-12-07 13:54:19.000000 dranspose-0.0.2/dranspose/replay.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)    14981 2023-12-22 15:28:48.000000 dranspose-0.0.2/dranspose/worker.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.358728 dranspose-0.0.2/dranspose.egg-info/
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1676 2024-01-08 16:47:44.000000 dranspose-0.0.2/dranspose.egg-info/PKG-INFO
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3097 2024-01-08 16:47:44.000000 dranspose-0.0.2/dranspose.egg-info/SOURCES.txt
--rw-r--r--   0 feleng    (1000) feleng    (1000)        1 2024-01-08 16:47:44.000000 dranspose-0.0.2/dranspose.egg-info/dependency_links.txt
--rw-r--r--   0 feleng    (1000) feleng    (1000)       48 2024-01-08 16:47:44.000000 dranspose-0.0.2/dranspose.egg-info/entry_points.txt
--rw-r--r--   0 feleng    (1000) feleng    (1000)      182 2024-01-08 16:47:44.000000 dranspose-0.0.2/dranspose.egg-info/requires.txt
--rw-r--r--   0 feleng    (1000) feleng    (1000)       10 2024-01-08 16:47:44.000000 dranspose-0.0.2/dranspose.egg-info/top_level.txt
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.348728 dranspose-0.0.2/examples/
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.355395 dranspose-0.0.2/examples/dummy/
--rw-r--r--   0 feleng    (1000) feleng    (1000)      678 2023-12-06 15:25:04.000000 dranspose-0.0.2/examples/dummy/reducer.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1728 2023-12-07 14:38:24.000000 dranspose-0.0.2/examples/dummy/worker.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.355395 dranspose-0.0.2/examples/slow/
--rw-r--r--   0 feleng    (1000) feleng    (1000)      633 2023-12-09 17:05:31.000000 dranspose-0.0.2/examples/slow/worker.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)      460 2023-12-03 13:23:22.000000 dranspose-0.0.2/mkdocs.yml
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1820 2024-01-08 10:07:03.000000 dranspose-0.0.2/pyproject.toml
--rw-r--r--   0 feleng    (1000) feleng    (1000)       38 2024-01-08 16:47:44.358728 dranspose-0.0.2/setup.cfg
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.355395 dranspose-0.0.2/tests/
--rw-r--r--   0 feleng    (1000) feleng    (1000)        4 2023-11-30 14:57:04.000000 dranspose-0.0.2/tests/.gitignore
--rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2023-11-14 07:32:03.000000 dranspose-0.0.2/tests/__init__.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)    16693 2023-12-19 09:15:44.000000 dranspose-0.0.2/tests/conftest.py
-drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-01-08 16:47:44.358728 dranspose-0.0.2/tests/data/
--rw-r-----   0 feleng    (1000) feleng    (1000)    52937 2023-11-30 13:58:13.000000 dranspose-0.0.2/tests/data/contrast-dump.pkls
--rw-r-----   0 feleng    (1000) feleng    (1000)  1327179 2023-11-30 13:58:13.000000 dranspose-0.0.2/tests/data/xspress3-dump.pkls
--rw-r--r--   0 feleng    (1000) feleng    (1000)   736165 2023-12-07 14:50:55.000000 dranspose-0.0.2/tests/data/xspress3mini-dump20.pkls
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2159 2023-12-04 23:26:57.000000 dranspose-0.0.2/tests/stream1.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     8153 2023-12-19 09:26:43.000000 dranspose-0.0.2/tests/test_basics.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2828 2023-12-19 09:26:43.000000 dranspose-0.0.2/tests/test_controller.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1065 2023-12-04 23:26:09.000000 dranspose-0.0.2/tests/test_data_streams.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     5253 2023-12-19 09:26:43.000000 dranspose-0.0.2/tests/test_debugworker.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     6301 2023-12-19 09:26:43.000000 dranspose-0.0.2/tests/test_dumping.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1008 2023-12-03 16:20:54.000000 dranspose-0.0.2/tests/test_jsonpath.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     9100 2023-12-22 19:31:19.000000 dranspose-0.0.2/tests/test_mapping.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     5741 2023-12-22 15:28:58.000000 dranspose-0.0.2/tests/test_mulitple_scans.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2937 2023-12-19 12:47:21.000000 dranspose-0.0.2/tests/test_panda.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2249 2023-12-19 09:26:43.000000 dranspose-0.0.2/tests/test_param_descriptions.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3059 2023-12-19 09:26:43.000000 dranspose-0.0.2/tests/test_parameters.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     4529 2023-12-19 09:26:43.000000 dranspose-0.0.2/tests/test_processingtime.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     2026 2023-12-04 23:23:11.000000 dranspose-0.0.2/tests/test_protocol.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     4633 2023-12-19 09:28:08.000000 dranspose-0.0.2/tests/test_reducer.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     4328 2023-12-22 20:25:15.000000 dranspose-0.0.2/tests/test_sardana_hook.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     3019 2023-12-12 16:06:26.000000 dranspose-0.0.2/tests/test_sardana_ingester.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     6080 2023-12-22 15:28:48.000000 dranspose-0.0.2/tests/test_short_scans.py
--rw-r--r--   0 feleng    (1000) feleng    (1000)     1038 2023-12-22 15:28:48.000000 dranspose-0.0.2/tests/test_zmq_cancel.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.746570 dranspose-0.0.3/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      157 2024-03-24 16:22:49.000000 dranspose-0.0.3/.flake8
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      101 2024-01-12 22:49:34.000000 dranspose-0.0.3/.gitignore
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      504 2024-03-29 13:08:00.000000 dranspose-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      640 2024-01-12 22:49:34.000000 dranspose-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      630 2024-04-18 17:04:20.000000 dranspose-0.0.3/Dockerfile
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1072 2024-01-12 22:49:34.000000 dranspose-0.0.3/LICENSE
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1676 2024-04-19 08:25:47.743237 dranspose-0.0.3/PKG-INFO
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      601 2024-01-12 22:49:34.000000 dranspose-0.0.3/README.md
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.733237 dranspose-0.0.3/docs/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       48 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/.gitignore
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       10 2024-01-12 22:49:30.000000 dranspose-0.0.3/docs/CNAME
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.733237 dranspose-0.0.3/docs/applications/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     5230 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/applications/overview.md
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.733237 dranspose-0.0.3/docs/deployment/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1926 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/deployment/capturing.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1457 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/deployment/kubernetes.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2271 2024-02-06 09:18:19.000000 dranspose-0.0.3/docs/deployment/sardana.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1342 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/index.md
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.733237 dranspose-0.0.3/docs/poster-2024-01-15/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       19 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/.gitignore
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.733237 dranspose-0.0.3/docs/poster-2024-01-15/logo/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    42506 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/logo/lulogo.pdf
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    15700 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/logo/maxivlogo.pdf
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3744 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/lutheme.sty
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    12636 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/main.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      391 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/reducer.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    30338 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposter.cls
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2134 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterBackgroundstyles.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     8363 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterBlockstyles.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1537 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterColorpalettes.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     6502 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterColorstyles.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    10868 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterInnerblockstyles.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2747 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterLayoutthemes.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     7851 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterNotestyles.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     6372 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/tikzposterTitlestyles.tex
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      509 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/values.yaml
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      186 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/viewer.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      418 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/poster-2024-01-15/worker.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/docs/reference/
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/docs/reference/internals/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       27 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/reference/internals/distributed_service.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       22 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/reference/internals/ingester.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      172 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/reference/middlewares.md
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/docs/reference/protocols/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       25 2024-02-05 10:47:16.000000 dranspose-0.0.3/docs/reference/protocols/STINS.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       24 2024-02-05 10:54:26.000000 dranspose-0.0.3/docs/reference/protocols/albaem.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       26 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/reference/protocols/contrast.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       44 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/reference/protocols/events.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       25 2024-02-05 11:00:17.000000 dranspose-0.0.3/docs/reference/protocols/sardana.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       26 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/reference/protocols/xspress.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4805 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/reference/trigger_map.md
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/docs/seminar-2023-11-30/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    20633 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/seminar-2023-11-30/main.tex
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/docs/tutorials/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       78 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/tutorials/ingesters.md
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      697 2024-01-12 22:49:34.000000 dranspose-0.0.3/docs/tutorials/viewers.md
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/dranspose/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/__init__.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     9015 2024-03-28 00:32:20.000000 dranspose-0.0.3/dranspose/cli.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    23598 2024-04-18 16:10:07.000000 dranspose-0.0.3/dranspose/controller.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/dranspose/data/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/data/__init__.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1681 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/data/albaem.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2947 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/data/contrast.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1028 2024-03-13 14:47:37.000000 dranspose-0.0.3/dranspose/data/eiger_legacy.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      973 2024-03-23 13:37:00.000000 dranspose-0.0.3/dranspose/data/positioncap.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2538 2024-02-05 14:01:23.000000 dranspose-0.0.3/dranspose/data/sardana.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1572 2024-02-05 13:21:33.000000 dranspose-0.0.3/dranspose/data/stream1.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2202 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/data/xspress3.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2887 2024-03-25 13:08:31.000000 dranspose-0.0.3/dranspose/debug_worker.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     9304 2024-03-25 13:08:49.000000 dranspose-0.0.3/dranspose/distributed.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3647 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/event.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.736570 dranspose-0.0.3/dranspose/helpers/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/helpers/__init__.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2118 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/helpers/jsonpath_slice_ext.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1242 2024-03-23 13:36:13.000000 dranspose-0.0.3/dranspose/helpers/utils.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    13711 2024-03-25 14:26:22.000000 dranspose-0.0.3/dranspose/ingester.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/dranspose/ingesters/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      833 2024-03-14 15:27:55.000000 dranspose-0.0.3/dranspose/ingesters/__init__.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3877 2024-03-14 10:16:10.000000 dranspose-0.0.3/dranspose/ingesters/http_sardana.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2594 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/ingesters/tcp_positioncap.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2926 2024-03-13 14:47:37.000000 dranspose-0.0.3/dranspose/ingesters/zmqpull_eiger_legacy.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2789 2024-03-25 14:05:53.000000 dranspose-0.0.3/dranspose/ingesters/zmqpull_single.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2718 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/ingesters/zmqsub_albaem.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2905 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/ingesters/zmqsub_contrast.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3152 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/ingesters/zmqsub_xspress3.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     8788 2024-04-18 08:31:48.000000 dranspose-0.0.3/dranspose/mapping.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/dranspose/middlewares/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/middlewares/__init__.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      685 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/middlewares/contrast.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1753 2024-03-23 13:37:10.000000 dranspose-0.0.3/dranspose/middlewares/positioncap.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      600 2024-01-24 16:42:14.000000 dranspose-0.0.3/dranspose/middlewares/sardana.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1046 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/middlewares/stream1.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1810 2024-01-12 22:49:34.000000 dranspose-0.0.3/dranspose/middlewares/xspress.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1764 2024-02-10 12:00:34.000000 dranspose-0.0.3/dranspose/parameters.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     7655 2024-04-02 12:21:38.000000 dranspose-0.0.3/dranspose/protocol.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     7812 2024-03-23 21:47:11.000000 dranspose-0.0.3/dranspose/reducer.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     6210 2024-02-06 14:31:28.000000 dranspose-0.0.3/dranspose/replay.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    18868 2024-03-25 14:18:55.000000 dranspose-0.0.3/dranspose/worker.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.743237 dranspose-0.0.3/dranspose.egg-info/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1676 2024-04-19 08:25:47.000000 dranspose-0.0.3/dranspose.egg-info/PKG-INFO
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4163 2024-04-19 08:25:47.000000 dranspose-0.0.3/dranspose.egg-info/SOURCES.txt
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        1 2024-04-19 08:25:47.000000 dranspose-0.0.3/dranspose.egg-info/dependency_links.txt
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       48 2024-04-19 08:25:47.000000 dranspose-0.0.3/dranspose.egg-info/entry_points.txt
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      182 2024-04-19 08:25:47.000000 dranspose-0.0.3/dranspose.egg-info/requires.txt
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       10 2024-04-19 08:25:47.000000 dranspose-0.0.3/dranspose.egg-info/top_level.txt
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.733237 dranspose-0.0.3/examples/
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/examples/dummy/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      756 2024-01-12 22:49:34.000000 dranspose-0.0.3/examples/dummy/reducer.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1736 2024-01-12 22:49:34.000000 dranspose-0.0.3/examples/dummy/worker.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/examples/parser/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      828 2024-03-23 13:03:30.000000 dranspose-0.0.3/examples/parser/positioncap.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/examples/repub/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      922 2024-02-08 12:55:41.000000 dranspose-0.0.3/examples/repub/worker.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/examples/slow/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      626 2024-02-05 15:52:07.000000 dranspose-0.0.3/examples/slow/reducer.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      652 2024-03-23 20:46:37.000000 dranspose-0.0.3/examples/slow/worker.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      632 2024-02-05 14:18:00.000000 dranspose-0.0.3/mkdocs.yml
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/perf/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        7 2024-03-25 18:41:23.000000 dranspose-0.0.3/perf/.gitignore
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    49854 2024-04-02 14:20:44.000000 dranspose-0.0.3/perf/Cargo.lock
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      687 2024-04-02 14:20:36.000000 dranspose-0.0.3/perf/Cargo.toml
+-rw-r--r--   0 feleng    (1000) feleng    (1000)      660 2024-04-02 14:30:12.000000 dranspose-0.0.3/perf/Dockerfile
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.739903 dranspose-0.0.3/perf/src/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    10053 2024-04-02 14:02:06.000000 dranspose-0.0.3/perf/src/control_plane.rs
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     8799 2024-04-18 16:04:18.000000 dranspose-0.0.3/perf/src/data_plane.rs
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1049 2024-04-02 13:10:00.000000 dranspose-0.0.3/perf/src/dranspose.rs
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1714 2024-04-18 15:31:27.000000 dranspose-0.0.3/perf/src/main.rs
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1820 2024-01-12 22:49:34.000000 dranspose-0.0.3/pyproject.toml
+-rw-r--r--   0 feleng    (1000) feleng    (1000)       38 2024-04-19 08:25:47.746570 dranspose-0.0.3/setup.cfg
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.743237 dranspose-0.0.3/tests/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        4 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/.gitignore
+-rw-r--r--   0 feleng    (1000) feleng    (1000)        0 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/__init__.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    22622 2024-04-18 16:21:03.000000 dranspose-0.0.3/tests/conftest.py
+drwxr-xr-x   0 feleng    (1000) feleng    (1000)        0 2024-04-19 08:25:47.743237 dranspose-0.0.3/tests/data/
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1470 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/data/albaem-dump.pkls
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    52937 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/data/contrast-dump.pkls
+-rw-r--r--   0 feleng    (1000) feleng    (1000)   111100 2024-03-13 14:46:43.000000 dranspose-0.0.3/tests/data/eiger-small.pkls
+-rw-r--r--   0 feleng    (1000) feleng    (1000)  1327179 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/data/xspress3-dump.pkls
+-rw-r--r--   0 feleng    (1000) feleng    (1000)   736165 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/data/xspress3mini-dump20.pkls
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2159 2024-04-18 11:23:53.000000 dranspose-0.0.3/tests/stream1.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2732 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_albaem.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     8224 2024-04-02 13:07:55.000000 dranspose-0.0.3/tests/test_basics.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2852 2024-03-29 10:48:28.000000 dranspose-0.0.3/tests/test_controller.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1837 2024-03-13 15:59:42.000000 dranspose-0.0.3/tests/test_data_streams.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     5253 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_debugworker.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2287 2024-02-10 12:08:29.000000 dranspose-0.0.3/tests/test_default_parameters.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3799 2024-04-18 09:20:19.000000 dranspose-0.0.3/tests/test_discard_scan.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     7127 2024-04-18 09:20:55.000000 dranspose-0.0.3/tests/test_dumping.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2823 2024-03-23 13:36:50.000000 dranspose-0.0.3/tests/test_eiger_legacy.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3270 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_empty_event.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1008 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_jsonpath.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)    11700 2024-04-18 09:20:19.000000 dranspose-0.0.3/tests/test_mapping.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4493 2024-03-25 14:19:32.000000 dranspose-0.0.3/tests/test_maxrate.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     5741 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_mulitple_scans.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4111 2024-04-18 16:21:03.000000 dranspose-0.0.3/tests/test_outside_scan_push.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3133 2024-03-23 13:36:30.000000 dranspose-0.0.3/tests/test_panda.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2675 2024-02-10 12:12:23.000000 dranspose-0.0.3/tests/test_param_descriptions.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3298 2024-02-10 12:23:30.000000 dranspose-0.0.3/tests/test_parameters.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4659 2024-02-10 12:54:36.000000 dranspose-0.0.3/tests/test_processingtime.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2026 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_protocol.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4633 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_reducer.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4120 2024-02-08 16:14:52.000000 dranspose-0.0.3/tests/test_repub.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3460 2024-04-02 14:02:01.000000 dranspose-0.0.3/tests/test_restart_ingester.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3856 2024-02-10 13:18:48.000000 dranspose-0.0.3/tests/test_restart_worker.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3851 2024-02-08 13:06:35.000000 dranspose-0.0.3/tests/test_round_robin.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3059 2024-04-02 13:57:14.000000 dranspose-0.0.3/tests/test_rust_ingest.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     4328 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_sardana_hook.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3019 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_sardana_ingester.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     6080 2024-01-12 22:49:34.000000 dranspose-0.0.3/tests/test_short_scans.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     3507 2024-01-25 16:56:50.000000 dranspose-0.0.3/tests/test_slowreduce.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     1105 2024-03-14 10:15:18.000000 dranspose-0.0.3/tests/test_zmq_cancel.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     2774 2024-03-25 10:16:49.000000 dranspose-0.0.3/tests/test_zmq_multiroute.py
+-rw-r--r--   0 feleng    (1000) feleng    (1000)     6639 2024-03-25 14:22:05.000000 dranspose-0.0.3/tests/test_zmq_rate.py
```

### Comparing `dranspose-0.0.2/.pre-commit-config.yaml` & `dranspose-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/LICENSE` & `dranspose-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/PKG-INFO` & `dranspose-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dranspose
-Version: 0.0.2
+Version: 0.0.3
 Summary: A stream matrix transposition framework
 Author-email: Felix Engelmann <felix-github@nlogn.org>
 Project-URL: Homepage, https://github.com/felix-engelmann/dranspose
 Project-URL: Bug Tracker, https://github.com/felix-engelmann/dranspose/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dranspose-0.0.2/README.md` & `dranspose-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/applications/overview.md` & `dranspose-0.0.3/docs/applications/overview.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from dranspose.event import EventData
 from dranspose.middlewares import contrast
 from dranspose.middlewares import xspress
 
 logger = logging.getLogger(__name__)
 
 class FluorescenceWorker:
-    def __init__(self, parameters=None):
+    def __init__(self, parameters=None, **kwargs):
         self.number = 0
 
 ```
 The `process_event` function gets an [EventData](../reference/protocols/events.md) object which contains all required streams for the current event.
 The first step should be to check that the required streams for the analyis are present.
 ```python
     def process_event(self, event: EventData, parameters=None):
@@ -102,15 +102,15 @@
 The reducer may also have a setup in `__init__` where is may initialise the special `publish` attribute.
 This attribute is automatically exposed via *http* for live viewers
 
 ```python
 from dranspose.event import ResultData
 
 class FluorescenceReducer:
-    def __init__(self, parameters=None):
+    def __init__(self, parameters=None, **kwargs):
         self.number = 0
         self.publish = {"map": {}}
 ```
 In `process_result`, only simple operations are possible, such as appending to a dictionary, as this has to run at the acquisition speed.
 ```python
     def process_result(self, result: ResultData, parameters=None):
         print(result)
```

### Comparing `dranspose-0.0.2/docs/deployment/capturing.md` & `dranspose-0.0.3/docs/deployment/capturing.md`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/deployment/kubernetes.md` & `dranspose-0.0.3/docs/deployment/kubernetes.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # K8s deployment
 
-The most easy way to run a distributed version of dranspose is via a helm chart.
+The most easy way to run a distributed version of dranspose is via a [helm chart](https://github.com/felix-engelmann/dranspose-helm).
 
 
 ## Values
 
 The required values are a `beamline` to be able to mount the correct volumes.
 The `dump_prefix` may be set to a path to which the ingesters dump all stream messages.
 This is useful to get the initial data to develop a worker which can digest these.
 
-The `ingesters` map specifies the name of the stream, the `connect_url` on where to connect to and the class.
-Other ingesters may need additional settings.
+The `ingesters` map specifies the name of the stream, the `upstream_url` on where to connect to and the class.
+Other ingesters may need additional settings. 
+If the stream name contains underscores, a separate `stream` entry can be used as k8s does not allow underscore in deployment names.
 
 The `workers` and the `reducer` run with a custom docker image which contains all the dependencies for the analysis
 `worker.class` and `reducer.class` specify the paths to the correct classes in the analysis container.
 
 ```yaml
 global:
   beamline: nanomax
   dump_prefix: false #"/data/staff/dummymax/dumps/ingest_dump_"
 
 ingesters:
   contrast:
-    connect_url: "tcp://172.16.125.30:5556"
+    upstream_url: "tcp://172.16.125.30:5556"
     ingester_class: "StreamingContrastIngester"
+    stream: "contrast_one"
   xspress3:
-    connect_url: "tcp://172.16.126.70:9999"
+    upstream_url: "tcp://172.16.126.70:9999"
     ingester_class: "StreamingXspressIngester"
 
 science_image: "harbor.maxiv.lu.se/daq/dranspose/nanomax-fluorescence:main"
 
 worker:
   class: "src.worker:FluorescenceWorker"
 reducer:
```

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/logo/lulogo.pdf` & `dranspose-0.0.3/docs/poster-2024-01-15/logo/lulogo.pdf`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/logo/maxivlogo.pdf` & `dranspose-0.0.3/docs/poster-2024-01-15/logo/maxivlogo.pdf`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/lutheme.sty` & `dranspose-0.0.3/docs/poster-2024-01-15/lutheme.sty`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/main.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/main.tex`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 \usepackage{csquotes}
 %\usepackage[style=ieee]{biblatex}
 %\addbibresource{refs.bib}
 
 \usepackage{fontawesome5}
 
  % Title, Author, Institute
-\title{\texttt{dranspo}{\sffamily.}\texttt{se} – A Flexible Live Processing Pipeline}
+\title{\texttt{DRANSPO}{\sffamily.}\texttt{SE} – a Flexible Live Processing Pipeline}
 \author{Felix Engelmann}
-\institute{Scientific Data, MAX IV}
+\institute{Scientific Data}
 
 %Remove LaTeX tag at bottom of the poster
 \tikzposterlatexaffectionproofoff
 
 \newcommand\ttl[1]{\texttt{\lseries#1}}
 \newcommand\ttm[1]{\texttt{\mdseries#1}}
 \newcommand\ttb[1]{\texttt{\bfseries#1}}
@@ -48,20 +48,20 @@
 emphstyle=\ttfamily\bfseries\color{deepred},    % Custom highlighting style
 stringstyle=\color{deepgreen},
 %frame=tb,                         % Any extra options here
 showstringspaces=false
 }%}
 
 \lstdefinestyle{yaml}{
-     basicstyle=\color{blue}\footnotesize,
+     basicstyle=\ttfamily\color{blue}\footnotesize,
      rulecolor=\color{black},
      string=[s]{'}{'},
-     stringstyle=\color{blue},
+     stringstyle=\ttfamily\color{blue},
      comment=[l]{:},
-     commentstyle=\color{black},
+     commentstyle=\ttfamily\color{black},
      morecomment=[l]{-}
  }
 
 
 \lstset{style=mystyle}
 
 % Python environment
@@ -81,25 +81,50 @@
 \maketitle
 
 %Input logos in relation to title node
 %Go to the image bank https://lu-mediaportal.qbank.se for other images and logotypes.
 \node[anchor=west, xshift=15mm] at (TP@title.west) {\includegraphics[width=8cm]{lulogo.pdf}};
 \node[anchor=east,xshift=-15mm] at (TP@title.east) {\includegraphics[width=10cm]{maxivlogo.pdf}};
 
-\node[anchor=center, xshift=-219mm,yshift=-2cm] at (TP@title.center) {\qrcode[height=5cm]{https://dranspo.se/}};
+\node[anchor=center, xshift=-219mm,yshift=-2.2cm] at (TP@title.center) {\qrcode[height=5cm]{https://dranspo.se/}};
 
+\block{Accelerating Scientific Insight Through Rapid Feedback}{
+\centering
+\begin{tikzpicture}
+ \node[below right, text width=15cm] (sc) at (0,0) {{\huge Scanning}\\[1mm]
+ Sardana, Contrast, Hula};
+
+ \node[text width=20cm, below right] at (52,0) {{\huge Analysis}\\[1mm]
+   Event formation, Calibration, Corrections, Fitting, Azimuthal integration, $I_0$ normalisation,
+   Tomography angle augmentation, Sparsification, AI/ML alignment};
+
+ \node[below right] at (30,-3.5) {\huge Visualisation};
+
+ \node[below right] (det) at (22,0) {\huge Detectors};
+
+ \draw[-latex, line width=2mm] (8.5,-1.3) -- node[above]{ orchestration, triggers} +(12.5,0);
+ \draw[-latex, line width=2mm] (31,-1.3) -- node[above]{ unprocessed, separate data streams} +(20,0);
+
+ \draw[-latex, line width=2mm] (51,-4.8) -- node[above]{results} +(-10,0);
+
+ \draw[dash pattern=on 3cm off 1cm, line width=2mm] (29,-4.8) -| node[very near start, above]{scientist's interpretation} (-2,-3.5);
+
+ \draw[-latex,line width=2mm] (51,-7.2) -| node[near start, above]{automatic scanning decision} (-2,-3.5) |- (-1,-1.3);
+
+\end{tikzpicture}
+}
 
  % First block
 \begin{columns}
 
    % FIRST column
   \column{0.5}% Width set relative to text width
 
-  \block{Ingesters}{
-  Ingesters connect to different data sources, such as detectors, electrometers and encoders and form events according to the Trigger Map.
+  \block{Source Trigger Map}{
+  \textbf{Ingesters} connect to different data sources, such as detectors, electrometers and encoders and form events according to the Trigger Map.
   \bigskip
 
   \begin{minipage}{0.2\columnwidth}
   \begin{tikzpicture}[scale=2]
   \node (det1) at (0,0) {\faCamera};
   \node (mot) at (4,0) {\faSlidersH}; %\faCameraRetro};
   \node (temp) at (6,0) {\faThermometerHalf};
@@ -127,77 +152,70 @@
    \item STINS (2d detectors, multipart zmq PULL)
    \item PandABox PCAP (encoders, TCP/ascii)
    \item Contrast/Sardana (snapshots)
    \item Xspress3 (energy spectra, zmq SUB)
   \end{itemize}
 
  \end{minipage}
-
-  }
-
-   % SECOND column
-   % Second column with first block's top edge aligned with with previous column's top.
-
-   % Second column - first block
-   % Need to reset font, pretty ugly
-  \block{Trigger Map}{
-  Which \emph{frames} from which \emph{detectors} belong to the same \emph{event} and have to be processed by the same \emph{worker} with which \emph{tags}?
+\bigskip
+\coloredbox[bgcolor=blocktitlebgcolor, framecolor=blocktitlebgcolor]{
+ Which \emph{frames} from which \emph{detectors} belong to the same \emph{event} and have to be processed by the same \emph{worker} having which \emph{tags}?}
   \medskip
 
   \begin{center}
   \begin{tabular}{rccccccccc}
    \faCamera & all & 1 & \{3,debug\} & 5 & 7 & 8 & 10 & 10 & 11 \\
    \faVideo & all & 2 & \{4,debug\}  & 6 & 7 & 9 & 10 & 10 & 11 \\
    \faSlidersH & all & all & debug & none & $\emptyset$ &none & none& none & none\\
    \faThermometerHalf & all & \{1,2\} & none & \{5,6\} & none  & \{8,9\} & 10 & none & 11 \\
   \end{tabular}
   \end{center}
 
-  This supports detectors not producing a frame for a trigger (none) and discarding frames ($\emptyset$). Meta information is easily distributed to all workers by \emph{all}. Tags allow different sets of workers, the debug worker just exposes the last n events.
+  This supports detectors not producing a frame for a trigger (\emph{none}) and discarding frames ($\emptyset$). Meta information is easily distributed to all workers by \emph{all}. Tags allow different sets of workers, the \textbf{debug worker} just exposes the last n events.
 
   The trigger map is provided by the scanning software:
   \begin{description}
    \item[contrast:] patch after \texttt{\_generate\_positions}
    \item[sardana:] global hook to extract number of points
   \end{description}
 
 
   }
-  \block{Workers}{
-  Events are dispatched to the next free available worker satisfying the constraints and tags. The fine graind load balancing allows to keep state in the worker. This enables temporal analysis, e.g. calculate the difference of two consecutive exposures. All required parameters need to be described.
+  \block{Map Reduce}{
+  Events are dispatched to the \textbf{next free} available worker satisfying the constraints and tags. The fine grained \textbf{load balancing} allows to keep state in the worker. This enables \textbf{temporal analysis}, e.g. calculate the difference of two consecutive exposures. All required parameters need to be described.
   {\footnotesize
   \lstinputlisting[language=Python]{worker.py}
   }
-  Workers emit arbitrary objects as results. It is important that the output of all workers combined does not exceed a bottleneck of around 10\,Gbit/s.
-}
-  \block{Reducer}{
-  The results of workers are forwarded to a single reducer which has access to the full history of the scan. It has limited capacity and needs to operate at line speed which is fine for simple operations such as appending worker results to a list.
+  Workers emit arbitrary objects as reduced results. It is important that the output of all workers combined does not exceed a bottleneck of around 10\,Gbit/s.
+  \bigskip
+
+  The results of workers are forwarded to a \textbf{single reducer} which has access to the full history of the scan. It has limited capacity and needs to operate at line speed which is fine for simple operations such as appending worker results to a list.
   {\footnotesize
   \lstinputlisting[language=Python]{reducer.py}
   }
-  The reducer has a special attribute \emph{publish} which is exposed through a REST api with JsonPATH selections and numpy slicing.
+  The reducer has a special attribute \texttt{publish} which is exposed through a REST api with JsonPATH selections and numpy slicing.
   }
 
 
-  \block{Viewer}{
+  \block{Visualisation}{
   The most flexible way to view results is to access the reducer data through a Jupyter notebook.
 
 {\footnotesize
   \lstinputlisting[language=Python]{viewer.py}
   }
 
-  Alternatively a custom GUI may be developed which integrates setting parameters or selectively zooming into regions, if the whole data set is too large for the local memory.
+  Alternatively a custom GUI may be developed which integrates setting \textbf{parameters} or selectively zooming into regions, if the whole data set is too large for the local memory.
   }
 
 
   \column{0.5}
 
 
   \block{Control System Integration}{
-   A Tango device server presents the status of a pipeline and allows to set parameters. It shows which ingester streams are awailable and the load of workers, allowing to adjust the worker scaling. Pipeline parameters support \texttt{str}, \texttt{int}, \texttt{float} and \texttt{file}.
+   A Tango device server presents the status of a pipeline and allows to set parameters. It shows which ingester streams are available and the load of workers, allowing to adjust the worker \textbf{scaling}. Pipeline parameters support \texttt{str}, \texttt{int}, \texttt{float} and \texttt{file}.
    \medskip
 
    \footnotesize
    \begin{tabular}{ll}
     State & CLOSE \\
    Status & contrast-ingester, streams: ['contrast']\\
 &xspress3-ingester, streams: ['xspress3']\\
@@ -208,64 +226,69 @@
 totalEvents&134\\
 mca\_config & /data/xrf/fit\_config\_removed.cfg\\
 \end{tabular}
   }
 
   \block{Architecture \& Performance}{
 
-  \begin{tikzpicture}[yscale=2, xscale=3]
-  \node at (-2,1) {Detectors};
-  \node (det1) at (0,1) {\faCamera};
-  \node (mot) at (4,1) {\faSlidersH}; %\faCameraRetro};
-  \node (temp) at (6,1) {\faThermometerHalf};
-  \node (det2) at (2,1) {\faVideo};
-
-  \node[ left] at (-1,0) {custom zmq};
-  \node[left] at (-1,-2) {wrapped(custom zmq)};
-  \node[ left] at (-1,-4) {pickle in zmq};
-
-  \node at (-2,-1) {Event Formation};
+  \begin{tikzpicture}[yscale=2.389, xscale=3]
+  \node[left, color=gray] at (-1,1) {Detectors};
+  \node[color=gray] (det1) at (0,1) {\faCamera};
+  \node[color=gray] (mot) at (4,1) {\faSlidersH}; %\faCameraRetro};
+  \node[color=gray] (temp) at (6,1) {\faThermometerHalf};
+  \node[color=gray] (det2) at (2,1) {\faVideo};
+
+  \node[ left, color=blocktitlefgcolor] at (-1,0) {custom};
+  \node[left, color=blocktitlefgcolor] at (-1,-2) {wrapped(custom)};
+  \node[ left, color=blocktitlefgcolor] at (-1,-4) {\texttt{pickle} in zmq};
+
+  \node (redis) at (7.5,-3){\includegraphics[width=1.5cm]{redis}};
+  \node (fast) at (7.5,-1){\includegraphics[width=1.5cm]{fastapi}};
+  \node[left] at (-1,-1) {Ingesters};
   \node (ef1) at (0,-1) {\faHatWizard};
   \node (ef2) at (2,-1) {\faHatWizard};
   \node (ef) at (5,-1) {\faHatWizard};
 
   \draw[very thick] (det1.south) --  (ef1);
   \draw[very thick] (det2.south) -- (ef2);
   \draw (mot.south) -- (ef);
   \draw (temp.south) -- (ef);
 
 
-  \node at (-2,-3) {Workers};
+  \node[left] at (-1,-3) {Workers};
   \node (crop1) at (0,-3) {\faCrop};
   \node (crop4) at (3,-3) {\faCrop};
   \node (crop7) at (6,-3) {\faCrop};
 
   \foreach \i in {1,4,7} {
     \draw (ef.south) -- (crop\i.north);
     \draw (ef1.south) -- (crop\i.north);
     \draw (ef2.south) -- (crop\i.north);
   };
 
-  \node at (-2,-5) {Reduce};
+  \node[left] at (-1,-5) {Reduce};
   \node (red) at (3,-5) {\faCog};
 
 
   \foreach \i in {1,4,7} {
     \draw (crop\i.south) -- (red.north);
   };
   \newcommand{\labeloffset}{3mm}
 
   \node[above of=ef2, yshift=\labeloffset, fill=white] {\small PULL};
   \node[above of=ef1, yshift=\labeloffset, fill=white] {\small PULL};
   \node[above of=ef, yshift=\labeloffset, fill=white] {\small SUB};
 
-  \node[below of=det1, yshift=-\labeloffset, fill=white] {\small PUSH};
-  \node[below of=det2, yshift=-\labeloffset, fill=white] {\small PUSH};
-  \node[below of=mot, yshift=-\labeloffset, fill=white] {\small PUB};
-  \node[below of=temp, yshift=-\labeloffset, fill=white] {\small PUB};
+  \node[below of=redis, yshift=-\labeloffset, fill=white] {\small redis};
+  \node[below of=fast, yshift=-\labeloffset,] {\small controller};
+
+  \node[below of=det1, yshift=-\labeloffset,color=gray,  fill=white] {\small PUSH};
+  \node[below of=det2, yshift=-\labeloffset,color=gray,  fill=white] {\small PUSH};
+  \node[below of=mot, yshift=-\labeloffset,color=gray,  fill=white] {\small PUB};
+  \node[below of=temp, yshift=-\labeloffset,color=gray,  fill=white] {\small PUB};
 
   \node[below of=ef1, yshift=-\labeloffset, fill=white] {\small ROUTER};
   \node[below of=ef2, yshift=-\labeloffset, fill=white] {\small ROUTER};
   \node[below of=ef, yshift=-\labeloffset, fill=white] {\small ROUTER};
 
   \node[above of=crop1, yshift=\labeloffset, fill=white] {\small DEALER};
   \node[above of=crop4, yshift=\labeloffset, fill=white] {\small DEALER};
@@ -277,47 +300,38 @@
 
   \node[above of=red, yshift=\labeloffset, fill=white] {\small PULL};
  \end{tikzpicture}
 
  The throughput of the system is only limited by the underlying kernel and zmq library. With jumbo frames, we successfully processed a single stream of \textbf{23\,GBit/s} from a 16\,bit \texttt{cmos} camera at 120\,Hz.
     Affinity of ingesters heavily impacts performance.
 
-    The design allows arbitrary \textbf{horizontal scaling} for many ingesters. If a detector supports one stream per module, multiple ingesters are used to reassemble full frames for a worker. We tested up events at \textbf{2\,kHz}.
+    The design allows arbitrary \textbf{horizontal scaling} for many ingesters. If a detector supports one stream per module, multiple ingesters are used to reassemble full frames for a worker. We tested ingesting events at up to \textbf{2\,kHz}.
 
   }
 
   \block{Deployment}{
   If a kubernetes cluster is available, deployment is handled by a \texttt{helm} chart with values
 
 {\footnotesize
   \lstinputlisting[style=yaml]{Values.yaml}
   }
-  Without kubernetes, the only dependency is a \texttt{redis} to which all components can connect.
+  Without kubernetes, the only dependency is a \texttt{redis} to which all \textbf{containerised} components connect.
   }
 
 
   \block{Development \texttt{pip install dranspose}}{
    The package provides a \texttt{dranspose} cli to run components or develop scientific code.
     \begin{itemize}
      \item Ingesters dump stream messages to storage.
      \item Replay streams to custom workers and reducers.
     \end{itemize}
     To develop a new ingester, capture the raw packets and perform test-driven development.
     To get insight into live packets, a \textbf{debug worker} exposes sampled full events over a REST interface.
 
     Documentation at \url{https://dranspo.se/}
-  }
-
-  \block{Examples}{
-  \begin{itemize}
-   \item PyMCA fitting of concentration maps from fluorescence data.
-   \item Azimutal integration of diffraction images with $I_0$ normalisation.
-   \item Augmentation of camera frames with stage rotation angles for live tomographic reconstruction.
-   \item Image sparsification for \texttt{cmos} direct photon detection.
-  \end{itemize}
 
   }
 
 
 
 \end{columns}
```

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposter.cls` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposter.cls`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterBackgroundstyles.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterBackgroundstyles.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterBlockstyles.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterBlockstyles.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterColorpalettes.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterColorpalettes.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterColorstyles.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterColorstyles.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterInnerblockstyles.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterInnerblockstyles.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterLayoutthemes.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterLayoutthemes.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterNotestyles.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterNotestyles.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/poster-2024-01-15/tikzposterTitlestyles.tex` & `dranspose-0.0.3/docs/poster-2024-01-15/tikzposterTitlestyles.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/reference/trigger_map.md` & `dranspose-0.0.3/docs/reference/trigger_map.md`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/seminar-2023-11-30/main.tex` & `dranspose-0.0.3/docs/seminar-2023-11-30/main.tex`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/docs/tutorials/viewers.md` & `dranspose-0.0.3/docs/tutorials/viewers.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Live Viewers
 
 The reducer publishes data available for live viewing or to influence the scanning.
 
 To retrieve the data, the reducer exposes a HTTP interface. All data is available at
 
 ```
-/api/v1/result/
+/api/v1/result/$
 ```
 
 and returns pickle objects.
 
 However, if you are only interested in a subset of data for your specific live viewer,
 use [JSONpath](https://pypi.org/project/jsonpath-ng/#description) to select the specific data you need. To handle large numpy arrays better,
 there is a special filter `numpy()` which takes numpy slicing syntax.
```

### Comparing `dranspose-0.0.2/dranspose/cli.py` & `dranspose-0.0.3/dranspose/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import asyncio
+import json
 import logging
 import os
 import signal
 from asyncio import Task
 from typing import Literal, Any, Optional
 
 import uvicorn
@@ -134,15 +135,27 @@
 
 
 def reducer(args: argparse.Namespace) -> None:
     try:
         if args.reducerclass:
             os.environ["REDUCER_CLASS"] = args.reducerclass
         config = uvicorn.Config(
-            reducer_app, port=5000, host=args.host, log_level="info"
+            reducer_app, port=5002, host=args.host, log_level="info"
+        )
+        server = uvicorn.Server(config)
+        server.run()
+    except KeyboardInterrupt:
+        print("exiting")
+
+
+def http_ingester(args: argparse.Namespace) -> None:
+    try:
+        os.environ["INGESTER_STREAMS"] = json.dumps([args.name])
+        config = uvicorn.Config(
+            args.ingesterapp, port=args.port or 5000, host=args.host, log_level="info"
         )
         server = uvicorn.Server(config)
         server.run()
     except KeyboardInterrupt:
         print("exiting")
 
 
@@ -160,15 +173,23 @@
 
 
 def combined(args: argparse.Namespace) -> None:
     asyncio.run(main())
 
 
 def replay(args: argparse.Namespace) -> None:
-    run_replay(args.workerclass, args.reducerclass, args.files, args.parameters)
+    run_replay(
+        args.workerclass,
+        args.reducerclass,
+        args.files,
+        args.parameters,
+        args.port,
+        args.keep_alive,
+        args.nworkers,
+    )
 
 
 def create_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(prog="dranspose", description="Transposes Streams")
 
     subparsers = parser.add_subparsers(title="commands", dest="subcommand")
 
@@ -209,14 +230,27 @@
     parser_ingester.add_argument(
         "-u", "--upstream_url", help="Where to connect to upstream", required=True
     )
     parser_ingester.add_argument(
         "-n", "--name", help="Name of the ingester", required=True
     )
 
+    parser_http_ingester = subparsers.add_parser(
+        "http_ingester", help="run http ingester"
+    )
+    parser_http_ingester.set_defaults(func=http_ingester)
+    parser_http_ingester.add_argument("--host", help="host to listen on")
+    parser_http_ingester.add_argument(
+        "-c", "--ingesterapp", help="Ingester App", required=True
+    )
+    parser_http_ingester.add_argument("-p", "--port", help="Where to listen on")
+    parser_http_ingester.add_argument(
+        "-n", "--name", help="Name of the ingester", required=True
+    )
+
     parser_all = subparsers.add_parser(
         "combined", help="run all parts in a single process"
     )
     parser_all.set_defaults(func=combined)
 
     parser_replay = subparsers.add_parser(
         "replay", help="run replay of ingester recorded files"
@@ -236,14 +270,26 @@
     )
     parser_replay.add_argument(
         "-f", "--files", nargs="+", help="List of files to replay", required=True
     )
     parser_replay.add_argument(
         "-p", "--parameters", help="parameter file, json or pickle"
     )
+    parser_replay.add_argument(
+        "--port", type=int, help="expose the reducer result via http on port"
+    )
+    parser_replay.add_argument(
+        "--keep-alive", action="store_true", help="keep the server alive after finish"
+    )
+    parser_replay.add_argument(
+        "--nworkers",
+        help="number of workers to distribute events to",
+        default=1,
+        type=int,
+    )
 
     return parser
 
 
 def run() -> None:
     parser = create_parser()
     args: argparse.Namespace = parser.parse_args()
```

### Comparing `dranspose-0.0.2/dranspose/controller.py` & `dranspose-0.0.3/dranspose/controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 """
 This is the central service to orchestrate all distributed components
 
 """
 import asyncio
 from asyncio import Task
 from collections import defaultdict
+from types import UnionType
 from typing import Dict, List, Any, AsyncGenerator, Optional, Annotated, Literal
 
 import logging
 import time
 
 from pydantic import UUID4
 from starlette.requests import Request
 from starlette.responses import Response
 
 from dranspose.distributed import DistributedSettings
-from dranspose.helpers.utils import parameters_hash, done_callback
+from dranspose.helpers.utils import parameters_hash, done_callback, cancel_and_wait
 from dranspose.mapping import Mapping
 import redis.asyncio as redis
 import redis.exceptions as rexceptions
 
 from contextlib import asynccontextmanager
 from fastapi import FastAPI, HTTPException, Query
 
 from dranspose.parameters import (
     Parameter,
     ParameterType,
+    StrParameter,
+    ParameterBase,
 )
 from dranspose.protocol import (
     IngesterState,
     WorkerState,
     RedisKeys,
     EnsembleState,
     WorkerUpdate,
-    WorkerStateEnum,
+    DistributedStateEnum,
     WorkerName,
     StreamName,
     EventNumber,
     VirtualWorker,
     WorkParameter,
     ControllerUpdate,
     ReducerState,
     WorkerTimes,
     Digest,
     ParameterName,
     SystemLoadType,
     IntervalLoad,
     WorkerLoad,
+    DistributedUpdate,
+    ReducerUpdate,
+    IngesterUpdate,
+    WorkAssignmentList,
+    WorkAssignment,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class ControllerSettings(DistributedSettings):
     pass
@@ -66,26 +74,41 @@
             f"{self.settings.redis_dsn}?decode_responses=True&protocol=3"
         )
         self.mapping = Mapping({})
         self.mapping_update_lock = asyncio.Lock()
         self.parameters: dict[ParameterName, WorkParameter] = {}
         self.parameters_hash = parameters_hash(self.parameters)
         self.completed: dict[EventNumber, list[WorkerName]] = defaultdict(list)
+        self.to_reduce: set[tuple[EventNumber, WorkerName]] = set()
+        self.reduced: dict[EventNumber, list[WorkerName]] = defaultdict(list)
+        self.processed_event_no: int = 0
         self.completed_events: list[int] = []
+        self.finished_components: list[UnionType] = []
         self.assign_task: Task[None]
+        self.config_fetch_time: float = 0
+        self.config_cache: EnsembleState
+        self.default_task: Task[None]
+        self.consistent_task: Task[None]
         self.worker_timing: dict[
             WorkerName, dict[EventNumber, WorkerTimes]
         ] = defaultdict(dict)
+        self.start_time: float
 
     async def run(self) -> None:
         logger.debug("started controller run")
         self.assign_task = asyncio.create_task(self.assign_work())
         self.assign_task.add_done_callback(done_callback)
+        self.default_task = asyncio.create_task(self.default_parameters())
+        self.default_task.add_done_callback(done_callback)
+        self.consistent_task = asyncio.create_task(self.consistent_parameters())
+        self.consistent_task.add_done_callback(done_callback)
 
     async def get_configs(self) -> EnsembleState:
+        if time.time() - self.config_fetch_time < 0.5:
+            return self.config_cache
         async with self.redis.pipeline() as pipe:
             await pipe.keys(RedisKeys.config("ingester"))
             await pipe.keys(RedisKeys.config("worker"))
             ingester_keys, worker_keys = await pipe.execute()
         async with self.redis.pipeline() as pipe:
             await pipe.mget(ingester_keys)
             await pipe.mget(worker_keys)
@@ -93,15 +116,19 @@
             ingester_json, worker_json, reducer_json = await pipe.execute()
 
         ingesters = [IngesterState.model_validate_json(i) for i in ingester_json]
         workers = [WorkerState.model_validate_json(w) for w in worker_json]
         reducer = None
         if reducer_json:
             reducer = ReducerState.model_validate_json(reducer_json)
-        return EnsembleState(ingesters=ingesters, workers=workers, reducer=reducer)
+        self.config_cache = EnsembleState(
+            ingesters=ingesters, workers=workers, reducer=reducer
+        )
+        self.config_fetch_time = time.time()
+        return self.config_cache
 
     async def get_load(self, intervals: list[int], scan: bool = True) -> SystemLoadType:
         ret = {}
         for wn, wt in self.worker_timing.items():
             last_event = max(wt.keys())
             itval: dict[int | Literal["scan"], IntervalLoad] = {}
             for interval in intervals:
@@ -125,15 +152,15 @@
                 )
             ret[wn] = WorkerLoad(last_event=last_event, intervals=itval)
         return ret
 
     async def set_mapping(self, m: Mapping) -> None:
         async with self.mapping_update_lock:
             logger.debug("cancelling assign task")
-            self.assign_task.cancel()
+            await cancel_and_wait(self.assign_task)
             logger.debug(
                 "deleting keys %s and %s",
                 RedisKeys.ready(self.mapping.uuid),
                 RedisKeys.assigned(self.mapping.uuid),
             )
             await self.redis.delete(RedisKeys.ready(self.mapping.uuid))
             await self.redis.delete(RedisKeys.assigned(self.mapping.uuid))
@@ -166,14 +193,15 @@
     async def set_param(self, name: ParameterName, data: bytes) -> Digest:
         param = WorkParameter(name=name, data=data)
         logger.debug("distributing parameter %s with uuid %s", param.name, param.uuid)
         await self.redis.set(RedisKeys.parameters(name, param.uuid), param.data)
         self.parameters[name] = param
         logger.debug("stored parameters")
         self.parameters_hash = parameters_hash(self.parameters)
+        logger.debug("parameter hash is now %s", self.parameters_hash)
         cupd = ControllerUpdate(
             mapping_uuid=self.mapping.uuid,
             parameters_version={n: p.uuid for n, p in self.parameters.items()},
         )
         logger.debug("send update %s", cupd)
         await self.redis.xadd(
             RedisKeys.updates(),
@@ -186,95 +214,237 @@
         param_json = await self.redis.mget(desc_keys)
 
         params: list[ParameterType] = []
         for i in param_json:
             val: ParameterType = Parameter.validate_json(i)  # type: ignore
             params.append(val)
 
+        params.append(
+            StrParameter(
+                name=ParameterName("dump_prefix"),
+                description="Prefix to dump ingester values",
+            )
+        )
         return sorted(params, key=lambda x: x.name)
 
+    async def default_parameters(self) -> None:
+        while True:
+            try:
+                desc_keys = await self.redis.keys(RedisKeys.parameter_description())
+                param_json = await self.redis.mget(desc_keys)
+                for i in param_json:
+                    val: ParameterType = Parameter.validate_json(i)  # type: ignore
+                    if val.name not in self.parameters:
+                        logger.info(
+                            "set parameter %s to default %s", val.name, val.default
+                        )
+                        await self.set_param(
+                            val.name, ParameterBase.to_bytes(val.default)
+                        )
+                await asyncio.sleep(2)
+            except asyncio.exceptions.CancelledError:
+                break
+
+    async def consistent_parameters(self) -> None:
+        while True:
+            try:
+                consistent = True
+                cfg = await self.get_configs()
+                if cfg.reducer and cfg.reducer.parameters_hash != self.parameters_hash:
+                    consistent = False
+                for wo in cfg.workers:
+                    if wo.parameters_hash != self.parameters_hash:
+                        consistent = False
+                for ing in cfg.ingesters:
+                    if ing.parameters_hash != self.parameters_hash:
+                        consistent = False
+
+                if not consistent:
+                    logger.info(
+                        "inconsistent parameters, redistribute hash %s",
+                        self.parameters_hash,
+                    )
+                    cupd = ControllerUpdate(
+                        mapping_uuid=self.mapping.uuid,
+                        parameters_version={
+                            n: p.uuid for n, p in self.parameters.items()
+                        },
+                        target_parameters_hash=self.parameters_hash,
+                    )
+                    logger.debug("send consistency update %s", cupd)
+                    await self.redis.xadd(
+                        RedisKeys.updates(),
+                        {"data": cupd.model_dump_json()},
+                    )
+                await asyncio.sleep(2)
+            except asyncio.exceptions.CancelledError:
+                break
+
+    async def _update_processing_times(self, update: WorkerUpdate) -> None:
+        if update.completed is None:
+            return
+        if update.processing_times:
+            self.worker_timing[update.worker][
+                update.completed[-1]
+            ] = update.processing_times
+        for compev, has_result in zip(update.completed, update.has_result):
+            self.completed[compev].append(update.worker)
+            logger.debug("added completed to set %s", self.completed)
+            wa = self.mapping.get_event_workers(compev)
+            if wa.get_all_workers() == set(self.completed[compev]):
+                self.completed_events.append(compev)
+            if has_result:
+                toadd = True
+                if compev in self.reduced:
+                    logger.debug(
+                        "events %s already received from reducer", self.reduced
+                    )
+                    if update.worker in self.reduced[compev]:
+                        # process worker update very late and already got reduced
+                        logger.debug(
+                            "event %s from worker %s was already reduced",
+                            compev,
+                            update.worker,
+                        )
+                        toadd = False
+                if toadd:
+                    logger.debug(
+                        "waiting for reduction for event %s from worker %s",
+                        compev,
+                        update.worker,
+                    )
+                    self.to_reduce.add((compev, update.worker))
+        # logger.error("time processtime %s", time.perf_counter() - start)
+
+    async def assign_worker_in_mapping(
+        self, worker: WorkerName, completed: EventNumber
+    ) -> None:
+        cfg = await self.get_configs()
+        # logger.error("time cfg %s", time.perf_counter() - start)
+        logger.debug(
+            "assigning worker %s with all %s",
+            worker,
+            [ws.name for ws in cfg.workers],
+        )
+        virt = self.mapping.assign_next(
+            next(w for w in cfg.workers if w.name == worker),
+            cfg.workers,
+            completed=completed,
+            horizon=5,
+        )
+        # logger.error("time assign %s", time.perf_counter() - start)
+        logger.debug("assigned worker %s to %s", worker, virt)
+        logger.debug(
+            "send out complete events in range(%d, %d)",
+            self.processed_event_no,
+            self.mapping.complete_events,
+        )
+        assignments: list[WorkAssignment] = []
+        for evn in range(self.processed_event_no, self.mapping.complete_events):
+            wrks = self.mapping.get_event_workers(EventNumber(evn))
+            assignments.append(wrks)
+            if wrks.get_all_workers() == set():
+                self.completed[wrks.event_number] = []
+                self.completed_events.append(wrks.event_number)
+            if evn % 1000 == 0:
+                logger.info(
+                    "1000 events in %lf",
+                    time.perf_counter() - self.start_time,
+                )
+                self.start_time = time.perf_counter()
+        if len(assignments) > 0:
+            await self.redis.xadd(
+                RedisKeys.assigned(self.mapping.uuid),
+                {"data": WorkAssignmentList.dump_json(assignments)},
+            )
+
+        # logger.error("time sent out %s", time.perf_counter() - start)
+        self.processed_event_no = self.mapping.complete_events
+
+    async def _process_worker_update(self, update: WorkerUpdate) -> None:
+        logger.debug("got a ready worker %s", update)
+        if update.state == DistributedStateEnum.READY:
+            await self.assign_worker_in_mapping(update.worker, EventNumber(0))
+        if update.state == DistributedStateEnum.IDLE:
+            # start = time.perf_counter()
+            await self.assign_worker_in_mapping(update.worker, update.completed[-1])
+
+            asyncio.create_task(self._update_processing_times(update))
+
+    async def completed_finish(self) -> bool:
+        fin_workers = set()
+        reducer = False
+        fin_ingesters = set()
+        for upd in self.finished_components:
+            if isinstance(upd, WorkerUpdate):
+                fin_workers.add(upd.worker)
+            elif isinstance(upd, ReducerUpdate):
+                reducer = True
+            elif isinstance(upd, IngesterUpdate):
+                fin_ingesters.add(upd.ingester)
+
+        cfgs = await self.get_configs()
+
+        return (
+            set([w.name for w in cfgs.workers]) == fin_workers
+            and set([i.name for i in cfgs.ingesters]) == fin_ingesters
+            and reducer
+        )
+
     async def assign_work(self) -> None:
         last = 0
-        event_no = 0
+        self.processed_event_no = 0
         self.completed = defaultdict(list)
+        self.reduced = defaultdict(list)
         self.completed_events = []
+        self.to_reduce = set()
+        self.finished_components = []
         self.worker_timing = defaultdict(dict)
         notify_finish = True
-        start = time.perf_counter()
+        self.start_time = time.perf_counter()
         while True:
             try:
                 workers = await self.redis.xread(
                     {RedisKeys.ready(self.mapping.uuid): last},
                     block=1000,
                 )
                 if RedisKeys.ready(self.mapping.uuid) in workers:
                     for ready in workers[RedisKeys.ready(self.mapping.uuid)][0]:
-                        update = WorkerUpdate.model_validate_json(ready[1]["data"])
-                        logger.debug("got a ready worker %s", update)
-                        if update.state == WorkerStateEnum.IDLE:
-                            cfg = await self.get_configs()
-                            logger.debug(
-                                "assigning worker %s with all %s",
-                                update.worker,
-                                [ws.name for ws in cfg.workers],
-                            )
-                            virt = self.mapping.assign_next(
-                                next(w for w in cfg.workers if w.name == update.worker),
-                                cfg.workers,
-                            )
-                            if not update.new:
-                                if update.processing_times:
-                                    self.worker_timing[update.worker][
-                                        update.completed
-                                    ] = update.processing_times
+                        update = DistributedUpdate.validate_json(ready[1]["data"])
+                        if isinstance(update, WorkerUpdate):
+                            await self._process_worker_update(update)
+                        elif isinstance(update, ReducerUpdate):
+                            if (
+                                update.completed is not None
+                                and update.worker is not None
+                            ):
                                 compev = update.completed
-                                self.completed[compev].append(update.worker)
-                                logger.debug(
-                                    "added completed to set %s", self.completed
-                                )
-                                wa = self.mapping.get_event_workers(compev)
-                                if wa.get_all_workers() == set(self.completed[compev]):
-                                    self.completed_events.append(compev)
-                            logger.debug(
-                                "assigned worker %s to %s", update.worker, virt
-                            )
-                            async with self.redis.pipeline() as pipe:
-                                logger.debug(
-                                    "send out complete events in range(%d, %d)",
-                                    event_no,
-                                    self.mapping.complete_events,
-                                )
-                                for evn in range(
-                                    event_no, self.mapping.complete_events
-                                ):
-                                    wrks = self.mapping.get_event_workers(
-                                        EventNumber(evn)
-                                    )
-                                    await pipe.xadd(
-                                        RedisKeys.assigned(self.mapping.uuid),
-                                        {"data": wrks.model_dump_json()},
-                                        id=evn + 1,
-                                    )
-                                    if evn % 1000 == 0:
-                                        logger.info(
-                                            "1000 events in %lf",
-                                            time.perf_counter() - start,
-                                        )
-                                        start = time.perf_counter()
-                                await pipe.execute()
-                            event_no = self.mapping.complete_events
+                                self.reduced[compev].append(update.worker)
+                                logger.debug("added reduced to set %s", self.reduced)
+                                if (compev, update.worker) in self.to_reduce:
+                                    self.to_reduce.remove((compev, update.worker))
+                        elif isinstance(update, IngesterUpdate):
+                            pass
+
+                        if hasattr(update, "state"):
+                            if update.state == DistributedStateEnum.FINISHED:
+                                logger.info("distributed %s has finished", update)
+                                self.finished_components.append(update)
+
                         last = ready[0]
                 logger.debug(
-                    "checking if finished, completed %d, len %d",
+                    "checking if finished, completed %d, len %d, to_reduce %s",
                     len(self.completed_events),
                     self.mapping.len(),
+                    self.to_reduce,
                 )
                 if (
                     len(self.completed_events) > 0
                     and len(self.completed_events) == self.mapping.len()
+                    and len(self.to_reduce) == 0
                     and notify_finish
                 ):
                     # all events done, send close
                     cupd = ControllerUpdate(
                         mapping_uuid=self.mapping.uuid,
                         parameters_version={
                             n: p.uuid for n, p in self.parameters.items()
@@ -287,14 +457,16 @@
                         {"data": cupd.model_dump_json()},
                     )
                     notify_finish = False
             except rexceptions.ConnectionError:
                 break
 
     async def close(self) -> None:
+        await cancel_and_wait(self.default_task)
+        await cancel_and_wait(self.consistent_task)
         await self.redis.delete(RedisKeys.updates())
         queues = await self.redis.keys(RedisKeys.ready("*"))
         if len(queues) > 0:
             await self.redis.delete(*queues)
         assigned = await self.redis.keys(RedisKeys.assigned("*"))
         if len(assigned) > 0:
             await self.redis.delete(*assigned)
@@ -311,15 +483,15 @@
 async def lifespan(app: FastAPI) -> AsyncGenerator[None, None]:
     # Load the ML model
     global ctrl
     ctrl = Controller()
     run_task = asyncio.create_task(ctrl.run())
     run_task.add_done_callback(done_callback)
     yield
-    run_task.cancel()
+    await cancel_and_wait(run_task)
     await ctrl.close()
     # Clean up the ML models and release the resources
 
 
 app = FastAPI(lifespan=lifespan)
 
 
@@ -333,15 +505,15 @@
 async def get_status() -> dict[str, Any]:
     global ctrl
     return {
         "work_completed": ctrl.completed,
         "last_assigned": ctrl.mapping.complete_events,
         "assignment": ctrl.mapping.assignments,
         "completed_events": ctrl.completed_events,
-        "finished": len(ctrl.completed_events) == ctrl.mapping.len(),
+        "finished": await ctrl.completed_finish(),
         "processing_times": ctrl.worker_timing,
     }
 
 
 @app.get("/api/v1/load")
 async def get_load(
     intervals: Annotated[list[int] | None, Query()] = None, scan: bool = True
@@ -355,32 +527,45 @@
 @app.get("/api/v1/progress")
 async def get_progress() -> dict[str, Any]:
     global ctrl
     return {
         "last_assigned": ctrl.mapping.complete_events,
         "completed_events": len(ctrl.completed_events),
         "total_events": ctrl.mapping.len(),
-        "finished": len(ctrl.completed_events) == ctrl.mapping.len(),
+        "finished": await ctrl.completed_finish(),
     }
 
 
 @app.post("/api/v1/mapping")
 async def set_mapping(
     mapping: Dict[StreamName, List[Optional[List[VirtualWorker]]]],
     all_wrap: bool = True,
 ) -> UUID4 | str:
     global ctrl
     config = await ctrl.get_configs()
     if set(mapping.keys()) - set(config.get_streams()) != set():
-        return (
-            f"streams {set(mapping.keys()) - set(config.get_streams())} not available"
+        logger.warning(
+            "bad request streams %s not available",
+            set(mapping.keys()) - set(config.get_streams()),
+        )
+        raise HTTPException(
+            status_code=400,
+            detail=f"streams {set(mapping.keys()) - set(config.get_streams())} not available",
         )
     m = Mapping(mapping, add_start_end=all_wrap)
     if len(config.workers) < m.min_workers():
-        return f"only {len(config.workers)} workers available, but {m.min_workers()} required"
+        logger.warning(
+            "only %d workers available, but %d required",
+            len(config.workers),
+            m.min_workers(),
+        )
+        raise HTTPException(
+            status_code=400,
+            detail=f"only {len(config.workers)} workers available, but {m.min_workers()} required",
+        )
     await ctrl.set_mapping(m)
     return m.uuid
 
 
 @app.get("/api/v1/mapping")
 async def get_mapping() -> Dict[StreamName, List[Optional[List[VirtualWorker]]]]:
     global ctrl
```

### Comparing `dranspose-0.0.2/dranspose/data/contrast.py` & `dranspose-0.0.3/dranspose/data/contrast.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/data/xspress3.py` & `dranspose-0.0.3/dranspose/data/xspress3.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/debug_worker.py` & `dranspose-0.0.3/dranspose/debug_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,55 +6,47 @@
 from typing import AsyncGenerator, Any
 
 import zmq
 from fastapi import FastAPI
 from starlette.responses import Response
 
 from dranspose.event import EventData
-from dranspose.helpers.utils import done_callback
-from dranspose.protocol import WorkerUpdate, WorkerStateEnum, RedisKeys
-from dranspose.worker import Worker, RedisException
+from dranspose.helpers.utils import done_callback, cancel_and_wait
+from dranspose.protocol import WorkerUpdate, DistributedStateEnum, RedisKeys
+from dranspose.worker import Worker
 
 logger = logging.getLogger(__name__)
 
 
 class DebugWorker(Worker):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.buffer: deque[EventData] = deque(maxlen=50)
 
     async def work(self) -> None:
         self._logger.info("started work task")
         await self.notify_worker_ready()
 
-        lastev = "0"
         while True:
-            try:
-                newlastev, ingesterset = await self.get_new_assignments(lastev)
-                if newlastev is None or ingesterset is None:
-                    continue
-                lastev = newlastev
-            except RedisException:
-                self._logger.warning("failed to access redis, exiting worker")
-                break
-
-            if len(ingesterset) == 0:
-                continue
+            self.dequeue_task = None
+            self.dequeue_task = asyncio.create_task(self.assignment_queue.get())
+            ingesterset = await self.dequeue_task
             done = await self.poll_internals(ingesterset)
             if set(done) != {zmq.POLLIN}:
                 self._logger.warning("not all sockets are pollIN %s", done)
                 continue
 
             event = await self.build_event(ingesterset)
             self._logger.debug("adding event %s to buffer", event)
             self.buffer.append(event)
 
             wu = WorkerUpdate(
-                state=WorkerStateEnum.IDLE,
-                completed=event.event_number,
+                state=DistributedStateEnum.IDLE,
+                completed=[event.event_number],
+                has_result=[False],
                 worker=self.state.name,
             )
             await self.redis.xadd(
                 RedisKeys.ready(self.state.mapping_uuid),
                 {"data": wu.model_dump_json()},
             )
             self.state.processed_events += 1
@@ -67,15 +59,15 @@
 async def lifespan(app: FastAPI) -> AsyncGenerator[None, None]:
     # Load the ML model
     global worker
     worker = DebugWorker()
     run_task = asyncio.create_task(worker.run())
     run_task.add_done_callback(done_callback)
     yield
-    run_task.cancel()
+    await cancel_and_wait(run_task)
     await worker.close()
     # Clean up the ML models and release the resources
 
 
 app = FastAPI(lifespan=lifespan)
```

### Comparing `dranspose-0.0.2/dranspose/distributed.py` & `dranspose-0.0.3/dranspose/distributed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import abc
 import logging
-from typing import Optional
+import time
+from typing import Optional, Any
 
 import redis.asyncio as redis
 from pydantic import UUID4, AliasChoices, Field, RedisDsn
 from pydantic_core import Url
 from pydantic_settings import BaseSettings
 
-from dranspose.helpers.utils import parameters_hash
+from dranspose.helpers.utils import parameters_hash, cancel_and_wait
+from dranspose.parameters import Parameter, ParameterType
 from dranspose.protocol import (
     RedisKeys,
     ControllerUpdate,
     IngesterState,
     WorkerState,
     ReducerState,
     ParameterName,
@@ -59,30 +61,32 @@
         )
         self.raw_redis = redis.from_url(
             f"{self._distributed_settings.redis_dsn}?protocol=3"
         )
         self._logger = logging.getLogger(f"{__name__}+{self.state.name}")
         self.parameters: dict[ParameterName, WorkParameter] = {}
 
+    def get_category(self) -> str:
+        if isinstance(self.state, IngesterState):
+            category = "ingester"
+        elif isinstance(self.state, WorkerState):
+            category = "worker"
+        elif isinstance(self.state, ReducerState):
+            category = "reducer"
+        else:
+            raise NotImplementedError(
+                "Distributed Service not implemented for your Service"
+            )
+        return category
+
     async def publish_config(self) -> None:
         self._logger.debug("publish config %s", self.state)
         async with self.redis.pipeline() as pipe:
-            if isinstance(self.state, IngesterState):
-                category = "ingester"
-            elif isinstance(self.state, WorkerState):
-                category = "worker"
-            elif isinstance(self.state, ReducerState):
-                category = "reducer"
-            else:
-                raise NotImplementedError(
-                    "Distributed Service not implemented for your Service"
-                )
-
             await pipe.setex(
-                RedisKeys.config(category, self.state.name),
+                RedisKeys.config(self.get_category(), self.state.name),
                 10,
                 self.state.model_dump_json(),
             )
             if hasattr(self, "param_descriptions"):
                 for p in self.param_descriptions:
                     self._logger.debug("register parameter %s", p)
                     try:
@@ -134,39 +138,91 @@
                             try:
                                 params = await self.raw_redis.get(
                                     RedisKeys.parameters(name, paramuuids[name])
                                 )
                                 self._logger.debug(
                                     "received binary parameters for %s", name
                                 )
-                                if params:
+                                if params is not None:
                                     self._logger.info(
                                         "set parameter %s of length %s",
                                         name,
                                         len(params),
                                     )
                                     self.parameters[name] = WorkParameter(
                                         name=name, uuid=paramuuids[name], data=params
                                     )
+                                    # check if this parameter has a description and type
+                                    desc = await self.redis.get(
+                                        RedisKeys.parameter_description(name),
+                                    )
+                                    self._logger.debug("description is %s", desc)
+                                    if desc:
+                                        param_desc: ParameterType = Parameter.validate_json(desc)  # type: ignore
+                                        self._logger.info(
+                                            "set paremter has a description %s",
+                                            param_desc,
+                                        )
+                                        self.parameters[
+                                            name
+                                        ].value = param_desc.from_bytes(params)
+                                        self._logger.debug(
+                                            "parsed parameter value %s",
+                                            self.parameters[name].value,
+                                        )
                             except Exception as e:
                                 self._logger.error(
                                     "failed to get parameters %s", e.__repr__()
                                 )
                     self.state.parameters_hash = parameters_hash(self.parameters)
+                    self._logger.debug(
+                        "set local parameters to %s with hash %s",
+                        {n: p.uuid for n, p in self.parameters.items()},
+                        self.state.parameters_hash,
+                    )
                     if update.finished:
                         self._logger.info("finished messages")
                         await self.finish_work()
 
             except rexceptions.ConnectionError:
                 break
             except asyncio.exceptions.CancelledError:
                 break
 
+    async def multiprocess_run(self, queue: Any) -> None:
+        task = asyncio.create_task(self.run())
+        loop = asyncio.get_event_loop()
+        await loop.run_in_executor(None, queue.get)
+        await self.close()
+        await cancel_and_wait(task)
+
+    def sync_run(self, queue: Any) -> None:
+        asyncio.run(self.multiprocess_run(queue))
+
+    async def update_metrics(self) -> None:
+        while True:
+            start = time.time()
+            old = self.state.processed_events
+            await asyncio.sleep(1.0)
+            end = time.time()
+            if (self.state.processed_events - old) > 0:
+                rate = (self.state.processed_events - old) / (end - start)
+                self.state.event_rate = rate
+                self._logger.info("receiving %lf frames per second", rate)
+
+    async def run(self) -> None:
+        pass
+
     async def restart_work(self, uuid: UUID4) -> None:
         pass
 
     async def finish_work(self) -> None:
         pass
 
     async def close(self) -> None:
+        await self.redis.delete(RedisKeys.config(self.get_category(), self.state.name))
+        self._logger.info(
+            "deleted redis key %s",
+            RedisKeys.config(self.get_category(), self.state.name),
+        )
         await self.redis.aclose()
         await self.raw_redis.aclose()
```

### Comparing `dranspose-0.0.2/dranspose/event.py` & `dranspose-0.0.3/dranspose/event.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/helpers/jsonpath_slice_ext.py` & `dranspose-0.0.3/dranspose/helpers/jsonpath_slice_ext.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/helpers/utils.py` & `dranspose-0.0.3/dranspose/helpers/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import hashlib
 import importlib
 import logging
 import os
 import sys
 import traceback
-from asyncio import Future
+from asyncio import Future, Task
+from typing import Any
 
 from dranspose.protocol import Digest, WorkParameter, ParameterName
 
 
 def import_class(path: str) -> type:
     sys.path.append(os.getcwd())
     module = importlib.import_module(path.split(":")[0])
@@ -31,7 +32,19 @@
         pass
     except Exception as e:
         logging.error(
             "subroutine crashed %s trace: %s",
             e.__repr__(),
             traceback.format_exc(),
         )
+
+
+async def cancel_and_wait(task: Task[Any] | Future[Any]) -> None:
+    task.cancel()
+    try:
+        await task
+    except asyncio.CancelledError:
+        pass
+    except StopIteration:
+        pass
+    except Exception as e:
+        logging.error("cancel and wait task raised %s", e.__repr__())
```

### Comparing `dranspose-0.0.2/dranspose/ingester.py` & `dranspose-0.0.3/dranspose/ingester.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import asyncio
+import time
 import os
 import pickle
 from typing import AsyncGenerator, Optional, Awaitable, Any, IO
+from uuid import UUID
 
 import redis.exceptions as rexceptions
 import zmq.asyncio
 
 from pydantic import UUID4, model_validator
 
 from dranspose.distributed import DistributedService, DistributedSettings
 from dranspose.event import StreamData, InternalWorkerMessage
-from dranspose.helpers.utils import done_callback
+from dranspose.helpers.utils import done_callback, cancel_and_wait
 from dranspose.protocol import (
     IngesterState,
     StreamName,
     RedisKeys,
     WorkAssignment,
     IngesterName,
     ZmqUrl,
+    ParameterName,
+    ConnectedWorker,
+    IngesterUpdate,
+    DistributedStateEnum,
+    WorkAssignmentList,
 )
 
 
 class IngesterSettings(DistributedSettings):
     ingester_streams: list[StreamName]
     ingester_name: IngesterName
     ingester_url: ZmqUrl = ZmqUrl("tcp://localhost:10000")
@@ -62,44 +69,50 @@
             state,
             self._ingester_settings,
         )
         self.state: IngesterState
 
         self.dump_file: Optional[IO[bytes]] = None
 
+    def open_socket(self) -> None:
         self.ctx = zmq.asyncio.Context()
         self.out_socket = self.ctx.socket(zmq.ROUTER)
         self.out_socket.setsockopt(zmq.ROUTER_MANDATORY, 1)
         self.out_socket.setsockopt(zmq.TCP_KEEPALIVE, 1)
         self.out_socket.setsockopt(zmq.TCP_KEEPALIVE_IDLE, 300)
         self.out_socket.setsockopt(zmq.TCP_KEEPALIVE_INTVL, 300)
         self.out_socket.bind(f"tcp://*:{self._ingester_settings.ingester_url.port}")
 
     async def run(self) -> None:
         """
         Main function orchestrating the dependent tasks. This needs to be called from an async context once an instance is created.
         """
+        self.open_socket()
+
         self.accept_task = asyncio.create_task(self.accept_workers())
         self.accept_task.add_done_callback(done_callback)
         self.work_task = asyncio.create_task(self.work())
         self.work_task.add_done_callback(done_callback)
         self.assign_task = asyncio.create_task(self.manage_assignments())
         self.assign_task.add_done_callback(done_callback)
         self.assignment_queue: asyncio.Queue[WorkAssignment] = asyncio.Queue()
+        self.metrics_task = asyncio.create_task(self.update_metrics())
+        self.metrics_task.add_done_callback(done_callback)
+        self._logger.info("all subtasks running")
         await self.register()
 
     async def restart_work(self, new_uuid: UUID4) -> None:
         """
         Restarts all work related tasks to make sure no old state is present in a new scan.
 
         Arguments:
             new_uuid: The uuid of the new mapping
         """
-        self.work_task.cancel()
-        self.assign_task.cancel()
+        await cancel_and_wait(self.work_task)
+        await cancel_and_wait(self.assign_task)
         self.state.mapping_uuid = new_uuid
         self.assignment_queue = asyncio.Queue()
         self.work_task = asyncio.create_task(self.work())
         self.work_task.add_done_callback(done_callback)
         self.assign_task = asyncio.create_task(self.manage_assignments())
         self.assign_task.add_done_callback(done_callback)
 
@@ -109,14 +122,24 @@
         """
         self._logger.info("finishing work")
         if self.dump_file:
             self.dump_file.close()
             self._logger.info("closed dump file at finish %s", self.dump_file)
             self.dump_file = None
 
+        await self.redis.xadd(
+            RedisKeys.ready(self.state.mapping_uuid),
+            {
+                "data": IngesterUpdate(
+                    state=DistributedStateEnum.FINISHED,
+                    ingester=self.state.name,
+                ).model_dump_json()
+            },
+        )
+
     async def manage_assignments(self) -> None:
         """
         A background task reading assignments from the controller, filering them for the relevant ones and enqueueing them for when the frame arrives.
         """
         self._logger.info("started ingester manage assign task")
         lastev = 0
         while True:
@@ -126,54 +149,67 @@
             except rexceptions.ConnectionError:
                 break
             if sub not in assignments:
                 continue
             assignment_evs = assignments[sub][0]
             self._logger.debug("got assignments %s", assignment_evs)
             for assignment in assignment_evs:
-                wa = WorkAssignment.model_validate_json(assignment[1]["data"])
-                mywa = wa.get_workers_for_streams(self.state.streams)
-                await self.assignment_queue.put(mywa)
+                was = WorkAssignmentList.validate_json(assignment[1]["data"])
+                for wa in was:
+                    mywa = wa.get_workers_for_streams(self.state.streams)
+                    await self.assignment_queue.put(mywa)
                 lastev = assignment[0]
 
     async def work(self) -> None:
         """
         The heavy liftig function of an ingester. It consumes a generator `run_source()` which
         should be implemented for a specific protocol.
         It then assembles all streams for this ingester and forwards them to the assigned workers.
 
         Optionally the worker dumps the internal messages to disk. This is useful to develop workers with actual data captured.
         """
         self._logger.info("started ingester work task")
         sourcegens = {stream: self.run_source(stream) for stream in self.state.streams}
         self.dump_file = None
-        if self._ingester_settings.dump_path:
-            self.dump_file = open(self._ingester_settings.dump_path, "ab")
+        self.dump_filename = self._ingester_settings.dump_path
+        if self.dump_filename is None and "dump_prefix" in self.parameters:
+            val = self.parameters[ParameterName("dump_prefix")].data.decode("utf8")
+            if len(val) > 0:
+                self.dump_filename = f"{val}{self._ingester_settings.ingester_name}-{self.state.mapping_uuid}.pkls"
+        if self.dump_filename:
+            self.dump_file = open(self.dump_filename, "ab")
             self._logger.info(
                 "dump file %s opened at %s",
-                self._ingester_settings.dump_path,
+                self.dump_filename,
                 self.dump_file,
             )
         try:
+            took = []
+            empties = []
             while True:
+                empty = False
+                if self.assignment_queue.empty():
+                    empty = True
+                start = time.perf_counter()
                 work_assignment: WorkAssignment = await self.assignment_queue.get()
+                if empty:
+                    empties.append(work_assignment.event_number)
+
                 workermessages = {}
                 zmqyields: list[Awaitable[StreamData]] = []
                 streams: list[StreamName] = []
                 for stream in work_assignment.assignments:
                     zmqyields.append(anext(sourcegens[stream]))
                     streams.append(stream)
                 zmqstreams: list[StreamData] = await asyncio.gather(*zmqyields)
                 zmqparts: dict[StreamName, StreamData] = {
                     stream: zmqpart for stream, zmqpart in zip(streams, zmqstreams)
                 }
                 if self.dump_file:
-                    self._logger.debug(
-                        "writing dump to path %s", self._ingester_settings.dump_path
-                    )
+                    self._logger.debug("writing dump to path %s", self.dump_filename)
                     allstr = InternalWorkerMessage(
                         event_number=work_assignment.event_number,
                         streams={k: v.get_bytes() for k, v in zmqparts.items()},
                     )
                     try:
                         pickle.dump(allstr, self.dump_file)
                     except Exception as e:
@@ -200,24 +236,37 @@
                             message.model_dump_json(
                                 exclude={"streams": {"__all__": "frames"}}
                             ).encode("utf8")
                         ]
                         + message.get_all_frames()
                     )
                     self._logger.debug("sent message to worker %s", worker)
+                end = time.perf_counter()
+                took.append(end - start)
+                if len(took) > 1000:
+                    self._logger.info(
+                        "forwarding took avg %lf, min %f max %f",
+                        sum(took) / len(took),
+                        min(took),
+                        max(took),
+                    )
+                    self._logger.info("waiting for queue %d of 1000", len(empties))
+                    took = []
+                    empties = []
                 self.state.processed_events += 1
         except asyncio.exceptions.CancelledError:
             self._logger.info("stopping worker")
             for stream in self.state.streams:
                 await self.stop_source(stream)
             if self.dump_file:
                 self._logger.info(
                     "closing dump file %s at cancelled work", self.dump_file
                 )
                 self.dump_file.close()
+                self.dump_file = None
 
     async def run_source(self, stream: StreamName) -> AsyncGenerator[StreamData, None]:
         """
         This generator must be implemented by the customised subclass. It should return exactly one `StreamData` object
         for every frame arriving from upstream.
 
         Arguments:
@@ -239,19 +288,39 @@
         """
         poller = zmq.asyncio.Poller()
         poller.register(self.out_socket, zmq.POLLIN)
         while True:
             socks = dict(await poller.poll())
             for sock in socks:
                 data = await sock.recv_multipart()
-                self._logger.debug("new worker connected %s", data[0])
+                connected_worker = ConnectedWorker(
+                    name=data[0], service_uuid=UUID(bytes=data[1])
+                )
+                fast_publish = False
+                if connected_worker.service_uuid not in self.state.connected_workers:
+                    fast_publish = True
+                self.state.connected_workers[
+                    connected_worker.service_uuid
+                ] = connected_worker
+                now = time.time()
+                self.state.connected_workers = {
+                    uuid: cw
+                    for uuid, cw in self.state.connected_workers.items()
+                    if now - cw.last_seen < 3
+                }
+                self._logger.debug("worker pinnged %s", connected_worker)
+                if fast_publish:
+                    self._logger.debug("fast publish")
+                    await self.publish_config()
 
     async def close(self) -> None:
         """
         Clean up any open connections
         """
-        self.accept_task.cancel()
-        self.work_task.cancel()
+        await cancel_and_wait(self.accept_task)
+        await cancel_and_wait(self.work_task)
+        await cancel_and_wait(self.metrics_task)
+        await cancel_and_wait(self.assign_task)
         await self.redis.delete(RedisKeys.config("ingester", self.state.name))
         await super().close()
         self.ctx.destroy(linger=0)
         self._logger.info("closed ingester")
```

### Comparing `dranspose-0.0.2/dranspose/ingesters/__init__.py` & `dranspose-0.0.3/dranspose/ingesters/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,23 @@
     HttpSardanaIngester,
     HttpSardanaSettings,
 )
 from dranspose.ingesters.zmqpull_single import (  # noqa: F401
     ZmqPullSingleIngester,
     ZmqPullSingleSettings,
 )
+from dranspose.ingesters.zmqpull_eiger_legacy import (  # noqa: F401
+    ZmqPullEigerLegacyIngester,
+    ZmqPullEigerLegacySettings,
+)
 from dranspose.ingesters.zmqsub_contrast import (  # noqa: F401
     ZmqSubContrastIngester,
     ZmqSubContrastSettings,
 )
 from dranspose.ingesters.zmqsub_xspress3 import (  # noqa: F401
     ZmqSubXspressIngester,
     ZmqSubXspressSettings,
 )
+from dranspose.ingesters.zmqsub_albaem import (  # noqa: F401
+    ZmqSubAlbaemIngester,
+    ZmqSubAlbaemSettings,
+)
```

### Comparing `dranspose-0.0.2/dranspose/ingesters/http_sardana.py` & `dranspose-0.0.3/dranspose/ingesters/http_sardana.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dranspose.data.sardana import (
     SardanaDataDescription,
     SardanaRecordEnd,
     SardanaRecordData,
     SardanaPacketType,
 )
 from dranspose.event import StreamData
-from dranspose.helpers.utils import done_callback
+from dranspose.helpers.utils import done_callback, cancel_and_wait
 from dranspose.ingester import Ingester, IngesterSettings
 from dranspose.protocol import StreamName
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -76,40 +76,40 @@
 async def lifespan(app: FastAPI) -> AsyncGenerator[None, None]:
     # Load the ML model
     global sardana_ingester
     sardana_ingester = HttpSardanaIngester()
     run_task = asyncio.create_task(sardana_ingester.run())
     run_task.add_done_callback(done_callback)
     yield
-    run_task.cancel()
+    await cancel_and_wait(run_task)
     await sardana_ingester.close()
     # Clean up the ML models and release the resources
 
 
 app = FastAPI(lifespan=lifespan)
 
 
 @app.post("/v1/data_desc")
-async def post_data_desc(payload: dict[str, Any] = Body(...)) -> None:
+async def post_data_desc(data: SardanaDataDescription = Body(...)) -> None:
     global sardana_ingester
-    await sardana_ingester.receive(SardanaDataDescription(description=payload))
-    logging.info("data_desc received %s", payload)
+    await sardana_ingester.receive(data)  # SardanaDataDescription(description=payload))
+    logger.info("data_desc received %s", data.__repr__())
 
 
 @app.post("/v1/record_data")
-async def post_record_data(payload: dict[str, Any] = Body(...)) -> None:
+async def post_record_data(data: SardanaRecordData = Body(...)) -> None:
     global sardana_ingester
-    await sardana_ingester.receive(SardanaRecordData(record=payload))
-    logging.debug("record_data received %s", payload)
+    await sardana_ingester.receive(data)
+    logger.debug("record_data received %s", data.__repr__())
 
 
 @app.post("/v1/custom_data")
 async def post_custom_data(payload: dict[str, Any] = Body(...)) -> None:
     global sardana_ingester
-    logging.debug("ignoring custom_data received %s", payload)
+    logger.debug("ignoring custom_data received %s", payload)
 
 
 @app.post("/v1/record_end")
-async def post_record_end(payload: dict[str, Any] = Body(...)) -> None:
+async def post_record_end(data: SardanaRecordEnd = Body(...)) -> None:
     global sardana_ingester
-    await sardana_ingester.receive(SardanaRecordEnd(end=payload))
-    logging.debug("record_end received %s", payload)
+    await sardana_ingester.receive(data)
+    logging.debug("record_end received %s", data.__repr__())
```

### Comparing `dranspose-0.0.2/dranspose/ingesters/tcp_positioncap.py` & `dranspose-0.0.3/dranspose/ingesters/tcp_positioncap.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/ingesters/zmqpull_single.py` & `dranspose-0.0.3/dranspose/ingesters/zmqpull_single.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/ingesters/zmqsub_contrast.py` & `dranspose-0.0.3/dranspose/ingesters/zmqsub_contrast.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/ingesters/zmqsub_xspress3.py` & `dranspose-0.0.3/dranspose/ingesters/zmqsub_xspress3.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/mapping.py` & `dranspose-0.0.3/dranspose/mapping.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                         for vw in frame:
                             tags.update(vw.tags)
 
             for li in m.values():
                 li.insert(0, [VirtualWorker(tags={t}) for t in tags])
                 li.append([VirtualWorker(tags={t}) for t in tags])
 
-        print("mapping is", m)
+        # print("mapping is", m)
         self.mapping = m
         self.uuid = uuid.uuid4()
         self.assignments: dict[VirtualConstraint, WorkerName] = {}
         self.all_assignments: dict[
             tuple[EventNumber, StreamName, int], list[WorkerName]
         ] = defaultdict(list)
         self.complete_events = 0
@@ -54,18 +54,30 @@
     def len(self) -> int:
         if len(self.mapping) > 0:
             return len(list(self.mapping.values())[0])
         else:
             return 0
 
     def assign_next(
-        self, worker: WorkerState, all_workers: list[WorkerState]
+        self,
+        worker: WorkerState,
+        all_workers: list[WorkerState],
+        completed: Optional[EventNumber] = None,
+        horizon: int = 0,
     ) -> list[VirtualWorker]:
-        assigned_to = []
+        assigned_to: list[VirtualWorker] = []
         maxassign = EventNumber(self.len() + 1)
+        still_has_work = False
+        if completed is not None:
+            for evnint in range(completed + 1, self.complete_events - horizon):
+                wa = self.get_event_workers(EventNumber(evnint))
+                if worker.name in wa.get_all_workers():
+                    still_has_work = True
+        if still_has_work:
+            return assigned_to
         for evnint in range(self.complete_events, self.len()):
             evn = EventNumber(evnint)
             for stream, v in self.mapping.items():  # first fill the alls
                 assign = v[evn]
                 if (
                     assign is not None and len(assign) > 0
                 ):  # frame exists and is not discarded
@@ -100,14 +112,16 @@
                                     self.assignments[vw.constraint] = worker.name
                                     self.update_filled(all_workers)
                                     assigned_to.append(vw)
                                     return assigned_to
             if evn == maxassign:
                 self.update_filled(all_workers)
                 return assigned_to
+        if assigned_to == []:
+            self.update_filled(all_workers)
         return assigned_to
 
     def min_workers(self) -> int:
         minimum = 0
         for i in zip(*self.mapping.values()):
             workers = set()
             for val in i:
@@ -130,14 +144,16 @@
         ret: dict[StreamName, set[WorkerName]] = defaultdict(set)
         if no > self.complete_events - 1:
             raise NotYetAssigned()
         for s, v in self.mapping.items():
             assign = v[no]
             if assign is None:
                 continue
+            if len(assign) == 0:
+                ret[s] = set()
             for i, vw in enumerate(assign):
                 if vw.constraint is None:  # get from all
                     ret[s].update(self.all_assignments[(no, s, i)])
                 else:
                     ret[s].add(self.assignments[vw.constraint])
         return WorkAssignment(
             event_number=no, assignments={s: sorted(v) for s, v in ret.items()}
```

### Comparing `dranspose-0.0.2/dranspose/middlewares/contrast.py` & `dranspose-0.0.3/dranspose/middlewares/contrast.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/middlewares/stream1.py` & `dranspose-0.0.3/dranspose/middlewares/stream1.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         val = json.loads(frame.bytes)
     elif isinstance(frame, bytes):
         val = json.loads(frame)
     else:
         raise Exception("invalid StreamData")
 
     packet = Stream1Packet.validate_python(val)
-    print("packet", packet)
     if isinstance(packet, Stream1Data):
         assert data.length == 2
         bufframe = data.frames[1]
         if isinstance(bufframe, zmq.Frame):
             bufframe = bufframe.bytes
         buf = np.frombuffer(bufframe, dtype=packet.type)
         img = buf.reshape(packet.shape)
```

### Comparing `dranspose-0.0.2/dranspose/middlewares/xspress.py` & `dranspose-0.0.3/dranspose/middlewares/xspress.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/dranspose/protocol.py` & `dranspose-0.0.3/dranspose/protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import time
 import uuid
 from enum import Enum
 from typing import NewType, Literal, Annotated, Optional, TypeAlias
 
 from pydantic import (
     UUID4,
     BaseModel,
     validate_call,
     UrlConstraints,
     Field,
+    TypeAdapter,
 )
 
 from uuid import uuid4
 from functools import cache, cached_property
 
 from pydantic_core import Url
 
@@ -109,20 +111,22 @@
 class ProtocolException(Exception):
     pass
 
 
 class ControllerUpdate(BaseModel):
     mapping_uuid: UUID4
     parameters_version: dict[ParameterName, UUID4]
+    target_parameters_hash: Optional[Digest] = None
     finished: bool = False
 
 
 class WorkParameter(BaseModel):
     name: str
     data: bytes
+    value: Optional[int | str | bytes | float | bool] = None
     uuid: UUID4 = Field(default_factory=uuid4)
 
 
 class WorkAssignment(BaseModel):
     event_number: EventNumber
     assignments: dict[StreamName, list[WorkerName]]
 
@@ -133,24 +137,30 @@
                 ret.assignments[stream] = self.assignments[stream]
         return ret
 
     def get_all_workers(self) -> set[WorkerName]:
         return set([x for stream in self.assignments.values() for x in stream])
 
 
-class WorkerStateEnum(Enum):
+WorkAssignmentList = TypeAdapter(list[WorkAssignment])
+
+
+class DistributedStateEnum(Enum):
+    READY = "ready"
     IDLE = "idle"
+    FINISHED = "finished"
 
 
 class WorkerTimes(BaseModel):
-    get_assignments: float
-    get_messages: float
-    assemble_event: float
-    custom_code: float
-    send_result: float
+    get_assignments: float = 0.0
+    get_messages: float = 0.0
+    assemble_event: float = 0.0
+    custom_code: float = 0.0
+    send_result: float = 0.0
+    no_events: int = 1
 
     @classmethod
     def from_timestamps(
         cls,
         start: float,
         assignments: float,
         messages: float,
@@ -162,14 +172,24 @@
             get_assignments=assignments - start,
             get_messages=messages - assignments,
             assemble_event=event - messages,
             custom_code=custom - event,
             send_result=send - custom,
         )
 
+    def __add__(self, other: "WorkerTimes") -> "WorkerTimes":
+        return WorkerTimes(
+            get_assignments=self.get_assignments + other.get_assignments,
+            get_messages=self.get_messages + other.get_messages,
+            assemble_event=self.assemble_event + other.assemble_event,
+            custom_code=self.custom_code + other.custom_code,
+            send_result=self.send_result + other.send_result,
+            no_events=self.no_events + other.no_events,
+        )
+
     @cached_property
     def total(self) -> float:
         return self.get_assignments + self.get_messages + self.active
 
     @cached_property
     def active(self) -> float:
         return self.assemble_event + self.custom_code + self.send_result
@@ -193,32 +213,60 @@
     last_event: int
     intervals: dict[int | Literal["scan"], IntervalLoad]
 
 
 SystemLoadType = dict[WorkerName, WorkerLoad]
 
 
-class WorkerUpdate(BaseModel):
-    state: WorkerStateEnum
-    completed: EventNumber
+class BaseUpdate(BaseModel):
+    state: DistributedStateEnum
+
+
+class WorkerUpdate(BaseUpdate):
+    source: Literal["worker"] = "worker"
+    completed: list[EventNumber] = []
     worker: WorkerName
-    new: bool = False
+    has_result: list[bool] = []
     processing_times: Optional[WorkerTimes] = None
 
 
+class ReducerUpdate(BaseUpdate):
+    source: Literal["reducer"] = "reducer"
+    completed: Optional[EventNumber] = None
+    worker: Optional[WorkerName] = None
+
+
+class IngesterUpdate(BaseUpdate):
+    source: Literal["ingester"] = "ingester"
+    ingester: IngesterName
+
+
+DistributedUpdateType = WorkerUpdate | ReducerUpdate | IngesterUpdate
+
+DistributedUpdate = TypeAdapter(WorkerUpdate | ReducerUpdate | IngesterUpdate)
+
+
 class DistributedState(BaseModel):
     service_uuid: UUID4 = Field(default_factory=uuid.uuid4)
     mapping_uuid: Optional[UUID4] = None
     parameters_hash: Optional[Digest] = None
     processed_events: int = 0
+    event_rate: float = 0.0
+
+
+class ConnectedWorker(BaseModel):
+    name: WorkerName
+    service_uuid: UUID4
+    last_seen: float = Field(default_factory=time.time)
 
 
 class IngesterState(DistributedState):
     name: IngesterName
     url: ZmqUrl
+    connected_workers: dict[UUID4, ConnectedWorker] = {}
     streams: list[StreamName] = []
 
 
 class WorkerState(DistributedState):
     name: WorkerName
     ingesters: list[IngesterState] = []
     tags: set[WorkerTag] = {GENERIC_WORKER}
@@ -237,7 +285,10 @@
     def get_streams(self) -> list[StreamName]:
         ingester_streams = set([s for i in self.ingesters for s in i.streams])
         worker_streams = [
             set([s for i in w.ingesters for s in i.streams]) for w in self.workers
         ]
 
         return list(ingester_streams.intersection(*worker_streams))
+
+    def get_workers(self) -> list[WorkerName]:
+        return [w.name for w in self.workers]
```

### Comparing `dranspose-0.0.2/dranspose/reducer.py` & `dranspose-0.0.3/dranspose/reducer.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,22 @@
 from pydantic import UUID4
 from starlette.responses import Response
 
 from dranspose.helpers import utils
 from dranspose.distributed import DistributedService, DistributedSettings
 from dranspose.event import ResultData
 from dranspose.helpers.jsonpath_slice_ext import NumpyExtentedJsonPathParser
-from dranspose.helpers.utils import done_callback
-from dranspose.protocol import ReducerState, ZmqUrl, RedisKeys
+from dranspose.helpers.utils import done_callback, cancel_and_wait
+from dranspose.protocol import (
+    ReducerState,
+    ZmqUrl,
+    RedisKeys,
+    ReducerUpdate,
+    DistributedStateEnum,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class ReducerSettings(DistributedSettings):
     reducer_url: ZmqUrl = ZmqUrl("tcp://localhost:10200")
     reducer_class: Optional[str] = None
@@ -40,14 +46,15 @@
         self.in_socket = self.ctx.socket(zmq.PULL)
         self.in_socket.setsockopt(zmq.TCP_KEEPALIVE, 1)
         self.in_socket.setsockopt(zmq.TCP_KEEPALIVE_IDLE, 300)
         self.in_socket.setsockopt(zmq.TCP_KEEPALIVE_INTVL, 300)
         self.in_socket.bind(f"tcp://*:{self._reducer_settings.reducer_url.port}")
 
         self.custom = None
+        self.custom_context: dict[Any, Any] = {}
         if self._reducer_settings.reducer_class:
             try:
                 self.custom = utils.import_class(self._reducer_settings.reducer_class)
                 self._logger.info("custom reducer class %s", self.custom)
                 try:
                     self.param_descriptions = self.custom.describe_parameters()  # type: ignore[attr-defined]
                 except AttributeError:
@@ -65,43 +72,89 @@
                     e.__repr__(),
                     traceback.format_exc(),
                 )
 
     async def run(self) -> None:
         self.work_task = asyncio.create_task(self.work())
         self.work_task.add_done_callback(done_callback)
+        self.metrics_task = asyncio.create_task(self.update_metrics())
+        self.metrics_task.add_done_callback(done_callback)
         await self.register()
 
     async def work(self) -> None:
         self._logger.info("started work task")
         self.reducer = None
         if self.custom:
-            self.reducer = self.custom(self.parameters)
+            self.reducer = self.custom(
+                parameters=self.parameters, context=self.custom_context
+            )
         while True:
             parts = await self.in_socket.recv_multipart()
             prelim = json.loads(parts[0])
             prelim["payload"] = pickle.loads(parts[1])
             result = ResultData.model_validate(prelim)
             if self.reducer:
                 try:
-                    result = self.reducer.process_result(result, self.parameters)
+                    loop = asyncio.get_event_loop()
+                    await loop.run_in_executor(
+                        None, self.reducer.process_result, result, self.parameters
+                    )
                 except Exception as e:
-                    self._logger.error("custom reducer failed: %s", e.__repr__())
-            self._logger.debug("received %s", result)
+                    self._logger.error(
+                        "custom reducer failed: %s\n%s",
+                        e.__repr__(),
+                        traceback.format_exc(),
+                    )
+            ru = ReducerUpdate(
+                state=DistributedStateEnum.IDLE,
+                completed=result.event_number,
+                worker=result.worker,
+            )
+            self._logger.debug("result processed, notify controller with %s", ru)
+            await self.redis.xadd(
+                RedisKeys.ready(self.state.mapping_uuid),
+                {"data": ru.model_dump_json()},
+            )
+            self._logger.debug("processed result %s", result)
             self.state.processed_events += 1
 
     async def restart_work(self, new_uuid: UUID4) -> None:
         self._logger.info("resetting config %s", new_uuid)
-        self.work_task.cancel()
+        await cancel_and_wait(self.work_task)
         self.state.mapping_uuid = new_uuid
         self.work_task = asyncio.create_task(self.work())
         self.work_task.add_done_callback(done_callback)
 
+    async def finish_work(self) -> None:
+        self._logger.info("finishing reducer work")
+        if self.reducer:
+            if hasattr(self.reducer, "finish"):
+                try:
+                    loop = asyncio.get_event_loop()
+                    await loop.run_in_executor(
+                        None, self.reducer.finish, self.parameters
+                    )
+                except Exception as e:
+                    self._logger.error(
+                        "custom reducer finish failed: %s\n%s",
+                        e.__repr__(),
+                        traceback.format_exc(),
+                    )
+        await self.redis.xadd(
+            RedisKeys.ready(self.state.mapping_uuid),
+            {
+                "data": ReducerUpdate(
+                    state=DistributedStateEnum.FINISHED,
+                ).model_dump_json()
+            },
+        )
+
     async def close(self) -> None:
-        self.work_task.cancel()
+        await cancel_and_wait(self.work_task)
+        await cancel_and_wait(self.metrics_task)
         await self.redis.delete(RedisKeys.config("reducer", self.state.name))
         await super().close()
         self.ctx.destroy(linger=0)
         self._logger.info("closed reducer")
 
 
 reducer: Reducer
@@ -111,15 +164,15 @@
 async def lifespan(app: FastAPI) -> AsyncGenerator[None, None]:
     # Load the ML model
     global reducer
     reducer = Reducer()
     run_task = asyncio.create_task(reducer.run())
     run_task.add_done_callback(done_callback)
     yield
-    run_task.cancel()
+    await cancel_and_wait(run_task)
     await reducer.close()
     # Clean up the ML models and release the resources
 
 
 app = FastAPI(lifespan=lifespan)
```

### Comparing `dranspose-0.0.2/dranspose/worker.py` & `dranspose-0.0.3/dranspose/worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import asyncio
 import json
 import pickle
 import random
 import socket
 import string
 import time
-from asyncio import Future
-from typing import Optional
+import traceback
+from asyncio import Future, Task
+from typing import Optional, Any
 
 import zmq.asyncio
 
 from pydantic import UUID4, BaseModel, ConfigDict, Field
 
 from dranspose.helpers import utils
 import redis.exceptions as rexceptions
 
 from dranspose.distributed import DistributedService, DistributedSettings
 from dranspose.event import InternalWorkerMessage, EventData, ResultData
-from dranspose.helpers.utils import done_callback
+from dranspose.helpers.utils import done_callback, cancel_and_wait
 from dranspose.protocol import (
     WorkerState,
     RedisKeys,
     IngesterState,
     WorkerUpdate,
-    WorkerStateEnum,
-    WorkAssignment,
+    DistributedStateEnum,
     WorkerName,
-    EventNumber,
     IngesterName,
     StreamName,
     ReducerState,
     WorkerTimes,
     GENERIC_WORKER,
     WorkerTag,
+    WorkAssignmentList,
 )
 
 
 class RedisException(Exception):
     pass
 
 
 class ConnectedIngester(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     socket: zmq.asyncio.Socket
     config: IngesterState
+    pinged_since: float = Field(default_factory=time.time)
 
 
 def random_worker_name() -> WorkerName:
     randid = "".join([random.choice(string.ascii_letters) for _ in range(10)])
     name = "Worker-{}-{}".format(socket.gethostname(), randid)
     return WorkerName(name)
 
@@ -76,16 +77,22 @@
         self._ingesters: dict[IngesterName, ConnectedIngester] = {}
         self._stream_map: dict[StreamName, zmq._future._AsyncSocket] = {}
         self.poll_task: Optional[Future[list[int]]] = None
 
         self._reducer_service_uuid: Optional[UUID4] = None
         self.out_socket: Optional[zmq._future._AsyncSocket] = None
 
+        self.assignment_queue: asyncio.Queue[
+            set[zmq._future._AsyncSocket]
+        ] = asyncio.Queue()
+        self.dequeue_task: Optional[Task[set[zmq._future._AsyncSocket]]] = None
+
         self.param_descriptions = []
         self.custom = None
+        self.custom_context: dict[Any, Any] = {}
         self.worker = None
         if self._worker_settings.worker_class:
             try:
                 self.custom = utils.import_class(self._worker_settings.worker_class)
                 self._logger.info("custom worker class %s", self.custom)
 
                 try:
@@ -98,71 +105,78 @@
                     self._logger.error(
                         "custom worker parameter descripition is broken: %s",
                         e.__repr__(),
                     )
 
             except Exception as e:
                 self._logger.error(
-                    "no custom worker class loaded, discarding events, err %s",
+                    "no custom worker class loaded, discarding events, err %s\n%s",
                     e.__repr__(),
+                    traceback.format_exc(),
                 )
 
     async def run(self) -> None:
         self.manage_ingester_task = asyncio.create_task(self.manage_ingesters())
         self.manage_ingester_task.add_done_callback(done_callback)
         self.manage_receiver_task = asyncio.create_task(self.manage_receiver())
         self.manage_receiver_task.add_done_callback(done_callback)
+        self.assignment_queue = asyncio.Queue()
         self.work_task = asyncio.create_task(self.work())
         self.work_task.add_done_callback(done_callback)
+        self.assign_task = asyncio.create_task(self.manage_assignments())
+        self.assign_task.add_done_callback(done_callback)
+        self.metrics_task = asyncio.create_task(self.update_metrics())
+        self.metrics_task.add_done_callback(done_callback)
         await self.register()
 
     async def notify_worker_ready(self) -> None:
         await self.redis.xadd(
             RedisKeys.ready(self.state.mapping_uuid),
             {
                 "data": WorkerUpdate(
-                    state=WorkerStateEnum.IDLE,
-                    new=True,
-                    completed=EventNumber(0),
+                    state=DistributedStateEnum.READY,
                     worker=self.state.name,
                 ).model_dump_json()
             },
         )
 
         self._logger.info("registered ready message")
 
-    async def get_new_assignments(
-        self, lastev: str
-    ) -> tuple[Optional[str], Optional[set[zmq._future._AsyncSocket]]]:
+    async def manage_assignments(self) -> None:
         sub = RedisKeys.assigned(self.state.mapping_uuid)
-        try:
-            assignments = await self.redis.xread({sub: lastev}, block=1000, count=1)
-        except rexceptions.ConnectionError:
-            raise RedisException()
-        if sub not in assignments:
-            return None, None
-        assignments = assignments[sub][0][0]
-        self._logger.debug("got assignments %s", assignments)
-        self._logger.debug("stream map %s", self._stream_map)
-        work_assignment = WorkAssignment.model_validate_json(assignments[1]["data"])
-        ingesterset = set()
-        for stream, workers in work_assignment.assignments.items():
-            if self.state.name in workers:
-                try:
-                    ingesterset.add(self._stream_map[stream])
-                except KeyError:
-                    self._logger.error(
-                        "ingester for stream %s not connected, available: %s",
-                        stream,
-                        self._ingesters,
-                    )
-        self._logger.debug("receive from ingesters %s", ingesterset)
-
-        lastev = assignments[0]
-        return lastev, ingesterset
+        lastev = 0
+        while True:
+            try:
+                assignments = await self.redis.xread({sub: lastev}, block=1000, count=1)
+            except rexceptions.ConnectionError:
+                break
+            if sub not in assignments:
+                continue
+            assignments = assignments[sub][0][0]
+            self._logger.debug("got assignments %s", assignments)
+            self._logger.debug("stream map %s", self._stream_map)
+            work_assignment_list = WorkAssignmentList.validate_json(
+                assignments[1]["data"]
+            )
+            for work_assignment in work_assignment_list:
+                ingesterset = set()
+                for stream, workers in work_assignment.assignments.items():
+                    if self.state.name in workers:
+                        try:
+                            ingesterset.add(self._stream_map[stream])
+                        except KeyError:
+                            self._logger.error(
+                                "ingester for stream %s not connected, available: %s",
+                                stream,
+                                self._ingesters,
+                            )
+                self._logger.debug("receive from ingesters %s", ingesterset)
+                if len(ingesterset) > 0:
+                    await self.assignment_queue.put(ingesterset)
+            lastev = assignments[0]
 
     async def poll_internals(
         self, ingesterset: set[zmq._future._AsyncSocket]
     ) -> list[int]:
         self._logger.debug("poll internal sockets %s", ingesterset)
         poll_tasks = [sock.poll() for sock in ingesterset]
         self._logger.debug("await poll tasks %s", poll_tasks)
@@ -189,131 +203,173 @@
 
     async def work(self) -> None:
         self._logger.info("started work task")
 
         self.worker = None
         if self.custom:
             try:
-                self.worker = self.custom(self.parameters)
+                self.worker = self.custom(
+                    parameters=self.parameters,
+                    context=self.custom_context,
+                    state=self.state,
+                )
             except Exception as e:
                 self._logger.error(
                     "Failed to instantiate custom worker: %s", e.__repr__()
                 )
 
         await self.notify_worker_ready()
+        try:
+            proced = 0
+            completed = []
+            has_result = []
+            accum_times = WorkerTimes(no_events=0)
+            accum_start = time.time()
+            while True:
+                perf_start = time.perf_counter()
 
-        lastev: str = "0"
-        proced = 0
-        while True:
-            perf_start = time.perf_counter()
-            try:
-                newlastev, ingesterset = await self.get_new_assignments(lastev)
-                if newlastev is None or ingesterset is None:
+                self.dequeue_task = None
+                self.dequeue_task = asyncio.create_task(self.assignment_queue.get())
+                ingesterset = await self.dequeue_task
+                perf_got_assignments = time.perf_counter()
+                done = await self.poll_internals(ingesterset)
+                if set(done) != {zmq.POLLIN}:
+                    self._logger.warning("not all sockets are pollIN %s", done)
                     continue
-                lastev = newlastev
-            except RedisException:
-                self._logger.warning("failed to access redis, exiting worker")
-                break
-            perf_got_assignments = time.perf_counter()
-
-            if len(ingesterset) == 0:
-                continue
-            done = await self.poll_internals(ingesterset)
-            if set(done) != {zmq.POLLIN}:
-                self._logger.warning("not all sockets are pollIN %s", done)
-                continue
 
-            perf_got_work = time.perf_counter()
+                perf_got_work = time.perf_counter()
 
-            event = await self.build_event(ingesterset)
+                event = await self.build_event(ingesterset)
 
-            perf_assembled_event = time.perf_counter()
-            self._logger.debug("received work %s", event)
-            result = None
-            if self.worker:
-                try:
-                    loop = asyncio.get_event_loop()
-                    result = await loop.run_in_executor(
-                        None, self.worker.process_event, event, self.parameters
+                perf_assembled_event = time.perf_counter()
+                self._logger.debug("received work %s", event)
+                result = None
+                if self.worker:
+                    try:
+                        loop = asyncio.get_event_loop()
+                        result = await loop.run_in_executor(
+                            None, self.worker.process_event, event, self.parameters
+                        )
+                    except Exception as e:
+                        self._logger.error(
+                            "custom worker failed: %s\n%s",
+                            e.__repr__(),
+                            traceback.format_exc(),
+                        )
+                perf_custom_code = time.perf_counter()
+                self._logger.debug("got result %s", result)
+                if result is not None:
+                    rd = ResultData(
+                        event_number=event.event_number,
+                        worker=self.state.name,
+                        payload=result,
+                        parameters_hash=self.state.parameters_hash,
                     )
-                except Exception as e:
-                    self._logger.error("custom worker failed: %s", e.__repr__())
-            perf_custom_code = time.perf_counter()
-            self._logger.debug("got result %s", result)
-            rd = ResultData(
-                event_number=event.event_number,
-                worker=self.state.name,
-                payload=result,
-                parameters_hash=self.state.parameters_hash,
-            )
-            if self.out_socket:
-                try:
-                    header = rd.model_dump_json(exclude={"payload"}).encode("utf8")
-                    body = pickle.dumps(rd.payload)
-                    self._logger.debug(
-                        "send result to reducer with header %s, len-payload %d",
-                        header,
-                        len(body),
+                    if self.out_socket:
+                        try:
+                            header = rd.model_dump_json(exclude={"payload"}).encode(
+                                "utf8"
+                            )
+                            body = pickle.dumps(rd.payload)
+                            self._logger.debug(
+                                "send result to reducer with header %s, len-payload %d",
+                                header,
+                                len(body),
+                            )
+                            await self.out_socket.send_multipart([header, body])
+                        except Exception as e:
+                            self._logger.error(
+                                "could not send out result %s", e.__repr__()
+                            )
+                perf_sent_result = time.perf_counter()
+                proced += 1
+                self.state.processed_events += 1
+                if proced % 500 == 0:
+                    self._logger.info("processed %d events", proced)
+                completed.append(event.event_number)
+                has_result.append(result is not None)
+                times = WorkerTimes.from_timestamps(
+                    perf_start,
+                    perf_got_assignments,
+                    perf_got_work,
+                    perf_assembled_event,
+                    perf_custom_code,
+                    perf_sent_result,
+                )
+                accum_times += times
+                if self.assignment_queue.empty() or time.time() - accum_start > 1:
+                    wu = WorkerUpdate(
+                        state=DistributedStateEnum.IDLE,
+                        completed=completed,
+                        worker=self.state.name,
+                        has_result=has_result,
+                        processing_times=accum_times,
                     )
-                    await self.out_socket.send_multipart([header, body])
-                except Exception as e:
-                    self._logger.error("could not dump result %s", e.__repr__())
-            perf_sent_result = time.perf_counter()
-            proced += 1
-            self.state.processed_events += 1
-            if proced % 500 == 0:
-                self._logger.info("processed %d events", proced)
-            times = WorkerTimes.from_timestamps(
-                perf_start,
-                perf_got_assignments,
-                perf_got_work,
-                perf_assembled_event,
-                perf_custom_code,
-                perf_sent_result,
-            )
-            wu = WorkerUpdate(
-                state=WorkerStateEnum.IDLE,
-                completed=event.event_number,
-                worker=self.state.name,
-                processing_times=times,
-            )
-            self._logger.debug("all work done, notify controller with %s", wu)
-            await self.redis.xadd(
-                RedisKeys.ready(self.state.mapping_uuid),
-                {"data": wu.model_dump_json()},
-            )
+                    self._logger.debug("all work done, notify controller with %s", wu)
+                    await self.redis.xadd(
+                        RedisKeys.ready(self.state.mapping_uuid),
+                        {"data": wu.model_dump_json()},
+                    )
+                    completed = []
+                    has_result = []
+                    accum_times = WorkerTimes(no_events=0)
+                    accum_start = time.time()
+        except asyncio.exceptions.CancelledError:
+            pass
         self._logger.info("work thread finished")
 
     async def finish_work(self) -> None:
         self._logger.info("finishing work")
         if self.worker:
             if hasattr(self.worker, "finish"):
-                loop = asyncio.get_event_loop()
-                await loop.run_in_executor(None, self.worker.finish, self.parameters)
+                try:
+                    loop = asyncio.get_event_loop()
+                    await loop.run_in_executor(
+                        None, self.worker.finish, self.parameters
+                    )
+                except Exception as e:
+                    self._logger.error(
+                        "custom worker finish failed: %s\n%s",
+                        e.__repr__(),
+                        traceback.format_exc(),
+                    )
+        await self.redis.xadd(
+            RedisKeys.ready(self.state.mapping_uuid),
+            {
+                "data": WorkerUpdate(
+                    state=DistributedStateEnum.FINISHED,
+                    worker=self.state.name,
+                ).model_dump_json()
+            },
+        )
 
     async def restart_work(self, new_uuid: UUID4) -> None:
         self._logger.info("resetting config %s", new_uuid)
         if self.poll_task:
-            self.poll_task.cancel()
+            await cancel_and_wait(self.poll_task)
             self.poll_task = None
             self._logger.debug("cancelled poll task")
-        self.work_task.cancel()
+        await cancel_and_wait(self.work_task)
         self._logger.info("clean up in sockets")
+        await cancel_and_wait(self.assign_task)
         for iname, ing in self._ingesters.items():
             while True:
                 res = await ing.socket.poll(timeout=0.001)
                 if res == zmq.POLLIN:
                     await ing.socket.recv_multipart(copy=False)
                     self._logger.debug("discarded internal message from %s", iname)
                 else:
                     break
 
+        self.assignment_queue = asyncio.Queue()
         self.state.mapping_uuid = new_uuid
         self.work_task = asyncio.create_task(self.work())
         self.work_task.add_done_callback(done_callback)
+        self.assign_task = asyncio.create_task(self.manage_assignments())
+        self.assign_task.add_done_callback(done_callback)
 
     async def manage_receiver(self) -> None:
         while True:
             config = await self.redis.get(RedisKeys.config("reducer"))
             if config is None:
                 self._logger.warning("cannot get reducer configuration")
                 await asyncio.sleep(1)
@@ -333,35 +389,48 @@
         while True:
             configs = await self.redis.keys(RedisKeys.config("ingester"))
             processed = []
             for key in configs:
                 cfg = IngesterState.model_validate_json(await self.redis.get(key))
                 iname = cfg.name
                 processed.append(iname)
-                if (
-                    iname in self._ingesters
-                    and self._ingesters[iname].config.service_uuid != cfg.service_uuid
-                ):
-                    self._logger.warning(
-                        "service_uuid of ingester changed from %s to %s, disconnecting",
-                        self._ingesters[iname].config.service_uuid,
-                        cfg.service_uuid,
+                if iname in self._ingesters:
+                    pinged_for_long = (
+                        time.time() - self._ingesters[iname].pinged_since > 10
+                    )
+                    reached_ingester = (
+                        self.state.service_uuid in cfg.connected_workers.keys()
                     )
-                    self._ingesters[iname].socket.close()
-                    del self._ingesters[iname]
+
+                    if self._ingesters[iname].config.service_uuid != cfg.service_uuid:
+                        self._logger.warning(
+                            "service_uuid of ingester changed from %s to %s, disconnecting",
+                            self._ingesters[iname].config.service_uuid,
+                            cfg.service_uuid,
+                        )
+                        self._ingesters[iname].socket.close()
+                        del self._ingesters[iname]
+
+                    elif pinged_for_long and not reached_ingester:
+                        self._logger.warning(
+                            "we send pings, but don't reach ingester %s, disconnecting",
+                            iname,
+                        )
+                        self._ingesters[iname].socket.close()
+                        del self._ingesters[iname]
 
                 if iname not in self._ingesters:
                     self._logger.info("adding new ingester %s", iname)
                     sock = self.ctx.socket(zmq.DEALER)
                     sock.setsockopt(zmq.IDENTITY, self.state.name.encode("ascii"))
                     sock.connect(str(cfg.url))
-                    await sock.send(b"")
+                    await sock.send(self.state.service_uuid.bytes)
                     self._ingesters[iname] = ConnectedIngester(config=cfg, socket=sock)
 
-                await self._ingesters[iname].socket.send(b"")
+                await self._ingesters[iname].socket.send(self.state.service_uuid.bytes)
                 self._logger.debug("pinged %s", iname)
             for iname in set(self._ingesters.keys()) - set(processed):
                 self._logger.info("removing stale ingester %s", iname)
                 self._ingesters[iname].socket.close()
                 del self._ingesters[iname]
             self._stream_map = {
                 s: conn_ing.socket
@@ -375,13 +444,17 @@
                     "changed ingester config, fast publish %s", new_ingesters
                 )
                 await self.publish_config()
 
             await asyncio.sleep(2)
 
     async def close(self) -> None:
-        self.manage_ingester_task.cancel()
-        self.manage_receiver_task.cancel()
+        await cancel_and_wait(self.manage_ingester_task)
+        await cancel_and_wait(self.manage_receiver_task)
+        await cancel_and_wait(self.metrics_task)
+        await cancel_and_wait(self.assign_task)
+        if self.dequeue_task is not None:
+            await cancel_and_wait(self.dequeue_task)
         await self.redis.delete(RedisKeys.config("worker", self.state.name))
         await super().close()
         self.ctx.destroy()
         self._logger.info("worker closed")
```

### Comparing `dranspose-0.0.2/dranspose.egg-info/PKG-INFO` & `dranspose-0.0.3/dranspose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dranspose
-Version: 0.0.2
+Version: 0.0.3
 Summary: A stream matrix transposition framework
 Author-email: Felix Engelmann <felix-github@nlogn.org>
 Project-URL: Homepage, https://github.com/felix-engelmann/dranspose
 Project-URL: Bug Tracker, https://github.com/felix-engelmann/dranspose/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dranspose-0.0.2/dranspose.egg-info/SOURCES.txt` & `dranspose-0.0.3/dranspose.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
 README.md
 mkdocs.yml
 pyproject.toml
 docs/.gitignore
+docs/CNAME
 docs/index.md
 docs/applications/overview.md
 docs/deployment/capturing.md
 docs/deployment/kubernetes.md
+docs/deployment/sardana.md
 docs/poster-2024-01-15/.gitignore
 docs/poster-2024-01-15/lutheme.sty
 docs/poster-2024-01-15/main.tex
 docs/poster-2024-01-15/reducer.py
 docs/poster-2024-01-15/tikzposter.cls
 docs/poster-2024-01-15/tikzposterBackgroundstyles.tex
 docs/poster-2024-01-15/tikzposterBlockstyles.tex
@@ -30,16 +32,19 @@
 docs/poster-2024-01-15/worker.py
 docs/poster-2024-01-15/logo/lulogo.pdf
 docs/poster-2024-01-15/logo/maxivlogo.pdf
 docs/reference/middlewares.md
 docs/reference/trigger_map.md
 docs/reference/internals/distributed_service.md
 docs/reference/internals/ingester.md
+docs/reference/protocols/STINS.md
+docs/reference/protocols/albaem.md
 docs/reference/protocols/contrast.md
 docs/reference/protocols/events.md
+docs/reference/protocols/sardana.md
 docs/reference/protocols/xspress.md
 docs/seminar-2023-11-30/main.tex
 docs/tutorials/ingesters.md
 docs/tutorials/viewers.md
 dranspose/__init__.py
 dranspose/cli.py
 dranspose/controller.py
@@ -56,52 +61,87 @@
 dranspose.egg-info/PKG-INFO
 dranspose.egg-info/SOURCES.txt
 dranspose.egg-info/dependency_links.txt
 dranspose.egg-info/entry_points.txt
 dranspose.egg-info/requires.txt
 dranspose.egg-info/top_level.txt
 dranspose/data/__init__.py
+dranspose/data/albaem.py
 dranspose/data/contrast.py
+dranspose/data/eiger_legacy.py
+dranspose/data/positioncap.py
 dranspose/data/sardana.py
 dranspose/data/stream1.py
 dranspose/data/xspress3.py
 dranspose/helpers/__init__.py
 dranspose/helpers/jsonpath_slice_ext.py
 dranspose/helpers/utils.py
 dranspose/ingesters/__init__.py
 dranspose/ingesters/http_sardana.py
 dranspose/ingesters/tcp_positioncap.py
+dranspose/ingesters/zmqpull_eiger_legacy.py
 dranspose/ingesters/zmqpull_single.py
+dranspose/ingesters/zmqsub_albaem.py
 dranspose/ingesters/zmqsub_contrast.py
 dranspose/ingesters/zmqsub_xspress3.py
 dranspose/middlewares/__init__.py
 dranspose/middlewares/contrast.py
+dranspose/middlewares/positioncap.py
+dranspose/middlewares/sardana.py
 dranspose/middlewares/stream1.py
 dranspose/middlewares/xspress.py
 examples/dummy/reducer.py
 examples/dummy/worker.py
+examples/parser/positioncap.py
+examples/repub/worker.py
+examples/slow/reducer.py
 examples/slow/worker.py
+perf/.gitignore
+perf/Cargo.lock
+perf/Cargo.toml
+perf/Dockerfile
+perf/src/control_plane.rs
+perf/src/data_plane.rs
+perf/src/dranspose.rs
+perf/src/main.rs
 tests/.gitignore
 tests/__init__.py
 tests/conftest.py
 tests/stream1.py
+tests/test_albaem.py
 tests/test_basics.py
 tests/test_controller.py
 tests/test_data_streams.py
 tests/test_debugworker.py
+tests/test_default_parameters.py
+tests/test_discard_scan.py
 tests/test_dumping.py
+tests/test_eiger_legacy.py
+tests/test_empty_event.py
 tests/test_jsonpath.py
 tests/test_mapping.py
+tests/test_maxrate.py
 tests/test_mulitple_scans.py
+tests/test_outside_scan_push.py
 tests/test_panda.py
 tests/test_param_descriptions.py
 tests/test_parameters.py
 tests/test_processingtime.py
 tests/test_protocol.py
 tests/test_reducer.py
+tests/test_repub.py
+tests/test_restart_ingester.py
+tests/test_restart_worker.py
+tests/test_round_robin.py
+tests/test_rust_ingest.py
 tests/test_sardana_hook.py
 tests/test_sardana_ingester.py
 tests/test_short_scans.py
+tests/test_slowreduce.py
 tests/test_zmq_cancel.py
+tests/test_zmq_multiroute.py
+tests/test_zmq_rate.py
+tests/data/albaem-dump.pkls
 tests/data/contrast-dump.pkls
+tests/data/eiger-small.pkls
 tests/data/xspress3-dump.pkls
 tests/data/xspress3mini-dump20.pkls
```

### Comparing `dranspose-0.0.2/examples/dummy/reducer.py` & `dranspose-0.0.3/examples/dummy/reducer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dranspose.event import ResultData
 from dranspose.parameters import StrParameter, FileParameter
 
 
 class FluorescenceReducer:
-    def __init__(self, parameters=None):
+    def __init__(self, **kwargs):
         self.number = 0
         self.publish = {"map": {}}
 
     @staticmethod
     def describe_parameters():
         params = [
             StrParameter(name="string_parameter"),
@@ -17,7 +17,10 @@
 
     def process_result(self, result: ResultData, parameters=None):
         print(result)
         if result.payload:
             self.publish["map"][result.payload["position"]] = result.payload[
                 "concentations"
             ]
+
+    def finish(self, parameters=None):
+        print("finished dummy reducer work")
```

### Comparing `dranspose-0.0.2/examples/dummy/worker.py` & `dranspose-0.0.3/examples/dummy/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from dranspose.middlewares import xspress
 from dranspose.parameters import StrParameter, FileParameter
 
 logger = logging.getLogger(__name__)
 
 
 class FluorescenceWorker:
-    def __init__(self, parameters=None):
+    def __init__(self, **kwargs):
         self.number = 0
 
     @staticmethod
     def describe_parameters():
         params = [
-            StrParameter(name="roi1"),
+            StrParameter(name="roi1", default="bla"),
             FileParameter(name="file_parameter"),
         ]
         return params
 
     def process_event(self, event: EventData, parameters=None):
         logger.debug("using parameters %s", parameters)
         roi_slice = json.loads(parameters["roi1"].data)
```

### Comparing `dranspose-0.0.2/examples/slow/worker.py` & `dranspose-0.0.3/examples/slow/worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 from dranspose.event import EventData
 from dranspose.parameters import FloatParameter
 
 logger = logging.getLogger(__name__)
 
 
 class SlowWorker:
-    def __init__(self, parameters=None):
+    def __init__(self, **kwargs):
         pass
 
     @staticmethod
     def describe_parameters():
         params = [
             FloatParameter(name="sleep_time"),
         ]
         return params
 
     def process_event(self, event: EventData, parameters=None):
         logger.debug("using parameters %s", parameters)
         if "sleep_time" in parameters:
-            time.sleep(float(parameters["sleep_time"]))
+            time.sleep(parameters["sleep_time"].value)
         else:
             time.sleep(0.28)
+        return "not empty"
```

### Comparing `dranspose-0.0.2/pyproject.toml` & `dranspose-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/conftest.py` & `dranspose-0.0.3/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,211 @@
 import asyncio
 import json
 import logging
+import multiprocessing
 import os
 import pickle
 import random
-from asyncio import StreamReader, StreamWriter
+import struct
+import time
+from asyncio import StreamReader, StreamWriter, Task
+from dataclasses import dataclass
+from multiprocessing import Process
 from typing import (
     Coroutine,
     AsyncIterator,
     Callable,
     Any,
     Optional,
 )
 
 import aiohttp
 import numpy as np
 import pytest_asyncio
 import uvicorn
 import zmq
+from _pytest.fixtures import FixtureRequest
 from fastapi import FastAPI
 from pydantic import HttpUrl
 from pydantic_core import Url
 
 from dranspose.controller import app
-from dranspose.ingester import Ingester
+from dranspose.distributed import DistributedService
+from dranspose.helpers.utils import cancel_and_wait
+from dranspose.ingester import Ingester, IngesterSettings
+from dranspose.ingesters.zmqpull_single import ZmqPullSingleIngester
 from dranspose.protocol import WorkerName
 from dranspose.worker import Worker, WorkerSettings
 from dranspose.reducer import app as reducer_app
 from dranspose.debug_worker import app as debugworker_app
 from tests.stream1 import AcquisitionSocket
 
+from pytest import Parser
+
+
+def pytest_addoption(parser: Parser) -> None:
+    parser.addoption(
+        "--rust",
+        action="store_true",
+        dest="rust",
+        default=False,
+        help="enable rust decorated tests",
+    )
+
 
 @pytest_asyncio.fixture()
 async def controller() -> AsyncIterator[None]:
     config = uvicorn.Config(app, port=5000, log_level="debug")
     server = uvicorn.Server(config)
     server_task = asyncio.create_task(server.serve())
     while server.started is False:
         await asyncio.sleep(0.1)
     yield
     server.should_exit = True
     await server_task
     await asyncio.sleep(0.1)
 
 
+@dataclass
+class AsyncDistributed:
+    instance: DistributedService
+    task: Task[Any]
+
+    async def stop(self) -> None:
+        await self.instance.close()
+        await cancel_and_wait(self.task)
+
+
+@dataclass
+class ProcessDistributed:
+    instance: DistributedService
+    process: multiprocessing.Process
+    queue: Any
+
+    async def stop(self) -> None:
+        self.queue.put("stop")
+        self.process.join()
+
+
+@dataclass
+class ExternalDistributed:
+    instance: DistributedService
+    process: asyncio.subprocess.Process
+    log_task: Task[Any]
+
+    async def stop(self) -> None:
+        logging.warning("stopping process")
+        self.process.terminate()
+        await self.process.wait()
+        logging.warning("stopping log task")
+        self.log_task.cancel()
+
+
 @pytest_asyncio.fixture
 async def create_worker() -> AsyncIterator[
     Callable[[WorkerName], Coroutine[None, None, Worker]]
 ]:
-    workers = []
+    workers: list[AsyncDistributed | ProcessDistributed] = []
 
-    async def _make_worker(name: WorkerName | Worker) -> Worker:
+    async def _make_worker(
+        name: WorkerName | Worker, subprocess: bool = False
+    ) -> Worker:
         if not isinstance(name, Worker):
             worker = Worker(WorkerSettings(worker_name=name))
         else:
             worker = name
-        worker_task = asyncio.create_task(worker.run())
-        workers.append((worker, worker_task))
+
+        if subprocess:
+            q: Any = multiprocessing.Queue()
+            p = Process(target=worker.sync_run, args=(q,), daemon=True)
+            p.start()
+            workers.append(ProcessDistributed(instance=worker, process=p, queue=q))
+        else:
+            worker_task = asyncio.create_task(worker.run())
+            workers.append(AsyncDistributed(instance=worker, task=worker_task))
+
         return worker
 
     yield _make_worker
 
-    for worker, task in workers:
-        await worker.close()
-        task.cancel()
+    for wo in workers:
+        await wo.stop()
 
 
 @pytest_asyncio.fixture
-async def create_ingester() -> AsyncIterator[
-    Callable[[Ingester], Coroutine[None, None, Ingester]]
-]:
-    ingesters = []
+async def create_ingester(
+    request: FixtureRequest,
+) -> AsyncIterator[Callable[[Ingester], Coroutine[None, None, Ingester]]]:
+    ingesters: list[AsyncDistributed | ProcessDistributed | ExternalDistributed] = []
 
-    async def _make_ingester(inst: Ingester) -> Ingester:
-        ingester_task = asyncio.create_task(inst.run())
-        ingesters.append((inst, ingester_task))
+    async def forward_pipe(
+        out: StreamReader | None, settings: IngesterSettings
+    ) -> None:
+        if out is None:
+            return
+        while True:
+            try:
+                data = await out.readline()
+                line = data.decode("ascii").rstrip()
+                if len(line) > 0:
+                    fn = logging.error
+                    parts = line.split("]")
+                    if len(parts) > 1:
+                        if "INFO" in parts[0]:
+                            fn = logging.info
+                        elif "DEBUG" in parts[0]:
+                            fn = logging.debug
+                        # line = "]".join(parts[1:])
+                    fn("rust_%s: %s", settings.ingester_streams[0], line)
+                else:
+                    break
+            except Exception as e:
+                logging.error("outputing broke %s", e.__repr__())
+                break
+
+    async def _make_ingester(inst: Ingester, subprocess: bool = False) -> Ingester:
+        if request.config.getoption("rust"):
+            logging.warning("replace ingester with rust")
+            if isinstance(inst, ZmqPullSingleIngester):
+                logging.warning("ues settings %s", inst._streaming_single_settings)
+                proc = await asyncio.create_subprocess_exec(
+                    "./perf/target/debug/fast_ingester",
+                    "--stream",
+                    inst._streaming_single_settings.ingester_streams[0],
+                    "--upstream-url",
+                    str(inst._streaming_single_settings.upstream_url),
+                    "--ingester-url",
+                    str(inst._streaming_single_settings.ingester_url),
+                    stdout=asyncio.subprocess.PIPE,
+                    stderr=asyncio.subprocess.PIPE,
+                )
+                output = asyncio.create_task(
+                    forward_pipe(proc.stdout, inst._streaming_single_settings)
+                )
+                output = asyncio.create_task(
+                    forward_pipe(proc.stderr, inst._streaming_single_settings)
+                )
+                ingesters.append(
+                    ExternalDistributed(instance=inst, process=proc, log_task=output)
+                )
+                return inst
+        if subprocess:
+            q: Any = multiprocessing.Queue()
+            p = Process(target=inst.sync_run, args=(q,), daemon=True)
+            p.start()
+            ingesters.append(ProcessDistributed(instance=inst, process=p, queue=q))
+        else:
+            ingester_task = asyncio.create_task(inst.run())
+            ingesters.append(AsyncDistributed(instance=inst, task=ingester_task))
         return inst
 
     yield _make_ingester
 
-    for inst, task in ingesters:
-        await inst.close()
-        task.cancel()
+    for ing in ingesters:
+        await ing.stop()
 
 
 @pytest_asyncio.fixture()
 async def reducer(
     tmp_path: Any,
 ) -> AsyncIterator[Callable[[Optional[str]], Coroutine[None, None, None]]]:
     server_tasks = []
@@ -104,14 +224,16 @@
         config = uvicorn.Config(
             reducer_app, port=5001, log_level="debug", env_file=envfile
         )
         server = uvicorn.Server(config)
         server_tasks.append((server, asyncio.create_task(server.serve())))
         while server.started is False:
             await asyncio.sleep(0.1)
+        if custom:
+            del os.environ["REDUCER_CLASS"]
 
     yield start_reducer
 
     for server, task in server_tasks:
         server.should_exit = True
         await task
 
@@ -302,31 +424,81 @@
         await acq.close()
         await socket.close()
 
     return _make_orca
 
 
 @pytest_asyncio.fixture
-async def stream_alba() -> Callable[
-    [zmq.Context[Any], int, int], Coroutine[Any, Any, None]
+async def stream_small() -> Callable[
+    [zmq.Context[Any], int | str, int], Coroutine[Any, Any, None]
 ]:
-    async def _make_alba(ctx: zmq.Context[Any], port: int, nframes: int) -> None:
-        socket = AcquisitionSocket(ctx, Url(f"tcp://*:{port}"))
+    async def _make_alba(
+        ctx: zmq.Context[Any], port: int | str, nframes: int, frame_time: float = 0.1
+    ) -> None:
+        if type(port) is str:
+            socket = AcquisitionSocket(ctx, Url(port))
+        else:
+            socket = AcquisitionSocket(ctx, Url(f"tcp://*:{port}"))
         acq = await socket.start(filename="")
-        val = np.zeros((0,), dtype=np.float64)
+        val = np.zeros((10000,), dtype=np.float64)
+        start = time.perf_counter()
         for frameno in range(nframes):
             await acq.image(val, val.shape, frameno)
-            await asyncio.sleep(0.1)
+            if frame_time:
+                await asyncio.sleep(frame_time)
+            if frameno % 1000 == 0:
+                end = time.perf_counter()
+                logging.info(
+                    "send 1000 packets took %s: %lf p/s",
+                    end - start,
+                    1000 / (end - start),
+                )
+                start = end
         await acq.close()
         await socket.close()
 
     return _make_alba
 
 
 @pytest_asyncio.fixture
+async def time_beacon() -> Callable[
+    [zmq.Context[Any], int, int], Coroutine[Any, Any, None]
+]:
+    async def _make_time(
+        ctx: zmq.Context[Any],
+        port: int,
+        nframes: int,
+        frame_time: float = 0.1,
+        flags: int = 0,
+    ) -> None:
+        sout = ctx.socket(zmq.PUSH)
+        sout.bind(f"tcp://*:{port}")
+        start = time.perf_counter()
+        for i in range(nframes):
+            data = struct.pack(">d", time.perf_counter())
+            try:
+                await sout.send(data, flags=flags)
+            except zmq.Again:
+                pass
+            if frame_time is not None:
+                await asyncio.sleep(frame_time)
+            if i % 1000 == 0:
+                end = time.perf_counter()
+                logging.info(
+                    "send 1000 time packets took %s: %lf p/s",
+                    end - start,
+                    1000 / (end - start),
+                )
+                start = end
+        sout.close(linger=0)
+
+    return _make_time
+
+
+@pytest_asyncio.fixture
 async def stream_sardana() -> Callable[[HttpUrl, int], Coroutine[Any, Any, None]]:
     async def _make_sardana(url: HttpUrl, nframes: int) -> None:
         async with aiohttp.ClientSession() as session:
             descurl = HttpUrl.build(
                 scheme=url.scheme,
                 username=url.username,
                 password=url.password,
@@ -470,15 +642,15 @@
         logging.warning("started server %s", server.is_serving())
         # async with server:
         #    await server.serve_forever()
 
     yield _make_pcap
 
     for task in server_tasks:
-        task.cancel()
+        await cancel_and_wait(task)
 
 
 multiscan_trace = """
 
 OK
 arm_time: 2023-12-19T08:49:51.103Z
 missed: 0
```

### Comparing `dranspose-0.0.2/tests/data/contrast-dump.pkls` & `dranspose-0.0.3/tests/data/contrast-dump.pkls`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/data/xspress3-dump.pkls` & `dranspose-0.0.3/tests/data/xspress3-dump.pkls`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/data/xspress3mini-dump20.pkls` & `dranspose-0.0.3/tests/data/xspress3mini-dump20.pkls`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/stream1.py` & `dranspose-0.0.3/tests/stream1.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_basics.py` & `dranspose-0.0.3/tests/test_basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
     )
 
     r = redis.Redis(host="localhost", port=6379, decode_responses=True, protocol=3)
 
     async with aiohttp.ClientSession() as session:
         st = await session.get("http://localhost:5000/api/v1/config")
         state = EnsembleState.model_validate(await st.json())
-        while {"eiger"} - set(state.get_streams()) != set():
+        while {"eiger"} - set(state.get_streams()) != set() or {"w1"} - set(
+            state.get_workers()
+        ) != set():
             await asyncio.sleep(0.3)
             st = await session.get("http://localhost:5000/api/v1/config")
             state = EnsembleState.model_validate(await st.json())
 
         ntrig = 10
         resp = await session.post(
             "http://localhost:5000/api/v1/mapping",
@@ -103,15 +105,15 @@
 async def test_map(
     controller: None,
     reducer: Callable[[Optional[str]], Awaitable[None]],
     create_worker: Callable[[WorkerName], Awaitable[Worker]],
     create_ingester: Callable[[Ingester], Awaitable[Ingester]],
     stream_eiger: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
     stream_orca: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
-    stream_alba: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
+    stream_small: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
 ) -> None:
     await reducer(None)
     await create_worker(WorkerName("w1"))
     await create_worker(WorkerName("w2"))
     await create_worker(WorkerName("w3"))
     await create_ingester(
         ZmqPullSingleIngester(
@@ -219,16 +221,16 @@
     print("presentkeys", present_keys)
     assert present_keys - set(keys) == set()
 
     context = zmq.asyncio.Context()
 
     asyncio.create_task(stream_eiger(context, 9999, ntrig - 1))
     asyncio.create_task(stream_orca(context, 9998, ntrig - 1))
-    asyncio.create_task(stream_alba(context, 9997, ntrig - 1))
-    asyncio.create_task(stream_alba(context, 9996, ntrig // 4))
+    asyncio.create_task(stream_small(context, 9997, ntrig - 1))
+    asyncio.create_task(stream_small(context, 9996, ntrig // 4))
 
     async with aiohttp.ClientSession() as session:
         st = await session.get("http://localhost:5000/api/v1/progress")
         content = await st.json()
         while not content["finished"]:
             await asyncio.sleep(0.3)
             st = await session.get("http://localhost:5000/api/v1/progress")
```

### Comparing `dranspose-0.0.2/tests/test_controller.py` & `dranspose-0.0.3/tests/test_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,17 @@
                             mode="json"
                         )
                     ]
                     for i in range(1, ntrig)
                 ],
             },
         )
-        assert resp.status == 200
+        assert resp.status == 400
         response = await resp.json()
-        assert "streams {'eiger'} not available" == response
+        assert {"detail": "streams {'eiger'} not available"} == response
 
 
 @pytest.mark.asyncio
 async def test_not_enough_workers(
     controller: None, create_ingester: Callable[[Ingester], Awaitable[Ingester]]
 ) -> None:
     await create_ingester(
@@ -80,10 +80,10 @@
                             mode="json"
                         )
                     ]
                     for i in range(1, ntrig)
                 ],
             },
         )
-        assert resp.status == 200
+        assert resp.status == 400
         response = await resp.json()
-        assert "only 0 workers available, but 1 required" == response
+        assert {"detail": "only 0 workers available, but 1 required"} == response
```

### Comparing `dranspose-0.0.2/tests/test_debugworker.py` & `dranspose-0.0.3/tests/test_debugworker.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_dumping.py` & `dranspose-0.0.3/tests/test_dumping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import logging
 import pickle
 from typing import Awaitable, Callable, Any, Coroutine, Optional
 
 import aiohttp
 
 import pytest
 import zmq.asyncio
@@ -25,23 +26,24 @@
 )
 
 import redis.asyncio as redis
 
 from dranspose.worker import Worker
 
 
+@pytest.mark.skipif("config.getoption('rust')", reason="rust does not support dumping")
 @pytest.mark.asyncio
 async def test_dump(
     controller: None,
     reducer: Callable[[Optional[str]], Awaitable[None]],
     create_worker: Callable[[WorkerName], Awaitable[Worker]],
     create_ingester: Callable[[Ingester], Awaitable[Ingester]],
     stream_eiger: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
     stream_orca: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
-    stream_alba: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
+    stream_small: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]],
     tmp_path: Any,
 ) -> None:
     await reducer(None)
     await create_worker(WorkerName("w1"))
     await create_worker(WorkerName("w2"))
     await create_worker(WorkerName("w3"))
 
@@ -86,21 +88,31 @@
     )
 
     r = redis.Redis(host="localhost", port=6379, decode_responses=True, protocol=3)
 
     async with aiohttp.ClientSession() as session:
         st = await session.get("http://localhost:5000/api/v1/config")
         state = EnsembleState.model_validate(await st.json())
-        print("content", state.ingesters)
+        logging.debug("content %s", state)
         while {"eiger", "orca", "alba", "slow"} - set(state.get_streams()) != set():
             await asyncio.sleep(0.3)
             st = await session.get("http://localhost:5000/api/v1/config")
             state = EnsembleState.model_validate(await st.json())
 
-        print("startup done")
+        logging.info("startup done")
+
+        p_prefix = tmp_path / "dump_"
+        logging.info("prefix is %s encoded: %s", p_prefix, str(p_prefix).encode("utf8"))
+
+        resp = await session.post(
+            "http://localhost:5000/api/v1/parameter/dump_prefix",
+            data=str(p_prefix).encode("utf8"),
+        )
+        assert resp.status == 200
+
         ntrig = 10
         resp = await session.post(
             "http://localhost:5000/api/v1/mapping",
             json={
                 "eiger": [
                     [
                         VirtualWorker(constraint=VirtualConstraint(2 * i)).model_dump(
@@ -155,16 +167,16 @@
     print("presentkeys", present_keys)
     assert present_keys - set(keys) == set()
 
     context = zmq.asyncio.Context()
 
     asyncio.create_task(stream_eiger(context, 9999, ntrig - 1))
     asyncio.create_task(stream_orca(context, 9998, ntrig - 1))
-    asyncio.create_task(stream_alba(context, 9997, ntrig - 1))
-    asyncio.create_task(stream_alba(context, 9996, ntrig // 4))
+    asyncio.create_task(stream_small(context, 9997, ntrig - 1))
+    asyncio.create_task(stream_small(context, 9996, ntrig // 4))
 
     async with aiohttp.ClientSession() as session:
         st = await session.get("http://localhost:5000/api/v1/progress")
         content = await st.json()
         while not content["finished"]:
             await asyncio.sleep(0.3)
             st = await session.get("http://localhost:5000/api/v1/progress")
@@ -179,13 +191,27 @@
                 evs.append(dat.event_number)
                 print("loaded dump type", type(dat))
             except EOFError:
                 break
 
     print(evs)
     assert evs == list(range(0, ntrig + 1))
+
+    # read prefix dump
+    with open(f"{p_prefix}orca-ingester-{uuid}.pkls", "rb") as f:
+        evs = []
+        while True:
+            try:
+                dat = pickle.load(f)
+                evs.append(dat.event_number)
+                print("loaded dump type", type(dat))
+            except EOFError:
+                break
+
+    print(evs)
+    assert evs == list(range(0, ntrig + 1))
 
     context.destroy()
 
     await r.aclose()
 
     print(content)
```

### Comparing `dranspose-0.0.2/tests/test_jsonpath.py` & `dranspose-0.0.3/tests/test_jsonpath.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_mapping.py` & `dranspose-0.0.3/tests/test_mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,14 +54,114 @@
 
     m.assign_next(all_workers[0], all_workers)
 
     assign = m.get_event_workers(EventNumber(8))
     assert assign.assignments[StreamName("test")] == [WorkerName("w1")]
 
 
+def test_discard() -> None:
+    ntrig = 10
+    m = Mapping(
+        {StreamName("test"): [[] for i in range(ntrig)]},
+        add_start_end=False,
+    )
+
+    m.print()
+    all_workers = [
+        WorkerState(name=WorkerName("w1")),
+        WorkerState(name=WorkerName("w2")),
+    ]
+    r = m.assign_next(all_workers[0], all_workers)
+    print(r)
+    r = m.assign_next(all_workers[1], all_workers)
+    print(r)
+
+    m.print()
+    print("completed", m.complete_events)
+
+    # m.assign_next(all_workers[0], all_workers)
+
+    assign = m.get_event_workers(EventNumber(8))
+    print("assign is", assign)
+    assert assign.assignments == {"test": []}
+
+
+def test_partial_discard() -> None:
+    ntrig = 10
+    m = Mapping(
+        {
+            StreamName("test"): [
+                [VirtualWorker(constraint=VirtualConstraint(i))]
+                if i < 2 or i > 7
+                else []
+                if i < 5
+                else None
+                for i in range(ntrig)
+            ]
+        },
+        add_start_end=False,
+    )
+
+    m.print()
+    all_workers = [
+        WorkerState(name=WorkerName("w1")),
+        WorkerState(name=WorkerName("w2")),
+    ]
+    r = m.assign_next(all_workers[0], all_workers)
+    print(r)
+    r = m.assign_next(all_workers[1], all_workers)
+    print(r)
+    r = m.assign_next(all_workers[0], all_workers)
+    print(r)
+
+    m.print()
+    print("completed", m.complete_events)
+
+    # m.assign_next(all_workers[0], all_workers)
+
+    assign = m.get_event_workers(EventNumber(4))
+    assert assign.assignments == {"test": []}
+    assign = m.get_event_workers(EventNumber(6))
+    assert assign.assignments == {}
+    assign = m.get_event_workers(EventNumber(8))
+    assert assign.assignments == {"test": ["w1"]}
+
+
+def test_discard_only_one() -> None:
+    ntrig = 10
+    m = Mapping(
+        {
+            StreamName("test"): [[] for i in range(ntrig)],
+            StreamName("test2"): [
+                [VirtualWorker(constraint=VirtualConstraint(i))] for i in range(ntrig)
+            ],
+        },
+        add_start_end=False,
+    )
+
+    m.print()
+    all_workers = [
+        WorkerState(name=WorkerName("w1")),
+        WorkerState(name=WorkerName("w2")),
+    ]
+    m.assign_next(all_workers[0], all_workers)
+    m.assign_next(all_workers[1], all_workers)
+
+    m.print()
+    print("completed", m.complete_events)
+
+    with pytest.raises(NotYetAssigned):
+        m.get_event_workers(EventNumber(8))
+
+    m.assign_next(all_workers[0], all_workers)
+
+    assign = m.get_event_workers(EventNumber(2))
+    assert assign.assignments[StreamName("test2")] == [WorkerName("w1")]
+
+
 def test_auto() -> None:
     ntrig = 10
     m = Mapping(
         {
             StreamName("test"): [
                 [VirtualWorker(constraint=VirtualConstraint(i))] if i % 4 == 0 else None
                 for i in range(ntrig)
```

### Comparing `dranspose-0.0.2/tests/test_mulitple_scans.py` & `dranspose-0.0.3/tests/test_mulitple_scans.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_panda.py` & `dranspose-0.0.3/tests/test_panda.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     EnsembleState,
     StreamName,
     WorkerName,
     VirtualWorker,
     VirtualConstraint,
 )
 
-from dranspose.worker import Worker
+from dranspose.worker import Worker, WorkerSettings
 
 
 @pytest.mark.asyncio
 async def test_panda_pcap(
     stream_pcap: Callable[[int], Coroutine[None, None, None]],
 ) -> None:
     ntrig = 10
@@ -39,20 +39,27 @@
     await asyncio.sleep(1)
 
 
 @pytest.mark.asyncio
 async def test_pcapingester(
     controller: None,
     reducer: Callable[[Optional[str]], Awaitable[None]],
-    create_worker: Callable[[WorkerName], Awaitable[Worker]],
+    create_worker: Callable[[Worker], Awaitable[Worker]],
     create_ingester: Callable[[Ingester], Awaitable[Ingester]],
     stream_pcap: Callable[[int], Coroutine[None, None, None]],
 ) -> None:
     await reducer(None)
-    await create_worker(WorkerName("w1"))
+    await create_worker(
+        Worker(
+            settings=WorkerSettings(
+                worker_name=WorkerName("w1"),
+                worker_class="examples.parser.positioncap:PcapWorker",
+            ),
+        )
+    )
     await create_ingester(
         TcpPcapIngester(
             settings=TcpPcapSettings(
                 ingester_streams=[StreamName("pcap")],
                 upstream_url=Url("tcp://localhost:8889"),
             ),
         )
```

### Comparing `dranspose-0.0.2/tests/test_param_descriptions.py` & `dranspose-0.0.3/tests/test_default_parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 
 from dranspose.ingester import Ingester
 from dranspose.ingesters.zmqpull_single import (
     ZmqPullSingleIngester,
     ZmqPullSingleSettings,
 )
-from dranspose.parameters import ParameterList, FileParameter, StrParameter
+from dranspose.parameters import ParameterList
 from dranspose.protocol import WorkerName, StreamName, EnsembleState
 from dranspose.worker import Worker, WorkerSettings
 
 
 @pytest.mark.asyncio
-async def test_params(
+async def test_default_params(
     controller: None,
     reducer: Callable[[Optional[str]], Awaitable[None]],
     create_worker: Callable[[Worker], Awaitable[Worker]],
     create_ingester: Callable[[Ingester], Awaitable[Ingester]],
 ) -> None:
     await reducer("examples.dummy.reducer:FluorescenceReducer")
     await create_worker(
@@ -48,16 +48,23 @@
         state = EnsembleState.model_validate(await st.json())
         while {"eiger"} - set(state.get_streams()) != set():
             await asyncio.sleep(0.3)
             st = await session.get("http://localhost:5000/api/v1/config")
             state = EnsembleState.model_validate(await st.json())
 
         par = await session.get("http://localhost:5000/api/v1/parameters")
+        assert par.status == 200
         params = ParameterList.validate_python(await par.json())
 
         logging.warning("params %s", params)
-        assert params == [
-            FileParameter(name="file_parameter", description=None, dtype="file"),
-            FileParameter(name="other_file_parameter", description=None, dtype="file"),
-            StrParameter(name="roi1", description=None, dtype="str"),
-            StrParameter(name="string_parameter", description=None, dtype="str"),
-        ]
+
+        resp = await session.get(
+            "http://localhost:5000/api/v1/parameter/roi1",
+        )
+        assert resp.status == 200
+        assert await resp.content.read() == b"bla"
+
+        resp = await session.get(
+            "http://localhost:5000/api/v1/parameter/file_parameter",
+        )
+        assert resp.status == 200
+        assert await resp.content.read() == b""
```

### Comparing `dranspose-0.0.2/tests/test_parameters.py` & `dranspose-0.0.3/tests/test_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         par = await session.get("http://localhost:5000/api/v1/parameters")
         assert par.status == 200
         params = ParameterList.validate_python(await par.json())
 
         logging.warning("params %s", params)
 
         resp = await session.post(
-            "http://localhost:5000/api/v1/parameter/roi",
+            "http://localhost:5000/api/v1/parameter/roi1",
             json=[0, 10],
         )
         assert resp.status == 200
 
         resp = await session.post(
             "http://localhost:5000/api/v1/parameter/additional",
             data=b"asdasd",
@@ -77,14 +77,23 @@
         assert await resp.content.read() == b"asdasd"
 
         resp = await session.get(
             "http://localhost:5000/api/v1/parameter/nonexistant",
         )
         assert resp.status == 404
 
+        await asyncio.sleep(3)
+
+        resp = await session.post(
+            "http://localhost:5000/api/v1/parameter/additional",
+            data=b"asdasd",
+        )
+        assert resp.status == 200
+        hash = await resp.json()
+
         st = await session.get("http://localhost:5000/api/v1/config")
         state = EnsembleState.model_validate(await st.json())
         print("state", state)
         while str(state.workers[0].parameters_hash) != hash:
             await asyncio.sleep(0.3)
             st = await session.get("http://localhost:5000/api/v1/config")
             state = EnsembleState.model_validate(await st.json())
```

### Comparing `dranspose-0.0.2/tests/test_processingtime.py` & `dranspose-0.0.3/tests/test_processingtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,19 @@
         st = await session.get("http://localhost:5000/api/v1/config")
         state = EnsembleState.model_validate(await st.json())
         while {"eiger"} - set(state.get_streams()) != set():
             await asyncio.sleep(0.3)
             st = await session.get("http://localhost:5000/api/v1/config")
             state = EnsembleState.model_validate(await st.json())
 
+        await session.post(
+            "http://localhost:5000/api/v1/parameter/sleep_time",
+            data=b"0.28",
+        )
+
         st = await session.get(
             "http://localhost:5000/api/v1/load?intervals=1&intervals=10&scan=True"
         )
         load = await st.json()
         assert load == {}
 
         ntrig = 100
```

### Comparing `dranspose-0.0.2/tests/test_protocol.py` & `dranspose-0.0.3/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_reducer.py` & `dranspose-0.0.3/tests/test_reducer.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_sardana_hook.py` & `dranspose-0.0.3/tests/test_sardana_hook.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_sardana_ingester.py` & `dranspose-0.0.3/tests/test_sardana_ingester.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_short_scans.py` & `dranspose-0.0.3/tests/test_short_scans.py`

 * *Files identical despite different names*

### Comparing `dranspose-0.0.2/tests/test_zmq_cancel.py` & `dranspose-0.0.3/tests/test_zmq_cancel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import asyncio
 import logging
 from typing import Callable, Any, Coroutine
 
 import pytest
 import zmq.asyncio
 
+from dranspose.helpers.utils import cancel_and_wait
+
 
 @pytest.mark.asyncio
 async def test_zmq_cancel(
     stream_eiger: Callable[[zmq.Context[Any], int, int], Coroutine[Any, Any, None]]
 ) -> None:
     async def consume() -> None:
         c = zmq.asyncio.Context()
         s = c.socket(zmq.PULL)
         s.connect("tcp://localhost:9999")
         for i in range(13):
             logging.info("recv %d", i)
             task = s.poll()
             waiting = asyncio.gather(*[task])
             if i == 6:
-                waiting.cancel()
+                await cancel_and_wait(waiting)
                 continue
             done = await waiting
             logging.info("done %s", done)
             data = s.recv_multipart(copy=False)
             logging.info("i %d, data %s", i, data)
         c.destroy()
```

