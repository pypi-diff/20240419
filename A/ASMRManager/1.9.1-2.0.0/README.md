# Comparing `tmp/asmrmanager-1.9.1.tar.gz` & `tmp/asmrmanager-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmrmanager-1.9.1.tar", last modified: Sat Mar 30 06:46:06 2024, max compression
+gzip compressed data, was "asmrmanager-2.0.0.tar", last modified: Fri Apr 19 17:51:35 2024, max compression
```

## Comparing `asmrmanager-1.9.1.tar` & `asmrmanager-2.0.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0     1065 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/LICENSE
--rw-r--r--   0        0        0     6953 2024-03-10 15:25:20.988269 asmrmanager-1.9.1/README.md
--rw-r--r--   0        0        0      269 2023-12-29 06:07:22.402888 asmrmanager-1.9.1/asmrmanager/__init__.py
--rw-r--r--   0        0        0       46 2024-01-30 08:57:30.179230 asmrmanager-1.9.1/asmrmanager/__main__.py
--rw-r--r--   0        0        0       21 2024-03-30 06:46:06.449284 asmrmanager-1.9.1/asmrmanager/_version.py
--rw-r--r--   0        0        0    10557 2024-03-14 05:42:14.862697 asmrmanager-1.9.1/asmrmanager/cli/core.py
--rw-r--r--   0        0        0     5466 2024-02-27 08:47:35.786130 asmrmanager-1.9.1/asmrmanager/cli/dl.py
--rw-r--r--   0        0        0     6063 2024-03-08 04:02:26.986301 asmrmanager-1.9.1/asmrmanager/cli/file.py
--rw-r--r--   0        0        0      530 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/cli/hold.py
--rw-r--r--   0        0        0     1656 2024-01-30 12:35:12.948712 asmrmanager-1.9.1/asmrmanager/cli/info.py
--rw-r--r--   0        0        0     1996 2024-02-19 16:39:42.712693 asmrmanager-1.9.1/asmrmanager/cli/main.py
--rw-r--r--   0        0        0     2354 2024-01-13 17:56:02.338104 asmrmanager-1.9.1/asmrmanager/cli/pl.py
--rw-r--r--   0        0        0      967 2024-03-30 06:44:45.749287 asmrmanager-1.9.1/asmrmanager/cli/play.py
--rw-r--r--   0        0        0     1598 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/cli/query.py
--rw-r--r--   0        0        0      919 2023-12-18 03:28:37.596535 asmrmanager-1.9.1/asmrmanager/cli/review.py
--rw-r--r--   0        0        0     2140 2024-01-13 17:33:20.948158 asmrmanager-1.9.1/asmrmanager/cli/sql.py
--rw-r--r--   0        0        0     1805 2024-03-30 06:44:45.759287 asmrmanager-1.9.1/asmrmanager/cli/view.py
--rw-r--r--   0        0        0      890 2024-01-30 05:59:06.229650 asmrmanager-1.9.1/asmrmanager/cli/which.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/common/__init__.py
--rw-r--r--   0        0        0      821 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/common/browse_params.py
--rw-r--r--   0        0        0      527 2023-12-21 14:14:16.443072 asmrmanager-1.9.1/asmrmanager/common/download_params.py
--rw-r--r--   0        0        0      612 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/common/output.py
--rw-r--r--   0        0        0      719 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/common/parse_filter.py
--rw-r--r--   0        0        0      867 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/common/rj_parse.py
--rw-r--r--   0        0        0      913 2024-03-29 06:19:00.412674 asmrmanager-1.9.1/asmrmanager/common/select.py
--rw-r--r--   0        0        0      770 2024-03-08 04:02:26.946301 asmrmanager-1.9.1/asmrmanager/common/types.py
--rw-r--r--   0        0        0     1331 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/common/vtt2lrc.py
--rw-r--r--   0        0        0     2637 2024-03-14 05:43:28.099361 asmrmanager-1.9.1/asmrmanager/config.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/database/__init__.py
--rw-r--r--   0        0        0     2258 2023-12-21 13:15:18.463211 asmrmanager-1.9.1/asmrmanager/database/database.py
--rw-r--r--   0        0        0      343 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/database/engine.py
--rw-r--r--   0        0        0     4964 2023-12-24 08:26:10.979470 asmrmanager-1.9.1/asmrmanager/database/manage.py
--rw-r--r--   0        0        0      592 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/database/orm_type.py
--rw-r--r--   0        0        0      972 2023-12-24 08:21:53.859480 asmrmanager-1.9.1/asmrmanager/database/q_func.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/database/utils/__init__.py
--rw-r--r--   0        0        0      480 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/database/utils/add2db.py
--rw-r--r--   0        0        0     1290 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/database/utils/uuid_sqlite.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/filemanager/__init__.py
--rw-r--r--   0        0        0      312 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/filemanager/appdirs_.py
--rw-r--r--   0        0        0      108 2023-12-17 15:01:39.136126 asmrmanager-1.9.1/asmrmanager/filemanager/exceptions.py
--rw-r--r--   0        0        0      477 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/filemanager/file_zipper.py
--rw-r--r--   0        0        0    11707 2024-03-30 06:44:45.855954 asmrmanager-1.9.1/asmrmanager/filemanager/manager.py
--rw-r--r--   0        0        0     3194 2024-03-14 05:39:35.879370 asmrmanager-1.9.1/asmrmanager/filemanager/resources/config.example.toml
--rw-r--r--   0        0        0       65 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/circle_name.sql
--rw-r--r--   0        0        0      425 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/score.sql
--rw-r--r--   0        0        0     1663 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/search.sql
--rw-r--r--   0        0        0       92 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/tags.sql
--rw-r--r--   0        0        0      602 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/test.sql
--rw-r--r--   0        0        0       53 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/vas.sql
--rw-r--r--   0        0        0     1579 2024-03-29 06:23:40.599330 asmrmanager-1.9.1/asmrmanager/filemanager/utils.py
--rw-r--r--   0        0        0     1038 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/logger/__init__.py
--rw-r--r--   0        0        0       68 2023-12-24 08:26:10.649470 asmrmanager-1.9.1/asmrmanager/lrcplayer/__init__.py
--rw-r--r--   0        0        0     2318 2023-12-31 11:19:36.902077 asmrmanager-1.9.1/asmrmanager/lrcplayer/lrcparse.py
--rw-r--r--   0        0        0      328 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/lrcplayer/main.css
--rw-r--r--   0        0        0     5052 2024-01-06 08:17:52.872546 asmrmanager-1.9.1/asmrmanager/lrcplayer/main.py
--rw-r--r--   0        0        0     3845 2023-12-31 11:19:36.902077 asmrmanager-1.9.1/asmrmanager/lrcplayer/player/base.py
--rw-r--r--   0        0        0     4292 2024-01-06 16:43:32.998016 asmrmanager-1.9.1/asmrmanager/lrcplayer/player/mpdplayer.py
--rw-r--r--   0        0        0     1777 2023-12-31 11:19:36.902077 asmrmanager-1.9.1/asmrmanager/lrcplayer/player/pygameplayer.py
--rw-r--r--   0        0        0       75 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/spider/__init__.py
--rw-r--r--   0        0        0     5225 2024-03-30 06:44:45.789287 asmrmanager-1.9.1/asmrmanager/spider/asmrapi.py
--rw-r--r--   0        0        0    10003 2024-03-30 06:44:45.825954 asmrmanager-1.9.1/asmrmanager/spider/downloader.py
--rw-r--r--   0        0        0     9076 2024-03-30 06:44:45.832621 asmrmanager-1.9.1/asmrmanager/spider/interface.py
--rw-r--r--   0        0        0     1849 2024-03-30 06:44:45.785954 asmrmanager-1.9.1/asmrmanager/spider/playlist.py
--rw-r--r--   0        0        0     4092 2023-12-17 15:01:39.139459 asmrmanager-1.9.1/asmrmanager/spider/utils/IDMHelper.py
--rw-r--r--   0        0        0     1355 2024-03-30 06:44:45.769287 asmrmanager-1.9.1/asmrmanager/spider/utils/aria2_downloader.py
--rw-r--r--   0        0        0     1527 2024-03-30 06:46:06.455951 asmrmanager-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     8329 1970-01-01 00:00:00.000000 asmrmanager-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/LICENSE
+-rw-r--r--   0        0        0     7221 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/README.md
+-rw-r--r--   0        0        0      269 2023-12-29 06:07:22.402888 asmrmanager-2.0.0/asmrmanager/__init__.py
+-rw-r--r--   0        0        0       46 2024-01-30 08:57:30.179230 asmrmanager-2.0.0/asmrmanager/__main__.py
+-rw-r--r--   0        0        0       21 2024-04-19 17:51:35.292944 asmrmanager-2.0.0/asmrmanager/_version.py
+-rw-r--r--   0        0        0    14684 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/asmrmanager/cli/core.py
+-rw-r--r--   0        0        0     5720 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/asmrmanager/cli/dl.py
+-rw-r--r--   0        0        0     6292 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/asmrmanager/cli/file.py
+-rw-r--r--   0        0        0      612 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/hold.py
+-rw-r--r--   0        0        0     2274 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/info.py
+-rw-r--r--   0        0        0     2060 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/main.py
+-rw-r--r--   0        0        0     2353 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/pl.py
+-rw-r--r--   0        0        0     1076 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/play.py
+-rw-r--r--   0        0        0     1599 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/query.py
+-rw-r--r--   0        0        0     1008 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/review.py
+-rw-r--r--   0        0        0     2140 2024-01-13 17:33:20.948158 asmrmanager-2.0.0/asmrmanager/cli/sql.py
+-rw-r--r--   0        0        0     1768 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/utils.py
+-rw-r--r--   0        0        0     1934 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/view.py
+-rw-r--r--   0        0        0      971 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/which.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/__init__.py
+-rw-r--r--   0        0        0      821 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/browse_params.py
+-rw-r--r--   0        0        0      527 2023-12-21 14:14:16.443072 asmrmanager-2.0.0/asmrmanager/common/download_params.py
+-rw-r--r--   0        0        0     1115 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/common/fileconverter.py
+-rw-r--r--   0        0        0      612 2024-04-09 08:45:58.879878 asmrmanager-2.0.0/asmrmanager/common/output.py
+-rw-r--r--   0        0        0      719 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/parse_filter.py
+-rw-r--r--   0        0        0     1768 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/common/rj_parse.py
+-rw-r--r--   0        0        0      913 2024-03-29 06:19:00.412674 asmrmanager-2.0.0/asmrmanager/common/select.py
+-rw-r--r--   0        0        0      894 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/common/types.py
+-rw-r--r--   0        0        0     1331 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/vtt2lrc.py
+-rw-r--r--   0        0        0     2637 2024-03-14 05:43:28.099361 asmrmanager-2.0.0/asmrmanager/config.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/database.py
+-rw-r--r--   0        0        0      343 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/engine.py
+-rw-r--r--   0        0        0     5793 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/manage.py
+-rw-r--r--   0        0        0      619 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/orm_type.py
+-rw-r--r--   0        0        0     1485 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/q_func.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/utils/__init__.py
+-rw-r--r--   0        0        0      480 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/utils/add2db.py
+-rw-r--r--   0        0        0     1290 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/utils/uuid_sqlite.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/filemanager/__init__.py
+-rw-r--r--   0        0        0      312 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/filemanager/appdirs_.py
+-rw-r--r--   0        0        0      108 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/filemanager/exceptions.py
+-rw-r--r--   0        0        0      477 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/file_zipper.py
+-rw-r--r--   0        0        0    12030 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/filemanager/manager.py
+-rw-r--r--   0        0        0     3194 2024-03-14 05:39:35.879370 asmrmanager-2.0.0/asmrmanager/filemanager/resources/config.example.toml
+-rw-r--r--   0        0        0       65 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/circle_name.sql
+-rw-r--r--   0        0        0      425 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/score.sql
+-rw-r--r--   0        0        0     1663 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/search.sql
+-rw-r--r--   0        0        0       92 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/tags.sql
+-rw-r--r--   0        0        0      602 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/test.sql
+-rw-r--r--   0        0        0       53 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/vas.sql
+-rw-r--r--   0        0        0     1579 2024-03-29 06:23:40.599330 asmrmanager-2.0.0/asmrmanager/filemanager/utils.py
+-rw-r--r--   0        0        0     1038 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/logger/__init__.py
+-rw-r--r--   0        0        0       68 2023-12-24 08:26:10.649470 asmrmanager-2.0.0/asmrmanager/lrcplayer/__init__.py
+-rw-r--r--   0        0        0     2318 2023-12-31 11:19:36.902077 asmrmanager-2.0.0/asmrmanager/lrcplayer/lrcparse.py
+-rw-r--r--   0        0        0      328 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/lrcplayer/main.css
+-rw-r--r--   0        0        0     5379 2024-04-08 06:16:03.019693 asmrmanager-2.0.0/asmrmanager/lrcplayer/main.py
+-rw-r--r--   0        0        0     3845 2024-04-05 09:59:01.476032 asmrmanager-2.0.0/asmrmanager/lrcplayer/player/base.py
+-rw-r--r--   0        0        0     4767 2024-04-08 06:16:03.006360 asmrmanager-2.0.0/asmrmanager/lrcplayer/player/mpdplayer.py
+-rw-r--r--   0        0        0     1777 2023-12-31 11:19:36.902077 asmrmanager-2.0.0/asmrmanager/lrcplayer/player/pygameplayer.py
+-rw-r--r--   0        0        0       75 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/spider/__init__.py
+-rw-r--r--   0        0        0     5368 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/spider/asmrapi.py
+-rw-r--r--   0        0        0    10001 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/spider/downloader.py
+-rw-r--r--   0        0        0     9594 2024-04-19 17:50:58.546279 asmrmanager-2.0.0/asmrmanager/spider/interface.py
+-rw-r--r--   0        0        0     1844 2024-04-19 17:50:58.546279 asmrmanager-2.0.0/asmrmanager/spider/playlist.py
+-rw-r--r--   0        0        0     4092 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/spider/utils/IDMHelper.py
+-rw-r--r--   0        0        0     1355 2024-03-30 06:44:45.769287 asmrmanager-2.0.0/asmrmanager/spider/utils/aria2_downloader.py
+-rw-r--r--   0        0        0     1554 2024-04-19 17:51:35.296278 asmrmanager-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8632 1970-01-01 00:00:00.000000 asmrmanager-2.0.0/PKG-INFO
```

### Comparing `asmrmanager-1.9.1/LICENSE` & `asmrmanager-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/README.md` & `asmrmanager-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 ### 播放
 
 非常简陋的终端播放界面，支持歌词显示，按照歌词信息快进，切换歌曲，支持以pygame(sdl)或mpd做为后端，可以预见的将来应该会完善一下(但感觉够用了应该不会再加啥功能了)。
 ![tui-screenshot](./assets/tui-screenshot.png)
 
 ## 使用方法
 
