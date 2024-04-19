# Comparing `tmp/ragu-0.1.29.tar.gz` & `tmp/ragu-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.29.tar", last modified: Fri Mar 29 15:11:08 2024, max compression
+gzip compressed data, was "ragu-0.1.30.tar", last modified: Fri Apr 19 16:36:20 2024, max compression
```

## Comparing `ragu-0.1.29.tar` & `ragu-0.1.30.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.563760 ragu-0.1.29/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.29/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    47206 2024-03-29 15:11:08.563553 ragu-0.1.29/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     5995 2024-02-24 23:44:42.000000 ragu-0.1.29/README.md
--rw-r--r--   0 btober     (501) staff       (20)      942 2024-03-29 15:10:31.000000 ragu-0.1.29/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2024-03-29 15:11:08.563796 ragu-0.1.29/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.29/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.536596 ragu-0.1.29/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.537826 ragu-0.1.29/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.538750 ragu-0.1.29/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.29/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.536743 ragu-0.1.29/src/ragu/dat/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.538875 ragu-0.1.29/src/ragu/dat/mars/
--rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.29/src/ragu/dat/mars/mega90n000eb.tif
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.558187 ragu-0.1.29/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2411 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2454 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     3005 2024-03-29 14:58:23.000000 ragu-0.1.29/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3366 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2562 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2896 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2474 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5780 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14181 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2537 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2931 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3640 2024-03-29 15:04:24.000000 ragu-0.1.29/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.558476 ragu-0.1.29/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    21336 2024-03-29 14:58:23.000000 ragu-0.1.29/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.558932 ragu-0.1.29/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7657 2024-03-29 15:06:16.000000 ragu-0.1.29/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    13365 2024-03-29 15:08:40.000000 ragu-0.1.29/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.561578 ragu-0.1.29/src/ragu/recs/
--rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.29/src/ragu/recs/20190928-235534_compiled.jpg
--rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.29/src/ragu/recs/basemap_icon.png
--rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.29/src/ragu/recs/bulb.jpg
--rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.29/src/ragu/recs/ragu_logo.png
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.562090 ragu-0.1.29/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.563054 ragu-0.1.29/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.29/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    68641 2024-03-29 15:09:02.000000 ragu-0.1.29/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.29/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-03-29 15:11:08.563262 ragu-0.1.29/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    47206 2024-03-29 15:11:08.000000 ragu-0.1.29/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1369 2024-03-29 15:11:08.000000 ragu-0.1.29/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2024-03-29 15:11:08.000000 ragu-0.1.29/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2024-03-29 15:11:08.000000 ragu-0.1.29/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2024-03-29 15:11:08.000000 ragu-0.1.29/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       10 2024-03-29 15:11:08.000000 ragu-0.1.29/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.580006 ragu-0.1.30/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.30/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    47233 2024-04-19 16:36:20.579730 ragu-0.1.30/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     6022 2024-03-29 15:25:52.000000 ragu-0.1.30/README.md
+-rw-r--r--   0 btober     (501) staff       (20)      942 2024-04-19 16:29:45.000000 ragu-0.1.30/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2024-04-19 16:36:20.580078 ragu-0.1.30/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.30/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.522058 ragu-0.1.30/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.524100 ragu-0.1.30/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.526336 ragu-0.1.30/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.522252 ragu-0.1.30/src/ragu/dat/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.526889 ragu-0.1.30/src/ragu/dat/mars/
+-rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/dat/mars/mega90n000eb.tif
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.570591 ragu-0.1.30/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2411 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2454 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     3005 2024-04-05 18:35:16.000000 ragu-0.1.30/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3366 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2562 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2896 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2474 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5780 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14181 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2537 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2931 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3640 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.571337 ragu-0.1.30/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    21336 2024-03-29 14:58:23.000000 ragu-0.1.30/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.572252 ragu-0.1.30/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7657 2024-03-29 15:06:16.000000 ragu-0.1.30/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    14075 2024-04-19 16:27:32.000000 ragu-0.1.30/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.577005 ragu-0.1.30/src/ragu/recs/
+-rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/20190928-235534_compiled.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/basemap_icon.png
+-rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/bulb.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/ragu_logo.png
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.577777 ragu-0.1.30/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.579275 ragu-0.1.30/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    68791 2024-04-19 16:28:48.000000 ragu-0.1.30/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.525744 ragu-0.1.30/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    47233 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1369 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       10 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.29/LICENSE.txt` & `ragu-0.1.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/PKG-INFO` & `ragu-0.1.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.29
+Version: 0.1.30
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,15 @@
 ## What is RAGU?
 RAGU is a user-interface radar interpretation software written in Python 3 and released under the GNU General Public License v3. RAGU was originally developed to ingest and interpret NASA Operation IceBridge airborne radar sounding data, but has been expanded for use with other sounder and ground penetrating radar datasets. While RAGU is primarily an interpretation software, minimal radar processing tools are included with the software.
 
 ### Dataset Capabilities:
 RAGU was originally developed to work with NASA's Operation IceBridge Alaska radar sounding data. The dataset capabilities have since been expanded to include the following:
 
 - NASA OIB-AK
