# Comparing `tmp/txtai-7.0.0.tar.gz` & `tmp/txtai-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txtai-7.0.0.tar", last modified: Wed Feb 21 19:52:15 2024, max compression
+gzip compressed data, was "txtai-7.1.0.tar", last modified: Fri Apr 19 13:07:55 2024, max compression
```

## Comparing `txtai-7.0.0.tar` & `txtai-7.1.0.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.105217 txtai-7.0.0/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)    10754 2021-01-12 02:31:22.000000 txtai-7.0.0/LICENSE
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    26235 2024-02-21 19:52:15.105217 txtai-7.0.0/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    18503 2024-02-21 19:29:19.000000 txtai-7.0.0/README.md
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)       31 2021-01-23 16:25:29.000000 txtai-7.0.0/pyproject.toml
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2024-02-21 19:52:15.105217 txtai-7.0.0/setup.cfg
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3911 2024-02-20 23:25:28.000000 txtai-7.0.0/setup.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.087217 txtai-7.0.0/src/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.088217 txtai-7.0.0/src/python/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.089217 txtai-7.0.0/src/python/txtai/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2024-01-29 15:16:27.000000 txtai-7.0.0/src/python/txtai/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.089217 txtai-7.0.0/src/python/txtai/ann/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      198 2023-05-02 19:52:58.000000 txtai-7.0.0/src/python/txtai/ann/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1886 2023-09-08 13:19:22.000000 txtai-7.0.0/src/python/txtai/ann/annoy.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3205 2023-09-08 13:19:37.000000 txtai-7.0.0/src/python/txtai/ann/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1467 2023-06-14 16:28:58.000000 txtai-7.0.0/src/python/txtai/ann/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6526 2023-11-04 13:45:52.000000 txtai-7.0.0/src/python/txtai/ann/faiss.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3207 2023-10-27 17:13:57.000000 txtai-7.0.0/src/python/txtai/ann/hnsw.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4085 2023-10-27 19:09:06.000000 txtai-7.0.0/src/python/txtai/ann/numpy.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      894 2023-10-27 19:03:54.000000 txtai-7.0.0/src/python/txtai/ann/torch.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.090217 txtai-7.0.0/src/python/txtai/api/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      510 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2931 2024-02-05 22:48:18.000000 txtai-7.0.0/src/python/txtai/api/application.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1312 2023-12-26 16:31:07.000000 txtai-7.0.0/src/python/txtai/api/authorization.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4736 2024-02-20 16:43:38.000000 txtai-7.0.0/src/python/txtai/api/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8500 2024-02-20 16:44:37.000000 txtai-7.0.0/src/python/txtai/api/cluster.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-7.0.0/src/python/txtai/api/extension.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      640 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.090217 txtai-7.0.0/src/python/txtai/api/responses/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2024-02-06 01:16:00.000000 txtai-7.0.0/src/python/txtai/api/responses/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      608 2024-02-05 22:28:09.000000 txtai-7.0.0/src/python/txtai/api/responses/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1318 2024-02-06 16:38:51.000000 txtai-7.0.0/src/python/txtai/api/responses/json.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1007 2024-02-06 16:39:02.000000 txtai-7.0.0/src/python/txtai/api/responses/messagepack.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1375 2024-02-06 16:39:23.000000 txtai-7.0.0/src/python/txtai/api/route.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.091217 txtai-7.0.0/src/python/txtai/api/routers/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      357 2024-02-04 12:33:23.000000 txtai-7.0.0/src/python/txtai/api/routers/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      741 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7615 2024-02-20 16:53:10.000000 txtai-7.0.0/src/python/txtai/api/routers/embeddings.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      807 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/entity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      658 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1212 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/labels.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      843 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/objects.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      769 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/segmentation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1210 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/similarity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1188 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      803 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/tabular.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      782 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/textractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      795 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/transcription.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/translation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2024-02-06 16:31:35.000000 txtai-7.0.0/src/python/txtai/api/routers/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.091217 txtai-7.0.0/src/python/txtai/app/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-7.0.0/src/python/txtai/app/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24345 2024-02-20 16:53:11.000000 txtai-7.0.0/src/python/txtai/app/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.091217 txtai-7.0.0/src/python/txtai/archive/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-7.0.0/src/python/txtai/archive/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-7.0.0/src/python/txtai/archive/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-12-04 17:41:19.000000 txtai-7.0.0/src/python/txtai/archive/compress.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-7.0.0/src/python/txtai/archive/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-12-04 14:24:11.000000 txtai-7.0.0/src/python/txtai/archive/tar.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1027 2023-12-04 17:56:46.000000 txtai-7.0.0/src/python/txtai/archive/zip.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.091217 txtai-7.0.0/src/python/txtai/cloud/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-7.0.0/src/python/txtai/cloud/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-7.0.0/src/python/txtai/cloud/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-7.0.0/src/python/txtai/cloud/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-7.0.0/src/python/txtai/cloud/hub.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3783 2023-10-03 15:47:36.000000 txtai-7.0.0/src/python/txtai/cloud/storage.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.091217 txtai-7.0.0/src/python/txtai/console/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-7.0.0/src/python/txtai/console/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-7.0.0/src/python/txtai/console/__main__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-7.0.0/src/python/txtai/console/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.091217 txtai-7.0.0/src/python/txtai/data/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-7.0.0/src/python/txtai/data/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-7.0.0/src/python/txtai/data/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-7.0.0/src/python/txtai/data/labels.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-7.0.0/src/python/txtai/data/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-7.0.0/src/python/txtai/data/sequences.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-7.0.0/src/python/txtai/data/texts.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-7.0.0/src/python/txtai/data/tokens.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.092217 txtai-7.0.0/src/python/txtai/database/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2023-08-22 13:28:05.000000 txtai-7.0.0/src/python/txtai/database/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9739 2024-01-23 18:09:29.000000 txtai-7.0.0/src/python/txtai/database/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5291 2023-11-07 14:59:56.000000 txtai-7.0.0/src/python/txtai/database/client.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4381 2023-11-07 15:54:54.000000 txtai-7.0.0/src/python/txtai/database/duckdb.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1910 2023-08-23 11:53:19.000000 txtai-7.0.0/src/python/txtai/database/embedded.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.092217 txtai-7.0.0/src/python/txtai/database/encoder/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-7.0.0/src/python/txtai/database/encoder/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-7.0.0/src/python/txtai/database/encoder/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-7.0.0/src/python/txtai/database/encoder/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2023-04-21 14:52:54.000000 txtai-7.0.0/src/python/txtai/database/encoder/image.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      435 2023-08-07 00:41:39.000000 txtai-7.0.0/src/python/txtai/database/encoder/pickle.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1790 2023-09-07 14:18:38.000000 txtai-7.0.0/src/python/txtai/database/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16236 2024-02-06 15:37:09.000000 txtai-7.0.0/src/python/txtai/database/rdbms.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.092217 txtai-7.0.0/src/python/txtai/database/schema/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       76 2023-08-22 09:49:40.000000 txtai-7.0.0/src/python/txtai/database/schema/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2321 2023-08-26 00:47:23.000000 txtai-7.0.0/src/python/txtai/database/schema/orm.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3110 2023-09-19 13:47:26.000000 txtai-7.0.0/src/python/txtai/database/schema/statement.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.092217 txtai-7.0.0/src/python/txtai/database/sql/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-7.0.0/src/python/txtai/database/sql/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-7.0.0/src/python/txtai/database/sql/aggregate.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-10-26 16:22:14.000000 txtai-7.0.0/src/python/txtai/database/sql/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13855 2023-11-07 01:06:06.000000 txtai-7.0.0/src/python/txtai/database/sql/expression.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-7.0.0/src/python/txtai/database/sql/token.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1588 2023-08-22 13:25:25.000000 txtai-7.0.0/src/python/txtai/database/sqlite.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.092217 txtai-7.0.0/src/python/txtai/embeddings/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      100 2023-08-09 11:18:31.000000 txtai-7.0.0/src/python/txtai/embeddings/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    33582 2024-02-18 12:26:43.000000 txtai-7.0.0/src/python/txtai/embeddings/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.093217 txtai-7.0.0/src/python/txtai/embeddings/index/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      293 2024-02-02 12:33:35.000000 txtai-7.0.0/src/python/txtai/embeddings/index/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      152 2023-07-09 19:17:44.000000 txtai-7.0.0/src/python/txtai/embeddings/index/action.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2154 2023-07-10 16:44:09.000000 txtai-7.0.0/src/python/txtai/embeddings/index/autoid.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1890 2023-08-09 09:52:25.000000 txtai-7.0.0/src/python/txtai/embeddings/index/documents.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4329 2023-08-08 10:14:35.000000 txtai-7.0.0/src/python/txtai/embeddings/index/functions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4263 2024-02-02 14:35:15.000000 txtai-7.0.0/src/python/txtai/embeddings/index/indexes.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1286 2024-01-30 20:32:31.000000 txtai-7.0.0/src/python/txtai/embeddings/index/indexids.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2717 2023-08-09 10:05:10.000000 txtai-7.0.0/src/python/txtai/embeddings/index/reducer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2109 2023-08-23 14:12:53.000000 txtai-7.0.0/src/python/txtai/embeddings/index/stream.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7192 2024-01-19 01:38:26.000000 txtai-7.0.0/src/python/txtai/embeddings/index/transform.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.093217 txtai-7.0.0/src/python/txtai/embeddings/search/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      194 2024-01-21 13:37:35.000000 txtai-7.0.0/src/python/txtai/embeddings/search/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9317 2024-01-30 16:50:02.000000 txtai-7.0.0/src/python/txtai/embeddings/search/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      138 2023-08-08 13:42:50.000000 txtai-7.0.0/src/python/txtai/embeddings/search/errors.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4132 2023-07-25 21:39:08.000000 txtai-7.0.0/src/python/txtai/embeddings/search/explain.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1305 2024-01-30 16:48:28.000000 txtai-7.0.0/src/python/txtai/embeddings/search/ids.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-7.0.0/src/python/txtai/embeddings/search/query.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6023 2023-11-07 15:38:49.000000 txtai-7.0.0/src/python/txtai/embeddings/search/scan.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-7.0.0/src/python/txtai/embeddings/search/terms.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.093217 txtai-7.0.0/src/python/txtai/graph/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      139 2022-09-03 13:13:44.000000 txtai-7.0.0/src/python/txtai/graph/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    21228 2024-02-20 15:22:59.000000 txtai-7.0.0/src/python/txtai/graph/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1133 2023-06-14 16:29:08.000000 txtai-7.0.0/src/python/txtai/graph/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6393 2024-02-20 23:25:28.000000 txtai-7.0.0/src/python/txtai/graph/networkx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4549 2024-01-22 22:57:23.000000 txtai-7.0.0/src/python/txtai/graph/topics.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.093217 txtai-7.0.0/src/python/txtai/models/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      176 2023-10-06 15:17:23.000000 txtai-7.0.0/src/python/txtai/models/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7416 2023-11-01 19:05:30.000000 txtai-7.0.0/src/python/txtai/models/models.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3508 2023-02-19 19:01:48.000000 txtai-7.0.0/src/python/txtai/models/onnx.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.093217 txtai-7.0.0/src/python/txtai/models/pooling/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2023-10-09 16:17:44.000000 txtai-7.0.0/src/python/txtai/models/pooling/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3025 2023-10-09 15:30:36.000000 txtai-7.0.0/src/python/txtai/models/pooling/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      563 2023-10-09 16:01:10.000000 txtai-7.0.0/src/python/txtai/models/pooling/cls.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2244 2023-10-09 16:23:50.000000 txtai-7.0.0/src/python/txtai/models/pooling/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      801 2023-10-06 16:10:02.000000 txtai-7.0.0/src/python/txtai/models/pooling/mean.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-7.0.0/src/python/txtai/models/registry.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4659 2023-04-14 21:23:31.000000 txtai-7.0.0/src/python/txtai/models/tokendetection.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.094217 txtai-7.0.0/src/python/txtai/pipeline/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      326 2023-12-09 16:19:47.000000 txtai-7.0.0/src/python/txtai/pipeline/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.094217 txtai-7.0.0/src/python/txtai/pipeline/audio/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/audio/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3823 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/audio/texttospeech.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6568 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/audio/transcription.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      536 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.094217 txtai-7.0.0/src/python/txtai/pipeline/data/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/data/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3765 2023-11-29 13:00:51.000000 txtai-7.0.0/src/python/txtai/pipeline/data/segmentation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/data/tabular.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7455 2023-12-24 14:57:25.000000 txtai-7.0.0/src/python/txtai/pipeline/data/textractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4236 2023-12-03 15:18:53.000000 txtai-7.0.0/src/python/txtai/pipeline/data/tokenizer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3684 2023-09-26 13:45:56.000000 txtai-7.0.0/src/python/txtai/pipeline/hfmodel.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3530 2023-09-26 13:33:11.000000 txtai-7.0.0/src/python/txtai/pipeline/hfpipeline.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.094217 txtai-7.0.0/src/python/txtai/pipeline/image/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/image/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1523 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/image/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/image/imagehash.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2726 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/image/objects.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.094217 txtai-7.0.0/src/python/txtai/pipeline/llm/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      200 2023-12-09 16:43:34.000000 txtai-7.0.0/src/python/txtai/pipeline/llm/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1998 2023-12-09 11:31:56.000000 txtai-7.0.0/src/python/txtai/pipeline/llm/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2154 2023-12-09 03:15:53.000000 txtai-7.0.0/src/python/txtai/pipeline/llm/generation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3710 2023-12-09 01:27:30.000000 txtai-7.0.0/src/python/txtai/pipeline/llm/huggingface.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1868 2023-12-26 16:19:57.000000 txtai-7.0.0/src/python/txtai/pipeline/llm/litellm.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1841 2023-12-09 17:55:52.000000 txtai-7.0.0/src/python/txtai/pipeline/llm/llama.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1267 2023-12-09 16:40:59.000000 txtai-7.0.0/src/python/txtai/pipeline/llm/llm.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/nop.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/tensors.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.095217 txtai-7.0.0/src/python/txtai/pipeline/text/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      282 2023-12-09 16:19:47.000000 txtai-7.0.0/src/python/txtai/pipeline/text/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2619 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/text/crossencoder.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2539 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/text/entity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    17142 2023-12-16 17:56:03.000000 txtai-7.0.0/src/python/txtai/pipeline/text/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5328 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/text/labels.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1417 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/text/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2257 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/text/similarity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2836 2023-07-08 20:26:24.000000 txtai-7.0.0/src/python/txtai/pipeline/text/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9333 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/text/translation.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.095217 txtai-7.0.0/src/python/txtai/pipeline/train/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/train/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5998 2023-10-09 15:52:01.000000 txtai-7.0.0/src/python/txtai/pipeline/train/hfonnx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13634 2024-01-31 20:03:20.000000 txtai-7.0.0/src/python/txtai/pipeline/train/hftrainer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1991 2023-07-07 22:15:31.000000 txtai-7.0.0/src/python/txtai/pipeline/train/mlonnx.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.095217 txtai-7.0.0/src/python/txtai/scoring/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      156 2023-07-18 19:36:05.000000 txtai-7.0.0/src/python/txtai/scoring/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    12600 2023-09-02 13:44:59.000000 txtai-7.0.0/src/python/txtai/scoring/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      673 2023-07-27 01:21:09.000000 txtai-7.0.0/src/python/txtai/scoring/bm25.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1603 2023-09-06 21:23:10.000000 txtai-7.0.0/src/python/txtai/scoring/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      846 2023-07-20 01:44:25.000000 txtai-7.0.0/src/python/txtai/scoring/sif.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14471 2023-08-08 10:55:46.000000 txtai-7.0.0/src/python/txtai/scoring/terms.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.095217 txtai-7.0.0/src/python/txtai/util/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       96 2023-10-03 17:56:55.000000 txtai-7.0.0/src/python/txtai/util/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2023-07-10 16:06:01.000000 txtai-7.0.0/src/python/txtai/util/resolver.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      349 2023-10-03 18:38:54.000000 txtai-7.0.0/src/python/txtai/util/template.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.095217 txtai-7.0.0/src/python/txtai/vectors/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      201 2022-05-12 15:49:17.000000 txtai-7.0.0/src/python/txtai/vectors/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7660 2023-10-28 16:32:30.000000 txtai-7.0.0/src/python/txtai/vectors/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1548 2024-01-29 20:20:38.000000 txtai-7.0.0/src/python/txtai/vectors/external.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1870 2023-07-20 17:41:39.000000 txtai-7.0.0/src/python/txtai/vectors/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1809 2023-12-05 02:54:51.000000 txtai-7.0.0/src/python/txtai/vectors/transformers.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6579 2023-08-07 00:44:22.000000 txtai-7.0.0/src/python/txtai/vectors/words.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      111 2024-02-18 12:13:38.000000 txtai-7.0.0/src/python/txtai/version.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.096217 txtai-7.0.0/src/python/txtai/workflow/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2023-03-21 22:13:38.000000 txtai-7.0.0/src/python/txtai/workflow/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5486 2023-04-14 21:51:47.000000 txtai-7.0.0/src/python/txtai/workflow/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2845 2021-12-05 00:26:44.000000 txtai-7.0.0/src/python/txtai/workflow/execute.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      965 2023-04-14 21:51:47.000000 txtai-7.0.0/src/python/txtai/workflow/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.096217 txtai-7.0.0/src/python/txtai/workflow/task/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      440 2023-04-14 21:51:47.000000 txtai-7.0.0/src/python/txtai/workflow/task/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-11 17:31:41.000000 txtai-7.0.0/src/python/txtai/workflow/task/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-7.0.0/src/python/txtai/workflow/task/console.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-7.0.0/src/python/txtai/workflow/task/export.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-7.0.0/src/python/txtai/workflow/task/factory.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-7.0.0/src/python/txtai/workflow/task/file.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-7.0.0/src/python/txtai/workflow/task/image.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1711 2023-10-03 16:41:51.000000 txtai-7.0.0/src/python/txtai/workflow/task/retrieve.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-7.0.0/src/python/txtai/workflow/task/service.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3342 2023-10-03 15:07:03.000000 txtai-7.0.0/src/python/txtai/workflow/task/storage.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      935 2023-04-17 14:31:28.000000 txtai-7.0.0/src/python/txtai/workflow/task/stream.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3453 2023-10-14 10:26:45.000000 txtai-7.0.0/src/python/txtai/workflow/task/template.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-7.0.0/src/python/txtai/workflow/task/url.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-7.0.0/src/python/txtai/workflow/task/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-02-21 19:52:15.089217 txtai-7.0.0/src/python/txtai.egg-info/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    26235 2024-02-21 19:52:15.000000 txtai-7.0.0/src/python/txtai.egg-info/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7552 2024-02-21 19:52:15.000000 txtai-7.0.0/src/python/txtai.egg-info/SOURCES.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2024-02-21 19:52:15.000000 txtai-7.0.0/src/python/txtai.egg-info/dependency_links.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2024-02-21 19:52:15.000000 txtai-7.0.0/src/python/txtai.egg-info/requires.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2024-02-21 19:52:15.000000 txtai-7.0.0/src/python/txtai.egg-info/top_level.txt
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.488750 txtai-7.1.0/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)    10754 2021-01-12 02:31:22.000000 txtai-7.1.0/LICENSE
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    26266 2024-04-19 13:07:55.488750 txtai-7.1.0/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    18444 2024-04-18 17:11:10.000000 txtai-7.1.0/README.md
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)       31 2021-01-23 16:25:29.000000 txtai-7.1.0/pyproject.toml
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2024-04-19 13:07:55.488750 txtai-7.1.0/setup.cfg
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3932 2024-04-19 10:24:30.000000 txtai-7.1.0/setup.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.470749 txtai-7.1.0/src/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.470749 txtai-7.1.0/src/python/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.472750 txtai-7.1.0/src/python/txtai/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2024-01-29 15:16:27.000000 txtai-7.1.0/src/python/txtai/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.472750 txtai-7.1.0/src/python/txtai/ann/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      198 2023-05-02 19:52:58.000000 txtai-7.1.0/src/python/txtai/ann/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1886 2023-09-08 13:19:22.000000 txtai-7.1.0/src/python/txtai/ann/annoy.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3205 2023-09-08 13:19:37.000000 txtai-7.1.0/src/python/txtai/ann/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1467 2023-06-14 16:28:58.000000 txtai-7.1.0/src/python/txtai/ann/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6526 2023-11-04 13:45:52.000000 txtai-7.1.0/src/python/txtai/ann/faiss.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3207 2023-10-27 17:13:57.000000 txtai-7.1.0/src/python/txtai/ann/hnsw.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4085 2023-10-27 19:09:06.000000 txtai-7.1.0/src/python/txtai/ann/numpy.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      894 2023-10-27 19:03:54.000000 txtai-7.1.0/src/python/txtai/ann/torch.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/api/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      510 2024-03-30 12:38:43.000000 txtai-7.1.0/src/python/txtai/api/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2931 2024-02-05 22:48:18.000000 txtai-7.1.0/src/python/txtai/api/application.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1312 2023-12-26 16:31:07.000000 txtai-7.1.0/src/python/txtai/api/authorization.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4736 2024-02-20 16:43:38.000000 txtai-7.1.0/src/python/txtai/api/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8500 2024-02-20 16:44:37.000000 txtai-7.1.0/src/python/txtai/api/cluster.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-7.1.0/src/python/txtai/api/extension.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      640 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/api/responses/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2024-02-06 01:16:00.000000 txtai-7.1.0/src/python/txtai/api/responses/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      608 2024-02-05 22:28:09.000000 txtai-7.1.0/src/python/txtai/api/responses/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1318 2024-02-06 16:38:51.000000 txtai-7.1.0/src/python/txtai/api/responses/json.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1007 2024-02-06 16:39:02.000000 txtai-7.1.0/src/python/txtai/api/responses/messagepack.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1375 2024-02-06 16:39:23.000000 txtai-7.1.0/src/python/txtai/api/route.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/api/routers/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      357 2024-02-04 12:33:23.000000 txtai-7.1.0/src/python/txtai/api/routers/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      741 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7615 2024-02-20 16:53:10.000000 txtai-7.1.0/src/python/txtai/api/routers/embeddings.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      807 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      658 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1212 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/labels.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      843 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/objects.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      769 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/segmentation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1210 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/similarity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1188 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      803 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/tabular.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      782 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/textractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      795 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/transcription.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/translation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/app/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-7.1.0/src/python/txtai/app/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24345 2024-02-20 16:53:11.000000 txtai-7.1.0/src/python/txtai/app/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/archive/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-7.1.0/src/python/txtai/archive/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-7.1.0/src/python/txtai/archive/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-12-04 17:41:19.000000 txtai-7.1.0/src/python/txtai/archive/compress.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-7.1.0/src/python/txtai/archive/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-12-04 14:24:11.000000 txtai-7.1.0/src/python/txtai/archive/tar.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1027 2023-12-04 17:56:46.000000 txtai-7.1.0/src/python/txtai/archive/zip.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/cloud/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-7.1.0/src/python/txtai/cloud/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-7.1.0/src/python/txtai/cloud/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-7.1.0/src/python/txtai/cloud/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-7.1.0/src/python/txtai/cloud/hub.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3741 2024-03-05 16:14:02.000000 txtai-7.1.0/src/python/txtai/cloud/storage.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/console/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-7.1.0/src/python/txtai/console/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-7.1.0/src/python/txtai/console/__main__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-7.1.0/src/python/txtai/console/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/data/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-7.1.0/src/python/txtai/data/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-7.1.0/src/python/txtai/data/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-7.1.0/src/python/txtai/data/labels.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-7.1.0/src/python/txtai/data/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-7.1.0/src/python/txtai/data/sequences.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-7.1.0/src/python/txtai/data/texts.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-7.1.0/src/python/txtai/data/tokens.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2023-08-22 13:28:05.000000 txtai-7.1.0/src/python/txtai/database/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9739 2024-01-23 18:09:29.000000 txtai-7.1.0/src/python/txtai/database/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5308 2024-04-17 12:20:59.000000 txtai-7.1.0/src/python/txtai/database/client.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4381 2023-11-07 15:54:54.000000 txtai-7.1.0/src/python/txtai/database/duckdb.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1801 2024-04-17 12:20:59.000000 txtai-7.1.0/src/python/txtai/database/embedded.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/encoder/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-7.1.0/src/python/txtai/database/encoder/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-7.1.0/src/python/txtai/database/encoder/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-7.1.0/src/python/txtai/database/encoder/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2023-04-21 14:52:54.000000 txtai-7.1.0/src/python/txtai/database/encoder/image.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      435 2023-08-07 00:41:39.000000 txtai-7.1.0/src/python/txtai/database/encoder/pickle.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1790 2023-09-07 14:18:38.000000 txtai-7.1.0/src/python/txtai/database/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16441 2024-04-17 12:20:59.000000 txtai-7.1.0/src/python/txtai/database/rdbms.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/schema/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       76 2023-08-22 09:49:40.000000 txtai-7.1.0/src/python/txtai/database/schema/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2321 2023-08-26 00:47:23.000000 txtai-7.1.0/src/python/txtai/database/schema/orm.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3110 2023-09-19 13:47:26.000000 txtai-7.1.0/src/python/txtai/database/schema/statement.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/sql/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-7.1.0/src/python/txtai/database/sql/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-7.1.0/src/python/txtai/database/sql/aggregate.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-10-26 16:22:14.000000 txtai-7.1.0/src/python/txtai/database/sql/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13855 2023-11-07 01:06:06.000000 txtai-7.1.0/src/python/txtai/database/sql/expression.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-7.1.0/src/python/txtai/database/sql/token.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1588 2023-08-22 13:25:25.000000 txtai-7.1.0/src/python/txtai/database/sqlite.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/embeddings/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      100 2023-08-09 11:18:31.000000 txtai-7.1.0/src/python/txtai/embeddings/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    33434 2024-04-17 11:52:42.000000 txtai-7.1.0/src/python/txtai/embeddings/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/embeddings/index/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      293 2024-02-02 12:33:35.000000 txtai-7.1.0/src/python/txtai/embeddings/index/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      152 2023-07-09 19:17:44.000000 txtai-7.1.0/src/python/txtai/embeddings/index/action.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2154 2023-07-10 16:44:09.000000 txtai-7.1.0/src/python/txtai/embeddings/index/autoid.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1890 2023-08-09 09:52:25.000000 txtai-7.1.0/src/python/txtai/embeddings/index/documents.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4329 2023-08-08 10:14:35.000000 txtai-7.1.0/src/python/txtai/embeddings/index/functions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4568 2024-02-28 15:34:15.000000 txtai-7.1.0/src/python/txtai/embeddings/index/indexes.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1286 2024-01-30 20:32:31.000000 txtai-7.1.0/src/python/txtai/embeddings/index/indexids.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2717 2023-08-09 10:05:10.000000 txtai-7.1.0/src/python/txtai/embeddings/index/reducer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2109 2023-08-23 14:12:53.000000 txtai-7.1.0/src/python/txtai/embeddings/index/stream.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7192 2024-01-19 01:38:26.000000 txtai-7.1.0/src/python/txtai/embeddings/index/transform.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/embeddings/search/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      194 2024-01-21 13:37:35.000000 txtai-7.1.0/src/python/txtai/embeddings/search/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9490 2024-03-31 16:05:43.000000 txtai-7.1.0/src/python/txtai/embeddings/search/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      138 2023-08-08 13:42:50.000000 txtai-7.1.0/src/python/txtai/embeddings/search/errors.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4132 2023-07-25 21:39:08.000000 txtai-7.1.0/src/python/txtai/embeddings/search/explain.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1305 2024-01-30 16:48:28.000000 txtai-7.1.0/src/python/txtai/embeddings/search/ids.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-7.1.0/src/python/txtai/embeddings/search/query.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6023 2023-11-07 15:38:49.000000 txtai-7.1.0/src/python/txtai/embeddings/search/scan.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-7.1.0/src/python/txtai/embeddings/search/terms.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/graph/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      139 2022-09-03 13:13:44.000000 txtai-7.1.0/src/python/txtai/graph/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    21990 2024-04-17 12:28:46.000000 txtai-7.1.0/src/python/txtai/graph/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1133 2023-06-14 16:29:08.000000 txtai-7.1.0/src/python/txtai/graph/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6543 2024-04-17 12:28:46.000000 txtai-7.1.0/src/python/txtai/graph/networkx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4549 2024-01-22 22:57:23.000000 txtai-7.1.0/src/python/txtai/graph/topics.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/models/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      176 2023-10-06 15:17:23.000000 txtai-7.1.0/src/python/txtai/models/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7543 2024-02-28 00:08:15.000000 txtai-7.1.0/src/python/txtai/models/models.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3508 2023-02-19 19:01:48.000000 txtai-7.1.0/src/python/txtai/models/onnx.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/models/pooling/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2023-10-09 16:17:44.000000 txtai-7.1.0/src/python/txtai/models/pooling/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3112 2024-02-28 00:07:11.000000 txtai-7.1.0/src/python/txtai/models/pooling/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      563 2023-10-09 16:01:10.000000 txtai-7.1.0/src/python/txtai/models/pooling/cls.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2351 2024-02-28 00:04:26.000000 txtai-7.1.0/src/python/txtai/models/pooling/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      801 2023-10-06 16:10:02.000000 txtai-7.1.0/src/python/txtai/models/pooling/mean.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-7.1.0/src/python/txtai/models/registry.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4659 2023-04-14 21:23:31.000000 txtai-7.1.0/src/python/txtai/models/tokendetection.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      326 2023-12-09 16:19:47.000000 txtai-7.1.0/src/python/txtai/pipeline/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/audio/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/audio/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3823 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/audio/texttospeech.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6568 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/audio/transcription.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      536 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/data/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/data/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3765 2023-11-29 13:00:51.000000 txtai-7.1.0/src/python/txtai/pipeline/data/segmentation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/data/tabular.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7455 2024-03-05 18:21:46.000000 txtai-7.1.0/src/python/txtai/pipeline/data/textractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4236 2023-12-03 15:18:53.000000 txtai-7.1.0/src/python/txtai/pipeline/data/tokenizer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3684 2023-09-26 13:45:56.000000 txtai-7.1.0/src/python/txtai/pipeline/hfmodel.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3530 2023-09-26 13:33:11.000000 txtai-7.1.0/src/python/txtai/pipeline/hfpipeline.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/image/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/image/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1523 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/image/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/image/imagehash.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2726 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/image/objects.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/llm/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      200 2023-12-09 16:43:34.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1998 2023-12-09 11:31:56.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2154 2023-12-09 03:15:53.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/generation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3710 2023-12-09 01:27:30.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/huggingface.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1868 2023-12-26 16:19:57.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/litellm.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1841 2023-12-09 17:55:52.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/llama.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1267 2023-12-09 16:40:59.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/llm.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/nop.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/tensors.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/pipeline/text/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      282 2023-12-09 16:19:47.000000 txtai-7.1.0/src/python/txtai/pipeline/text/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2619 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/crossencoder.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2539 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    17142 2023-12-16 17:56:03.000000 txtai-7.1.0/src/python/txtai/pipeline/text/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5328 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/labels.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1417 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2257 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/similarity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2836 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9333 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/text/translation.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/pipeline/train/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/train/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5998 2023-10-09 15:52:01.000000 txtai-7.1.0/src/python/txtai/pipeline/train/hfonnx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13634 2024-01-31 20:03:20.000000 txtai-7.1.0/src/python/txtai/pipeline/train/hftrainer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1991 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/train/mlonnx.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/scoring/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      156 2023-07-18 19:36:05.000000 txtai-7.1.0/src/python/txtai/scoring/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    12600 2023-09-02 13:44:59.000000 txtai-7.1.0/src/python/txtai/scoring/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      673 2023-07-27 01:21:09.000000 txtai-7.1.0/src/python/txtai/scoring/bm25.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1603 2023-09-06 21:23:10.000000 txtai-7.1.0/src/python/txtai/scoring/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      846 2023-07-20 01:44:25.000000 txtai-7.1.0/src/python/txtai/scoring/sif.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14471 2023-08-08 10:55:46.000000 txtai-7.1.0/src/python/txtai/scoring/terms.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/util/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       96 2023-10-03 17:56:55.000000 txtai-7.1.0/src/python/txtai/util/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2023-07-10 16:06:01.000000 txtai-7.1.0/src/python/txtai/util/resolver.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      349 2023-10-03 18:38:54.000000 txtai-7.1.0/src/python/txtai/util/template.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.479750 txtai-7.1.0/src/python/txtai/vectors/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      201 2022-05-12 15:49:17.000000 txtai-7.1.0/src/python/txtai/vectors/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9070 2024-03-11 01:48:40.000000 txtai-7.1.0/src/python/txtai/vectors/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1569 2024-02-27 23:36:17.000000 txtai-7.1.0/src/python/txtai/vectors/external.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1945 2024-02-27 22:21:09.000000 txtai-7.1.0/src/python/txtai/vectors/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2115 2024-02-28 02:20:24.000000 txtai-7.1.0/src/python/txtai/vectors/transformers.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2024-02-27 23:36:29.000000 txtai-7.1.0/src/python/txtai/vectors/words.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      111 2024-02-22 01:16:23.000000 txtai-7.1.0/src/python/txtai/version.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.479750 txtai-7.1.0/src/python/txtai/workflow/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2023-03-21 22:13:38.000000 txtai-7.1.0/src/python/txtai/workflow/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5486 2023-04-14 21:51:47.000000 txtai-7.1.0/src/python/txtai/workflow/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2845 2021-12-05 00:26:44.000000 txtai-7.1.0/src/python/txtai/workflow/execute.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      965 2023-04-14 21:51:47.000000 txtai-7.1.0/src/python/txtai/workflow/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.479750 txtai-7.1.0/src/python/txtai/workflow/task/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      440 2023-04-14 21:51:47.000000 txtai-7.1.0/src/python/txtai/workflow/task/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-11 17:31:41.000000 txtai-7.1.0/src/python/txtai/workflow/task/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-7.1.0/src/python/txtai/workflow/task/console.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-7.1.0/src/python/txtai/workflow/task/export.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-7.1.0/src/python/txtai/workflow/task/factory.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-7.1.0/src/python/txtai/workflow/task/file.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-7.1.0/src/python/txtai/workflow/task/image.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1711 2023-10-03 16:41:51.000000 txtai-7.1.0/src/python/txtai/workflow/task/retrieve.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-7.1.0/src/python/txtai/workflow/task/service.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3295 2024-03-05 16:14:02.000000 txtai-7.1.0/src/python/txtai/workflow/task/storage.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      935 2023-04-17 14:31:28.000000 txtai-7.1.0/src/python/txtai/workflow/task/stream.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3453 2023-10-14 10:26:45.000000 txtai-7.1.0/src/python/txtai/workflow/task/template.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-7.1.0/src/python/txtai/workflow/task/url.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-7.1.0/src/python/txtai/workflow/task/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.472750 txtai-7.1.0/src/python/txtai.egg-info/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    26266 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7552 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/SOURCES.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/dependency_links.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2438 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/requires.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/top_level.txt
```

### Comparing `txtai-7.0.0/LICENSE` & `txtai-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/PKG-INFO` & `txtai-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 7.0.0
+Version: 7.1.0
 Summary: All-in-one open-source embeddings database for semantic search, LLM orchestration and language model workflows
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
@@ -17,15 +17,15 @@
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: faiss-cpu>=1.7.1.post2
 Requires-Dist: torch>=1.12.1