+**注意**：由于网站最近更新了针对BJ和VJ的支持，本项目进行了很大的重构，2.0.0 版本暂并不保证稳定运行，如果没有对BJ和VJ的需求，可以考虑继续使用1代的最后一个版本`pip install ASMRManager[依赖]==1.9.1`
+
 本工具支持 `python >= 3.10`, 安装方法如下：
 
 ```shell
 pip install ASMRManager[依赖]
 ```
 
 可选则的依赖项有 `idm`, `aria2`, `tui`，`pygame`,`mpd`, `all`，多个依赖使用逗号分隔，其中`all`为安装所有依赖。例如 `pip install ASMRManager[idm,tui]`
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/dl.py` & `asmrmanager-2.0.0/asmrmanager/cli/dl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,92 @@
-from typing import Iterable, Tuple
+from typing import List, Tuple
 
 import click
 
 from asmrmanager.cli.core import (
     browse_param_options,
     create_database,
     create_downloader_and_database,
     download_param_options,
     fm,
     interval_preprocess_cb,
     multi_rj_argument,
 )
 from asmrmanager.common.browse_params import BrowseParams
 from asmrmanager.common.download_params import DownloadParams
-from asmrmanager.common.rj_parse import RJID, id2rj
+from asmrmanager.common.rj_parse import SourceID, id2source_name
+from asmrmanager.common.types import LocalSourceID, RemoteSourceID
 from asmrmanager.logger import logger
 
 
 @click.group(help="download ASMR")
 def dl():
     pass
 
 
 @click.command()
-@multi_rj_argument
+@multi_rj_argument("remote")
 @download_param_options
-def get(rj_ids: Iterable[RJID], download_params: DownloadParams):
+def get(source_ids: List[RemoteSourceID], download_params: DownloadParams):
     """get ASMR by RJ ids"""
-    if not rj_ids:
-        logger.error("You must give at least one RJ id!")
+    if not source_ids:
+        logger.error("You must give at least one source id!")
         return
     spider, db = create_downloader_and_database(download_params)
-    spider.run(spider.get(rj_ids))
+    spider.run(spider.get(source_ids))
     db.commit()
 
 
 @click.command()
-@multi_rj_argument
-def update(rj_ids: Iterable[RJID]):
+@multi_rj_argument("remote")
+def update(source_ids: List[RemoteSourceID]):
     """update metadata, including recover file and description file"""
-    if not rj_ids:
-        logger.error("You must give at least one RJ id!")
+    if not source_ids:
+        logger.error("You must give at least one source id!")
         return
     spider, db = create_downloader_and_database(
         DownloadParams(False, False, False, True)
     )
