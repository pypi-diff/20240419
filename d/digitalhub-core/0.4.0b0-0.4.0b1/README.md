# Comparing `tmp/digitalhub_core-0.4.0b0.tar.gz` & `tmp/digitalhub_core-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_core-0.4.0b0.tar", last modified: Wed Apr 17 12:33:12 2024, max compression
+gzip compressed data, was "digitalhub_core-0.4.0b1.tar", last modified: Fri Apr 19 08:58:18 2024, max compression
```

## Comparing `digitalhub_core-0.4.0b0.tar` & `digitalhub_core-0.4.0b1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.810489 digitalhub_core-0.4.0b0/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.4.0b0/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14639 2024-04-17 12:33:12.810489 digitalhub_core-0.4.0b0/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       84 2023-11-17 11:56:29.000000 digitalhub_core-0.4.0b0/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.786489 digitalhub_core-0.4.0b0/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.790489 digitalhub_core-0.4.0b0/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2328 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.790489 digitalhub_core-0.4.0b0/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.4.0b0/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1194 2024-03-19 15:41:29.000000 digitalhub_core-0.4.0b0/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8193 2024-04-16 14:02:23.000000 digitalhub_core-0.4.0b0/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15046 2024-04-04 07:48:11.000000 digitalhub_core-0.4.0b0/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.790489 digitalhub_core-0.4.0b0/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.4.0b0/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2803 2024-03-19 15:49:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.790489 digitalhub_core-0.4.0b0/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.790489 digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3107 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2487 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1026 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1569 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.794489 digitalhub_core-0.4.0b0/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1389 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1025 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1347 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.794489 digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-04-16 14:28:24.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13389 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.794489 digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-04-16 14:28:24.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16171 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.798489 digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-04-16 14:28:24.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21771 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1894 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.798489 digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-04-16 14:28:24.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14183 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-03-22 13:57:11.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.798489 digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-04-16 14:28:24.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8250 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.798489 digitalhub_core-0.4.0b0/digitalhub_core/entities/services/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/services/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-04-16 14:28:24.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/services/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6907 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/services/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/services/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/services/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/services/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.802489 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5473 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10189 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.802489 digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6280 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15418 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.802489 digitalhub_core-0.4.0b0/digitalhub_core/registry/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/registry/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2417 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/registry/import_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1069 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/registry/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1192 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/registry/registry.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.802489 digitalhub_core-0.4.0b0/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.4.0b0/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4203 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      720 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/runtimes/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.802489 digitalhub_core-0.4.0b0/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-04-16 14:28:24.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.806489 digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-01-03 08:29:18.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-01-03 08:29:18.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-01-03 08:29:18.000000 digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.806489 digitalhub_core-0.4.0b0/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/env_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/file_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4181 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3029 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/git_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:33:12.806489 digitalhub_core-0.4.0b0/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14639 2024-04-17 12:33:12.000000 digitalhub_core-0.4.0b0/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4131 2024-04-17 12:33:12.000000 digitalhub_core-0.4.0b0/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-17 12:33:12.000000 digitalhub_core-0.4.0b0/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-04-17 12:33:12.000000 digitalhub_core-0.4.0b0/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-17 12:33:12.000000 digitalhub_core-0.4.0b0/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b0/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-17 12:33:12.810489 digitalhub_core-0.4.0b0/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.469614 digitalhub_core-0.4.0b1/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.4.0b1/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-04-19 08:58:18.469614 digitalhub_core-0.4.0b1/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-19 08:36:26.000000 digitalhub_core-0.4.0b1/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.449614 digitalhub_core-0.4.0b1/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.449614 digitalhub_core-0.4.0b1/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-19 07:53:56.000000 digitalhub_core-0.4.0b1/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.449614 digitalhub_core-0.4.0b1/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.4.0b1/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-19 08:17:10.000000 digitalhub_core-0.4.0b1/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8684 2024-04-19 08:17:10.000000 digitalhub_core-0.4.0b1/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15648 2024-04-19 08:17:10.000000 digitalhub_core-0.4.0b1/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.453614 digitalhub_core-0.4.0b1/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.4.0b1/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-19 08:17:10.000000 digitalhub_core-0.4.0b1/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.453614 digitalhub_core-0.4.0b1/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.453614 digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2982 2024-04-19 08:10:33.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-18 15:21:56.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-18 15:23:10.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.453614 digitalhub_core-0.4.0b1/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1801 2024-04-18 15:27:11.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1442 2024-04-18 15:30:16.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1755 2024-04-18 15:31:15.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.453614 digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6563 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    13509 2024-04-19 08:10:33.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.457614 digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6220 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16136 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.457614 digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8627 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    21748 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1894 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.457614 digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4819 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14144 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3620 2024-04-18 08:07:40.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2692 2024-03-20 12:21:43.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.457614 digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6082 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8227 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.461614 digitalhub_core-0.4.0b1/digitalhub_core/entities/services/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/services/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6043 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/services/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6884 2024-04-19 08:10:33.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/services/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/services/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/services/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/services/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.461614 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5472 2024-04-19 08:14:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10135 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.461614 digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6280 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    15395 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.461614 digitalhub_core-0.4.0b1/digitalhub_core/registry/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/registry/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2543 2024-04-19 08:44:21.000000 digitalhub_core-0.4.0b1/digitalhub_core/registry/import_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-18 15:04:25.000000 digitalhub_core-0.4.0b1/digitalhub_core/registry/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-18 15:09:16.000000 digitalhub_core-0.4.0b1/digitalhub_core/registry/registry.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.461614 digitalhub_core-0.4.0b1/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.4.0b1/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-18 14:08:36.000000 digitalhub_core-0.4.0b1/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1012 2024-04-18 13:55:02.000000 digitalhub_core-0.4.0b1/digitalhub_core/runtimes/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.461614 digitalhub_core-0.4.0b1/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-04-19 08:14:48.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.465614 digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.465614 digitalhub_core-0.4.0b1/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/env_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-18 15:15:32.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/git_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-17 12:32:27.000000 digitalhub_core-0.4.0b1/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:18.465614 digitalhub_core-0.4.0b1/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-04-19 08:58:18.000000 digitalhub_core-0.4.0b1/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4131 2024-04-19 08:58:18.000000 digitalhub_core-0.4.0b1/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-19 08:58:18.000000 digitalhub_core-0.4.0b1/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-04-19 08:58:18.000000 digitalhub_core-0.4.0b1/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-19 08:58:18.000000 digitalhub_core-0.4.0b1/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-04-19 08:46:19.000000 digitalhub_core-0.4.0b1/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-19 08:58:18.469614 digitalhub_core-0.4.0b1/setup.cfg
```

### Comparing `digitalhub_core-0.4.0b0/LICENSE.txt` & `digitalhub_core-0.4.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/PKG-INFO` & `digitalhub_core-0.4.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b0
+Version: 0.4.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -247,8 +247,12 @@
 Provides-Extra: docs
 Requires-Dist: Sphinx>=7; extra == "docs"
 Requires-Dist: pydata-sphinx-theme>=0.15; extra == "docs"
 Requires-Dist: numpydoc>=1.6; extra == "docs"
 
 # Digitalhub-core Library
 