-Requires-Dist: transformers>=4.27.0
+Requires-Dist: transformers>=4.28.0
 Requires-Dist: huggingface-hub>=0.9.0
 Requires-Dist: numpy>=1.18.4
 Requires-Dist: pyyaml>=5.3
 Requires-Dist: regex>=2022.8.17
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
@@ -36,14 +36,15 @@
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Provides-Extra: api
 Requires-Dist: aiohttp>=3.8.1; extra == "api"
 Requires-Dist: fastapi>=0.94.0; extra == "api"
 Requires-Dist: msgpack>=1.0.7; extra == "api"
+Requires-Dist: pillow>=7.1.2; extra == "api"
 Requires-Dist: python-multipart>=0.0.7; extra == "api"
 Requires-Dist: uvicorn>=0.12.1; extra == "api"
 Provides-Extra: cloud
 Requires-Dist: apache-libcloud>=3.3.1; extra == "cloud"
 Provides-Extra: console
 Requires-Dist: rich>=12.0.1; extra == "console"
 Provides-Extra: database
@@ -69,21 +70,21 @@
 Requires-Dist: pandas>=1.1.0; extra == "pipeline-data"
 Requires-Dist: tika>=1.24; extra == "pipeline-data"
 Provides-Extra: pipeline-image
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline-image"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline-image"
 Requires-Dist: timm>=0.4.12; extra == "pipeline-image"
 Provides-Extra: pipeline-llm