-    spider.run(spider.update(rj_ids))
+    spider.run(spider.update(source_ids))
     db.commit()
 
 
 @click.command()
-@multi_rj_argument
-def check(rj_ids: Iterable[RJID]):
+@multi_rj_argument("local")
+def check(source_ids: List[LocalSourceID]):
     """check for existence of the file and its store field"""
     db = create_database()
     dl_queue = []
-    for rj_id in rj_ids:
-        rj = id2rj(rj_id)
+    for source_id in source_ids:
+        source_name = id2source_name(source_id)
 
-        asmr = db.check_exists(rj_id)
+        asmr = db.check_exists(source_id)
         if asmr is None:
             logger.warning(
-                f"Not found In Database: {rj}, please manually download it"
+                f"Not found In Database: {source_name}, please manually download it"
             )
             continue
 
-        src = fm.get_location(rj_id)
+        src = fm.get_location(source_id)
         if src is None:
-            logger.warning(f"Not found: {rj}, add to download")
-            dl_queue.append(rj)
+            logger.warning(f"Not found: {source_name}, add to download")
+            dl_queue.append(source_name)
             continue
 
         if src == "download" and asmr.stored:
-            logger.info(f"Already stored: {rj}, move to storage path")
-            fm.store(rj_id)
+            logger.info(f"Already stored: {source_name}, move to storage path")
+            fm.store(source_id)
             continue
 
         if src == "storage" and not asmr.stored:
-            logger.info(f"Already in storage: {rj}, update database")
+            logger.info(f"Already in storage: {source_name}, update database")
             asmr.stored = True
             continue
 
-        logger.info(f"No need to update {rj}")
+        logger.info(f"No need to update {source_name}")
     db.commit()
     print("Update succesfully.")
     if dl_queue:
         print("Please check the item to download and get theme manually:")
         print(" ".join(dl_queue))
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/file.py` & `asmrmanager-2.0.0/asmrmanager/cli/file.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,71 +6,72 @@
 
 from asmrmanager.cli.core import (
     create_database,
     fm,
     multi_rj_argument,
     rj_argument,
 )
-from asmrmanager.common.rj_parse import RJID
+from asmrmanager.common.rj_parse import SourceID
+from asmrmanager.common.types import LocalSourceID
 from asmrmanager.filemanager.exceptions import DstItemAlreadyExistsException
 from asmrmanager.logger import logger
 
 
 @click.group()
 def file():
     """file management"""
 
 
 @click.command("del")
-@rj_argument
-def del_(rj_id: RJID):
+@rj_argument("local")
+def del_(source_id: LocalSourceID):
     """not implemented"""
     raise NotImplementedError
     from asmrmanager.cli.core import create_fm
     from asmrmanager.filemanager.utils import folder_chooser_multiple
 
     fm = create_fm()
 
-    rj_path = fm.get_path(rj_id)
+    rj_path = fm.get_path(source_id)
 
     if rj_path is None:
-        logger.error(f"item {rj_id} does not exists")
+        logger.error(f"item {source_id} does not exists")
         return
 
     folders = folder_chooser_multiple(
         rj_path,
         lambda p: any(
             [i.suffix != ".info" for i in p.iterdir() if not i.is_dir()]
         ),
     )
 
     for folder in folders:
         pass
 
 
 @click.command()
-@rj_argument
+@rj_argument("local")
 @click.option(
     "--regex", "-r", type=str, default=".*", help="use regex to match"
 )
 @click.option(
     "--ignore-filter",
     "-i",
     "ignore_filter",
     is_flag=True,
     default=False,
     show_default=True,
     help="recover files that have been filtered out",
 )
-def recover(rj_id: RJID, regex: str, ignore_filter: bool):
+def recover(source_id: LocalSourceID, regex: str, ignore_filter: bool):
     """recover a file from recover file"""
 
     url2download: List[Tuple[str, Path]] = []
 
-    res = fm.load_recover(rj_id)
+    res = fm.load_recover(source_id)
     if res is None:
         return
     rj_path, recovers = res
 
     for recover in recovers:
         rel_path = recover["path"]
 
@@ -104,15 +105,15 @@
             downloader.downloader.process_download(url, path.parent, path.name)
         )
 
     downloader.run(*tasks)
 
 
 @click.command()
-@multi_rj_argument
+@multi_rj_argument("local")
 @click.option(
     "--replace/--no-replace",
     "-r/-nr",
     is_flag=True,
     default=True,
     show_default=True,
     help="replace the files if exists",
@@ -122,15 +123,15 @@
     "-a",
     "all_",
     is_flag=True,
     default=False,
     show_default=True,
     help="store all files",
 )
-def store(rj_ids: List[RJID], replace: bool, all_: bool):
+def store(source_ids: List[LocalSourceID], replace: bool, all_: bool):
     """
     store the downloaded files to the storage
     """
 
     db = create_database()
     try:
         if all_:
@@ -141,17 +142,17 @@
             )
             if res is None or res is False:
                 return
             fm.store_all(replace=replace)
             id_to_store = fm.list_("download")
 
         else:
-            for rj_id in rj_ids:
+            for rj_id in source_ids:
                 fm.store(rj_id, replace=replace)
-            id_to_store = rj_ids
+            id_to_store = source_ids
 
         for id_ in id_to_store:
             res = db.check_exists(id_)
             if not res:
                 logger.error(
                     "no such id: %s, which is an unexpected situation", id_
                 )
@@ -160,27 +161,31 @@
         db.commit()
         logger.info("succesfully stored all files")
     except DstItemAlreadyExistsException as e:
         logger.error("storing terminated for %s", e)
 
 
 @click.command()
-@rj_argument
-def diff(rj_id: RJID):
+@rj_argument("local")
+def diff(source_id: LocalSourceID):
     """
     Diff local files and the remote files,
     display files filtered, missing and added
     """
-    if res := fm.load_recover(rj_id):
-        rj_path, recovers = res
+    if res := fm.load_recover(source_id):
+        source_path, recovers = res
     else:
         return
 
     local_files = set(
-        [i.relative_to(rj_path) for i in rj_path.rglob("*") if not i.is_dir()]
+        [
+            i.relative_to(source_path)
+            for i in source_path.rglob("*")
+            if not i.is_dir()
+        ]
     )
     remote_files_should_down = set(
         [Path(i["path"]) for i in recovers if i["should_download"]]
     )
     remote_files_filterd = set(
         [Path(i["path"]) for i in recovers if not i["should_download"]]
     )
@@ -204,15 +209,15 @@
             color_map[file] = "dim"
         else:
             color_map[file] = "tree"
 
     from rich import print
     from rich.tree import Tree
 
-    tree = Tree(str(rj_path))
+    tree = Tree(str(source_path))
     p2tree = {Path("."): tree}
     for file in sorted(all_files, key=lambda x: x.parts):
         # if p2tree.get(file.parent) is None:
         #     p2tree[file.parent] = Tree(file.parent.name)
         # p2tree[file.parent].add(file.name, style=color_map[file])
         for path in reversed(file.parents):  # from . → ./a → ./a/b
             if p2tree.get(path) is None:
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/hold.py` & `asmrmanager-2.0.0/asmrmanager/cli/hold.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import click
 
 from asmrmanager.cli.core import rj_argument
+from asmrmanager.common.types import LocalSourceID
 from asmrmanager.logger import logger
 
 
 @click.command()
-@rj_argument
+@rj_argument("local")
 @click.option("-c", "--comment", type=str, default=None, show_default=True)
-def hold(rj_id: int, comment: str | None = None):
+def hold(source_id: LocalSourceID, comment: str | None = None):
     """set the ASMR.hold to true, and add a comment for the reason"""
-    logger.info(f"run command hold with rj_id={rj_id} comment={comment}")
+    logger.info(f"run command hold with rj_id={source_id} comment={comment}")
 
     from asmrmanager.cli.core import create_database
 
     db = create_database()
-    db.hold_item(rj_id, comment)
+    db.hold_item(source_id, comment)
     db.commit()
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/info.py` & `asmrmanager-2.0.0/asmrmanager/cli/info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import click
 
 from asmrmanager.cli.core import (
+    convert2remote_id,
     create_database,
     create_downloader_and_database,
     rj_argument,
 )
-from asmrmanager.common.rj_parse import RJID
+from asmrmanager.common.rj_parse import SourceID
+from asmrmanager.common.types import LocalSourceID, RemoteSourceID
 from asmrmanager.database.orm_type import ASMRInstance
 from asmrmanager.logger import logger
 
 
 def print_asmr_info(asmr: ASMRInstance):
     from rich.console import Console
     from rich.markdown import Markdown