+- Groundhog (UArizona/UAF)
 - CReSIS (Radar Depth Sounder & Snow Radar)
 - SHARAD (USRDR, USGEOM, US clutter sims)
 - MARSIS (JPL multilook products)
 - KAGUYA (SELENE) Lunar Radar Sounder (LRS)
 - RIMFAX
 - GSSI
 - pulseEKKO
```

### Comparing `ragu-0.1.29/README.md` & `ragu-0.1.30/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ## What is RAGU?
 RAGU is a user-interface radar interpretation software written in Python 3 and released under the GNU General Public License v3. RAGU was originally developed to ingest and interpret NASA Operation IceBridge airborne radar sounding data, but has been expanded for use with other sounder and ground penetrating radar datasets. While RAGU is primarily an interpretation software, minimal radar processing tools are included with the software.
 
 ### Dataset Capabilities:
 RAGU was originally developed to work with NASA's Operation IceBridge Alaska radar sounding data. The dataset capabilities have since been expanded to include the following:
 
 - NASA OIB-AK
+- Groundhog (UArizona/UAF)
 - CReSIS (Radar Depth Sounder & Snow Radar)
 - SHARAD (USRDR, USGEOM, US clutter sims)
 - MARSIS (JPL multilook products)
 - KAGUYA (SELENE) Lunar Radar Sounder (LRS)
 - RIMFAX
 - GSSI
 - pulseEKKO
```

### Comparing `ragu-0.1.29/pyproject.toml` & `ragu-0.1.30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ragu"
-version = "0.1.29"
+version = "0.1.30"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
      {name = "Brandon Tober", email = "tobers.brandon@gmail.com"},
      {name = "Michael Christoffersen", email = "mchristo28@gmail.com"},