-Requires-Dist: litellm>=1.15.8; extra == "pipeline-llm"
+Requires-Dist: litellm>=1.31.2; extra == "pipeline-llm"
 Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline-llm"
 Provides-Extra: pipeline-text
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline-text"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline-text"
 Provides-Extra: pipeline-train
-Requires-Dist: accelerate>=0.19.0; extra == "pipeline-train"
+Requires-Dist: accelerate>=0.26.0; extra == "pipeline-train"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline-train"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline-train"
 Requires-Dist: onnxmltools>=1.9.1; extra == "pipeline-train"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline-train"
 Requires-Dist: peft>=0.8.1; extra == "pipeline-train"
 Requires-Dist: skl2onnx>=1.9.1; extra == "pipeline-train"
 Provides-Extra: pipeline
@@ -95,19 +96,19 @@
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "pipeline"
 Requires-Dist: nltk>=3.5; extra == "pipeline"
 Requires-Dist: pandas>=1.1.0; extra == "pipeline"
 Requires-Dist: tika>=1.24; extra == "pipeline"
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline"
 Requires-Dist: timm>=0.4.12; extra == "pipeline"
-Requires-Dist: litellm>=1.15.8; extra == "pipeline"
+Requires-Dist: litellm>=1.31.2; extra == "pipeline"
 Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline"
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline"
-Requires-Dist: accelerate>=0.19.0; extra == "pipeline"
+Requires-Dist: accelerate>=0.26.0; extra == "pipeline"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline"
 Requires-Dist: onnxmltools>=1.9.1; extra == "pipeline"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline"
 Requires-Dist: peft>=0.8.1; extra == "pipeline"
 Requires-Dist: skl2onnx>=1.9.1; extra == "pipeline"
 Provides-Extra: similarity