@@ -33,43 +35,59 @@
 - review count: {count}
 - held: {held}
 - stored: {stored}
 
 {comment}
     """
     res: dict = asmr.__dict__.copy()
+    # logger.debug(res)
     tags = "\n".join([f"  - {t}" for t in asmr.tags])
     cvs = "\n".join([f"  - {c}" for c in asmr.vas])
+    if res.get("tags"):
+        del res["tags"]
     s = template.format(tags=tags, cvs=cvs, **res)
     console = Console()
     console.print(Markdown(s))
 
 
-def info_from_web(rj_id: int):
+def info_from_web(source_id: RemoteSourceID):
     downloader, db = create_downloader_and_database()
-    (rj_info,) = downloader.run(downloader.downloader.get_voice_info(rj_id))
+    (rj_info,) = downloader.run(
+        downloader.downloader.get_voice_info(source_id)
+    )
+    # logger.debug(rj_info)
 
     res = db.parse_info(rj_info)
+    res.star = 0
+    res.count = 0
+    res.held = False
+    res.stored = False
+    res.comment = ""
     print_asmr_info(res)
 
 
 @click.command()
 @click.option(
     "--rand",
     "-r",
     is_flag=True,
     default=False,
     show_default=True,
     help="get a random info in the database",
 )
-@rj_argument
-def info(rj_id: RJID, rand: bool):
+@rj_argument("local")
+def info(source_id: LocalSourceID, rand: bool):
     """show info of the ASMR by id"""
     db = create_database()
 
-    v_info = db.func.get_info(rj_id, rand=rand)
+    v_info = db.func.get_info(source_id, rand=rand)
     if v_info is None:
-        logger.info(f"RJ{rj_id} not exists, try getting from web")
-        info_from_web(rj_id)
+        logger.info(f"{source_id} not exists, try getting from web")
+        remote_source_id = convert2remote_id(source_id)
+        if remote_source_id is None:
+            logger.error(f"cannot convert {source_id} to remote id")
+            return
+        # logger.debug(f"converted {source_id} to {remote_source_id}")
+        info_from_web(remote_source_id)
         return
 
     print_asmr_info(v_info)
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/main.py` & `asmrmanager-2.0.0/asmrmanager/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from asmrmanager.cli.hold import hold
 from asmrmanager.cli.info import info
 from asmrmanager.cli.pl import pl
 from asmrmanager.cli.play import play
 from asmrmanager.cli.query import query
 from asmrmanager.cli.review import review
 from asmrmanager.cli.sql import sql
+from asmrmanager.cli.utils import utils
 from asmrmanager.cli.view import view
 from asmrmanager.cli.which import which
 from asmrmanager.logger import logger
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 sys.stdout.reconfigure(encoding="utf-8")  # type: ignore
 sys.stderr.reconfigure(encoding="utf-8")  # type: ignore
@@ -61,10 +62,11 @@
 main.add_command(sql)
 main.add_command(view)
 main.add_command(hold)
 main.add_command(query)
 main.add_command(which)
 main.add_command(file)
 main.add_command(pl)
+main.add_command(utils)
 
 if __name__ == "__main__":
     main()
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/pl.py` & `asmrmanager-2.0.0/asmrmanager/cli/pl.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 from asmrmanager.cli.core import (
     create_playlist,
     fm,
     multi_rj_argument,
     pl_preprocess_cb,
 )
-from asmrmanager.common.rj_parse import RJID
-from asmrmanager.common.types import PlayListItem
+from asmrmanager.common.types import PlayListItem, RemoteSourceID
 
 
 class PLID(click.ParamType):
     name = "pl_id"
 
     def shell_complete(
         self, ctx: "click.Context", param: "click.Parameter", incomplete: str
@@ -59,19 +58,19 @@
     """list all playlists"""
     pl = create_playlist()
     pl.run(pl.list(num, raw))
 
 
 @click.command()
 @click.argument("pl_id", type=PLID(), callback=pl_preprocess_cb)
-@multi_rj_argument
-def add(rj_ids: List[RJID], pl_id: uuid.UUID):
+@multi_rj_argument("remote")
+def add(source_ids: List[RemoteSourceID], pl_id: uuid.UUID):
     """add a playlist"""
     pl = create_playlist()
-    pl.run(pl.add(rj_ids, pl_id))
+    pl.run(pl.add(source_ids, pl_id))
 
 
 @click.command("rm")
 @click.argument("pl_ids", type=PLID(), nargs=-1, callback=pl_preprocess_cb)
 def remove(pl_ids: List[uuid.UUID]):
     """remove a playlist"""
     pl = create_playlist()
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/query.py` & `asmrmanager-2.0.0/asmrmanager/cli/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             ASMR.circle_name.contains(keyword)
             | ASMR.title.contains(keyword)
             | Tag.name.contains(keyword)
         )
         .group_by(ASMR.id)
     )
 
-    assert limit > 0
+    assert limit >= 0
     if limit == 0:
         res = res_query.all()
     else:
         res = res_query.limit(limit).all()
 
     titles = [
         "id",
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/review.py` & `asmrmanager-2.0.0/asmrmanager/cli/review.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import click
 
 from asmrmanager.cli.core import rj_argument
-from asmrmanager.common.rj_parse import RJID
+from asmrmanager.common.rj_parse import SourceID
+from asmrmanager.common.types import LocalSourceID
 from asmrmanager.logger import logger
 
 
 @click.command()
-@rj_argument
+@rj_argument("local")
 @click.option("-s", "--star", type=int, help="must be integer in [1, 5]")
 @click.option("-c", "--comment", type=str)
-def review(rj_id: RJID, star: int, comment: str):
+def review(source_id: LocalSourceID, star: int, comment: str):
     """review an ASMR with star(1-5) and comment and add it to storage path"""
     logger.info(
-        f"run command review with rj_id={rj_id}, star={star} comment={comment}"
+        f"run command review with rj_id={source_id}, star={star} comment={comment}"
     )
 
     from asmrmanager.cli.core import create_database, fm
 
     db = create_database()
 
     update_stored = False
     if not fm.could_store():
         logger.warning(
             "storage/download path not found skip storing operation"
         )
     else:
-        fm.store(rj_id)
+        fm.store(source_id)
         update_stored = True
-    db.update_review(rj_id, star, comment, update_stored=update_stored)
+    db.update_review(source_id, star, comment, update_stored=update_stored)
     db.commit()
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/sql.py` & `asmrmanager-2.0.0/asmrmanager/cli/sql.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/view.py` & `asmrmanager-2.0.0/asmrmanager/cli/view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from typing import Literal
 
 import click
 
-from asmrmanager.cli.core import fm, id2rj, rj_argument
-from asmrmanager.common.rj_parse import RJID
+from asmrmanager.cli.core import fm, id2source_name, rj_argument
+from asmrmanager.common.rj_parse import SourceID
+from asmrmanager.common.types import LocalSourceID
 from asmrmanager.filemanager.exceptions import (
     DstItemAlreadyExistsException,
     SrcNotExistsException,
 )
 from asmrmanager.logger import logger
 
 
 @click.group(help="some operation about view_path")
 def view():
     pass
 
 
 @click.command()
-@rj_argument
+@rj_argument("local")
 @click.option(
     "--mode",
     "-m",
     type=click.Choice(["link", "zip", "adb", "copy"]),
     default="zip",
     show_default=True,
 )
-def add(rj_id: RJID, mode: Literal["link", "zip", "adb", "copy"]):
+def add(source_id: LocalSourceID, mode: Literal["link", "zip", "adb", "copy"]):
     """add an ASMR to view path (use zip by default)"""
     from asmrmanager.cli.core import fm
     from asmrmanager.filemanager.utils import folder_chooser
 
-    src = fm.get_path(rj_id)
+    src = fm.get_path(source_id)
     if src is None:
         raise SrcNotExistsException
 
-    rj_name = id2rj(rj_id)
+    rj_name = id2source_name(source_id)
     dst = fm.view_path / rj_name
     if dst.exists():
         i = 1
         while True:
             dst = fm.view_path / f"{rj_name}.{i}"
             if not dst.exists():
                 break
@@ -63,16 +64,16 @@
 def list_():
     """list all files in view path"""
     rjs = fm.list_("view")
     print(*rjs, sep="\n")
 
 
 @click.command()
-@rj_argument
-def remove(rj_id: RJID):
+@rj_argument("local")
+def remove(source_id: LocalSourceID):
     """remove a file link in view path"""
-    fm.remove_view(rj_id)
+    fm.remove_view(source_id)
 
 
 view.add_command(add)
 view.add_command(list_)
 view.add_command(remove)
```

### Comparing `asmrmanager-1.9.1/asmrmanager/cli/which.py` & `asmrmanager-2.0.0/asmrmanager/cli/which.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 
 import click
 
 from asmrmanager.cli.core import rj_argument
-from asmrmanager.common.rj_parse import RJID
+from asmrmanager.common.rj_parse import SourceID
+from asmrmanager.common.types import LocalSourceID
 from asmrmanager.logger import logger
 
 
 @click.command()
-@rj_argument
+@rj_argument("local")
 @click.option("--show", is_flag=True, default=False, show_default=True)
-def which(rj_id: RJID, show: bool):
+def which(source_id: LocalSourceID, show: bool):
     """Get the path from the given rj_id"""
     from asmrmanager.cli.core import fm
 
-    path = str(fm.get_path(rj_id))
+    path = str(fm.get_path(source_id))
 
     if not show:
         click.echo(path)
     else:
         import sys
 
         if sys.platform == "win32":
```

### Comparing `asmrmanager-1.9.1/asmrmanager/common/browse_params.py` & `asmrmanager-2.0.0/asmrmanager/common/browse_params.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/common/download_params.py` & `asmrmanager-2.0.0/asmrmanager/common/download_params.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/common/output.py` & `asmrmanager-2.0.0/asmrmanager/common/output.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/common/parse_filter.py` & `asmrmanager-2.0.0/asmrmanager/common/parse_filter.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/common/select.py` & `asmrmanager-2.0.0/asmrmanager/common/select.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/common/vtt2lrc.py` & `asmrmanager-2.0.0/asmrmanager/common/vtt2lrc.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/config.py` & `asmrmanager-2.0.0/asmrmanager/config.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/database/database.py` & `asmrmanager-2.0.0/asmrmanager/database/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 
 Base = declarative_base()
 
 
 class ASMR(Base):
     __tablename__ = "asmr"
     id = Column(Integer, primary_key=True)
-    title = Column(Text)
+    remote_id = Column(Integer, unique=True)
 
+    title = Column(Text)
     circle_name = Column(Text)  # 对应name字段
     tags = relationship("Tag", secondary="asmrs2tags", backref="asmrs")
     vas = relationship("VoiceActor", secondary="asmrs2vas", backref="asmrs")
     nsfw = Column(Boolean)
     release_date = Column(Date)  # 对应release字段
     price = Column(Integer)
     dl_count = Column(Integer)
```

### Comparing `asmrmanager-1.9.1/asmrmanager/database/orm_type.py` & `asmrmanager-2.0.0/asmrmanager/database/orm_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from datetime import date
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from asmrmanager.common.rj_parse import RJID
+    from asmrmanager.common.rj_parse import SourceID
 
 
 class ASMRInstance:
-    id: "RJID"
+    id: "SourceID"
+    remote_id: int
     title: str
     circle_name: str
     tags: list["TagInstance"]
     vas: list["VoiceActorInstance"]
     nsfw: bool
     release_date: date
     price: int
```

### Comparing `asmrmanager-1.9.1/asmrmanager/database/q_func.py` & `asmrmanager-2.0.0/asmrmanager/database/q_func.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,49 @@
-from typing import Optional
+import typing
 
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 
+from asmrmanager.common.types import LocalSourceID
 from asmrmanager.database.orm_type import ASMRInstance
+from asmrmanager.logger import logger
 
 from .database import ASMR, Tag
 
 
 class QFunc:
     def __init__(self, ss: Session):
         self.ss = ss
 
-    def get_info(self, rj_id: int, rand: bool) -> ASMRInstance | None:
+    def get_info(
+        self, local_source_id: LocalSourceID, rand: bool
+    ) -> ASMRInstance | None:
+        logger.debug(local_source_id)
         if rand:
             return self.ss.query(ASMR).order_by(func.random()).first()
-        return self.ss.query(ASMR).get(rj_id)
+        return self.ss.query(ASMR).get(local_source_id)
 
-    def get_tag_id(self, name: str) -> Optional[int]:
+    def get_tag_id(self, name: str) -> int | None:
         res = self.ss.query(Tag).filter(Tag.name == name).one_or_none()
         if res:
             return getattr(res, "id")
         return None
 
     def get_tag_name(self, tid: int):
         res = self.ss.query(Tag).filter(Tag.id == tid).one_or_none()
         if res:
             return res.name
         return None
 
     def get_stored(self, rj_id: int):
         res = self.ss.query(ASMR).get(rj_id)
         return res.stored if res is not None else None
+
+    def get_local_id(self, remote_id: int) -> int | None:
+        res = self.ss.query(ASMR).filter_by(remote_id=remote_id).one_or_none()
+        if res:
+            return typing.cast(int, res.id)
+
+    def get_remote_id(self, local_id: int) -> int | None:
+        res = self.ss.query(ASMR).get(local_id)
+        if res:
+            return int(res.remote_id)
```

### Comparing `asmrmanager-1.9.1/asmrmanager/database/utils/uuid_sqlite.py` & `asmrmanager-2.0.0/asmrmanager/database/utils/uuid_sqlite.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/filemanager/manager.py` & `asmrmanager-2.0.0/asmrmanager/filemanager/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Iterable, List, Literal, NamedTuple, Tuple
 
 import toml
 
-from asmrmanager.common.rj_parse import RJID, id2rj, rj2id
-from asmrmanager.common.types import PlayListItem, RecoverRecord
+from asmrmanager.common.rj_parse import (
+    SourceID,
+    id2source_name,
+    source2id,
+    source_name2id,
+)
+from asmrmanager.common.types import (
+    LocalSourceID,
+    PlayListItem,
+    RecoverRecord,
+    SourceName,
+)
 from asmrmanager.config import config
 from asmrmanager.filemanager.appdirs_ import (
     CACHE_PATH,
     CONFIG_PATH,
     DATA_PATH,
     LOG_PATH,
 )
@@ -115,19 +125,19 @@
         self.view_path_exists = (
             True if os.path.exists(self.view_path) else False
         )
 
     def could_store(self):
         return self.storage_path_exists and self.download_path_exists
 
-    def store(self, rj_id: RJID, replace=True):
+    def store(self, source_id: LocalSourceID, replace=True):
         """sync download path and storage path"""
         # TODO 换用fcp实现？
         assert self.could_store()
-        rj_name = id2rj(rj_id)
+        rj_name = id2source_name(source_id)
         if not os.path.exists(self.download_path / rj_name):
             logger.warning(f"item {rj_name} does not exists, skip it")
             return
 
         # if os.path.exists(self.storage_path / rj_name):
         #     if not exists_ok:
         #         logger.error(f"the item {rj_name} to store already exists!")
@@ -182,19 +192,19 @@
         #         f"deleting original files error: {e}, terminated, please"
         #         f" munually clean the files at {self.download_path / rj_name}"
         #     )
         #     exit(-1)
 
     def store_all(self, replace=True):
         for file in os.listdir(self.download_path):
-            rj_id = rj2id(file)
-            if rj_id is None:
+            source_id = source_name2id(SourceName(file))
+            if source_id is None:
                 logger.warning(f"Ignore invalid file {file} in download path")
                 continue
-            self.store(rj_id, replace=replace)
+            self.store(source_id, replace=replace)
 
     def could_view(self):
         """
         either storage_path or download_path exists ok,
         view path must exists
         """
         return self.view_path_exists and (
@@ -218,17 +228,17 @@
             return
 
         dst.mkdir(parents=True, exist_ok=True)
 
         for subfile in src.iterdir():
             FileManager._copy(subfile, dst / subfile.name, depth - 1)
 
-    def remove_view(self, rj_id: RJID):
+    def remove_view(self, source_id: LocalSourceID):
         assert self.could_view()
-        rj_name = id2rj(rj_id)
+        rj_name = id2source_name(source_id)
 
         for path in self.view_path.iterdir():
             if path.stem != rj_name:
                 continue
             if path.is_dir() and path.is_symlink():
                 os.remove(path)
                 return
@@ -240,55 +250,55 @@
             return
         # path = self.view_path / rj_name
         # assert path.is_dir() and path.is_symlink()
         # os.remove(path)
 
     def list_(
         self, path: Literal["download", "view", "storage"]
-    ) -> Iterable[RJID]:
+    ) -> Iterable[LocalSourceID]:
         if path == "download":
             p = self.download_path
         elif path == "view":
             p = self.view_path
         elif path == "storage":
             p = self.storage_path
         else:
             logger.error("Invalid path")
             return []
 
         for name in p.iterdir():
-            rj_id = rj2id(name.name)
+            rj_id = source_name2id(SourceName(name.name))
             if rj_id is None:
                 continue
             yield rj_id
 
     def zip_file(self, src: Path, dst: Path):
         from asmrmanager.filemanager.file_zipper import zip_chosen_folder
 
         zip_chosen_folder(src, dst)
 
     def get_location(
-        self, rj_id: RJID
+        self, source_id: LocalSourceID
     ) -> Literal["download", "storage", None]:
-        rj_name = id2rj(rj_id)
-        if (self.storage_path / rj_name).exists():
+        source_name = id2source_name(source_id)
+        if (self.storage_path / source_name).exists():
             return "storage"
-        if (self.download_path / rj_name).exists():
+        if (self.download_path / source_name).exists():
             return "download"
         return None
 
-    def get_path(self, rj_id: RJID) -> Path | None:
+    def get_path(self, source_id: LocalSourceID) -> Path | None:
         """get rj file path"""
-        res = self.get_location(rj_id)
+        res = self.get_location(source_id)
 
         match res:
             case "download":
-                return self.download_path / id2rj(rj_id)
+                return self.download_path / id2source_name(source_id)
             case "storage":
-                return self.storage_path / id2rj(rj_id)
+                return self.storage_path / id2source_name(source_id)
             case _:
                 return None
 
     def check_exists(self, rel_path: str):
         download, storage = False, False
         download_file_path = self.download_path / rel_path
         storage_file_path = self.storage_path / rel_path
@@ -329,26 +339,26 @@
                     return True
             case _:
                 pass
 
         return False
 
     def load_recover(
-        self, rj_id: RJID
+        self, source_id: LocalSourceID
     ) -> Tuple[Path, List[RecoverRecord]] | None:
 
-        rj_path = self.get_path(rj_id)
+        rj_path = self.get_path(source_id)
         if rj_path is None:
-            logger.error(f"item {rj_id} does not exist")
+            logger.error(f"item {source_id} does not exist")
             return
 
         recover_path = rj_path / ".recover"
         if not recover_path.exists():
             logger.error(
-                f"item {rj_id} does not have recover file, please update this"
+                f"item {source_id} does not have recover file, please update this"
                 " rj id first"
             )
             return
 
         import json
 
         recovers: List[RecoverRecord] = json.loads(
```

### Comparing `asmrmanager-1.9.1/asmrmanager/filemanager/resources/config.example.toml` & `asmrmanager-2.0.0/asmrmanager/filemanager/resources/config.example.toml`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/search.sql` & `asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/search.sql`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/filemanager/resources/sqls.example/test.sql` & `asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/test.sql`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/filemanager/utils.py` & `asmrmanager-2.0.0/asmrmanager/filemanager/utils.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/logger/__init__.py` & `asmrmanager-2.0.0/asmrmanager/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/lrcplayer/lrcparse.py` & `asmrmanager-2.0.0/asmrmanager/lrcplayer/lrcparse.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/lrcplayer/main.py` & `asmrmanager-2.0.0/asmrmanager/lrcplayer/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import time
 from pathlib import Path
+from time import monotonic
 from typing import List
 
 import click
 from textual.app import App, ComposeResult
 from textual.containers import Center
 from textual.widgets import Footer, Label, ProgressBar
 
@@ -25,14 +27,15 @@
         ("j", "forward", "快进"),
         ("k", "backward", "快退"),
         ("l", "next_voice", "下一首"),
         ("h", "prev_voice", "上一首"),
     ]
     LRC_PREV = 1
     LRC_NEXT = 1
+    OPERATION_FREQ = 0.05
 
     def __init__(self, episodes: List[Music], *args, **kwargs):
         self.episodes = episodes
         match config.player:
             case "pygame":
                 from .player.pygameplayer import PyGamePlayer
 
@@ -42,14 +45,21 @@
 
                 self.player = MPDPlayer(episodes)
             case _:
                 logger.error(f"player {config.player} not supported")
                 assert False
 
         super().__init__(*args, **kwargs)
+        self.last_operation_time = monotonic()
+
+    def check_freq(self):
+        if (
+            delta := monotonic() - self.last_operation_time
+        ) < self.OPERATION_FREQ:
+            time.sleep(delta)
 
     def on_mount(self):
         self.player.play()
         self.progress_timer = self.set_interval(0.05, self.progress)
 
     def progress(self):
         if not self.player.is_playing:
@@ -105,17 +115,19 @@
             self.player.pause()
             self.progress_timer.pause()
         else:
             self.player.unpause()
             self.progress_timer.resume()
 
     def action_forward(self):
+        self.check_freq()
         self.player.forward()
 
     def action_backward(self):
+        self.check_freq()
         self.player.backward()
 
     def switch_voice(self, idx: int):
         self.player.switch_music(idx)
         self.query_one("#title", expect_type=Label).update(self.player.title)
 
     def action_next_voice(self):
```

### Comparing `asmrmanager-1.9.1/asmrmanager/lrcplayer/player/base.py` & `asmrmanager-2.0.0/asmrmanager/lrcplayer/player/base.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/lrcplayer/player/mpdplayer.py` & `asmrmanager-2.0.0/asmrmanager/lrcplayer/player/mpdplayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,27 @@
         ("state", Literal["play", "pause", "stop"]),
         ("song", int),
         ("total_time", int),
         ("pos", int),
     ],
 )
 
+import threading
+
+
+def do_every(interval, worker_func, iterations=0):
+    if iterations != 1:
+        threading.Timer(
+            interval,
+            do_every,
+            [interval, worker_func, 0 if iterations == 0 else iterations - 1],
+        ).start()
+
+    worker_func()
+
 
 class MPDPlayer(BasePlayer):
     bin = os.path.expanduser(config.mpd_config.bin)
     music_directory: Path = (
         Path(config.mpd_config.music_directory)
         if config.mpd_config.music_directory
         else FileManager.DATA_PATH / "mpd" / "music"
@@ -45,26 +58,25 @@
             f"{cls.bin} {FileManager.CONFIG_PATH / 'mpd.conf'} {cmd}",
             shell=True,
             capture_output=True,
             text=True,
             check=check,
         ).stdout
 
-    @property
-    def _status(self):
-        status = self.client.status()
-        if status.get("song"):
-            self._index = int(status["song"])
-
-        return MPDStatus(
-            playlistlength=int(status["playlistlength"]),
-            state=status["state"],
-            song=int(status.get("song", 0)),
-            pos=int(float(status.get("elapsed", 0)) * 1000),
-            total_time=int(float(status.get("duration", 0)) * 1000),
+    def __update_status(self):
+        self.__status = self.client.status()
+        if self.__status.get("song"):
+            self._index = int(self.__status["song"])
+
+        self._status = MPDStatus(
+            playlistlength=int(self.__status["playlistlength"]),
+            state=self.__status["state"],
+            song=int(self.__status.get("song", 0)),
+            pos=int(float(self.__status.get("elapsed", 0)) * 1000),
+            total_time=int(float(self.__status.get("duration", 0)) * 1000),
         )
 
     def __init__(self, music_list: List[Music]) -> None:
         super().__init__(music_list)
 
         # d = uuid.uuid1()
 
@@ -103,14 +115,16 @@
         self.client.add("default")
         while len(self.client.playlist()) != len(music_list):
             time.sleep(0.01)
         logger.info(f"mpd add finished {self.client.playlist()}")
         self.client.play()
         self.client.single(0)
 
+        do_every(0.1, self.__update_status)
+
     def switch_music(self, index: int) -> None:
         # self.client.stop()
         self.client.play(index)
 
     @property
     def is_playing(self) -> bool:
         return self._status.state == "play"
@@ -119,29 +133,32 @@
     def pos(self) -> int:
         return self._status.pos
 
     @pos.setter
     def pos(self, pos: int) -> None:
         if self._status.state == "stop":
             return
-        self.client.seekcur(int(pos / 1000))
+        self.client.seekcur((pos / 1000))
+        # self.__update_status()
         # self.client.pause()
         # self.client.pause()
 
     @property
     def is_paused(self) -> bool:
         return self._status.state == "pause"
 
     def pause(self) -> None:
         if not self.is_paused:
             self.client.pause()
+        self.__update_status()
 
     def unpause(self) -> None:
         if self.is_paused:
             self.client.pause()
+        self.__update_status()
 
     def play(self) -> None:
         self.client.stop()
         self.client.play()
 
     @property
     def total_time(self) -> int:
```

### Comparing `asmrmanager-1.9.1/asmrmanager/lrcplayer/player/pygameplayer.py` & `asmrmanager-2.0.0/asmrmanager/lrcplayer/player/pygameplayer.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/spider/asmrapi.py` & `asmrmanager-2.0.0/asmrmanager/spider/asmrapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 from typing import Any, Dict, List, TypeVar
 
 from aiohttp import ClientConnectorError, ClientSession
 from aiohttp.connector import TCPConnector
 
-from asmrmanager.common.rj_parse import RJID, id2rj
+from asmrmanager.common.rj_parse import SourceID, id2source_name
+from asmrmanager.common.types import RemoteSourceID
 from asmrmanager.logger import logger
 
 T = TypeVar("T", bound="ASMRAPI")
 
 
 class ASMRAPI:
     base_api_url = "https://api.asmr-200.com/api/"
@@ -51,17 +52,19 @@
             async with self._session.post(
                 self.base_api_url + "auth/me",
                 json={"name": self.name, "password": self.password},
                 headers=self.headers,
                 proxy=self.proxy,
             ) as resp:
                 token = (await resp.json())["token"]
-                self.headers.update({
-                    "Authorization": f"Bearer {token}",
-                })
+                self.headers.update(
+                    {
+                        "Authorization": f"Bearer {token}",
+                    }
+                )
         except ClientConnectorError as err:
             logger.error(f"Login failed, {err}")
 
     async def get(self, route: str, params: dict | None = None) -> Any:
         resp_json = None
         while not resp_json:
             try:
@@ -118,18 +121,20 @@
                 "description": desc or "",
                 "privacy": privacy,
                 "locale": "zh-CN",
                 "works": [],
             },
         )
 
-    async def _add_works_to_playlist(self, rj_ids: List[RJID], pl_id: str):
+    async def _add_works_to_playlist(
+        self, source_ids: List[RemoteSourceID], pl_id: str
+    ):
         return await self.post(
             "playlist/add-works-to-playlist",
-            data={"id": pl_id, "works": rj_ids},
+            data={"id": pl_id, "works": source_ids},
         )
 
     async def _delete_playlist(self, pl_id: str):
         return await self.post("playlist/delete-playlist", data={"id": pl_id})
 
     async def get_search_result(
         self, content: str, params: dict
```

### Comparing `asmrmanager-1.9.1/asmrmanager/spider/downloader.py` & `asmrmanager-2.0.0/asmrmanager/spider/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import json
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Literal, TypeVar
 
+import asyncstdlib
+
+from asmrmanager.common.types import RemoteSourceID
+
 T = TypeVar("T", bound="ASMRDownloadAPI")
 
 
-from asmrmanager.common.rj_parse import RJID, id2rj
+from asmrmanager.common.rj_parse import (
+    SourceID,
+    id2source_name,
+    source_name2id,
+)
 from asmrmanager.config import Aria2Config
 from asmrmanager.logger import logger
 from asmrmanager.spider.asmrapi import ASMRAPI
 
 try:
     IDMHELPER_EXIST = True
     from .utils.IDMHelper import IDMHelper
@@ -47,24 +55,14 @@
         limit: int = 3,
         download_method: Literal["aria2", "idm"] = "idm",
         aria2_config: Aria2Config | None = None,
     ):
         # self._session: Optional[ClientSession] = None  # for __aenter__
         super().__init__(name, password, proxy, limit)
         self.save_path = fm.download_path
-        # self.pop_keys = (
-        #             "create_date",
-        #             "userRating",
-        #             "review_text",
-        #             "progress",
-        #             "updated_at",
-        #             "user_name",
-        #             "rate_count_detail",
-        #             "rank"
-        #     )
         self.json_should_download = json_should_download
         self.name_should_download = name_should_download
         self.replace = replace
         self.download_file = (
             self.download_by_idm
             if download_method == "idm"
             else self.download_by_aria2
@@ -74,27 +72,31 @@
             assert Aria2Downloader
             self.aria2_downloader = Aria2Downloader(proxy)
         self.aria2_config = aria2_config
         self.download_method = download_method
 
     async def download(
         self,
-        voice_id: int,
+        voice_id: RemoteSourceID,
         save_path: Path | None = None,
     ) -> None:
         voice_info = await self.get_voice_info(voice_id)
 
         should_down = self.json_should_download(voice_info)
         if not should_down:
             logger.info(f"stop download {voice_id}")
             return
         if save_path is None:
             save_path = self.save_path
 
-        voice_path = save_path / id2rj(RJID(voice_id))
+        assert (
+            id2source_name(source_name2id(voice_info["source_id"]))
+            == voice_info["source_id"]
+        )
+        voice_path = save_path / voice_info["source_id"]
         if voice_path.exists():
             logger.warning(f"path {voice_path} already exists.")
 
         voice_path.mkdir(parents=True, exist_ok=True)
         self.create_info_file(voice_info, voice_path=voice_path)
 
         tracks = await self.get_voice_tracks(voice_id)
@@ -120,20 +122,21 @@
                 "should_download": file.should_download,
             }
             for file in file_list
         ]
         with open(voice_path / ".recover", "w", encoding="utf-8") as f:
             json.dump(recover, f, ensure_ascii=False, indent=4)
 
-    async def get_voice_info(self, voice_id: int) -> Dict[str, Any]:
+    @asyncstdlib.lru_cache(None)
+    async def get_voice_info(self, voice_id: RemoteSourceID) -> Dict[str, Any]:
         voice_info = await self.get(f"work/{voice_id}")
         assert isinstance(voice_info, dict)
         return voice_info
 
-    async def get_voice_tracks(self, voice_id: int):
+    async def get_voice_tracks(self, voice_id: RemoteSourceID):
         return await self.get(f"tracks/{voice_id}")
 
     @staticmethod
     async def download_by_idm(
         url: str, save_path: Path, file_name: str
     ) -> bool:
         """the save path + file should not exist,