```

### Comparing `ragu-0.1.29/src/ragu/bin/ragu.py` & `ragu-0.1.30/src/ragu/bin/ragu.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/config.py` & `ragu-0.1.30/src/ragu/config.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/dat/mars/mega90n000eb.tif` & `ragu-0.1.30/src/ragu/dat/mars/mega90n000eb.tif`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/__init__.py` & `ragu-0.1.30/src/ragu/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.30/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.30/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.30/src/ragu/ingest/ingest_groundhog.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.30/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.30/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.30/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.30/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.30/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.30/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.30/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.30/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_template.py` & `ragu-0.1.30/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.30/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/nav/gps.py` & `ragu-0.1.30/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/nav/navparse.py` & `ragu-0.1.30/src/ragu/nav/navparse.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/radar/__init__.py` & `ragu-0.1.30/src/ragu/radar/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/radar/pick.py` & `ragu-0.1.30/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/radar/processing.py` & `ragu-0.1.30/src/ragu/radar/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,63 +245,78 @@
     # log
     self.log("self.rdata.filter(btype='{}', lowcut={}, highcut={}, order={}, direction={})".format(btype, lowcut, highcut, order, direction))
     print("# filter applied: btype='{}', lowcut={}, highcut={}, order={}, direction={}".format(btype, lowcut, highcut, order, direction))
 
     return
 
 
-def restack(self, intrvl=None):
+def restack(self, intrvl=None,thold=None):
+    # get coordinate transformation
+    xform = pyproj.Transformer.from_crs(self.geocrs, self.xyzcrs)
+
     # restack radar data to specified along-track distance
     amp = self.proc.get_curr_amp()
     self.proc.set_prev_amp(amp)
+    navdf = self.navdf.copy()
+    # first account for any static traces where there may be gps drift
+    if thold > 0:
+        consecutive_dist = np.zeros_like(self.navdf.x)
+        consecutive_dist[1:] = np.sqrt(np.diff(self.navdf.x.to_numpy()) ** 2.0 + np.diff(self.navdf.y.to_numpy()) ** 2.0 + np.diff(self.navdf.z.to_numpy()) ** 2.0)
+        drift_mask = consecutive_dist >= thold
+
+        # drop data from these traces
+        namp = amp[:,drift_mask]
+        navdf = navdf[drift_mask]
+        navdf["dist"] = navparse.euclid_dist(navdf["x"], navdf["y"], navdf["z"])
+        self.snum, self.tnum = namp.shape
+        amp = namp
 
-    totdist = self.navdf.dist.iloc[-1]  # Total distance
+    totdist = navdf.dist.iloc[-1]  # Total distance
     ntrace = int(totdist//intrvl)
 
     rstack = np.zeros((self.snum, ntrace))
     lat = np.zeros(ntrace)
     lon = np.zeros(ntrace)
     hgt = np.zeros(ntrace)
 
     for i in range(ntrace):
-        stack_slice = np.logical_and(self.navdf.dist > i*intrvl, self.navdf.dist < (i+1)*intrvl)
+        stack_slice = np.logical_and(navdf.dist > i*intrvl, navdf.dist < (i+1)*intrvl)
         nstack = np.sum(stack_slice)
         if(nstack == 0):
             rstack[:, i] = rstack[:, i-1]
             lat[i] = lat[i-1]
             lon[i] = lon[i-1]
             hgt[i] = hgt[i-1]
             continue
 
         rstack[:, i] = np.sum(amp[:, stack_slice], axis=1)/nstack
-        lat[i] = np.mean(self.navdf["lat"][stack_slice])
-        lon[i] = np.mean(self.navdf["lon"][stack_slice])
-        hgt[i] = np.mean(self.navdf["elev"][stack_slice])
+        lat[i] = np.mean(navdf["lat"][stack_slice])
+        lon[i] = np.mean(navdf["lon"][stack_slice])
+        hgt[i] = np.mean(navdf["elev"][stack_slice])
 
     # store twtt_wind from navdf before cleaning up
-    twtt_wind_ = self.navdf["twtt_wind"]
+    twtt_wind_ = navdf["twtt_wind"]
     # store updated nav data
     self.navdf = pd.DataFrame()
     self.navdf["lon"] = lon
     self.navdf["lat"] = lat
     self.navdf["elev"] = hgt
 
-    xform = pyproj.Transformer.from_crs(self.geocrs, self.xyzcrs)
     self.navdf["x"], self.navdf["y"], self.navdf["z"] = xform.transform(self.navdf["lon"], self.navdf["lat"], self.navdf["elev"])
     self.navdf["dist"] = navparse.euclid_dist(self.navdf["x"], self.navdf["y"], self.navdf["z"])
     if (twtt_wind_ == 0.0).all():
         self.navdf["twtt_wind"] = 0.0
     else:
         self.navdf["twtt_wind"] = np.nan
 
     self.snum, self.tnum = rstack.shape
     self.set_proc(rstack)
     # log
-    self.log("self.rdata.restack(intrvl={})".format(intrvl))
-    print("# data restacked at an interval of {} m".format(intrvl))
+    self.log("self.rdata.restack(intrvl={},thold={})".format(intrvl,thold))
+    print("# data restacked at an interval of {} m, with a minimum distance threshold of {} m".format(intrvl,thold))
     
     return
 
 
 def tpowGain(self, power):
     # t-power gain to each trace with the given exponent.
     amp = self.proc.get_curr_amp()
```