@@ -125,14 +126,15 @@
 Requires-Dist: pillow>=7.1.2; extra == "workflow"
 Requires-Dist: requests>=2.26.0; extra == "workflow"
 Requires-Dist: xmltodict>=0.12.0; extra == "workflow"
 Provides-Extra: all
 Requires-Dist: aiohttp>=3.8.1; extra == "all"
 Requires-Dist: fastapi>=0.94.0; extra == "all"
 Requires-Dist: msgpack>=1.0.7; extra == "all"
+Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: python-multipart>=0.0.7; extra == "all"
 Requires-Dist: uvicorn>=0.12.1; extra == "all"
 Requires-Dist: apache-libcloud>=3.3.1; extra == "all"
 Requires-Dist: rich>=12.0.1; extra == "all"
 Requires-Dist: duckdb>=0.7.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
@@ -149,19 +151,19 @@
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "all"
 Requires-Dist: nltk>=3.5; extra == "all"
 Requires-Dist: pandas>=1.1.0; extra == "all"
 Requires-Dist: tika>=1.24; extra == "all"
 Requires-Dist: imagehash>=4.2.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: timm>=0.4.12; extra == "all"
-Requires-Dist: litellm>=1.15.8; extra == "all"
+Requires-Dist: litellm>=1.31.2; extra == "all"
 Requires-Dist: llama-cpp-python>=0.2.20; extra == "all"
 Requires-Dist: fasttext>=0.9.2; extra == "all"
 Requires-Dist: sentencepiece>=0.1.91; extra == "all"
-Requires-Dist: accelerate>=0.19.0; extra == "all"
+Requires-Dist: accelerate>=0.26.0; extra == "all"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxmltools>=1.9.1; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: peft>=0.8.1; extra == "all"
 Requires-Dist: skl2onnx>=1.9.1; extra == "all"
 Requires-Dist: annoy>=1.16.3; extra == "all"