@@ -192,18 +195,18 @@
 
         logger.info(f"Downloading {file_path}")
         if not await self.download_file(url, save_path, file_name):
             logger.error(f"Download {file_path} failed")
             return
 
     def create_info_file(self, voice_info: Dict[str, Any], voice_path: Path):
-        rj_name = id2rj(voice_info["id"])
+        source_name = voice_info["source_id"]
         # info中有名字信息，理论上应该是一样的，但有可能为空，所以不考虑使用
         # recv_rj_name = voice_info['original_workno']
-        json_path = voice_path / f"{rj_name}.json"
+        json_path = voice_path / f"{source_name}.json"
         if json_path.exists():
             logger.info(f"Path {json_path} already exists, update it...")
         with open(json_path, "w", encoding="utf-8") as f:
             json.dump(voice_info, f, ensure_ascii=False, indent=4)
 
     async def create_dir_and_download(self, file_list: List[FileInfo]) -> None:
         for file_info in file_list:
```

### Comparing `asmrmanager-1.9.1/asmrmanager/spider/interface.py` & `asmrmanager-2.0.0/asmrmanager/spider/interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import asyncio
 import uuid
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
-    Iterable,
     List,
     Literal,
     Tuple,
     TypeVar,
 )
 
-from asmrmanager.cli.core import fm
 from asmrmanager.common.browse_params import BrowseParams