### Comparing `ragu-0.1.29/src/ragu/recs/20190928-235534_compiled.jpg` & `ragu-0.1.30/src/ragu/recs/20190928-235534_compiled.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/recs/basemap_icon.png` & `ragu-0.1.30/src/ragu/recs/basemap_icon.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/recs/bulb.jpg` & `ragu-0.1.30/src/ragu/recs/bulb.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/recs/ragu_logo.png` & `ragu-0.1.30/src/ragu/recs/ragu_logo.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/tools/export.py` & `ragu-0.1.30/src/ragu/tools/export.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/tools/utils.py` & `ragu-0.1.30/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ui/basemap.py` & `ragu-0.1.30/src/ragu/ui/basemap.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ui/gui.py` & `ragu-0.1.30/src/ragu/ui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1027,16 +1027,17 @@
 
             elif arg == "vroll":
                 samples = tk.simpledialog.askinteger("input","number of samples to roll data array")
                 self.rdata.vertical_roll(samples)
                 procFlag = True
 
             elif arg == "restack":
-                dist = tk.simpledialog.askinteger("input","restacking distance (m)")
-                self.rdata.restack(dist)
+                thold = tk.simpledialog.askfloat("input","GPS drift threshold between consecutive traces (m)", initialvalue=0.5)
+                dist = tk.simpledialog.askfloat("input","restacking distance (m)", initialvalue=0)
+                self.rdata.restack(dist, thold)
                 procFlag = True
 
             elif arg == "dewow":
                 print("dewow currently in development")
                 # window = tk.simpledialog.askfloat("input","dewow window size (# samples/" +  str(int(self.rdata.snum)) + ")?")
                 # proc = processing.dewow(self.rdata.dat, window=10)
                 # procFlag = True
```

### Comparing `ragu-0.1.29/src/ragu/ui/impick.py` & `ragu-0.1.30/src/ragu/ui/impick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ui/notepad.py` & `ragu-0.1.30/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu/ui/wvpick.py` & `ragu-0.1.30/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.29/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.30/src/ragu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.29
+Version: 0.1.30
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,15 @@
 ## What is RAGU?
 RAGU is a user-interface radar interpretation software written in Python 3 and released under the GNU General Public License v3. RAGU was originally developed to ingest and interpret NASA Operation IceBridge airborne radar sounding data, but has been expanded for use with other sounder and ground penetrating radar datasets. While RAGU is primarily an interpretation software, minimal radar processing tools are included with the software.
 
 ### Dataset Capabilities:
 RAGU was originally developed to work with NASA's Operation IceBridge Alaska radar sounding data. The dataset capabilities have since been expanded to include the following:
 
 - NASA OIB-AK
+- Groundhog (UArizona/UAF)
 - CReSIS (Radar Depth Sounder & Snow Radar)
 - SHARAD (USRDR, USGEOM, US clutter sims)
 - MARSIS (JPL multilook products)
 - KAGUYA (SELENE) Lunar Radar Sounder (LRS)
 - RIMFAX
 - GSSI
 - pulseEKKO
```

### Comparing `ragu-0.1.29/src/ragu.egg-info/SOURCES.txt` & `ragu-0.1.30/src/ragu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