-Python package to interact with the Digitalhub Core API.
+The Digitalhub-core SDK library is used to manage entities and executions in Digitalhub from Python.
+The Digitalhub-core layer is the foundational layer of the Digitalhub Data platform.
+It contains the core entities and objects (Artifacts, Projects, Secrets, Functions, Workflows, Task and Runs) and the methods to manage them.
+
+A more detailed description of the library can be found in the [official documentation](https://scc-digitalhub.github.io/docs/) of Digitalhub.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/__init__.py` & `digitalhub_core-0.4.0b1/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/client/builder.py` & `digitalhub_core-0.4.0b1/digitalhub_core/client/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     from digitalhub_core.client.objects.base import Client
 
 
 class ClientBuilder:
     """
     The client builder class.
 
-    It implements the builder pattern to create a client instance.
+    It implements the builder pattern to create a Singleton client instance.
     The client builder can be used to create a local or non-local client instance.
     """
 
     def __init__(self) -> None:
         """
         Constructor.
         """
         self._local = None
         self._dhcore = None
 
-    def build(self, local: bool = False, config: dict = None) -> Client:
+    def build(self, local: bool = False, config: dict | None = None) -> Client:
         """
         Method to create a client instance.
 
         Parameters
         ----------
         local : bool
             Whether to create a local client or not.
@@ -64,15 +64,15 @@
     -------
     Client
         The client instance.
     """
     return client_builder.build(local)
 
 
-def build_client(local: bool = False, config: dict = None) -> None:
+def build_client(local: bool = False, config: dict | None = None) -> None:
     """
     Wrapper around ClientBuilder.build.
 
     Parameters
     ----------
     local : bool
         Whether to create a local client or not.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/client/objects/base.py` & `digitalhub_core-0.4.0b1/digitalhub_core/client/objects/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
     A client handles the lifeciycle of an object during a coding session.
     It manages the creation, reading, updating and deleting of objects and comes
     into 2 subclasses: Local and DHCore.
     """
 
     @abstractmethod
-    def create_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def create_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
         Create object method.
         """
 
     @abstractmethod
     def read_object(self, api: str, **kwargs) -> dict:
         """
         Read object method.
         """
 
     @abstractmethod
-    def update_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def update_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
         Update object method.
         """
 
     @abstractmethod
     def delete_object(self, api: str, **kwargs) -> dict:
         """
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/client/objects/dhcore.py` & `digitalhub_core-0.4.0b1/digitalhub_core/client/objects/dhcore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 DHCore Client module.
 """
 from __future__ import annotations
 
 import os
 
-import requests
 from digitalhub_core.client.objects.base import Client
 from digitalhub_core.utils.exceptions import BackendError
 from pydantic import BaseModel
+from requests import request
+from requests.exceptions import RequestException, Timeout
 
 
 class AuthConfig(BaseModel):
     """Client configuration model."""
 
     user: str = None
     """Username."""
@@ -32,122 +33,136 @@
     """Basic authentication password."""
 
 
 class ClientDHCore(Client):
     """
     DHCore client.
 
-    The DHCore client is used to communicate with the Digitalhub Core backendAPI via REST.
-    At creation, the client trys to get the endpoint and authentication parameters
-    from the environment variables. In case the endpoint is not set, it raises an exception.
+    The DHCore client is used to communicate with the Digitalhub Core
+    backendAPI via REST. The client supports basic authentication and
+    OAuth2 token authentication.
+    At creation, the client tries to get the endpoint and authentication
+    parameters from the environment variables. In case the user incours
+    into an authentication/endpoint error during the client creation it
+    has the possibility to update the correct endpoint/authentication
+    parameters using the `set_dhub_env` function.
+    If the dhcore client is already initialized, this function will override
+    the configuration, otherwise it simply set the environment variables.
     """
 
-    def __init__(self, config: dict = None) -> None:
+    def __init__(self, config: dict | None = None) -> None:
         """
         Constructor.
         """
         super().__init__()
 
-        self._endpoint = None
-
-        self._auth_type = None
-        self._user = None
-        self._password = None
-        self._access_token = None
+        self._endpoint: str | None = None
+        self._auth_type: str | None = None
+        self._user: str | None = None
+        self._password: str | None = None
+        self._access_token: str | None = None
 
         self._configure(config)
 
-    def create_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def create_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
-        Create an object.
+        Create an object in DHCore.
 
         Parameters
         ----------
+        api : str
+            Create API.
         obj : dict
             The object to create.
-        api : str
-            The api to create the object with.
+        **kwargs
+            Keyword arguments to pass to the request.
 
         Returns
         -------
         dict
-            The created object.
+            Response object.
         """
         kwargs["json"] = obj
         return self._call("POST", api, **kwargs)
 
     def read_object(self, api: str, **kwargs) -> dict:
         """
-        Get an object.
+        Get an object from DHCore.
 
         Parameters
         ----------
         api : str
-            The api to get the object with.
+            Read API.
+        **kwargs
+            Keyword arguments to pass to the request.
 
         Returns
         -------
         dict
-            The object.
+            Response object.
         """
         return self._call("GET", api, **kwargs)
 
-    def update_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def update_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
-        Update an object.
+        Update an object in DHCore.
 
         Parameters
         ----------
+        api : str
+            Update API.
         obj : dict
             The object to update.
-        api : str
-            The api to update the object with.
+        **kwargs
+            Keyword arguments to pass to the request.
 
         Returns
         -------
         dict
-            The updated object.
+            Response object.
         """
         kwargs["json"] = obj
         return self._call("PUT", api, **kwargs)
 
     def delete_object(self, api: str, **kwargs) -> dict:
         """
-        Delete an object.
+        Delete an object from DHCore.
 
         Parameters
         ----------
         api : str
-            The api to delete the object with.
+            Delete API.
+        **kwargs
+            Keyword arguments to pass to the request.
 
         Returns
         -------
         dict
-            A generic dictionary.
+            Response object.
         """
         resp = self._call("DELETE", api, **kwargs)
         if isinstance(resp, bool):
             resp = {"deleted": resp}
         return resp
 
     def list_objects(self, api: str, **kwargs) -> list[dict]:
         """
-        List objects.
+        List objects from DHCore.
 
         Parameters
         ----------
         api : str
-            The api to list the objects with.
-        **kwargs : dict
-
+            List API.
+        **kwargs
+            Keyword arguments to pass to the request.
 
         Returns
         -------
         list[dict]
-            The list of objects.
+            Response objects.
         """
         if kwargs is None:
             kwargs = {}
 
         if kwargs.get("params") is None:
             kwargs["params"] = {}
 
@@ -166,102 +181,98 @@
             kwargs["params"]["page"] += 1
 
         return objects
 
     def _call(self, call_type: str, api: str, **kwargs) -> dict:
         """
         Make a call to the DHCore API.
-        Keyword arguments are passed to the session.request function.
 
         Parameters
         ----------
         call_type : str
             The type of call to make.
         api : str
             The api to call.
         **kwargs
-            Keyword arguments.
+            Keyword arguments to pass to the request.
 
         Returns
         -------
         dict
-            The response object.
+            Response object.
         """
         url = self._endpoint + api
 
         # Choose auth type
         if self._auth_type == "basic":
             kwargs["auth"] = self._user, self._password
         elif self._auth_type == "oauth2":
             kwargs["headers"] = {"Authorization": f"Bearer {self._access_token}"}
 
-        # Call
-        response = None
+        # Call the API
         try:
-            response = requests.request(call_type, url, timeout=60, **kwargs)
+            response = request(call_type, url, timeout=60, **kwargs)
             response.raise_for_status()
             return response.json()
-        except requests.exceptions.RequestException as e:
-            if isinstance(e, requests.exceptions.Timeout):
+        except RequestException as e:
+            if isinstance(e, Timeout):
                 msg = "Request to DHCore backend timed out."
-            elif isinstance(e, requests.exceptions.ConnectionError):
+            elif isinstance(e, ConnectionError):
                 msg = "Unable to connect to DHCore backend."
-            elif isinstance(e, requests.exceptions.JSONDecodeError):
-                return {}
             else:
                 msg = f"Backend error: {e}"
             raise BackendError(msg) from e
+        except Exception as e:
+            msg = f"Some error occurred: {e}"
+            raise RuntimeError(msg) from e
 
     ################################
     # Configuration methods
     ################################
 
     def _configure(self, config: dict | None = None) -> None:
         """
-        Function to set environment variables for DHub Core config.
+        Configure the client attributes with config (given or from
+        environment).
+        Regarding authentication parameters, the config parameter
+        takes precedence over the env variables, and the token
+        over the basic auth. Furthermore, the config parameter is
+        validated against the proper pydantic model.
 
         Parameters
         ----------
-        config : ClientConfig
-            The client config.
+        config : dict
+            Configuration dictionary.
 
         Returns
         -------
         None
         """
-
-        # Get endpoint at the beginning
         self._get_endpoint_from_env()
 
-        # Evaluate configuration authentication parameters
         if config is not None:
-            # Validate configuration against pydantic model
-
-            # Try to get user/access_token or user/password
-
             if config.get("access_token") is not None:
                 config = OAuth2TokenAuth(**config)
                 self._user = config.user
                 self._access_token = config.access_token
                 self._auth_type = "oauth2"
 
             elif config.get("user") is not None and config.get("password") is not None:
                 config = BasicAuth(**config)
                 self._user = config.user
                 self._password = config.password
                 self._auth_type = "basic"
 
             return
 
-        # Otherwise, use environment variables
         self._get_auth_from_env()
 
     def _get_endpoint_from_env(self) -> None:
         """
-        Get DHub Core endpoint environment variables.
+        Get the DHCore endpoint from the env.
 
         Returns
         -------
         None
 
         Raises
         ------
@@ -280,21 +291,18 @@
 
     def _get_auth_from_env(self) -> None:
         """
         Get authentication parameters from the env.
 
         Returns
         -------
-        tuple[str, str], str, None
-            The authentication parameters.
+        None
         """
-        # User for future entity ownership
         self._user = os.getenv("DIGITALHUB_CORE_USER")
 
-        # Prioritize token over user/password
         token = os.getenv("DIGITALHUB_CORE_TOKEN")
         if token is not None:
             self._auth_type = "oauth2"
             self._access_token = token
             return
 
         password = os.getenv("DIGITALHUB_CORE_PASSWORD")
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/client/objects/local.py` & `digitalhub_core-0.4.0b1/digitalhub_core/client/objects/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,22 +30,22 @@
         super().__init__()
         self._db: dict[str, dict[str, dict]] = {}
 
     ########################
     # CRUD
     ########################
 
-    def create_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def create_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
-        Create an object.
+        Create an object in local.
 
         Parameters
         ----------
         api : str
-            The api to create the object with.
+            Create API.
         obj : dict
             The object to create.
 
         Returns
         -------
         dict
             The created object.
@@ -100,25 +100,25 @@
         # If try to create already existing object
         except ValueError:
             msg = self._format_msg(2, entity_type=entity_type, entity_id=entity_id)
             raise BackendError(msg)
 
     def read_object(self, api: str, **kwargs) -> dict:
         """
-        Get an object.
+        Get an object from local.
 
         Parameters
         ----------
         api : str
-            The api to get the object with.
+            Read API.
 
         Returns
         -------
-        dict or None
-            The object, or None if it doesn't exist.
+        dict
+            The read object.
         """
         entity_type, entity_id, context_api = self._parse_api(api)
         if entity_id is None:
             msg = self._format_msg(4)
             raise BackendError(msg)
         try:
             # Base API
@@ -153,24 +153,24 @@
                 else:
                     raise KeyError
 
         except KeyError:
             msg = self._format_msg(3, entity_type=entity_type, entity_id=entity_id)
             raise BackendError(msg)
 
-    def update_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def update_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
-        Update an object.
+        Update an object in local.
 
         Parameters
         ----------
+        api : str
+            Update API.
         obj : dict
             The object to update.
-        api : str
-            The api to update the object with.
 
         Returns
         -------
         dict
             The updated object.
         """
         entity_type, entity_id, context_api = self._parse_api(api)
@@ -195,25 +195,27 @@
             msg = self._format_msg(3, entity_type=entity_type, entity_id=entity_id)
             raise BackendError(msg)
 
         return obj
 
     def delete_object(self, api: str, **kwargs) -> dict:
         """
-        Delete an object.
+        Delete an object from local.
 
         Parameters
         ----------
         api : str
-            The api to delete the object with.
+            Delete API.
+        **kwargs
+            Keyword arguments parsed from request.
 
         Returns
         -------
         dict
-            A generic dictionary.
+            Response object.
         """
         entity_type, entity_id, context_api = self._parse_api(api)
         try:
             # Base API
             #
             # DELETE /api/v1/projects/<entity_id>
 
@@ -226,14 +228,17 @@
             #
             # We do not handle cascade in local client and
             # in the sdk we selectively delete objects by id,
             # not by name nor entity_type.
 
             else:
                 reset_latest = False
+
+                # Name is optional and extracted from kwargs
+                # "params": {"name": <name>}
                 name = kwargs.get("params", {}).get("name")
 
                 # Delete by name
                 if entity_id is None and name is not None:
                     self._db[entity_type].pop(name, None)
                     return {"deleted": True}
 
@@ -257,27 +262,30 @@
                         self._db[entity_type].pop(name)
 
                     # Handle latest
                     elif reset_latest:
                         latest_uuid = None
                         latest_date = None
                         for k, v in self._db[entity_type][name].items():
-                            # Accept only ISO format
+                            # Get created from metadata. If tzinfo is None, set it to UTC
+                            # If created is not in ISO format, use fallback
                             fallback = datetime.fromtimestamp(0, timezone.utc)
                             try:
                                 current_created = datetime.fromisoformat(v.get("metadata", {}).get("created"))
                                 if current_created.tzinfo is None:
                                     current_created = current_created.replace(tzinfo=timezone.utc)
                             except ValueError:
                                 current_created = fallback
 
+                            # Update latest date and uuid
                             if latest_date is None or current_created > latest_date:
                                 latest_uuid = k
                                 latest_date = current_created
 
+                        # Set new latest
                         if latest_uuid is not None:
                             self._db[entity_type][name]["latest"] = self._db[entity_type][name][latest_uuid]
 
         except KeyError:
             msg = self._format_msg(3, entity_type=entity_type, entity_id=entity_id)
             raise BackendError(msg)
         return {"deleted": True}
@@ -285,44 +293,52 @@
     def list_objects(self, api: str, **kwargs) -> list:
         """
         List objects.
 
         Parameters
         ----------
         api : str
-            The api to list the objects with.
+            List API.
+        **kwargs
+            Keyword arguments parsed from request.
 
         Returns
         -------
         list | None
             The list of objects.
         """
         entity_type, _, _ = self._parse_api(api)
+
+        # Name is optional and extracted from kwargs
+        # "params": {"name": <name>}
         name = kwargs.get("params", {}).get("name")
         if name is not None:
             return [self._db[entity_type][name]["latest"]]
+
+        # If no name is provided, return objects by entity_type
         return [v["latest"] for _, v in self._db[entity_type].items()]
 
     ########################
     # Helpers
     ########################
 
-    def _parse_api(self, api: str) -> list[str]:
+    def _parse_api(self, api: str) -> tuple:
         """
-        Parse the given API.
+        Parse the given API to extract the entity_type, entity_id
+        and if its a context API.
 
         Parameters
         ----------
         api : str
-            The API to parse.
+            API to parse.
 
         Returns
         -------
-        list[str]
-            The parsed API elements.
+        tuple
+            Parsed elements.
         """
         # Remove prefix from API
         api = api.removeprefix("/api/v1/")
 
         # Set context flag by default to False
         context_api = False
 
@@ -339,22 +355,22 @@
         """
         Parse the elements from the given API.
         Elements returned are: entity_type, entity_id, context_api.
 
         Parameters
         ----------
         api : str
-            The parsed API.
+            Parsed API.
         context_api : bool
             True if the API is a context API.
 
         Returns
         -------
         tuple
-            The parsed elements from the API.
+            Parsed elements from the API.
         """
         # Split API path
         parsed = api.split("/")
 
         # Base API for versioned objects
 
         # POST /api/v1/<entity_type>
@@ -375,17 +391,19 @@
             return parsed[1], None, context_api
 
         # GET/DELETE/UPDATE /api/v1/-/<project>/<entity_type>/<entity_id>
         # Return entity_type, entity_id, True
         if len(parsed) == 3 and context_api:
             return parsed[1], parsed[2], context_api
 
+        raise ValueError(f"Invalid API: {api}")
+
     def _get_project_spec(self, obj: dict, name: str) -> dict:
         """
-        Read the project spec.
+        Enrich project object with spec (artifacts, functions, etc.).
 
         Parameters
         ----------
         obj : dict
             The project object.
         name : str
             The project name.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/context/builder.py` & `digitalhub_core-0.4.0b1/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/context/context.py` & `digitalhub_core-0.4.0b1/digitalhub_core/context/context.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,101 +7,104 @@
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities.projects.entity import Project
 
 
 class Context:
     """
-    Context class.
-
-    It contains the project name, client and information about the type of client.
-    It exposes CRUD operations for the entities and act as a layer between the
-    project object and the client.
-    The context is created by the context builder.
+    Context class built forom a `Project` instance. It contains
+    some information about the project, such as the project name,
+    a client instance (local or non-local), the local context
+    project path and information about client locality.
+    It exposes CRUD operations for the entities and act as a layer
+    between the project object and its client.
     """
 
     def __init__(self, project: Project) -> None:
         """
         Constructor.
-
-        Parameters
-        ----------
-        project : Project
-            The project object to create the context from.
         """
         self.name = project.name
         self.client = project._client
         self.local = project._client.is_local()
         self.project_dir = project.spec.context
 
-    def create_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def create_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
         Create an object.
 
         Parameters
         ----------
+        api : str
+            Create API.
         obj : dict
             The object to create.
-        api : str
-            The api to create the object with.
+        **kwargs
+            Keyword arguments passed to the request.
 
         Returns
         -------
         dict
-            The created object.
+            Response object.
         """
         return self.client.create_object(api, obj, **kwargs)
 
     def read_object(self, api: str, **kwargs) -> dict:
         """
-        Get an object.
+        Read an object.
 
         Parameters
         ----------
         api : str
-            The api to get the object with.
+            Read API.
+        **kwargs
+            Keyword arguments passed to the request.
 
         Returns
         -------
         dict
-            The read object.
+            Response object.
         """
         return self.client.read_object(api, **kwargs)
 
-    def update_object(self, api: str, obj: dict | None = None, **kwargs) -> dict:
+    def update_object(self, api: str, obj: dict, **kwargs) -> dict:
         """
         Update an object.
 
         Parameters
         ----------
+        api : str
+            Update API.
         obj : dict
             The object to update.
-        api : str
-            The api to update the object with.
+        **kwargs
+            Keyword arguments passed to the request.
 
         Returns
         -------
         dict
-            The updated object.
+            Response object.
         """
         return self.client.update_object(api, obj, **kwargs)
 
     def delete_object(self, api: str, **kwargs) -> dict:
         """
         Delete an object.
 
         Parameters
         ----------
         api : str
-            The api to delete the object with.
+            Delete API.
+        **kwargs
+            Keyword arguments passed to the request.
 
         Returns
         -------
         dict
-            The deleted object.
+            Response object.
         """
         return self.client.delete_object(api, **kwargs)
 
     def list_objects(self, api: str, **kwargs) -> dict:
         """
         List objects.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/base.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,32 +28,29 @@
     def _update_attributes(self, obj: dict) -> None:
         """
         Update attributes.
 
         Parameters
         ----------
         obj : dict
-            Mapping representation of object from backend.
+            Mapping representation of object.
         """
         new_obj = self.from_dict(obj, validate=False)
         self.metadata = new_obj.metadata
         self.spec = new_obj.spec
         self.status = new_obj.status
         self.user = new_obj.user
 
     @abstractmethod
     def export(self, filename: str | None = None) -> None:
         """
-        Abstract save method.
+        Abstract export method.
         """
 
-    def to_dict(
-        self,
-        include_all_non_private: bool = False,
-    ) -> dict:
+    def to_dict(self, include_all_non_private: bool = False) -> dict:
         """
         Override default to_dict method to add the possibility to exclude
         some attributes. This requires to set a list of _obj_attr
         attributes in the subclass.
 
         Parameters
         ----------
@@ -68,19 +65,15 @@
         """
         dict_ = super().to_dict()
         if include_all_non_private:
             return dict_
         return {k: v for k, v in dict_.items() if k in self._obj_attr}
 
     @classmethod
-    def from_dict(
-        cls,
-        obj: dict,
-        validate: bool = True,
-    ) -> "Entity":
+    def from_dict(cls, obj: dict, validate: bool = True) -> Entity:
         """
         Create object instance from a dictionary.
 
         Parameters
         ----------
         obj : dict
             Dictionary to create object from.
@@ -88,26 +81,20 @@
             Flag to indicate if arguments validation against a pydantic schema must be ignored.
 
         Returns
         -------
         Self
             Self instance.
         """
-        parsed_dict = cls._parse_dict(
-            obj,
-            validate=validate,
-        )
+        parsed_dict = cls._parse_dict(obj, validate=validate)
         return cls(**parsed_dict)
 
     @staticmethod
     @abstractmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Parse a dictionary to a valid entity dictionary.
         """
 
     def __repr__(self) -> str:
         """
         Return string representation of the entity object.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/metadata.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self.created_by = created_by
         self.updated_by = updated_by
         self.embedded = embedded
 
         self._any_setter(**kwargs)
 
     @classmethod
-    def from_dict(cls, obj: dict) -> "Metadata":
+    def from_dict(cls, obj: dict) -> Metadata:
         """
         Return entity metadata object from dictionary.
 
         Parameters
         ----------
         obj : dict
             A dictionary containing the attributes of the entity metadata.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/spec.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     A class representing the specification of an entity.
     Specification is a collection of information about an entity
     thought to be immutable by the user.
     """
 
     @classmethod
-    def from_dict(cls, obj: dict) -> "Spec":
+    def from_dict(cls, obj: dict) -> Spec:
         """
         Return entity specification object from dictionary.
 
         Parameters
         ----------
         obj : dict
             A dictionary containing the attributes of the entity specification.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/_base/status.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/_base/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         message : str
             Error message.
         """
         self.state = state
         self.message = message
 
     @classmethod
-    def from_dict(cls, obj: dict) -> "Status":
+    def from_dict(cls, obj: dict) -> Status:
         """
         Return entity status object from dictionary.
 
         Parameters
         ----------
         obj : dict
             A dictionary containing the attributes of the entity status.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/_builders/metadata.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/_builders/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,20 +12,28 @@
 if typing.TYPE_CHECKING:
     from digitalhub_core.entities._base.metadata import Metadata
     from digitalhub_core.registry.models import RegistryEntry
 
 
 def build_metadata(kind: str, **kwargs) -> Metadata:
     """
-    Build entity metadata object.
+    Build entity metadata object. The builder takes as input
+    the kind of metadata's object to build and the keyword
+    arguments to pass to the metadata's constructor.
+    The specific Metadata class is searched in the global
+    registry, where lies info about where to find the class.
+    The arguments are parsed, eventually adding default values,
+    and then passed to the constructor.
 
     Parameters
     ----------
     kind : str
-        The type of metadata to build.
+        Registry entry kind.
+    **kwargs
+        Keyword arguments for the constructor.
 
     Returns
     -------
     Metadata
         Metadata object.
     """
     infos: RegistryEntry = getattr(registry, kind)
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/_builders/spec.py` & `digitalhub_core-0.4.0b1/digitalhub_core/runtimes/builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
-Spec factory entity.
+Runtime builder function.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.registry.import_utils import import_class
 from digitalhub_core.registry.registry import registry
 
 if typing.TYPE_CHECKING:
-    from digitalhub_core.entities._base.spec import Spec
     from digitalhub_core.registry.models import RegistryEntry
+    from digitalhub_core.runtimes.base import Runtime
 
 
-def build_spec(kind: str, validate: bool = True, **kwargs) -> Spec:
+def build_runtime(kind: str) -> Runtime:
     """
-    Build entity spec object.
+    Build runtime object. The builder takes in input a kind.
+    This kind can derive from functions, tasks, or runs, and
+    is inserted in the global kind registry where the runtimes
+    pakages are registered.
+    The builder requires the module path where the Runtime
+    subclass is defined and the class name.
 
     Parameters
     ----------
     kind : str
-        The type of spec to build.
-    validate : bool
-        Flag to determine if arguments validation against a pydantic schema must be ignored.
+        The type of runtime to build.
 
     Returns
     -------
-    Spec
-        Spec object.
+    Runtime
+        Runtime object.
     """
     infos: RegistryEntry = getattr(registry, kind)
-    spec = import_class(infos.spec.module, infos.spec.class_name)
-    validator = import_class(infos.spec.module, infos.spec.parameters_validator)
-    if validate:
-        kwargs = validator(**kwargs).dict(by_alias=True, exclude_none=True)
-    return spec(**kwargs)
+    runtime = import_class(infos.runtime.module, infos.runtime.class_name)
+    return runtime()
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         Get artifact as file. In the case of a local store, the store returns the current
         path of the artifact. In the case of a remote store, the artifact is downloaded in
         a temporary directory.
 
         Parameters
         ----------
         target : str
-            Target path is the remote path of the artifact where it is stored
+            Target path is the remote path of the artifact where it is stored.
 
         Returns
         -------
         str
             Path of the artifact (temporary or not).
         """
         # Check if target path is provided and if it is remote
@@ -179,23 +179,28 @@
         if store.is_local():
             src = self._parameter_or_default(None, self.spec.src_path)
             self._check_local(src)
             return src
 
         return store.download(trg)
 
-    def download(self, target: str | None = None, dst: str | None = None, overwrite: bool = False) -> str:
+    def download(
+        self,
+        target: str | None = None,
+        destination: str | None = None,
+        overwrite: bool = False,
+    ) -> str:
         """
-        Download artifact from backend.
+        Download artifact from remote storage.
 
         Parameters
         ----------
         target : str
             Target path is the remote path of the artifact
-        dst : str
+        destination : str
             Destination path as filename
         overwrite : bool
             Specify if overwrite an existing file
 
         Returns
         -------
         str
@@ -203,35 +208,35 @@
         """
 
         # Check if target path is provided and if it is remote
         trg = self._parameter_or_default(target, self.spec.path)
         self._check_remote(trg)
 
         # Check if download destination path is specified and rebuild it if necessary
-        if dst is None:
+        if destination is None:
             filename = urlparse(trg).path.split("/")[-1]
-            dst = f"{self.project}/artifacts/{self.kind}/{filename}"
+            destination = f"{self.project}/artifacts/{self.kind}/{filename}"
 
         # Check if destination path exists for overwrite
-        self._check_overwrite(dst, overwrite)
+        self._check_overwrite(destination, overwrite)
 
         # Download artifact and return path
         store = get_store(trg)
-        return store.download(trg, dst)
+        return store.download(trg, destination)
 
     def upload(self, source: str | None = None, target: str | None = None) -> str:
         """
-        Upload artifact to backend.
+        Upload artifact to remote storage from source path to target destination.
 
         Parameters
         ----------
         source : str
-            Source path is the local path of the artifact
+            Source path is the local path of the artifact.
         target : str
-            Target path is the remote path of the artifact
+            Target path is the remote path of the artifact.
 
         Returns
         -------
         str
             Path of the uploaded artifact.
         """
         # Check if target path is provided and if it is remote
@@ -353,18 +358,15 @@
             raise EntityError(f"File {dst} already exists.")
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         entity : str
             Entity type.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/artifacts/spec.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,29 +163,28 @@
         self,
         action: str,
         node_selector: list[dict] | None = None,
         volumes: list[dict] | None = None,
         resources: list[dict] | None = None,
         affinity: dict | None = None,
         tolerations: list[dict] | None = None,
-        labels: list[dict] | None = None,
         env: list[dict] | None = None,
         secrets: list[str] | None = None,
         backoff_limit: int | None = None,
         schedule: str | None = None,
         replicas: int | None = None,
-        inputs: dict | None = None,
-        outputs: dict | None = None,
+        inputs: list | None = None,
+        outputs: list | None = None,
         parameters: dict | None = None,
         values: list | None = None,
         local_execution: bool = False,
         **kwargs,
     ) -> Run:
         """
-        Run function.
+        Run function. This method creates a new run and executes it.
 
         Parameters
         ----------
         action : str
             Action to execute. Task parameter.
         node_selector : list[dict]
             The node selector of the task. Task parameter.
@@ -193,29 +192,27 @@
             The volumes of the task. Task parameter.
         resources : list[dict]
             Kubernetes resources for the task. Task parameter.
         affinity : Affinity
             Kubernetes affinity parameters. Task parameter.
         tolerations : list[dict]
             Kubernetes tolerations parameters. Task parameter.
-        labels : list[dict]
-            The labels of the task.
         env : list[dict]
             The env variables of the task. Task parameter.
         secrets : list[str]
             The secrets of the task. Task parameter.
         backoff_limit : int
             The backoff limit of the task. Task parameter.
         schedule : str
             The schedule of the task. Task parameter.
         replicas : int
             The replicas of the task. Task parameter.
-        inputs : dict
+        inputs : list
             Function inputs. Run parameter.
-        outputs : dict
+        outputs : list
             Function outputs. Run parameter.
         parameters : dict
             Function parameters. Run parameter.
         values : list
             Function values. Run parameter.
         local_execution : bool
             Flag to determine if object has local execution. Run parameter.
@@ -257,15 +254,16 @@
 
         # If execution is done by DHCore backend, return the object
         if not local_execution:
             if self._context().local:
                 raise BackendError("Cannot run remote function with local backend.")
             return run
 
-        # If local execution, build and launch run
+        # If local execution, build and launch run.
+        # Detach the run from the main thread
         run.build()
         with ThreadPoolExecutor(max_workers=1) as executor:
             result = executor.submit(run.run)
         return result.result()
 
     def _check_task_in_backend(self, action: str) -> None | Task:
         """
@@ -464,18 +462,15 @@
             raise EntityError("Task does not exist.")
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         obj : dict
             Dictionary to parse.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/functions/spec.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/functions/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -703,18 +703,15 @@
         return list_secrets(self.name, **kwargs)
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         entity : str
             Entity type.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/projects/spec.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/registries.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         Kind of the object.
     uuid : str
         ID of the object in form of UUID.
     source : str
         Remote git source for object.
     labels : list[str]
         List of labels.
-    inputs : dict
+    inputs : list
         Inputs of the run.
     outputs : list
         Outputs of the run.
     parameters : dict
         Parameters of the run.
     values : list
         Values of the run.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._base.status import State
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
+from digitalhub_core.registry.registry import registry
 from digitalhub_core.runtimes.builder import build_runtime
 from digitalhub_core.utils.api import api_base_list, api_ctx_create, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 
 if typing.TYPE_CHECKING:
@@ -346,17 +347,16 @@
 
         Returns
         -------
         dict
             Executable (function or workflow) from backend.
         """
         parsed = self._parse_task_string()
-        entity_type = runtime.get_entity_type()
-        api_entity_type = "functions" if entity_type == "function" else "workflows"
-        api = api_ctx_read(self.project, api_entity_type, parsed.exec_id)
+        entity_type = registry.get_entity_type(parsed.exec_kind)
+        api = api_ctx_read(self.project, entity_type, parsed.exec_id)
         return self._context().read_object(api)
 
     def _get_task(self) -> dict:
         """
         Get object from backend. Reimplemented to avoid circular imports.
 
         Returns
@@ -399,18 +399,15 @@
         return build_runtime(exec_kind)
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         entity : str
             Entity type.
@@ -467,15 +464,15 @@
         Kind of the object.
     uuid : str
         ID of the object in form of UUID.
     source : str
         Remote git source for object.
     labels : list[str]
         List of labels.
-    inputs : dict
+    inputs : list
         Inputs of the run.
     outputs : list
         Outputs of the run.
     parameters : dict
         Parameters of the run.
     values : list
         Values of the run.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/spec.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 class RunSpec(Spec):
     """Run specification."""
 
     def __init__(
         self,
         task: str,
-        inputs: dict | None = None,
-        outputs: dict | None = None,
+        inputs: list | None = None,
+        outputs: list | None = None,
         parameters: dict | None = None,
         values: list | None = None,
         local_execution: bool = False,
     ) -> None:
         """
         Constructor.
         """
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/runs/status.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/runs/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,18 +189,15 @@
         return self._context().read_object(api, params=params)
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         obj : dict
             Dictionary to parse.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/secrets/spec.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/services/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/services/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/services/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/services/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,18 +142,15 @@
         return get_context(self.project)
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         obj : dict
             Dictionary to parse.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     labels: list[str] | None = None,
     function: str | None = "",
     node_selector: list[dict] | None = None,
     volumes: list[dict] | None = None,
     resources: list[dict] | None = None,
     affinity: dict | None = None,
     tolerations: list[dict] | None = None,
-
     env: list[dict] | None = None,
     secrets: list[str] | None = None,
     backoff_limit: int | None = None,
     schedule: str | None = None,
     replicas: int | None = None,
     **kwargs,
 ) -> Task:
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,18 +249,15 @@
         delete_run(self.project, entity_id)
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         entity : str
             Entity type.
@@ -299,15 +296,14 @@
     labels: list[str] | None = None,
     function: str | None = "",
     node_selector: list[dict] | None = None,
     volumes: list[dict] | None = None,
     resources: list[dict] | None = None,
     affinity: dict | None = None,
     tolerations: list[dict] | None = None,
-
     env: list[dict] | None = None,
     secrets: list[str] | None = None,
     backoff_limit: int | None = None,
     schedule: str | None = None,
     replicas: int | None = None,
     **kwargs,
 ) -> Task:
@@ -364,15 +360,14 @@
     )
     k8s = {
         "node_selector": node_selector,
         "volumes": volumes,
         "resources": resources,
         "affinity": affinity,
         "tolerations": tolerations,
-        "labels": k8s_labels,
         "env": env,
         "secrets": secrets,
         "backoff_limit": backoff_limit,
         "schedule": schedule,
         "replicas": replicas,
     }
     kwargs["k8s"] = k8s
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/tasks/models.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/crud.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/entities/workflows/entity.py` & `digitalhub_core-0.4.0b1/digitalhub_core/entities/workflows/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,16 @@
     def run(
         self,
         action: str = "pipeline",
         labels: list[dict] | None = None,
         env: list[dict] | None = None,
         secrets: list[str] | None = None,
         schedule: str | None = None,
-        inputs: dict | None = None,
-        outputs: dict | None = None,
+        inputs: list | None = None,
+        outputs: list | None = None,
         parameters: dict | None = None,
         values: list | None = None,
         local_execution: bool = False,
         **kwargs,
     ) -> Run:
         """
         Run workflow.
@@ -181,17 +181,17 @@
             The labels of the task.
         env : list[dict]
             The env variables of the task. Task parameter.
         secrets : list[str]
             The secrets of the task. Task parameter.
         schedule : str
             The schedule of the task. Task parameter.
-        inputs : dict
+        inputs : list
             Workflow inputs. Run parameter.
-        outputs : dict
+        outputs : list
             Workflow outputs. Run parameter.
         parameters : dict
             Workflow parameters. Run parameter.
         values : list
             Workflow values. Run parameter.
         local_execution : bool
             Flag to determine if object has local execution. Run parameter.
@@ -434,18 +434,15 @@
             raise EntityError("Task does not exist.")
 
     #############################
     #  Static interface methods
     #############################
 
     @staticmethod
-    def _parse_dict(
-        obj: dict,
-        validate: bool = True,
-    ) -> dict:
+    def _parse_dict(obj: dict, validate: bool = True) -> dict:
         """
         Get dictionary and parse it to a valid entity dictionary.
 
         Parameters
         ----------
         obj : dict
             Dictionary to parse.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/registry/import_utils.py` & `digitalhub_core-0.4.0b1/digitalhub_core/registry/import_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 import sys
 from types import ModuleType
 
 
 def import_module(package: str) -> ModuleType:
     """
-    Import modules.
+    Import modules from package name.
 
     Parameters
     ----------
     package : str
         Package name.
 
     Returns
@@ -94,14 +94,16 @@
     """
     for layer in ["core", "data", "ml", "ai"]:
         # Check if package exists
         package = f"digitalhub_{layer}"
         try:
             importlib.metadata.distribution(package)
         except importlib.metadata.PackageNotFoundError:
+            # Return because the layers are pyramidal from
+            # core to ai
             return
 
-        # Import registry module
+        # Try ot import registry from entities.registries module
         try:
             import_module(f"{package}.entities.registries")
-        except Exception as e:
-            raise e
+        except Exception:
+            pass
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/registry/models.py` & `digitalhub_core-0.4.0b1/digitalhub_core/registry/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 
 from pydantic import BaseModel
 
 
 class RuntimeEntry(BaseModel):
     """
     Model for Runtime entry.
+    It specifies the module path and the runtime class name.
     """
 
     module: str
     """Module path."""
 
     class_name: str
     """Class name."""
 
 
 class SpecEntry(BaseModel):
     """
     Model for Spec entry.
+    It specifies the module path, the spec class name
+    and the spec pydantic class validator.
     """
 
     module: str
     """Module path."""
 
     class_name: str
     """Class name."""
@@ -29,36 +32,43 @@
     parameters_validator: str
     """Class name of the parameter validator."""
 
 
 class StatusEntry(BaseModel):
     """
     Model for Status entry.
+    It specifies the module path and the status class name.
     """
 
     module: str
     """Module path."""
 
     class_name: str
     """Class name."""
 
 
 class MetadataEntry(BaseModel):
     """
     Model for Metadata entry.
+    It specifies the module path and the metadata class name.
     """
 
     module: str
     """Module path."""
 
     class_name: str
     """Class name."""
 
 
 class RegistryEntry(BaseModel):
+    """
+    Basic entry model for every entity.
+    Functions, tasks and runs specify also the runtime field.
+    """
+
     entity_type: str
     """Entity type."""
 
     spec: SpecEntry
     """Spec infos."""
 
     status: StatusEntry
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/registry/registry.py` & `digitalhub_core-0.4.0b1/digitalhub_core/registry/registry.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,23 @@
     """
 
     def register(self, entity_kind: str, entry: dict) -> None:
         """
         Register an entity kind.
 
         Parameters
+        ----------
+        entity_kind : str
+            Entity kind to be registered.
+        entry : dict
+            Entry to be registered.
+
+        Returns
+        -------
+        None
 
         """
         if hasattr(self, entity_kind):
             raise ValueError(f"Entity kind {entity_kind} already registered")
         entry = RegistryEntry(**entry)
         setattr(self, entity_kind, entry)
 
@@ -38,9 +47,28 @@
         """
         if hasattr(self, entity_kind):
             entry = RegistryEntry(**entry)
             setattr(self, entity_kind, entry)
         else:
             raise ValueError(f"Entity kind {entity_kind} not registered")
 
+    def get_entity_type(self, entity_kind: str) -> str:
+        """
+        Get entity type from kind.
+
+        Parameters
+        ----------
+        entity_kind : str
+            Entity kind.
+
+        Returns
+        -------
+        str
+            Entity type.
+        """
+        if not hasattr(self, entity_kind):
+            raise ValueError(f"Entity kind {entity_kind} not registered")
+        entry: RegistryEntry = getattr(self, entity_kind)
+        return entry.entity_type
+
 
 registry = GlobalEntityRegistry()
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/runtimes/base.py` & `digitalhub_core-0.4.0b1/digitalhub_core/runtimes/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 
 class Runtime:
     """
     Base Runtime class.
 
     Runtimes are the entities responsible for the actual execution
     of a given run. They are highly specialized components which
-    can translate the representation of a given execution as
-    expressed in the run into an actual execution operation performed
-    via libraries, code, external tools etc.
-    Runtime types match executable types.
+    can translate the representation of a given execution as expressed
+    in the run into an actual execution operation performed via
+    libraries, code, external tools etc.
     """
 
     ##################################
     # Abstract methods
     ##################################
 
     # This attribute is a list of allowed actions (tasks)
@@ -51,25 +50,17 @@
         Execute run task.
         """
 
     @staticmethod
     @abstractmethod
     def _get_executable(action: str) -> Callable:
         """
-        Get function from action.
+        Get executable from action.
         """
 
-    def get_entity_type(self) -> str:
-        """
-        Get the type of entity that the runtime is managing. Default implementation is "function".
-        Returns:
-            str: _description_
-        """
-        return "function"
-
     ##################################
     # Private methods
     ##################################
 
     def _validate_task(self, run: dict) -> str:
         """
         Check if task is allowed. This presumes that the
@@ -98,15 +89,15 @@
         """
         Get action to execute from run.
 
         The run object stores in its spec the identifier of the task
         it is associated with. The task string is derived from the
         function string, and has the following format:
 
-        <function-kind>+<task-action>://<function-name>:<function-id>
+        <function-kind>+<task-action>://<project-name>/<function-name>:<function-id>
 
         Parameters
         ----------
         run : dict
             Run object dictionary.
 
         Returns
@@ -117,17 +108,17 @@
         Raises
         ------
         RuntimeError
             If malformed run spec.
 
         Examples
         --------
-        >>> run = {"spec": {"task": dbt+transform://dbt-example-function:some-uuid4}}
+        >>> run = {"spec": {"task": fnckind+action://project/function:uuid4}}
         >>> Runtime._get_action(run)
-        'transform'
+        'action'
         """
         try:
             return run["spec"]["task"].split(":")[0].split("+")[1]
         except (KeyError, IndexError):
             msg = "Malformed run spec."
             LOGGER.exception(msg)
             raise RuntimeError(msg)
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/stores/builder.py` & `digitalhub_core-0.4.0b1/digitalhub_core/stores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/base.py` & `digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/local.py` & `digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/remote.py` & `digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/remote.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/s3.py` & `digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/s3.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/stores/objects/sql.py` & `digitalhub_core-0.4.0b1/digitalhub_core/stores/objects/sql.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/utils/api.py` & `digitalhub_core-0.4.0b1/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/utils/env_utils.py` & `digitalhub_core-0.4.0b1/digitalhub_core/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/utils/file_utils.py` & `digitalhub_core-0.4.0b1/digitalhub_core/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/utils/generic_utils.py` & `digitalhub_core-0.4.0b1/digitalhub_core/utils/generic_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import os
 from datetime import datetime
 from pathlib import Path
 from urllib.parse import urlparse
 from uuid import uuid4
 from zipfile import ZipFile
 
-import boto3
-import requests
+from boto3 import client as boto3_client
 from digitalhub_core.utils.io_utils import read_text
+from requests import get as requests_get
 
 
 def build_uuid(uuid: str | None = None) -> str:
     """
     Create a uuid if not given
 
     Parameters
@@ -141,24 +141,24 @@
     filename : Path
         Path where to save the file.
 
     Returns
     -------
     None
     """
-    with requests.get(source, stream=True) as r:
+    with requests_get(source, stream=True) as r:
         r.raise_for_status()
         with filename.open("wb") as f:
             for chunk in r.iter_content(chunk_size=8192):
                 f.write(chunk)
 
 
 def extract_archive(path: Path, filename: Path) -> None:
     """
-    Extract an archive.
+    Extract a zip archive.
 
     Parameters
     ----------
     path : Path
         Path where to extract the archive.
     filename : Path
         Path to the archive.
@@ -184,15 +184,15 @@
     filename : Path
         Path where to save the function source.
 
     Returns
     -------
     None
     """
-    s3 = boto3.client("s3", endpoint_url=os.getenv("S3_ENDPOINT_URL"))
+    s3 = boto3_client("s3", endpoint_url=os.getenv("S3_ENDPOINT_URL"))
     s3.download_file(bucket, key, filename)
 
 
 def get_bucket_and_key(path: str) -> tuple[str, str]:
     """
     Get bucket and key from path.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/utils/git_utils.py` & `digitalhub_core-0.4.0b1/digitalhub_core/utils/git_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,50 +29,32 @@
     repo = clone_from_url(url, path)
     if checkout_object != "":
         repo.git.checkout(checkout_object)
 
 
 def get_checkout_object(url: str) -> str:
     """
-    Get checkout object.
+    Get checkout object from url fragment.
 
     Parameters
     ----------
     url : str
         URL of the repository.
 
     Returns
     -------
     str
         Checkout object (branch, tag, commit).
     """
     return urlparse(url).fragment
 
 
-def checkout(repo: Repo, checkout_object: str) -> None:
-    """
-    Checkout object.
-
-    Parameters
-    ----------
-    repo : Repo
-        Repository.
-    checkout_object : str
-        Object to checkout.
-
-    Returns
-    -------
-    None
-    """
-    repo.git.checkout(checkout_object)
-
-
 def clean_path(path: Path) -> None:
     """
-    Clean path.
+    Clean path from any files.
 
     Parameters
     ----------
     path : Path
 
     Returns
     -------
@@ -80,15 +62,20 @@
     """
 
     shutil.rmtree(path, ignore_errors=True)
 
 
 def get_git_username_password_from_token(token: str) -> tuple[str, str]:
     """
-    Parse token to get username and password.
+    Parse token to get username and password. The token
+    can be one of the following:
+
+    - GitHub/GitLab personal access token (github_pat_.../glpat...)
+    - GitHub/GitLab access token
+    - Other generic token
 
     Parameters
     ----------
     token : str
         Token to parse.
 
     Returns
@@ -123,22 +110,22 @@
     url_obj = urlparse(url)
 
     # Get credentials from environment variables
     username = os.getenv("GIT_USERNAME")
     password = os.getenv("GIT_PASSWORD")
     token = os.getenv("GIT_TOKEN")
 
-    # Get credentials from token
+    # Get credentials from token. Override username and password
     if token is not None:
         username, password = get_git_username_password_from_token(token)
 
+    # Add credentials to url if needed
     if username is not None and password is not None:
         return f"https://{username}:{password}@{url_obj.hostname}{url_obj.path}"
-
-    return url
+    return f"https://{url_obj.hostname}{url_obj.path}"
 
 
 def clone_from_url(url: str, path: Path) -> Repo:
     """
     Clone repository from url. Wraps git.Repo.clone_from.
 
     Parameters
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/utils/io_utils.py` & `digitalhub_core-0.4.0b1/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core/utils/uri_utils.py` & `digitalhub_core-0.4.0b1/digitalhub_core/utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core.egg-info/PKG-INFO` & `digitalhub_core-0.4.0b1/digitalhub_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b0
+Version: 0.4.0b1
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -247,8 +247,12 @@
 Provides-Extra: docs
 Requires-Dist: Sphinx>=7; extra == "docs"
 Requires-Dist: pydata-sphinx-theme>=0.15; extra == "docs"
 Requires-Dist: numpydoc>=1.6; extra == "docs"
 
 # Digitalhub-core Library
 
-Python package to interact with the Digitalhub Core API.
+The Digitalhub-core SDK library is used to manage entities and executions in Digitalhub from Python.
+The Digitalhub-core layer is the foundational layer of the Digitalhub Data platform.
+It contains the core entities and objects (Artifacts, Projects, Secrets, Functions, Workflows, Task and Runs) and the methods to manage them.
+
+A more detailed description of the library can be found in the [official documentation](https://scc-digitalhub.github.io/docs/) of Digitalhub.
```

### Comparing `digitalhub_core-0.4.0b0/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub_core-0.4.0b1/digitalhub_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b0/pyproject.toml` & `digitalhub_core-0.4.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.4.0b0"
+version = "0.4.0b1"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -61,15 +61,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.4.0b0"
+current_version = "0.4.0b1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