-from asmrmanager.common.rj_parse import RJID, id2rj
+from asmrmanager.common.rj_parse import (
+    SourceID,
+    id2source_name,
+    source_name2id,
+)
 from asmrmanager.common.select import select, select_multiple
+from asmrmanager.common.types import LocalSourceID, RemoteSourceID
 from asmrmanager.config import Aria2Config
+from asmrmanager.filemanager.manager import fm
 from asmrmanager.logger import logger
 from asmrmanager.spider.asmrapi import ASMRAPI
 from asmrmanager.spider.playlist import ASMRPlayListAPI
 
 from .downloader import ASMRDownloadAPI
 
 T = TypeVar("T", bound=Any)
@@ -41,15 +45,15 @@
 
 class ASMRDownloadManager(AsyncManager):
     def __init__(
         self,
         name: str,
         password: str,
         proxy: str | None,
-        id_should_download: Callable[[RJID], bool] | None = None,
+        id_should_download: Callable[[RemoteSourceID], bool] | None = None,
         json_should_download: Callable[[Dict[str, Any]], bool] | None = None,
         name_should_download: (
             Callable[[str, Literal["directory", "file"]], bool] | None
         ) = None,
         replace=False,
         download_method: Literal["aria2", "idm"] = "idm",
         aria2_config: Aria2Config | None = None,
@@ -63,21 +67,21 @@
             replace=replace,
             download_method=download_method,
             aria2_config=aria2_config,
         )
         super().__init__(self.downloader)
         self.id_should_download = id_should_download or (lambda _: True)
 