@@ -307,16 +309,16 @@
 ![rag](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/rag.png#gh-light-mode-only)
 
 A novel feature of txtai is that it can provide both an answer and source citation.
 
 | Notebook  | Description  |       |
 |:----------|:-------------|------:|
 | [Build RAG pipelines with txtai](https://github.com/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) | Guide on retrieval augmented generation including how to create citations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) |
-| [Generate knowledge with Semantic Graphs and RAG](https://github.com/neuml/txtai/blob/master/examples/55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) | Knowledge exploration and discovery with Semantic Graphs and RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) |
 | [Advanced RAG with graph path traversal](https://github.com/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) | Graph path traversal to collect complex sets of data for advanced RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) |
+| [Advanced RAG with guided generation](https://github.com/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) |
 
 ### Language Model Workflows
 
 Language model workflows, also known as semantic workflows, connect language models together to build intelligent applications.
 
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
```

### Comparing `txtai-7.0.0/README.md` & `txtai-7.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,16 @@
 ![rag](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/rag-dark.png#gh-dark-mode-only)
 
 A novel feature of txtai is that it can provide both an answer and source citation.
 
 | Notebook  | Description  |       |
 |:----------|:-------------|------:|
 | [Build RAG pipelines with txtai](https://github.com/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) | Guide on retrieval augmented generation including how to create citations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) |
-| [Generate knowledge with Semantic Graphs and RAG](https://github.com/neuml/txtai/blob/master/examples/55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) | Knowledge exploration and discovery with Semantic Graphs and RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) |
 | [Advanced RAG with graph path traversal](https://github.com/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) | Graph path traversal to collect complex sets of data for advanced RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) |
+| [Advanced RAG with guided generation](https://github.com/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) |
 
 ### Language Model Workflows
 
 Language model workflows, also known as semantic workflows, connect language models together to build intelligent applications.
 
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows-dark.png#gh-dark-mode-only)
```

#### html2text {}

```diff
@@ -108,29 +108,28 @@
 rag-dark.png#gh-dark-mode-only) A novel feature of txtai is that it can provide
 both an answer and source citation. | Notebook | Description | | |:----------|:
 -------------|------:| | [Build RAG pipelines with txtai](https://github.com/
 neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) |
 Guide on retrieval augmented generation including how to create citations | [!
 [Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/github/neuml/txtai/blob/master/examples/
-52_Build_RAG_pipelines_with_txtai.ipynb) | | [Generate knowledge with Semantic
-Graphs and RAG](https://github.com/neuml/txtai/blob/master/examples/
-55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) | Knowledge
-exploration and discovery with Semantic Graphs and RAG | [![Open In Colab]
-(https://colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/github/neuml/txtai/blob/master/examples/
-55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) | | [Advanced RAG
-with graph path traversal](https://github.com/neuml/txtai/blob/master/examples/
+52_Build_RAG_pipelines_with_txtai.ipynb) | | [Advanced RAG with graph path
+traversal](https://github.com/neuml/txtai/blob/master/examples/
 58_Advanced_RAG_with_graph_path_traversal.ipynb) | Graph path traversal to
 collect complex sets of data for advanced RAG | [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
-58_Advanced_RAG_with_graph_path_traversal.ipynb) | ### Language Model Workflows
-Language model workflows, also known as semantic workflows, connect language
-models together to build intelligent applications. ![flows](https://
+58_Advanced_RAG_with_graph_path_traversal.ipynb) | | [Advanced RAG with guided
+generation](https://github.com/neuml/txtai/blob/master/examples/
+60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided
+Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/
+examples/60_Advanced_RAG_with_guided_generation.ipynb) | ### Language Model
+Workflows Language model workflows, also known as semantic workflows, connect
+language models together to build intelligent applications. ![flows](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-
 mode-only) ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/
 images/flows-dark.png#gh-dark-mode-only) While LLMs are powerful, there are
 plenty of smaller, more specialized models that work better and faster for
 specific tasks. This includes models for extractive question-answering,
 automatic summarization, text-to-speech, transcription and translation. |
 Notebook | Description | | |:----------|:-------------|------:| | [Run pipeline
```

### Comparing `txtai-7.0.0/setup.py` & `txtai-7.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     # Remove GitHub dark mode images
     DESCRIPTION = "".join([line for line in f if "gh-dark-mode-only" not in line])
 
 # Required dependencies
-install = ["faiss-cpu>=1.7.1.post2", "torch>=1.12.1", "transformers>=4.27.0"]
+install = ["faiss-cpu>=1.7.1.post2", "torch>=1.12.1", "transformers>=4.28.0"]
 
 # Required dependencies that are also transformers dependencies
 install += ["huggingface-hub>=0.9.0", "numpy>=1.18.4", "pyyaml>=5.3", "regex>=2022.8.17"]
 
 # Optional dependencies
 extras = {}
 
@@ -27,14 +27,15 @@
     "pylint",
 ]
 
 extras["api"] = [
     "aiohttp>=3.8.1",
     "fastapi>=0.94.0",
     "msgpack>=1.0.7",
+    "pillow>=7.1.2",
     "python-multipart>=0.0.7",
     "uvicorn>=0.12.1",
 ]
 
 extras["cloud"] = ["apache-libcloud>=3.3.1"]
 
 extras["console"] = ["rich>=12.0.1"]
@@ -47,20 +48,20 @@
 
 extras["pipeline-audio"] = ["onnx>=1.11.0", "onnxruntime>=1.11.0", "soundfile>=0.10.3.post1", "scipy>=1.4.1", "ttstokenizer>=1.0.0"]
 
 extras["pipeline-data"] = ["beautifulsoup4>=4.9.3", "nltk>=3.5", "pandas>=1.1.0", "tika>=1.24"]
 
 extras["pipeline-image"] = ["imagehash>=4.2.1", "pillow>=7.1.2", "timm>=0.4.12"]
 
-extras["pipeline-llm"] = ["litellm>=1.15.8", "llama-cpp-python>=0.2.20"]
+extras["pipeline-llm"] = ["litellm>=1.31.2", "llama-cpp-python>=0.2.20"]
 
 extras["pipeline-text"] = ["fasttext>=0.9.2", "sentencepiece>=0.1.91"]
 
 extras["pipeline-train"] = [
-    "accelerate>=0.19.0",
+    "accelerate>=0.26.0",
     "bitsandbytes>=0.42.0",
     "onnx>=1.11.0",
     "onnxmltools>=1.9.1",
     "onnxruntime>=1.11.0",
     "peft>=0.8.1",
     "skl2onnx>=1.9.1",
 ]
@@ -103,15 +104,15 @@
     + extras["pipeline"]
     + extras["similarity"]
     + extras["workflow"]
 )
 
 setup(
     name="txtai",
-    version="7.0.0",
+    version="7.1.0",
     author="NeuML",
     description="All-in-one open-source embeddings database for semantic search, LLM orchestration and language model workflows",
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/neuml/txtai",
     project_urls={
         "Documentation": "https://github.com/neuml/txtai",
```

### Comparing `txtai-7.0.0/src/python/txtai/ann/annoy.py` & `txtai-7.1.0/src/python/txtai/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/ann/base.py` & `txtai-7.1.0/src/python/txtai/ann/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/ann/factory.py` & `txtai-7.1.0/src/python/txtai/ann/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/ann/faiss.py` & `txtai-7.1.0/src/python/txtai/ann/faiss.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/ann/hnsw.py` & `txtai-7.1.0/src/python/txtai/ann/hnsw.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/ann/numpy.py` & `txtai-7.1.0/src/python/txtai/ann/numpy.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/ann/torch.py` & `txtai-7.1.0/src/python/txtai/ann/torch.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/application.py` & `txtai-7.1.0/src/python/txtai/api/application.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/authorization.py` & `txtai-7.1.0/src/python/txtai/api/authorization.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/base.py` & `txtai-7.1.0/src/python/txtai/api/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/cluster.py` & `txtai-7.1.0/src/python/txtai/api/cluster.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/factory.py` & `txtai-7.1.0/src/python/txtai/api/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/responses/factory.py` & `txtai-7.1.0/src/python/txtai/api/responses/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/responses/json.py` & `txtai-7.1.0/src/python/txtai/api/responses/json.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/responses/messagepack.py` & `txtai-7.1.0/src/python/txtai/api/responses/messagepack.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/route.py` & `txtai-7.1.0/src/python/txtai/api/route.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/caption.py` & `txtai-7.1.0/src/python/txtai/api/routers/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/embeddings.py` & `txtai-7.1.0/src/python/txtai/api/routers/embeddings.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/entity.py` & `txtai-7.1.0/src/python/txtai/api/routers/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/extractor.py` & `txtai-7.1.0/src/python/txtai/api/routers/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/labels.py` & `txtai-7.1.0/src/python/txtai/api/routers/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/objects.py` & `txtai-7.1.0/src/python/txtai/api/routers/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/segmentation.py` & `txtai-7.1.0/src/python/txtai/api/routers/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/similarity.py` & `txtai-7.1.0/src/python/txtai/api/routers/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/summary.py` & `txtai-7.1.0/src/python/txtai/api/routers/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/tabular.py` & `txtai-7.1.0/src/python/txtai/api/routers/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/textractor.py` & `txtai-7.1.0/src/python/txtai/api/routers/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/transcription.py` & `txtai-7.1.0/src/python/txtai/api/routers/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/translation.py` & `txtai-7.1.0/src/python/txtai/api/routers/translation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/api/routers/workflow.py` & `txtai-7.1.0/src/python/txtai/api/routers/workflow.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/app/base.py` & `txtai-7.1.0/src/python/txtai/app/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/archive/base.py` & `txtai-7.1.0/src/python/txtai/archive/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/archive/compress.py` & `txtai-7.1.0/src/python/txtai/archive/compress.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/archive/tar.py` & `txtai-7.1.0/src/python/txtai/archive/tar.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/archive/zip.py` & `txtai-7.1.0/src/python/txtai/archive/zip.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/cloud/base.py` & `txtai-7.1.0/src/python/txtai/cloud/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/cloud/factory.py` & `txtai-7.1.0/src/python/txtai/cloud/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/cloud/hub.py` & `txtai-7.1.0/src/python/txtai/cloud/hub.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/cloud/storage.py` & `txtai-7.1.0/src/python/txtai/cloud/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,18 +45,15 @@
         # Get driver for provider
         driver = get_driver(config["provider"])
 
         # Get client connection
         self.client = driver(
             config.get("key", os.environ.get("ACCESS_KEY")),
             config.get("secret", os.environ.get("ACCESS_SECRET")),
-            host=config.get("host"),
-            port=config.get("port"),
-            token=config.get("token"),
-            region=config.get("region"),
+            **{field: config.get(field) for field in ["host", "port", "region", "token"] if config.get(field)},
         )
 
     def metadata(self, path=None):
         try:
             # If this is an archive path, check if file exists
             if self.isarchive(path):
                 return self.client.get_object(self.config["container"], self.objectname(path))
```

### Comparing `txtai-7.0.0/src/python/txtai/console/base.py` & `txtai-7.1.0/src/python/txtai/console/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/data/base.py` & `txtai-7.1.0/src/python/txtai/data/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/data/labels.py` & `txtai-7.1.0/src/python/txtai/data/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/data/questions.py` & `txtai-7.1.0/src/python/txtai/data/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/data/sequences.py` & `txtai-7.1.0/src/python/txtai/data/sequences.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/data/texts.py` & `txtai-7.1.0/src/python/txtai/data/texts.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/data/tokens.py` & `txtai-7.1.0/src/python/txtai/data/tokens.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/base.py` & `txtai-7.1.0/src/python/txtai/database/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/client.py` & `txtai-7.1.0/src/python/txtai/database/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         d = aliased(Document, name="d")
 
         # Build JSON column expression for column
         return str(cast(d.data[name].as_string(), Text).compile(dialect=self.connection.bind.dialect, compile_kwargs={"literal_binds": True}))
 
     def createtables(self):
         # Create tables
-        Base.metadata.create_all(self.connection.bind)
+        Base.metadata.create_all(self.connection.bind, checkfirst=True)
 
         # Clear existing data - table schema is created upon connecting to database
         for table in ["sections", "documents", "objects"]:
             self.cursor.execute(f"DELETE FROM {table}")
 
     def finalize(self):
         # Flush cached objects
@@ -124,15 +124,15 @@
 
     def addfunctions(self):
         return
 
 
 class Cursor:
     """
-    Implements basic compatability with the Python DB-API.
+    Implements basic compatibility with the Python DB-API.
     """
 
     def __init__(self, connection):
         self.connection = connection
         self.result = None
 
     def __iter__(self):
```

### Comparing `txtai-7.0.0/src/python/txtai/database/duckdb.py` & `txtai-7.1.0/src/python/txtai/database/duckdb.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/embedded.py` & `txtai-7.1.0/src/python/txtai/database/embedded.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,21 +39,17 @@
             # Copy data from current to new
             connection = self.copy(path)
 
             # Close temporary database
             self.connection.close()
 
             # Point connection to new connection
-            self.connection = connection
-            self.cursor = self.getcursor()
+            self.session(connection=connection)
             self.path = path
 
-            # Register custom functions
-            self.addfunctions()
-
         # Paths are equal, commit changes
         elif self.path == path:
             self.connection.commit()
 
         # New path is different from current path, copy data and continue using current connection
         else:
             self.copy(path).close()
```

### Comparing `txtai-7.0.0/src/python/txtai/database/encoder/base.py` & `txtai-7.1.0/src/python/txtai/database/encoder/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/encoder/factory.py` & `txtai-7.1.0/src/python/txtai/database/encoder/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/encoder/image.py` & `txtai-7.1.0/src/python/txtai/database/encoder/image.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/factory.py` & `txtai-7.1.0/src/python/txtai/database/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/rdbms.py` & `txtai-7.1.0/src/python/txtai/database/rdbms.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,15 @@
 
         # Database connection
         self.connection = None
         self.cursor = None
 
     def load(self, path):
         # Load an existing database. Thread locking must be handled externally.
-        self.connection = self.connect(path)
-        self.cursor = self.getcursor()
-
-        # Register custom functions
-        self.addfunctions()
+        self.session(path)
 
     def insert(self, documents, index=0):
         # Initialize connection if not open
         self.initialize()
 
         # Get entry date
         entry = datetime.datetime.now()
@@ -246,23 +242,39 @@
     def initialize(self):
         """
         Creates connection and initial database schema if no connection exists.
         """
 
         if not self.connection:
             # Create temporary database. Thread locking must be handled externally.
-            self.connection = self.connect()
-            self.cursor = self.getcursor()
-
-            # Register custom functions
-            self.addfunctions()
+            self.session()
 
             # Create initial table schema
             self.createtables()
 
+    def session(self, path=None, connection=None):
+        """
+        Starts a new database session.
+
+        Args:
+            path: path to database file
+            connection: existing connection to use
+        """
+
+        # Create database connection and cursor
+        self.connection = connection if connection else self.connect(path) if path else self.connect()
+        self.cursor = self.getcursor()
+
+        # Register custom functions - session scope
+        self.addfunctions()
+
+        # Create temporary tables - session scope
+        self.createbatch()
+        self.createscores()
+
     def createtables(self):
         """
         Creates the initial table schema.
         """
 
         self.cursor.execute(Statement.CREATE_DOCUMENTS)
         self.cursor.execute(Statement.CREATE_OBJECTS)
@@ -408,17 +420,14 @@
 
         Args:
             indexids: list of indexids
             ids: list of ids
             batch: batch index, used when statement has multiple subselects
         """
 
-        # Create or replace batch table
-        self.createbatch()
-
         # Delete batch when batch id is empty or for batch 0
         if not batch:
             self.cursor.execute(Statement.DELETE_BATCH)
 
         # Add batch
         self.insertbatch(indexids, ids, batch)
 
@@ -444,17 +453,14 @@
         """
         Loads a batch of similarity scores to a temporary table for efficient query processing.
 
         Args:
             similarity: similarity results as [(indexid, score)]
         """
 
-        # Create or replace scores table
-        self.createscores()
-
         # Delete scores
         self.cursor.execute(Statement.DELETE_SCORES)
 
         if similarity:
             # Average scores per id, needed for multiple similar() clauses
             scores = {}
             for s in similarity:
```

### Comparing `txtai-7.0.0/src/python/txtai/database/schema/orm.py` & `txtai-7.1.0/src/python/txtai/database/schema/orm.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/schema/statement.py` & `txtai-7.1.0/src/python/txtai/database/schema/statement.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/sql/aggregate.py` & `txtai-7.1.0/src/python/txtai/database/sql/aggregate.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/sql/base.py` & `txtai-7.1.0/src/python/txtai/database/sql/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/sql/expression.py` & `txtai-7.1.0/src/python/txtai/database/sql/expression.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/sql/token.py` & `txtai-7.1.0/src/python/txtai/database/sql/token.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/database/sqlite.py` & `txtai-7.1.0/src/python/txtai/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/base.py` & `txtai-7.1.0/src/python/txtai/embeddings/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,21 @@
 
         # Merge configuration into single dictionary
         config = {**config, **kwargs} if config and kwargs else kwargs if kwargs else config
 
         # Set initial configuration
         self.configure(config)
 
+    def __del__(self):
+        """
+        Clean resources when embeddings is deleted.
+        """
+
+        self.close()
+
     def score(self, documents):
         """
         Builds a term weighting scoring index. Only used by word vectors models.
 
         Args:
             documents: iterable of (id, data, tags), (id, data) or data
         """
@@ -144,15 +151,15 @@
 
         # Index subindexes, if necessary
         if self.indexes:
             self.indexes.index()
 
         # Index graph, if necessary
         if self.graph:
-            self.graph.index(Search(self, True), Ids(self), self.batchsimilarity)
+            self.graph.index(Search(self, indexonly=True), Ids(self), self.batchsimilarity)
 
     def upsert(self, documents):
         """
         Runs an embeddings upsert operation. If the index exists, new data is
         appended to the index, existing data is updated. If the index doesn't exist,
         this method runs a standard index operation.
 
@@ -191,15 +198,15 @@
 
         # Subindexes upsert, if necessary
         if self.indexes:
             self.indexes.upsert()
 
         # Graph upsert, if necessary
         if self.graph:
-            self.graph.upsert(Search(self, True), Ids(self), self.batchsimilarity)
+            self.graph.upsert(Search(self, indexonly=True), Ids(self), self.batchsimilarity)
 
     def delete(self, ids):
         """
         Deletes from an embeddings index. Returns list of ids deleted.
 
         Args:
             ids: list of ids to delete
@@ -311,15 +318,15 @@
             embeddings vectors
         """
 
         # Initialize default parameters, if necessary
         self.defaults()
 
         # Default vector model, if necessary
-        model = self.model if self.model else next(iter(self.models.values()))
+        model = self.model if self.model else self.indexes.model()
 
         # Convert documents into sentence embeddings
         embeddings = model.batchtransform(Stream(self)(documents), category)
 
         # Reduce the dimensionality of the embeddings. Scale the embeddings using this
         # model to reduce the noise of common but less relevant terms.
         if self.reducer:
@@ -388,15 +395,15 @@
             list of graph per query when graph is set to True
         """
 
         # Determine if graphs should be returned
         graph = graph if self.graph else False
 
         # Execute search
-        results = Search(self, graph)(queries, limit, weights, index, parameters)
+        results = Search(self, indexids=graph)(queries, limit, weights, index, parameters)
 
         # Create subgraphs using results, if necessary
         return [self.graph.filter(x) for x in results] if graph else results
 
     def similarity(self, query, data):
         """
         Computes the similarity between query and list of data. Returns a list of
@@ -873,27 +880,16 @@
             vector model
         """
 
         # Create model cache if subindexes are enabled
         if "indexes" in self.config and self.models is None:
             self.models = {}
 
-        # Model path
-        path = self.config.get("path")
-
-        # Check if model is cached
-        if self.models and path in self.models:
-            return self.models[path]
-
-        # Load and store uncached model
-        model = VectorsFactory.create(self.config, self.scoring)
-        if self.models is not None and path:
-            self.models[path] = model
-
-        return model
+        # Load vector model
+        return VectorsFactory.create(self.config, self.scoring, self.models)
 
     def loadquery(self):
         """
         Loads a query model set in config.
 
         Returns:
             query model
```

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/autoid.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/autoid.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/documents.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/documents.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/functions.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/functions.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/indexes.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/indexes.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def __init__(self, embeddings, indexes):
         """
         Creates a new indexes instance.
 
         Args:
             embeddings: embeddings instance
-            indexes: list of subindexes to add
+            indexes: dict of subindexes to add
         """
 
         self.embeddings = embeddings
         self.indexes = indexes
 
         self.documents = None
 
@@ -79,14 +79,26 @@
 
         Returns:
             default index
         """
 
         return list(self.indexes.keys())[0]
 
+    def model(self):
+        """
+        Scans indexes and gets the first vector model.
+
+        Returns:
+            Vectors
+        """
+
+        # Return first vector model
+        matches = [index.model for index in self.indexes.values() if index.model]
+        return matches[0] if matches else None
+
     def insert(self, documents, index=None):
         """
         Inserts a batch of documents into each subindex.
 
         Args:
             documents: list of (id, data, tags)
             index: indexid offset
```

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/indexids.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/indexids.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/reducer.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/reducer.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/stream.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/stream.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/index/transform.py` & `txtai-7.1.0/src/python/txtai/embeddings/index/transform.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/search/base.py` & `txtai-7.1.0/src/python/txtai/embeddings/search/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 
 
 class Search:
     """
     Executes a batch search action. A search can be both index and/or database driven.
     """
 
-    def __init__(self, embeddings, indexids=False):
+    def __init__(self, embeddings, indexids=False, indexonly=False):
         """
         Creates a new search action.
 
         Args:
             embeddings: embeddings instance
             indexids: searches return indexids when True, otherwise run standard search
+            indexonly: always runs an index search even when a database is available
         """
 
         self.embeddings = embeddings
-        self.indexids = indexids
+        self.indexids = indexids or indexonly
+        self.indexonly = indexonly
 
         # Alias embeddings attributes
         self.ann = embeddings.ann
         self.batchtransform = embeddings.batchtransform
         self.database = embeddings.database
         self.ids = embeddings.ids
         self.indexes = embeddings.indexes
@@ -62,15 +64,15 @@
             return [[]] * len(queries)
 
         # Default index name if only subindexes set
         if not index and not self.ann and not self.scoring and self.indexes:
             index = self.indexes.default()
 
         # Database search
-        if self.database:
+        if not self.indexonly and self.database:
             return self.dbsearch(queries, limit, weights, index, parameters)
 
         # Default vector index query (sparse, dense or hybrid)
         return self.search(queries, limit, weights, index)
 
     def search(self, queries, limit, weights, index):
         """
```

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/search/explain.py` & `txtai-7.1.0/src/python/txtai/embeddings/search/explain.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/search/ids.py` & `txtai-7.1.0/src/python/txtai/embeddings/search/ids.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/search/query.py` & `txtai-7.1.0/src/python/txtai/embeddings/search/query.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/search/scan.py` & `txtai-7.1.0/src/python/txtai/embeddings/search/scan.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/embeddings/search/terms.py` & `txtai-7.1.0/src/python/txtai/embeddings/search/terms.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/graph/base.py` & `txtai-7.1.0/src/python/txtai/graph/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,24 @@
         Args:
             node: node id
             attrs: node attributes
         """
 
         raise NotImplementedError
 
+    def addnodes(self, nodes):
+        """
+        Adds nodes to the graph.
+
+        Args:
+            nodes: list of (node, attributes) to add
+        """
+
+        raise NotImplementedError
+
     def removenode(self, node):
         """
         Removes a node and all it's edges from graph.
 
         Args:
             node: node id
         """
@@ -196,14 +206,24 @@
         Args:
             source: node 1 id
             target: node 2 id
         """
 
         raise NotImplementedError
 
+    def addedges(self, edges):
+        """
+        Adds an edge to graph.
+
+        Args:
+            edges: list of (source, target, attributes) to add
+        """
+
+        raise NotImplementedError
+
     def hasedge(self, source, target=None):
         """
         Returns True if edge found, False otherwise. If target is None, this method
         returns True if any edge is found.
 
         Args:
             source: node 1 id
@@ -405,14 +425,15 @@
             documents: list of (id, data, tags)
             index: indexid offset, used for node ids
         """
 
         # Initialize graph backend
         self.initialize()
 
+        nodes = []
         for uid, document, _ in documents:
             # Relationships are manually-provided edges
             relations = None
 
             # Extract data from dictionary
             if isinstance(document, dict):
                 # Extract relationships
@@ -423,21 +444,23 @@
 
             if document is not None:
                 if isinstance(document, list):
                     # Join tokens as text
                     document = " ".join(document)
 
                 # Create node
-                self.addnode(index, id=uid, data=document)
+                nodes.append((index, {"id": uid, "data": document}))
 
                 # Add relationships
                 self.addrelations(index, relations)
 
                 index += 1
 
+        self.addnodes(nodes)
+
     def delete(self, ids):
         """
         Deletes ids from graph.
 
         Args:
             ids: node ids to delete
         """
@@ -467,16 +490,16 @@
             ids: ids function - internal id resolver
             similarity: batch similarity function - takes a list of text and labels and returns best matches
         """
 
         # Add relationship edges
         self.resolverelations(ids)
 
-        # Add node edges
-        self.addedges(self.scan(), search)
+        # Infer node edges using search function
+        self.inferedges(self.scan(), search)
 
         # Label categories/topics
         if "topics" in self.config:
             self.addtopics(similarity)
 
     def upsert(self, search, ids, similarity=None):
         """
@@ -490,39 +513,40 @@
 
         # Detect if topics processing is enabled
         hastopics = "topics" in self.config
 
         # Add relationship edges
         self.resolverelations(ids)
 
-        # Add node edges using new/updated nodes, set updated flag for topic processing, if necessary
-        self.addedges(self.scan(attribute="data"), search, {"updated": True} if hastopics else None)
+        # Infer node edges using new/updated nodes, set updated flag for topic processing, if necessary
+        self.inferedges(self.scan(attribute="data"), search, {"updated": True} if hastopics else None)
 
         # Infer topics with topics of connected nodes
         if hastopics:
             # Infer topics if there is at least one topic, otherwise rebuild
             if self.topics:
                 self.infertopics()
             else:
                 self.addtopics(similarity)
 
-    def filter(self, nodes):
+    def filter(self, nodes, graph=None):
         """
         Creates a subgraph of this graph using the list of input nodes. This method creates a new graph
         selecting only matching nodes, edges, topics and categories.
 
         Args:
             nodes: nodes to select as a list of ids or list of (id, score) tuples
+            graph: optional graph used to store filtered results
 
         Returns:
             graph
         """
 
-        # Create a new empty graph of the same type
-        graph = type(self)(self.config)
+        # Set graph if available, otherwise create a new empty graph of the same type
+        graph = graph if graph else type(self)(self.config)
 
         # Initalize subgraph
         graph.initialize()
 
         nodeids = {node[0] if isinstance(node, tuple) else node for node in nodes}
         for node in nodes:
             # Unpack node and score, if available
@@ -583,14 +607,17 @@
         """
         Resolves ids and creates edges for manually-provided relationships.
 
         Args:
             ids: internal id resolver
         """
 
+        # Relationship edges
+        edges = []
+
         # Resolve ids and create edges for relationships
         for node, relations in self.relations.items():
             # Resolve internal ids
             iids = ids(y["id"] for y in relations)
 
             # Add each edge
             for relation in relations:
@@ -603,22 +630,25 @@
                 # Create edge for each instance of id - internal id pair
                 if targets:
                     for target in targets:
                         # Add weight, if not provided
                         relation["weight"] = relation.get("weight", 1.0)
 
                         # Add edge and all other attributes
-                        self.addedge(node, target, **relation)
+                        edges.append((node, target, relation))
+
+        # Add relationships
+        self.addedges(edges)
 
         # Clear temporary relationship storage
         self.relations = {}
 
-    def addedges(self, nodes, search, attributes=None):
+    def inferedges(self, nodes, search, attributes=None):
         """
-        Adds edges for a list of nodes using a score-based search function.
+        Infers edges for a list of nodes using a score-based search function.
 
         Args:
             nodes: list of nodes
             search: search function to use to identify edges
             attribute: dictionary of attributes to add to each node
         """
 
@@ -637,15 +667,15 @@
 
             # Add additional attributes, if specified
             if attributes:
                 for field, value in attributes.items():
                     self.addattribute(node, field, value)
 
             # Skip nodes with existing edges when building an approximate network
-            if not self.hasedge(node) or not approximate:
+            if not approximate or not self.hasedge(node):
                 batch.append((node, data))
 
             # Process batch
             if len(batch) == batchsize:
                 self.addbatch(search, batch, limit, minscore)
                 batch = []
 
@@ -660,22 +690,25 @@
         Args:
             search: search function to use to identify edges
             batch: batch to add
             limit: max edges to add per node
             minscore: min score to add node edge
         """
 
+        edges = []
         for x, result in enumerate(search([data for _, data in batch], limit)):
             # Get input node id
             x, _ = batch[x]
 
             # Add edges for each input node id and result node id pair that meets specified criteria
             for y, score in result:
-                if x != y and score > minscore and not self.hasedge(x, y):
-                    self.addedge(x, y, weight=score)
+                if str(x) != str(y) and score > minscore:
+                    edges.append((x, y, {"weight": score}))
+
+        self.addedges(edges)
 
     def addtopics(self, similarity=None):
         """
         Identifies and adds topics using community detection.
 
         Args:
             similarity: similarity function for labeling categories
```

### Comparing `txtai-7.0.0/src/python/txtai/graph/factory.py` & `txtai-7.1.0/src/python/txtai/graph/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/graph/networkx.py` & `txtai-7.1.0/src/python/txtai/graph/networkx.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,27 @@
 
         # Return all nodes
         return self.backend
 
     def node(self, node):
         return self.backend.nodes.get(node)
 
-    def hasnode(self, node):
-        return self.backend.has_node(node)
-
     def addnode(self, node, **attrs):
         self.backend.add_node(node, **attrs)
 
+    def addnodes(self, nodes):
+        self.backend.add_nodes_from(nodes)
+
     def removenode(self, node):
         if self.hasnode(node):
             self.backend.remove_node(node)
 
+    def hasnode(self, node):
+        return self.backend.has_node(node)
+
     def attribute(self, node, field):
         return self.node(node).get(field) if self.hasnode(node) else None
 
     def addattribute(self, node, field, value):
         if self.hasnode(node):
             self.node(node)[field] = value
 
@@ -77,24 +80,27 @@
     def edges(self, node):
         edges = self.backend.adj.get(node)
         if edges:
             return dict(sorted(edges.items(), key=lambda x: x[1]["weight"], reverse=True))
 
         return None
 
+    def addedge(self, source, target, **attrs):
+        self.backend.add_edge(source, target, **attrs)
+
+    def addedges(self, edges):
+        self.backend.add_edges_from(edges)
+
     def hasedge(self, source, target=None):
         if not target:
             edges = self.backend.adj.get(source)
             return len(edges) > 0 if edges else False
 
         return self.backend.has_edge(source, target)
 
-    def addedge(self, source, target, **attrs):
-        self.backend.add_edge(source, target, **attrs)
-
     def centrality(self):
         rank = nx.degree_centrality(self.backend)
         return dict(sorted(rank.items(), key=lambda x: x[1], reverse=True))
 
     def pagerank(self):
         rank = nx.pagerank(self.backend, weight="weight")
         return dict(sorted(rank.items(), key=lambda x: x[1], reverse=True))
```

### Comparing `txtai-7.0.0/src/python/txtai/graph/topics.py` & `txtai-7.1.0/src/python/txtai/graph/topics.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/models/models.py` & `txtai-7.1.0/src/python/txtai/models/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         Returns:
             name of first alternative accelerator available or None if not found
         """
 
         return next((device for device in ["xpu"] if hasattr(torch, device) and getattr(torch, device).is_available()), None)
 
     @staticmethod
-    def load(path, config=None, task="default"):
+    def load(path, config=None, task="default", modelargs=None):
         """
         Loads a machine learning model. Handles multiple model frameworks (ONNX, Transformers).
 
         Args:
             path: path to model
             config: path to model configuration
             task: task name used to lookup model type
@@ -196,16 +196,19 @@
             "default": AutoModel.from_pretrained,
             "question-answering": AutoModelForQuestionAnswering.from_pretrained,
             "summarization": AutoModelForSeq2SeqLM.from_pretrained,
             "text-classification": AutoModelForSequenceClassification.from_pretrained,
             "zero-shot-classification": AutoModelForSequenceClassification.from_pretrained,
         }
 
+        # Pass modelargs as keyword arguments
+        modelargs = modelargs if modelargs else {}
+
         # Load model for supported tasks. Return path for unsupported tasks.
-        return models[task](path) if task in models else path
+        return models[task](path, **modelargs) if task in models else path
 
     @staticmethod
     def tokenizer(path, **kwargs):
         """
         Loads a tokenizer from path.
 
         Args:
```

### Comparing `txtai-7.0.0/src/python/txtai/models/onnx.py` & `txtai-7.1.0/src/python/txtai/models/onnx.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/models/pooling/base.py` & `txtai-7.1.0/src/python/txtai/models/pooling/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 
 
 class Pooling(nn.Module):
     """
     Builds pooled vectors usings outputs from a transformers model.
     """
 
-    def __init__(self, path, device, tokenizer=None, maxlength=None):
+    def __init__(self, path, device, tokenizer=None, maxlength=None, modelargs=None):
         """
         Creates a new Pooling model.
 
         Args:
             path: path to model, accepts Hugging Face model hub id or local path
             device: tensor device id
             tokenizer: optional path to tokenizer
             maxlength: max sequence length
+            modelargs: additional model arguments
         """
 
         super().__init__()
 
-        self.model = Models.load(path)
+        self.model = Models.load(path, modelargs=modelargs)
         self.tokenizer = Models.tokenizer(tokenizer if tokenizer else path)
         self.device = Models.device(device)
 
         # Detect unbounded tokenizer typically found in older models
         Models.checklength(self.model, self.tokenizer)
 
         # Set max length
```

### Comparing `txtai-7.0.0/src/python/txtai/models/pooling/cls.py` & `txtai-7.1.0/src/python/txtai/models/pooling/cls.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/models/pooling/factory.py` & `txtai-7.1.0/src/python/txtai/models/pooling/factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,29 +28,30 @@
 
         Returns:
             Pooling
         """
 
         # Unpack parameters
         path, device, tokenizer, method = config["path"], config["device"], config.get("tokenizer"), config.get("method")
+        modelargs = config.get("modelargs")
 
         # Default pooling returns hidden state
         if isinstance(path, bytes) or (isinstance(path, str) and os.path.isfile(path)) or method == "pooling":
-            return Pooling(path, device=device, tokenizer=tokenizer)
+            return Pooling(path, device=device, tokenizer=tokenizer, modelargs=modelargs)
 
         # Derive pooling method if it's not specified, path is a string and path is not a local path
         if (not method or method not in ("clspooling", "meanpooling")) and (isinstance(path, str) and not os.path.exists(path)):
             method = PoolingFactory.method(path)
 
         # Check for cls pooling
         if method == "clspooling":
-            return ClsPooling(path, device, tokenizer)
+            return ClsPooling(path, device, tokenizer, modelargs=modelargs)
 
         # Default to mean pooling
-        return MeanPooling(path, device, tokenizer)
+        return MeanPooling(path, device, tokenizer, modelargs=modelargs)
 
     @staticmethod
     def method(path):
         """
         Determines the pooling method using the sentence transformers pooling config.
 
         Args:
```

### Comparing `txtai-7.0.0/src/python/txtai/models/pooling/mean.py` & `txtai-7.1.0/src/python/txtai/models/pooling/mean.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/models/registry.py` & `txtai-7.1.0/src/python/txtai/models/registry.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/models/tokendetection.py` & `txtai-7.1.0/src/python/txtai/models/tokendetection.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/audio/texttospeech.py` & `txtai-7.1.0/src/python/txtai/pipeline/audio/texttospeech.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/audio/transcription.py` & `txtai-7.1.0/src/python/txtai/pipeline/audio/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/base.py` & `txtai-7.1.0/src/python/txtai/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/data/segmentation.py` & `txtai-7.1.0/src/python/txtai/pipeline/data/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/data/tabular.py` & `txtai-7.1.0/src/python/txtai/pipeline/data/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/data/textractor.py` & `txtai-7.1.0/src/python/txtai/pipeline/data/textractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             node: input node
             nodes: input node's children
 
         Returns:
             True if this is a container element, False otherwise
         """
 
-        return node.name in ("div", "body") or (children and not any(isinstance(x, NavigableString) for x in children))
+        return children and (node.name in ("div", "body") or not any(isinstance(x, NavigableString) for x in children))
 
     def children(self, node):
         """
         Gets the node children, if available.
 
         Args:
             node: input node
```

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/data/tokenizer.py` & `txtai-7.1.0/src/python/txtai/pipeline/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/factory.py` & `txtai-7.1.0/src/python/txtai/pipeline/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/hfmodel.py` & `txtai-7.1.0/src/python/txtai/pipeline/hfmodel.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/hfpipeline.py` & `txtai-7.1.0/src/python/txtai/pipeline/hfpipeline.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/image/caption.py` & `txtai-7.1.0/src/python/txtai/pipeline/image/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/image/imagehash.py` & `txtai-7.1.0/src/python/txtai/pipeline/image/imagehash.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/image/objects.py` & `txtai-7.1.0/src/python/txtai/pipeline/image/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/llm/factory.py` & `txtai-7.1.0/src/python/txtai/pipeline/llm/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/llm/generation.py` & `txtai-7.1.0/src/python/txtai/pipeline/llm/generation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/llm/huggingface.py` & `txtai-7.1.0/src/python/txtai/pipeline/llm/huggingface.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/llm/litellm.py` & `txtai-7.1.0/src/python/txtai/pipeline/llm/litellm.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/llm/llama.py` & `txtai-7.1.0/src/python/txtai/pipeline/llm/llama.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/llm/llm.py` & `txtai-7.1.0/src/python/txtai/pipeline/llm/llm.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/tensors.py` & `txtai-7.1.0/src/python/txtai/pipeline/tensors.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/crossencoder.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/crossencoder.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/entity.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/extractor.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/labels.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/questions.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/similarity.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/summary.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/text/translation.py` & `txtai-7.1.0/src/python/txtai/pipeline/text/translation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/train/hfonnx.py` & `txtai-7.1.0/src/python/txtai/pipeline/train/hfonnx.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/train/hftrainer.py` & `txtai-7.1.0/src/python/txtai/pipeline/train/hftrainer.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/pipeline/train/mlonnx.py` & `txtai-7.1.0/src/python/txtai/pipeline/train/mlonnx.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/scoring/base.py` & `txtai-7.1.0/src/python/txtai/scoring/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/scoring/bm25.py` & `txtai-7.1.0/src/python/txtai/scoring/bm25.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/scoring/factory.py` & `txtai-7.1.0/src/python/txtai/scoring/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/scoring/sif.py` & `txtai-7.1.0/src/python/txtai/scoring/sif.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/scoring/terms.py` & `txtai-7.1.0/src/python/txtai/scoring/terms.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/util/resolver.py` & `txtai-7.1.0/src/python/txtai/util/resolver.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/vectors/base.py` & `txtai-7.1.0/src/python/txtai/vectors/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 
 
 class Vectors:
     """
     Base class for sentence embeddings/vector models. Vector models transform input content into numeric vectors.
     """
 
-    def __init__(self, config, scoring):
+    def __init__(self, config, scoring, models):
         """
         Creates a new vectors instance.
 
         Args:
             config: vector configuration
             scoring: optional scoring instance for term weighting
+            models: models cache
         """
 
         # Store parameters
         self.config = config
         self.scoring = scoring
+        self.models = models
 
         if config:
             # Detect if this is an initialized configuration
             self.initialized = "dimensions" in config
 
             # Enables optional string tokenization
             self.tokenize = config.get("tokenize")
@@ -40,19 +42,22 @@
 
             # Encode batch size - controls underlying model batch size when encoding vectors
             self.encodebatch = config.get("encodebatch", 32)
 
             # Embeddings instructions
             self.instructions = config.get("instructions")
 
+            # Truncate embeddings to this dimensionality
+            self.dimensionality = config.get("dimensionality")
+
             # Scalar quantization - supports 1-bit through 8-bit quantization
             quantize = config.get("quantize")
             self.qbits = max(min(quantize, 8), 1) if isinstance(quantize, int) and not isinstance(quantize, bool) else None
 
-    def load(self, path):
+    def loadmodel(self, path):
         """
         Loads vector model at path.
 
         Args:
             path: path to vector model
 
         Returns:
@@ -70,14 +75,36 @@
 
         Return:
             transformed data
         """
 
         raise NotImplementedError
 
+    def load(self, path):
+        """
+        Loads a model using the current configuration. This method will return previously cached models
+        if available.
+
+        Returns:
+            model
+        """
+
+        # Check if model is cached
+        if self.models and path in self.models:
+            return self.models[path]
+
+        # Create new model
+        model = self.loadmodel(path)
+
+        # Store model in cache
+        if self.models is not None and path:
+            self.models[path] = model
+
+        return model
+
     def index(self, documents, batchsize=500):
         """
         Converts a list of documents to a temporary file with embeddings arrays. Returns a tuple of document ids,
         number of dimensions and temporary file with embeddings.
 
         Args:
             documents: list of (id, data, tags)
@@ -195,37 +222,58 @@
         return data
 
     def vectorize(self, data):
         """
         Runs data vectorization, which consists of the following steps.
 
           1. Encode data into vectors using underlying model
-          2. Normalize vectors
-          3. Quantize vectors, if necessary
+          2. Truncate vectors, if necessary
+          3. Normalize vectors
+          4. Quantize vectors, if necessary
 
         Args:
             data: input data
 
         Returns:
             embeddings vectors
         """
 
         # Transform data into vectors
         embeddings = self.encode(data)
 
         if embeddings is not None:
+            # Truncate embeddings, if necessary
+            if self.dimensionality and self.dimensionality < embeddings.shape[1]:
+                embeddings = self.truncate(embeddings)
+
             # Normalize data
             self.normalize(embeddings)
 
             # Apply quantization, if necessary
             if self.qbits:
                 embeddings = self.quantize(embeddings)
 
         return embeddings
 
+    def truncate(self, embeddings):
+        """
+        Truncates embeddings to the configured dimensionality.
+
+        This is only useful for models trained to store more important information in
+        earlier dimensions such as Matryoshka Representation Learning (MRL).
+
+        Args:
+            embeddings: input embeddings
+
+        Returns:
+            truncated embeddings
+        """
+
+        return embeddings[:, : self.dimensionality]
+
     def normalize(self, embeddings):
         """
         Normalizes embeddings using L2 normalization. Operation applied directly on array.
 
         Args:
             embeddings: input embeddings
         """
```

### Comparing `txtai-7.0.0/src/python/txtai/vectors/external.py` & `txtai-7.1.0/src/python/txtai/vectors/external.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 class ExternalVectors(Vectors):
     """
     Loads pre-computed vectors. Pre-computed vectors allow integrating other vector models. They can also be used to efficiently
     test different model configurations without having to recompute vectors.
     """
 
-    def __init__(self, config, scoring):
-        super().__init__(config, scoring)
+    def __init__(self, config, scoring, models):
+        super().__init__(config, scoring, models)
 
         # Lookup and resolve transform function
         self.transform = self.resolve(config.get("transform"))
 
-    def load(self, path):
+    def loadmodel(self, path):
         return None
 
     def encode(self, data):
         # Call external transform function, if available and data not already an array
         if self.transform and data and not isinstance(data[0], np.ndarray):
             data = self.transform(data)
```

### Comparing `txtai-7.0.0/src/python/txtai/vectors/factory.py` & `txtai-7.1.0/src/python/txtai/vectors/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,43 +9,44 @@
 
 class VectorsFactory:
     """
     Methods to create Vectors models.
     """
 
     @staticmethod
-    def create(config, scoring):
+    def create(config, scoring=None, models=None):
         """
         Create a Vectors model instance.
 
         Args:
             config: vector configuration
             scoring: scoring instance
+            models: models cache
 
         Returns:
             Vectors
         """
 
         # Determine vector method
         method = VectorsFactory.method(config)
         if method == "external":
-            return ExternalVectors(config, scoring)
+            return ExternalVectors(config, scoring, models)
 
         if method == "words":
             if not WORDS:
                 # Raise error if trying to create Word Vectors without similarity extra
                 raise ImportError(
                     'Word vector models are not available - install "similarity" extra to enable. Otherwise, specify '
                     + 'method="transformers" to use transformer backed models'
                 )
 
-            return WordVectors(config, scoring)
+            return WordVectors(config, scoring, models)
 
         # Default to TransformersVectors when configuration available
-        return TransformersVectors(config, scoring) if config and "path" in config else None
+        return TransformersVectors(config, scoring, models) if config and "path" in config else None
 
     @staticmethod
     def method(config):
         """
         Get or derive the vector method.
 
         Args:
```

### Comparing `txtai-7.0.0/src/python/txtai/vectors/transformers.py` & `txtai-7.1.0/src/python/txtai/vectors/transformers.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,36 +16,44 @@
 
 
 class TransformersVectors(Vectors):
     """
     Builds sentence embeddings/vectors using the transformers library.
     """
 
-    def load(self, path):
+    def loadmodel(self, path):
         # Flag that determines if transformers or sentence-transformers should be used to build embeddings
         method = self.config.get("method")
         transformers = method != "sentence-transformers"
 
         # Tensor device id
         deviceid = Models.deviceid(self.config.get("gpu", True))
 
+        # Additional model arguments
+        modelargs = self.config.get("vectors", {})
+
         # Build embeddings with transformers (default)
         if transformers:
-            return PoolingFactory.create({"path": path, "device": deviceid, "tokenizer": self.config.get("tokenizer"), "method": method})
+            return PoolingFactory.create(
+                {"path": path, "device": deviceid, "tokenizer": self.config.get("tokenizer"), "method": method, "modelargs": modelargs}
+            )
 
         # Otherwise, use sentence-transformers library
         if not SENTENCE_TRANSFORMERS:
             raise ImportError('sentence-transformers is not available - install "similarity" extra to enable')
 
         # Build embeddings with sentence-transformers
-        return SentenceTransformer(path, device=Models.device(deviceid))
+        return SentenceTransformer(path, device=Models.device(deviceid), **modelargs)
 
     def encode(self, data):
+        # Get batch parameter name
+        param = "batch_size" if self.config.get("method") == "sentence-transformers" else "batch"
+
         # Encode data using vectors model
-        return self.model.encode(data, self.encodebatch)
+        return self.model.encode(data, **{param: self.encodebatch})
 
     def prepare(self, data, category=None):
         # Optional string tokenization
         if self.tokenize and isinstance(data, str):
             data = Tokenizer.tokenize(data)
 
         # Convert token list to string
```

### Comparing `txtai-7.0.0/src/python/txtai/vectors/words.py` & `txtai-7.1.0/src/python/txtai/vectors/words.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         config: vector configuration
         scoring: scoring instance
     """
 
     global VECTORS
 
     # Create a global embedding object using configuration and saved
-    VECTORS = WordVectors(config, scoring)
+    VECTORS = WordVectors(config, scoring, None)
 
 
 def transform(document):
     """
     Multiprocessing helper method. Transforms document into an embeddings vector.
 
     Args:
@@ -64,15 +64,15 @@
 
 
 class WordVectors(Vectors):
     """
     Builds sentence embeddings/vectors using weighted word embeddings.
     """
 
-    def load(self, path):
+    def loadmodel(self, path):
         # Ensure that vector path exists
         if not path or not os.path.isfile(path):
             raise IOError(ENOENT, "Vector model file not found", path)
 
         # Load magnitude model. If this is a training run (uninitialized config), block until vectors are fully loaded
         return Magnitude(path, case_insensitive=True, blocking=not self.initialized)
```

### Comparing `txtai-7.0.0/src/python/txtai/workflow/base.py` & `txtai-7.1.0/src/python/txtai/workflow/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/execute.py` & `txtai-7.1.0/src/python/txtai/workflow/execute.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/factory.py` & `txtai-7.1.0/src/python/txtai/workflow/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/base.py` & `txtai-7.1.0/src/python/txtai/workflow/task/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/export.py` & `txtai-7.1.0/src/python/txtai/workflow/task/export.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/factory.py` & `txtai-7.1.0/src/python/txtai/workflow/task/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/file.py` & `txtai-7.1.0/src/python/txtai/workflow/task/file.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/image.py` & `txtai-7.1.0/src/python/txtai/workflow/task/image.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/retrieve.py` & `txtai-7.1.0/src/python/txtai/workflow/task/retrieve.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/service.py` & `txtai-7.1.0/src/python/txtai/workflow/task/service.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/storage.py` & `txtai-7.1.0/src/python/txtai/workflow/task/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -100,18 +100,11 @@
         parts = container.split("/", 1)
         container, prefix = (parts[0], parts[1]) if len(parts) > 1 else (container, None)
 
         # Get driver for provider
         driver = get_driver(provider)
 
         # Get client connection
-        client = driver(
-            key,
-            secret,
-            host=self.host,
-            port=self.port,
-            token=self.token,
-            region=self.region,
-        )
+        client = driver(key, secret, **{field: getattr(self, field) for field in ["host", "port", "region", "token"] if getattr(self, field)})
 
         container = client.get_container(container_name=container)
         return [client.get_object_cdn_url(obj) for obj in client.list_container_objects(container=container, prefix=prefix)]
```

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/stream.py` & `txtai-7.1.0/src/python/txtai/workflow/task/stream.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai/workflow/task/template.py` & `txtai-7.1.0/src/python/txtai/workflow/task/template.py`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai.egg-info/PKG-INFO` & `txtai-7.1.0/src/python/txtai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 7.0.0
+Version: 7.1.0
 Summary: All-in-one open-source embeddings database for semantic search, LLM orchestration and language model workflows
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
@@ -17,15 +17,15 @@
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: faiss-cpu>=1.7.1.post2
 Requires-Dist: torch>=1.12.1
-Requires-Dist: transformers>=4.27.0
+Requires-Dist: transformers>=4.28.0
 Requires-Dist: huggingface-hub>=0.9.0
 Requires-Dist: numpy>=1.18.4
 Requires-Dist: pyyaml>=5.3
 Requires-Dist: regex>=2022.8.17
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
@@ -36,14 +36,15 @@
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Provides-Extra: api
 Requires-Dist: aiohttp>=3.8.1; extra == "api"
 Requires-Dist: fastapi>=0.94.0; extra == "api"
 Requires-Dist: msgpack>=1.0.7; extra == "api"
+Requires-Dist: pillow>=7.1.2; extra == "api"
 Requires-Dist: python-multipart>=0.0.7; extra == "api"
 Requires-Dist: uvicorn>=0.12.1; extra == "api"
 Provides-Extra: cloud
 Requires-Dist: apache-libcloud>=3.3.1; extra == "cloud"
 Provides-Extra: console
 Requires-Dist: rich>=12.0.1; extra == "console"
 Provides-Extra: database
@@ -69,21 +70,21 @@
 Requires-Dist: pandas>=1.1.0; extra == "pipeline-data"
 Requires-Dist: tika>=1.24; extra == "pipeline-data"
 Provides-Extra: pipeline-image
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline-image"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline-image"
 Requires-Dist: timm>=0.4.12; extra == "pipeline-image"
 Provides-Extra: pipeline-llm
-Requires-Dist: litellm>=1.15.8; extra == "pipeline-llm"
+Requires-Dist: litellm>=1.31.2; extra == "pipeline-llm"
 Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline-llm"
 Provides-Extra: pipeline-text
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline-text"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline-text"
 Provides-Extra: pipeline-train
-Requires-Dist: accelerate>=0.19.0; extra == "pipeline-train"
+Requires-Dist: accelerate>=0.26.0; extra == "pipeline-train"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline-train"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline-train"
 Requires-Dist: onnxmltools>=1.9.1; extra == "pipeline-train"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline-train"
 Requires-Dist: peft>=0.8.1; extra == "pipeline-train"
 Requires-Dist: skl2onnx>=1.9.1; extra == "pipeline-train"
 Provides-Extra: pipeline
@@ -95,19 +96,19 @@
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "pipeline"
 Requires-Dist: nltk>=3.5; extra == "pipeline"
 Requires-Dist: pandas>=1.1.0; extra == "pipeline"
 Requires-Dist: tika>=1.24; extra == "pipeline"
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline"
 Requires-Dist: timm>=0.4.12; extra == "pipeline"
-Requires-Dist: litellm>=1.15.8; extra == "pipeline"
+Requires-Dist: litellm>=1.31.2; extra == "pipeline"
 Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline"
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline"
-Requires-Dist: accelerate>=0.19.0; extra == "pipeline"
+Requires-Dist: accelerate>=0.26.0; extra == "pipeline"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline"
 Requires-Dist: onnxmltools>=1.9.1; extra == "pipeline"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline"
 Requires-Dist: peft>=0.8.1; extra == "pipeline"
 Requires-Dist: skl2onnx>=1.9.1; extra == "pipeline"
 Provides-Extra: similarity
@@ -125,14 +126,15 @@
 Requires-Dist: pillow>=7.1.2; extra == "workflow"
 Requires-Dist: requests>=2.26.0; extra == "workflow"
 Requires-Dist: xmltodict>=0.12.0; extra == "workflow"
 Provides-Extra: all
 Requires-Dist: aiohttp>=3.8.1; extra == "all"
 Requires-Dist: fastapi>=0.94.0; extra == "all"
 Requires-Dist: msgpack>=1.0.7; extra == "all"
+Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: python-multipart>=0.0.7; extra == "all"
 Requires-Dist: uvicorn>=0.12.1; extra == "all"
 Requires-Dist: apache-libcloud>=3.3.1; extra == "all"
 Requires-Dist: rich>=12.0.1; extra == "all"
 Requires-Dist: duckdb>=0.7.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
@@ -149,19 +151,19 @@
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "all"
 Requires-Dist: nltk>=3.5; extra == "all"
 Requires-Dist: pandas>=1.1.0; extra == "all"
 Requires-Dist: tika>=1.24; extra == "all"
 Requires-Dist: imagehash>=4.2.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: timm>=0.4.12; extra == "all"
-Requires-Dist: litellm>=1.15.8; extra == "all"
+Requires-Dist: litellm>=1.31.2; extra == "all"
 Requires-Dist: llama-cpp-python>=0.2.20; extra == "all"
 Requires-Dist: fasttext>=0.9.2; extra == "all"
 Requires-Dist: sentencepiece>=0.1.91; extra == "all"
-Requires-Dist: accelerate>=0.19.0; extra == "all"
+Requires-Dist: accelerate>=0.26.0; extra == "all"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxmltools>=1.9.1; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: peft>=0.8.1; extra == "all"
 Requires-Dist: skl2onnx>=1.9.1; extra == "all"
 Requires-Dist: annoy>=1.16.3; extra == "all"
@@ -307,16 +309,16 @@
 ![rag](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/rag.png#gh-light-mode-only)
 
 A novel feature of txtai is that it can provide both an answer and source citation.
 
 | Notebook  | Description  |       |
 |:----------|:-------------|------:|
 | [Build RAG pipelines with txtai](https://github.com/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) | Guide on retrieval augmented generation including how to create citations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) |
-| [Generate knowledge with Semantic Graphs and RAG](https://github.com/neuml/txtai/blob/master/examples/55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) | Knowledge exploration and discovery with Semantic Graphs and RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/55_Generate_knowledge_with_Semantic_Graphs_and_RAG.ipynb) |
 | [Advanced RAG with graph path traversal](https://github.com/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) | Graph path traversal to collect complex sets of data for advanced RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) |
+| [Advanced RAG with guided generation](https://github.com/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) |
 
 ### Language Model Workflows
 
 Language model workflows, also known as semantic workflows, connect language models together to build intelligent applications.
 
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
```

### Comparing `txtai-7.0.0/src/python/txtai.egg-info/SOURCES.txt` & `txtai-7.1.0/src/python/txtai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `txtai-7.0.0/src/python/txtai.egg-info/requires.txt` & `txtai-7.1.0/src/python/txtai.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 faiss-cpu>=1.7.1.post2
 torch>=1.12.1
-transformers>=4.27.0
+transformers>=4.28.0
 huggingface-hub>=0.9.0
 numpy>=1.18.4
 pyyaml>=5.3
 regex>=2022.8.17
 
 [all]
 aiohttp>=3.8.1
 fastapi>=0.94.0
 msgpack>=1.0.7
+pillow>=7.1.2
 python-multipart>=0.0.7
 uvicorn>=0.12.1
 apache-libcloud>=3.3.1
 rich>=12.0.1
 duckdb>=0.7.1
-pillow>=7.1.2
 sqlalchemy>=2.0.20
 grand-cypher>=0.6.0
 networkx>=2.6.3
 python-louvain>=0.16
 onnx>=1.11.0
 onnxruntime>=1.11.0
 soundfile>=0.10.3.post1
@@ -27,19 +27,19 @@
 ttstokenizer>=1.0.0
 beautifulsoup4>=4.9.3
 nltk>=3.5
 pandas>=1.1.0
 tika>=1.24
 imagehash>=4.2.1
 timm>=0.4.12
-litellm>=1.15.8
+litellm>=1.31.2
 llama-cpp-python>=0.2.20
 fasttext>=0.9.2
 sentencepiece>=0.1.91
-accelerate>=0.19.0
+accelerate>=0.26.0
 bitsandbytes>=0.42.0
 onnxmltools>=1.9.1
 peft>=0.8.1
 skl2onnx>=1.9.1
 annoy>=1.16.3
 hnswlib>=0.5.0
 pymagnitude-lite>=0.1.43
@@ -50,14 +50,15 @@
 requests>=2.26.0
 xmltodict>=0.12.0
 
 [api]
 aiohttp>=3.8.1
 fastapi>=0.94.0
 msgpack>=1.0.7
+pillow>=7.1.2
 python-multipart>=0.0.7
 uvicorn>=0.12.1
 
 [cloud]
 apache-libcloud>=3.3.1
 
 [console]
@@ -97,19 +98,19 @@
 beautifulsoup4>=4.9.3
 nltk>=3.5
 pandas>=1.1.0
 tika>=1.24
 imagehash>=4.2.1
 pillow>=7.1.2
 timm>=0.4.12
-litellm>=1.15.8
+litellm>=1.31.2
 llama-cpp-python>=0.2.20
 fasttext>=0.9.2
 sentencepiece>=0.1.91
-accelerate>=0.19.0
+accelerate>=0.26.0
 bitsandbytes>=0.42.0
 onnxmltools>=1.9.1
 peft>=0.8.1
 skl2onnx>=1.9.1
 
 [pipeline-audio]
 onnx>=1.11.0
@@ -126,23 +127,23 @@
 
 [pipeline-image]
 imagehash>=4.2.1
 pillow>=7.1.2
 timm>=0.4.12
 
 [pipeline-llm]
-litellm>=1.15.8
+litellm>=1.31.2
 llama-cpp-python>=0.2.20
 
 [pipeline-text]
 fasttext>=0.9.2
 sentencepiece>=0.1.91
 
 [pipeline-train]
-accelerate>=0.19.0
+accelerate>=0.26.0
 bitsandbytes>=0.42.0
 onnx>=1.11.0
 onnxmltools>=1.9.1
 onnxruntime>=1.11.0
 peft>=0.8.1
 skl2onnx>=1.9.1
```