-    async def get(self, ids: Iterable[RJID]):
+    async def get(self, ids: List[RemoteSourceID]):
         tasks = []
-        for arg in ids:
-            if not self.id_should_download(arg):
-                logger.info(f"RJ{arg} already exists.")
+        for id_ in ids:
+            if not self.id_should_download(id_):
+                logger.info(f"RJ{id_} already exists.")
                 continue
-            tasks.append(self.downloader.download(arg))
+            tasks.append(self.downloader.download(id_))
         await asyncio.gather(*tasks)
 
     async def search(
         self,
         text: str,
         tags: Tuple[str],
         vas: Tuple[str],
@@ -130,15 +134,18 @@
         if all_:
             await self.get(ids)
             return
 
         # select RJs
         titles = [work["title"] for work in search_result["works"]]
         indexes = select_multiple(
-            [f"{id2rj(id_)} | {title}" for id_, title in zip(ids, titles)],
+            [
+                f"{id2source_name(id_)} | {title}"
+                for id_, title in zip(ids, titles)
+            ],
         )
         if not indexes:
             logger.error("Nothing was selected.")
             return
 
         await self.get([ids[i] for i in indexes])
 
@@ -150,38 +157,43 @@
 
     async def va(self, va_name: str, params: BrowseParams):
         """tag 和 va 一样，都是调用了特殊的search方法"""
         va_res = await self.downloader.tag(va_name, params=params.params)
         ids = [work["id"] for work in va_res["works"]]
         await self.get(ids)
 
-    async def update(self, ids: Iterable[RJID]):
-        async def update_one(rj_id_: RJID):
-            voice_info = await self.downloader.get_voice_info(rj_id_)
+    async def update(self, ids: List[RemoteSourceID]):
+        async def update_one(source_id_: RemoteSourceID):
+            voice_info = await self.downloader.get_voice_info(source_id_)
 
             # should_down = self.spider.json_should_download(voice_info)
             # if not should_down:
             #     logger.info(f"stop download {rj_id_}")
             #     return
             save_path = fm.storage_path
 
-            voice_path = save_path / id2rj(rj_id_)
+            local_source_id = source_name2id(voice_info["source_id"])
+            if local_source_id is None:
+                logger.error(f"Failded to convert {source_id_} to local id.")
+                return
+            voice_path = save_path / id2source_name(local_source_id)
+            assert voice_path.name == voice_info["source_id"]
             if not voice_path.exists():
                 logger.warning(
                     "There are no such files in your storage path for"
-                    f" RJ{rj_id_}"
+                    f" RJ{source_id_}"
                 )
 
             voice_path.mkdir(parents=True, exist_ok=True)
             self.downloader.create_info_file(voice_info, voice_path)
 
-            tracks = await self.downloader.get_voice_tracks(rj_id_)
+            tracks = await self.downloader.get_voice_tracks(source_id_)
             if isinstance(tracks, dict):
                 if error_info := tracks.get("error"):
-                    logger.error(f"RJ{rj_id_} not found, {error_info}")
+                    logger.error(f"RJ{source_id_} not found, {error_info}")
                     return
                 else:
                     logger.error("Unexpected track type: dict")
                     return
 
             file_list = self.downloader.get_file_list(tracks, voice_path)
             self.downloader.create_recover_file(file_list, voice_path)
@@ -216,15 +228,15 @@
             ],
             raw=raw,
         )
         print(f"({len(playlists)}/{total})")
 
         fm.save_playlist_cache(playlists)
 
-    async def remove(self, pl_ids: Iterable[uuid.UUID]):
+    async def remove(self, pl_ids: List[uuid.UUID]):
         res = await asyncio.gather(*map(self.playlist.delete_playlist, pl_ids))
 
         if not isinstance(res, list):
             logger.error(f"Unexpected response type when delete playlists.")
             return
         for r in res:
             if not isinstance(r, dict):
@@ -250,16 +262,16 @@
             logger.error(f"Unexpected response type when create playlist.")
             return
         if res.get("error"):
             logger.error(f"Error when creating playlist:{res}")
             return
         logger.info(f"Sucessfully create playlist: {res['id']}.")
 
-    async def add(self, rj_ids: Iterable[RJID], pl_id: uuid.UUID):
-        res = await self.playlist.add_works_to_playlist(rj_ids, pl_id)
+    async def add(self, source_ids: List[RemoteSourceID], pl_id: uuid.UUID):
+        res = await self.playlist.add_works_to_playlist(source_ids, pl_id)
         if not isinstance(res, dict):
             logger.error(
                 f"Unexpected response type when add works to {pl_id}."
             )
             return
         if res.get("error"):
             logger.error(f"Error when add works to playlist:{res}")
```

### Comparing `asmrmanager-1.9.1/asmrmanager/spider/playlist.py` & `asmrmanager-2.0.0/asmrmanager/spider/playlist.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import uuid
-from collections.abc import Iterable
 from typing import Any, List, Tuple
 
-from asmrmanager.common.rj_parse import RJID
-from asmrmanager.common.types import PRIVACY, PlayListItem
+from asmrmanager.common.rj_parse import SourceID
+from asmrmanager.common.types import PRIVACY, PlayListItem, RemoteSourceID
 
 from .asmrapi import ASMRAPI
 
 
 class ASMRPlayListAPI(ASMRAPI):
     def __init__(
         self, name: str, password: str, proxy: str | None, limit: int = 3
@@ -29,28 +28,28 @@
         name: str,
         desc: str | None = None,
         privacy: PRIVACY = PRIVACY.PRIVATE,
     ):
         return await self._create_playlist(name, desc, privacy.value)
 
     async def add_works_to_playlist(
-        self, rj_ids: Iterable[RJID], pl_id: uuid.UUID
+        self, source_ids: List[RemoteSourceID], pl_id: uuid.UUID
     ):
-        return await self._add_works_to_playlist(list(rj_ids), str(pl_id))
+        return await self._add_works_to_playlist(source_ids, str(pl_id))
 
     async def delete_playlist(self, pl_id: uuid.UUID):
         return await self._delete_playlist(str(pl_id))
 
     def process_playlists(self, playlists: List[Any]) -> List[PlayListItem]:
         res = []
         for item in playlists:
             res.append(
                 PlayListItem(
                     id=uuid.UUID(item["id"]),
                     name=item["name"],
                     privacy=PRIVACY(item["privacy"]),
                     desc=item["description"],
                     works_count=item["works_count"],
-                    latest_work_id=RJID(item["latestWorkID"]),
+                    latest_work_id=SourceID(item["latestWorkID"]),
                 )
             )
         return res
```

### Comparing `asmrmanager-1.9.1/asmrmanager/spider/utils/IDMHelper.py` & `asmrmanager-2.0.0/asmrmanager/spider/utils/IDMHelper.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/asmrmanager/spider/utils/aria2_downloader.py` & `asmrmanager-2.0.0/asmrmanager/spider/utils/aria2_downloader.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-1.9.1/pyproject.toml` & `asmrmanager-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,19 @@
     "rich>=13.0.0",
     "SQLAlchemy==2.0.10",
     "textual==0.26.0",
     "mutagen>=1.46.0",
     "appdirs>=1.4.4",
     "toml>=0.10.2",
     "beaupy>=3.7.2",
+    "asyncstdlib>=3.12.2",
 ]
 requires-python = ">=3.10,<3.12"
 readme = "README.md"
-version = "1.9.1"
+version = "2.0.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/slqy123/ASMRManager"
```

### Comparing `asmrmanager-1.9.1/PKG-INFO` & `asmrmanager-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ASMRManager
-Version: 1.9.1
+Version: 2.0.0
 Summary: download, manage and play the voices on asmr.one
-Keywords: asmr downloader music player manager cli tui commandline terminal
+Keywords: asmr,downloader,music,player,manager,cli,tui,commandline,terminal
 Author-Email: SLQY <sqiyel@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/slqy123/ASMRManager
 Requires-Python: <3.12,>=3.10
 Requires-Dist: aiohttp>=3.8.6
 Requires-Dist: chardet>=5.1.0
 Requires-Dist: click>=8.1.3
@@ -15,14 +15,15 @@
 Requires-Dist: rich>=13.0.0
 Requires-Dist: SQLAlchemy==2.0.10
 Requires-Dist: textual==0.26.0
 Requires-Dist: mutagen>=1.46.0
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: toml>=0.10.2
 Requires-Dist: beaupy>=3.7.2
+Requires-Dist: asyncstdlib>=3.12.2
 Requires-Dist: aioaria2>=1.3.4; extra == "aria2"
 Requires-Dist: comtypes>=1.2.0; extra == "idm"
 Requires-Dist: trogon==0.4.0; extra == "tui"
 Requires-Dist: pygame==2.4.0; extra == "pygame"
 Requires-Dist: python-mpd2>=3.1.0; extra == "mpd"
 Requires-Dist: black>=23.12.0; extra == "dev"
 Requires-Dist: autoflake>=2.2.1; extra == "dev"
@@ -118,14 +119,16 @@
 ### 播放
 
 非常简陋的终端播放界面，支持歌词显示，按照歌词信息快进，切换歌曲，支持以pygame(sdl)或mpd做为后端，可以预见的将来应该会完善一下(但感觉够用了应该不会再加啥功能了)。
 ![tui-screenshot](./assets/tui-screenshot.png)
 
 ## 使用方法
 
+**注意**：由于网站最近更新了针对BJ和VJ的支持，本项目进行了很大的重构，2.0.0 版本暂并不保证稳定运行，如果没有对BJ和VJ的需求，可以考虑继续使用1代的最后一个版本`pip install ASMRManager[依赖]==1.9.1`
+
 本工具支持 `python >= 3.10`, 安装方法如下：
 
 ```shell
 pip install ASMRManager[依赖]
 ```
 
 可选则的依赖项有 `idm`, `aria2`, `tui`，`pygame`,`mpd`, `all`，多个依赖使用逗号分隔，其中`all`为安装所有依赖。例如 `pip install ASMRManager[idm,tui]`
```

