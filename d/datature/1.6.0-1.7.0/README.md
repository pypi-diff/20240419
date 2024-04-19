# Comparing `tmp/datature-1.6.0.tar.gz` & `tmp/datature-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datature-1.6.0.tar", last modified: Wed Feb  7 11:35:11 2024, max compression
+gzip compressed data, was "datature-1.7.0.tar", last modified: Fri Apr 19 10:47:26 2024, max compression
```

## Comparing `datature-1.6.0.tar` & `datature-1.7.0.tar`

### file list

```diff
@@ -1,105 +1,121 @@
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.612200 datature-1.6.0/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      414 2024-02-07 11:03:38.000000 datature-1.6.0/CHANGELOG.md
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    11357 2024-02-07 11:03:38.000000 datature-1.6.0/LICENSE
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      130 2024-02-07 11:03:38.000000 datature-1.6.0/MANIFEST.in
--rw-r--r--   0 lmd       (1000) lmd       (1000)    12347 2024-02-07 11:35:11.612200 datature-1.6.0/PKG-INFO
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    11132 2024-02-07 11:03:38.000000 datature-1.6.0/README.md
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.604200 datature-1.6.0/datature/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:03:38.000000 datature-1.6.0/datature/__init__.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.604200 datature-1.6.0/datature/nexus/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      506 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/__init__.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.604200 datature-1.6.0/datature/nexus/api/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:03:38.000000 datature-1.6.0/datature/nexus/api/__init__.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.604200 datature-1.6.0/datature/nexus/api/annotation/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:03:38.000000 datature-1.6.0/datature/nexus/api/annotation/__init__.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    22275 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/api/annotation/annotation.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    11386 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/api/annotation/import_session.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    13877 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/api/artifact.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.608200 datature-1.6.0/datature/nexus/api/asset/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:03:38.000000 datature-1.6.0/datature/nexus/api/asset/__int__.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    13876 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/api/asset/asset.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    13767 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/api/asset/upload_session.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    14221 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/api/deployment.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1980 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/api/ontology.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     6341 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/api/operation.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     9138 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/api/project.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    13516 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/api/run.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     6635 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/api/tag.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    19248 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/api/types.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     5451 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/api/workflow.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.608200 datature-1.6.0/datature/nexus/cli/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:03:38.000000 datature-1.6.0/datature/nexus/cli/__init__.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     6803 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/cli/commands.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     6250 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/cli/config.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    19464 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/cli/functions.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2840 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/cli/main.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2938 2024-02-07 11:34:55.000000 datature-1.6.0/datature/nexus/cli/messages.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     3596 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/client.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1411 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/client_context.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      666 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/config.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1238 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/error.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.608200 datature-1.6.0/datature/nexus/medical/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      716 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/medical/__init__.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      683 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/medical/base_processor.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2342 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/medical/dicom_processor.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     4176 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/medical/nii_processor.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    41952 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/models.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     6973 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/requester.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.608200 datature-1.6.0/datature/nexus/utils/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:03:38.000000 datature-1.6.0/datature/nexus/utils/__init__.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     3079 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/utils/file_signature.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     5145 2024-02-07 11:34:54.000000 datature-1.6.0/datature/nexus/utils/utils.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      343 2024-02-07 11:35:01.000000 datature-1.6.0/datature/nexus/version.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.612200 datature-1.6.0/datature.egg-info/
--rw-r--r--   0 lmd       (1000) lmd       (1000)    12347 2024-02-07 11:35:11.000000 datature-1.6.0/datature.egg-info/PKG-INFO
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2477 2024-02-07 11:35:11.000000 datature-1.6.0/datature.egg-info/SOURCES.txt
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        1 2024-02-07 11:35:11.000000 datature-1.6.0/datature.egg-info/dependency_links.txt
--rw-rw-r--   0 lmd       (1000) lmd       (1000)       58 2024-02-07 11:35:11.000000 datature-1.6.0/datature.egg-info/entry_points.txt
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      236 2024-02-07 11:35:11.000000 datature-1.6.0/datature.egg-info/requires.txt
--rw-rw-r--   0 lmd       (1000) lmd       (1000)       31 2024-02-07 11:35:11.000000 datature-1.6.0/datature.egg-info/top_level.txt
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.608200 datature-1.6.0/docs/
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.608200 datature-1.6.0/docs/source/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1244 2024-02-07 11:34:55.000000 datature-1.6.0/docs/source/conf.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1385 2024-02-07 11:03:38.000000 datature-1.6.0/docs/source/functions.rst
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      390 2024-02-07 11:03:38.000000 datature-1.6.0/docs/source/index.rst
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      111 2024-02-07 11:03:38.000000 datature-1.6.0/docs/source/msgspec.rst
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1151 2024-02-07 11:04:12.000000 datature-1.6.0/docs/source/readme.rst
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1387 2024-02-07 11:03:38.000000 datature-1.6.0/docs/source/types.rst
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2221 2024-02-07 11:34:55.000000 datature-1.6.0/docs/upload.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      235 2024-02-07 11:03:38.000000 datature-1.6.0/requirements.txt
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      131 2024-02-07 11:03:38.000000 datature-1.6.0/requirements_dev.txt
--rw-rw-r--   0 lmd       (1000) lmd       (1000)       38 2024-02-07 11:35:11.612200 datature-1.6.0/setup.cfg
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1992 2024-02-07 11:34:54.000000 datature-1.6.0/setup.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.608200 datature-1.6.0/test/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2023-06-05 11:42:53.000000 datature-1.6.0/test/__init__.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.612200 datature-1.6.0/test/api/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:03:38.000000 datature-1.6.0/test/api/__init__.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     7254 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_annotation.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)    10847 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_annotation_import_session.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     4043 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_artifact.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     4116 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_asset.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     8192 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_asset_upload_session.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1683 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_client.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     3849 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_deploy.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1303 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_ontology.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     3336 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_operation.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2296 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_project.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     4240 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_run.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     3503 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_tag.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2286 2024-02-07 11:35:01.000000 datature-1.6.0/test/api/test_workflow.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.612200 datature-1.6.0/test/fixture/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2023-06-05 11:42:53.000000 datature-1.6.0/test/fixture/__init__.py
-drwxrwxr-x   0 lmd       (1000) lmd       (1000)        0 2024-02-07 11:35:11.612200 datature-1.6.0/test/fixture/data/
--rw-rw-r--   0 lmd       (1000) lmd       (1000)        0 2023-06-05 11:42:53.000000 datature-1.6.0/test/fixture/data/__init__.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     4514 2024-02-07 11:35:00.000000 datature-1.6.0/test/fixture/data/artifact_fixture.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2654 2024-02-07 11:34:56.000000 datature-1.6.0/test/fixture/data/asset_fixture.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      806 2024-02-07 11:35:00.000000 datature-1.6.0/test/fixture/data/error_fixture.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      685 2024-02-07 11:34:56.000000 datature-1.6.0/test/fixture/data/frame_fixture.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     4942 2024-02-07 11:35:00.000000 datature-1.6.0/test/fixture/data/operation_fixture.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1215 2024-02-07 11:35:01.000000 datature-1.6.0/test/fixture/data/projects_fixture.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     1750 2024-02-07 11:35:00.000000 datature-1.6.0/test/fixture/data/upload_session_fixture.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)      599 2024-02-07 11:34:56.000000 datature-1.6.0/test/fixture/mock.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2584 2024-02-07 11:34:56.000000 datature-1.6.0/test/test_file_signature.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     3443 2024-02-07 11:34:56.000000 datature-1.6.0/test/test_medical.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     6043 2024-02-07 11:34:56.000000 datature-1.6.0/test/test_requester.py
--rw-rw-r--   0 lmd       (1000) lmd       (1000)     2299 2024-02-07 11:34:56.000000 datature-1.6.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.838978 datature-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-19 10:47:20.000000 datature-1.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 10:47:20.000000 datature-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 10:47:20.000000 datature-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-04-19 10:47:26.838978 datature-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-19 10:47:20.000000 datature-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.810978 datature-1.7.0/datature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.810978 datature-1.7.0/datature/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/api/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22046 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/annotation/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/annotation/import_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/api/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/asset/__int__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/asset/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/asset/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19098 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/api/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.814978 datature-1.7.0/datature/nexus/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/cli/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/client_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/nexus/medical/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/dicom_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/medical/nii_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41184 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/nexus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/utils/file_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 10:47:20.000000 datature-1.7.0/datature/nexus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/utils/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.818978 datature-1.7.0/datature/utils/experimental/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30527 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32462 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-19 10:47:20.000000 datature-1.7.0/datature/utils/experimental/convert/tensorrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.838978 datature-1.7.0/datature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17170 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 10:47:26.000000 datature-1.7.0/datature.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.806978 datature-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.822978 datature-1.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/msgspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-19 10:47:20.000000 datature-1.7.0/docs/source/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 10:47:20.000000 datature-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:47:26.838978 datature-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-19 10:47:20.000000 datature-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.822978 datature-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.822978 datature-1.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.826978 datature-1.7.0/tests/unit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_annotation_import_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_asset_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/api/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.826978 datature-1.7.0/tests/unit/fixture/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.826978 datature-1.7.0/tests/unit/fixture/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/artifact_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/asset_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/error_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/frame_fixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:47:26.830978 datature-1.7.0/tests/unit/fixture/data/medical/
+-rw-r--r--   0 runner    (1001) docker     (127)  1702398 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/medical/0002.DCM
+-rw-r--r--   0 runner    (1001) docker     (127)  1049988 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/medical/0015.DCM
+-rw-r--r--   0 runner    (1001) docker     (127)  4765024 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/medical/MR_Gd.nii
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/operation_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/projects_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/data/upload_session_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/fixture/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_file_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_medical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-19 10:47:20.000000 datature-1.7.0/tests/unit/test_utils.py
```

### Comparing `datature-1.6.0/LICENSE` & `datature-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datature-1.6.0/PKG-INFO` & `datature-1.7.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,195 +1,114 @@
-Metadata-Version: 2.1
-Name: datature
-Version: 1.6.0
-Summary: Python bindings for the Datature API
-Author: Raighne Weng
-Author-email: raighne@datature.io
-Project-URL: Homepage, https://www.datature.io/
-Project-URL: Documentation, https://developers.datature.io/docs/python-sdk
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.28.1
-Requires-Dist: google-crc32c==1.5.0
-Requires-Dist: pyyaml>=6.0.0
-Requires-Dist: inquirer>=2.10.1
-Requires-Dist: halo==0.0.31
-Requires-Dist: filetype==1.2.0
-Requires-Dist: opencv-python==4.7.0.72
-Requires-Dist: alive-progress==3.0.1
-Requires-Dist: pydicom>=2.3.1
-Requires-Dist: nibabel>=4.0.2
-Requires-Dist: matplotlib>=3.5.3
-Requires-Dist: numpy>=1.17.3
-Requires-Dist: Pillow>=9.5.0
-Requires-Dist: msgspec>=0.18.4
-
 <div align="center">
 
 # :hammer: Datature Python SDK :hammer:
 
 [![Python - Version](https://img.shields.io/pypi/pyversions/datature?label=Python)](https://pypi.org/project/datature)
 [![PyPI - Version](https://img.shields.io/pypi/v/datature?label=Pypi%20Package)](https://pypi.org/project/datature)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/datature?label=Pypi%20Downloads)](https://pypi.org/project/datature)
 
 [![Join Datature Slack](https://img.shields.io/badge/Join%20The%20Community-Datature%20Slack-blueviolet?style=plastic)](https://datature.io/community) [![MIT license](https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=plastic)](https://lbesson.apache-license.org/)
 
-<a href="https://datature.io">
-    <img
-      src="assets/datature.svg"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://www.datature.io/blog">
-    <img
-      src="assets/blog.svg"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://developers.datature.io/">
-    <img
-      src="https://cdn.simpleicons.org/readme/#018EF5"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://www.youtube.com/channel/UCd3UQZ9piasi0vgfg5xI59w">
-    <img
-      src="https://cdn.simpleicons.org/youtube/#FF0000"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://www.linkedin.com/company/datature/">
-    <img
-      src="https://cdn.simpleicons.org/linkedin/#0A66C2"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://twitter.com/DatatureAI">
-    <img
-      src="https://cdn.simpleicons.org/twitter/#1D9BF0"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://datature.io/community">
-    <img
-      src="assets/slack.png"
-      width="3%"
-    />
-</a>
+<a href="https://datature.io"><img src="assets/datature.svg" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://www.datature.io/blog"><img src="assets/blog.svg" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://developers.datature.io/"><img src="https://cdn.simpleicons.org/readme/#018EF5" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://www.youtube.com/channel/UCd3UQZ9piasi0vgfg5xI59w"><img src="https://cdn.simpleicons.org/youtube/#FF0000" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://www.linkedin.com/company/datature/"><img src="https://cdn.simpleicons.org/linkedin/#0A66C2" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://twitter.com/DatatureAI"><img src="https://cdn.simpleicons.org/twitter/#1D9BF0" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://datature.io/community"><img src="assets/slack.png" width="3%"/></a>
 
 ---
 
 :zap: Empower your MLOps pipelines and applications with seamless integrations :zap:
 
-Automate tasks to manage your datasets, run training experiments, export and deploy your models from [Datature Nexus](https://www.datature.io/nexus?utm_source=github) with ease. Perform development via [Python scripts](#python-usage) or with the [CLI](#cli-usage) - your choice!
+Automate tasks to manage your datasets, run training experiments, export and deploy your models from [Datature Nexus](https://www.datature.io/nexus?utm_source=github) with ease. Perform development via [Python Scripts](#python-usage) or with the [Command-Line Interface](#cli-usage).
 
 </div>
 
 ---
 
 <div align="center">
 
-## :rocket: Getting Started :rocket:
+## Getting Started
 
 </div>
 
-## :snake: Prerequisites
+## Prerequisites
 
 - `3.8` <= Python <= `3.12`
 
 We recommend users to create a virtual environment before installing any dependencies. For more information on virtual environments, please refer to:
 
 - [Python venv](https://docs.python.org/3/tutorial/venv.html)
 - [Conda](https://conda.io/projects/conda/en/stable/user-guide/install/index.html)
 - [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/)
 
-## :gear: Installation
+## Installation
 
 ```sh
 pip install --upgrade datature
 ```
 
 ---
 
 ## Python Usage
 
 For a full list of documentation and examples, please refer to the [API docs](https://developers.datature.io/docs/python-sdk).
 
 ### Authentication
 
-To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (signing up is free!). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
+To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (you can create sign up for a free account [here](https://nexus.datature.io/)). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or have been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
 
 ### Examples
 
 To list projects:
 
 ```python
 from datature import nexus
 
-client = nexus.Client("3736971xxxxx")
-
+client = nexus.Client("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117")
 projects = client.list_projects()
 ```
 
 To upload assets:
 
 ```python
 import os
 from datature import nexus
 
 logging.basicConfig()
-
-client = nexus.Client("3736971xxxxx")
-
-project = client.list_projects("proj_xxxxx")
-
+client = nexus.Client("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117")
+project = client.list_projects("proj_fca32b1bb15405d1c2bde19fd90b516d")
 
 upload_session = project.assets.create_upload_session(groups=["dataset"])
-
 with upload_session as session:
   session.add_path("/Users/dataset")
-
 print(len(upload_session))
 ```
 
 ### Logging
 
 You can vary the logging level depending on your task or use case (such as `DEBUG` to provide more insights), but the default `INFO` level is typically best suited for production use.
 
 ```python
 import logging
 
 logging.basicConfig()
-logging.getLogger("nexus").setLevel(logging.DEBUG)
+logging.getLogger("datature-nexus").setLevel(logging.DEBUG)
 ```
 
 ---
 
 ## CLI Usage
 
 For a full list of documentation and examples, please refer to the [CLI docs](https://developers.datature.io/docs/cli).
 
 ### Authentication
 
-To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (signing up is free!). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
+To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (you can create sign up for a free account [here](https://nexus.datature.io/)). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or have been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
 
 Once you have the project secret, you will now be able to make API requests using the CLI by entering the command `datature projects auth`:
 
 ```bash
 datature projects auth
 [?] Enter the project secret: ************************************************
 [?] Make [Your Project Name] the default project? (Y/n): y
@@ -201,49 +120,49 @@
 
 ### Project Management
 
 `datature projects`
 
 Show a help page of various functions to add projects, select the default project, and retrieve project information.
 
-#### Auth Project
+#### Authenticate Project
 
 `datature projects auth`
 
-Authenticate new projects using the [project secret key](https://developers.datature.io/v2.0.0/docs/hub-and-api). Multiple projects can be authenticated and stored using different secret keys.
+Authenticate new projects using the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). Multiple projects can be authenticated and stored using different secret keys.
 
 #### Select Project
 
 `datature projects select`
 
 Select an active project to work on from a list of saved projects. All subsequent CLI commands will be in the context of the selected project until a different project is selected, or the shell session is terminated.
 
 ```bash
 $ datature projects select
 
-> My Cool Project
-  New Test Project
+> Brain Tumor DICOM
+  Hand Gesture Keypoint Detection
 
-Your active project is now: [Dicom]
+Your active project is now: [Brain Tumor DICOM]
 ```
 
 #### List Projects
 
 `datature projects list`
 
 View a table of saved projects with columns containing the names of the projects, the total number of assets, the number of annotated assets, the number of annotations, and the number of tags for each project. The name of the active project is displayed at the bottom of the list.
 
 ```bash
 $ datature projects list
 
-NAME                TOTAL_ASSETS        ANNOTATED_ASSETS    ANNOTATIONS         TAGS
-My Cool Project     4071                433                 1874                3
-New Test Project    718                 53                  959                 4
+NAME                               TOTAL_ASSETS        ANNOTATED_ASSETS    ANNOTATIONS         TAGS
+Brain Tumor DICOM                  4071                433                 1874                3
+Hand Gesture Keypoint Detection    718                 53                  959                 4
 
-Your active project is now: [My Cool Project]
+Your active project is now: [Brain Tumor DICOM]
 ```
 
 ### Asset Management
 
 #### Upload Assets
 
 `datature assets upload`
@@ -268,15 +187,15 @@
 
 List asset group information within your project. You will be prompted to select an existing group or create a new group. If you select an existing group, information about the selected group will be displayed, including the total number of assets in the group, the number of assets that have been annotated, reviewed, or marked for fixes, and the number of assets that have been completed.
 
 ```bash
 $ datature assets groups
 
 > main
-  groupName2
+  validation
 
 NAME            TOTAL           ANNOTATED       REVIEW          TOFIX           COMPLETED
 main            8               1               0               0               0
 ```
 
 ### Annotation Management
 
@@ -323,17 +242,120 @@
 `datature artifacts download`
 
 Download a model artifact from [Datature Nexus](https://www.datature.io/nexus?utm_source=github). You will be prompted to enter a folder path to save the model to, and select the name and [export format](https://developers.datature.io/docs/export-formats) of the artifact to download.
 
 ```bash
 $ datature artifacts download
 [?] Enter the folder path to save model: /Volumes/
-[?] Which artifact do you want to download?: BEAF45-Workflowc
- > BEAF45-Workflowc
+[?] Which artifact do you want to download?: BEAF45-Workflow
+ > BEAF45-Workflow
 
 [?] Which model format do you want to download?: tensorflow
- > tensorflow
-   tflite
-   onnx
+ > TensorFlow
+   TFLite
+   ONNX
 
 Downloading  |████████████████████████████████████████| 100% [443421394/443421394] in 7.1s (62639992.12/s)
 ```
+
+## FAQ
+
+### How do I find my Secret Key and Project Key?
+
+We provide a step-by-step guide to finding these two crucial keys in our [Developer's Documentation](https://developers.datature.io/docs/project-keys-and-secret-keys). You can also explore the other sections under [Python SDK](https://developers.datature.io/docs/python-sdk) to learn more about the full functionality and feature set.
+
+### I'm facing some issues, what now?
+
+We're sorry to hear that, please head over to our [Issues](https://github.com/datature/datature-py/issues) page and post a detailed bug report following our guidelines, and we will address your concerns as soon as we can. Alternatively, ping us in our [Community Slack](https://datature.io/community) where our engineers will attend to your needs.
+
+### I've noticed that some features are missing, how do I contribute?
+
+Datature Python SDK is open-source and we welcome everyone to help to improve it. Please check out our [Contributing Guide](CONTRIBUTING.md) to learn how you can be a part of the team.
+
+### How do I resolve the `command not found: datature` error for the CLI?
+
+The `command not found: datature` error indicates that the Datature SDK/CLI tool is not installed properly in your system's PATH, or it has not been installed at all. To resolve this error, please follow these steps:
+
+#### Ensure Datature CLI is Installed
+
+Before anything else, verify that you've installed the Datature CLI. You can install it using pip with the following command:
+
+```bash
+pip install datature
+```
+
+If you're using a virtual environment (which is recommended), ensure that it's activated before running the installation command.
+
+#### Check Your PATH
+
+After installation, the datature command should be automatically added to your system's PATH. If it's not found, you may need to manually add the directory containing the datature executable to your PATH:
+
+```bash
+which datature
+```
+
+Or
+
+```bash
+pip show datature
+```
+
+As expected, it will show the location of the package like this:
+
+```bash
+Location: /Users/.pyenv/versions/3.8.18/lib/python3.8/site-packages
+```
+
+#### Add the Path to Your Profile
+
+Open your shell profile file with a text editor. This file could be one of ~/.bash_profile, ~/.bashrc, ~/.zshrc, etc., depending on which shell you use and the specific configuration of your operating system.
+
+For example, you can add the path using the following command:
+
+```bash
+echo 'export PATH="$PATH:/path/to/datature"' >> ~/.bash_profile
+```
+
+Replace /path/to/datature with the actual path you found with which datature or pip show datature.
+
+#### Restart Your Terminal
+
+Sometimes, changes to the PATH environment variable do not take effect until you open a new terminal session. After installation or modification of the PATH, close your current terminal and open a new one, then try the command again.
+
+### What does the warning `As the c extension couldn't be imported, google-crc32c is using a pure python implementation that is significantly slower. If possible, please configure a c build environment and compile the extension` mean, and do I need to take any action?
+
+This warning is indicating that the `google-crc32c` library is falling back to a pure Python implementation for calculating CRC32C checksums because it cannot find the C extension which is usually faster. The Python implementation is fully functional but performs slower than its C counterpart. While this won't harm the function of the library, you may experience performance issues if your application requires high-speed checksum computing.
+
+To address this warning for improved performance, you can take the following steps to compile the C extension:
+
+#### Install the Build Essentials
+
+Make sure that you have the necessary build tools installed to compile the C extension.
+
+On Ubuntu/Debian systems, you can install build-essential by running:
+
+```bash
+sudo apt-get install build-essential
+```
+
+On Red Hat/CentOS systems, you can use:
+
+```bash
+sudo yum install gcc gcc-c++ make
+```
+
+On macOS, ensure you have Xcode Command Line Tools installed:
+
+```bash
+xcode-select --install
+```
+
+#### Reinstall google-crc32c with C Extension
+
+With the build environment configured, you can attempt to reinstall the google-crc32c library which should now include the C extension:
+
+```bash
+pip install --no-cache-dir --force-reinstall google-crc32c
+```
+
+By taking these steps, you should be able to eliminate the warning by having the faster C extension compiled and used by google-crc32c.
+If speed is not critical for your use case, you can choose to ignore this warning, and the library will still function correctly, albeit with potentially decreased performance.
```

#### html2text {}

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1 Name: datature Version: 1.6.0 Summary: Python bindings
-for the Datature API Author: Raighne Weng Author-email: raighne@datature.io
-Project-URL: Homepage, https://www.datature.io/ Project-URL: Documentation,
-https://developers.datature.io/docs/python-sdk Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: requests>=2.28.1 Requires-Dist: google-crc32c==1.5.0
-Requires-Dist: pyyaml>=6.0.0 Requires-Dist: inquirer>=2.10.1 Requires-Dist:
-halo==0.0.31 Requires-Dist: filetype==1.2.0 Requires-Dist: opencv-
-python==4.7.0.72 Requires-Dist: alive-progress==3.0.1 Requires-Dist:
-pydicom>=2.3.1 Requires-Dist: nibabel>=4.0.2 Requires-Dist: matplotlib>=3.5.3
-Requires-Dist: numpy>=1.17.3 Requires-Dist: Pillow>=9.5.0 Requires-Dist:
-msgspec>=0.18.4
      # :hammer: Datature Python SDK :hammer: [![Python - Version](https://
    img.shields.io/pypi/pyversions/datature?label=Python)](https://pypi.org/
       project/datature) [![PyPI - Version](https://img.shields.io/pypi/v/
  datature?label=Pypi%20Package)](https://pypi.org/project/datature) [![PyPI -
   Downloads](https://img.shields.io/pypi/dm/datature?label=Pypi%20Downloads)]
      (https://pypi.org/project/datature) [![Join Datature Slack](https://
          img.shields.io/badge/Join%20The%20Community-Datature%20Slack-
@@ -30,76 +13,80 @@
      _c_d_n_._s_i_m_p_l_e_i_c_o_n_s_._o_r_g_/_y_o_u_t_u_b_e_/_#_F_F_0_0_0_0_][assets/transparent.png]_[_h_t_t_p_s_:_/_/
     _c_d_n_._s_i_m_p_l_e_i_c_o_n_s_._o_r_g_/_l_i_n_k_e_d_i_n_/_#_0_A_6_6_C_2_][assets/transparent.png]_[_h_t_t_p_s_:_/_/
 _c_d_n_._s_i_m_p_l_e_i_c_o_n_s_._o_r_g_/_t_w_i_t_t_e_r_/_#_1_D_9_B_F_0_][assets/transparent.png]_[_a_s_s_e_t_s_/_s_l_a_c_k_._p_n_g_]-
      -- :zap: Empower your MLOps pipelines and applications with seamless
     integrations :zap: Automate tasks to manage your datasets, run training
    experiments, export and deploy your models from [Datature Nexus](https://
  www.datature.io/nexus?utm_source=github) with ease. Perform development via
- [Python scripts](#python-usage) or with the [CLI](#cli-usage) - your choice!
+  [Python Scripts](#python-usage) or with the [Command-Line Interface](#cli-
+                                    usage).
 ---
-                     ## :rocket: Getting Started :rocket:
-## :snake: Prerequisites - `3.8` <= Python <= `3.12` We recommend users to
-create a virtual environment before installing any dependencies. For more
-information on virtual environments, please refer to: - [Python venv](https://
-docs.python.org/3/tutorial/venv.html) - [Conda](https://conda.io/projects/
-conda/en/stable/user-guide/install/index.html) - [virtualenvwrapper](https://
-virtualenvwrapper.readthedocs.io/en/latest/) ## :gear: Installation ```sh pip
-install --upgrade datature ``` --- ## Python Usage For a full list of
-documentation and examples, please refer to the [API docs](https://
-developers.datature.io/docs/python-sdk). ### Authentication To get started, you
-will first need to create a project on [Datature Nexus](https://
-www.datature.io/nexus?utm_source=github) (signing up is free!). You will then
-need to locate the [project secret key](https://developers.datature.io/v1.0.0/
-docs/hub-and-api). This key can only be accessed if you are the Project Owner
-or been granted elevated permissions by the Project Owner, and will be used for
-all subsequent authentication when invoking the various SDK functions. ###
-Examples To list projects: ```python from datature import nexus client =
-nexus.Client("3736971xxxxx") projects = client.list_projects() ``` To upload
-assets: ```python import os from datature import nexus logging.basicConfig()
-client = nexus.Client("3736971xxxxx") project = client.list_projects
-("proj_xxxxx") upload_session = project.assets.create_upload_session(groups=
-["dataset"]) with upload_session as session: session.add_path("/Users/dataset")
-print(len(upload_session)) ``` ### Logging You can vary the logging level
-depending on your task or use case (such as `DEBUG` to provide more insights),
-but the default `INFO` level is typically best suited for production use.
-```python import logging logging.basicConfig() logging.getLogger
-("nexus").setLevel(logging.DEBUG) ``` --- ## CLI Usage For a full list of
-documentation and examples, please refer to the [CLI docs](https://
-developers.datature.io/docs/cli). ### Authentication To get started, you will
-first need to create a project on [Datature Nexus](https://www.datature.io/
-nexus?utm_source=github) (signing up is free!). You will then need to locate
+                              ## Getting Started
+## Prerequisites - `3.8` <= Python <= `3.12` We recommend users to create a
+virtual environment before installing any dependencies. For more information on
+virtual environments, please refer to: - [Python venv](https://docs.python.org/
+3/tutorial/venv.html) - [Conda](https://conda.io/projects/conda/en/stable/user-
+guide/install/index.html) - [virtualenvwrapper](https://
+virtualenvwrapper.readthedocs.io/en/latest/) ## Installation ```sh pip install
+--upgrade datature ``` --- ## Python Usage For a full list of documentation and
+examples, please refer to the [API docs](https://developers.datature.io/docs/
+python-sdk). ### Authentication To get started, you will first need to create a
+project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github)
+(you can create sign up for a free account [here](https://nexus.datature.io/)).
+You will then need to locate the [project secret key](https://
+developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed
+if you are the Project Owner or have been granted elevated permissions by the
+Project Owner, and will be used for all subsequent authentication when invoking
+the various SDK functions. ### Examples To list projects: ```python from
+datature import nexus client = nexus.Client
+("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117") projects =
+client.list_projects() ``` To upload assets: ```python import os from datature
+import nexus logging.basicConfig() client = nexus.Client
+("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117") project =
+client.list_projects("proj_fca32b1bb15405d1c2bde19fd90b516d") upload_session =
+project.assets.create_upload_session(groups=["dataset"]) with upload_session as
+session: session.add_path("/Users/dataset") print(len(upload_session)) ``` ###
+Logging You can vary the logging level depending on your task or use case (such
+as `DEBUG` to provide more insights), but the default `INFO` level is typically
+best suited for production use. ```python import logging logging.basicConfig()
+logging.getLogger("datature-nexus").setLevel(logging.DEBUG) ``` --- ## CLI
+Usage For a full list of documentation and examples, please refer to the [CLI
+docs](https://developers.datature.io/docs/cli). ### Authentication To get
+started, you will first need to create a project on [Datature Nexus](https://
+www.datature.io/nexus?utm_source=github) (you can create sign up for a free
+account [here](https://nexus.datature.io/)). You will then need to locate the
+[project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api).
+This key can only be accessed if you are the Project Owner or have been granted
+elevated permissions by the Project Owner, and will be used for all subsequent
+authentication when invoking the various SDK functions. Once you have the
+project secret, you will now be able to make API requests using the CLI by
+entering the command `datature projects auth`: ```bash datature projects auth
+[?] Enter the project secret: ************************************************
+[?] Make [Your Project Name] the default project? (Y/n): y Authentication
+succeeded. ``` You will now be able to run your desired CLI commands as
+outlined above. To see all possible functions as well as view the required
+inputs and expected outputs, check out the following documentation. ### Project
+Management `datature projects` Show a help page of various functions to add
+projects, select the default project, and retrieve project information. ####
+Authenticate Project `datature projects auth` Authenticate new projects using
 the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-
-api). This key can only be accessed if you are the Project Owner or been
-granted elevated permissions by the Project Owner, and will be used for all
-subsequent authentication when invoking the various SDK functions. Once you
-have the project secret, you will now be able to make API requests using the
-CLI by entering the command `datature projects auth`: ```bash datature projects
-auth [?] Enter the project secret:
-************************************************ [?] Make [Your Project Name]
-the default project? (Y/n): y Authentication succeeded. ``` You will now be
-able to run your desired CLI commands as outlined above. To see all possible
-functions as well as view the required inputs and expected outputs, check out
-the following documentation. ### Project Management `datature projects` Show a
-help page of various functions to add projects, select the default project, and
-retrieve project information. #### Auth Project `datature projects auth`
-Authenticate new projects using the [project secret key](https://
-developers.datature.io/v2.0.0/docs/hub-and-api). Multiple projects can be
-authenticated and stored using different secret keys. #### Select Project
-`datature projects select` Select an active project to work on from a list of
-saved projects. All subsequent CLI commands will be in the context of the
-selected project until a different project is selected, or the shell session is
-terminated. ```bash $ datature projects select > My Cool Project New Test
-Project Your active project is now: [Dicom] ``` #### List Projects `datature
-projects list` View a table of saved projects with columns containing the names
-of the projects, the total number of assets, the number of annotated assets,
-the number of annotations, and the number of tags for each project. The name of
-the active project is displayed at the bottom of the list. ```bash $ datature
-projects list NAME TOTAL_ASSETS ANNOTATED_ASSETS ANNOTATIONS TAGS My Cool
-Project 4071 433 1874 3 New Test Project 718 53 959 4 Your active project is
-now: [My Cool Project] ``` ### Asset Management #### Upload Assets `datature
+api). Multiple projects can be authenticated and stored using different secret
+keys. #### Select Project `datature projects select` Select an active project
+to work on from a list of saved projects. All subsequent CLI commands will be
+in the context of the selected project until a different project is selected,
+or the shell session is terminated. ```bash $ datature projects select > Brain
+Tumor DICOM Hand Gesture Keypoint Detection Your active project is now: [Brain
+Tumor DICOM] ``` #### List Projects `datature projects list` View a table of
+saved projects with columns containing the names of the projects, the total
+number of assets, the number of annotated assets, the number of annotations,
+and the number of tags for each project. The name of the active project is
+displayed at the bottom of the list. ```bash $ datature projects list NAME
+TOTAL_ASSETS ANNOTATED_ASSETS ANNOTATIONS TAGS Brain Tumor DICOM 4071 433 1874
+3 Hand Gesture Keypoint Detection 718 53 959 4 Your active project is now:
+[Brain Tumor DICOM] ``` ### Asset Management #### Upload Assets `datature
 assets upload` Upload assets to [Datature Nexus](https://www.datature.io/
 nexus?utm_source=github). You will be prompted to enter the path to the folder
 containing the assets that you wish to upload, as well as optional group name
 (s) to categorize the set of assets. This function is designed specially for
 bulk uploading of large datasets, which accelerates the process of onboarding
 data for subsequent annotation and training. This function also supports DICOM
 and NIfTI file upload, which caters to important medical use cases. ```bash $
@@ -112,15 +99,15 @@
 100% [281/281] in 1:17.5 (3.56/s) Server processing completed. ``` #### Group
 Assets `datature assets groups` List asset group information within your
 project. You will be prompted to select an existing group or create a new
 group. If you select an existing group, information about the selected group
 will be displayed, including the total number of assets in the group, the
 number of assets that have been annotated, reviewed, or marked for fixes, and
 the number of assets that have been completed. ```bash $ datature assets groups
-> main groupName2 NAME TOTAL ANNOTATED REVIEW TOFIX COMPLETED main 8 1 0 0 0
+> main validation NAME TOTAL ANNOTATED REVIEW TOFIX COMPLETED main 8 1 0 0 0
 ``` ### Annotation Management #### Upload Annotations `datature annotations
 upload` Upload annotation files to [Datature Nexus](https://www.datature.io/
 nexus?utm_source=github) You will be prompted to enter the path of the
 annotation file you wish to upload and select a [supported annotation format]
 (https://developers.datature.io/docs/uploading-annotations#supported-
 annotation-formats). ```bash $ datature annotations upload [?] Enter the
 annotation files path to be uploaded: /Users/Downloads/Training.csv Processing
@@ -139,12 +126,73 @@
 100% [1/1] in 7.0s (0.14/s) Server processing completed. ``` ### Artifact
 Management #### Artifact Download `datature artifacts download` Download a
 model artifact from [Datature Nexus](https://www.datature.io/
 nexus?utm_source=github). You will be prompted to enter a folder path to save
 the model to, and select the name and [export format](https://
 developers.datature.io/docs/export-formats) of the artifact to download.
 ```bash $ datature artifacts download [?] Enter the folder path to save model:
-/Volumes/ [?] Which artifact do you want to download?: BEAF45-Workflowc >
-BEAF45-Workflowc [?] Which model format do you want to download?: tensorflow >
-tensorflow tflite onnx Downloading
+/Volumes/ [?] Which artifact do you want to download?: BEAF45-Workflow >
+BEAF45-Workflow [?] Which model format do you want to download?: tensorflow >
+TensorFlow TFLite ONNX Downloading
 |ââââââââââââââââââââââââââââââââââââââââ|
-100% [443421394/443421394] in 7.1s (62639992.12/s) ```
+100% [443421394/443421394] in 7.1s (62639992.12/s) ``` ## FAQ ### How do I find
+my Secret Key and Project Key? We provide a step-by-step guide to finding these
+two crucial keys in our [Developer's Documentation](https://
+developers.datature.io/docs/project-keys-and-secret-keys). You can also explore
+the other sections under [Python SDK](https://developers.datature.io/docs/
+python-sdk) to learn more about the full functionality and feature set. ### I'm
+facing some issues, what now? We're sorry to hear that, please head over to our
+[Issues](https://github.com/datature/datature-py/issues) page and post a
+detailed bug report following our guidelines, and we will address your concerns
+as soon as we can. Alternatively, ping us in our [Community Slack](https://
+datature.io/community) where our engineers will attend to your needs. ### I've
+noticed that some features are missing, how do I contribute? Datature Python
+SDK is open-source and we welcome everyone to help to improve it. Please check
+out our [Contributing Guide](CONTRIBUTING.md) to learn how you can be a part of
+the team. ### How do I resolve the `command not found: datature` error for the
+CLI? The `command not found: datature` error indicates that the Datature SDK/
+CLI tool is not installed properly in your system's PATH, or it has not been
+installed at all. To resolve this error, please follow these steps: #### Ensure
+Datature CLI is Installed Before anything else, verify that you've installed
+the Datature CLI. You can install it using pip with the following command:
+```bash pip install datature ``` If you're using a virtual environment (which
+is recommended), ensure that it's activated before running the installation
+command. #### Check Your PATH After installation, the datature command should
+be automatically added to your system's PATH. If it's not found, you may need
+to manually add the directory containing the datature executable to your PATH:
+```bash which datature ``` Or ```bash pip show datature ``` As expected, it
+will show the location of the package like this: ```bash Location: /
+Users/.pyenv/versions/3.8.18/lib/python3.8/site-packages ``` #### Add the Path
+to Your Profile Open your shell profile file with a text editor. This file
+could be one of ~/.bash_profile, ~/.bashrc, ~/.zshrc, etc., depending on which
+shell you use and the specific configuration of your operating system. For
+example, you can add the path using the following command: ```bash echo 'export
+PATH="$PATH:/path/to/datature"' >> ~/.bash_profile ``` Replace /path/to/
+datature with the actual path you found with which datature or pip show
+datature. #### Restart Your Terminal Sometimes, changes to the PATH environment
+variable do not take effect until you open a new terminal session. After
+installation or modification of the PATH, close your current terminal and open
+a new one, then try the command again. ### What does the warning `As the c
+extension couldn't be imported, google-crc32c is using a pure python
+implementation that is significantly slower. If possible, please configure a c
+build environment and compile the extension` mean, and do I need to take any
+action? This warning is indicating that the `google-crc32c` library is falling
+back to a pure Python implementation for calculating CRC32C checksums because
+it cannot find the C extension which is usually faster. The Python
+implementation is fully functional but performs slower than its C counterpart.
+While this won't harm the function of the library, you may experience
+performance issues if your application requires high-speed checksum computing.
+To address this warning for improved performance, you can take the following
+steps to compile the C extension: #### Install the Build Essentials Make sure
+that you have the necessary build tools installed to compile the C extension.
+On Ubuntu/Debian systems, you can install build-essential by running: ```bash
+sudo apt-get install build-essential ``` On Red Hat/CentOS systems, you can
+use: ```bash sudo yum install gcc gcc-c++ make ``` On macOS, ensure you have
+Xcode Command Line Tools installed: ```bash xcode-select --install ``` ####
+Reinstall google-crc32c with C Extension With the build environment configured,
+you can attempt to reinstall the google-crc32c library which should now include
+the C extension: ```bash pip install --no-cache-dir --force-reinstall google-
+crc32c ``` By taking these steps, you should be able to eliminate the warning
+by having the faster C extension compiled and used by google-crc32c. If speed
+is not critical for your use case, you can choose to ignore this warning, and
+the library will still function correctly, albeit with potentially decreased
+performance.
```

### Comparing `datature-1.6.0/datature/nexus/api/annotation/annotation.py` & `datature-1.7.0/datature/nexus/api/annotation/annotation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   annotation.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Annotation API
-'''
+"""
 
 import json
 import zipfile
-from typing import Union
 from pathlib import Path
+from typing import Union
 
 import msgspec
-
-from datature.nexus.utils import utils
-from datature.nexus import models, error
-from datature.nexus.api.operation import Operation
+from datature.nexus import error, models
 from datature.nexus.api.annotation.import_session import ImportSession
+from datature.nexus.api.operation import Operation
+from datature.nexus.api.types import (
+    AnnotationExportMetadata,
+    AnnotationFilter,
+    AnnotationMetadata,
+    Pagination,
+)
 from datature.nexus.client_context import ClientContext, RestContext
-from datature.nexus.api.types import (AnnotationMetadata, Pagination,
-                                      AnnotationExportMetadata,
-                                      AnnotationFilter)
+from datature.nexus.utils import utils
 
 
 class Annotation(RestContext):
     """Datature Annotation API Resource."""
 
     def __init__(self, client_context: ClientContext):
         """Initialize the API Resource."""
         super().__init__(client_context)
         self.operation = Operation(client_context)
 
     def list(
         self,
         pagination: Union[Pagination, dict, None] = None,
         filters: Union[AnnotationFilter, dict, None] = None,
-        include_attributes: bool = False
+        include_attributes: bool = False,
     ) -> models.PaginationResponse[models.Annotation]:
         """Lists all annotations of a specific asset.
 
         :param pagination: The pagination options.
         :param filters: The filter options.
         :param include_attributes: A flag indicating whether to include the annotation attributes.
         :return: A list of msgspec struct containing
             annotation metadata with the following structure:
 
             .. code-block:: python
 
                 PaginationResponse(
-                    next_page='NjVhYTE0ZDY3YzQ5MThlMTJjYTUyOGRk', 
-                    prev_page=None, 
+                    next_page='NjVhYTE0ZDY3YzQ5MThlMTJjYTUyOGRk',
+                    prev_page=None,
                     data=[
                         Annotation(
                             id='annot_e5028bdc-122e-4837-b354-d82b95320b69',
-                            project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                            asset_id='asset_6647b58e-86af-460c-9a85-efead830aee8', 
-                            tag='dog', 
-                            bound_type='Polygon', 
+                            project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                            asset_id='asset_6647b58e-86af-460c-9a85-efead830aee8',
+                            tag='dog',
+                            bound_type='Polygon',
                             bound=[
-                                [0.42918, 0.45322666666666667], 
-                                [0.43677999999999995, 0.4579466666666666], 
-                                [0.43677999999999995, 0.46941333333333335], 
-                                [0.44236000000000003, 0.4788800000000001], 
-                                [0.45146, 0.4829333333333333], 
-                                [0.45754, 0.48696000000000006], 
-                                [0.48234, 0.4842666666666666], 
-                                [0.4869, 0.43432000000000004], 
+                                [0.42918, 0.45322666666666667],
+                                [0.43677999999999995, 0.4579466666666666],
+                                [0.43677999999999995, 0.46941333333333335],
+                                [0.44236000000000003, 0.4788800000000001],
+                                [0.45146, 0.4829333333333333],
+                                [0.45754, 0.48696000000000006],
+                                [0.48234, 0.4842666666666666],
+                                [0.4869, 0.43432000000000004],
                                 [0.50514, 0.4302666666666667]
-                            ], 
+                            ],
                             create_date=None,
                             ontology_id='ontology_843e486c-58d7-45a7-b722-f4948e204a56',
                             attributes=[
                                 OntologyAttributeValue(
                                     id='attri_d0877827-63d6-4794-b520-ef3e0c57ef71',
                                     name='Tag Group',
                                     value=['person']
@@ -118,38 +120,38 @@
         if filters is None:
             filters = AnnotationFilter()
 
         return self.requester.GET(
             f"/projects/{self.project_id}/annotations",
             query={
                 **pagination.to_json(),
-                **filters.to_json(), "includeAttributes": include_attributes
+                **filters.to_json(),
+                "includeAttributes": include_attributes,
             },
-            response_type=models.PaginationResponse[models.Annotation])
+            response_type=models.PaginationResponse[models.Annotation],
+        )
 
-    def create(
-            self, annotation: Union[AnnotationMetadata,
-                                    dict]) -> models.Annotation:
+    def create(self, annotation: Union[AnnotationMetadata, dict]) -> models.Annotation:
         """Creates an annotation.
 
         :param annotation: The metadata of the annotation.
         :return: A msgspec struct containing the annotation metadata with the following structure:
 
             .. code-block:: python
 
                 Annotation(
-                    id='annot_ffcd02f1-bac2-4cd4-b959-a04e0c67b44e', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                    asset_id='asset_dd0c72a4-a8c4-479e-a130-432e699351fc', 
-                    tag='boat', 
+                    id='annot_ffcd02f1-bac2-4cd4-b959-a04e0c67b44e',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                    asset_id='asset_dd0c72a4-a8c4-479e-a130-432e699351fc',
+                    tag='boat',
                     bound_type='Rectangle',
                     bound=[
-                        [0.425, 0.49382716049382713], 
-                        [0.425, 0.6419753086419753], 
-                        [0.6, 0.6419753086419753], 
+                        [0.425, 0.49382716049382713],
+                        [0.425, 0.6419753086419753],
+                        [0.6, 0.6419753086419753],
                         [0.6, 0.49382716049382713]
                     ],
                     create_date=1701927649302,
                 )
 
         :example:
             .. code-block:: python
@@ -169,41 +171,43 @@
                 })
         """
         assert isinstance(annotation, (AnnotationMetadata, dict))
 
         if isinstance(annotation, dict):
             annotation = AnnotationMetadata(**annotation)
 
-        return self.requester.POST(f"/projects/{self.project_id}/annotations",
-                                   request_body=annotation.to_json(),
-                                   response_type=models.Annotation)
-
-    def get(self,
-            annotation_id: str,
-            include_attributes: bool = False) -> models.Annotation:
+        return self.requester.POST(
+            f"/projects/{self.project_id}/annotations",
+            request_body=annotation.to_json(),
+            response_type=models.Annotation,
+        )
+
+    def get(
+        self, annotation_id: str, include_attributes: bool = False
+    ) -> models.Annotation:
         """Retrieves a specific annotation using the annotation ID.
 
         :param annotation_id: The ID of the annotation.
         :param include_attributes: A flag indicating whether to include the annotation attributes.
         :return: A msgspec struct containing
             the specific annotation metadata with the following structure:
 
             .. code-block:: python
 
                     Annotation(
-                        id='annot_a9ff9b21-c0e2-49ff-8a69-773aaf00a6f8', 
-                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                        asset_id='asset_f4dcb429-0332-4dd6-a1b4-fee794031ba6', 
-                        tag='boat', 
+                        id='annot_a9ff9b21-c0e2-49ff-8a69-773aaf00a6f8',
+                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                        asset_id='asset_f4dcb429-0332-4dd6-a1b4-fee794031ba6',
+                        tag='boat',
                         bound_type='Rectangle',
                         create_date=1701927649302,
                         bound=[
-                            [0.2772511848341232, 0.34635416666666663], 
-                            [0.2772511848341232, 0.46875], 
-                            [0.54739336492891, 0.46875], 
+                            [0.2772511848341232, 0.34635416666666663],
+                            [0.2772511848341232, 0.46875],
+                            [0.54739336492891, 0.46875],
                             [0.54739336492891, 0.34635416666666663]
                         ],
                         ontology_id='ontology_843e486c-58d7-45a7-b722-f4948e204a56',
                         attributes=[
                             OntologyAttributeValue(
                                 id='attri_d0877827-63d6-4794-b520-ef3e0c57ef71',
                                 name='Tag Group',
@@ -223,15 +227,16 @@
                         include_attributes=True
                     )
         """
         assert isinstance(annotation_id, str)
         return self.requester.GET(
             f"/projects/{self.project_id}/annotations/{annotation_id}",
             query={"includeAttributes": include_attributes},
-            response_type=models.Annotation)
+            response_type=models.Annotation,
+        )
 
     def delete(self, annotation_id: str) -> models.DeleteResponse:
         """Deletes a specific annotation from the project.
 
         :param annotation_id: The ID of the annotation.
         :return: A msgspec struct containing
             the deleted annotation ID and the deletion status with the following structure:
@@ -247,48 +252,51 @@
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.annotations.delete("asset_6aea3395-9a72-4bb5-9ee0-19248c903c56")
         """
         assert isinstance(annotation_id, str)
         return self.requester.DELETE(
             f"/projects/{self.project_id}/annotations/{annotation_id}",
-            response_type=models.DeleteResponse)
+            response_type=models.DeleteResponse,
+        )
 
-    def create_export(self,
-                      export_metadata: Union[AnnotationExportMetadata, dict],
-                      background: bool = False) -> models.Operation:
+    def create_export(
+        self,
+        export_metadata: Union[AnnotationExportMetadata, dict],
+        background: bool = False,
+    ) -> models.Operation:
         """Exports all annotations from the project in a specific annotation format.
 
         :param export_metadata: A dict containing other export options.
         :param background: Signal to complete the annotation export
                             process in the background. Defaults to False.
         :return: A msgspec struct containing the operation metadata of the annotation export
             with the following structure:
 
             .. code-block:: python
 
                 Operation(
-                    id='op_ea10c06e-0e2a-4087-b2cf-1a1c9c42d83d', 
-                    kind='nexus.annotations.export', 
+                    id='op_ea10c06e-0e2a-4087-b2cf-1a1c9c42d83d',
+                    kind='nexus.annotations.export',
                     status=OperationStatus(
                         overview='Finished',
-                        message='Operation finished', 
+                        message='Operation finished',
                         progress=OperationProgress(
-                            unit='whole operation', 
+                            unit='whole operation',
                             with_status=OperationProgressWithStatus(
-                                Queued=0, 
-                                Running=0, 
-                                Finished=1, 
-                                Cancelled=0, 
+                                Queued=0,
+                                Running=0,
+                                Finished=1,
+                                Cancelled=0,
                                 Errored=0
                             )
                         )
-                    ), 
+                    ),
                     create_date=1701927649302,
-                    update_date=1701927649302    
+                    update_date=1701927649302
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
@@ -308,38 +316,38 @@
 
         if isinstance(export_metadata, dict):
             export_metadata = AnnotationExportMetadata(**export_metadata)
 
         operation = self.requester.POST(
             f"/projects/{self.project_id}/annotationexports",
             request_body=export_metadata.to_json(),
-            response_type=models.Operation)
+            response_type=models.Operation,
+        )
 
         if background:
             return operation
 
         return self.operation.wait_until_done(operation.id)
 
     def download_exported_file(
-            self,
-            op_id: str,
-            path: Union[str, Path, None] = None) -> models.LocalAnnotations:
+        self, op_id: str, path: Union[str, Path, None] = None
+    ) -> models.LocalAnnotations:
         """Retrieves the download link of the exported annotations.
 
         :param op_id: The operation ID of the annotation export.
         :param path: The download path for the annotation, default current path.
         :return: A msgspec struct with the download metadata of
             the annotation export with the following structure:
 
             .. code-block:: python
 
                 LocalAnnotations(
-                    download_path='local', 
+                    download_path='local',
                     file_names=[
-                        'cd067221d5a6e4007ccbb4afb5966535/train.csv', 
+                        'cd067221d5a6e4007ccbb4afb5966535/train.csv',
                         'cd067221d5a6e4007ccbb4afb5966535/validate.csv'
                     ]
                 )
 
         :example:
             .. code-block:: python
 
@@ -352,41 +360,40 @@
                 )
         """
         assert isinstance(op_id, str)
         assert isinstance(path, (str, Path, type(None)))
 
         exported_files = self.requester.GET(
             f"/projects/{self.project_id}/annotationexports/{op_id}",
-            response_type=models.ExportedAnnotations)
+            response_type=models.ExportedAnnotations,
+        )
 
         download_path = utils.get_download_path(path)
 
         if exported_files.status == "Finished" and exported_files.download is not None:
-            download_tmpfile = utils.download_files_to_tempfile(
-                exported_files.download)
+            download_tmpfile = utils.download_files_to_tempfile(exported_files.download)
 
-            with zipfile.ZipFile(download_tmpfile, 'r') as zip_ref:
+            with zipfile.ZipFile(download_tmpfile, "r") as zip_ref:
                 zip_ref.extractall(download_path)
 
                 file_names = [
-                    info.filename for info in zip_ref.infolist()
-                    if not info.is_dir()
+                    info.filename for info in zip_ref.infolist() if not info.is_dir()
                 ]
 
-            return msgspec.json.decode(json.dumps({
-                "download_path":
-                str(download_path),
-                "file_names":
-                file_names
-            }),
-                                       type=models.LocalAnnotations)
+            return msgspec.json.decode(
+                json.dumps(
+                    {"download_path": str(download_path), "file_names": file_names}
+                ),
+                type=models.LocalAnnotations,
+            )
 
         # If didn't find the model key in the artifacts, raise an 404 error
         raise error.NotFoundError(
-            f"Export with id {op_id} not found, please export first.")
+            f"Export with id {op_id} not found, please export first."
+        )
 
     def create_import_session(self, background: bool = False):
         """
         Creates an import session to import or update annotations.
             For bulk annotation import, we allow the user to add up to 1000
             files in one single import session.
             To add file into the import session, simply include its file path as an argument
@@ -430,36 +437,36 @@
         """Lists the import sessions from the project.
 
         :return: A list of msgspec struct containing import sessions with the following structure:
 
             .. code-block:: python
 
                 [ImportSession(
-                    id='annotsess_58bb96a6-9dd5-4c78-89e7-57366060318e', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                    id='annotsess_58bb96a6-9dd5-4c78-89e7-57366060318e',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
                     status=ImportSessionStatus(
                         overview='Finished',
                         message='Annotation Imported successfully.',
-                        update_date=1701677312962, 
+                        update_date=1701677312962,
                         annotations=ImportSessionStatusAnnotations(
                             with_status=ImportSessionAnnotationStatus(
-                                Processed=1548, 
+                                Processed=1548,
                                 Committed=1548
                             )
-                        ), 
+                        ),
                         files=ImportSessionStatusFiles(
-                            total_size_bytes=63368, 
-                            page_count=1, 
+                            total_size_bytes=63368,
+                            page_count=1,
                             with_status=ImportSessionFilesStatus(
-                                Processing=0, 
-                                Processed=1, 
+                                Processing=0,
+                                Processed=1,
                                 FailedProcess=0
                             )
                         )
-                    ), 
+                    ),
                     expiry_date=1701927649302,
                     create_date=1701927649302,
                     update_date=1701927649302
                 )]
 
         :example:
 
@@ -469,49 +476,49 @@
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                 project.annotations.list_import_sessions()
         """
         return self.requester.GET(
             f"/projects/{self.project_id}/annotationimportsessions",
-            response_type=models.ImportSessions)
+            response_type=models.ImportSessions,
+        )
 
-    def get_import_session(self,
-                           import_session_id: str) -> models.ImportSession:
+    def get_import_session(self, import_session_id: str) -> models.ImportSession:
         """Retrieves a specific import session from the project.
 
         :param import_session_id: The ID of the import session.
 
         :return: A msgspec struct containing the import session with the following structure:
 
             .. code-block:: python
 
                 ImportSession(
-                    id='annotsess_58bb96a6-9dd5-4c78-89e7-57366060318e', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                    id='annotsess_58bb96a6-9dd5-4c78-89e7-57366060318e',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
                     status=ImportSessionStatus(
                         overview='Finished',
                         message='Annotation Imported successfully.',
                         update_date=1701677312962,
                         annotations=ImportSessionStatusAnnotations(
                             with_status=ImportSessionAnnotationStatus(
-                                Processed=1548, 
+                                Processed=1548,
                                 Committed=1548
                             )
-                        ), 
+                        ),
                         files=ImportSessionStatusFiles(
-                            total_size_bytes=63368, 
-                            page_count=1, 
+                            total_size_bytes=63368,
+                            page_count=1,
                             with_status=ImportSessionFilesStatus(
-                                Processing=0, 
-                                Processed=1, 
+                                Processing=0,
+                                Processed=1,
                                 FailedProcess=0
                             )
                         )
-                    ), 
+                    ),
                     expiry_date=1701927649302,
                     create_date=1701927649302,
                     update_date=1701927649302
                 )
 
         :example:
 
@@ -525,29 +532,31 @@
                     "annotsess_75879caf-184d-4d82-912b-180609a72ace"
                 )
         """
         assert isinstance(import_session_id, str)
 
         return self.requester.GET(
             f"/projects/{self.project_id}/annotationimportsessions/{import_session_id}",
-            response_type=models.ImportSession)
+            response_type=models.ImportSession,
+        )
 
     def get_import_session_logs(
-            self, import_session_id: str) -> models.ImportSessionLog:
+        self, import_session_id: str
+    ) -> models.ImportSessionLog:
         """Retrieves import session logs from the project.
 
         :param import_session_id: The ID of the import session.
 
         :return: A msgspec struct containing the import session logs with the following structure:
 
             .. code-block:: python
 
                 ImportSessionLog(
-                    id='annotsess_1e433826-ab9c-402e-8b9a-a95d82f358f1', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                    id='annotsess_1e433826-ab9c-402e-8b9a-a95d82f358f1',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
                     logs=[]
                 )
 
         :example:
 
             .. code-block:: python
 
@@ -558,8 +567,9 @@
                 project.annotations.get_import_session_logs(
                     "annotsess_75879caf-184d-4d82-912b-180609a72ace"
                 )
         """
         assert isinstance(import_session_id, str)
         return self.requester.GET(
             f"/projects/{self.project_id}/annotationimportsessions/{import_session_id}/logs",
-            response_type=models.ImportSessionLog)
+            response_type=models.ImportSessionLog,
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/annotation/import_session.py` & `datature-1.7.0/datature/nexus/api/annotation/import_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   upload_session.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session
-'''
+"""
 # pylint: disable=E1102,R0914,R0912,R0902,R1732
 
-import time
 import base64
+import concurrent.futures
 import logging
 import threading
-from os import path
-import concurrent.futures
+import time
 from contextlib import ContextDecorator
 from datetime import datetime, timedelta
+from os import path
 
 import google_crc32c
-
-from datature.nexus import models
-from datature.nexus.utils import utils
-from datature.nexus import error, config
+from datature.nexus import config, error, models
 from datature.nexus.api.types import OperationStatusOverview
 from datature.nexus.client_context import ClientContext, RestContext
+from datature.nexus.utils import utils
 
-logger = logging.getLogger("nexus")
+logger = logging.getLogger("datature-nexus")
 
 
 class ImportSession(RestContext, ContextDecorator):
     """
     Datature Annotation Import Session Class.
 
     :param background: A flag indicating whether
@@ -50,60 +48,63 @@
         self.max_files_per_batch = config.ANNOTATION_IMPORT_SESSION_BATCH_SIZE
         self.max_bytes_per_batch = config.ANNOTATION_IMPORT_SESSION_BATCH_BYTES
 
         self._local = threading.local()
 
         import_session = self.requester.POST(
             f"/projects/{self.project_id}/annotationimportsessions",
-            response_type=models.ImportSession)
+            response_type=models.ImportSession,
+        )
 
         self.import_session_id = import_session.id
         self.background = background
 
         self.current_batch = []
         self.annotations_contents_map = {}
         self.current_batch_bytes_size = 0
         self.filenames = set()
 
     def _init_http_session(self):
-        """ Init gcs upload session. """
+        """Init gcs upload session."""
         self._local.http_session = utils.init_gcs_upload_session()
 
     def __enter__(self):
         return self
 
     def __exit__(self, _exc_type, exc_val, _exc_tb):
         """
         Exit function.
         The function will be called if an exception is raised inside the context manager
         """
         if exc_val is not None:
             # Error handling, patch import session status
-            self._patch_status({
-                "condition": "FilesProcessed",
-                "status": "FailedReach",
-            })
+            self._patch_status(
+                {
+                    "condition": "FilesProcessed",
+                    "status": "FailedReach",
+                }
+            )
             logger.warning(
-                "Import session error existed, no file will be updated: %s",
-                exc_val)
+                "Import session error existed, no file will be updated: %s", exc_val
+            )
             return True
 
         self._upload_current_batch()
 
         # Patch import session status
         self._patch_status({"condition": "FilesInserted", "status": "Reached"})
 
         if self.background:
             return True
 
         # Looping check import session status
         return self.wait_until_done()
 
     def __len__(self):
-        """ Over write len function. """
+        """Over write len function."""
         return len(self.filenames)
 
     def _calculate_file_hash(self, file_contents):
         """Calculate and return the CRC32C hash of the given file contents."""
         file_hash = google_crc32c.Checksum()
         file_hash.update(file_contents)
         return base64.b64encode(file_hash.digest()).decode("utf-8")
@@ -118,163 +119,170 @@
         """
         if len(self.filenames) + 1 > self.max_files_per_session:
             raise error.Error(
                 f"One import session allow max {self.max_files_per_session} files."
             )
         if filename in self.filenames:
             raise error.Error(
-                f"Filename {filename} already exists in this import session.")
+                f"Filename {filename} already exists in this import session."
+            )
 
         # Push the file to the current batch
         self.filenames.add(filename)
         self.current_batch_bytes_size += len(file_bytes)
 
         self.annotations_contents_map[filename] = {
             "file_type": "bytes",
-            "contents": file_bytes
+            "contents": file_bytes,
         }
 
-        self.current_batch.append({
-            "filename":
-            filename,
-            "size":
-            len(file_bytes),
-            "crc32c":
-            self._calculate_file_hash(file_bytes)
-        })
+        self.current_batch.append(
+            {
+                "filename": filename,
+                "size": len(file_bytes),
+                "crc32c": self._calculate_file_hash(file_bytes),
+            }
+        )
 
         # Check current batch size
-        if len(self.filenames) >= self.max_files_per_batch or \
-           self.current_batch_bytes_size >= self.max_bytes_per_batch:
+        if (
+            len(self.filenames) >= self.max_files_per_batch
+            or self.current_batch_bytes_size >= self.max_bytes_per_batch
+        ):
             self._upload_current_batch()
 
     def add_path(self, file_path: str):
         """
         Attach file path or folders to import session
 
         :param file_path: The file or folder path.
         :returns: None
         """
         if path.isdir(file_path):
             file_path_list = utils.find_all_annotations_files(file_path)
         else:
             file_path_list = [file_path]
 
-        if len(self.filenames) + len(
-                file_path_list) > self.max_files_per_session:
+        if len(self.filenames) + len(file_path_list) > self.max_files_per_session:
             raise error.Error(
                 f"One import session allow max {self.max_files_per_session} files."
             )
 
         for _file_path in file_path_list:
-            with open(_file_path, 'rb') as file:
+            with open(_file_path, "rb") as file:
                 contents = file.read()
                 filename = path.basename(_file_path)
 
                 if filename in self.filenames:
                     raise error.Error(
                         f"Filename {filename} already exists in this import session."
                     )
 
                 self.filenames.add(filename)
                 self.current_batch_bytes_size += len(contents)
 
                 self.annotations_contents_map[filename] = {
                     "file_type": "path",
-                    "contents": _file_path
+                    "contents": _file_path,
                 }
 
-                self.current_batch.append({
-                    "filename":
-                    filename,
-                    "size":
-                    len(contents),
-                    "crc32c":
-                    self._calculate_file_hash(contents)
-                })
+                self.current_batch.append(
+                    {
+                        "filename": filename,
+                        "size": len(contents),
+                        "crc32c": self._calculate_file_hash(contents),
+                    }
+                )
 
         # Check current batch size
-        if len(self.filenames) >= self.max_files_per_batch or \
-           self.current_batch_bytes_size >= self.max_bytes_per_batch:
+        if (
+            len(self.filenames) >= self.max_files_per_batch
+            or self.current_batch_bytes_size >= self.max_bytes_per_batch
+        ):
             self._upload_current_batch()
 
     def wait_until_done(self):
         """
         Wait for all operations to be done.
             This function only works when background is set to False.
         """
         elapsed_time = datetime.now() + timedelta(
-            seconds=config.OPERATION_LOOPING_TIMEOUT_SECONDS)
+            seconds=config.OPERATION_LOOPING_TIMEOUT_SECONDS
+        )
 
         while True:
             import_session = self.requester.GET(
                 f"/projects/{self.project_id}/annotationimportsessions/{self.import_session_id}",
-                response_type=models.ImportSession)
+                response_type=models.ImportSession,
+            )
 
             logger.debug("Looping import sessions status: %s", import_session)
 
             if import_session.status.overview == OperationStatusOverview.ERRORED.value:
                 raise error.BadRequestError(
                     f"Error: Please use 'retrieve_import_session_logs"
-                    f"({self.import_session_id})' to check the error details.")
+                    f"({self.import_session_id})' to check the error details."
+                )
 
             if import_session.status.overview == OperationStatusOverview.FINISHED.value:
                 return True
 
             # if the operation has not finished when the timeouts
             if elapsed_time < datetime.now():
                 logger.warning(
                     "Operation timeout: Please use"
                     " 'retrieve_import_session_logs(%s)' to check the error details.",
-                    self.import_session_id)
+                    self.import_session_id,
+                )
                 return False
 
             time.sleep(config.OPERATION_LOOPING_DELAY_SECONDS)
 
     def _upload_file(self, filename, signed_url):
-        """ Upload file to GCS. """
+        """Upload file to GCS."""
         file_info = self.annotations_contents_map[filename]
         file_type = file_info["file_type"]
         file_contents = file_info["contents"]
 
         self._local.http_session.request(
             signed_url.get("method"),
             signed_url.get("url"),
             headers=signed_url.get("headers"),
-            data=file_contents if file_type == "bytes" else open(
-                file_contents, 'rb'),
-            timeout=config.REQUEST_TIME_OUT_SECONDS)
+            data=file_contents if file_type == "bytes" else open(file_contents, "rb"),
+            timeout=config.REQUEST_TIME_OUT_SECONDS,
+        )
 
         return filename
 
     def _upload_current_batch(self):
         batch_segments = [
-            self.current_batch[i:i + self.max_files_per_batch] for i in range(
-                0, len(self.current_batch), self.max_files_per_batch)
+            self.current_batch[i : i + self.max_files_per_batch]
+            for i in range(0, len(self.current_batch), self.max_files_per_batch)
         ]
 
         for segment in batch_segments:
             # Add files to import session
-            logger.debug("Start uploading files to import session: %s",
-                         segment)
+            logger.debug("Start uploading files to import session: %s", segment)
 
             files_res = self.requester.POST(
                 f"""/projects/{self.project_id}/annotationimportsessions/{
                     self.import_session_id}/files""",
                 request_body={"files": segment},
-                response_type=models.InsertImportSessionFiles)
+                response_type=models.InsertImportSessionFiles,
+            )
 
-            logger.debug("Start uploading files to import session: %s",
-                         files_res)
+            logger.debug("Start uploading files to import session: %s", files_res)
 
             with concurrent.futures.ThreadPoolExecutor(
-                    initializer=self._init_http_session) as executor:
+                initializer=self._init_http_session
+            ) as executor:
                 futures = [
-                    executor.submit(self._upload_file, upload_file.filename,
-                                    upload_file.upload)
+                    executor.submit(
+                        self._upload_file, upload_file.filename, upload_file.upload
+                    )
                     for upload_file in files_res.files
                 ]
 
                 for future in concurrent.futures.as_completed(futures):
                     filename = future.result()
 
                     logger.debug("Finished Uploading: % s", filename)
@@ -283,37 +291,36 @@
 
         # Reset current batch
         self.current_batch = []
         self.annotations_contents_map = {}
         self.current_batch_bytes_size = 0
 
     def _patch_status(self, status_condition: dict) -> models.ImportSession:
-        """ Patch import session status """
+        """Patch import session status"""
         import_session = self.requester.PATCH(
             f"/projects/{self.project_id}/annotationimportsessions/{self.import_session_id}",
-            request_body={"status": {
-                "conditions": [status_condition]
-            }},
-            response_type=models.ImportSession)
+            request_body={"status": {"conditions": [status_condition]}},
+            response_type=models.ImportSession,
+        )
 
         return import_session
 
     def get_logs(self) -> models.ImportSessionLog:
         """
         Retrieves import session logs from the project.
 
         :param import_session_id: The ID of the import session.
 
         :return: A msgspec struct containing the import session logs with the following structure:
 
             .. code-block:: python
 
                 ImportSessionLog(
-                    id='annotsess_1e433826-ab9c-402e-8b9a-a95d82f358f1', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                    id='annotsess_1e433826-ab9c-402e-8b9a-a95d82f358f1',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
                     logs=[]
                 )
 
         :example:
 
             .. code-block:: python
 
@@ -321,8 +328,9 @@
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                 project.annotations.retrieve_import_session_logs()
         """
         return self.requester.GET(
             f"/projects/{self.project_id}/annotationimportsessions/{self.import_session_id}/logs",
-            response_type=models.ImportSessionLog)
+            response_type=models.ImportSessionLog,
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/artifact.py` & `datature-1.7.0/datature/nexus/api/artifact.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,94 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   artifact.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Artifact API
-'''
+"""
 
-import time
 import json
+import time
 import zipfile
-from typing import Union
 from pathlib import Path
+from typing import Union
 
 import msgspec
-
-from datature.nexus.utils import utils
-from datature.nexus import models, error, config
+from datature.nexus import config, error, models
+from datature.nexus.api.types import (
+    ArtifactExportOptions,
+    ArtifactFilters,
+    OperationStatusOverview,
+)
 from datature.nexus.client_context import RestContext
-from datature.nexus.api.types import (OperationStatusOverview,
-                                      ArtifactExportOptions, ArtifactFilters)
+from datature.nexus.utils import utils
 
 
 class Artifact(RestContext):
     """Datature Artifact API Resource."""
 
-    def list(self,
-             filters: Union[ArtifactFilters, dict] = None,
-             include_exports: bool = False) -> models.Artifacts:
+    def list(
+        self,
+        filters: Union[ArtifactFilters, dict] = None,
+        include_exports: bool = False,
+    ) -> models.Artifacts:
         """Lists all artifacts in the project.
 
         :param filters: The filters to apply to the artifacts.
         :param include_exports: The boolean indication on whether to return the exported models.
         :return: A list of msgspec structs containing
             the artifact metadata with the following structure:
 
             .. code-block:: python
 
                 [Artifact(
-                    id='artifact_65ae274540259e2a07533532', 
-                    project_id='proj_ecfb4589d153999ba9ce01f54568fa72', 
-                    run_id='run_4a5d406d-464d-470c-bd7d-e92456621ad3', 
-                    flow_title='Test workflow', 
-                    artifact_name='ckpt-20', 
-                    create_date=1705912133684, 
-                    is_training=False, 
-                    step=5000, 
-                    is_deployed=False, 
+                    id='artifact_65ae274540259e2a07533532',
+                    project_id='proj_ecfb4589d153999ba9ce01f54568fa72',
+                    run_id='run_4a5d406d-464d-470c-bd7d-e92456621ad3',
+                    flow_title='Test workflow',
+                    artifact_name='ckpt-20',
+                    create_date=1705912133684,
+                    is_training=False,
+                    step=5000,
+                    is_deployed=False,
                     metric=ArtifactMetric(
-                        total_loss=0.32356, 
-                        classification_loss=0.012036, 
-                        localization_loss=0.010706, 
+                        total_loss=0.32356,
+                        classification_loss=0.012036,
+                        localization_loss=0.010706,
                         regularization_loss=0.0
-                    ), 
-                    model_name='fasterrcnn-inceptionv2-1024x1024', 
+                    ),
+                    model_name='fasterrcnn-inceptionv2-1024x1024',
                     export_options=[
                         ArtifactExportOptions(
-                            format='ONNX', 
+                            format='ONNX',
                             optimizations=ArtifactExportOptimizations(
                                 quantization=['float32', 'float16']
-                            ), 
+                            ),
                             default_optimizations=ArtifactExportOptimizations(
                                 quantization='float32'
                             )
-                        ), 
+                        ),
                         ArtifactExportOptions(
-                            format='TensorFlow', 
+                            format='TensorFlow',
                             optimizations=ArtifactExportOptimizations(
                                 quantization=['float32']
-                            ), 
+                            ),
                             default_optimizations=ArtifactExportOptimizations(
                                 quantization='float32'
                             )
-                        ), 
-                    ], 
+                        ),
+                    ],
                     exports=None
                 )]
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
@@ -102,85 +106,83 @@
         assert isinstance(filters, (ArtifactFilters, dict, type(None)))
 
         if isinstance(filters, dict):
             filters = ArtifactFilters(**filters)
         if filters is None:
             filters = ArtifactFilters()
 
-        return self.requester.GET(f"/projects/{self.project_id}/artifacts",
-                                  query={
-                                      "includeExports": include_exports,
-                                      **filters.to_json()
-                                  },
-                                  response_type=models.Artifacts)
-
-    def get(self,
-            artifact_id: str,
-            include_exports: bool = False) -> models.Artifact:
+        return self.requester.GET(
+            f"/projects/{self.project_id}/artifacts",
+            query={"includeExports": include_exports, **filters.to_json()},
+            response_type=models.Artifacts,
+        )
+
+    def get(self, artifact_id: str, include_exports: bool = False) -> models.Artifact:
         """Retrieves a specific artifact using the artifact ID.
 
         :param artifact_id: The ID of the artifact as a string.
         :param include_exports: The boolean indication on whether to return the exported models.
         :return: A msgspec struct containing the specific
             artifact metadata with the following structure:
 
             .. code-block:: python
 
                 Artifact(
-                    id='artifact_65ae274540259e2a07533532', 
-                    project_id='proj_ecfb4589d153999ba9ce01f54568fa72', 
-                    run_id='run_4a5d406d-464d-470c-bd7d-e92456621ad3', 
-                    flow_title='Test workflow', 
-                    artifact_name='ckpt-20', 
-                    create_date=1705912133684, 
-                    is_training=False, 
-                    step=5000, 
-                    is_deployed=False, 
+                    id='artifact_65ae274540259e2a07533532',
+                    project_id='proj_ecfb4589d153999ba9ce01f54568fa72',
+                    run_id='run_4a5d406d-464d-470c-bd7d-e92456621ad3',
+                    flow_title='Test workflow',
+                    artifact_name='ckpt-20',
+                    create_date=1705912133684,
+                    is_training=False,
+                    step=5000,
+                    is_deployed=False,
                     metric=ArtifactMetric(
-                        total_loss=0.32356, 
-                        classification_loss=0.012036, 
-                        localization_loss=0.010706, 
+                        total_loss=0.32356,
+                        classification_loss=0.012036,
+                        localization_loss=0.010706,
                         regularization_loss=0.0
-                    ), 
-                    model_name='fasterrcnn-inceptionv2-1024x1024', 
+                    ),
+                    model_name='fasterrcnn-inceptionv2-1024x1024',
                     export_options=[
                         ArtifactExportOptions(
-                            format='ONNX', 
+                            format='ONNX',
                             optimizations=ArtifactExportOptimizations(
                                 quantization=['float32', 'float16']
-                            ), 
+                            ),
                             default_optimizations=ArtifactExportOptimizations(
                                 quantization='float32'
                             )
-                        ), 
+                        ),
                         ArtifactExportOptions(
-                            format='TensorFlow', 
+                            format='TensorFlow',
                             optimizations=ArtifactExportOptimizations(
                                 quantization=['float32']
-                            ), 
+                            ),
                             default_optimizations=ArtifactExportOptimizations(
                                 quantization='float32'
                             )
-                        ), 
-                    ], 
+                        ),
+                    ],
                     exports=None
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.artifacts.get("artifact_63bd140e67b42dc9f431ffe2", include_exports=True)
         """
         return self.requester.GET(
             f"/projects/{self.project_id}/artifacts/{artifact_id}",
             query={"includeExports": include_exports},
-            response_type=models.Artifact)
+            response_type=models.Artifact,
+        )
 
     def list_exported_models(self, artifact_id: str) -> models.ArtifactModels:
         """Lists all exported models of a specific artifact.
 
         :param artifact_id: The ID of the artifact as a string.
         :return: A list of msgspec structs with the
             exported model metadata with the following structure:
@@ -209,92 +211,97 @@
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.artifacts.list_exported_models("artifact_63bd140e67b42dc9f431ffe2")
         """
         assert isinstance(artifact_id, str)
 
         return self.requester.GET(
             f"/projects/{self.project_id}/artifacts/{artifact_id}/exports",
-            response_type=models.ArtifactModels)
+            response_type=models.ArtifactModels,
+        )
 
-    def create_export(self,
-                      artifact_id: str,
-                      export_options: Union[ArtifactExportOptions, dict],
-                      background: bool = False) -> models.ArtifactModel:
+    def create_export(
+        self,
+        artifact_id: str,
+        export_options: Union[ArtifactExportOptions, dict],
+        background: bool = False,
+    ) -> models.ArtifactModel:
         """Exports an artifact model in a specific model format.
 
         :param artifact_id: The ID of the artifact as a string.
         :param export_options: The export options of the model.
 
         :return: A msgspec struct containing the operation
             metadata of the model export with the following structure:
 
             .. code-block:: python
 
                 ArtifactModel(
-                    id='model_15x95x513v9yrvvx2x329vvr34308w96', 
-                    artifact_id='artifact_656eb13aa533dcb05a020124', 
-                    status='Queued', 
-                    format='TensorFlow', 
+                    id='model_15x95x513v9yrvvx2x329vvr34308w96',
+                    artifact_id='artifact_656eb13aa533dcb05a020124',
+                    status='Queued',
+                    format='TensorFlow',
                     quantization='float32',
                     create_date=1701927649302,
                     download=None
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.artifacts.create_export(
-                    "artifact_63bd140e67b42dc9f431ffe2", 
+                    "artifact_63bd140e67b42dc9f431ffe2",
                     {
                         "format": "TensorFlow",
                     }
                 )
         """
         assert isinstance(artifact_id, str)
         assert isinstance(export_options, (ArtifactExportOptions, dict))
 
         if isinstance(export_options, dict):
             export_options = ArtifactExportOptions(**export_options)
 
         new_export = self.requester.POST(
             f"/projects/{self.project_id}/artifacts/{artifact_id}/exports",
             request_body=export_options.to_json(),
-            response_type=models.ArtifactModel)
+            response_type=models.ArtifactModel,
+        )
 
         if background:
             return new_export
 
         # Wait for the export to finish
         while True:
             exports = self.list_exported_models(artifact_id)
             for export in exports:
-                if (export.status == OperationStatusOverview.FINISHED.value
-                        and export.id == new_export.id):
+                if (
+                    export.status == OperationStatusOverview.FINISHED.value
+                    and export.id == new_export.id
+                ):
                     return new_export
             time.sleep(config.OPERATION_LOOPING_DELAY_SECONDS)
 
     def download_exported_model(
-            self,
-            model_id: str,
-            path: Union[str, Path, None] = None) -> models.LocalArtifact:
+        self, model_id: str, path: Union[str, Path, None] = None
+    ) -> models.LocalArtifact:
         """Download and unzip an artifact model to local path.
 
         :param model_id: The ID of the artifact exported model.
         :param path: The download path for the model, default current path.
 
         :return: A msgspec struct containing the download path of the model:
 
             .. code-block:: python
 
                 LocalArtifact(
-                    download_path='local', 
-                    model_filename='datature-yolov8l.pt', 
+                    download_path='local',
+                    model_filename='datature-yolov8l.pt',
                     label_filename='label_map.pbtxt'
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
@@ -314,41 +321,51 @@
         download_path = utils.get_download_path(path)
 
         for artifact in artifacts:
             if not artifact.exports:
                 continue
 
             for model in artifact.exports:
-                if (model.status == OperationStatusOverview.FINISHED.value
-                        and model_id in (model.id, model.id.split('_')[1])):
+                if (
+                    model.status == OperationStatusOverview.FINISHED.value
+                    and model_id in (model.id, model.id.split("_")[1])
+                ):
 
-                    download_tmpfile = utils.download_files_to_tempfile(
-                        model.download)
+                    download_tmpfile = utils.download_files_to_tempfile(model.download)
 
                     # Unzip the file
                     model_files = []
 
-                    with zipfile.ZipFile(download_tmpfile, 'r') as zip_ref:
+                    with zipfile.ZipFile(download_tmpfile, "r") as zip_ref:
                         zip_ref.extractall(download_path)
 
                         for file_name in zip_ref.namelist():
                             # Check if the file ends with the desired extension
                             if any(
-                                    file_name.endswith(ext)
-                                    for ext in [".onnx", ".tflite", ".pt"]):
+                                file_name.endswith(ext)
+                                for ext in [".onnx", ".tflite", ".pt"]
+                            ):
                                 model_files.append(file_name)
 
-                    return msgspec.json.decode(json.dumps({
-                        "download_path":
-                        str(download_path),
-                        "model_filename":
-                        "saved_model/"
-                        if model.format == 'TensorFlow' else model_files[0],
-                        "label_filename":
-                        "label.txt"
-                        if model.format == 'TFLite' else "label_map.pbtxt",
-                    }),
-                                               type=models.LocalArtifact)
+                    return msgspec.json.decode(
+                        json.dumps(
+                            {
+                                "download_path": str(download_path),
+                                "model_filename": (
+                                    "saved_model/"
+                                    if model.format == "TensorFlow"
+                                    else model_files[0]
+                                ),
+                                "label_filename": (
+                                    "label.txt"
+                                    if model.format == "TFLite"
+                                    else "label_map.pbtxt"
+                                ),
+                            }
+                        ),
+                        type=models.LocalArtifact,
+                    )
 
         # If didn't find the model key in the artifacts, raise an 404 error
         raise error.NotFoundError(
-            f"Model with id {model_id} not found, please export model first.")
+            f"Model with id {model_id} not found, please export model first."
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/asset/asset.py` & `datature-1.7.0/datature/nexus/api/asset/asset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   asset.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset API
-'''
+"""
 
-from typing import Optional, List, Union
+from typing import List, Optional, Union
 
 from datature.nexus import models
-from datature.nexus.api.operation import Operation
-from datature.nexus.api.types import AssetMetadata, Pagination, AssetFilter
 from datature.nexus.api.asset.upload_session import UploadSession
+from datature.nexus.api.operation import Operation
+from datature.nexus.api.types import AssetFilter, AssetMetadata, Pagination
 from datature.nexus.client_context import ClientContext, RestContext
 
 
 class Asset(RestContext):
     """Datature Annotation API Resource."""
 
     def __init__(self, client_context: ClientContext):
         """Initialize the API Resource."""
         super().__init__(client_context)
         self.operation = Operation(client_context)
 
     def list(
         self,
         pagination: Union[Pagination, dict, None] = None,
-        filters: Union[AssetFilter, dict, None] = None
+        filters: Union[AssetFilter, dict, None] = None,
     ) -> models.PaginationResponse[models.Asset]:
         """Retrieves a list of all assets in the project.
 
-        :param pagination: A dictionary containing the limit of 
-                            the number of assets to be returned in each page (defaults to 100), 
+        :param pagination: A dictionary containing the limit of
+                            the number of assets to be returned in each page (defaults to 100),
                             and the page cursor for page selection (defaults to the first page).
-        :param filters: A dictionary containing the filters of 
+        :param filters: A dictionary containing the filters of
                             the assets to be returned.
         :return: A msgspec struct of pagination response with the following structure:
 
                 .. code-block:: python
 
                     PaginationResponse(
-                        next_page='T2YAGDY1NWFlNDcyMzZkiMDYwMTQ5N2U2', 
-                        prev_page=None, 
+                        next_page='T2YAGDY1NWFlNDcyMzZkiMDYwMTQ5N2U2',
+                        prev_page=None,
                         data=[
                             Asset(
-                                id='asset_8208740a-2d9c-46e8-abb9-5777371bdcd3', 
-                                filename='boat180.png', 
-                                project='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                                id='asset_8208740a-2d9c-46e8-abb9-5777371bdcd3',
+                                filename='boat180.png',
+                                project='proj_cd067221d5a6e4007ccbb4afb5966535',
                                 status='None',
                                 create_date=1701927649302,
                                 url='',
                                 metadata=AssetMetadata(
-                                    file_size=186497, 
-                                    mime_type='image/png', 
-                                    height=243, 
-                                    width=400, 
-                                    groups=['main'], 
+                                    file_size=186497,
+                                    mime_type='image/png',
+                                    height=243,
+                                    width=400,
+                                    groups=['main'],
                                     custom_metadata={'captureAt': '2021-03-10T09:00:00Z'}
-                                ), 
+                                ),
                                 statistic=AssetAnnotationsStatistic(
-                                    tags_count=[], 
+                                    tags_count=[],
                                     total_annotations=0
                                 )
                             )
                         ]
                     )
 
         :example:
@@ -88,15 +88,15 @@
                             "status": "Annotated",
                             "groups": ["main"],
                         })
 
                         # or
                         project.assets.list(
                             nexus.ApiTypes.Pagination(
-                                limit= 2, 
+                                limit= 2,
                                 page="ZjYzYmJkM2FjN2UxOTA4ZmU0ZjE0Yjk5Mg"
                             ),
                             filters=nexus.ApiTypes.AssetFilter(status="Annotated", groups=["main"])
                         )
 
         """
         assert isinstance(pagination, (Pagination, dict, type(None)))
@@ -110,45 +110,43 @@
         if isinstance(filters, dict):
             filters = AssetFilter(**filters)
         if filters is None:
             filters = AssetFilter()
 
         return self.requester.GET(
             f"/projects/{self.project_id}/assets",
-            query={
-                **pagination.to_json(),
-                **filters.to_json()
-            },
-            response_type=models.PaginationResponse[models.Asset])
+            query={**pagination.to_json(), **filters.to_json()},
+            response_type=models.PaginationResponse[models.Asset],
+        )
 
     def get(self, asset_id_or_name: str) -> models.Asset:
         """Retrieves a specific asset using the asset ID or file name.
 
         :param asset_id_or_name: The ID or file name of the asset as a string.
         :return: A msgspec struct containing the metadata of one asset with the following structure:
 
                 .. code-block:: python
 
                         Asset(
-                            id='asset_8208740a-2d9c-46e8-abb9-5777371bdcd3', 
-                            filename='boat180.png', 
-                            project='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                            id='asset_8208740a-2d9c-46e8-abb9-5777371bdcd3',
+                            filename='boat180.png',
+                            project='proj_cd067221d5a6e4007ccbb4afb5966535',
                             status='None',
                             create_date=1701927649302,
                             url='',
                             metadata=AssetMetadata(
-                                file_size=186497, 
-                                mime_type='image/png', 
-                                height=243, 
-                                width=400, 
-                                groups=['main'], 
+                                file_size=186497,
+                                mime_type='image/png',
+                                height=243,
+                                width=400,
+                                groups=['main'],
                                 custom_metadata={'captureAt': '2021-03-10T09:00:00Z'}
-                            ), 
+                            ),
                             statistic=AssetAnnotationsStatistic(
-                                tags_count=[], 
+                                tags_count=[],
                                 total_annotations=0
                             )
                         )
 
         :example:
                 .. code-block:: python
 
@@ -156,43 +154,45 @@
 
                         project = Client("5aa41e8ba........").get_project("proj_b705a........")
                         project.assets.get("asset_6aea3395-9a72-4bb5-9ee0-19248c903c56")
         """
         assert isinstance(asset_id_or_name, str)
         return self.requester.GET(
             f"/projects/{self.project_id}/assets/{asset_id_or_name}",
-            response_type=models.Asset)
+            response_type=models.Asset,
+        )
 
-    def update(self, asset_id_or_name: str,
-               asset_meta: Union[AssetMetadata, dict]) -> models.Asset:
+    def update(
+        self, asset_id_or_name: str, asset_meta: Union[AssetMetadata, dict]
+    ) -> models.Asset:
         """Updates the metadata of a specific asset.
 
         :param asset_id_or_name: The ID or file name of the asset as a string.
         :param asset_meta: The new metadata of the asset to be updated.
         :return: A msgspec struct containing the metadata of one asset with the following structure:
 
                 .. code-block:: python
 
                         Asset(
-                            id='asset_f4dcb429-0332-4dd6-a1b4-fee794031ba6', 
-                            project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                            filename='boat194.png', 
+                            id='asset_f4dcb429-0332-4dd6-a1b4-fee794031ba6',
+                            project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                            filename='boat194.png',
                             status='None',
                             create_date=1701927649302,
-                            url='', 
+                            url='',
                             metadata=AssetMetadata(
-                                file_size=172676, 
-                                mime_type='image/png', 
-                                height=384, 
-                                width=422, 
-                                groups=['main'], 
+                                file_size=172676,
+                                mime_type='image/png',
+                                height=384,
+                                width=422,
+                                groups=['main'],
                                 custom_metadata={'captureAt': '2021-03-10T09:00:00Z'}
-                            ), 
+                            ),
                             statistic=AssetAnnotationsStatistic(
-                                tags_count=[], 
+                                tags_count=[],
                                 total_annotations=0
                             )
                         )
 
         :example:
                 .. code-block:: python
 
@@ -212,15 +212,16 @@
 
         if isinstance(asset_meta, dict):
             asset_meta = AssetMetadata(**asset_meta)
 
         return self.requester.PATCH(
             f"/projects/{self.project_id}/assets/{asset_id_or_name}",
             request_body=asset_meta.to_json(),
-            response_type=models.Asset)
+            response_type=models.Asset,
+        )
 
     def delete(self, asset_id_or_name: str) -> models.DeleteResponse:
         """Deletes a specific asset from the project.
 
         :param asset_id_or_name: The ID or file name of the asset as a string.
         :return: A msgspec struct containing the
             deleted asset ID and the deletion status with the following structure.
@@ -240,19 +241,20 @@
                         project.assets.delete(
                             "asset_6aea3395-9a72-4bb5-9ee0-19248c903c56",
                         )
         """
         assert isinstance(asset_id_or_name, str)
         return self.requester.DELETE(
             f"/projects/{self.project_id}/assets/{asset_id_or_name}",
-            response_type=models.DeleteResponse)
+            response_type=models.DeleteResponse,
+        )
 
-    def create_upload_session(self,
-                              groups: Optional[List[str]] = None,
-                              background: bool = False) -> UploadSession:
+    def create_upload_session(
+        self, groups: Optional[List[str]] = None, background: bool = False
+    ) -> UploadSession:
         """
         Creates a new upload session with specified
         groups and an option to run in the background.
 
         This method initializes and returns an UploadSession object,
         which can be used to manage file uploads within the system.
 
@@ -265,65 +267,63 @@
                 .. code-block:: python
 
                     from datature.nexus import Client
 
                     project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                     upload_session = project.assets.create_upload_session(
-                                                groups=["main"], 
+                                                groups=["main"],
                                                 background=True
                                             )
 
                     with upload_session as session:
                         # add assets path to upload session
                         upload_session.add_path(
-                            "folder/path/to/files", 
+                            "folder/path/to/files",
                             custom_metadata={"key": "value"}
                         )
 
                         upload_session.add_bytes(
-                            b"bytes/of/file", 
-                            "filename", 
+                            b"bytes/of/file",
+                            "filename",
                             custom_metadata={"key": "value"}
                         )
         """
         assert isinstance(groups, (list, type(None)))
         assert isinstance(background, bool)
 
         return UploadSession(self._context, groups, background)
 
-    def list_groups(self,
-                    groups: Union[List[str],
-                                  None] = None) -> models.AssetGroups:
+    def list_groups(self, groups: Union[List[str], None] = None) -> models.AssetGroups:
         """Retrieve asset statistics categorized by asset group and asset status.
 
         :param groups: A string array of name(s) of asset group(s).
         :return: A list of msgspec struct of
             the categorized asset statistics with the following structure:
 
                 .. code-block:: python
 
                         [
                             AssetGroup(
-                                group='1', 
+                                group='1',
                                 statistic=AssetGroupStatistic(
-                                    total_assets=1, 
-                                    annotated_assets=0, 
-                                    reviewed_assets=0, 
-                                    to_fixed_assets=0, 
+                                    total_assets=1,
+                                    annotated_assets=0,
+                                    reviewed_assets=0,
+                                    to_fixed_assets=0,
                                     completed_assets=0
                                 )
-                            ), 
+                            ),
                             AssetGroup(
-                                group='main', 
+                                group='main',
                                 statistic=AssetGroupStatistic(
-                                    total_assets=503, 
-                                    annotated_assets=0, 
-                                    reviewed_assets=0, 
-                                    to_fixed_assets=0, 
+                                    total_assets=503,
+                                    annotated_assets=0,
+                                    reviewed_assets=0,
+                                    to_fixed_assets=0,
                                     completed_assets=0
                                 )
                             )
                         ]
 
         :example:
 
@@ -332,10 +332,12 @@
                     from datature.nexus import Client
 
                     project = Client("5aa41e8ba........").get_project("proj_b705a........")
                     project.assets.list_groups()
         """
         assert isinstance(groups, (list, type(None)))
 
-        return self.requester.GET(f"/projects/{self.project_id}/assetgroups",
-                                  query={"group": groups},
-                                  response_type=models.AssetGroups)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/assetgroups",
+            query={"group": groups},
+            response_type=models.AssetGroups,
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/asset/upload_session.py` & `datature-1.7.0/datature/nexus/api/asset/upload_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   upload_session.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session
-'''
+"""
 # pylint: disable=R1732, R0902, E0203, W0201
 
-import struct
+import concurrent.futures
 import logging
+import struct
 import tempfile
 import threading
+from contextlib import ContextDecorator
 from os import path
 from pathlib import Path
-import concurrent.futures
-from contextlib import ContextDecorator
 from typing import List, Optional, Union
 
 import cv2
 import google_crc32c
 from filetype import filetype
 
-from datature.nexus.utils import utils
-from datature.nexus.utils import file_signature
-from datature.nexus import error, config
-from datature.nexus.medical import get_processor
+from datature.nexus import config, error
 from datature.nexus.api.operation import Operation
 from datature.nexus.api.types import OperationStatusOverview
 from datature.nexus.client_context import ClientContext, RestContext
+from datature.nexus.medical import get_processor
 from datature.nexus.models import UploadSession as UploadSessionModel
+from datature.nexus.utils import file_signature, utils
 
-logger = logging.getLogger("nexus")
+logger = logging.getLogger("datature-nexus")
 
 
 class UploadSession(RestContext, ContextDecorator):
     """Datature Asset Upload Session Class.
 
     :param client_context: An instance of ClientContext.
     :param groups: A list of group names to categorize the upload. Default is None.
-    :param background: 
+    :param background:
         A flag indicating whether the upload should run in the background. Default is False.
     """
 
-    def __init__(self,
-                 client_context: ClientContext,
-                 groups: Optional[List[str]] = None,
-                 background: bool = False):
+    def __init__(
+        self,
+        client_context: ClientContext,
+        groups: Optional[List[str]] = None,
+        background: bool = False,
+    ):
         """Initialize the API Resource."""
         super().__init__(client_context)
         self._local = threading.local()
 
         self._operation = None  # Lazy initialization if needed
         self.assets = []
         self.file_name_map = {}
@@ -70,23 +71,23 @@
     def operation(self):
         """Initialize operation."""
         if self._operation is None:
             self._operation = Operation(self._context)
         return self._operation
 
     def _init_http_session(self):
-        """ Initialize local session and retry policy. """
+        """Initialize local session and retry policy."""
 
         self._local.http_session = utils.init_gcs_upload_session()
 
     def __enter__(self):
         return self
 
     def __exit__(self, _exc_type, exc_val, _exc_tb):
-        """ Exit function.
+        """Exit function.
         The function will be called if an exception is raised inside the context manager
         """
         if exc_val is not None:
             # Error handling, patch import session status
             logger.warning("Upload session error existed: %s", exc_val)
             raise error.Error(exc_val)
 
@@ -104,15 +105,15 @@
 
         # Wait server finish generate thumbnail
         self.wait_until_done()
 
         return {"op_ids": self.operation_ids}
 
     def __len__(self):
-        """ Over write len function. """
+        """Over write len function."""
         return len(self.file_name_map)
 
     def add_path(self, file_path: str, custom_metadata: dict = None, **kwargs):
         """
         Add asset to upload.
 
         :param file_path: The path of the file to upload.
@@ -127,26 +128,26 @@
         else:
             file_paths = [file_path]
 
         # Convert DICOM and NII file to video asset
         processed_files = self._pre_process_medical_file(file_paths, kwargs)
 
         for processed_file in processed_files:
-            self._generate_metadata(processed_file.get("filename"),
-                                    processed_file.get("file_path"),
-                                    custom_metadata)
+            self._generate_metadata(
+                processed_file.get("filename"),
+                processed_file.get("file_path"),
+                custom_metadata,
+            )
             # check current asset size
             self._check_current_asset_size()
 
-    def add_bytes(self,
-                  file_bytes: bytes,
-                  filename: str,
-                  custom_metadata: dict = None,
-                  **kwargs):
-        """ Attach file in bytes to upload session 
+    def add_bytes(
+        self, file_bytes: bytes, filename: str, custom_metadata: dict = None, **kwargs
+    ):
+        """Attach file in bytes to upload session
 
         :param file_bytes: The bytes of the file to upload.
         :param filename: The name of the file to upload, should include the file extension.
         :param custom_metadata: A dictionary of custom metadata to attach to the asset.
         :param kwargs: Additional keyword arguments to pass to the API.
         """
         file_mime_type = file_signature.get_file_mime_by_signature(file_bytes)
@@ -157,63 +158,58 @@
         # Create a temporary directory
         temp_dir = tempfile.mkdtemp()
 
         # Create a temporary file path
         temp_file_path = path.join(temp_dir, filename)
 
         # Write file bytes to the temporary file
-        with open(temp_file_path, 'wb') as temp_file:
+        with open(temp_file_path, "wb") as temp_file:
             temp_file.write(file_bytes)
 
         # Convert DICOM and NII file to video asset
-        processed_files = self._pre_process_medical_file([temp_file_path],
-                                                         kwargs)
+        processed_files = self._pre_process_medical_file([temp_file_path], kwargs)
 
         for processed_file in processed_files:
-            self._generate_metadata(processed_file.get("filename"),
-                                    processed_file.get("file_path"),
-                                    custom_metadata)
+            self._generate_metadata(
+                processed_file.get("filename"),
+                processed_file.get("file_path"),
+                custom_metadata,
+            )
             # check current asset size
             self._check_current_asset_size()
 
     def _pre_process_medical_file(self, file_paths: str, options: dict = None):
         """Pre process the file, if medical file convert to MP4 first."""
         pre_processed_medical_file = []
 
         for file_path in file_paths:
-            if file_path.lower().endswith(('.dcm', '.nii')):
+            if file_path.lower().endswith((".dcm", ".nii")):
                 processor = get_processor(file_path)
 
                 process_data = {"file": file_path, "options": options}
                 processor.valid(process_data)
                 resp = processor.process(process_data)
 
                 if resp:
                     # change the converted file_path and filename
                     pre_processed_medical_file = pre_processed_medical_file + [
-                        {
-                            "filename": Path(file_path).stem,
-                            "file_path": file_path
-                        } for file_path in resp
+                        {"filename": Path(file_path).stem, "file_path": file_path}
+                        for file_path in resp
                     ]
             else:
-                pre_processed_medical_file.append({
-                    "filename":
-                    path.basename(file_path),
-                    "file_path":
-                    file_path
-                })
+                pre_processed_medical_file.append(
+                    {"filename": path.basename(file_path), "file_path": file_path}
+                )
         return pre_processed_medical_file
 
-    def _generate_metadata(self,
-                           filename: str,
-                           file_path: str,
-                           custom_metadata: dict = None):
+    def _generate_metadata(
+        self, filename: str, file_path: str, custom_metadata: dict = None
+    ):
         """process the file to asset metadata."""
-        with open(file_path, 'rb') as file:
+        with open(file_path, "rb") as file:
             contents = file.read()
 
             # calculate file crc32
             file_hash = google_crc32c.Checksum()
             file_hash.update(contents)
 
             # To fix the wrong crc32 caused by mac M1 clip
@@ -226,38 +222,35 @@
             file.close()
 
             if self.file_name_map.get(filename) is not None:
                 raise error.Error(
                     f"Cannot add multiple files with the same name, {filename}"
                 )
 
-            if (filename and size and crc32 and mime_kind):
+            if filename and size and crc32 and mime_kind:
                 if mime_kind.mime in ["image/jpeg", "image/png"]:
                     asset_metadata = {
                         "filename": filename,
                         "size": size,
                         "crc32c": crc32,
                         "mime": mime_kind.mime,
-                        "customMetadata": custom_metadata or {}
+                        "customMetadata": custom_metadata or {},
                     }
                 elif mime_kind.mime == "video/mp4":
                     cap = cv2.VideoCapture(file_path)
                     frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
 
                     asset_metadata = {
                         "filename": filename,
                         "size": size,
                         "crc32c": crc32,
                         "mime": mime_kind.mime,
                         "frames": frames,
-                        "encoder": {
-                            "profile": "h264Saver",
-                            "everyNthFrame": 1
-                        },
-                        "customMetadata": custom_metadata or {}
+                        "encoder": {"profile": "h264Saver", "everyNthFrame": 1},
+                        "customMetadata": custom_metadata or {},
                     }
                 else:
                     raise error.Error("UnSupported asset file")
 
                 self.assets.append(asset_metadata)
                 self.file_name_map[filename] = {"path": file_path}
 
@@ -270,35 +263,34 @@
         file_path = self.file_name_map.get(filename)["path"]
 
         # upload asset to GCP
         self._local.http_session.request(
             asset_upload.upload.method,
             asset_upload.upload.url,
             headers=asset_upload.upload.headers,
-            data=open(file_path, 'rb'),
-            timeout=config.REQUEST_TIME_OUT_SECONDS)
+            data=open(file_path, "rb"),
+            timeout=config.REQUEST_TIME_OUT_SECONDS,
+        )
         return filename
 
     def _upload_assets(self):
-        """ Use ThreadPoolExecutor to upload files to GCP."""
+        """Use ThreadPoolExecutor to upload files to GCP."""
         upload_session_response = self.requester.POST(
             f"/projects/{self.project_id}/assetuploadsessions",
-            request_body={
-                "groups": self.groups,
-                "assets": self.assets
-            },
-            response_type=UploadSessionModel)
+            request_body={"groups": self.groups, "assets": self.assets},
+            response_type=UploadSessionModel,
+        )
 
         # Use ThreadPoolExecutor to upload files in parallel
         with concurrent.futures.ThreadPoolExecutor(
-                initializer=self._init_http_session) as executor:
+            initializer=self._init_http_session
+        ) as executor:
             # Submit tasks to the executor
             futures = [
-                executor.submit(self._upload_file_thought_signed_url,
-                                asset_upload)
+                executor.submit(self._upload_file_thought_signed_url, asset_upload)
                 for asset_upload in upload_session_response.assets
             ]
 
             # Optionally, you can handle the results of the uploads here
             for future in futures:
                 filename = future.result()
 
@@ -306,16 +298,18 @@
 
             logger.debug("All files uploaded")
 
         return upload_session_response
 
     def wait_until_done(
         self,
-        raise_exception_if: Union[OperationStatusOverview,
-                                  str] = OperationStatusOverview.ERRORED):
+        raise_exception_if: Union[
+            OperationStatusOverview, str
+        ] = OperationStatusOverview.ERRORED,
+    ):
         """
         Wait for all operations to be done.
         This function only works when background is set to False.
         It functions the same as Operation.wait_until_done.
 
         :param raise_exception_if: The condition to raise error.
         :return: The operation status metadata if the operation has finished,
@@ -329,52 +323,55 @@
             logger.debug("All operations finished")
             return True
 
         # Use ThreadPoolExecutor to upload files in parallel
         with concurrent.futures.ThreadPoolExecutor() as executor:
             # Submit tasks to the executor
             futures = [
-                executor.submit(self.operation.wait_until_done,
-                                op_id,
-                                raise_exception_if=raise_exception_if)
+                executor.submit(
+                    self.operation.wait_until_done,
+                    op_id,
+                    raise_exception_if=raise_exception_if,
+                )
                 for op_id in self.operation_ids
             ]
 
             # Optionally, you can handle the results of the uploads here
             for future in futures:
                 res = future.result()
 
                 logger.debug("Finished operation: % s", res)
 
             logger.debug("All operations finished")
         return True
 
     # check current asset size
+
     def _check_current_asset_size(self):
         if len(self.assets) >= config.ASSET_UPLOAD_SESSION_BATCH_SIZE:
             upload_operation = self._upload_assets()
 
             self.operation_ids.append(upload_operation.op_id)
             # clear current batch
             self.assets = []
 
     def get_operation_ids(self):
         """
         A list of operation IDs. Because some dependency limits,
-        each operation allows a maximum of 5000 assets. 
-        So if the total number of assets goes up over 5000, 
+        each operation allows a maximum of 5000 assets.
+        So if the total number of assets goes up over 5000,
         it will return a list of operation IDs.
 
-        If you want to control the operations manually, 
+        If you want to control the operations manually,
         you can use this function to get the operation ids.
-        And the call project.operation.wait_until_done or project.operation.get 
+        And the call project.operation.wait_until_done or project.operation.get
         to wait for the operations to finish.
 
         :return: A list of operation ids.
 
         :example:
             .. code-block:: python
 
-                ['op_1', 'op_2', 'op_3']    
+                ['op_1', 'op_2', 'op_3']
 
         """
         return self.operation_ids
```

### Comparing `datature-1.6.0/datature/nexus/api/deployment.py` & `datature-1.7.0/datature/nexus/api/deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,139 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   Deploy.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Deploy API
-'''
+"""
 
 from typing import Union
 
 from datature.nexus import models
-from datature.nexus.client_context import RestContext
 from datature.nexus.api.types import DeploymentMetadata
+from datature.nexus.client_context import RestContext
 
 
 class Deployment(RestContext):
     """Datature Deploy API Resource."""
 
     def list(self) -> models.Deployments:
         """Lists all deployments in a project.
 
         :return: A list of msgspec structs containing
             deployment metadata with the following structure:
 
             .. code-block:: python
 
                 [Deployment(
-                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9', 
-                    name='My API', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                    artifact_id='artifact_65a7678a91afa7d22455c5ba', 
-                    version_tag='v1.0.0', 
+                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9',
+                    name='My API',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                    artifact_id='artifact_65a7678a91afa7d22455c5ba',
+                    version_tag='v1.0.0',
                     history_versions=[
                         DeploymentHistoryVersion(
-                            version_tag='v1.0.0', 
-                            artifact_id='artifact_65a7678a91afa7d22455c5ba', 
+                            version_tag='v1.0.0',
+                            artifact_id='artifact_65a7678a91afa7d22455c5ba',
                             update_date=1705475663570
                         )
-                    ], 
+                    ],
                     resources=DeploymentResources(
-                        cpu=4, 
-                        ram=8192, 
+                        cpu=4,
+                        ram=8192,
                         GPU_T4=None
-                    ), 
+                    ),
                     scaling=DeploymentScaling(
-                        replicas=1, 
+                        replicas=1,
                         mode='FixedReplicaCount'
-                    ), 
+                    ),
                     status=DeploymentStatus(
-                        overview='Available', 
+                        overview='Available',
                         message='Created service successfully',
                         update_data=1705475727032
-                    ), 
-                    create_date=1705475663570, 
-                    update_date=1705475727051, 
+                    ),
+                    create_date=1705475663570,
+                    update_date=1705475727051,
                     url='https://asia-inference.nip.io/1c144673-c757-40b4-8eeb-d400f0b9b2f9'
                 )]
 
         :example:
                 .. code-block:: python
 
                         from datature.nexus import Client
 
                         project = Client("5aa41e8ba........").get_project("proj_b705a........")
                         project.deployments.list()
         """
-        return self.requester.GET(f"/projects/{self.project_id}/deployments",
-                                  response_type=models.Deployments)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/deployments", response_type=models.Deployments
+        )
 
     def get(self, deploy_id: str) -> models.Deployment:
         """Retrieves a specific deployment using the deployment ID.
 
         :param deploy_id: The ID of the deployment as a string.
         :return: A msgspec struct containing the
             specific deployment metadata with the following structure:
 
             .. code-block:: python
 
                 Deployment(
-                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9', 
-                    name='My API', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                    artifact_id='artifact_65a7678a91afa7d22455c5ba', 
-                    version_tag='v1.0.0', 
+                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9',
+                    name='My API',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                    artifact_id='artifact_65a7678a91afa7d22455c5ba',
+                    version_tag='v1.0.0',
                     history_versions=[
                         DeploymentHistoryVersion(
-                            version_tag='v1.0.0', 
-                            artifact_id='artifact_65a7678a91afa7d22455c5ba', 
+                            version_tag='v1.0.0',
+                            artifact_id='artifact_65a7678a91afa7d22455c5ba',
                             update_date=1705475663570
                         )
-                    ], 
+                    ],
                     resources=DeploymentResources(
-                        cpu=4, 
-                        ram=8192, 
+                        cpu=4,
+                        ram=8192,
                         GPU_T4=None
-                    ), 
+                    ),
                     scaling=DeploymentScaling(
-                        replicas=1, 
+                        replicas=1,
                         mode='FixedReplicaCount'
-                    ), 
+                    ),
                     status=DeploymentStatus(
-                        overview='Available', 
+                        overview='Available',
                         message='Created service successfully',
                         update_data=1705475727032
-                    ), 
-                    create_date=1705475663570, 
-                    update_date=1705475727051, 
+                    ),
+                    create_date=1705475663570,
+                    update_date=1705475727051,
                     url='https://asia-inference.nip.io/1c144673-c757-40b4-8eeb-d400f0b9b2f9'
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.deployments.get("deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9")
         """
         assert isinstance(deploy_id, str)
         return self.requester.GET(
             f"/projects/{self.project_id}/deployments/{deploy_id}",
-            response_type=models.Deployment)
+            response_type=models.Deployment,
+        )
 
     def delete(self, deploy_id: str) -> models.DeleteResponse:
         """Deletes a specific deployment from the project.
 
         :param deploy_id: The id of the deployment.
         :return: A msgspec struct containing the deleted
             deployment ID and the deletion status with the following structure:
@@ -147,56 +149,55 @@
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.deployments.delete("deploy_30922d5e-b2f6-43dc-b7b4-e29e2c30fb45")
         """
         assert isinstance(deploy_id, str)
         return self.requester.DELETE(
             f"/projects/{self.project_id}/deployments/{deploy_id}",
-            response_type=models.DeleteResponse)
+            response_type=models.DeleteResponse,
+        )
 
-    def create(
-            self, deployment: Union[DeploymentMetadata,
-                                    dict]) -> models.Deployment:
+    def create(self, deployment: Union[DeploymentMetadata, dict]) -> models.Deployment:
         """Creates a deployment for a specific model using the model ID.
 
         :param deployment: The configuration metadata of the deployment.
         :return: A msgspec struct containing the specific
             deployment metadata with the following structure:
 
             .. code-block:: python
 
                 Deployment(
-                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9', 
-                    name='My API', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                    artifact_id='artifact_65a7678a91afa7d22455c5ba', 
-                    version_tag='v1.0.0', 
+                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9',
+                    name='My API',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                    artifact_id='artifact_65a7678a91afa7d22455c5ba',
+                    version_tag='v1.0.0',
                     history_versions=[
                         DeploymentHistoryVersion(
-                            version_tag='v1.0.0', 
-                            artifact_id='artifact_65a7678a91afa7d22455c5ba', 
+                            version_tag='v1.0.0',
+                            artifact_id='artifact_65a7678a91afa7d22455c5ba',
                             update_date=1705475663570
                         )
-                    ], 
+                    ],
                     resources=DeploymentResources(
-                        cpu=4, 
-                        ram=8192, 
+                        cpu=4,
+                        ram=8192,
                         GPU_T4=None
-                    ), 
+                    ),
                     scaling=DeploymentScaling(
-                        replicas=1, 
+                        replicas=1,
                         mode='FixedReplicaCount'
-                    ), 
+                    ),
                     status=DeploymentStatus(
-                        overview='Creating', 
+                        overview='Creating',
                         message='Creating service.',
                         update_data=1705475727032
-                    ), 
-                    create_date=1705475663570, 
-                    update_date=1705475727051, 
+                    ),
+                    create_date=1705475663570,
+                    update_date=1705475727051,
                     url=None
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
@@ -210,57 +211,59 @@
                 })
         """
         assert isinstance(deployment, (DeploymentMetadata, dict))
 
         if isinstance(deployment, dict):
             deployment = DeploymentMetadata(**deployment)
 
-        return self.requester.POST(f"/projects/{self.project_id}/deployments",
-                                   request_body=deployment.to_json(),
-                                   response_type=models.Deployment)
+        return self.requester.POST(
+            f"/projects/{self.project_id}/deployments",
+            request_body=deployment.to_json(),
+            response_type=models.Deployment,
+        )
 
     def update(
-            self, deploy_id: str,
-            deployment: Union[DeploymentMetadata, dict]) -> models.Deployment:
+        self, deploy_id: str, deployment: Union[DeploymentMetadata, dict]
+    ) -> models.Deployment:
         """Creates a deployment for a specific model using the model ID.
 
         :param deploy_id: The ID of the deployment as a string.
         :param deployment: The configuration metadata of the deployment.
         :return: A msgspec struct containing the
             specific deployment metadata with the following structure:
 
             .. code-block:: python
 
                 Deployment(
-                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9', 
+                    id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9',
                     name='My First API v2',
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                    artifact_id='artifact_65a7678a91afa7d22455c5ba', 
-                    version_tag='v1.0.0', 
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                    artifact_id='artifact_65a7678a91afa7d22455c5ba',
+                    version_tag='v1.0.0',
                     history_versions=[DeploymentHistoryVersion(
-                        version_tag='v1.0.0', 
-                        artifact_id='artifact_65a7678a91afa7d22455c5ba', 
+                        version_tag='v1.0.0',
+                        artifact_id='artifact_65a7678a91afa7d22455c5ba',
                         update_date=1705475663570
-                    )], 
+                    )],
                     resources=DeploymentResources(
-                        cpu=4, 
+                        cpu=4,
                         ram=8192,
                         GPU_T4=1
-                    ), 
+                    ),
                     scaling=DeploymentScaling(
-                        replicas=1, 
+                        replicas=1,
                         mode='FixedReplicaCount'
-                    ), 
+                    ),
                     status=DeploymentStatus(
-                        overview='Creating', 
-                        message='Creating service', 
+                        overview='Creating',
+                        message='Creating service',
                         update_data=1705475679244
                     ),
                     create_date=1705475663570,
-                    update_date=1705477694540, 
+                    update_date=1705477694540,
                     url=None
                 )
 
         :example:
 
             .. code-block:: python
 
@@ -284,62 +287,64 @@
 
         if isinstance(deployment, dict):
             deployment = DeploymentMetadata(**deployment)
 
         return self.requester.PATCH(
             f"/projects/{self.project_id}/deployments/{deploy_id}",
             request_body=deployment.to_json(),
-            response_type=models.Deployment)
+            response_type=models.Deployment,
+        )
 
-    def create_version(self, deploy_id: str, version_tag: str,
-                       artifact_id: str) -> models.Deployment:
+    def create_version(
+        self, deploy_id: str, version_tag: str, artifact_id: str
+    ) -> models.Deployment:
         """Updates a deployment version for a specific artifact using the artifact ID.
 
         :param deploy_id: The ID of the deployment as a string.
         :param version_tag: The new version tag name of the deployment.
         :param artifact_id: The ID of the artifact as a string.
         :return: A msgspec struct containing the specific
             deployment metadata with the following structure:
 
             .. code-block:: python
 
                 Deployment(
                     id='deploy_1c144673-c757-40b4-8eeb-d400f0b9b2f9',
-                    name='My API', 
+                    name='My API',
                     project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
-                    artifact_id='artifact_65a75d4891afa7d22455c54d', 
-                    version_tag='v2.0.0', 
+                    artifact_id='artifact_65a75d4891afa7d22455c54d',
+                    version_tag='v2.0.0',
                     history_versions=[
                         DeploymentHistoryVersion(
-                            version_tag='v1.0.0', 
+                            version_tag='v1.0.0',
                             artifact_id='artifact_65a7678a91afa7d22455c5ba',
                             update_date=1705475663570
-                        ), 
+                        ),
                         DeploymentHistoryVersion(
-                            version_tag='v2.0.0', 
-                            artifact_id='artifact_65a75d4891afa7d22455c54d', 
+                            version_tag='v2.0.0',
+                            artifact_id='artifact_65a75d4891afa7d22455c54d',
                             update_date=1705477973476
                         )
-                    ], 
+                    ],
                     resources=DeploymentResources(
-                        cpu=4, 
+                        cpu=4,
                         ram=8192,
                         GPU_T4=1
-                    ), 
+                    ),
                     scaling=DeploymentScaling(
-                        replicas=1, 
+                        replicas=1,
                         mode='FixedReplicaCount'
-                    ), 
+                    ),
                     status=DeploymentStatus(
-                        overview='Creating', 
-                        message='Creating service', 
+                        overview='Creating',
+                        message='Creating service',
                         update_data=1705475679244
                     ),
                     create_date=1705475663570,
-                    update_date=1705477694540, 
+                    update_date=1705477694540,
                     url=None
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
@@ -356,10 +361,11 @@
         assert isinstance(version_tag, str)
         assert isinstance(artifact_id, str)
 
         return self.requester.POST(
             f"/projects/{self.project_id}/deployments/{deploy_id}/versions",
             request_body={
                 "versionTag": version_tag,
-                'artifactId': artifact_id,
+                "artifactId": artifact_id,
             },
-            response_type=models.Deployment)
+            response_type=models.Deployment,
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/ontology.py` & `datature-1.7.0/datature/nexus/api/ontology.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   ontology.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Ontology API
-'''
+"""
 # pylint: disable=R0903
 
 from datature.nexus import models
 from datature.nexus.client_context import RestContext
 
 
 class Ontology(RestContext):
@@ -27,37 +27,38 @@
 
         :return: A msgspec struct containing
             the ontology metadata with the following structure:
 
             .. code-block:: json
 
                 [Ontology(
-                    id='ontology_843e486c-58d7-45a7-b722-f4948e204a56', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                    id='ontology_843e486c-58d7-45a7-b722-f4948e204a56',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
                     index=1,
                     name='person',
-                    color='#c1ff72', 
+                    color='#c1ff72',
                     description='TEST'
                     attributes=[OntologyAttribute(
-                      id='attri_d0877827-63d6-4794-b520-ef3e0c57ef71', 
-                      name='Tag Group', 
-                      description='', 
-                      type='Categorical', 
-                      required=True, 
+                      id='attri_d0877827-63d6-4794-b520-ef3e0c57ef71',
+                      name='Tag Group',
+                      description='',
+                      type='Categorical',
+                      required=True,
                       options=OntologyAttributeOptions(
                         categories=['person', 'dog']
-                      ), 
+                      ),
                       default=['person']
                     )]
                 )]
 
         :example:
             .. code-block:: python
 
             from datature.nexus import Client
 
             project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
             ontologies = project.ontologies.list_schemas()
         """
-        return self.requester.GET(f"/projects/{self.project_id}/ontologies",
-                                  response_type=models.Ontologies)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/ontologies", response_type=models.Ontologies
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/operation.py` & `datature-1.7.0/datature/nexus/api/operation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   operation.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Operation API
-'''
+"""
 
-import time
 import logging
-from typing import Union
+import time
 from datetime import datetime, timedelta
+from typing import Union
 
-from datature.nexus import error, config, models
-from datature.nexus.client_context import RestContext
+from datature.nexus import config, error, models
 from datature.nexus.api.types import OperationStatusOverview
+from datature.nexus.client_context import RestContext
 
-logger = logging.getLogger("nexus")
+logger = logging.getLogger("datature-nexus")
 
 
 class Operation(RestContext):
     """Datature Operation API Resource."""
 
     def get(self, op_id: str) -> models.Operation:
         """Retrieves an executed operation status using the operation link.
 
         :param op_id: The id of the operation as a string.
         :return: A msgspec struct containing the operation metadata with the following structure.
 
                 .. code-block:: python
 
                         Operation(
-                            id='op_d52ab4e6-7760-4d12-9c43-7fc1b8ce1616', 
-                            kind='nexus.annotations.export', 
+                            id='op_d52ab4e6-7760-4d12-9c43-7fc1b8ce1616',
+                            kind='nexus.annotations.export',
                             status=OperationStatus(
                                 overview='Finished',
-                                message='Operation finished', 
+                                message='Operation finished',
                                 progress=OperationProgress(
-                                    unit='whole operation', 
+                                    unit='whole operation',
                                     with_status=OperationProgressWithStatus(
-                                        Queued=0, 
-                                        Running=0, 
-                                        Finished=1, 
-                                        Cancelled=0, 
+                                        Queued=0,
+                                        Running=0,
+                                        Finished=1,
+                                        Cancelled=0,
                                         Errored=0
                                     )
                                 )
-                            ), 
+                            ),
                             create_date=1701927649302,
                             update_date=1701927649302
                         )
 
         :example:
                 .. code-block:: python
 
@@ -66,54 +66,56 @@
                         project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                         project.operations.get("op_508fc5d1-e908-486d-9e7b-1dca99b80024")
         """
         assert isinstance(op_id, str)
         return self.requester.GET(
             f"/projects/{self.project_id}/operations/{op_id}",
-            response_type=models.Operation)
+            response_type=models.Operation,
+        )
 
     def wait_until_done(
         self,
         op_id: str,
         timeout: int = config.OPERATION_LOOPING_TIMEOUT_SECONDS,
-        raise_exception_if: Union[OperationStatusOverview,
-                                  str] = OperationStatusOverview.ERRORED
+        raise_exception_if: Union[
+            OperationStatusOverview, str
+        ] = OperationStatusOverview.ERRORED,
     ) -> models.Operation:
         """Continuously retrieves an executed operation status for a
         specified number of times at a specified delay interval.
 
-        Can be used to poll a running operation to monitor execution status. 
+        Can be used to poll a running operation to monitor execution status.
 
         :param op_id: The id of the operation as a string.
         :param timeout: The maximum number of times to loop the operation retrieval.
         :param raise_exception_if: The condition to raise error.
         :return: The operation status metadata if the operation has finished,
             a BadRequestError if the operation has errored out,
             or None if the operation is still running.
 
                 .. code-block:: python
 
                     Operation(
-                        id='op_d52ab4e6-7760-4d12-9c43-7fc1b8ce1616', 
-                        kind='nexus.annotations.export', 
+                        id='op_d52ab4e6-7760-4d12-9c43-7fc1b8ce1616',
+                        kind='nexus.annotations.export',
                         status=OperationStatus(
                             overview='Finished',
-                            message='Operation finished', 
+                            message='Operation finished',
                             progress=OperationProgress(
-                                unit='whole operation', 
+                                unit='whole operation',
                                 with_status=OperationProgressWithStatus(
-                                    Queued=0, 
-                                    Running=0, 
-                                    Finished=1, 
-                                    Cancelled=0, 
+                                    Queued=0,
+                                    Running=0,
+                                    Finished=1,
+                                    Cancelled=0,
                                     Errored=0
                                 )
                             )
-                        ), 
+                        ),
                         create_date=1701927649302,
                         update_date=1701927649302
                     )
 
         :example:
                 .. code-block:: python
 
@@ -134,30 +136,35 @@
         timeout = timeout or config.OPERATION_LOOPING_TIMEOUT_SECONDS
         response = None
         elapsed_time = datetime.now() + timedelta(seconds=timeout)
 
         while True:
             response = self.requester.GET(
                 f"/projects/{self.project_id}/operations/{op_id}",
-                response_type=models.Operation)
+                response_type=models.Operation,
+            )
 
             logger.debug("Operation status: %s ", response.status)
 
             if response.status.overview == OperationStatusOverview.FINISHED.value:
                 return response
 
             if response.status.overview == raise_exception_if.value:
-                logger.warning("Operation %s %s: please contacts our support",
-                               raise_exception_if.value, op_id)
+                logger.warning(
+                    "Operation %s %s: please contacts our support",
+                    raise_exception_if.value,
+                    op_id,
+                )
 
                 raise error.BadRequestError(
                     f"Operation {raise_exception_if.value} {op_id}: please contacts our support"
                 )
 
             # if the operation has not finished when the timeouts
             if elapsed_time < datetime.now():
                 logger.warning(
                     "Operation timeout: please use operation.get(%s) to get the status",
-                    op_id)
+                    op_id,
+                )
                 return response
 
             time.sleep(config.OPERATION_LOOPING_DELAY_SECONDS)
```

### Comparing `datature-1.6.0/datature/nexus/api/project.py` & `datature-1.7.0/datature/nexus/api/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   project.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Project API
-'''
+"""
 # pylint: disable=R0902
 
 from abc import ABC
-from typing import Union
-from inspect import isclass
 from collections import ChainMap
+from inspect import isclass
+from typing import Union
 
-from datature.nexus.api.run import Run
-from datature.nexus.api.tag import Tag
-from datature.nexus.api.workflow import Workflow
+from datature.nexus import models
+from datature.nexus.api.annotation.annotation import Annotation
 from datature.nexus.api.artifact import Artifact
 from datature.nexus.api.asset.asset import Asset
-from datature.nexus.api.operation import Operation
 from datature.nexus.api.deployment import Deployment
-from datature.nexus.api.annotation.annotation import Annotation
 from datature.nexus.api.ontology import Ontology
-
-from datature.nexus import models
+from datature.nexus.api.operation import Operation
+from datature.nexus.api.run import Run
+from datature.nexus.api.tag import Tag
 from datature.nexus.api.types import ProjectMetadata
+from datature.nexus.api.workflow import Workflow
 from datature.nexus.client_context import ClientContext, RestContext
 
 
 class Project(ABC):
     """Datature Project API Resource."""
 
     _context: ClientContext
@@ -57,196 +56,206 @@
 
         # Init sub resources
         self._auto_init_resources()
 
     def _get_all_annotations(self):
         """Get annotations for this class and all superclasses."""
         # See https://stackoverflow.com/a/72037059.
-        return ChainMap(*(c.__annotations__ for c in self.__class__.__mro__
-                          if "__annotations__" in c.__dict__))
+        return ChainMap(
+            *(
+                c.__annotations__
+                for c in self.__class__.__mro__
+                if "__annotations__" in c.__dict__
+            )
+        )
 
     def _auto_init_resources(self):
         for name, type_annot in self._get_all_annotations().items():
 
             # Don't overwrite existing fields
             if hasattr(self, name):
                 continue
 
             # Only initialize if the type is a class and a subclass of RestContext
-            if (not isclass(type_annot)
-                    or not issubclass(type_annot, RestContext)):
+            if not isclass(type_annot) or not issubclass(type_annot, RestContext):
                 continue
 
             setattr(self, name, type_annot(self._context))
 
     def get_info(self) -> models.Project:
         """Retrieves project information.
 
         :return: A msgspec struct containing the projects with the following structure:
 
             .. code-block:: python
 
                 Project(
-                    id='proj_9004a21df7b040ace4674c4879603fe8', 
-                    name='keypoints', 
-                    workspace_id='ws_1c8aab980f174b0296c7e35e88665b13', 
+                    id='proj_9004a21df7b040ace4674c4879603fe8',
+                    name='keypoints',
+                    workspace_id='ws_1c8aab980f174b0296c7e35e88665b13',
                     type='ObjectDetection',
                     create_date=1701927649302,
-                    localization='MULTI', 
-                    tags=['cat faces'], 
-                    groups=['main', 'cats'], 
+                    localization='MULTI',
+                    tags=['cat faces'],
+                    groups=['main', 'cats'],
                     statistic=Statistic(
-                        tags_count=[TagsCountItem(name='cat faces', count=0)], 
-                        total_assets=28, 
-                        annotated_assets=0, 
+                        tags_count=[TagsCountItem(name='cat faces', count=0)],
+                        total_assets=28,
+                        annotated_assets=0,
                         total_annotations=0
                     )
                 )
 
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.get_info()
         """
-        project = self._context.requester.GET(f"/projects/{self.project_id}",
-                                              response_type=models.Project)
+        project = self._context.requester.GET(
+            f"/projects/{self.project_id}", response_type=models.Project
+        )
 
         return project
 
     def update(self, project: Union[ProjectMetadata, dict]) -> models.Project:
         """Updates the project with project meta fields.
 
         :param project: The new metadata of the project to be updated.
         :return: A msgspec struct containing the projects with the following structure:
 
             .. code-block:: python
 
                 Project(
-                    id='proj_9004a21df7b040ace4674c4879603fe8', 
-                    name='My Cool Project', 
-                    workspace_id='ws_1c8aab980f174b0296c7e35e88665b13', 
+                    id='proj_9004a21df7b040ace4674c4879603fe8',
+                    name='My Cool Project',
+                    workspace_id='ws_1c8aab980f174b0296c7e35e88665b13',
                     type='ObjectDetection',
                     create_date=1701927649302,
-                    localization='MULTI', 
-                    tags=['cat faces'], 
-                    groups=['main', 'cats'], 
+                    localization='MULTI',
+                    tags=['cat faces'],
+                    groups=['main', 'cats'],
                     statistic=Statistic(
-                        tags_count=[TagsCountItem(name='cat faces', count=0)], 
-                        total_assets=28, 
-                        annotated_assets=0, 
+                        tags_count=[TagsCountItem(name='cat faces', count=0)],
+                        total_assets=28,
+                        annotated_assets=0,
                         total_annotations=0
                     )
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client, ApiTypes
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                 project.update({"name":"My Cool Project"})
-                // Or 
+                // Or
                 project.update(ApiTypes.ProjectMetadata(name="My Cool Project"))
         """
         assert isinstance(project, (ProjectMetadata, dict))
 
         if isinstance(project, dict):
             project = ProjectMetadata(**project)
 
-        return self.requester.PATCH(f"/projects/{self.project_id}",
-                                    request_body=project.to_json(),
-                                    response_type=models.Project)
+        return self.requester.PATCH(
+            f"/projects/{self.project_id}",
+            request_body=project.to_json(),
+            response_type=models.Project,
+        )
 
     def list_insights(self) -> models.ProjectInsights:
         """Retrieves project insight and metrics of the completed training runs.
 
-        :return: A msgspec struct containing 
+        :return: A msgspec struct containing
             the project insights metadata with the following structure:
 
             .. code-block:: python
 
                 [ProjectInsight(
-                    flow_title='Test workflow', 
-                    run_id='run_4a5d406d-464d-470c-bd7d-e92456621ad3', 
+                    flow_title='Test workflow',
+                    run_id='run_4a5d406d-464d-470c-bd7d-e92456621ad3',
                     dataset=InsightDataset(
-                        data_type='Rectangle', 
-                        num_classes=1, 
-                        average_annotations=5.19, 
-                        total_assets=500, 
+                        data_type='Rectangle',
+                        num_classes=1,
+                        average_annotations=5.19,
+                        total_assets=500,
                         settings=DatasetSettings(
-                            split_ratio=0.3, 
-                            shuffle=True, 
-                            seed=0, 
+                            split_ratio=0.3,
+                            shuffle=True,
+                            seed=0,
                             using_sliding_window=False
                         )
-                    ), 
+                    ),
                     model=InsightModel(
-                        name='fasterrcnn-inceptionv2-1024x1024', 
-                        batch_size=2, 
-                        training_steps=5000, 
-                        max_detection_per_class=100, 
-                        solver='momentum', 
-                        learning_rate=0.04, 
+                        name='fasterrcnn-inceptionv2-1024x1024',
+                        batch_size=2,
+                        training_steps=5000,
+                        max_detection_per_class=100,
+                        solver='momentum',
+                        learning_rate=0.04,
                         momentum=0.9
-                    ), 
+                    ),
                     checkpoint=RunCheckpoint(
-                        strategy='STRAT_ALWAYS_SAVE_LATEST', 
-                        evaluation_interval=250, 
+                        strategy='STRAT_ALWAYS_SAVE_LATEST',
+                        evaluation_interval=250,
                         metric=None
-                    ), 
+                    ),
                     artifact=InsightArtifact(
-                        id='artifact_65ae274540259e2a07533532', 
-                        is_training=False, 
-                        step=5000, 
+                        id='artifact_65ae274540259e2a07533532',
+                        is_training=False,
+                        step=5000,
                         metric=ArtifactMetric(
-                            total_loss=0.32356, 
-                            classification_loss=0.012036, 
-                            localization_loss=0.010706, 
+                            total_loss=0.32356,
+                            classification_loss=0.012036,
+                            localization_loss=0.010706,
                             regularization_loss=0.0
                         )
                     ),
                     create_date=1705912133684
                 )]
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.list_insights()
         """
-        return self.requester.GET(f"/projects/{self.project_id}/insights",
-                                  response_type=models.ProjectInsights)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/insights",
+            response_type=models.ProjectInsights,
+        )
 
     def list_users(self) -> models.ProjectUsers:
-        """Retrieves all users in the project. 
+        """Retrieves all users in the project.
             This includes Project Owners, Collaborators and Datature Experts.
 
         :return: A list of msgspec struct containing
             the project user metadata with the following structure:
 
             .. code-block:: python
 
                 [ProjectUser(
-                    id='user_6323fea23e292439f31c58cd', 
+                    id='user_6323fea23e292439f31c58cd',
                     access_type='Owner',
-                    email='raighne@datature.io', 
-                    nickname='raighne', 
+                    email='raighne@datature.io',
+                    nickname='raighne',
                     picture='https://s.gravatar.com/avatar/avatars%2Fra.png'
                 )]
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.list_users()
         """
-        return self.requester.GET(f"/projects/{self.project_id}/users",
-                                  response_type=models.ProjectUsers)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/users", response_type=models.ProjectUsers
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/run.py` & `datature-1.7.0/datature/nexus/api/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,154 +1,156 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   run.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Run API
-'''
+"""
 
 from typing import Union
 
 from datature.nexus import models
-from datature.nexus.client_context import RestContext
 from datature.nexus.api.types import RunSetupMetadata
+from datature.nexus.client_context import RestContext
 
 
 class Run(RestContext):
     """Datature Run API Resource."""
 
     def list(self) -> models.Runs:
         """Lists all training runs regardless of status.
 
         :return: A list of msgspec structs containing
             the training run metadata with the following structure:
 
             .. code-block:: python
 
                 [Run(
-                    id='run_610ba26c-6fbb-42eb-b838-839c61b68b26', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                    id='run_610ba26c-6fbb-42eb-b838-839c61b68b26',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
                     flow_id='flow_63bbd3bf8a78eb906f417396',
                     execution=RunExecution(
                         accelerator=RunAccelerator(name='GPU_T4', count=1),
                         checkpoint=RunCheckpoint(
-                            strategy='STRAT_ALWAYS_SAVE_LATEST', 
-                            evaluation_interval=250, 
+                            strategy='STRAT_ALWAYS_SAVE_LATEST',
+                            evaluation_interval=250,
                             metric=None
                         ),
                         limit=RunLimit(metric='LIM_NONE', value=0)
                     ),
                     features=RunFeatures(preview=True, matrix=True, using_sliding_window=False),
                     status=RunStatus(
-                        overview='Creating', 
-                        message='Creating service.', 
+                        overview='Creating',
+                        message='Creating service.',
                         update_data=1705466384796
-                    ), 
-                    create_date=1705466384796, 
-                    update_date=1705466392067, 
+                    ),
+                    create_date=1705466384796,
+                    update_date=1705466392067,
                     log_ids=['runlog_UjYxMGJhMjZjLTZmYmItNDJlYi1iODM4LTgzOWM2MWI2OGIyNg']
                 )]
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                 project.runs.list()
         """
-        return self.requester.GET(f"/projects/{self.project_id}/runs",
-                                  response_type=models.Runs)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/runs", response_type=models.Runs
+        )
 
     def get(self, run_id: str) -> models.Run:
         """Retrieves a specific training run using the run ID.
 
         :param run_id: The ID of the training run.
         :return: A msgspec struct containing the specific
             training run metadata with the following structure:
 
             .. code-block:: python
 
                 Run(
-                    id='run_610ba26c-6fbb-42eb-b838-839c61b68b26', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
+                    id='run_610ba26c-6fbb-42eb-b838-839c61b68b26',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
                     flow_id='flow_63bbd3bf8a78eb906f417396',
                     execution=RunExecution(
                         accelerator=RunAccelerator(name='GPU_T4', count=1),
                         checkpoint=RunCheckpoint(
-                            strategy='STRAT_ALWAYS_SAVE_LATEST', 
-                            evaluation_interval=250, 
+                            strategy='STRAT_ALWAYS_SAVE_LATEST',
+                            evaluation_interval=250,
                             metric=None
                         ),
                         limit=RunLimit(metric='LIM_NONE', value=0)
                     ),
                     features=RunFeatures(preview=True, matrix=True, using_sliding_window=False),
                     status=RunStatus(
-                        overview='Creating', 
-                        message='Creating service.', 
+                        overview='Creating',
+                        message='Creating service.',
                         update_data=1705466384796
-                    ), 
-                    create_date=1705466384796, 
-                    update_date=1705466392067, 
+                    ),
+                    create_date=1705466384796,
+                    update_date=1705466392067,
                     log_ids=['runlog_UjYxMGJhMjZjLTZmYmItNDJlYi1iODM4LTgzOWM2MWI2OGIyNg']
                 )
 
         :example:
             .. code-block:: python
 
                     from datature.nexus import Client
 
                     project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                     project.runs.get("run_610ba26c-6fbb-42eb-b838-839c61b68b26")
         """
         assert isinstance(run_id, str)
 
-        return self.requester.GET(f"/projects/{self.project_id}/runs/{run_id}",
-                                  response_type=models.Run)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/runs/{run_id}", response_type=models.Run
+        )
 
     def kill(self, run_id: str) -> models.Run:
         """Kills a specific training run using the run ID.
 
         :param run_id: The ID of the training run.
         :return: A msgspec struct containing the
             killed training metadata with the following structure:
 
             .. code-block:: python
 
                 Run(
-                    id='run_e2a14cee-eacc-4335-bc95-94c3ee196b04', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                    flow_id='flow_64e812a7e47592ef374cbbc2', 
+                    id='run_e2a14cee-eacc-4335-bc95-94c3ee196b04',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                    flow_id='flow_64e812a7e47592ef374cbbc2',
                     execution=RunExecution(
-                        accelerator=RunAccelerator(name='GPU_L4', count=1), 
+                        accelerator=RunAccelerator(name='GPU_L4', count=1),
                         checkpoint=RunCheckpoint(
-                            strategy='STRAT_LOWEST_VALIDATION_LOSS', 
-                            evaluation_interval=220, 
+                            strategy='STRAT_LOWEST_VALIDATION_LOSS',
+                            evaluation_interval=220,
                             metric='Loss/total_loss'
-                        ), 
+                        ),
                         limit=RunLimit(metric='LIM_NONE', value=0)
-                    ), 
+                    ),
                     status=RunStatus(
                         overview='Cancelled',
                         message='Training cancelled.',
                         update_data=1700204316180
                     ),
                     create_date=1701927649302,
                     update_date=1701927649302,
-                    features=RunFeatures(preview=True, matrix=True), 
+                    features=RunFeatures(preview=True, matrix=True),
                     log_ids=['runlog_UmUyYTE0Y2VlLWVhY2MtNDMzNS1iYzk1LTk0YzNlZTE5NmIwNA']
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
@@ -158,48 +160,48 @@
                 project.runs.kill("run_63eb212ff0f856bf95085095")
         """
         assert isinstance(run_id, str)
 
         return self.requester.PATCH(
             f"/projects/{self.project_id}/runs/{run_id}",
             request_body={"status": "Cancelled"},
-            response_type=models.Run)
+            response_type=models.Run,
+        )
 
-    def start(self, flow_id: str, setup: Union[RunSetupMetadata,
-                                               dict]) -> models.Run:
+    def start(self, flow_id: str, setup: Union[RunSetupMetadata, dict]) -> models.Run:
         """Starts a new training run from a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow.
         :param setup: The metadata of the training.
         :return: A msgspec struct containing the
             newly-initialized training run metadata with the following structure:
 
             .. code-block:: python
 
                 Run(
-                    id='run_e2a14cee-eacc-4335-bc95-94c3ee196b04', 
-                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                    flow_id='flow_64e812a7e47592ef374cbbc2', 
+                    id='run_e2a14cee-eacc-4335-bc95-94c3ee196b04',
+                    project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                    flow_id='flow_64e812a7e47592ef374cbbc2',
                     execution=RunExecution(
-                        accelerator=RunAccelerator(name='GPU_L4', count=1), 
+                        accelerator=RunAccelerator(name='GPU_L4', count=1),
                         checkpoint=RunCheckpoint(
-                            strategy='STRAT_LOWEST_VALIDATION_LOSS', 
-                            evaluation_interval=220, 
+                            strategy='STRAT_LOWEST_VALIDATION_LOSS',
+                            evaluation_interval=220,
                             metric='Loss/total_loss'
-                        ), 
+                        ),
                         limit=RunLimit(metric='LIM_NONE', value=0)
-                    ), 
+                    ),
                     status=RunStatus(
                         overview='Creating',
                         message='Training starting.',
                         update_data=1700204316180
                     ),
                     create_date=1701927649302,
                     update_date=1701927649302,
-                    features=RunFeatures(preview=True, matrix=True), 
+                    features=RunFeatures(preview=True, matrix=True),
                     log_ids=['runlog_UmUyYTE0Y2VlLWVhY2MtNDMzNS1iYzk1LTk0YzNlZTE5NmIwNA']
                 )
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
@@ -225,56 +227,51 @@
         """
         assert isinstance(flow_id, str)
         assert isinstance(setup, (RunSetupMetadata, dict))
 
         if isinstance(setup, dict):
             setup = RunSetupMetadata(**setup)
 
-        return self.requester.POST(f"/projects/{self.project_id}/runs",
-                                   request_body={
-                                       "flowId": flow_id,
-                                       "execution": {
-                                           "accelerator":
-                                           setup.accelerator.to_json(),
-                                           "checkpoint":
-                                           setup.checkpoint.to_json(),
-                                           "limit":
-                                           setup.limit.to_json(),
-                                           "debug":
-                                           setup.debug
-                                       },
-                                       "features": {
-                                           "preview": setup.matrix,
-                                           "matrix": setup.matrix
-                                       }
-                                   },
-                                   response_type=models.Run)
+        return self.requester.POST(
+            f"/projects/{self.project_id}/runs",
+            request_body={
+                "flowId": flow_id,
+                "execution": {
+                    "accelerator": setup.accelerator.to_json(),
+                    "checkpoint": setup.checkpoint.to_json(),
+                    "limit": setup.limit.to_json(),
+                    "debug": setup.debug,
+                },
+                "features": {"preview": setup.matrix, "matrix": setup.matrix},
+            },
+            response_type=models.Run,
+        )
 
     def get_logs(self, log_id: str) -> models.RunLogs:
         """
         Retrieves a specific training log using the log ID.
 
         :param log_id: The ID of the training log.
         :return: A msgspec struct with the specific
             training log metadata with the following structure:
 
             .. code-block:: python
 
                 RunLogs(
-                    id='runlog_UmUyYTE0Y2VlLWVhY2MtNDMzNS1iYzk1LTk0YzNlZTE5NmIwNA', 
+                    id='runlog_UmUyYTE0Y2VlLWVhY2MtNDMzNS1iYzk1LTk0YzNlZTE5NmIwNA',
                     logs=[
                         {
-                            'ev': 'trainingCheckpoint', 
-                            't': 1700200466147, 
+                            'ev': 'trainingCheckpoint',
+                            't': 1700200466147,
                             'pl': {
-                                'step': 0, 
+                                'step': 0,
                                 'log': 'Step 0, totalLoss: 6.4055E+01, boxLoss: 5.3928E+00, classificationLoss: 5.2646E+01, distributedFocalLoss: 6.0163E+00.',
-                                'totalLoss': 64.055, 
+                                'totalLoss': 64.055,
                                 'boxLoss': 5.3928,
-                                'classificationLoss': 52.646, 
+                                'classificationLoss': 52.646,
                                 'distributedFocalLoss': 6.0163
                             }
                         }
                     ]
                 )
 
         :example:
@@ -285,15 +282,16 @@
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                 project.runs.get_logs("runlog_63eb212ff0f856bf95085095")
         """
         assert isinstance(log_id, str)
         return self.requester.GET(
             f"/projects/{self.project_id}/runs/logs/{log_id}",
-            response_type=models.RunLogs)
+            response_type=models.RunLogs,
+        )
 
     def get_confusion_matrix(self, run_id: str) -> models.RunConfusionMatrix:
         """Retrieves a training confusion matrix using the run ID.
 
         :param run_id: The ID of the training run.
         :return: A msgspec struct containing the specific
             training matrix json string with the following structure:
@@ -312,8 +310,9 @@
 
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.runs.get_confusion_matrix("run_63eb212ff0f856bf95085095")
         """
         assert isinstance(run_id, str)
         return self.requester.GET(
             f"/projects/{self.project_id}/runs/{run_id}/confusionMatrix",
-            response_type=models.RunConfusionMatrix)
+            response_type=models.RunConfusionMatrix,
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/tag.py` & `datature-1.7.0/datature/nexus/api/tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   tag.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Tag API
-'''
+"""
 
 from typing import Union
 
 from datature.nexus import models
 from datature.nexus.api.types import TagMetadata
 from datature.nexus.client_context import RestContext
 
@@ -28,51 +28,52 @@
         """Lists all tags in the project.
 
         :return: A msgspec struct containing tag metadata with the following structure:
 
             .. code-block:: python
 
                 [Tag(
-                    index=0, 
-                    name='Platelets', 
+                    index=0,
+                    name='Platelets',
                     color=None,
                     description=None
                 )]
 
         :example:
                 .. code-block:: python
 
                         from datature.nexus import Client
 
                         project = Client("5aa41e8ba........").get_project("proj_b705a........")
                         project.tags.list()
         """
-        return self.requester.GET(f"/projects/{self.project_id}/tags",
-                                  response_type=models.Tags)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/tags", response_type=models.Tags
+        )
 
     def create(self, metadata: Union[TagMetadata, dict]) -> models.Tags:
-        """Creates a new tag. 
+        """Creates a new tag.
             The indices of new tags created will begin from the last existing tag index.
 
         :param metadata: The metadata of the new tag.
         :return: An updated msgspec struct containing tag metadata with the following structure:
 
             .. code-block:: python
 
                 [
                     Tag(
-                        index=0, 
-                        name='boat', 
-                        color='#7ed957', 
+                        index=0,
+                        name='boat',
+                        color='#7ed957',
                         description='boat'
-                    ), 
+                    ),
                     Tag(
-                        index=1, 
-                        name='boat2', 
-                        color='#ff3131', 
+                        index=1,
+                        name='boat2',
+                        color='#ff3131',
                         description=None
                     )
                 ]
 
 
         :example:
             .. code-block:: python
@@ -82,48 +83,49 @@
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                 project.tags.create({"name": "boat2", "color": "#ff3131"}
 
                 # or
                 project.tags.create(ApiTypes.TagMetadata(
                                         name="boat2",
-                                        color="#ff3131", 
+                                        color="#ff3131",
                                         description="This is a boat"
-                                    )) 
+                                    ))
         """
         assert isinstance(metadata, (TagMetadata, dict))
 
         if isinstance(metadata, dict):
             metadata = TagMetadata(**metadata)
 
-        return self.requester.POST(f"/projects/{self.project_id}/tags",
-                                   request_body=metadata.to_json(),
-                                   response_type=models.Tags)
+        return self.requester.POST(
+            f"/projects/{self.project_id}/tags",
+            request_body=metadata.to_json(),
+            response_type=models.Tags,
+        )
 
-    def update(self, index: int, metadata: Union[TagMetadata,
-                                                 dict]) -> models.Tags:
+    def update(self, index: int, metadata: Union[TagMetadata, dict]) -> models.Tags:
         """Updates the name of a specific tag using the tag index.
 
         :param index: The index of the tag to update.
         :param metadata: The new metadata of the tag.
         :return: An updated msgspec struct containing tag metadata with the following structure:
 
             .. code-block:: python
 
                 [
                     Tag(
-                        index=0, 
-                        name='boat', 
-                        color='#7ed957', 
+                        index=0,
+                        name='boat',
+                        color='#7ed957',
                         description='boat'
-                    ), 
+                    ),
                     Tag(
-                        index=1, 
-                        name='tagName', 
-                        color='#ff3131', 
+                        index=1,
+                        name='tagName',
+                        color='#ff3131',
                         description=None
                     )
                 ]
 
         :example:
                 .. code-block:: python
 
@@ -138,18 +140,19 @@
 
         if isinstance(metadata, dict):
             metadata = TagMetadata(**metadata)
 
         return self.requester.PATCH(
             f"/projects/{self.project_id}/tags/{index}",
             request_body=metadata.to_json(),
-            response_type=models.Tags)
+            response_type=models.Tags,
+        )
 
     def delete(self, index: int) -> models.DeleteResponse:
-        """Deletes a specific tag using the tag index. 
+        """Deletes a specific tag using the tag index.
             The tag indices of other tags will be left unchanged.
             The indices of new tags created will begin from the last existing tag index.
 
         :param index: The index of the tag.
         :return: A msgspec struct containing the deletion
             status of the tag with the following structure:
 
@@ -165,30 +168,31 @@
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                 project.tags.delete(1)
         """
         assert isinstance(index, int)
         return self.requester.DELETE(
             f"/projects/{self.project_id}/tags/{index}",
-            response_type=models.DeleteResponse)
+            response_type=models.DeleteResponse,
+        )
 
     def merge(self, index: int, target_index: int) -> models.Tags:
         """Merges a tag into another tag. .
 
         :param index: The index of the tag to merge.
         :param target_index: The index of the tag to merge into.
         :return: An updated msgspec struct containing tag
             metadata with the following structure:
 
             .. code-block:: python
 
                 [Tag(
-                    index=0, 
+                    index=0,
                     name='boat',
-                    color='#7ed957', 
+                    color='#7ed957',
                     description='boat'
                 )]
 
         :example:
             .. code-block:: python
 
                 from datature.nexus import Client
@@ -197,8 +201,9 @@
                 project.tags.merge(1, 0)
         """
         assert isinstance(index, int)
         assert isinstance(target_index, int)
 
         return self.requester.POST(
             f"/projects/{self.project_id}/tags/{index}-{target_index}:merge",
-            response_type=models.Tags)
+            response_type=models.Tags,
+        )
```

### Comparing `datature-1.6.0/datature/nexus/api/types.py` & `datature-1.7.0/datature/nexus/api/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   types.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Types for Datature API resources.
-'''
+"""
 # pylint: disable=R0902,C0103,W0212
 
-from typing import Union, List
-from enum import Enum, unique
 from dataclasses import dataclass
+from enum import Enum, unique
+from typing import List, Union
 
 
 def add_mapping(enum_cls):
     """Add Mapping to Type."""
 
     for key, value in enum_cls.__MAPPING__.items():
         enum_cls._member_map_[key] = value
@@ -34,15 +34,15 @@
 
     :param name: The name of the project.
     """
 
     name: str
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         return {
             "name": self.name,
         }
 
 
 @add_mapping
 @unique
@@ -154,16 +154,15 @@
         "None": NONE,
     }
 
 
 @add_mapping
 @unique
 class OperationStatusOverview(Enum):
-    """Operation Status. 
-    """
+    """Operation Status."""
 
     QUEUED = "Queued"
     RUNNING = "Running"
     FINISHED = "Finished"
     CANCELLED = "Cancelled"
     ERRORED = "Errored"
 
@@ -175,16 +174,15 @@
         "Errored": ERRORED,
     }
 
 
 @add_mapping
 @unique
 class DeploymentStatusOverview(Enum):
-    """Deployment Status. 
-    """
+    """Deployment Status."""
 
     CREATING = "Creating"
     UPDATING = "Updating"
     REMOVING = "Removing"
     AVAILABLE = "Available"
     ERRORED = "Errored"
 
@@ -196,16 +194,16 @@
         "Errored": ERRORED,
     }
 
 
 @add_mapping
 @unique
 class RunStatusOverview(Enum):
-    """Run Status. 
-    """
+    """Run Status."""
+
     CREATING = "Creating"
     RUNNING = "Running"
     FINISHED = "Finished"
     ERRORED = "Errored"
     CANCELLED = "Cancelled"
 
     __MAPPING__ = {
@@ -216,28 +214,28 @@
         "Cancelled": CANCELLED,
     }
 
 
 @add_mapping
 @unique
 class ModelFormat(Enum):
-    """Artifact supported Models Format. 
-    """
+    """Artifact supported Models Format."""
+
     TENSORFLOW = "TensorFlow"
     TFLITE = "TFLite"
     ONNX = "ONNX"
     PYTORCH = "PyTorch"
     COREML = "CoreML"
 
     __MAPPING__ = {
         "TensorFlow": TENSORFLOW,
         "TFLite": TFLITE,
         "ONNX": ONNX,
         "PyTorch": PYTORCH,
-        "CoreML": COREML
+        "CoreML": COREML,
     }
 
 
 @dataclass
 class AnnotationMetadata:
     """Annotation metadata.
 
@@ -254,15 +252,15 @@
     bound: list
 
     def __post_init__(self):
         if isinstance(self.bound_type, str):
             self.bound_type = BoundType(self.bound_type)
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         return {
             "assetId": self.asset_id,
             "tag": self.tag,
             "boundType": self.bound_type.value,
             "bound": self.bound,
         }
 
@@ -273,48 +271,50 @@
 
     :param split_ratio: The ratio used to split the data into training and validation sets.
     :param seed: The number used to initialize a pseudorandom
         number generator to randomize the annotation shuffling.
     :param normalized: Boolean to indicate whether the bound
         coordinates of the exported annotations should be normalized. Defaults to True.
     """
+
     split_ratio: int
     seed: int
     normalized: bool = True
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         return {
             "splitRatio": self.split_ratio,
             "seed": self.seed,
             "normalized": self.normalized,
         }
 
 
 @dataclass
 class AnnotationExportMetadata:
     """Annotation exported metadata.
 
     :param format: The annotation format for bounding boxes or polygons as a string.
     :param options: The exporting options.
     """
+
     format: Union[AnnotationExportFormat, str]
     options: Union[AnnotationExportOptions, dict]
 
     def __post_init__(self):
         assert isinstance(self.format, (AnnotationExportFormat, str))
         assert isinstance(self.options, (AnnotationExportOptions, dict))
 
         if isinstance(self.format, str):
             self.format = AnnotationExportFormat(self.format)
         if isinstance(self.options, dict):
             self.options = AnnotationExportOptions(**self.options)
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         return {"format": self.format.value, "options": self.options.to_json()}
 
 
 @dataclass
 class Pagination:
     """Pagination Params.
     If the length of the function call results exceeds the limit,
@@ -324,15 +324,15 @@
     :param limit: A limit on the number of objects to be returned in a page. Defaults to 100.
     """
 
     page: str = None
     limit: int = 100
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         pagination = {
             "page": self.page,
             "limit": self.limit,
         }
 
         # Remove None values
         return {k: v for k, v in pagination.items() if v is not None}
@@ -346,15 +346,15 @@
     :param custom_metadata: A dictionary containing any key-value pairs.
     """
 
     status: Union[AssetStatus, None] = None
     custom_metadata: object = None
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         asset_metadata = {
             "status": self.status,
             "customMetadata": self.custom_metadata,
         }
 
         # Remove None values
         return {k: v for k, v in asset_metadata.items() if v is not None}
@@ -367,20 +367,21 @@
     :param evaluation_strategy: The evaluation strategy to use
         of each Inference API, default entropy_score.
     :param evaluation_threshold: The evaluation threshold to
         use to trigger post-evaluation actions, default 0.5.
     :param evaluation_group: The asset group to which assets
         triggered by the active learning route will be uploaded, comma-separated list.
     """
+
     evaluation_strategy: str = None
     evaluation_threshold: float = None
     evaluation_group: [str] = None
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         options = {
             "evaluationStrategy": self.evaluation_strategy,
             "evaluationThreshold": self.evaluation_threshold,
             "evaluationGroup": self.evaluation_group,
         }
         # Remove None values
         return {k: v for k, v in options.items() if v is not None}
@@ -393,15 +394,15 @@
     :param GPU_T4: The number of NVIDIA Tesla T4 GPUs to
         allocate to each Inference API instance, optional.
     """
 
     GPU_T4: int = None
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         resource = {
             "GPU_T4": self.GPU_T4,
         }
         # Remove None values
         return {k: v for k, v in resource.items() if v is not None}
 
 
@@ -429,35 +430,28 @@
     def __post_init__(self):
         if isinstance(self.options, dict):
             self.options = DeploymentOptions(**self.options)
         if isinstance(self.resources, dict):
             self.resources = DeploymentResource(**self.resources)
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         deployment_metadata = {
-            'name':
-            self.name,
-            "versionTag":
-            self.version_tag,
-            'modelId':
-            self.model_id,
-            'artifactId':
-            self.artifact_id,
-            'replicas':
-            self.replicas,
-            'resources':
-            self.resources.to_json() if self.resources is not None else None,
-            'options':
-            self.options.to_json() if self.options is not None else None,
+            "name": self.name,
+            "versionTag": self.version_tag,
+            "modelId": self.model_id,
+            "artifactId": self.artifact_id,
+            "replicas": self.replicas,
+            "resources": (
+                self.resources.to_json() if self.resources is not None else None
+            ),
+            "options": self.options.to_json() if self.options is not None else None,
         }
         return {
-            k: v
-            for k, v in deployment_metadata.items()
-            if v is not None and v != {}
+            k: v for k, v in deployment_metadata.items() if v is not None and v != {}
         }
 
 
 @dataclass
 class Accelerator:
     """The hardware accelerator to be used for the training.
 
@@ -467,15 +461,15 @@
         More GPUs will use up more compute minutes. Defaults to 1.
     """
 
     name: str
     count: int = 1
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         return {
             "name": self.name,
             "count": self.count,
         }
 
 
 @dataclass
@@ -522,15 +516,15 @@
     """
 
     strategy: str
     metric: str = None
     evaluation_interval: int = 250
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
 
         checkpoint = {
             "strategy": self.strategy,
             "metric": self.metric,
             "evaluationInterval": self.evaluation_interval,
         }
         # Remove None values
@@ -552,15 +546,15 @@
         used if the limit metric is "LIM_NONE". Defaults to 1.
     """
 
     metric: str
     value: int = 1
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         return {
             "metric": self.metric,
             "value": self.value,
         }
 
 
 @dataclass
@@ -596,118 +590,118 @@
 
     :param title: The title of the workflow.
     """
 
     title: str
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         return {
             "title": self.title,
         }
 
 
 @dataclass
 class AssetFilter:
-    """Asset list filter.
-    """
+    """Asset list filter."""
+
     groups: List[str] = None
     filename: str = None
     metadata_query: str = None
     status: Union[AssetStatus, str, None] = None
 
     def __post_init__(self):
         assert isinstance(self.groups, (List, type(None)))
 
         if isinstance(self.status, str):
             self.status = AssetStatus(self.status)
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         asset_filters = {
             "group": self.groups,
             "filename": self.filename,
             "metadataQuery": self.metadata_query,
             "status": self.status.value if self.status is not None else None,
         }
 
         return {k: v for k, v in asset_filters.items() if v is not None}
 
 
 @dataclass
 class AnnotationFilter:
-    """Annotation list filter.
-    """
+    """Annotation list filter."""
+
     asset_ids: List[str] = None
 
     def __post_init__(self):
         assert isinstance(self.asset_ids, (List, type(None)))
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         annotation_filters = {
             "assetId": self.asset_ids,
         }
 
         return {k: v for k, v in annotation_filters.items() if v is not None}
 
 
 @dataclass
 class TagMetadata:
-    """Tag Metadata.
-    """
+    """Tag Metadata."""
+
     name: str = None
     color: str = None
     description: str = None
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         tag = {
             "name": self.name,
             "color": self.color,
             "description": self.description,
         }
 
         # Remove None values
         return {k: v for k, v in tag.items() if v is not None}
 
 
 @dataclass
 class ArtifactExportOptions:
-    """Artifact Export Options.
-    """
+    """Artifact Export Options."""
+
     format: Union[ModelFormat, str]
     quantization: str = None
 
     def __post_init__(self):
         assert isinstance(self.format, (ModelFormat, str))
 
         if isinstance(self.format, str):
             self.format = ModelFormat(self.format)
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         options = {
             "format": self.format.value,
             "quantization": self.quantization,
         }
 
         # Remove None values
         return {k: v for k, v in options.items() if v is not None}
 
 
 @dataclass
 class ArtifactFilters:
-    """Artifact list filter.
-    """
+    """Artifact list filter."""
+
     run_ids: List[str] = None
 
     def __post_init__(self):
         assert isinstance(self.run_ids, (List, type(None)))
 
     def to_json(self):
-        """ Function to convert dataclass to dict """
+        """Function to convert dataclass to dict"""
         artifact_filters = {
             "runId": self.run_ids,
         }
 
         return {k: v for k, v in artifact_filters.items() if v is not None}
```

### Comparing `datature-1.6.0/datature/nexus/api/workflow.py` & `datature-1.7.0/datature/nexus/api/workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   workflow.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Workflow API
-'''
+"""
 
 from typing import Union
 
 from datature.nexus import models
 from datature.nexus.api.types import FlowMetadata
 from datature.nexus.client_context import RestContext
 
 
 class Workflow(RestContext):
     """Datature Workflow API Resource."""
 
     def list(self) -> models.Workflows:
         """Lists all workflows in the project.
 
-        :return: 
+        :return:
             A list of msgspec structs containing the workflow metadata with the following structure:
 
                 .. code-block:: python
 
                     [Workflow(
-                        id='flow_64e812a7e47592ef374cbbc2', 
-                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                        title='Yolov8 Workflow', 
+                        id='flow_64e812a7e47592ef374cbbc2',
+                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                        title='Yolov8 Workflow',
                         create_date=1701927649302,
                         update_date=1701927649302
                     )]
 
         :example:
                 .. code-block:: python
 
                     from datature.nexus import Client
 
                     project = Client("5aa41e8ba........").get_project("proj_b705a........")
                     project.workflows.list()
         """
-        return self.requester.GET(f"/projects/{self.project_id}/workflows",
-                                  response_type=models.Workflows)
+        return self.requester.GET(
+            f"/projects/{self.project_id}/workflows", response_type=models.Workflows
+        )
 
     def get(self, flow_id: str) -> models.Workflow:
         """Retrieves a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow.
-        :return: 
+        :return:
             A msgspec struct containing the specific workflow metadata with the following structure:
 
                 .. code-block:: python
 
                     Workflow(
-                        id='flow_64e812a7e47592ef374cbbc2', 
-                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                        title='Yolov8 Workflow', 
+                        id='flow_64e812a7e47592ef374cbbc2',
+                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                        title='Yolov8 Workflow',
                         create_date=1701927649302,
                         update_date=1701927649302
                     )
 
 
         :example:
                 .. code-block:: python
@@ -77,61 +78,62 @@
                         project = Client("5aa41e8ba........").get_project("proj_b705a........")
                         project.workflows.get("flow_639309be08b4488a914b8802")
         """
         assert isinstance(flow_id, str)
 
         return self.requester.GET(
             f"/projects/{self.project_id}/workflows/{flow_id}",
-            response_type=models.Workflow)
+            response_type=models.Workflow,
+        )
 
-    def update(self, flow_id: str, flow: Union[FlowMetadata,
-                                               dict]) -> models.Workflow:
+    def update(self, flow_id: str, flow: Union[FlowMetadata, dict]) -> models.Workflow:
         """Updates title of a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow.
         :param flow: The new metadata of the workflow to be updated.
         :return: A msgspec struct containing the updated workflow metadata with the following structure:
 
                 .. code-block:: python
 
                     Workflow(
-                        id='flow_64e812a7e47592ef374cbbc2', 
-                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535', 
-                        title='My awesome workflow', 
+                        id='flow_64e812a7e47592ef374cbbc2',
+                        project_id='proj_cd067221d5a6e4007ccbb4afb5966535',
+                        title='My awesome workflow',
                         create_date=1701927649302,
                         update_date=1701927649302
                     )
 
         :example:
                 .. code-block:: python
 
                         from datature.nexus import Client, ApiTypes
 
                         project = Client("5aa41e8ba........").get_project("proj_b705a........")
 
                         project.workflows.update(
-                            "flow_639309be08b4488a914b8802", 
+                            "flow_639309be08b4488a914b8802",
                             {"title": "My awesome workflow"}
                         )
                         // or
                         project.workflows.update(
-                            "flow_639309be08b4488a914b8802", 
+                            "flow_639309be08b4488a914b8802",
                             ApiTypes.FlowMetadata(title="My awesome workflow")
                         )
         """
         assert isinstance(flow_id, str)
         assert isinstance(flow, (FlowMetadata, dict))
 
         if isinstance(flow, dict):
             flow = FlowMetadata(**flow)
 
         return self.requester.PATCH(
             f"/projects/{self.project_id}/workflows/{flow_id}",
             request_body=flow.to_json(),
-            response_type=models.Workflow)
+            response_type=models.Workflow,
+        )
 
     def delete(self, flow_id: str) -> models.DeleteResponse:
         """Deletes a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow
         :return: A msgspec struct containing the deleted
             workflow ID and deletion status with the following structure:
@@ -148,8 +150,9 @@
                 project = Client("5aa41e8ba........").get_project("proj_b705a........")
                 project.workflows.delete("flow_639309be08b4488a914b8802")
         """
         assert isinstance(flow_id, str)
 
         return self.requester.DELETE(
             f"/projects/{self.project_id}/workflows/{flow_id}",
-            response_type=models.DeleteResponse)
+            response_type=models.DeleteResponse,
+        )
```

### Comparing `datature-1.6.0/datature/nexus/cli/commands.py` & `datature-1.7.0/datature/nexus/cli/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,154 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   commands.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI supported commands
-'''
+"""
 
 import sys
-from typing import Optional
 from argparse import ArgumentParser, _SubParsersAction
+from typing import Optional
 
 from datature import nexus
 
 # pylint: disable=W0212
 
 
 class Commands:
     """All Datature CLI commands."""
 
     def __init__(self) -> None:
         self.parser = ArgumentParser(
-            prog='datature',
-            description=
-            "Command line tool to create/upload/download datasets on datature nexus.",
+            prog="datature",
+            description="Command line tool to create/upload/download datasets on datature nexus.",
         )
 
-        self.parser.add_argument('-v',
-                                 '--version',
-                                 action='version',
-                                 version=f'%(prog)s {nexus.__version__}')
+        self.parser.add_argument(
+            "-v", "--version", action="version", version=f"%(prog)s {nexus.__version__}"
+        )
 
         self.subparsers = self.parser.add_subparsers(dest="command")
         self._add_project_parser()
         self._add_asset_parser()
         self._add_annotation_parser()
         self._add_artifact_parser()
         self._add_help_parser()
 
     def _add_project_parser(self):
         """Project level parser."""
         projects = self.subparsers.add_parser(
             "projects",
             help="Projects management.",
-            description=
-            "datature projects - auth/list/select project from saved project.",
+            description="datature projects - auth/list/select project from saved project.",
         )
         projects_action = projects.add_subparsers(dest="action")
 
-        projects_action.add_parser('auth',
-                                   help='Authenticate and save the project.')
+        projects_action.add_parser("auth", help="Authenticate and save the project.")
         projects_action.add_parser(
-            'select', help='Select the project from saved projects.')
-        projects_action.add_parser('list', help='List the saved projects.')
+            "select", help="Select the project from saved projects."
+        )
+        projects_action.add_parser("list", help="List the saved projects.")
 
-        projects_action.add_parser('help',
-                                   help='Show this help message and exit.',
-                                   add_help=False)
+        projects_action.add_parser(
+            "help", help="Show this help message and exit.", add_help=False
+        )
 
     def _add_asset_parser(self):
         """Asset level parser."""
         assets = self.subparsers.add_parser(
             "assets",
             help="Assets management.",
             description="datature assets - upload/group assets.",
         )
         assets_action = assets.add_subparsers(dest="action")
 
         assets_upload = assets_action.add_parser(
-            'upload',
-            help='Bulk update assets.',
+            "upload",
+            help="Bulk update assets.",
+        )
+        assets_upload.add_argument("path", nargs="*", help="The asset path to upload.")
+        assets_upload.add_argument(
+            "groups", nargs="*", help="The asset groups to upload."
         )
-        assets_upload.add_argument("path",
-                                   nargs='*',
-                                   help='The asset path to upload.')
-        assets_upload.add_argument("groups",
-                                   nargs='*',
-                                   help='The asset groups to upload.')
 
         assets_group = assets_action.add_parser(
-            'groups',
-            help='List assets group details.',
+            "groups",
+            help="List assets group details.",
+        )
+        assets_group.add_argument("group", nargs="*", help="The asset group name.")
+
+        assets_action.add_parser(
+            "help", help="Show this help message and exit.", add_help=False
         )
-        assets_group.add_argument("group",
-                                  nargs='*',
-                                  help='The asset group name.')
-
-        assets_action.add_parser('help',
-                                 help='Show this help message and exit.',
-                                 add_help=False)
 
     def _add_annotation_parser(self):
         """Annotation level parser."""
         annotations = self.subparsers.add_parser(
             "annotations",
             help="Annotations management.",
             description="datature annotations - upload/download annotations.",
         )
         annotations_action = annotations.add_subparsers(dest="action")
 
         annotations_upload = annotations_action.add_parser(
-            'upload',
-            help='Bulk upload annotations from file.',
+            "upload",
+            help="Bulk upload annotations from file.",
+        )
+        annotations_upload.add_argument(
+            "path", nargs="*", help="The annotations file path."
         )
-        annotations_upload.add_argument("path",
-                                        nargs='*',
-                                        help='The annotations file path.')
 
         annotations_download = annotations_action.add_parser(
-            'download',
-            help='Bulk download annotations to file.',
+            "download",
+            help="Bulk download annotations to file.",
+        )
+        annotations_download.add_argument(
+            "path", nargs="*", help="The annotations file path."
         )
-        annotations_download.add_argument("path",
-                                          nargs='*',
-                                          help='The annotations file path.')
         annotations_download.add_argument(
-            "format", nargs='*', help='The annotations format to download.')
+            "format", nargs="*", help="The annotations format to download."
+        )
 
-        annotations_action.add_parser('help',
-                                      help='Show this help message and exit.',
-                                      add_help=False)
+        annotations_action.add_parser(
+            "help", help="Show this help message and exit.", add_help=False
+        )
 
     def _add_artifact_parser(self):
         """Artifact level parser."""
         artifacts = self.subparsers.add_parser(
             "artifacts",
             help="Artifacts management.",
             description="datature artifacts - download artifact models.",
         )
         artifacts_action = artifacts.add_subparsers(dest="action")
 
         artifacts_download = artifacts_action.add_parser(
-            'download',
-            help='Download artifact model.',
+            "download",
+            help="Download artifact model.",
+        )
+        artifacts_download.add_argument(
+            "artifact_id", nargs="*", help="The id of the artifact."
+        )
+        artifacts_download.add_argument(
+            "format", nargs="*", help="The artifact model format."
+        )
+
+        artifacts_action.add_parser(
+            "help", help="Show this help message and exit.", add_help=False
         )
-        artifacts_download.add_argument("artifact_id",
-                                        nargs='*',
-                                        help='The id of the artifact.')
-        artifacts_download.add_argument("format",
-                                        nargs='*',
-                                        help='The artifact model format.')
-
-        artifacts_action.add_parser('help',
-                                    help='Show this help message and exit.',
-                                    add_help=False)
 
     def _add_help_parser(self):
         """Help level parser."""
         help_parser = self.subparsers.add_parser(
             "help",
             description="Show this help message and exit.",
         )
@@ -184,13 +178,14 @@
 
         : param subparser: The name of subparser.
         :return: None
         """
         parser = self.parser
 
         if subparser:
-            parser = next(action.choices[subparser]
-                          for action in parser._actions
-                          if isinstance(action, _SubParsersAction)
-                          and subparser in action.choices)
+            parser = next(
+                action.choices[subparser]
+                for action in parser._actions
+                if isinstance(action, _SubParsersAction) and subparser in action.choices
+            )
 
         parser.print_help()
```

### Comparing `datature-1.6.0/datature/nexus/cli/config.py` & `datature-1.7.0/datature/nexus/cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   config.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI config class
-'''
+"""
 
-import os
+import base64
 import io
+import os
 import sys
-import base64
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import yaml
 
 from .messages import INVALID_PROJECT_MESSAGE, NO_PROJECT_MESSAGE
 
 
-class Config():
+class Config:
     """Handles YAML configuration files"""
 
     def __init__(self):
         """Init config file"""
 
         self._path = self._get_config_path()
         self._data = self._parse()
@@ -57,15 +57,15 @@
         try:
             with open(self._path, "r", encoding="utf8") as stream:
                 return yaml.safe_load(stream)
         except FileNotFoundError:
             return {}
 
     def _get(self, key: str, default: Optional[Any] = None) -> Dict[str, Any]:
-        """Get JSON value from self._data """
+        """Get JSON value from self._data"""
 
         data: Any = self._data.copy()
 
         while True:
             if isinstance(key, str):
                 key = key.split("/")
             key, *keys = key
@@ -80,23 +80,19 @@
 
     def _save(self) -> None:
         """Persist the config to the file system"""
 
         if not self._path:
             return
         with io.open(self._path, "w", encoding="utf8") as config_file:
-            yaml.dump(self._data,
-                      config_file,
-                      default_flow_style=False,
-                      allow_unicode=True)
-
-    def set(self,
-            key: Union[str, List[str]],
-            value: Any,
-            save: bool = True) -> None:
+            yaml.dump(
+                self._data, config_file, default_flow_style=False, allow_unicode=True
+            )
+
+    def set(self, key: Union[str, List[str]], value: Any, save: bool = True) -> None:
         """
         Sets the value for the specified key.
 
         :param key: The key where the value is going to be stored.
         :param value: The value to be stored.
         :param save: If ``True``, persists the value in the FileSystem. Defaults to ``True``.
         :return: None
@@ -109,28 +105,34 @@
         for k in key[:-1]:
             pointer = pointer.setdefault(k, {})
         pointer[key[-1]] = str(value)
 
         if save:
             self._save()
 
-    def set_project(self, project_id: str, project_name: str,
-                    project_secret: str, default_project: bool) -> None:
+    def set_project(
+        self,
+        project_id: str,
+        project_name: str,
+        project_secret: str,
+        default_project: bool,
+    ) -> None:
         """
         Stores the project secret and project information.
 
         :param project_id: The id of the project.
         :param project_name: The name of the project.
         :param project_secret: The secret of the project.
         :param default_project: If set this project as the default project.
         :return: None
         """
         self.set(
             f"project/{project_id}/project_secret",
-            base64.b64encode(project_secret.encode("ascii")).decode("ascii"))
+            base64.b64encode(project_secret.encode("ascii")).decode("ascii"),
+        )
         self.set(f"project/{project_id}/project_name", project_name)
 
         if default_project or len(self._get("project").keys()) == 1:
             self.set("default_project", project_id)
 
     def get_all_project_names(self) -> [str]:
         """
@@ -160,22 +162,19 @@
         project_id = self._get("default_project")
 
         if project_id is None:
             print(NO_PROJECT_MESSAGE)
             sys.exit(1)
 
         return {
-            "project_name":
-            self._get(f"project/{project_id}/project_name"),
-            "project_id":
-            project_id,
-            "project_secret":
-            base64.b64decode(
-                self._get(f"project/{project_id}/project_secret").encode(
-                    'ascii')).decode('ascii'),
+            "project_name": self._get(f"project/{project_id}/project_name"),
+            "project_id": project_id,
+            "project_secret": base64.b64decode(
+                self._get(f"project/{project_id}/project_secret").encode("ascii")
+            ).decode("ascii"),
         }
 
     def set_default_project(self, project_id: str) -> None:
         """
         Set default project
 
         :param project_id: The id of the project.
@@ -200,19 +199,18 @@
         :return: dict
         """
         project_ids = list(self._get("project").keys())
 
         for project_id in project_ids:
             if project_name == self._get(f"project/{project_id}/project_name"):
                 return {
-                    "project_name":
-                    self._get(f"project/{project_id}/project_name"),
-                    "project_id":
-                    project_id,
-                    "project_secret":
-                    base64.b64decode(
-                        self._get(f"project/{project_id}/project_secret").
-                        encode('ascii')).decode('ascii'),
+                    "project_name": self._get(f"project/{project_id}/project_name"),
+                    "project_id": project_id,
+                    "project_secret": base64.b64decode(
+                        self._get(f"project/{project_id}/project_secret").encode(
+                            "ascii"
+                        )
+                    ).decode("ascii"),
                 }
 
         print(INVALID_PROJECT_MESSAGE)
         sys.exit(1)
```

### Comparing `datature-1.6.0/datature/nexus/cli/functions.py` & `datature-1.7.0/datature/nexus/cli/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   functions.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI functions
-'''
+"""
 # pylint: disable=E1102,R0912,C0103,R0914
 
 import os
 import re
 import sys
 import time
+from os.path import basename, exists, isdir, join
 from pathlib import Path
 from typing import Optional
-from os.path import basename, exists, join, isdir
 
 import inquirer
 import requests
-from halo import Halo
 from alive_progress import alive_bar
+from halo import Halo
 
 from datature import nexus
-from datature.nexus import error, config
-from datature.nexus.utils import utils
+from datature.nexus import config, error
 from datature.nexus.cli import messages
 from datature.nexus.cli.config import Config
+from datature.nexus.utils import utils
 
 
 def start_spinner(fn: callable):
-    """ Start spinner for the function. """
+    """Start spinner for the function."""
 
     def wrapper(*args, **kwargs):
-        wait_spinner = Halo(text=messages.REQUEST_SERVER_MESSAGE,
-                            spinner='dots')
+        wait_spinner = Halo(text=messages.REQUEST_SERVER_MESSAGE, spinner="dots")
         wait_spinner.start()
 
         try:
             result = fn(*args, **kwargs)
             return result
         finally:
             wait_spinner.stop()
@@ -62,49 +61,50 @@
     project = cli_config.get_default_project()
 
     if project is None:
         print(messages.NO_PROJECT_MESSAGE)
         sys.exit(1)
 
     return nexus.Client(project.get("project_secret")).get_project(
-        project.get("project_id"))
+        project.get("project_id")
+    )
 
 
 @start_spinner
 def sdk_list_project(secret_key: str):
-    """ Retrieve project from server. """
+    """Retrieve project from server."""
     sdk_client = nexus.Client(secret_key)
 
     projects = sdk_client.list_projects()
     # Support to use workspace after one secret support multiple projects
     return projects
 
 
 @start_spinner
 def sdk_retrieve_project(project_secret: str, project_id: str):
-    """ Retrieve project from server. """
+    """Retrieve project from server."""
     sdk_project = nexus.Client(project_secret)
 
     project = sdk_project.get_project(project_id)
 
     return project
 
 
 @start_spinner
 def sdk_create_upload_session():
-    """ Retrieve project from server. """
+    """Retrieve project from server."""
     sdk_project = get_default_datature_client()
 
     import_session = sdk_project.annotations.create_import_session()
 
     return import_session
 
 
 def sdk_retrieve_operation(op_id: str):
-    """ Retrieve operation from server. """
+    """Retrieve operation from server."""
     sdk_project = get_default_datature_client()
 
     operation = sdk_project.operations.get(op_id)
     return operation
 
 
 def download_file_from_link(link: str, download_path: str):
@@ -116,21 +116,19 @@
     :return: None
     """
     query_string_removed = link.split("?")[0]
     file_name = basename(query_string_removed)
 
     resp = requests.get(link, stream=True, timeout=120)
 
-    total = int(resp.headers.get('content-length', 0))
+    total = int(resp.headers.get("content-length", 0))
     current_size = 0
-    with open(join(download_path, file_name),
-              'wb') as file, alive_bar(total,
-                                       title='Downloading',
-                                       title_length=12,
-                                       manual=True) as progress_bar:
+    with open(join(download_path, file_name), "wb") as file, alive_bar(
+        total, title="Downloading", title_length=12, manual=True
+    ) as progress_bar:
         for data in resp.iter_content(chunk_size=1024):
             size = file.write(data)
             current_size += size
             progress_bar(float(current_size / total))
         progress_bar(1.0)
 
 
@@ -157,19 +155,19 @@
         )
 
         for project in projects:
             if project.get_info().name == project_name:
                 project_id = project.get_info().id
 
         default_project = inquirer.confirm(
-            f"Make [{project_name}] the default project?", default=True)
+            f"Make [{project_name}] the default project?", default=True
+        )
 
         cli_config = Config()
-        cli_config.set_project(project_id, project_name, secret_key,
-                               default_project)
+        cli_config.set_project(project_id, project_name, secret_key, default_project)
 
     except error.ForbiddenError:
         print(messages.INVALID_PROJECT_SECRET_MESSAGE)
         sys.exit(1)
     print(messages.AUTHENTICATION_MESSAGE)
 
 
@@ -198,39 +196,44 @@
 
     :return: None
     """
     cli_config = Config()
     project_names = cli_config.get_all_project_names()
     default_project = cli_config.get_default_project()
 
-    output = [[
-        "NAME", "TOTAL_ASSETS", "ANNOTATED_ASSETS", "ANNOTATIONS", "TAGS"
-    ]]
+    output = [["NAME", "TOTAL_ASSETS", "ANNOTATED_ASSETS", "ANNOTATIONS", "TAGS"]]
     for project_name in project_names:
         project = cli_config.get_project_by_name(project_name)
         try:
-            project = sdk_retrieve_project(project.get("project_secret"),
-                                           project.get("project_id"))
+            project = sdk_retrieve_project(
+                project.get("project_secret"), project.get("project_id")
+            )
             project_info = project.get_info()
 
             total_assets = project_info.statistic.total_assets
             annotated_assets = project_info.statistic.annotated_assets
             total_annotations = project_info.statistic.total_annotations
             tags = project_info.tags
 
-            output.append([
-                project_name, total_assets, annotated_assets,
-                total_annotations,
-                len(tags)
-            ])
+            output.append(
+                [
+                    project_name,
+                    total_assets,
+                    annotated_assets,
+                    total_annotations,
+                    len(tags),
+                ]
+            )
         except error.ForbiddenError:
-            print((
-                f"\nProject {[project_name]} "
-                "authentication failed, please use 'datature projects auth' again."
-            ))
+            print(
+                (
+                    f"\nProject {[project_name]} "
+                    "authentication failed, please use 'datature projects auth' again."
+                )
+            )
             sys.exit(1)
     print_table(output, 20)
     print(
         f"\n{messages.ACTIVE_PROJECT_MESSAGE}: [{default_project.get('project_name')}]"
     )
 
 
@@ -239,16 +242,17 @@
     Upload annotations from path.
 
     :param path: The annotation path to upload.
     :param annotation_format: The annotation format to upload.
     :return: None
     """
     # Custom manage loop
-    with alive_bar(data_size, title='Processing', title_length=12,
-                   manual=True) as progress_bar:
+    with alive_bar(
+        data_size, title="Processing", title_length=12, manual=True
+    ) as progress_bar:
         while True:
             operation = sdk_retrieve_operation(op_id)
 
             if operation.status.overview == "Errored":
                 print(messages.UNKNOWN_ERROR_MESSAGE)
                 sys.exit(1)
 
@@ -256,40 +260,48 @@
 
             queued = count.Queued
             running = count.Running
             finished = count.Finished
             cancelled = count.Cancelled
             errored = count.Errored
             percentage = float(
-                (int(errored) + int(cancelled) + int(finished)) /
-                (int(errored) + int(cancelled) + int(finished) + int(queued) +
-                 int(running)))
+                (int(errored) + int(cancelled) + int(finished))
+                / (
+                    int(errored)
+                    + int(cancelled)
+                    + int(finished)
+                    + int(queued)
+                    + int(running)
+                )
+            )
 
             if percentage == 1:
                 break
 
             progress_bar(percentage)
             time.sleep(config.OPERATION_LOOPING_DELAY_SECONDS)
-        progress_bar(1.)
+        progress_bar(1.0)
     print(messages.SERVER_COMPLETED_MESSAGE)
 
 
 def upload_assets(path: Optional[Path] = None, groups: Optional[str] = None):
     """
     Upload assets from path.
 
     :param path: The folder to upload assets.
     :return: None
     """
     # check path if exist
     if not path:
         questions = [
-            inquirer.Path("path_result",
-                          message=messages.ASSETS_FOLDER_MESSAGE,
-                          default=os.getcwd()),
+            inquirer.Path(
+                "path_result",
+                message=messages.ASSETS_FOLDER_MESSAGE,
+                default=os.getcwd(),
+            ),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         path = answer.get("path_result").strip()
 
     if not exists(path):
         print(messages.PATH_NOT_EXISTS_MESSAGE)
         sys.exit(1)
@@ -298,62 +310,60 @@
     file_paths = utils.find_all_assets(path)
 
     if len(file_paths) == 0:
         print(messages.NO_ASSETS_FOUND_MESSAGE)
         sys.exit(1)
 
     nifti_orientation = None
-    if '.nii' in ",".join(str(file_path).lower() for file_path in file_paths):
+    if ".nii" in ",".join(str(file_path).lower() for file_path in file_paths):
         nifti_orientation = inquirer.text(
             messages.ASSETS_NIFTI_DIRECTION_CHOICE_MESSAGE,
             validate=lambda _, x: x in ["", "x", "y", "z"],
         )
 
     if not groups:
         groups_res = inquirer.text(
             messages.ASSETS_GROUPS_MESSAGE,
             default="main",
             validate=lambda _, x: re.match("^[A-Za-z0-9,]*$", x),
         )
-        groups = [
-            group.strip() for group in groups_res.split(',') if group.strip()
-        ]
+        groups = [group.strip() for group in groups_res.split(",") if group.strip()]
 
     confirm = inquirer.confirm(
         f"""{len(file_paths)} assets will be uploaded to group(s) ({
             ', '.join(groups)})?""",
-        default=True)
+        default=True,
+    )
     if not confirm:
         sys.exit(0)
 
     batch_size = config.ASSET_UPLOAD_SESSION_BATCH_SIZE
 
     num_batches = len(file_paths) // batch_size
     batches = [
-        file_paths[i * batch_size:(i + 1) * batch_size]
-        for i in range(num_batches)
+        file_paths[i * batch_size : (i + 1) * batch_size] for i in range(num_batches)
     ]
 
     if len(file_paths) % batch_size != 0:
-        batches.append(file_paths[num_batches * batch_size:])
+        batches.append(file_paths[num_batches * batch_size :])
 
     sdk_project = get_default_datature_client()
     # Loop Prepare asset metadata
     for _, batch in enumerate(batches):
         upload_session = sdk_project.assets.create_upload_session(
-            groups=groups, background=True)
+            groups=groups, background=True
+        )
 
         with alive_bar(
-                len(batch),
-                title='Preparing',
-                title_length=12,
+            len(batch),
+            title="Preparing",
+            title_length=12,
         ) as progress_bar, upload_session as session:
             for file_path in batch:
-                session.add_path(file_path,
-                                 nifti_orientation=nifti_orientation)
+                session.add_path(file_path, nifti_orientation=nifti_orientation)
                 progress_bar()
 
         operations = upload_session.get_operation_ids()
 
         cli_loop_operation(operations[0], len(upload_session))
 
 
@@ -362,75 +372,78 @@
     Upload annotations from path.
 
     :param path: The annotation path to upload.
     :return: None
     """
     if not path:
         questions = [
-            inquirer.Path("path_result",
-                          message=messages.ANNOTATION_FOLDER_MESSAGE),
+            inquirer.Path("path_result", message=messages.ANNOTATION_FOLDER_MESSAGE),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         path = answer.get("path_result").strip()
 
     # find all images under folder and sub folders
     if isdir(path):
         file_paths = utils.find_all_annotations_files(path)
     else:
         file_paths = [path]
 
     confirm = inquirer.confirm(
-        f"""{len(file_paths)} files will be uploaded?""", default=True)
+        f"""{len(file_paths)} files will be uploaded?""", default=True
+    )
     if not confirm:
         sys.exit(0)
 
     batch_size = config.ANNOTATION_IMPORT_SESSION_BATCH_SIZE
 
     num_batches = len(file_paths) // batch_size
     batches = [
-        file_paths[i * batch_size:(i + 1) * batch_size]
-        for i in range(num_batches)
+        file_paths[i * batch_size : (i + 1) * batch_size] for i in range(num_batches)
     ]
 
     if len(file_paths) % batch_size != 0:
-        batches.append(file_paths[num_batches * batch_size:])
+        batches.append(file_paths[num_batches * batch_size :])
 
     # Loop Prepare asset metadata
     for _, batch in enumerate(batches):
         import_session = sdk_create_upload_session()
 
         with alive_bar(
-                len(batch),
-                title='Preparing',
-                title_length=12,
+            len(batch),
+            title="Preparing",
+            title_length=12,
         ) as progress_bar, import_session as session:
             for file_path in batch:
                 progress_bar()
 
                 session.add_path(file_path)
 
     print(messages.SERVER_COMPLETED_MESSAGE)
 
 
-def download_artifact(artifact_id: Optional[str] = None,
-                      model_format: Optional[str] = None,
-                      path: Optional[str] = None):
+def download_artifact(
+    artifact_id: Optional[str] = None,
+    model_format: Optional[str] = None,
+    path: Optional[str] = None,
+):
     """
     Download artifact model.
 
     :param artifact_id: The id of the artifact.
     :param model_format: The artifact model to download.
     :param path: The path to download the model.
     :return: None
     """
     if not path:
         questions = [
-            inquirer.Path("path_result",
-                          message=messages.ARTIFACT_MODEL_FOLDER_MESSAGE,
-                          default=os.getcwd()),
+            inquirer.Path(
+                "path_result",
+                message=messages.ARTIFACT_MODEL_FOLDER_MESSAGE,
+                default=os.getcwd(),
+            ),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         path = answer.get("path_result").strip()
 
     if not exists(path):
         print(messages.PATH_NOT_EXISTS_MESSAGE)
         sys.exit(1)
@@ -443,16 +456,16 @@
         if len(artifacts) == 0:
             print(messages.NO_ARTIFACTS_MESSAGE)
             sys.exit(1)
 
         artifact_lists = []
         artifacts_key_map = {}
         for artifact in artifacts:
-            key = (f"""{artifact.get('run_id')[-6:].upper()
-                     }-{artifact.get('flow_title')}""")
+            key = f"""{artifact.get('run_id')[-6:].upper()
+                     }-{artifact.get('flow_title')}"""
             artifact_lists.append(key)
             artifacts_key_map[key] = artifact
 
         questions = [
             inquirer.List(
                 "artifact",
                 message=messages.ARTIFACT_DOWNLOAD_MESSAGE,
@@ -480,120 +493,126 @@
         for model in artifact.exports:
             if model.format == model_format and model.status == "Finished":
                 download_file_from_link(model.download.url, path)
 
     else:
         # not exported, need looping query download status
         # Loop to query status,
-        wait_spinner = Halo(text=messages.EXPORT_ARTIFACT_WAITING_MESSAGE,
-                            spinner='dots')
+        wait_spinner = Halo(
+            text=messages.EXPORT_ARTIFACT_WAITING_MESSAGE, spinner="dots"
+        )
         wait_spinner.start()
-        models = sdk_project.artifacts.create_export(artifact.id,
-                                                     {"format": model_format})
+        models = sdk_project.artifacts.create_export(
+            artifact.id, {"format": model_format}
+        )
 
         while True:
-            models = sdk_project.artifacts.list_exported_models(
-                artifact.get("id"))
+            models = sdk_project.artifacts.list_exported_models(artifact.get("id"))
             for model in models:
-                if model.get("format") == model_format and model.get(
-                        "status") == "Finished":
+                if (
+                    model.get("format") == model_format
+                    and model.get("status") == "Finished"
+                ):
                     # start download
                     wait_spinner.stop()
                     download_file_from_link(model.download.url, path)
 
                     return
 
             time.sleep(config.OPERATION_LOOPING_DELAY_SECONDS)
 
 
-def download_annotations(path: Optional[Path] = None,
-                         annotation_format: Optional[str] = None):
+def download_annotations(
+    path: Optional[Path] = None, annotation_format: Optional[str] = None
+):
     """
     Export annotations from path.
 
     :param path: The annotation path to export.
     :param annotation_format: The annotation format to export.
     :return: None
     """
     sdk_project = get_default_datature_client()
     if not path:
         questions = [
-            inquirer.Path("path_result",
-                          message=messages.EXPORT_ANNOTATION_FOLDER_MESSAGE,
-                          default=os.getcwd()),
+            inquirer.Path(
+                "path_result",
+                message=messages.EXPORT_ANNOTATION_FOLDER_MESSAGE,
+                default=os.getcwd(),
+            ),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         path = answer.get("path_result").strip()
 
     if not exists(path):
         print(messages.PATH_NOT_EXISTS_MESSAGE)
         sys.exit(1)
 
     if not annotation_format:
         project = sdk_project.get_info()
 
-        annotations_formats = utils.get_exportable_annotations_formats(
-            project.type)
+        annotations_formats = utils.get_exportable_annotations_formats(project.type)
         questions = [
             inquirer.List(
                 "annotation_format",
                 message=messages.ANNOTATION_FORMAT_MESSAGE,
                 choices=annotations_formats,
             ),
             inquirer.Text(
-                "normalized",
-                message=messages.DOWNLOAD_ANNOTATIONS_NORMALIZED_MESSAGE),
+                "normalized", message=messages.DOWNLOAD_ANNOTATIONS_NORMALIZED_MESSAGE
+            ),
             inquirer.Text(
                 "split_ratio",
                 message=messages.DOWNLOAD_ANNOTATIONS_SPLIT_RATIO_MESSAGE,
                 default=0.5,
-                validate=lambda _, x: re.match(r'^(0(\.\d+)?|1(\.0+)?)$', x)),
+                validate=lambda _, x: re.match(r"^(0(\.\d+)?|1(\.0+)?)$", x),
+            ),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         annotation_format = answer.get("annotation_format")
         normalized = answer.get("normalized") not in ["n", "N"]
         split_ratio = min(max(float(answer.get("split_ratio")), 0), 1)
 
     # Loop to query status,
-    wait_spinner = Halo(text=messages.ANNOTATION_DOWNLOAD_MESSAGE,
-                        spinner='dots')
+    wait_spinner = Halo(text=messages.ANNOTATION_DOWNLOAD_MESSAGE, spinner="dots")
     wait_spinner.start()
-    operation = sdk_project.annotations.create_export({
-        "format": "csv_fourcorner",
-        "options": {
-            "split_ratio": split_ratio,
-            "seed": 1337,
-            "normalized": normalized
+    operation = sdk_project.annotations.create_export(
+        {
+            "format": "csv_fourcorner",
+            "options": {
+                "split_ratio": split_ratio,
+                "seed": 1337,
+                "normalized": normalized,
+            },
         }
-    })
+    )
 
     wait_spinner.stop()
 
     cli_loop_operation(operation.id, 1)
 
     sdk_project.annotations.download_exported_file(operation.id, path)
 
     print(messages.ANNOTATION_DOWNLOADED_MESSAGE)
 
 
 def print_table(data: [[str]], column_width: int = 16):
     """
-        List assets group statistics.
+    List assets group statistics.
 
-        :param data: The element array.
-        :param column_width: The column widths and separator characters
-        :return: None
-        """
+    :param data: The element array.
+    :param column_width: The column widths and separator characters
+    :return: None
+    """
     # Print the table header
     print("".join(f"{item:{column_width}}" for _, item in enumerate(data[0])))
 
     # Print the table data
     for row in data[1:]:
-        print("".join(f"{str(item):{column_width}}"
-                      for _, item in enumerate(row)))
+        print("".join(f"{str(item):{column_width}}" for _, item in enumerate(row)))
 
 
 def assets_group(group: Optional[str] = None):
     """
     List assets group statistics.
 
     :param group: The name of group.
@@ -613,16 +632,19 @@
             messages.CHOOSE_GROUP_MESSAGE,
             choices=groups,
         )
 
         statistics = sdk_project.assets.list_groups([group])
         statistic = statistics[0].statistic
 
-        table = [[
-            "NAME", "TOTAL", "ANNOTATED", "REVIEW", "TOFIX", "COMPLETED"
-        ]]
-        table.append([
-            group, statistic.total_assets, statistic.annotated_assets,
-            statistic.reviewed_assets, statistic.to_fixed_assets,
-            statistic.completed_assets
-        ])
+        table = [["NAME", "TOTAL", "ANNOTATED", "REVIEW", "TOFIX", "COMPLETED"]]
+        table.append(
+            [
+                group,
+                statistic.total_assets,
+                statistic.annotated_assets,
+                statistic.reviewed_assets,
+                statistic.to_fixed_assets,
+                statistic.completed_assets,
+            ]
+        )
         print_table(table)
```

### Comparing `datature-1.6.0/datature/nexus/cli/main.py` & `datature-1.7.0/datature/nexus/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   main.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI main entrance
-'''
+"""
 
 import sys
 
-from datature.nexus.cli.commands import Commands
 from datature.nexus.cli import functions, messages
+from datature.nexus.cli.commands import Commands
 from datature.nexus.error import ErrorWithCode, ForbiddenError
 
 
 def main() -> None:
     """
     Executes the main function of cli.
```

### Comparing `datature-1.6.0/datature/nexus/cli/messages.py` & `datature-1.7.0/datature/nexus/cli/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,73 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   messages.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   collect all string messages variables
-'''
+"""
 
 REQUEST_SERVER_MESSAGE = "Communicating with server."
 SERVER_COMPLETED_MESSAGE = "Server processing completed."
 INVALID_PROJECT_SECRET_MESSAGE = (
     "\nInvalid project secret key, "
-    "generate one for your project on nexus: Advanced/API Management")
+    "generate one for your project on nexus: Advanced/API Management"
+)
 AUTHENTICATION_MESSAGE = "Authentication succeeded."
 AUTHENTICATION_REMINDER_MESSAGE = (
     "\nSecret Key needed, "
-    "generate one for your project on nexus: Advanced/API Management")
-NO_PROJECT_MESSAGE = "\nMissing authentication, please authenticate with 'datature projects auth'."
-ASSETS_FOLDER_MESSAGE = 'Enter the assets folder path to be uploaded'
+    "generate one for your project on nexus: Advanced/API Management"
+)
+NO_PROJECT_MESSAGE = (
+    "\nMissing authentication, please authenticate with 'datature projects auth'."
+)
+ASSETS_FOLDER_MESSAGE = "Enter the assets folder path to be uploaded"
 ASSETS_GROUPS_MESSAGE = "Enter the assets group name(s), split by ','"
 ANNOTATION_FOLDER_MESSAGE = "Enter the annotation files path to be uploaded"
 ANNOTATION_FORMAT_MESSAGE = "Select the annotation file format"
-NO_ARTIFACTS_MESSAGE = "\nNo artifacts can be downloaded, please start a training first."
+NO_ARTIFACTS_MESSAGE = (
+    "\nNo artifacts can be downloaded, please start a training first."
+)
 ARTIFACT_DOWNLOAD_MESSAGE = "Which artifact do you want to download?"
 ARTIFACT_MODEL_FORMAT_DOWNLOAD_MESSAGE = "Which model format do you want to download?"
-EXPORT_ARTIFACT_WAITING_MESSAGE = "Processing artifact for download, it may take 5-10 minutes.\n"
-ARTIFACT_MODEL_FOLDER_MESSAGE = 'Enter the folder path to save model'
+EXPORT_ARTIFACT_WAITING_MESSAGE = (
+    "Processing artifact for download, it may take 5-10 minutes.\n"
+)
+ARTIFACT_MODEL_FOLDER_MESSAGE = "Enter the folder path to save model"
 EXPORT_ANNOTATION_FOLDER_MESSAGE = "Enter the folder path to save annotation files"
 CHOOSE_GROUP_MESSAGE = "Which asset group do you want to list?"
 INVALID_PROJECT_MESSAGE = "\nInvalid project name."
 PATH_NOT_EXISTS_MESSAGE = "\nPath does not exists."
 NO_ASSETS_GROUP_MESSAGE = "\nNo asset groups exist in this project."
 DOWNLOAD_ANNOTATIONS_NORMALIZED_MESSAGE = "Should the annotations be normalized? [Y/n]"
-DOWNLOAD_ANNOTATIONS_SPLIT_RATIO_MESSAGE = "Enter the split ratio for this download. [0-1]"
+DOWNLOAD_ANNOTATIONS_SPLIT_RATIO_MESSAGE = (
+    "Enter the split ratio for this download. [0-1]"
+)
 INVALID_SPLIT_RATIO_MESSAGE = "\nInvalid split ratio."
-AUTHENTICATION_FAILED_MESSAGE = "\nAuthentication failed, please use 'datature projects auth' again."
-UNKNOWN_ERROR_SUPPORT_MESSAGE = "\nCommunication failed, contact support at support@datature.io."
+AUTHENTICATION_FAILED_MESSAGE = (
+    "\nAuthentication failed, please use 'datature projects auth' again."
+)
+UNKNOWN_ERROR_SUPPORT_MESSAGE = (
+    "\nCommunication failed, contact support at support@datature.io."
+)
 CONNECTION_ERROR_MESSAGE = "\nConnection failed, please check your network."
-UNKNOWN_ERROR_MESSAGE = "\nUnknown error occurred, contact support at support@datature.io."
+UNKNOWN_ERROR_MESSAGE = (
+    "\nUnknown error occurred, contact support at support@datature.io."
+)
 ANNOTATION_DOWNLOAD_MESSAGE = "Processing annotations for download."
 ANNOTATION_DOWNLOADED_MESSAGE = "Downloaded annotations."
 ACTIVE_PROJECT_MESSAGE = "Your active project is now"
-NO_ASSETS_FOUND_MESSAGE = "No allowable assets found in folders, please change the folder path."
+NO_ASSETS_FOUND_MESSAGE = (
+    "No allowable assets found in folders, please change the folder path."
+)
 ASSETS_NIFTI_DIRECTION_CHOICE_MESSAGE = (
     "Select the axis of orientation, "
-    "if not provided, we will save videos for each axis. ['x','y','z']")
+    "if not provided, we will save videos for each axis. ['x','y','z']"
+)
```

### Comparing `datature-1.6.0/datature/nexus/client.py` & `datature-1.7.0/datature/nexus/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,97 +1,98 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   client.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   SDK Client module
-'''
+"""
 # pylint: disable=C0103
 
-import os
 import copy
+import os
 from abc import ABC
 from typing import List
 
 from datature.nexus import models
 from datature.nexus.api.project import Project
 from datature.nexus.client_context import ClientContext
 
 
 class Client(ABC):
     """Initialize the Datature client with a secret key and an API endpoint.
 
     Parameters:
         secret_key (str): The secret key used for authentication with the Datature API.
         endpoint (str): The base URL for the Datature API.
-            Defaults to the value of the DATATURE_API_BASE_URL environment variable, 
+            Defaults to the value of the DATATURE_API_BASE_URL environment variable,
             or "https://api.datature.io" if the environment variable is not set.
     """
 
     _context: ClientContext
 
-    def __init__(self,
-                 secret_key: str,
-                 endpoint: str = os.getenv("DATATURE_API_BASE_URL",
-                                           "https://api.datature.io")):
-        """ Initialize """
+    def __init__(
+        self,
+        secret_key: str,
+        endpoint: str = os.getenv("DATATURE_API_BASE_URL", "https://api.datature.io"),
+    ):
+        """Initialize"""
         self._context = ClientContext(secret_key, endpoint)
 
     def get_info(self) -> models.Workspace:
         """Retrieve this workspace.
 
         :return: A msgspec struct containing the workspace information with the following structure:
 
             .. code-block:: python
 
                 Workspace(
-                    id='ws_1c8aab980f174b0296c7e35e88665b13', 
-                    name="Raighne's Workspace", 
-                    owner='user_6323fea23e292439f31c58cd', 
+                    id='ws_1c8aab980f174b0296c7e35e88665b13',
+                    name="Raighne's Workspace",
+                    owner='user_6323fea23e292439f31c58cd',
                     tier='Developer',
                     create_date=1701927649302
                 )
 
         :example:
 
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 client = Client("5aa41e8ba........")
                 client.get_info()
         """
-        return self._context.requester.GET("/workspace",
-                                           response_type=models.Workspace)
+        return self._context.requester.GET("/workspace", response_type=models.Workspace)
 
     def list_projects(self) -> List[Project]:
-        """ List all projects under this workspace.
+        """List all projects under this workspace.
 
         :return: A List of project class instances.
         :example:
 
             .. code-block:: python
 
                 from datature.nexus import Client
 
                 projects = Client("5aa41e8ba........").list_projects()
 
                 for project in projects:
                     print(project.get_info())
         """
-        projects = self._context.requester.GET("/workspace/projects",
-                                               response_type=models.Projects)
+        projects = self._context.requester.GET(
+            "/workspace/projects", response_type=models.Projects
+        )
 
         projects_res = []
         for project in projects:
             project_context = copy.deepcopy(self._context)
             project_context.project_id = project.id
             projects_res.append(Project(project_context))
```

### Comparing `datature-1.6.0/datature/nexus/client_context.py` & `datature-1.7.0/datature/nexus/client_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   client_context.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   SDK Client module
-'''
+"""
 # pylint: disable=R0903
 
+
 from datature.nexus.requester import Requester
 
 
 class ClientContext:
     """
     Client context for Datature SDK.
     """
@@ -48,14 +49,15 @@
         :type: str
         """
         self._project_id = value
 
 
 class RestContext:
     """Datature REST Context."""
+
     _context: ClientContext
 
     def __init__(self, context: ClientContext):
         """Create a REST Context.
 
         :param context: REST context used to make REST calls.
         """
```

### Comparing `datature-1.6.0/datature/nexus/config.py` & `datature-1.7.0/datature/nexus/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   config.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   SDK config module
-'''
+"""
+
 
 # Default configurations
 ASSET_UPLOAD_SESSION_BATCH_SIZE: int = 5000
 ANNOTATION_IMPORT_SESSION_MAX_SIZE: int = 100000
 ANNOTATION_IMPORT_SESSION_BATCH_SIZE: int = 1000
-ANNOTATION_IMPORT_SESSION_BATCH_BYTES: int = 1.024e+9
+ANNOTATION_IMPORT_SESSION_BATCH_BYTES: int = 1.024e9
 OPERATION_LOOPING_TIMEOUT_SECONDS: int = 36000
 OPERATION_LOOPING_DELAY_SECONDS: int = 8
 REQUEST_TIME_OUT_SECONDS = (60, 3600)
```

### Comparing `datature-1.6.0/datature/nexus/error.py` & `datature-1.7.0/datature/nexus/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   error.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Error Class module
-'''
+"""
 
 
 class Error(Exception):
     """Error Class."""
 
     def __init__(
         self,
@@ -28,17 +28,19 @@
         self.detail = detail
 
 
 class ErrorWithCode(Error):
     """HTTP Error Class."""
 
     def __repr__(self):
-        return (f"{self.__class__.__name__}"
-                f"(message={self.message}, "
-                f"detail={self.detail})")
+        return (
+            f"{self.__class__.__name__}"
+            f"(message={self.message}, "
+            f"detail={self.detail})"
+        )
 
 
 class BadRequestError(ErrorWithCode):
     """BadRequestError http_code: 400"""
 
 
 class UnauthorizedError(ErrorWithCode):
```

### Comparing `datature-1.6.0/datature/nexus/medical/__init__.py` & `datature-1.7.0/datature/nexus/medical/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   __init__.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Processor package
-'''
+"""
 
-from os import PathLike
 import pathlib
+from os import PathLike
+
 from .dicom_processor import DicomProcessor
 from .nii_processor import NiiProcessor
 
 
 def get_processor(file_path: PathLike):
     """Get processor"""
```

### Comparing `datature-1.6.0/datature/nexus/medical/base_processor.py` & `datature-1.7.0/datature/nexus/medical/base_processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   base_processor.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Base Processor module
-'''
+"""
 
-from typing import List
 from abc import ABC, abstractmethod
+from typing import List
 
 
 class BaseProcessor(ABC):
     """Base processor class"""
 
     @abstractmethod
     def valid(self, request_data):
```

### Comparing `datature-1.6.0/datature/nexus/medical/dicom_processor.py` & `datature-1.7.0/datature/nexus/medical/dicom_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   dicom_processor.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Dicom Processor
-'''
+"""
 
 import tempfile
-from typing import List
-from pathlib import Path
 from os import makedirs, path
+from pathlib import Path
+from typing import List
 
 import cv2
 from pydicom import config, dcmread
-
 from datature.nexus import error
+
 from .base_processor import BaseProcessor
 
 # Enforcing Valid DICOM
 config.settings.reading_validation_mode = config.RAISE
 
 
 class DicomProcessor(BaseProcessor):
@@ -59,26 +59,28 @@
         if not path.exists(video_output):
             makedirs(video_output)
 
         dicom_data = dcmread(file_path)
 
         four_cc = cv2.VideoWriter_fourcc(*"mp4v")
 
-        number_of_frames = int(dicom_data.get('NumberOfFrames', 1))
+        number_of_frames = int(dicom_data.get("NumberOfFrames", 1))
 
         # if only contain one image, convert to image.
         if number_of_frames == 1:
-            cv2.imwrite(f"{video_output}/{file_name}.png",
-                        dicom_data.pixel_array)
+            cv2.imwrite(f"{video_output}/{file_name}.png", dicom_data.pixel_array)
 
             return [f"{video_output}/{file_name}.png"]
 
-        video_writer = cv2.VideoWriter(f"{video_output}/{file_name}.mp4",
-                                       four_cc, 30.0,
-                                       (dicom_data.Rows, dicom_data.Columns))
+        video_writer = cv2.VideoWriter(
+            f"{video_output}/{file_name}.mp4",
+            four_cc,
+            30.0,
+            (dicom_data.Rows, dicom_data.Columns),
+        )
 
         for _, image in enumerate(dicom_data.pixel_array):
             new_image = cv2.cvtColor(image, cv2.COLOR_GRAY2RGB)
             video_writer.write(new_image)
 
         video_writer.release()
```

### Comparing `datature-1.6.0/datature/nexus/medical/nii_processor.py` & `datature-1.7.0/datature/nexus/medical/nii_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   nii_processor.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Nii Processor
-'''
+"""
 
 import shutil
 import tempfile
-from typing import List
-from pathlib import Path
 from os import makedirs, path
+from pathlib import Path
+from typing import List
 
 import cv2
-import numpy as np
-import nibabel as nib
 import matplotlib.image as mpImage
-
+import nibabel as nib
+import numpy as np
 from datature.nexus import error
+
 from .base_processor import BaseProcessor
 
 
 class NiiProcessor(BaseProcessor):
     """Nii processor class"""
 
     def valid(self, request_data):
@@ -37,28 +37,26 @@
 
         :param request_data: The request data, include file path.
         :return: None.
         """
         file_path = request_data.get("file")
 
         if not file_path:
-            raise error.BadRequestError(
-                "Required field, must include file path")
+            raise error.BadRequestError("Required field, must include file path")
 
     def process(self, request_data) -> List[str]:
         """Start process file to asset video
 
         :param request_data: The request data, include file path.
         :return: str: The generate video path.
         """
         out_path = tempfile.mkdtemp()
 
         file_path = request_data.get("file")
-        orientation = request_data.get("options",
-                                       {}).get("nifti_orientation", None)
+        orientation = request_data.get("options", {}).get("nifti_orientation", None)
 
         file_name = Path(file_path).stem
 
         video_output = path.join(out_path, file_name)
 
         if not path.exists(video_output):
             makedirs(video_output)
@@ -66,68 +64,69 @@
         scan = nib.load(file_path)
 
         # Read data and get scan's shape
         scan_array = scan.get_fdata()
 
         # Get image pixel
         scan_headers = scan.header
-        pix_dim = scan_headers['pixdim'][1:4]
+        pix_dim = scan_headers["pixdim"][1:4]
 
         # Calculate new image dimensions from aspect ratio
         new_scan_dims = np.multiply(scan_array.shape, pix_dim)
-        new_scan_dims = (round(new_scan_dims[0]), round(new_scan_dims[1]),
-                         round(new_scan_dims[2]))
+        new_scan_dims = (
+            round(new_scan_dims[0]),
+            round(new_scan_dims[1]),
+            round(new_scan_dims[2]),
+        )
 
         # if client provide the orientation
         if orientation and orientation in ["x", "y", "z"]:
             output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
 
-            self.__write_video(scan_array, new_scan_dims, orientation,
-                               output_file_path)
+            self.__write_video(scan_array, new_scan_dims, orientation, output_file_path)
 
             return [output_file_path]
 
         # if not then save all orientations
         output_file_paths = []
         for orientation in ["x", "y", "z"]:
             output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
 
-            self.__write_video(scan_array, new_scan_dims, orientation,
-                               output_file_path)
+            self.__write_video(scan_array, new_scan_dims, orientation, output_file_path)
 
             output_file_paths.append(output_file_path)
         return output_file_paths
 
     def __write_video(self, scan_array, scan_dims, orientation, saved_path):
         """Write video to file
 
         :param scan_array: The NIfTI scan array data.
         :param scan_dims: The image dimensions of the file.
         :param orientation: The orientation of the pics.
         :param saved_path: The saved file path.
         """
-        axis = {'x': 0, 'y': 1, 'z': 2}[orientation]
+        axis = {"x": 0, "y": 1, "z": 2}[orientation]
         size = {
-            'x': [scan_dims[2], scan_dims[1]],
-            'y': [scan_dims[2], scan_dims[0]],
-            'z': [scan_dims[1], scan_dims[0]]
+            "x": [scan_dims[2], scan_dims[1]],
+            "y": [scan_dims[2], scan_dims[0]],
+            "z": [scan_dims[1], scan_dims[0]],
         }[orientation]
 
         four_cc = cv2.VideoWriter_fourcc(*"mp4v")
         video_writer = cv2.VideoWriter(saved_path, four_cc, 30.0, size)
 
         cache_path = tempfile.mkdtemp()
 
         for i in range(scan_array.shape[axis]):
             # Get slice along the correct axis and resize
             slice_axis = scan_array.take(i, axis=axis)
 
             # Convert to Grayscale and write to video file
-            mpImage.imsave(f'{cache_path}/{orientation}-{str(i)}.png',
-                           slice_axis,
-                           cmap='gray')
-            new_image = cv2.imread(f'{cache_path}/{orientation}-{str(i)}.png')
+            mpImage.imsave(
+                f"{cache_path}/{orientation}-{str(i)}.png", slice_axis, cmap="gray"
+            )
+            new_image = cv2.imread(f"{cache_path}/{orientation}-{str(i)}.png")
 
             new_image = cv2.resize(new_image, size)
             video_writer.write(new_image)
         shutil.rmtree(cache_path)
         video_writer.release()
```

### Comparing `datature-1.6.0/datature/nexus/models.py` & `datature-1.7.0/datature/nexus/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   models.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   SDK response msgspec model
-'''
+"""
 # pylint: disable=R0903,C0302,C0103
 
-from typing import Generic, TypeVar, Optional, List, Dict, Union, Any, Tuple
+from typing import Any, Dict, Generic, List, Optional, Tuple, TypeVar, Union
 
 import msgspec
 
 T = TypeVar("T")
 
 
 class NexusStruct(msgspec.Struct):
@@ -59,14 +59,15 @@
     Attributes:
         id (str): Unique identifier of the workspace.
         name (str): Name of the workspace.
         owner (str): Owner of the workspace.
         tier (str): The str or level of the workspace.
         create_date (int): The creation date of the workspace as an integer timestamp.
     """
+
     id: str
     name: str
     owner: str
     tier: str
     create_date: int = msgspec.field(name="createDate")
 
 
@@ -75,59 +76,65 @@
     Describes a checkpoint configuration in a training process.
 
     Attributes:
         strategy (str): Strategy for checkpoint creation (e.g., interval-based).
         evaluation_interval (int): Interval at which evaluations are performed.
         metric (Optional[str]): Metric used for evaluation.
     """
+
     strategy: str
     evaluation_interval: int = msgspec.field(name="evaluationInterval")
     metric: Optional[str] = None
 
 
 class TagsCountItem(NexusStruct):
     """
     Describes a tag count item in a project, indicating the number of occurrences of a specific tag.
 
     Attributes:
         name (str): The name of the tag.
         count (int): The count of how many times the tag appears.
     """
+
     name: str
     count: int
 
 
 class AssetAnnotationsStatistic(NexusStruct):
     """
     Represents statistical data related to a project.
 
     Attributes:
         tags_count (Optional[List[TagsCountItem]]): A list of tag count items.
         total_annotations (Optional[int]): Total number of annotations.
     """
-    tags_count: Optional[List[TagsCountItem]] = msgspec.field(name="tagsCount",
-                                                              default=None)
-    total_annotations: Optional[int] = msgspec.field(name="totalAnnotations",
-                                                     default=None)
+
+    tags_count: Optional[List[TagsCountItem]] = msgspec.field(
+        name="tagsCount", default=None
+    )
+    total_annotations: Optional[int] = msgspec.field(
+        name="totalAnnotations", default=None
+    )
 
 
 class AnnotationStatistic(AssetAnnotationsStatistic):
     """
     Represents statistical data related to a project.
 
     Attributes:
         tags_count (Optional[List[TagsCountItem]]): A list of tag count items.
         total_assets (Optional[int]): Total number of assets.
         annotated_assets (Optional[int]): Number of annotated assets.
         total_annotations (Optional[int]): Total number of annotations.
     """
-    total_assets: Optional[int] = msgspec.field(name="totalAssets",
-                                                default=None)
-    annotated_assets: Optional[int] = msgspec.field(name="annotatedAssets",
-                                                    default=None)
+
+    total_assets: Optional[int] = msgspec.field(name="totalAssets", default=None)
+    annotated_assets: Optional[int] = msgspec.field(
+        name="annotatedAssets", default=None
+    )
 
 
 class Project(NexusStruct):
     """
     Represents a project within a workspace, detailing its structure and attributes.
 
     Attributes:
@@ -137,14 +144,15 @@
         type (str): The type of the project.
         create_date (int): Creation date of the project as an integer timestamp.
         localization (str): Localization or region information of the project.
         tags (List[str]): List of tags associated with the project.
         groups (List[str]): List of groups associated with the project.
         statistic (Optional[Statistic]): Statistical data related to the project.
     """
+
     id: str
     name: str
     workspace_id: str = msgspec.field(name="workspaceId")
     type: str
     create_date: int = msgspec.field(name="createDate")
     localization: str
     tags: List[str]
@@ -162,14 +170,15 @@
     Attributes:
         id (str): Unique identifier of the user.
         access_type (str): The type of access the user has (e.g., admin, viewer).
         email (str): The email address of the user.
         nickname (str): The nickname or username of the user.
         picture (str): URL of the user's profile picture.
     """
+
     id: str
     access_type: str = msgspec.field(name="accessType")
     email: str
     nickname: str
     picture: str
 
 
@@ -182,55 +191,59 @@
 
     Attributes:
         total_loss (Optional[float]): The total loss metric.
         classification_loss (Optional[float]): Loss metric specific to classification tasks.
         localization_loss (Optional[float]): Loss metric specific to localization tasks.
         regularization_loss (Optional[float]): The regularization loss metric.
     """
+
     total_loss: Optional[float] = msgspec.field(name="totalLoss", default=None)
     classification_loss: Optional[float] = msgspec.field(
-        name="classificationLoss", default=None)
-    localization_loss: Optional[float] = msgspec.field(name="localizationLoss",
-                                                       default=None)
+        name="classificationLoss", default=None
+    )
+    localization_loss: Optional[float] = msgspec.field(
+        name="localizationLoss", default=None
+    )
     regularization_loss: Optional[float] = msgspec.field(
-        name="regularizationLoss", default=None)
+        name="regularizationLoss", default=None
+    )
 
 
 class DatasetSettings(NexusStruct):
     """
     Configuration settings for a dataset.
 
     Attributes:
         split_ratio (float): The ratio used to split the dataset.
         shuffle (bool): Whether to shuffle the dataset.
         seed (int): Seed for randomization, if shuffle is enabled.
         using_sliding_window (bool): Indicates whether a sliding window is used (default is False).
     """
+
     split_ratio: float = msgspec.field(name="splitRatio")
     shuffle: bool
     seed: int
-    using_sliding_window: bool = msgspec.field(name="usingSlidingWindow",
-                                               default=False)
+    using_sliding_window: bool = msgspec.field(name="usingSlidingWindow", default=False)
 
 
 class InsightDataset(NexusStruct):
     """
     Representation of a dataset with additional insights.
 
     Attributes:
         data_type (str): Type of data in the dataset.
         num_classes (int): Number of classes in the dataset.
         average_annotations (float): Average annotations per asset.
         total_assets (int): Total number of assets in the dataset.
         settings (DatasetSettings): Configuration settings for the dataset.
     """
+
     data_type: str = msgspec.field(name="dataType")
     num_classes: int = msgspec.field(name="numClasses", default=None)
-    average_annotations: float = msgspec.field(name="averageAnnotations",
-                                               default=None)
+    average_annotations: float = msgspec.field(name="averageAnnotations", default=None)
     total_assets: int = msgspec.field(name="totalAssets", default=None)
     settings: Union[DatasetSettings, None] = None
 
 
 class InsightModel(NexusStruct):
     """
     Representation of a machine learning model with training parameters.
@@ -240,14 +253,15 @@
         batch_size (int): Batch size used during training.
         training_steps (int): Number of training steps.
         max_detection_per_class (int): Maximum detections per class.
         solver (str): Solver used for training.
         learning_rate (float): Learning rate for the optimizer.
         momentum (float): Momentum for the optimizer.
     """
+
     name: str
     batch_size: int = msgspec.field(name="batchSize")
     training_steps: int = msgspec.field(name="trainingSteps")
     max_detection_per_class: int = msgspec.field(name="maxDetectionPerClass")
     solver: str
     learning_rate: float = msgspec.field(name="learningRate")
     momentum: float
@@ -259,14 +273,15 @@
 
     Attributes:
         id (str): Unique identifier of the artifact.
         is_training (bool): Indicates whether the artifact is related to training.
         step (int): Step number in the process.
         metric (ArtifactMetric): Metrics associated with the artifact.
     """
+
     id: str
     is_training: bool = msgspec.field(name="isTraining")
     step: int
     metric: ArtifactMetric
 
 
 class ProjectInsight(NexusStruct):
@@ -278,14 +293,15 @@
         run_id (str): Identifier for the run.
         dataset (InsightDataset): Dataset associated with the insight.
         model (InsightModel): Model associated with the insight.
         checkpoint (RunCheckpoint): Checkpointing configuration used during training.
         artifact: InsightArtifact: Artifact associated with the insight.
         create_date (int): Creation date of the insight.
     """
+
     flow_title: str = msgspec.field(name="flowTitle")
     run_id: str = msgspec.field(name="runId")
     dataset: InsightDataset
     model: InsightModel
     checkpoint: RunCheckpoint
     artifact: InsightArtifact
     create_date: int = msgspec.field(name="createDate")
@@ -299,14 +315,15 @@
     Represents a signed URL for downloading, including its method and expiry information.
 
     Attributes:
         method (str): HTTP method to be used with the URL (e.g., GET).
         expiry_date (int): Expiration date of the download URL as an integer timestamp.
         url (str): The signed URL for download.
     """
+
     method: str
     expiry_date: int = msgspec.field(name="expiryDate")
     url: str
 
 
 class AssetMetadata(NexusStruct):
     """
@@ -317,23 +334,23 @@
         mime_type (str): The MIME type of the file.
         height (int): The height of the image or asset in pixels.
         width (int): The width of the image or asset in pixels.
         groups (List[str]): List of groups associated with the asset.
         custom_metadata (Optional[Dict[str, Union[str, int, float, bool]]]):
             Additional custom metadata for the asset.
     """
+
     file_size: int = msgspec.field(name="fileSize")
     mime_type: str = msgspec.field(name="mimeType")
     height: int
     width: int
     groups: List[str]
-    custom_metadata: Optional[Dict[str, Union[str, int, float,
-                                              bool]]] = msgspec.field(
-                                                  name="customMetadata",
-                                                  default=None)
+    custom_metadata: Optional[Dict[str, Union[str, int, float, bool]]] = msgspec.field(
+        name="customMetadata", default=None
+    )
 
 
 class Asset(NexusStruct):
     """
     Describes an asset within a project, including its metadata and associated data.
 
     Attributes:
@@ -342,14 +359,15 @@
         project (str): The project to which this asset belongs.
         status (str): The status of the asset.
         create_date (int): The creation date of the asset as an integer timestamp.
         url (str): URL where the asset is located.
         metadata (AssetMetadata): Metadata associated with the asset.
         statistic (Optional[AssetAnnotationsStatistic]): Statistical data related to the asset.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     filename: str
     status: str
     create_date: int = msgspec.field(name="createDate")
     url: str
     metadata: AssetMetadata
@@ -361,27 +379,29 @@
     Generic structure for paginated responses, providing navigation to other pages.
 
     Attributes:
         next_page (Optional[str]): URL to the next page of results.
         prev_page (Optional[str]): URL to the previous page of results.
         data (List[T]): List of data items on the current page.
     """
+
     next_page: Optional[str] = msgspec.field(name="nextPage", default=None)
     prev_page: Optional[str] = msgspec.field(name="prevPage", default=None)
     data: List[T] = None
 
 
 class DeleteResponse(NexusStruct):
     """
     Structure representing the response to a delete request.
 
     Attributes:
         deleted (bool): Indicates whether the deletion was successful.
         id (Optional[str]): The ID of the deleted item, if applicable.
     """
+
     deleted: bool
     id: Optional[str] = None
 
 
 class AssetGroupStatistic(NexusStruct):
     """
     Represents statistics for a group of assets, providing various counts.
@@ -389,34 +409,35 @@
     Attributes:
         total_assets (Optional[int]): Total number of assets in the group.
         annotated_assets (Optional[int]): Number of annotated assets.
         reviewed_assets (Optional[int]): Number of reviewed assets.
         to_fixed_assets (Optional[int]): Number of assets marked to be fixed.
         completed_assets (Optional[int]): Number of completed assets.
     """
-    total_assets: Optional[int] = msgspec.field(name="totalAssets",
-                                                default=None)
-    annotated_assets: Optional[int] = msgspec.field(name="annotatedAssets",
-                                                    default=None)
-    reviewed_assets: Optional[int] = msgspec.field(name="reviewedAssets",
-                                                   default=None)
-    to_fixed_assets: Optional[int] = msgspec.field(name="toFixedAssets",
-                                                   default=None)
-    completed_assets: Optional[int] = msgspec.field(name="completedAssets",
-                                                    default=None)
+
+    total_assets: Optional[int] = msgspec.field(name="totalAssets", default=None)
+    annotated_assets: Optional[int] = msgspec.field(
+        name="annotatedAssets", default=None
+    )
+    reviewed_assets: Optional[int] = msgspec.field(name="reviewedAssets", default=None)
+    to_fixed_assets: Optional[int] = msgspec.field(name="toFixedAssets", default=None)
+    completed_assets: Optional[int] = msgspec.field(
+        name="completedAssets", default=None
+    )
 
 
 class AssetGroup(NexusStruct):
     """
     Describes a group of assets within a project, along with their statistics.
 
     Attributes:
         group (str): The name of the group.
         statistic (Optional[AssetGroupStatistic]): Statistical data for the group.
     """
+
     group: str = msgspec.field(name="group", default=None)
     statistic: Optional[AssetGroupStatistic] = None
 
 
 AssetGroups = List[AssetGroup]
 
 
@@ -426,14 +447,15 @@
 
     Attributes:
         method (str): HTTP method to be used with the URL (e.g., GET, POST).
         url (str): The signed URL.
         headers (Any): Headers required for accessing the URL.
         expiry_date (Optional[int]): Expiration date of the signed URL as an integer timestamp.
     """
+
     method: str
     url: str
     headers: Dict
     expiry_date: Optional[int] = msgspec.field(name="expiryDate", default=None)
 
 
 class UploadSessionAssetMetadata(NexusStruct):
@@ -442,41 +464,44 @@
 
     Attributes:
         filename (str): Name of the file.
         mime (str): MIME type of the file.
         size (int): Size of the file in bytes.
         crc32c (int): CRC32C checksum of the file for data integrity.
     """
+
     filename: str
     mime: str
     size: int
     crc32c: int
 
 
 class UploadSessionAssetItem(NexusStruct):
     """
     Represents an individual asset item within an upload session.
 
     Attributes:
         metadata (UploadSessionAssetMetadata): Metadata of the asset to be uploaded.
         upload (UploadSignedUrl): Signed URL for uploading the asset.
     """
+
     metadata: UploadSessionAssetMetadata
     upload: UploadSignedUrl
 
 
 class UploadSession(NexusStruct):
     """
     Represents an upload session, including its identifier and the assets to be uploaded.
 
     Attributes:
         id (str): Unique identifier of the upload session.
         op_id (str): Operation identifier for the session.
         assets (List[UploadSessionAssetItem]): List of assets included in the session.
     """
+
     id: str
     op_id: str = msgspec.field(name="opId")
     assets: List[UploadSessionAssetItem]
 
 
 class ArtifactModel(NexusStruct):
     """
@@ -487,14 +512,15 @@
         artifact_id (str): Identifier of the artifact associated with the model.
         status (str): Current status of the model.
         format (str): Format of the model.
         quantization (str): Quantization of the model.
         create_date (int): Creation date of the model as an integer timestamp.
         download (Optional[DownloadSignedUrl]): Signed URL for downloading the model, if available.
     """
+
     id: str
     artifact_id: str = msgspec.field(name="artifactId")
     status: str
     format: str
     quantization: str
     create_date: int = msgspec.field(name="createDate")
     download: Optional[DownloadSignedUrl] = None
@@ -504,36 +530,37 @@
 
 
 class ArtifactExportOptimizations(NexusStruct):
     """
     Represents optimization options for artifact export.
 
     Attributes:
-        quantization (Union[List[str], str]): Quantization options for optimization. 
+        quantization (Union[List[str], str]): Quantization options for optimization.
             Can be a list of quantization options or a single quantization option.
     """
 
     quantization: Union[List[str], str]
 
 
 class ArtifactExportOptions(NexusStruct):
     """
     Represents options for exporting an artifact.
 
     Attributes:
         format (str): Format in which the artifact should be exported.
         optimizations (ArtifactExportOptimizations): Optimization options for the export.
-        default_optimizations (ArtifactExportOptimizations): 
+        default_optimizations (ArtifactExportOptimizations):
             Default optimization options for the export.
     """
 
     format: str
     optimizations: ArtifactExportOptimizations
     default_optimizations: ArtifactExportOptimizations = msgspec.field(
-        name="defaultOptimizations")
+        name="defaultOptimizations"
+    )
 
 
 class Artifact(InsightArtifact):
     """
     Represents an artifact within a project, detailing its properties and associated metrics.
 
     Attributes:
@@ -548,84 +575,87 @@
         metric (ArtifactMetric): Metrics associated with the artifact.
         is_deployed (bool): Indicates whether the artifact is deployed.
         model_name (str): Name of the model associated with the artifact.
         exportable_formats (List[str]): List of exportable formats for the artifact.
         exports (Optional[List[ArtifactModel]]): List of exported
             models associated with the artifact.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     run_id: str = msgspec.field(name="runId")
     is_training: bool = msgspec.field(name="isTraining")
     step: int
     flow_title: str = msgspec.field(name="flowTitle")
     artifact_name: str = msgspec.field(name="artifactName")
     create_date: int = msgspec.field(name="createDate")
     metric: ArtifactMetric
     is_deployed: bool = msgspec.field(name="isDeployed")
     model_name: str = msgspec.field(name="modelName")
-    export_options: List[ArtifactExportOptions] = msgspec.field(
-        name="exportOptions")
+    export_options: List[ArtifactExportOptions] = msgspec.field(name="exportOptions")
     exports: Optional[List[ArtifactModel]] = None
 
 
 Artifacts = List[Artifact]
 
 
 class RunAccelerator(NexusStruct):
     """
     Describes a training accelerator, specifying its name and count.
 
     Attributes:
         name (str): Name of the accelerator (e.g., GPU type).
         count (int): Number of accelerator units.
     """
+
     name: str
     count: int
 
 
 class RunLimit(NexusStruct):
     """
     Represents a limit on a specific metric during training.
 
     Attributes:
         metric (str): The name of the metric to which the limit applies.
         value (int): The value of the limit for the specified metric.
     """
+
     metric: str
     value: int
 
 
 class RunExecution(NexusStruct):
     """
     Describes the execution parameters for a training process.
 
     Attributes:
         accelerator (Optional[RunAccelerator]): The accelerator used for training, if any.
         checkpoint (Optional[RunCheckpoint]): Checkpointing configuration used during training.
         limit (Optional[RunLimit]): Limit configuration applied to the training process.
     """
+
     accelerator: Optional[RunAccelerator] = None
     checkpoint: Optional[RunCheckpoint] = None
     limit: Optional[RunLimit] = None
 
 
 class RunFeatures(NexusStruct):
     """
     Specifies the additional features enabled for the training process.
 
     Attributes:
         preview (bool): Indicates whether a preview feature is enabled.
         matrix (bool): Indicates whether a matrix feature is enabled.
         using_sliding_window (bool): Indicates whether a sliding window feature is enabled.
     """
+
     preview: bool = False
     matrix: bool = False
-    using_sliding_window: bool = msgspec.field(name="usingSlidingWindow",
-                                               default=False)
+    using_sliding_window: bool = msgspec.field(name="usingSlidingWindow", default=False)
 
 
 class RunStatus(NexusStruct):
     """
     Represents the status of a machine learning model run.
 
     Attributes:
@@ -649,14 +679,15 @@
         flow_id (str): Identifier of the flow associated with this training.
         execution (RunExecution): Execution details of the training process.
         create_date (int): Creation date of the training process.
         update_date (int): The date when the training was last updated.
         features (Optional[RunFeatures]): Additional features related to the training.
         logs (Optional[List[str]]): Log entries associated with the training process.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     flow_id: str = msgspec.field(name="flowId")
     execution: RunExecution
     status: RunStatus
     create_date: int = msgspec.field(name="createDate")
     update_date: int = msgspec.field(name="updateDate")
@@ -671,38 +702,41 @@
     """
     Represents the logs associated with a specific training process.
 
     Attributes:
         id (str): Unique identifier for the training logs.
         logs (List[Any]): A list of log entries recorded during the training process.
     """
+
     id: str
     logs: List[Any]
 
 
 class RunConfusionMatrix(NexusStruct):
     """
     Represents a confusion matrix for a training process, useful for evaluating model performance.
 
     Attributes:
         data (Any): The data constituting the confusion matrix, usually a multidimensional array.
     """
+
     data: Any
 
 
 class Tag(NexusStruct):
     """
     Describes a tag used in a project, typically for categorization or labeling.
 
     Attributes:
         index (int): The index or identifier of the tag.
         name (str): The name of the tag.
         color (Optional[str]): The color of the tag.
         description (Optional[str]): The description of the tag.
     """
+
     index: int
     name: str
     color: Optional[str] = None
     description: Optional[str] = None
 
 
 Tags = List[Tag]
@@ -715,14 +749,15 @@
     Attributes:
         id (str): Unique identifier of the workflow.
         project_id (str): Identifier of the project associated with this workflow.
         title (str): Title of the workflow.
         create_date (int): Creation date of the workflow.
         update_date (int): The date when the workflow was last updated.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     title: str
     create_date: int = msgspec.field(name="createDate")
     update_date: int = msgspec.field(name="updateDate")
 
 
@@ -755,81 +790,87 @@
         asset_id (str): Identifier of the asset to which this annotation is linked.
         tag (str): Tag or label associated with the annotation.
         bound_type (str): The type of boundary used for the annotation (e.g., box, polygon).
         create_date (int): Creation date of the annotation as an integer timestamp.
         bound (Union[[], List[Tuple[float, float]], List[Tuple[float, float, int]]]):
             The coordinates defining the boundary of the annotation.
         ontology_id (Optional[str]): Identifier of the ontology associated with the annotation.
-        attributes (Optional[List[OntologyAttributeValue]]): 
+        attributes (Optional[List[OntologyAttributeValue]]):
             List of attributes associated with the annotation.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     asset_id: str = msgspec.field(name="assetId")
     tag: str
     bound_type: str = msgspec.field(name="boundType")
     bound: List[Union[Any, Tuple[float, float], Tuple[float, float, int]]]
     create_date: int = msgspec.field(name="createDate", default=None)
     ontology_id: str = msgspec.field(name="ontologyId", default=None)
-    attributes: List[OntologyAttributeValue] = msgspec.field(name="attributes",
-                                                             default=None)
+    attributes: List[OntologyAttributeValue] = msgspec.field(
+        name="attributes", default=None
+    )
 
 
 class DeploymentScaling(NexusStruct):
     """
     Describes the scaling configuration for a deployment, such as the number of instances.
 
     Attributes:
         num_instances (int): The number of instances to be used in the deployment.
         mode (str): The scaling mode, describing how scaling is managed (e.g., manual, auto).
     """
+
     replicas: int
     mode: str
 
 
 class DeploymentResources(NexusStruct):
     """
     Represents the resources allocated for a deployment, including CPU, RAM, and GPU.
 
     Attributes:
         cpu (int): The amount of CPU allocated for the deployment.
         ram (int): The amount of RAM allocated for the deployment, typically in megabytes.
         GPU_T4 (int): The number of T4 GPUs allocated for the deployment.
     """
+
     cpu: int
     ram: int
     GPU_T4: Optional[int] = None
 
 
 class DeploymentHistoryVersion(NexusStruct):
     """
     Represents a specific version within the deployment history.
 
     Attributes:
         version_tag (str): The tag identifying the version.
             This is typically used for version control and identification.
-        artifact_id (str): The identifier of the artifact 
+        artifact_id (str): The identifier of the artifact
             associated with this version of the deployment.
         update_date (int): The date and time when this version was last updated,
             represented in Unix milliseconds format.
     """
+
     version_tag: str = msgspec.field(name="versionTag")
     artifact_id: str = msgspec.field(name="artifactId")
     update_date: int = msgspec.field(name="updateDate")
 
 
 class DeploymentStatus(NexusStruct):
     """
     Represents the status of a deployed model.
 
     Attributes:
         overview (str): An overview of the deployment status.
         message (str): A message providing additional information about the deployment status.
         update_data (int): The date of the last update to the deployment status.
     """
+
     overview: str
     message: str
     update_data: int = msgspec.field(name="updateDate")
 
 
 class Deployment(NexusStruct):
     """
@@ -844,21 +885,23 @@
         create_date (int): Creation date of the deployment.
         update_date (int): The date when the deployment was last updated.
         scaling (DeploymentScaling): The scaling configuration for the deployment.
         resources (DeploymentResources): The resources allocated for the deployment.
         status (DeploymentStatus): Current status of the deployment.
         url (Optional[str]): URL where the deployment is accessible, if applicable.
     """
+
     id: str
     name: str
     project_id: str = msgspec.field(name="projectId")
     artifact_id: str = msgspec.field(name="artifactId")
     version_tag: str = msgspec.field(name="versionTag")
     history_versions: List[DeploymentHistoryVersion] = msgspec.field(
-        name="historyVersions")
+        name="historyVersions"
+    )
     resources: Optional[DeploymentResources]
     scaling: Optional[DeploymentScaling]
     status: DeploymentStatus
     create_date: int = msgspec.field(name="createDate")
     update_date: int = msgspec.field(name="updateDate")
     url: Optional[str] = None
 
@@ -884,41 +927,43 @@
     Represents the count of files in various processing states within an import session.
 
     Attributes:
         Processing (int): The number of files currently being processed.
         Processed (int): The number of files that have been processed.
         FailedProcess (int): The number of files that failed during processing.
     """
+
     Processing: int
     Processed: int
     FailedProcess: int
 
 
 class ImportSessionStatusAnnotations(NexusStruct):
     """
     Represents the status of annotations within an import session.
 
     Attributes:
         with_status (ImportSessionAnnotationStatus):
             The count of annotations in different processing states.
     """
-    with_status: ImportSessionAnnotationStatus = msgspec.field(
-        name="withStatus")
+
+    with_status: ImportSessionAnnotationStatus = msgspec.field(name="withStatus")
 
 
 class ImportSessionStatusFiles(NexusStruct):
     """
     Represents the status of files within an import session.
 
     Attributes:
         total_size_bytes (int): The total size of all files in bytes.
         page_count (int): The number of pages of files.
         status_count (ImportSessionStatusFilesCount):
             The count of files in various processing states.
     """
+
     total_size_bytes: int = msgspec.field(name="totalSizeBytes")
     page_count: int = msgspec.field(name="pageCount")
     with_status: ImportSessionFilesStatus = msgspec.field(name="withStatus")
 
 
 class ImportSessionStatus(NexusStruct):
     """
@@ -949,14 +994,15 @@
         id (str): Unique identifier of the import session.
         project_id (str): Identifier of the project associated with this import session.
         status (Any): Current status of the import session.
         expiry_date (int): Expiration date of the import session as an integer timestamp.
         create_date (int): Creation date of the import session.
         update_date (int): The date when the import session was last updated.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     status: ImportSessionStatus
     expiry_date: int = msgspec.field(name="expiryDate")
     create_date: int = msgspec.field(name="createDate")
     update_date: int = msgspec.field(name="updateDate")
 
@@ -968,102 +1014,109 @@
     """
     Represents a file within an import session, including its name and upload URL.
 
     Attributes:
         filename (str): The name of the file to be imported.
         upload (UploadSignedUrl): The signed URL for uploading the file.
     """
+
     filename: str
     upload: UploadSignedUrl
 
 
 class InsertImportSessionFiles(NexusStruct):
     """
     Describes a batch of files to be inserted into an import session.
 
     Attributes:
         id (str): Unique identifier of the import session to which these files belong.
         project_id (str): Identifier of the project associated with these files.
         files (List[ImportSessionFile]): List of files to be included in the import session.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     files: List[ImportSessionFile]
 
 
 class ImportSessionLogLogItem(NexusStruct):
     """
     Represents a single log entry in an import session.
 
     Attributes:
         timestamp (float): The timestamp when the log entry was recorded.
         level (str): The severity level of the log entry (e.g., 'INFO', 'ERROR').
         message (str): The message content of the log entry.
     """
+
     timestamp: float
     level: str
     message: str
 
 
 class ImportSessionLog(NexusStruct):
     """
     Represents a collection of log entries for an import session.
 
     Attributes:
         id (str): Unique identifier of the import session.
         project_id (str): Identifier of the project associated with this import session.
         logs (List[ImportSessionLogLogItem]): A list of log entries for the import session.
     """
+
     id: str
     project_id: str = msgspec.field(name="projectId")
     logs: List[ImportSessionLogLogItem]
 
 
 class LocalArtifact(NexusStruct):
     """
     Represents a local artifact consisting of model and label files.
 
     Attributes:
         download_path (str): The path where the artifact is downloaded or stored locally.
         model_filename (str): The filename of the model file included in the artifact.
         label_filename (str): The filename of the label file included in the artifact.
     """
+
     download_path: str
     model_filename: str
     label_filename: str
 
 
 class ExportedAnnotations(NexusStruct):
     """
     Represents the exported annotations from a project or operation.
 
     Attributes:
         op_id (str):
             The identifier of the operation associated with the export of annotations.
         status (str):
             The current status of the exported annotations (e.g., 'completed', 'in-progress').
-        download (Optional[DownloadSignedUrl]): 
+        download (Optional[DownloadSignedUrl]):
             An optional URL for downloading the exported annotations, if available.
     """
+
     op_id: str = msgspec.field(name="opId")
     status: str
     download: Optional[DownloadSignedUrl] = None
 
 
 class LocalAnnotations(NexusStruct):
     """
-    Represents local annotations stored in the filesystem, 
+    Represents local annotations stored in the filesystem,
         including their download path and file names.
 
     Attributes:
-        download_path (str): 
+        download_path (str):
             The file system path where the annotations are downloaded or stored locally.
-        file_names (List[str]): 
+        file_names (List[str]):
             A list of file names for the annotation files stored at the download path.
     """
+
     download_path: str
     file_names: List[str]
 
 
 class OperationProgressWithStatus(NexusStruct):
     """
     Represents the count of operations in various states.
@@ -1071,43 +1124,46 @@
     Attributes:
         Queued (int): The number of operations that are queued.
         Running (int): The number of operations that are currently running.
         Finished (int): The number of operations that have finished.
         Cancelled (int): The number of operations that have been cancelled.
         Errored (int): The number of operations that have encountered errors.
     """
+
     Queued: int
     Running: int
     Finished: int
     Cancelled: int
     Errored: int
 
 
 class OperationProgress(NexusStruct):
     """
     Represents the progress status of an operation.
 
     Attributes:
         unit (str): The unit of measurement for the progress (e.g., 'files', 'percent').
-        with_status (OperationProgressWithStatus): 
+        with_status (OperationProgressWithStatus):
             The progress of the operation categorized by different statuses.
     """
+
     unit: str
     with_status: OperationProgressWithStatus = msgspec.field(name="withStatus")
 
 
 class OperationStatus(NexusStruct):
     """
     Represents the status of an operation.
 
     Attributes:
         overview (str): A brief overview or summary of the operation's status.
         message (str): A detailed message describing the current status of the operation.
         progress (OperationProgress): The progress of the operation.
     """
+
     overview: str
     message: str
     progress: OperationProgress
 
 
 class Operation(NexusStruct):
     """
@@ -1116,14 +1172,15 @@
     Attributes:
         id (str): The unique identifier of the operation.
         kind (str): The kind or type of the operation.
         status (OperationStatus): The current status of the operation.
         create_date (int): The timestamp when the operation was created.
         update_date (int): The timestamp when the operation was last updated.
     """
+
     id: str
     kind: str
     status: OperationStatus
     create_date: int = msgspec.field(name="createDate")
     update_date: int = msgspec.field(name="updateDate")
 
 
@@ -1179,12 +1236,11 @@
 
     id: str
     project_id: str = msgspec.field(name="projectId")
     index: int
     name: str
     color: Optional[str] = None
     description: Optional[str] = None
-    attributes: List[OntologyAttribute] = msgspec.field(name="attributes",
-                                                        default=None)
+    attributes: List[OntologyAttribute] = msgspec.field(name="attributes", default=None)
 
 
 Ontologies = List[Ontology]
```

### Comparing `datature-1.6.0/datature/nexus/requester.py` & `datature-1.7.0/datature/nexus/requester.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   requester.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   A wrapper to make HTTP requests
-'''
+"""
 
 import json
 import logging
 import platform
 
 import msgspec
 from requests import Response, Session
 
-from datature.nexus import error, config
+from datature.nexus import config, error
 from datature.nexus.version import __version__
 
 system = platform.system()
 machine = platform.machine()
 python_version = platform.python_version()
-logger = logging.getLogger("nexus")
+
+logger = logging.getLogger("datature-nexus")
 
 # pylint: disable=R0913,C0103,R0914
 
 
 class Requester:
     """An HTTP requester."""
 
@@ -48,15 +49,16 @@
 
         self._session = Session()
 
         # CHeck Secret
         if secret_key is None:
             raise error.UnauthorizedError(
                 "No secret key provided. (Set your secret key"
-                " using client = nexus.Client('secret_key'))")
+                " using client = nexus.Client('secret_key'))"
+            )
         self.secret_key = secret_key
 
     def _request(
         self,
         method,
         path,
         response_type,
@@ -70,107 +72,101 @@
         :param method: The request method
         :param path: The request path
         :param query: The query object
         :param request_body: The request body
         :param request_headers: If have custom request headers
         """
         method = method.upper()
-        assert method in [
-            'GET', 'HEAD', 'DELETE', 'POST', 'PUT', 'PATCH', 'OPTIONS'
-        ]
+        assert method in ["GET", "HEAD", "DELETE", "POST", "PUT", "PATCH", "OPTIONS"]
 
         # Assemble queries and request body.
         post_data = None
         post_files = None
 
         absolute_url = f"{self._base_url}{path}"
 
         if query:
             encoded_params = self._make_query_string(query)
-            absolute_url = f'{absolute_url}?{encoded_params}'
+            absolute_url = f"{absolute_url}?{encoded_params}"
 
         if request_body:
             post_data = json.dumps(request_body)
 
         # Assemble request headers
         headers = self._make_headers(method, request_headers)
 
-        logger.debug("API request: %s %s Body %s", method, absolute_url,
-                     post_data)
+        logger.debug("API request: %s %s Body %s", method, absolute_url, post_data)
 
         # Call request to do a real HTTP call, default timeout 120s
-        response = self._session.request(method,
-                                         absolute_url,
-                                         headers=headers,
-                                         data=post_data,
-                                         files=post_files,
-                                         params=request_params,
-                                         timeout=self._timeout)
+        response = self._session.request(
+            method,
+            absolute_url,
+            headers=headers,
+            data=post_data,
+            files=post_files,
+            params=request_params,
+            timeout=self._timeout,
+        )
 
         self._interpret_response(response)
 
-        logger.debug("API response: %s %s Body %s", method, absolute_url,
-                     response.json())
+        logger.debug(
+            "API response: %s %s Body %s", method, absolute_url, response.json()
+        )
 
         return msgspec.json.decode(
             json.dumps(response.json()),
             type=response_type,
         )
 
     def GET(self, path, response_type, query=None, request_params=None):
-        """ GET Call. """
-        return self._request("GET",
-                             path,
-                             response_type,
-                             query=query,
-                             request_params=request_params)
-
-    def POST(self,
-             path,
-             response_type,
-             query=None,
-             request_body=None,
-             request_params=None):
-        """ POST Call. """
-        return self._request("POST",
-                             path,
-                             response_type,
-                             query=query,
-                             request_body=request_body,
-                             request_params=request_params)
-
-    def PATCH(self,
-              path,
-              response_type,
-              query=None,
-              request_body=None,
-              request_params=None):
-        """ PATCH Call. """
-        return self._request("PATCH",
-                             path,
-                             response_type,
-                             query=query,
-                             request_body=request_body,
-                             request_params=request_params)
+        """GET Call."""
+        return self._request(
+            "GET", path, response_type, query=query, request_params=request_params
+        )
+
+    def POST(
+        self, path, response_type, query=None, request_body=None, request_params=None
+    ):
+        """POST Call."""
+        return self._request(
+            "POST",
+            path,
+            response_type,
+            query=query,
+            request_body=request_body,
+            request_params=request_params,
+        )
+
+    def PATCH(
+        self, path, response_type, query=None, request_body=None, request_params=None
+    ):
+        """PATCH Call."""
+        return self._request(
+            "PATCH",
+            path,
+            response_type,
+            query=query,
+            request_body=request_body,
+            request_params=request_params,
+        )
 
     def DELETE(self, path, response_type):
-        """ DELETE Call. """
+        """DELETE Call."""
         return self._request("DELETE", path, response_type)
 
     def _make_headers(self, method, request_headers):
         """Make request headers
 
         :param method: The request method
         :param request_headers: The custom request headers
         """
         headers = {
-            "Secret-Key":
-            self.secret_key,
-            "User-Agent":
-            f"DatatureSDK/{__version__} "
+            "Secret-Key": self.secret_key,
+            "User-Agent": f"DatatureSDK/{__version__} "
             f"(Python/{python_version}; {system}/{machine})",
         }
 
         if method in ["POST", "PUT", "PATCH", "GET"]:
             headers["Content-Type"] = "application/json"
 
         if request_headers is not None:
@@ -207,16 +203,15 @@
         :param response: The request response
         """
         response_code = response.status_code
         response_data = response.json()
         if not 200 <= response_code < 300:
             error_message = response_data["message"]
 
-            logger.error("API response errored: %s %s", response_code,
-                         error_message)
+            logger.error("API response errored: %s %s", response_code, error_message)
 
             if response_code == 400:
                 raise error.BadRequestError(error_message, response_data)
             if response_code == 403:
                 raise error.ForbiddenError(error_message, response_data)
             if response_code == 404:
                 raise error.NotFoundError(
```

### Comparing `datature-1.6.0/datature/nexus/utils/utils.py` & `datature-1.7.0/datature/nexus/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   utils.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Utils Class module
-'''
+"""
 
-import os
 import glob
+import os
 import tempfile
-from typing import Union
 from pathlib import Path
+from typing import Union
 
 from requests import Session, request
 from requests.adapters import HTTPAdapter, Retry
 
-from datature.nexus import models, config
+from datature.nexus import config, models
 
-SUPPORTED_MRI_EXTENSIONS = ["*.dcm", "*.DCM", '*.nii', '*.NII']
+SUPPORTED_MRI_EXTENSIONS = ["*.dcm", "*.DCM", "*.nii", "*.NII"]
 
 SUPPORTED_IMAGE_VIDEO_EXTENSIONS = [
-    '*.jpg',
-    '*.JPG',
-    '*.png',
-    '*.PNG',
-    '*.jpeg',
-    '*.JPEG',
-    '*.mp4',
-    '*.MP4',
+    "*.jpg",
+    "*.JPG",
+    "*.png",
+    "*.PNG",
+    "*.jpeg",
+    "*.JPEG",
+    "*.mp4",
+    "*.MP4",
 ]
 
-SUPPORTED_FILE_EXTENSIONS = SUPPORTED_MRI_EXTENSIONS + \
-    SUPPORTED_IMAGE_VIDEO_EXTENSIONS
+SUPPORTED_FILE_EXTENSIONS = SUPPORTED_MRI_EXTENSIONS + SUPPORTED_IMAGE_VIDEO_EXTENSIONS
 
-ANNOTATION_FORMAT_EXTENSIONS = [
-    "*.json", "*.csv", "*.xml", "*.labels", "*.txt"
-]
+ANNOTATION_FORMAT_EXTENSIONS = ["*.json", "*.csv", "*.xml", "*.labels", "*.txt"]
 
 
 def find_all_assets(path: str) -> [str]:
     """
     List all assets under folder, include sub folder.
 
     :param path: The folder to upload assets.
     :return: assets path list.
     """
     file_paths = []
 
     # find all assets under folder and sub folders
     for file_ext in SUPPORTED_FILE_EXTENSIONS:
-        file_paths.extend(
-            glob.glob(os.path.join(path, '**', file_ext), recursive=True))
+        file_paths.extend(glob.glob(os.path.join(path, "**", file_ext), recursive=True))
 
     return file_paths
 
 
 def find_all_annotations_files(path: str) -> [str]:
     """
     List all annotations files under folder, include sub folder.
@@ -70,16 +66,15 @@
     :param path: The folder to upload annotations files.
     :return: assets path list.
     """
     file_paths = []
 
     # find all assets under folder and sub folders
     for file_ext in ANNOTATION_FORMAT_EXTENSIONS:
-        file_paths.extend(
-            glob.glob(os.path.join(path, '**', file_ext), recursive=True))
+        file_paths.extend(glob.glob(os.path.join(path, "**", file_ext), recursive=True))
 
     return file_paths
 
 
 def get_exportable_annotations_formats(project_type: str) -> [str]:
     """
     Get the exported annotations formats by project type.
@@ -90,54 +85,59 @@
     if project_type == "Classification":
         return ["csv_classification", "classification_tfrecord"]
 
     if project_type == "Keypoint":
         return ["keypoints_coco"]
 
     return [
-        "coco", "csv_fourcorner", "csv_widthheight", "pascal_voc",
-        "yolo_darknet", "yolo_keras_pytorch", "createml", "tfrecord",
-        "polygon_single", "polygon_coco"
+        "coco",
+        "csv_fourcorner",
+        "csv_widthheight",
+        "pascal_voc",
+        "yolo_darknet",
+        "yolo_keras_pytorch",
+        "createml",
+        "tfrecord",
+        "polygon_single",
+        "polygon_coco",
     ]
 
 
 def init_gcs_upload_session():
     """
-    Initializes an HTTP session for uploading files to 
+    Initializes an HTTP session for uploading files to
         Google Cloud Storage (GCS) with a configured retry policy.
 
-    The retry policy is configured to retry up to 5 times on specific 
-        HTTP status codes (500, 502, 503, 504) that commonly represent 
-        transient server errors. A backoff factor is used to introduce 
+    The retry policy is configured to retry up to 5 times on specific
+        HTTP status codes (500, 502, 503, 504) that commonly represent
+        transient server errors. A backoff factor is used to introduce
         a delay between retry attempts.
 
     Returns:
         Session: A requests Session object configured with the retry policy.
     """
     # Define the retry policy
-    retries = Retry(total=5,
-                    backoff_factor=0.1,
-                    status_forcelist=[500, 502, 503, 504])
+    retries = Retry(total=5, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
 
     http_session = Session()
     # Mount the retry policy for HTTP and HTTPS requests
     http_session.mount("http://", HTTPAdapter(max_retries=retries))
     http_session.mount("https://", HTTPAdapter(max_retries=retries))
 
     return http_session
 
 
 def get_download_path(path: Union[str, Path] = None) -> Path:
     """
-    Gets the download path for storing files. 
+    Gets the download path for storing files.
         If the provided path does not exist, it creates the directory.
 
     Args:
-        path (Union[str, Path], optional): 
-            The path where files should be downloaded or stored. 
+        path (Union[str, Path], optional):
+            The path where files should be downloaded or stored.
             It can be a string or a Path object. If None, the current working directory is used.
 
     Returns:
         Path: The resolved download path as a Path object.
     """
     if path:
         # Check if path is a string and convert it to a Path object if necessary
@@ -153,30 +153,27 @@
 
 
 def download_files_to_tempfile(signed_url: models.DownloadSignedUrl) -> str:
     """
     Downloads a file from a signed URL to a temporary file.
 
     Args:
-        signed_url (models.DownloadSignedUrl): 
+        signed_url (models.DownloadSignedUrl):
             An object containing the signed URL and the HTTP method for the request.
 
     Returns:
         Path: The path to the downloaded temporary file.
 
     Raises:
         requests.RequestException: If there is an issue with making the request.
     """
     method = signed_url.method
     url = signed_url.url
 
-    resp = request(method,
-                   url,
-                   stream=True,
-                   timeout=config.REQUEST_TIME_OUT_SECONDS)
+    resp = request(method, url, stream=True, timeout=config.REQUEST_TIME_OUT_SECONDS)
 
     # Download the file
     with tempfile.NamedTemporaryFile(delete=False) as temp_file:
         for data in resp.iter_content(chunk_size=1024):
             temp_file.write(data)
 
     return temp_file.name
```

### Comparing `datature-1.6.0/datature.egg-info/PKG-INFO` & `datature-1.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python bindings for the Datature API
-Author: Raighne Weng
-Author-email: raighne@datature.io
+Author: Datature
+Author-email: developers@datature.io
 Project-URL: Homepage, https://www.datature.io/
 Project-URL: Documentation, https://developers.datature.io/docs/python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,158 +38,111 @@
 
 [![Python - Version](https://img.shields.io/pypi/pyversions/datature?label=Python)](https://pypi.org/project/datature)
 [![PyPI - Version](https://img.shields.io/pypi/v/datature?label=Pypi%20Package)](https://pypi.org/project/datature)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/datature?label=Pypi%20Downloads)](https://pypi.org/project/datature)
 
 [![Join Datature Slack](https://img.shields.io/badge/Join%20The%20Community-Datature%20Slack-blueviolet?style=plastic)](https://datature.io/community) [![MIT license](https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=plastic)](https://lbesson.apache-license.org/)
 
-<a href="https://datature.io">
-    <img
-      src="assets/datature.svg"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://www.datature.io/blog">
-    <img
-      src="assets/blog.svg"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://developers.datature.io/">
-    <img
-      src="https://cdn.simpleicons.org/readme/#018EF5"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://www.youtube.com/channel/UCd3UQZ9piasi0vgfg5xI59w">
-    <img
-      src="https://cdn.simpleicons.org/youtube/#FF0000"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://www.linkedin.com/company/datature/">
-    <img
-      src="https://cdn.simpleicons.org/linkedin/#0A66C2"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://twitter.com/DatatureAI">
-    <img
-      src="https://cdn.simpleicons.org/twitter/#1D9BF0"
-      width="3%"
-    />
-</a>
-<img src="assets/transparent.png" width="3%"/>
-<a href="https://datature.io/community">
-    <img
-      src="assets/slack.png"
-      width="3%"
-    />
-</a>
+<a href="https://datature.io"><img src="assets/datature.svg" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://www.datature.io/blog"><img src="assets/blog.svg" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://developers.datature.io/"><img src="https://cdn.simpleicons.org/readme/#018EF5" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://www.youtube.com/channel/UCd3UQZ9piasi0vgfg5xI59w"><img src="https://cdn.simpleicons.org/youtube/#FF0000" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://www.linkedin.com/company/datature/"><img src="https://cdn.simpleicons.org/linkedin/#0A66C2" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://twitter.com/DatatureAI"><img src="https://cdn.simpleicons.org/twitter/#1D9BF0" width="3%"/></a><img src="assets/transparent.png" width="3%"/>
+<a href="https://datature.io/community"><img src="assets/slack.png" width="3%"/></a>
 
 ---
 
 :zap: Empower your MLOps pipelines and applications with seamless integrations :zap:
 
-Automate tasks to manage your datasets, run training experiments, export and deploy your models from [Datature Nexus](https://www.datature.io/nexus?utm_source=github) with ease. Perform development via [Python scripts](#python-usage) or with the [CLI](#cli-usage) - your choice!
+Automate tasks to manage your datasets, run training experiments, export and deploy your models from [Datature Nexus](https://www.datature.io/nexus?utm_source=github) with ease. Perform development via [Python Scripts](#python-usage) or with the [Command-Line Interface](#cli-usage).
 
 </div>
 
 ---
 
 <div align="center">
 
-## :rocket: Getting Started :rocket:
+## Getting Started
 
 </div>
 
-## :snake: Prerequisites
+## Prerequisites
 
 - `3.8` <= Python <= `3.12`
 
 We recommend users to create a virtual environment before installing any dependencies. For more information on virtual environments, please refer to:
 
 - [Python venv](https://docs.python.org/3/tutorial/venv.html)
 - [Conda](https://conda.io/projects/conda/en/stable/user-guide/install/index.html)
 - [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/)
 
-## :gear: Installation
+## Installation
 
 ```sh
 pip install --upgrade datature
 ```
 
 ---
 
 ## Python Usage
 
 For a full list of documentation and examples, please refer to the [API docs](https://developers.datature.io/docs/python-sdk).
 
 ### Authentication
 
-To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (signing up is free!). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
+To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (you can create sign up for a free account [here](https://nexus.datature.io/)). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or have been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
 
 ### Examples
 
 To list projects:
 
 ```python
 from datature import nexus
 
-client = nexus.Client("3736971xxxxx")
-
+client = nexus.Client("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117")
 projects = client.list_projects()
 ```
 
 To upload assets:
 
 ```python
 import os
 from datature import nexus
 
 logging.basicConfig()
-
-client = nexus.Client("3736971xxxxx")
-
-project = client.list_projects("proj_xxxxx")
-
+client = nexus.Client("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117")
+project = client.list_projects("proj_fca32b1bb15405d1c2bde19fd90b516d")
 
 upload_session = project.assets.create_upload_session(groups=["dataset"])
-
 with upload_session as session:
   session.add_path("/Users/dataset")
-
 print(len(upload_session))
 ```
 
 ### Logging
 
 You can vary the logging level depending on your task or use case (such as `DEBUG` to provide more insights), but the default `INFO` level is typically best suited for production use.
 
 ```python
 import logging
 
 logging.basicConfig()
-logging.getLogger("nexus").setLevel(logging.DEBUG)
+logging.getLogger("datature-nexus").setLevel(logging.DEBUG)
 ```
 
 ---
 
 ## CLI Usage
 
 For a full list of documentation and examples, please refer to the [CLI docs](https://developers.datature.io/docs/cli).
 
 ### Authentication
 
-To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (signing up is free!). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
+To get started, you will first need to create a project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github) (you can create sign up for a free account [here](https://nexus.datature.io/)). You will then need to locate the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed if you are the Project Owner or have been granted elevated permissions by the Project Owner, and will be used for all subsequent authentication when invoking the various SDK functions.
 
 Once you have the project secret, you will now be able to make API requests using the CLI by entering the command `datature projects auth`:
 
 ```bash
 datature projects auth
 [?] Enter the project secret: ************************************************
 [?] Make [Your Project Name] the default project? (Y/n): y
@@ -201,49 +154,49 @@
 
 ### Project Management
 
 `datature projects`
 
 Show a help page of various functions to add projects, select the default project, and retrieve project information.
 
-#### Auth Project
+#### Authenticate Project
 
 `datature projects auth`
 
-Authenticate new projects using the [project secret key](https://developers.datature.io/v2.0.0/docs/hub-and-api). Multiple projects can be authenticated and stored using different secret keys.
+Authenticate new projects using the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api). Multiple projects can be authenticated and stored using different secret keys.
 
 #### Select Project
 
 `datature projects select`
 
 Select an active project to work on from a list of saved projects. All subsequent CLI commands will be in the context of the selected project until a different project is selected, or the shell session is terminated.
 
 ```bash
 $ datature projects select
 
-> My Cool Project
-  New Test Project
+> Brain Tumor DICOM
+  Hand Gesture Keypoint Detection
 
-Your active project is now: [Dicom]
+Your active project is now: [Brain Tumor DICOM]
 ```
 
 #### List Projects
 
 `datature projects list`
 
 View a table of saved projects with columns containing the names of the projects, the total number of assets, the number of annotated assets, the number of annotations, and the number of tags for each project. The name of the active project is displayed at the bottom of the list.
 
 ```bash
 $ datature projects list
 
-NAME                TOTAL_ASSETS        ANNOTATED_ASSETS    ANNOTATIONS         TAGS
-My Cool Project     4071                433                 1874                3
-New Test Project    718                 53                  959                 4
+NAME                               TOTAL_ASSETS        ANNOTATED_ASSETS    ANNOTATIONS         TAGS
+Brain Tumor DICOM                  4071                433                 1874                3
+Hand Gesture Keypoint Detection    718                 53                  959                 4
 
-Your active project is now: [My Cool Project]
+Your active project is now: [Brain Tumor DICOM]
 ```
 
 ### Asset Management
 
 #### Upload Assets
 
 `datature assets upload`
@@ -268,15 +221,15 @@
 
 List asset group information within your project. You will be prompted to select an existing group or create a new group. If you select an existing group, information about the selected group will be displayed, including the total number of assets in the group, the number of assets that have been annotated, reviewed, or marked for fixes, and the number of assets that have been completed.
 
 ```bash
 $ datature assets groups
 
 > main
-  groupName2
+  validation
 
 NAME            TOTAL           ANNOTATED       REVIEW          TOFIX           COMPLETED
 main            8               1               0               0               0
 ```
 
 ### Annotation Management
 
@@ -323,17 +276,120 @@
 `datature artifacts download`
 
 Download a model artifact from [Datature Nexus](https://www.datature.io/nexus?utm_source=github). You will be prompted to enter a folder path to save the model to, and select the name and [export format](https://developers.datature.io/docs/export-formats) of the artifact to download.
 
 ```bash
 $ datature artifacts download
 [?] Enter the folder path to save model: /Volumes/
-[?] Which artifact do you want to download?: BEAF45-Workflowc
- > BEAF45-Workflowc
+[?] Which artifact do you want to download?: BEAF45-Workflow
+ > BEAF45-Workflow
 
 [?] Which model format do you want to download?: tensorflow
- > tensorflow
-   tflite
-   onnx
+ > TensorFlow
+   TFLite
+   ONNX
 
 Downloading  |████████████████████████████████████████| 100% [443421394/443421394] in 7.1s (62639992.12/s)
 ```
+
+## FAQ
+
+### How do I find my Secret Key and Project Key?
+
+We provide a step-by-step guide to finding these two crucial keys in our [Developer's Documentation](https://developers.datature.io/docs/project-keys-and-secret-keys). You can also explore the other sections under [Python SDK](https://developers.datature.io/docs/python-sdk) to learn more about the full functionality and feature set.
+
+### I'm facing some issues, what now?
+
+We're sorry to hear that, please head over to our [Issues](https://github.com/datature/datature-py/issues) page and post a detailed bug report following our guidelines, and we will address your concerns as soon as we can. Alternatively, ping us in our [Community Slack](https://datature.io/community) where our engineers will attend to your needs.
+
+### I've noticed that some features are missing, how do I contribute?
+
+Datature Python SDK is open-source and we welcome everyone to help to improve it. Please check out our [Contributing Guide](CONTRIBUTING.md) to learn how you can be a part of the team.
+
+### How do I resolve the `command not found: datature` error for the CLI?
+
+The `command not found: datature` error indicates that the Datature SDK/CLI tool is not installed properly in your system's PATH, or it has not been installed at all. To resolve this error, please follow these steps:
+
+#### Ensure Datature CLI is Installed
+
+Before anything else, verify that you've installed the Datature CLI. You can install it using pip with the following command:
+
+```bash
+pip install datature
+```
+
+If you're using a virtual environment (which is recommended), ensure that it's activated before running the installation command.
+
+#### Check Your PATH
+
+After installation, the datature command should be automatically added to your system's PATH. If it's not found, you may need to manually add the directory containing the datature executable to your PATH:
+
+```bash
+which datature
+```
+
+Or
+
+```bash
+pip show datature
+```
+
+As expected, it will show the location of the package like this:
+
+```bash
+Location: /Users/.pyenv/versions/3.8.18/lib/python3.8/site-packages
+```
+
+#### Add the Path to Your Profile
+
+Open your shell profile file with a text editor. This file could be one of ~/.bash_profile, ~/.bashrc, ~/.zshrc, etc., depending on which shell you use and the specific configuration of your operating system.
+
+For example, you can add the path using the following command:
+
+```bash
+echo 'export PATH="$PATH:/path/to/datature"' >> ~/.bash_profile
+```
+
+Replace /path/to/datature with the actual path you found with which datature or pip show datature.
+
+#### Restart Your Terminal
+
+Sometimes, changes to the PATH environment variable do not take effect until you open a new terminal session. After installation or modification of the PATH, close your current terminal and open a new one, then try the command again.
+
+### What does the warning `As the c extension couldn't be imported, google-crc32c is using a pure python implementation that is significantly slower. If possible, please configure a c build environment and compile the extension` mean, and do I need to take any action?
+
+This warning is indicating that the `google-crc32c` library is falling back to a pure Python implementation for calculating CRC32C checksums because it cannot find the C extension which is usually faster. The Python implementation is fully functional but performs slower than its C counterpart. While this won't harm the function of the library, you may experience performance issues if your application requires high-speed checksum computing.
+
+To address this warning for improved performance, you can take the following steps to compile the C extension:
+
+#### Install the Build Essentials
+
+Make sure that you have the necessary build tools installed to compile the C extension.
+
+On Ubuntu/Debian systems, you can install build-essential by running:
+
+```bash
+sudo apt-get install build-essential
+```
+
+On Red Hat/CentOS systems, you can use:
+
+```bash
+sudo yum install gcc gcc-c++ make
+```
+
+On macOS, ensure you have Xcode Command Line Tools installed:
+
+```bash
+xcode-select --install
+```
+
+#### Reinstall google-crc32c with C Extension
+
+With the build environment configured, you can attempt to reinstall the google-crc32c library which should now include the C extension:
+
+```bash
+pip install --no-cache-dir --force-reinstall google-crc32c
+```
+
+By taking these steps, you should be able to eliminate the warning by having the faster C extension compiled and used by google-crc32c.
+If speed is not critical for your use case, you can choose to ignore this warning, and the library will still function correctly, albeit with potentially decreased performance.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: datature Version: 1.6.0 Summary: Python bindings
-for the Datature API Author: Raighne Weng Author-email: raighne@datature.io
+Metadata-Version: 2.1 Name: datature Version: 1.7.0 Summary: Python bindings
+for the Datature API Author: Datature Author-email: developers@datature.io
 Project-URL: Homepage, https://www.datature.io/ Project-URL: Documentation,
 https://developers.datature.io/docs/python-sdk Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: License :: OSI Approved :: Apache Software License
@@ -30,76 +30,80 @@
      _c_d_n_._s_i_m_p_l_e_i_c_o_n_s_._o_r_g_/_y_o_u_t_u_b_e_/_#_F_F_0_0_0_0_][assets/transparent.png]_[_h_t_t_p_s_:_/_/
     _c_d_n_._s_i_m_p_l_e_i_c_o_n_s_._o_r_g_/_l_i_n_k_e_d_i_n_/_#_0_A_6_6_C_2_][assets/transparent.png]_[_h_t_t_p_s_:_/_/
 _c_d_n_._s_i_m_p_l_e_i_c_o_n_s_._o_r_g_/_t_w_i_t_t_e_r_/_#_1_D_9_B_F_0_][assets/transparent.png]_[_a_s_s_e_t_s_/_s_l_a_c_k_._p_n_g_]-
      -- :zap: Empower your MLOps pipelines and applications with seamless
     integrations :zap: Automate tasks to manage your datasets, run training
    experiments, export and deploy your models from [Datature Nexus](https://
  www.datature.io/nexus?utm_source=github) with ease. Perform development via
- [Python scripts](#python-usage) or with the [CLI](#cli-usage) - your choice!
+  [Python Scripts](#python-usage) or with the [Command-Line Interface](#cli-
+                                    usage).
 ---
-                     ## :rocket: Getting Started :rocket:
-## :snake: Prerequisites - `3.8` <= Python <= `3.12` We recommend users to
-create a virtual environment before installing any dependencies. For more
-information on virtual environments, please refer to: - [Python venv](https://
-docs.python.org/3/tutorial/venv.html) - [Conda](https://conda.io/projects/
-conda/en/stable/user-guide/install/index.html) - [virtualenvwrapper](https://
-virtualenvwrapper.readthedocs.io/en/latest/) ## :gear: Installation ```sh pip
-install --upgrade datature ``` --- ## Python Usage For a full list of
-documentation and examples, please refer to the [API docs](https://
-developers.datature.io/docs/python-sdk). ### Authentication To get started, you
-will first need to create a project on [Datature Nexus](https://
-www.datature.io/nexus?utm_source=github) (signing up is free!). You will then
-need to locate the [project secret key](https://developers.datature.io/v1.0.0/
-docs/hub-and-api). This key can only be accessed if you are the Project Owner
-or been granted elevated permissions by the Project Owner, and will be used for
-all subsequent authentication when invoking the various SDK functions. ###
-Examples To list projects: ```python from datature import nexus client =
-nexus.Client("3736971xxxxx") projects = client.list_projects() ``` To upload
-assets: ```python import os from datature import nexus logging.basicConfig()
-client = nexus.Client("3736971xxxxx") project = client.list_projects
-("proj_xxxxx") upload_session = project.assets.create_upload_session(groups=
-["dataset"]) with upload_session as session: session.add_path("/Users/dataset")
-print(len(upload_session)) ``` ### Logging You can vary the logging level
-depending on your task or use case (such as `DEBUG` to provide more insights),
-but the default `INFO` level is typically best suited for production use.
-```python import logging logging.basicConfig() logging.getLogger
-("nexus").setLevel(logging.DEBUG) ``` --- ## CLI Usage For a full list of
-documentation and examples, please refer to the [CLI docs](https://
-developers.datature.io/docs/cli). ### Authentication To get started, you will
-first need to create a project on [Datature Nexus](https://www.datature.io/
-nexus?utm_source=github) (signing up is free!). You will then need to locate
+                              ## Getting Started
+## Prerequisites - `3.8` <= Python <= `3.12` We recommend users to create a
+virtual environment before installing any dependencies. For more information on
+virtual environments, please refer to: - [Python venv](https://docs.python.org/
+3/tutorial/venv.html) - [Conda](https://conda.io/projects/conda/en/stable/user-
+guide/install/index.html) - [virtualenvwrapper](https://
+virtualenvwrapper.readthedocs.io/en/latest/) ## Installation ```sh pip install
+--upgrade datature ``` --- ## Python Usage For a full list of documentation and
+examples, please refer to the [API docs](https://developers.datature.io/docs/
+python-sdk). ### Authentication To get started, you will first need to create a
+project on [Datature Nexus](https://www.datature.io/nexus?utm_source=github)
+(you can create sign up for a free account [here](https://nexus.datature.io/)).
+You will then need to locate the [project secret key](https://
+developers.datature.io/v1.0.0/docs/hub-and-api). This key can only be accessed
+if you are the Project Owner or have been granted elevated permissions by the
+Project Owner, and will be used for all subsequent authentication when invoking
+the various SDK functions. ### Examples To list projects: ```python from
+datature import nexus client = nexus.Client
+("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117") projects =
+client.list_projects() ``` To upload assets: ```python import os from datature
+import nexus logging.basicConfig() client = nexus.Client
+("31a9f0dd997cb632765fc0d222369f6106327c3d20719d31f6ffafe51708f117") project =
+client.list_projects("proj_fca32b1bb15405d1c2bde19fd90b516d") upload_session =
+project.assets.create_upload_session(groups=["dataset"]) with upload_session as
+session: session.add_path("/Users/dataset") print(len(upload_session)) ``` ###
+Logging You can vary the logging level depending on your task or use case (such
+as `DEBUG` to provide more insights), but the default `INFO` level is typically
+best suited for production use. ```python import logging logging.basicConfig()
+logging.getLogger("datature-nexus").setLevel(logging.DEBUG) ``` --- ## CLI
+Usage For a full list of documentation and examples, please refer to the [CLI
+docs](https://developers.datature.io/docs/cli). ### Authentication To get
+started, you will first need to create a project on [Datature Nexus](https://
+www.datature.io/nexus?utm_source=github) (you can create sign up for a free
+account [here](https://nexus.datature.io/)). You will then need to locate the
+[project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-api).
+This key can only be accessed if you are the Project Owner or have been granted
+elevated permissions by the Project Owner, and will be used for all subsequent
+authentication when invoking the various SDK functions. Once you have the
+project secret, you will now be able to make API requests using the CLI by
+entering the command `datature projects auth`: ```bash datature projects auth
+[?] Enter the project secret: ************************************************
+[?] Make [Your Project Name] the default project? (Y/n): y Authentication
+succeeded. ``` You will now be able to run your desired CLI commands as
+outlined above. To see all possible functions as well as view the required
+inputs and expected outputs, check out the following documentation. ### Project
+Management `datature projects` Show a help page of various functions to add
+projects, select the default project, and retrieve project information. ####
+Authenticate Project `datature projects auth` Authenticate new projects using
 the [project secret key](https://developers.datature.io/v1.0.0/docs/hub-and-
-api). This key can only be accessed if you are the Project Owner or been
-granted elevated permissions by the Project Owner, and will be used for all
-subsequent authentication when invoking the various SDK functions. Once you
-have the project secret, you will now be able to make API requests using the
-CLI by entering the command `datature projects auth`: ```bash datature projects
-auth [?] Enter the project secret:
-************************************************ [?] Make [Your Project Name]
-the default project? (Y/n): y Authentication succeeded. ``` You will now be
-able to run your desired CLI commands as outlined above. To see all possible
-functions as well as view the required inputs and expected outputs, check out
-the following documentation. ### Project Management `datature projects` Show a
-help page of various functions to add projects, select the default project, and
-retrieve project information. #### Auth Project `datature projects auth`
-Authenticate new projects using the [project secret key](https://
-developers.datature.io/v2.0.0/docs/hub-and-api). Multiple projects can be
-authenticated and stored using different secret keys. #### Select Project
-`datature projects select` Select an active project to work on from a list of
-saved projects. All subsequent CLI commands will be in the context of the
-selected project until a different project is selected, or the shell session is
-terminated. ```bash $ datature projects select > My Cool Project New Test
-Project Your active project is now: [Dicom] ``` #### List Projects `datature
-projects list` View a table of saved projects with columns containing the names
-of the projects, the total number of assets, the number of annotated assets,
-the number of annotations, and the number of tags for each project. The name of
-the active project is displayed at the bottom of the list. ```bash $ datature
-projects list NAME TOTAL_ASSETS ANNOTATED_ASSETS ANNOTATIONS TAGS My Cool
-Project 4071 433 1874 3 New Test Project 718 53 959 4 Your active project is
-now: [My Cool Project] ``` ### Asset Management #### Upload Assets `datature
+api). Multiple projects can be authenticated and stored using different secret
+keys. #### Select Project `datature projects select` Select an active project
+to work on from a list of saved projects. All subsequent CLI commands will be
+in the context of the selected project until a different project is selected,
+or the shell session is terminated. ```bash $ datature projects select > Brain
+Tumor DICOM Hand Gesture Keypoint Detection Your active project is now: [Brain
+Tumor DICOM] ``` #### List Projects `datature projects list` View a table of
+saved projects with columns containing the names of the projects, the total
+number of assets, the number of annotated assets, the number of annotations,
+and the number of tags for each project. The name of the active project is
+displayed at the bottom of the list. ```bash $ datature projects list NAME
+TOTAL_ASSETS ANNOTATED_ASSETS ANNOTATIONS TAGS Brain Tumor DICOM 4071 433 1874
+3 Hand Gesture Keypoint Detection 718 53 959 4 Your active project is now:
+[Brain Tumor DICOM] ``` ### Asset Management #### Upload Assets `datature
 assets upload` Upload assets to [Datature Nexus](https://www.datature.io/
 nexus?utm_source=github). You will be prompted to enter the path to the folder
 containing the assets that you wish to upload, as well as optional group name
 (s) to categorize the set of assets. This function is designed specially for
 bulk uploading of large datasets, which accelerates the process of onboarding
 data for subsequent annotation and training. This function also supports DICOM
 and NIfTI file upload, which caters to important medical use cases. ```bash $
@@ -112,15 +116,15 @@
 100% [281/281] in 1:17.5 (3.56/s) Server processing completed. ``` #### Group
 Assets `datature assets groups` List asset group information within your
 project. You will be prompted to select an existing group or create a new
 group. If you select an existing group, information about the selected group
 will be displayed, including the total number of assets in the group, the
 number of assets that have been annotated, reviewed, or marked for fixes, and
 the number of assets that have been completed. ```bash $ datature assets groups
-> main groupName2 NAME TOTAL ANNOTATED REVIEW TOFIX COMPLETED main 8 1 0 0 0
+> main validation NAME TOTAL ANNOTATED REVIEW TOFIX COMPLETED main 8 1 0 0 0
 ``` ### Annotation Management #### Upload Annotations `datature annotations
 upload` Upload annotation files to [Datature Nexus](https://www.datature.io/
 nexus?utm_source=github) You will be prompted to enter the path of the
 annotation file you wish to upload and select a [supported annotation format]
 (https://developers.datature.io/docs/uploading-annotations#supported-
 annotation-formats). ```bash $ datature annotations upload [?] Enter the
 annotation files path to be uploaded: /Users/Downloads/Training.csv Processing
@@ -139,12 +143,73 @@
 100% [1/1] in 7.0s (0.14/s) Server processing completed. ``` ### Artifact
 Management #### Artifact Download `datature artifacts download` Download a
 model artifact from [Datature Nexus](https://www.datature.io/
 nexus?utm_source=github). You will be prompted to enter a folder path to save
 the model to, and select the name and [export format](https://
 developers.datature.io/docs/export-formats) of the artifact to download.
 ```bash $ datature artifacts download [?] Enter the folder path to save model:
-/Volumes/ [?] Which artifact do you want to download?: BEAF45-Workflowc >
-BEAF45-Workflowc [?] Which model format do you want to download?: tensorflow >
-tensorflow tflite onnx Downloading
+/Volumes/ [?] Which artifact do you want to download?: BEAF45-Workflow >
+BEAF45-Workflow [?] Which model format do you want to download?: tensorflow >
+TensorFlow TFLite ONNX Downloading
 |ââââââââââââââââââââââââââââââââââââââââ|
-100% [443421394/443421394] in 7.1s (62639992.12/s) ```
+100% [443421394/443421394] in 7.1s (62639992.12/s) ``` ## FAQ ### How do I find
+my Secret Key and Project Key? We provide a step-by-step guide to finding these
+two crucial keys in our [Developer's Documentation](https://
+developers.datature.io/docs/project-keys-and-secret-keys). You can also explore
+the other sections under [Python SDK](https://developers.datature.io/docs/
+python-sdk) to learn more about the full functionality and feature set. ### I'm
+facing some issues, what now? We're sorry to hear that, please head over to our
+[Issues](https://github.com/datature/datature-py/issues) page and post a
+detailed bug report following our guidelines, and we will address your concerns
+as soon as we can. Alternatively, ping us in our [Community Slack](https://
+datature.io/community) where our engineers will attend to your needs. ### I've
+noticed that some features are missing, how do I contribute? Datature Python
+SDK is open-source and we welcome everyone to help to improve it. Please check
+out our [Contributing Guide](CONTRIBUTING.md) to learn how you can be a part of
+the team. ### How do I resolve the `command not found: datature` error for the
+CLI? The `command not found: datature` error indicates that the Datature SDK/
+CLI tool is not installed properly in your system's PATH, or it has not been
+installed at all. To resolve this error, please follow these steps: #### Ensure
+Datature CLI is Installed Before anything else, verify that you've installed
+the Datature CLI. You can install it using pip with the following command:
+```bash pip install datature ``` If you're using a virtual environment (which
+is recommended), ensure that it's activated before running the installation
+command. #### Check Your PATH After installation, the datature command should
+be automatically added to your system's PATH. If it's not found, you may need
+to manually add the directory containing the datature executable to your PATH:
+```bash which datature ``` Or ```bash pip show datature ``` As expected, it
+will show the location of the package like this: ```bash Location: /
+Users/.pyenv/versions/3.8.18/lib/python3.8/site-packages ``` #### Add the Path
+to Your Profile Open your shell profile file with a text editor. This file
+could be one of ~/.bash_profile, ~/.bashrc, ~/.zshrc, etc., depending on which
+shell you use and the specific configuration of your operating system. For
+example, you can add the path using the following command: ```bash echo 'export
+PATH="$PATH:/path/to/datature"' >> ~/.bash_profile ``` Replace /path/to/
+datature with the actual path you found with which datature or pip show
+datature. #### Restart Your Terminal Sometimes, changes to the PATH environment
+variable do not take effect until you open a new terminal session. After
+installation or modification of the PATH, close your current terminal and open
+a new one, then try the command again. ### What does the warning `As the c
+extension couldn't be imported, google-crc32c is using a pure python
+implementation that is significantly slower. If possible, please configure a c
+build environment and compile the extension` mean, and do I need to take any
+action? This warning is indicating that the `google-crc32c` library is falling
+back to a pure Python implementation for calculating CRC32C checksums because
+it cannot find the C extension which is usually faster. The Python
+implementation is fully functional but performs slower than its C counterpart.
+While this won't harm the function of the library, you may experience
+performance issues if your application requires high-speed checksum computing.
+To address this warning for improved performance, you can take the following
+steps to compile the C extension: #### Install the Build Essentials Make sure
+that you have the necessary build tools installed to compile the C extension.
+On Ubuntu/Debian systems, you can install build-essential by running: ```bash
+sudo apt-get install build-essential ``` On Red Hat/CentOS systems, you can
+use: ```bash sudo yum install gcc gcc-c++ make ``` On macOS, ensure you have
+Xcode Command Line Tools installed: ```bash xcode-select --install ``` ####
+Reinstall google-crc32c with C Extension With the build environment configured,
+you can attempt to reinstall the google-crc32c library which should now include
+the C extension: ```bash pip install --no-cache-dir --force-reinstall google-
+crc32c ``` By taking these steps, you should be able to eliminate the warning
+by having the faster C extension compiled and used by google-crc32c. If speed
+is not critical for your use case, you can choose to ignore this warning, and
+the library will still function correctly, albeit with potentially decreased
+performance.
```

### Comparing `datature-1.6.0/datature.egg-info/SOURCES.txt` & `datature-1.7.0/datature.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
-requirements_dev.txt
 setup.py
 datature/__init__.py
 datature.egg-info/PKG-INFO
 datature.egg-info/SOURCES.txt
 datature.egg-info/dependency_links.txt
 datature.egg-info/entry_points.txt
 datature.egg-info/requires.txt
@@ -45,43 +44,55 @@
 datature/nexus/medical/__init__.py
 datature/nexus/medical/base_processor.py
 datature/nexus/medical/dicom_processor.py
 datature/nexus/medical/nii_processor.py
 datature/nexus/utils/__init__.py
 datature/nexus/utils/file_signature.py
 datature/nexus/utils/utils.py
-docs/upload.py
+datature/utils/__init__.py
+datature/utils/experimental/__init__.py
+datature/utils/experimental/convert/__init__.py
+datature/utils/experimental/convert/converter.py
+datature/utils/experimental/convert/logger.py
+datature/utils/experimental/convert/params.py
+datature/utils/experimental/convert/prediction_utils.py
+datature/utils/experimental/convert/predictor.py
+datature/utils/experimental/convert/tensorrt.py
 docs/source/conf.py
 docs/source/functions.rst
 docs/source/index.rst
 docs/source/msgspec.rst
 docs/source/readme.rst
 docs/source/types.rst
-test/__init__.py
-test/test_file_signature.py
-test/test_medical.py
-test/test_requester.py
-test/test_utils.py
-test/api/__init__.py
-test/api/test_annotation.py
-test/api/test_annotation_import_session.py
-test/api/test_artifact.py
-test/api/test_asset.py
-test/api/test_asset_upload_session.py
-test/api/test_client.py
-test/api/test_deploy.py
-test/api/test_ontology.py
-test/api/test_operation.py
-test/api/test_project.py
-test/api/test_run.py
-test/api/test_tag.py
-test/api/test_workflow.py
-test/fixture/__init__.py
-test/fixture/mock.py
-test/fixture/data/__init__.py
-test/fixture/data/artifact_fixture.py
-test/fixture/data/asset_fixture.py
-test/fixture/data/error_fixture.py
-test/fixture/data/frame_fixture.py
-test/fixture/data/operation_fixture.py
-test/fixture/data/projects_fixture.py
-test/fixture/data/upload_session_fixture.py
+tests/__init__.py
+tests/unit/__init__.py
+tests/unit/test_file_signature.py
+tests/unit/test_medical.py
+tests/unit/test_requester.py
+tests/unit/test_utils.py
+tests/unit/api/__init__.py
+tests/unit/api/test_annotation.py
+tests/unit/api/test_annotation_import_session.py
+tests/unit/api/test_artifact.py
+tests/unit/api/test_asset.py
+tests/unit/api/test_asset_upload_session.py
+tests/unit/api/test_client.py
+tests/unit/api/test_deploy.py
+tests/unit/api/test_ontology.py
+tests/unit/api/test_operation.py
+tests/unit/api/test_project.py
+tests/unit/api/test_run.py
+tests/unit/api/test_tag.py
+tests/unit/api/test_workflow.py
+tests/unit/fixture/__init__.py
+tests/unit/fixture/mock.py
+tests/unit/fixture/data/__init__.py
+tests/unit/fixture/data/artifact_fixture.py
+tests/unit/fixture/data/asset_fixture.py
+tests/unit/fixture/data/error_fixture.py
+tests/unit/fixture/data/frame_fixture.py
+tests/unit/fixture/data/operation_fixture.py
+tests/unit/fixture/data/projects_fixture.py
+tests/unit/fixture/data/upload_session_fixture.py
+tests/unit/fixture/data/medical/0002.DCM
+tests/unit/fixture/data/medical/0015.DCM
+tests/unit/fixture/data/medical/MR_Gd.nii
```

### Comparing `datature-1.6.0/docs/source/functions.rst` & `datature-1.7.0/docs/source/functions.rst`

 * *Files identical despite different names*

### Comparing `datature-1.6.0/docs/source/readme.rst` & `datature-1.7.0/docs/source/readme.rst`

 * *Files identical despite different names*

### Comparing `datature-1.6.0/docs/source/types.rst` & `datature-1.7.0/docs/source/types.rst`

 * *Files identical despite different names*

### Comparing `datature-1.6.0/setup.py` & `datature-1.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   setup.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Setup module
-'''
+"""
 
 import re
+
 import setuptools
 
 # read the contents of your README file
 with open("README.md", "r", encoding="utf8") as rd:
     long_description = rd.read()
 
 # read the version number
-with open('datature/nexus/version.py', "r", encoding="utf8") as rd:
-    version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-                        rd.read()).group(1)
+with open("datature/nexus/version.py", "r", encoding="utf8") as rd:
+    version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', rd.read()).group(1)
 
 REQUIRES = []
-with open('requirements.txt', "r", encoding="utf8") as f:
+with open("requirements.txt", "r", encoding="utf8") as f:
     for line in f:
-        line, _, _ = line.partition('#')
+        line, _, _ = line.partition("#")
         line = line.strip()
-        if not line or line.startswith('setuptools'):
+        if not line or line.startswith("setuptools"):
             continue
         REQUIRES.append(line)
 
 setuptools.setup(
     name="datature",
     version=version,
-    author="Raighne Weng",
-    author_email="raighne@datature.io",
+    author="Datature",
+    author_email="developers@datature.io",
     long_description_content_type="text/markdown",
     long_description=long_description,
     project_urls={
         "Homepage": "https://www.datature.io/",
-        "Documentation": "https://developers.datature.io/docs/python-sdk"
+        "Documentation": "https://developers.datature.io/docs/python-sdk",
     },
     description="Python bindings for the Datature API",
     packages=setuptools.find_namespace_packages(),
     python_requires=">=3.8",
     install_requires=REQUIRES,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
-        "License :: OSI Approved :: Apache Software License"
+        "License :: OSI Approved :: Apache Software License",
     ],
     entry_points={
-        'console_scripts': ['datature=datature.nexus.cli.main:main'],
+        "console_scripts": ["datature=datature.nexus.cli.main:main"],
     },
 )
```

### Comparing `datature-1.6.0/test/api/test_annotation.py` & `datature-1.7.0/tests/unit/api/test_annotation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_annotation.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Annotation API Test Cases
-'''
+"""
 
 import json
 import unittest
-from unittest.mock import MagicMock, ANY, patch
-from test.fixture.mock import MockResponse
-from test.fixture.data import operation_fixture
+from unittest.mock import ANY, MagicMock, patch
 
 import msgspec
-
 from datature.nexus import models
-from datature.nexus.client_context import ClientContext
 from datature.nexus.api.annotation.annotation import Annotation
 from datature.nexus.api.annotation.import_session import ImportSession
+from datature.nexus.client_context import ClientContext
+from tests.unit.fixture.data import operation_fixture
+from tests.unit.fixture.mock import MockResponse
 
 # pylint: disable=W0212,W0702
 
 
 class TestAnnotation(unittest.TestCase):
     """Datature Annotation API Resource Test Cases."""
 
@@ -49,64 +48,62 @@
         """Test retrieve a list of annotations."""
         self.annotation.list()
 
         self.annotation._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/annotations",
             ANY,
-            query={
-                "limit": 100,
-                "includeAttributes": False
-            },
+            query={"limit": 100, "includeAttributes": False},
             request_params=None,
         )
 
     def test_create(self):
         """Test create an annotation."""
-        self.annotation.create({
-            "asset_id":
-            "asset_id",
-            "tag":
-            "tagName",
-            "bound_type":
-            "Rectangle",
-            "bound": [[0.425, 0.49382716049382713],
-                      [0.425, 0.6419753086419753], [0.6, 0.6419753086419753],
-                      [0.6, 0.49382716049382713]]
-        })
+        self.annotation.create(
+            {
+                "asset_id": "asset_id",
+                "tag": "tagName",
+                "bound_type": "Rectangle",
+                "bound": [
+                    [0.425, 0.49382716049382713],
+                    [0.425, 0.6419753086419753],
+                    [0.6, 0.6419753086419753],
+                    [0.6, 0.49382716049382713],
+                ],
+            }
+        )
 
         self.annotation._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/annotations",
             ANY,
             request_body={
-                "assetId":
-                "asset_id",
-                "tag":
-                "tagName",
-                "boundType":
-                "Rectangle",
-                "bound": [[0.425, 0.49382716049382713],
-                          [0.425,
-                           0.6419753086419753], [0.6, 0.6419753086419753],
-                          [0.6, 0.49382716049382713]]
+                "assetId": "asset_id",
+                "tag": "tagName",
+                "boundType": "Rectangle",
+                "bound": [
+                    [0.425, 0.49382716049382713],
+                    [0.425, 0.6419753086419753],
+                    [0.6, 0.6419753086419753],
+                    [0.6, 0.49382716049382713],
+                ],
             },
             query=None,
             request_params=None,
         )
 
     def test_get(self):
         """Test retrieve an annotation."""
         self.annotation.get("annotation_id")
 
         self.annotation._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/annotations/annotation_id",
             ANY,
-            query={'includeAttributes': False},
+            query={"includeAttributes": False},
             request_params=None,
         )
 
     def test_delete(self):
         """Test delete an annotation."""
         self.annotation.delete("annotation_id")
 
@@ -117,48 +114,49 @@
         )
 
     def test_export_with_background(self):
         """Test export annotations."""
         self.annotation.create_export(
             {
                 "format": "csv_fourcorner",
-                "options": {
-                    "split_ratio": 0.4,
-                    "seed": 1337,
-                    "normalized": True
-                }
+                "options": {"split_ratio": 0.4, "seed": 1337, "normalized": True},
             },
-            background=True)
+            background=True,
+        )
 
         self.annotation._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/annotationexports",
             ANY,
             query=None,
             request_body={
                 "format": "csv_fourcorner",
                 "options": {
                     "splitRatio": 0.4,
                     "seed": 1337,
                     "normalized": True,
-                }
+                },
             },
-            request_params=None)
+            request_params=None,
+        )
 
     def test_export(self):
         """Test export annotations."""
-        self.annotation.create_export({
-            "format": "csv_fourcorner",
-            "options": {
-                "split_ratio": 0.4,
-                "seed": 1337,
+        self.annotation.create_export(
+            {
+                "format": "csv_fourcorner",
+                "options": {
+                    "split_ratio": 0.4,
+                    "seed": 1337,
+                },
             }
-        })
+        )
         self.annotation._context.requester._request.side_effect = MockResponse(
-            operation_fixture.pending_operation_response, 200)
+            operation_fixture.pending_operation_response, 200
+        )
 
         self.annotation.operation.wait_until_done.assert_called()
 
     @patch("datature.nexus.api.annotation.annotation.utils")
     @patch("datature.nexus.api.annotation.annotation.zipfile")
     def test_download_exported_file(self, patch_utils, patch_zipfile):
         """Test get export annotations."""
@@ -194,30 +192,33 @@
         self.annotation.list_import_sessions()
 
         self.annotation._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/annotationimportsessions",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_get_import_session(self):
         """Test export annotations."""
         self.annotation.get_import_session("import_session_id")
 
         self.annotation._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/annotationimportsessions/import_session_id",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_get_import_session_logs(self):
         """Test export annotations."""
         self.annotation.get_import_session_logs("import_session_id")
 
         self.annotation._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/annotationimportsessions/import_session_id/logs",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
```

### Comparing `datature-1.6.0/test/api/test_annotation_import_session.py` & `datature-1.7.0/tests/unit/api/test_annotation_import_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_annotation_import_session.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session API Test Cases
-'''
+"""
 # pylint: disable=W0703,R0913,W0613,W0212
 
 import json
 import unittest
-from unittest.mock import MagicMock, patch, ANY
-from test.fixture.data import operation_fixture
+from unittest.mock import ANY, MagicMock, patch
 
 import msgspec
-
 from datature.nexus import models
-from datature.nexus.error import Error
-from datature.nexus.client_context import ClientContext
 from datature.nexus.api.annotation.import_session import ImportSession
+from datature.nexus.client_context import ClientContext
+from datature.nexus.error import Error
+from tests.unit.fixture.data import operation_fixture
 
 
 class TestAnnotationImportSession(unittest.TestCase):
     """Datature Annotation Import Session API Resource Test Cases."""
 
     def __init__(self, *args, **kwargs):
         """init global variables."""
@@ -58,211 +57,213 @@
         import_session.get_logs()
 
         import_session._context.requester._request.assert_called_with(
             "GET",
             "/projects/project_id/annotationimportsessions/import_session_id/logs",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_patch_status(self):
         """Test patch_status function."""
         import_session = ImportSession(self.context)
 
         import_session.import_session_id = "import_session_id"
 
-        import_session._patch_status({
-            "condition": "FilesProcessed",
-            "status": "FailedReach",
-        })
+        import_session._patch_status(
+            {
+                "condition": "FilesProcessed",
+                "status": "FailedReach",
+            }
+        )
 
         import_session._context.requester._request.assert_called_with(
             "PATCH",
             "/projects/project_id/annotationimportsessions/import_session_id",
             ANY,
             query=None,
             request_params=None,
             request_body={
                 "status": {
-                    "conditions": [{
-                        "condition": "FilesProcessed",
-                        "status": "FailedReach",
-                    }]
+                    "conditions": [
+                        {
+                            "condition": "FilesProcessed",
+                            "status": "FailedReach",
+                        }
+                    ]
                 }
-            })
+            },
+        )
 
     def test_import_session_length(self):
         """Test len(import_session) function."""
         import_session = ImportSession(self.context)
 
         import_session.filenames = {"file1", "file2"}
 
         assert len(import_session) == 2
 
     @patch("datature.nexus.api.annotation.import_session.open")
     @patch("datature.nexus.api.annotation.import_session.path")
     @patch("datature.nexus.api.annotation.import_session.utils")
-    def test_add_path_to_import_session(self, patched_utils, patched_path,
-                                        patched_open):
-        """ Test import session. """
+    def test_add_path_to_import_session(
+        self, patched_utils, patched_path, patched_open
+    ):
+        """Test import session."""
         import_session = ImportSession(self.context)
 
         patched_open.__enter__.return_value.__len__.return_value = 100
         patched_path.isdir.return_value = True
         patched_path.basename.side_effect = ["file1", "file2"]
-        patched_utils.find_all_annotations_files.return_value = [
-            "file1", "file2"
-        ]
+        patched_utils.find_all_annotations_files.return_value = ["file1", "file2"]
 
         import_session._calculate_file_hash = MagicMock()
         import_session._calculate_file_hash.return_value = 1234
 
         import_session.add_path("assetPath")
 
     @patch("datature.nexus.api.annotation.import_session.open")
     @patch("datature.nexus.api.annotation.import_session.path")
     @patch("datature.nexus.api.annotation.import_session.utils")
-    def test_duplicate_path_to_import_session(self, patched_utils,
-                                              patched_path, patched_open):
-        """ Test import session. """
+    def test_duplicate_path_to_import_session(
+        self, patched_utils, patched_path, patched_open
+    ):
+        """Test import session."""
         import_session = ImportSession(self.context)
 
         patched_open.__enter__.return_value.__len__.return_value = 100
         patched_path.isdir.return_value = True
         patched_path.basename.side_effect = ["file1", "file1"]
-        patched_utils.find_all_annotations_files.return_value = [
-            "file1", "file2"
-        ]
+        patched_utils.find_all_annotations_files.return_value = ["file1", "file2"]
 
         import_session._calculate_file_hash = MagicMock()
         import_session._calculate_file_hash.return_value = 1234
 
         try:
             import_session.add_path("assetPath")
         except Exception as exception:
             assert isinstance(exception, Error)
 
     @patch("datature.nexus.api.annotation.import_session.open")
     @patch("datature.nexus.api.annotation.import_session.path")
     @patch("datature.nexus.api.annotation.import_session.utils")
-    def test_max_file_path_to_import_session(self, patched_utils, patched_path,
-                                             patched_open):
-        """ Test import session. """
+    def test_max_file_path_to_import_session(
+        self, patched_utils, patched_path, patched_open
+    ):
+        """Test import session."""
         import_session = ImportSession(self.context)
         import_session.filenames = {"filename1", "filename2"}
         import_session.max_files_per_session = 1
 
         patched_path.isdir.return_value = True
-        patched_utils.find_all_annotations_files.return_value = [
-            "file1", "file2"
-        ]
+        patched_utils.find_all_annotations_files.return_value = ["file1", "file2"]
 
         try:
             import_session.add_path("assetPath")
         except Exception as exception:
             assert isinstance(exception, Error)
 
     @patch("datature.nexus.api.annotation.import_session.open")
     @patch("datature.nexus.api.annotation.import_session.path")
     @patch("datature.nexus.api.annotation.import_session.utils")
-    def test_background_path_to_import_session(self, patched_utils,
-                                               patched_path, patched_open):
-        """ Test import session. """
+    def test_background_path_to_import_session(
+        self, patched_utils, patched_path, patched_open
+    ):
+        """Test import session."""
         import_session = ImportSession(self.context)
         import_session._upload_current_batch = MagicMock()
 
         patched_open.__enter__.return_value.__len__.return_value = 100
         import_session.max_files_per_batch = 1
         patched_path.isdir.return_value = True
         patched_path.basename.side_effect = ["file1", "file2"]
-        patched_utils.find_all_annotations_files.return_value = [
-            "file1", "file2"
-        ]
+        patched_utils.find_all_annotations_files.return_value = ["file1", "file2"]
 
         import_session._calculate_file_hash = MagicMock()
         import_session._calculate_file_hash.return_value = 1234
 
         import_session.add_path("assetPath")
         import_session._upload_current_batch.assert_called()
 
     def test_add_bytes_max_files_per_session(self):
-        """ Test import session add bytes. """
+        """Test import session add bytes."""
         import_session = ImportSession(self.context)
         import_session._upload_current_batch = MagicMock()
         import_session.filenames = {"filename1"}
 
         import_session._calculate_file_hash = MagicMock()
         import_session._calculate_file_hash.return_value = 1234
 
         import_session.max_files_per_session = 1
         try:
             import_session.add_bytes(b"assetPath", "file1")
         except Exception as exception:
             assert isinstance(exception, Error)
 
     def test_add_bytes_duplicate_file(self):
-        """ Test import session add duplicate file bytes. """
+        """Test import session add duplicate file bytes."""
         import_session = ImportSession(self.context)
         import_session._upload_current_batch = MagicMock()
         import_session.filenames = {"filename1"}
 
         import_session._calculate_file_hash = MagicMock()
         import_session._calculate_file_hash.return_value = 1234
 
         try:
             import_session.add_bytes(b"assetPath", "filename1")
         except Exception as exception:
             assert isinstance(exception, Error)
 
     def test_add_bytes(self):
-        """ Test import session add file bytes. """
+        """Test import session add file bytes."""
         import_session = ImportSession(self.context)
         import_session._upload_current_batch = MagicMock()
 
         import_session._calculate_file_hash = MagicMock()
         import_session._calculate_file_hash.return_value = 1234
 
         import_session.add_bytes(b"assetPath", "filename1")
 
     def test_add_bytes_with_upload_current_batch(self):
-        """ Test import session add file bytes. """
+        """Test import session add file bytes."""
         import_session = ImportSession(self.context)
         import_session._upload_current_batch = MagicMock()
         import_session.max_files_per_batch = 1
         import_session.max_bytes_per_batch = 1
 
         import_session._calculate_file_hash = MagicMock()
         import_session._calculate_file_hash.return_value = 1234
 
         import_session.add_bytes(b"assetPath", "filename1")
         import_session._upload_current_batch.assert_called()
 
     def test_calculate_file_hash(self):
-        """ Test calculate file hash. """
+        """Test calculate file hash."""
         import_session = ImportSession(self.context)
 
         c2c32 = import_session._calculate_file_hash(b"assetPath")
 
         assert c2c32 == "EUvjmg=="
 
     def test_wait_until_done(self):
-        """ Test wait until done. """
+        """Test wait until done."""
         import_session = ImportSession(self.context)
         import_session.import_session_id = "import_session_id"
 
         import_session._context.requester._request.return_value = msgspec.json.decode(
             json.dumps(operation_fixture.annotation_import_finished_response),
             type=models.ImportSession,
         )
 
         import_session.wait_until_done()
 
     @patch("datature.nexus.api.annotation.import_session.config")
     def test_wait_until_done_with_timeout(self, patched_config):
-        """ Test wait until done. """
+        """Test wait until done."""
         import_session = ImportSession(self.context)
         import_session.import_session_id = "import_session_id"
 
         patched_config.OPERATION_LOOPING_DELAY_SECONDS = 0
         patched_config.OPERATION_LOOPING_TIMEOUT_SECONDS = 2
 
         import_session._context.requester._request.return_value = msgspec.json.decode(
@@ -270,15 +271,15 @@
             type=models.ImportSession,
         )
 
         res = import_session.wait_until_done()
         assert res is False
 
     def test_wait_until_done_with_error(self):
-        """ Test wait until done. """
+        """Test wait until done."""
         import_session = ImportSession(self.context)
         import_session.import_session_id = "import_session_id"
 
         import_session._context.requester._request.return_value = msgspec.json.decode(
             json.dumps(operation_fixture.annotation_import_errored_response),
             type=models.ImportSession,
         )
```

### Comparing `datature-1.6.0/test/api/test_artifact.py` & `datature-1.7.0/tests/unit/api/test_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_artifact.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Artifact API Test Cases
-'''
+"""
 
 import json
 import unittest
-from unittest.mock import MagicMock, ANY, patch
-from test.fixture.data import artifact_fixture
+from unittest.mock import ANY, MagicMock, patch
 
 import msgspec
-
 from datature.nexus import models
 from datature.nexus.api.artifact import Artifact
 from datature.nexus.client_context import ClientContext
+from tests.unit.fixture.data import artifact_fixture
 
 # pylint: disable=W0212
 
 
 class TestArtifact(unittest.TestCase):
     """Datature Artifact API Resource Test Cases."""
 
@@ -77,50 +76,53 @@
             request_params=None,
         )
 
     @patch("datature.nexus.api.artifact.config")
     def test_export_model(self, patch_config):
         """Test export a artifact model."""
         patch_config.OPERATION_LOOPING_DELAY_SECONDS = 0
-        self.artifact.create_export("artifact_id", {"format": "TensorFlow"},
-                                    background=True)
+        self.artifact.create_export(
+            "artifact_id", {"format": "TensorFlow"}, background=True
+        )
 
         self.artifact._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/artifacts/artifact_id/exports",
             ANY,
             request_body={"format": "TensorFlow"},
             query=None,
             request_params=None,
         )
 
     @patch("datature.nexus.api.artifact.utils")
     @patch("datature.nexus.api.artifact.zipfile")
     def test_download_exported_model(self, patch_zipfile, patch_utils):
-        """ Test download exported model. """
+        """Test download exported model."""
         patch_utils.download_files_to_tempfile = MagicMock()
 
         patch_zipfile.ZipFile.return_value.__enter__.return_value.namelist.return_value = [
-            "datature-yolov8l.onnx", "datature-yolov8l.pt"
+            "datature-yolov8l.onnx",
+            "datature-yolov8l.pt",
         ]
 
         self.artifact.list = MagicMock()
 
         self.artifact.list.return_value = msgspec.json.decode(
             json.dumps(artifact_fixture.artifacts_includes_exports_response),
-            type=models.Artifacts)
+            type=models.Artifacts,
+        )
 
-        self.artifact.download_exported_model(
-            "model_x4qq70769621y5rrv007447q7y5xw279")
+        self.artifact.download_exported_model("model_x4qq70769621y5rrv007447q7y5xw279")
 
     def test_download_exported_model_not_found(self):
-        """ Test download exported model with wrong model key. """
+        """Test download exported model with wrong model key."""
         self.artifact.list = MagicMock()
 
         self.artifact.list.return_value = msgspec.json.decode(
             json.dumps(artifact_fixture.artifacts_includes_exports_response),
-            type=models.Artifacts)
+            type=models.Artifacts,
+        )
 
         try:
             self.artifact.download_exported_model("artifact_id")
         except:
             pass
```

### Comparing `datature-1.6.0/test/api/test_asset.py` & `datature-1.7.0/tests/unit/api/test_asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_asset.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset API Test Cases
-'''
+"""
 
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
+
 from datature.nexus.api.asset.asset import Asset
-from datature.nexus.client_context import ClientContext
 from datature.nexus.api.asset.upload_session import UploadSession
+from datature.nexus.client_context import ClientContext
 
 # pylint: disable=W0212
 
 
 class TestAsset(unittest.TestCase):
     """Datature Asset API Resource Test Cases."""
 
@@ -41,54 +42,52 @@
         self.asset.list()
 
         self.asset._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/assets",
             ANY,
             query={"limit": 100},
-            request_params=None)
+            request_params=None,
+        )
 
     def test_list_pagination(self):
         """Test retrieve a list of assets with pagination."""
         self.asset.list({"page": "nextPage", "limit": 5})
 
         self.asset._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/assets",
             ANY,
-            query={
-                "page": "nextPage",
-                "limit": 5
-            },
-            request_params=None)
+            query={"page": "nextPage", "limit": 5},
+            request_params=None,
+        )
 
     def test_list_filters(self):
         """Test retrieve a list of assets with filters."""
         self.asset.list(filters={"status": "None"})
 
         self.asset._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/assets",
             ANY,
-            query={
-                'limit': 100,
-                'status': 'None'
-            },
-            request_params=None)
+            query={"limit": 100, "status": "None"},
+            request_params=None,
+        )
 
     def test_get(self):
         """Test get an Asset."""
         self.asset.get("asset_id")
 
         self.asset._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/assets/asset_id",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_update(self):
         """Test update an asset."""
         self.asset.update("asset_id", {"status": "None"})
 
         self.asset._context.requester._request.assert_called_once_with(
             "PATCH",
@@ -113,15 +112,16 @@
         )
 
     def test_delete(self):
         """Test delete an asset."""
         self.asset.delete("asset_id")
 
         self.asset._context.requester._request.assert_called_once_with(
-            "DELETE", "/projects/project_id/assets/asset_id", ANY)
+            "DELETE", "/projects/project_id/assets/asset_id", ANY
+        )
 
     def test_upload_session(self):
         """Test create Asset."""
         upload_session = self.asset.create_upload_session()
 
         assert isinstance(upload_session, UploadSession)
 
@@ -129,9 +129,10 @@
         """Test retrieve assets statistic."""
         self.asset.list_groups()
 
         self.asset._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/assetgroups",
             ANY,
-            query={'group': None},
-            request_params=None)
+            query={"group": None},
+            request_params=None,
+        )
```

### Comparing `datature-1.6.0/test/api/test_asset_upload_session.py` & `datature-1.7.0/tests/unit/api/test_asset_upload_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_asset_upload_session.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Asset Upload Session API Test Cases
-'''
+"""
 # pylint: disable=W0703,R0913,W0613,W0212
 
 import json
 import unittest
 from unittest.mock import MagicMock, patch
-from test.fixture.data import upload_session_fixture
 
 import msgspec
-
 from datature.nexus import models
-from datature.nexus.error import Error
-from test.fixture.data import projects_fixture
-from datature.nexus.client_context import ClientContext
 from datature.nexus.api.asset.upload_session import UploadSession
+from datature.nexus.client_context import ClientContext
+from datature.nexus.error import Error
+from tests.unit.fixture.data import projects_fixture, upload_session_fixture
 
 
 class TestAssetUploadSession(unittest.TestCase):
     """Datature Asset Upload Session API Resource Test Cases."""
 
     def __init__(self, *args, **kwargs):
         """init global variables."""
@@ -52,17 +50,17 @@
 
     @patch("datature.nexus.api.asset.upload_session.config")
     @patch("datature.nexus.api.asset.upload_session.filetype")
     @patch("datature.nexus.api.asset.upload_session.struct")
     @patch("datature.nexus.api.asset.upload_session.google_crc32c")
     @patch("datature.nexus.api.asset.upload_session.path")
     @patch("datature.nexus.api.asset.upload_session.open")
-    def test_add_with_duplicated_file(self, patch_open, patch_path,
-                                      google_crc32c, struct, filetype,
-                                      patch_config):
+    def test_add_with_duplicated_file(
+        self, patch_open, patch_path, google_crc32c, struct, filetype, patch_config
+    ):
         """Test add asset to upload with duplicated file."""
         patch_config.ASSET_UPLOAD_SESSION_BATCH_SIZE = 100
 
         upload_session = UploadSession(self.context)
         upload_session.file_name_map = {"assetName": {"path": "file_path"}}
 
         struct.unpack.return_value = [-384617082]
@@ -81,16 +79,17 @@
 
     @patch("datature.nexus.api.asset.upload_session.config")
     @patch("datature.nexus.api.asset.upload_session.filetype")
     @patch("datature.nexus.api.asset.upload_session.path")
     @patch("datature.nexus.api.asset.upload_session.struct")
     @patch("datature.nexus.api.asset.upload_session.google_crc32c")
     @patch("datature.nexus.api.asset.upload_session.open")
-    def test_add_with_file_not_supported(self, patch_open, google_crc32c,
-                                         struct, path, filetype, patch_config):
+    def test_add_with_file_not_supported(
+        self, patch_open, google_crc32c, struct, path, filetype, patch_config
+    ):
         """Test add asset to upload with file not supported."""
         patch_config.ASSET_UPLOAD_SESSION_BATCH_SIZE = 100
 
         upload_session = UploadSession(self.context)
 
         struct.unpack.return_value = [-384617082]
         path.basename.return_value = "assetName"
@@ -108,16 +107,17 @@
 
     @patch("datature.nexus.api.asset.upload_session.config")
     @patch("datature.nexus.api.asset.upload_session.filetype")
     @patch("datature.nexus.api.asset.upload_session.path")
     @patch("datature.nexus.api.asset.upload_session.struct")
     @patch("datature.nexus.api.asset.upload_session.google_crc32c")
     @patch("datature.nexus.api.asset.upload_session.open")
-    def test_add_with_file(self, patch_open, google_crc32c, struct, path,
-                           filetype, patch_config):
+    def test_add_with_file(
+        self, patch_open, google_crc32c, struct, path, filetype, patch_config
+    ):
         """Test add asset to upload with file."""
         patch_config.ASSET_UPLOAD_SESSION_BATCH_SIZE = 100
         upload_session = UploadSession(self.context)
 
         struct.unpack.return_value = [-384617082]
         path.basename.return_value = "assetName"
         path.getsize.return_value = 5613
@@ -142,64 +142,72 @@
     def test_start(self, patch_open, patch_config):
         """Test start upload with empty assets ."""
         patch_config.ASSET_UPLOAD_SESSION_BATCH_SIZE = 100
 
         upload_session = UploadSession(self.context, ["main"], background=True)
         upload_session._upload_assets = MagicMock()
 
-        upload_session.assets = [{
-            "filename": "test.jpeg",
-            "mime": "image/jpeg",
-            "size": 5613,
-            "crc32c": -384617082
-        }]
+        upload_session.assets = [
+            {
+                "filename": "test.jpeg",
+                "mime": "image/jpeg",
+                "size": 5613,
+                "crc32c": -384617082,
+            }
+        ]
         upload_session.file_name_map = {"test.jpeg": {"path": "file_path"}}
 
         upload_session._context.requester._request.return_value = msgspec.json.decode(
             json.dumps(upload_session_fixture.upload_assets_response),
             type=models.UploadSession,
         )
 
-        upload_session.assets = [{
-            "filename": "test.jpeg",
-            "mime": "image/jpeg",
-            "size": 5613,
-            "crc32c": -384617082
-        }]
+        upload_session.assets = [
+            {
+                "filename": "test.jpeg",
+                "mime": "image/jpeg",
+                "size": 5613,
+                "crc32c": -384617082,
+            }
+        ]
 
         with upload_session as upload_session:
             pass
 
     @patch("datature.nexus.api.asset.upload_session.open")
     def test_start_with_background(self, patch_open):
         """Test start upload with wait server process."""
         upload_session = UploadSession(self.context, ["main"])
 
         upload_session.operation.wait_until_done = MagicMock()
         upload_session._upload_assets = MagicMock()
 
-        upload_session.assets = [{
-            "filename": "test.jpeg",
-            "mime": "image/jpeg",
-            "size": 5613,
-            "crc32c": -384617082
-        }]
+        upload_session.assets = [
+            {
+                "filename": "test.jpeg",
+                "mime": "image/jpeg",
+                "size": 5613,
+                "crc32c": -384617082,
+            }
+        ]
         upload_session.file_name_map = {"test.jpeg": {"path": "file_path"}}
 
         upload_session._context.requester._request.return_value = msgspec.json.decode(
             json.dumps(upload_session_fixture.upload_assets_response),
             type=models.UploadSession,
         )
 
-        upload_session.assets = [{
-            "filename": "test.jpeg",
-            "mime": "image/jpeg",
-            "size": 5613,
-            "crc32c": -384617082
-        }]
+        upload_session.assets = [
+            {
+                "filename": "test.jpeg",
+                "mime": "image/jpeg",
+                "size": 5613,
+                "crc32c": -384617082,
+            }
+        ]
 
         with upload_session as upload_session:
             pass
 
         upload_session.operation.wait_until_done.assert_called()
 
     def test_get_operation_ids(self):
```

### Comparing `datature-1.6.0/test/api/test_client.py` & `datature-1.7.0/tests/unit/api/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_client.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Project API Test Cases
-'''
+"""
 
 import json
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
 
 import msgspec
-
-from datature.nexus import Client
-from datature.nexus import models
+from datature.nexus import Client, models
 from datature.nexus.api.project import Project
-from test.fixture.data import projects_fixture
+from tests.unit.fixture.data import projects_fixture
 
 # pylint: disable=W0212
 
 
 class TestClient(unittest.TestCase):
     """Datature Client Test Cases."""
 
@@ -37,22 +35,23 @@
 
         client = Client("secret_key")
         client._context.requester._request = MagicMock()
 
         self.client = client
 
     def test_info(self):
-        """ Test retrieve workspace info. """
+        """Test retrieve workspace info."""
         self.client.get_info()
 
         self.client._context.requester._request.assert_called_once_with(
-            "GET", "/workspace", ANY, query=None, request_params=None)
+            "GET", "/workspace", ANY, query=None, request_params=None
+        )
 
     def test_list_projects(self):
-        """ Test retrieve workspace projects. """
+        """Test retrieve workspace projects."""
         self.client._context.requester._request.return_value = msgspec.json.decode(
             json.dumps(projects_fixture.list_projects_response),
             type=models.Projects,
         )
 
         self.client.list_projects()
```

### Comparing `datature-1.6.0/test/api/test_deploy.py` & `datature-1.7.0/tests/unit/api/test_deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_deploy.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Deploy API Test Cases
-'''
+"""
 
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
+
 from datature.nexus.api.deployment import Deployment
 from datature.nexus.client_context import ClientContext
 
 # pylint: disable=W0212
 
 
 class TestDeploy(unittest.TestCase):
@@ -40,79 +41,73 @@
         self.deployment.list()
 
         self.deployment._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/deployments",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_get(self):
         """Test get a deployment."""
         self.deployment.get("deploy_id")
 
         self.deployment._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/deployments/deploy_id",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_delete(self):
         """Test delete a deployment."""
         self.deployment.delete("deploy_id")
 
         self.deployment._context.requester._request.assert_called_once_with(
-            "DELETE", "/projects/project_id/deployments/deploy_id", ANY)
+            "DELETE", "/projects/project_id/deployments/deploy_id", ANY
+        )
 
     def test_create(self):
         """Test create a deployment."""
-        self.deployment.create({
-            "name": "name",
-            "model_id": "model_id",
-            "replicas": 1,
-            "resources": {
-                "GPU_T4": 1
-            },
-            "options": {
-                "evaluation_strategy": "evaluation_strategy"
+        self.deployment.create(
+            {
+                "name": "name",
+                "model_id": "model_id",
+                "replicas": 1,
+                "resources": {"GPU_T4": 1},
+                "options": {"evaluation_strategy": "evaluation_strategy"},
             }
-        })
+        )
 
         self.deployment._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/deployments",
             ANY,
             request_body={
                 "name": "name",
                 "modelId": "model_id",
                 "replicas": 1,
-                "resources": {
-                    "GPU_T4": 1
-                },
-                "options": {
-                    "evaluationStrategy": "evaluation_strategy"
-                }
+                "resources": {"GPU_T4": 1},
+                "options": {"evaluationStrategy": "evaluation_strategy"},
             },
             query=None,
             request_params=None,
         )
 
     def test_update(self):
         """Test update a deployment."""
         self.deployment.update("deploy_id", {"name": "name", "replicas": 2})
 
         self.deployment._context.requester._request.assert_called_once_with(
             "PATCH",
             "/projects/project_id/deployments/deploy_id",
             ANY,
-            request_body={
-                "name": "name",
-                "replicas": 2
-            },
+            request_body={"name": "name", "replicas": 2},
             query=None,
             request_params=None,
         )
 
     def test_create_version(self):
         """Test create a deployment version."""
         self.deployment.create_version("deploy_id", "name", "artifact_id")
```

### Comparing `datature-1.6.0/test/api/test_ontology.py` & `datature-1.7.0/tests/unit/api/test_ontology.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_ontology.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Ontology API Test Cases
-'''
+"""
 # pylint: disable=W0212
 
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
 
 from datature.nexus.api.ontology import Ontology
 from datature.nexus.client_context import ClientContext
 
 
 class TestOntology(unittest.TestCase):
     """Datature Ontology API Resource Test Cases."""
@@ -40,8 +40,9 @@
         self.ontology.list_schemas()
 
         self.ontology._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/ontologies",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
```

### Comparing `datature-1.6.0/test/api/test_operation.py` & `datature-1.7.0/tests/unit/api/test_operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_operation.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Operation API Test Cases
-'''
+"""
 
 import json
 import unittest
-from unittest.mock import MagicMock, ANY, patch
-from test.fixture.data import operation_fixture
+from unittest.mock import ANY, MagicMock, patch
 
 import msgspec
-
 from datature.nexus import models
-from datature.nexus.error import Error
 from datature.nexus.api.operation import Operation
 from datature.nexus.client_context import ClientContext
+from datature.nexus.error import Error
+from tests.unit.fixture.data import operation_fixture
 
 # pylint: disable=W0212
 
 
 class TestOperation(unittest.TestCase):
     """Datature Operation API Resource Test Cases."""
 
@@ -47,52 +46,57 @@
         self.operation.get("op_id")
 
         self.operation._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/operations/op_id",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     @patch("datature.nexus.api.operation.config")
     def test_wait_until_done(self, patch_config):
         """Test looping an operation."""
         patch_config.OPERATION_LOOPING_DELAY_SECONDS = 1
 
         self.operation._context.requester._request.side_effect = [
-            msgspec.json.decode(json.dumps(
-                operation_fixture.pending_operation_response),
-                                type=models.Operation),
-            msgspec.json.decode(json.dumps(
-                operation_fixture.finished_operation_response),
-                                type=models.Operation),
+            msgspec.json.decode(
+                json.dumps(operation_fixture.pending_operation_response),
+                type=models.Operation,
+            ),
+            msgspec.json.decode(
+                json.dumps(operation_fixture.finished_operation_response),
+                type=models.Operation,
+            ),
         ]
 
         self.operation.wait_until_done("op_id", raise_exception_if="Errored")
 
     @patch("datature.nexus.api.operation.config")
     def test_wait_until_done_with_status_error(self, patch_config):
         """Test looping an operation with error."""
         patch_config.OPERATION_LOOPING_DELAY_SECONDS = 1
         self.operation._context.requester._request.side_effect = [
-            msgspec.json.decode(json.dumps(
-                operation_fixture.errored_operation_response),
-                                type=models.Operation),
+            msgspec.json.decode(
+                json.dumps(operation_fixture.errored_operation_response),
+                type=models.Operation,
+            ),
         ]
 
         try:
             self.operation.wait_until_done("op_id")
         # pylint: disable=W0703
         except Exception as exception:
             assert isinstance(exception, Error)
 
     @patch("datature.nexus.api.operation.config")
     def test_wait_until_done_with_timeout(self, patch_config):
         """Test looping an operation with timeout."""
         patch_config.OPERATION_LOOPING_DELAY_SECONDS = 1
         self.operation._context.requester._request.return_value = msgspec.json.decode(
             json.dumps(operation_fixture.pending_operation_response),
-            type=models.Operation)
+            type=models.Operation,
+        )
 
         op = self.operation.wait_until_done("op_id", timeout=6)
 
         assert op.status.overview == "Running"
```

### Comparing `datature-1.6.0/test/api/test_project.py` & `datature-1.7.0/tests/unit/api/test_project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_project.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Project API Test Cases
-'''
+"""
 
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
+
 from datature.nexus.api.project import Project
 from datature.nexus.client_context import ClientContext
 
 # pylint: disable=W0212
 
 
 class TestProject(unittest.TestCase):
@@ -36,47 +37,39 @@
         self.project = Project(context)
 
     def test_retrieve(self):
         """Test retrieve a project."""
         self.project.get_info()
 
         self.project._context.requester._request.assert_called_once_with(
-            "GET",
-            "/projects/project_id",
-            ANY,
-            query=None,
-            request_params=None)
+            "GET", "/projects/project_id", ANY, query=None, request_params=None
+        )
 
     def test_modify(self):
         """Test update a project."""
 
         self.project.update({"name": "New Project Name"})
 
         self.project._context.requester._request.assert_called_once_with(
             "PATCH",
             "/projects/project_id",
             ANY,
             request_body={"name": "New Project Name"},
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_insight(self):
         """Test retrieve a project insight."""
         self.project.list_insights()
 
         self.project._context.requester._request.assert_called_once_with(
-            "GET",
-            "/projects/project_id/insights",
-            ANY,
-            query=None,
-            request_params=None)
+            "GET", "/projects/project_id/insights", ANY, query=None, request_params=None
+        )
 
     def test_users(self):
         """Test retrieve project users."""
         self.project.list_users()
 
         self.project._context.requester._request.assert_called_once_with(
-            "GET",
-            "/projects/project_id/users",
-            ANY,
-            query=None,
-            request_params=None)
+            "GET", "/projects/project_id/users", ANY, query=None, request_params=None
+        )
```

### Comparing `datature-1.6.0/test/api/test_run.py` & `datature-1.7.0/tests/unit/api/test_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_run.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Run API Test Cases
-'''
+"""
 
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
+
 from datature.nexus.api.run import Run
 from datature.nexus.client_context import ClientContext
 
 # pylint: disable=W0212
 
 
 class TestRun(unittest.TestCase):
@@ -36,108 +37,97 @@
         self.runs = Run(context)
 
     def test_list(self):
         """Test list training."""
         self.runs.list()
 
         self.runs._context.requester._request.assert_called_once_with(
-            "GET",
-            "/projects/project_id/runs",
-            ANY,
-            query=None,
-            request_params=None)
+            "GET", "/projects/project_id/runs", ANY, query=None, request_params=None
+        )
 
     def test_retrieve(self):
         """Test retrieve a training."""
         self.runs.get("run_id")
 
         self.runs._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/runs/run_id",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_kill(self):
         """Test kill a training."""
         self.runs.kill("run_id")
 
         self.runs._context.requester._request.assert_called_once_with(
             "PATCH",
             "/projects/project_id/runs/run_id",
             ANY,
             request_body={"status": "Cancelled"},
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_start(self):
         """Test start a training."""
         self.runs.start(
-            "flow_id", {
-                "accelerator": {
-                    "name": "GPU_T4",
-                    "count": 1
-                },
+            "flow_id",
+            {
+                "accelerator": {"name": "GPU_T4", "count": 1},
                 "checkpoint": {
                     "strategy": "STRAT_LOWEST_VALIDATION_LOSS",
                     "evaluation_interval": 250,
-                    "metric": "Loss/total_loss"
-                },
-                "limit": {
-                    "metric": "LIM_MINUTE",
-                    "value": 260
+                    "metric": "Loss/total_loss",
                 },
+                "limit": {"metric": "LIM_MINUTE", "value": 260},
                 "preview": True,
-                "matrix": True
-            })
+                "matrix": True,
+            },
+        )
 
         self.runs._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/runs",
             ANY,
             request_body={
                 "flowId": "flow_id",
                 "execution": {
-                    "accelerator": {
-                        "name": "GPU_T4",
-                        "count": 1
-                    },
+                    "accelerator": {"name": "GPU_T4", "count": 1},
                     "checkpoint": {
                         "strategy": "STRAT_LOWEST_VALIDATION_LOSS",
                         "evaluationInterval": 250,
-                        "metric": "Loss/total_loss"
-                    },
-                    "limit": {
-                        "metric": "LIM_MINUTE",
-                        "value": 260
+                        "metric": "Loss/total_loss",
                     },
-                    "debug": False
+                    "limit": {"metric": "LIM_MINUTE", "value": 260},
+                    "debug": False,
                 },
-                "features": {
-                    "preview": True,
-                    "matrix": True
-                }
+                "features": {"preview": True, "matrix": True},
             },
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_log(self):
         """Test retrieve a training log."""
         self.runs.get_logs("runlog_id")
 
         self.runs._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/runs/logs/runlog_id",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_get_confusion_matrix(self):
         """Test retrieve a training log."""
         self.runs.get_confusion_matrix("run_id")
 
         self.runs._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/runs/run_id/confusionMatrix",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
```

### Comparing `datature-1.6.0/test/api/test_tag.py` & `datature-1.7.0/tests/unit/api/test_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_tag.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Project API Test Cases.
-'''
+"""
 
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
+
 from datature.nexus.api.tag import Tag
 from datature.nexus.client_context import ClientContext
 
 # pylint: disable=W0212
 
 
 class TestTag(unittest.TestCase):
@@ -36,85 +37,82 @@
         self.tags = Tag(context)
 
     def test_list(self):
         """Test list tags."""
         self.tags.list()
 
         self.tags._context.requester._request.assert_called_once_with(
-            "GET",
-            "/projects/project_id/tags",
-            ANY,
-            query=None,
-            request_params=None)
+            "GET", "/projects/project_id/tags", ANY, query=None, request_params=None
+        )
 
     def test_create(self):
         """Test create a tag."""
         self.tags.create({"name": "New Tag Name"})
 
         self.tags._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/tags",
             ANY,
             request_body={"name": "New Tag Name"},
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_create_with_metadata(self):
         """Test create a tag with metadata."""
         self.tags.create({"name": "New Tag Name", "color": "#000000"})
 
         self.tags._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/tags",
             ANY,
-            request_body={
-                "name": "New Tag Name",
-                "color": "#000000"
-            },
+            request_body={"name": "New Tag Name", "color": "#000000"},
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_update(self):
         """Test update a tag."""
         self.tags.update(1, {"name": "New Tag Name"})
 
         self.tags._context.requester._request.assert_called_once_with(
             "PATCH",
             "/projects/project_id/tags/1",
             ANY,
             request_body={"name": "New Tag Name"},
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_update_with_metadata(self):
         """Test update a tag with metadata."""
         self.tags.update(1, {"name": "New Tag Name", "color": "#000000"})
 
         self.tags._context.requester._request.assert_called_once_with(
             "PATCH",
             "/projects/project_id/tags/1",
             ANY,
-            request_body={
-                "name": "New Tag Name",
-                "color": "#000000"
-            },
+            request_body={"name": "New Tag Name", "color": "#000000"},
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_delete(self):
         """Test delete a tag."""
         self.tags.delete(1)
 
         self.tags._context.requester._request.assert_called_once_with(
-            "DELETE", "/projects/project_id/tags/1", ANY)
+            "DELETE", "/projects/project_id/tags/1", ANY
+        )
 
     def test_merge(self):
         """Test merge a tag."""
         self.tags.merge(1, 0)
 
         self.tags._context.requester._request.assert_called_once_with(
             "POST",
             "/projects/project_id/tags/1-0:merge",
             ANY,
             query=None,
             request_body=None,
-            request_params=None)
+            request_params=None,
+        )
```

### Comparing `datature-1.6.0/test/api/test_workflow.py` & `datature-1.7.0/tests/unit/api/test_workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_workflow.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Workflow API Test Cases
-'''
+"""
 
 import unittest
-from unittest.mock import MagicMock, ANY
+from unittest.mock import ANY, MagicMock
+
 from datature.nexus.api.workflow import Workflow
 from datature.nexus.client_context import ClientContext
 
 # pylint: disable=W0212
 
 
 class TestWorkflow(unittest.TestCase):
@@ -40,38 +41,42 @@
         self.workflow.list()
 
         self.workflow._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/workflows",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_retrieve(self):
         """Test retrieve a workflow."""
         self.workflow.get("flow_id")
 
         self.workflow._context.requester._request.assert_called_once_with(
             "GET",
             "/projects/project_id/workflows/flow_id",
             ANY,
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_modify(self):
         """Test update a workflow."""
         self.workflow.update("flow_id", {"title": "New Workflow Title"})
 
         self.workflow._context.requester._request.assert_called_once_with(
             "PATCH",
             "/projects/project_id/workflows/flow_id",
             ANY,
             request_body={"title": "New Workflow Title"},
             query=None,
-            request_params=None)
+            request_params=None,
+        )
 
     def test_delete(self):
         """Test delete a workflow."""
         self.workflow.delete("flow_id")
 
         self.workflow._context.requester._request.assert_called_once_with(
-            "DELETE", "/projects/project_id/workflows/flow_id", ANY)
+            "DELETE", "/projects/project_id/workflows/flow_id", ANY
+        )
```

### Comparing `datature-1.6.0/test/fixture/data/asset_fixture.py` & `datature-1.7.0/tests/unit/fixture/data/asset_fixture.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   asset_fixture.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Assets Test Data
-'''
+"""
 
 # pylint: disable=C0301
 list_assets_response = {
-    "next_page":
-    "ZjY0YTdiYTI0NzAzNThlMDljZGNjYzY4Zg",
+    "next_page": "ZjY0YTdiYTI0NzAzNThlMDljZGNjYzY4Zg",
     "data": [
         {
-            "id":
-            "asset_e478b4d2-496b-4abe-a1d2-3cccad605002",
-            "object":
-            "asset",
-            "filename":
-            "boat180.png",
-            "project":
-            "proj_306c543ddd4ff1188a6e4b43a586b62a",
-            "create_date":
-            1688713764134,
+            "id": "asset_e478b4d2-496b-4abe-a1d2-3cccad605002",
+            "object": "asset",
+            "filename": "boat180.png",
+            "project": "proj_306c543ddd4ff1188a6e4b43a586b62a",
+            "create_date": 1688713764134,
             "metadata": {
                 "file_size": 186497,
                 "mime_type": "image/png",
                 "status": "annotated",
                 "height": 243,
                 "width": 400,
                 "groups": ["main"],
-                "custom_metadata": {}
+                "custom_metadata": {},
             },
             "statistic": {
-                "tags_count": [{
-                    "name": "boat",
-                    "count": 1
-                }],
-                "total_annotations": 1
+                "tags_count": [{"name": "boat", "count": 1}],
+                "total_annotations": 1,
             },
-            "url":
-            "https://storage.googleapis.com/assets.datature.io/306c543ddd4ff1188a6e4b43a586b62a/assets/boat180.png?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=gcs-asset-signer%40datature-nexus.iam.gserviceaccount.com%2F20230707%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20230707T071051Z&X-Goog-Expires=86400&X-Goog-SignedHeaders=host&generation=1688713773057960&X-Goog-Signature=81ed17f20a5af973c6c4a95e3ea454751f83abc91c0b95999329f68b85724f51f9df032789a7e29bb4bc09b6acffbbd4fca56b2e1c7ca133dff29c79088bbfcd123117ad31aacf7e146de6f98c90a9958985a1d38e781c4b2afae3a15c011404229d29445634b92f71468b78b50aec20bc8a10781305fac529d0c6b9b444c91536d95b2490acdc19341a2126aac40b1013514ef4b2082075c047bbcae1ffeb74044c6ec093d2dab6c391f4f3a886613c9faeb78e06ce4ccf7b428651623e4afc38a544fc4c8d934a9dbeb4ca61f68c103252e43a2248461613758e3421a4737707177ef16983e97aedd6aa36adfdd963c1b7a1d19c81abcdff0efd9373056c59"
+            "url": "https://storage.googleapis.com/assets.datature.io/306c543ddd4ff1188a6e4b43a586b62a/assets/boat180.png?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=gcs-asset-signer%40datature-nexus.iam.gserviceaccount.com%2F20230707%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20230707T071051Z&X-Goog-Expires=86400&X-Goog-SignedHeaders=host&generation=1688713773057960&X-Goog-Signature=81ed17f20a5af973c6c4a95e3ea454751f83abc91c0b95999329f68b85724f51f9df032789a7e29bb4bc09b6acffbbd4fca56b2e1c7ca133dff29c79088bbfcd123117ad31aacf7e146de6f98c90a9958985a1d38e781c4b2afae3a15c011404229d29445634b92f71468b78b50aec20bc8a10781305fac529d0c6b9b444c91536d95b2490acdc19341a2126aac40b1013514ef4b2082075c047bbcae1ffeb74044c6ec093d2dab6c391f4f3a886613c9faeb78e06ce4ccf7b428651623e4afc38a544fc4c8d934a9dbeb4ca61f68c103252e43a2248461613758e3421a4737707177ef16983e97aedd6aa36adfdd963c1b7a1d19c81abcdff0efd9373056c59",
         },
-    ]
+    ],
 }
 
-annotations_response = [{
-    "id":
-    "annot_1e1a0c12-cf6a-42cb-8347-6596006621b5",
-    "object":
-    "annotation",
-    "bound_type":
-    "rectangle",
-    "bound": [[0.425, 0.49382716049382713], [0.425, 0.6419753086419753],
-              [0.6, 0.6419753086419753], [0.6, 0.49382716049382713]],
-    "project_id":
-    "proj_306c543ddd4ff1188a6e4b43a586b62a",
-    "asset_id":
-    "asset_e478b4d2-496b-4abe-a1d2-3cccad605002",
-    "tag":
-    "boat"
-}]
+annotations_response = [
+    {
+        "id": "annot_1e1a0c12-cf6a-42cb-8347-6596006621b5",
+        "object": "annotation",
+        "bound_type": "rectangle",
+        "bound": [
+            [0.425, 0.49382716049382713],
+            [0.425, 0.6419753086419753],
+            [0.6, 0.6419753086419753],
+            [0.6, 0.49382716049382713],
+        ],
+        "project_id": "proj_306c543ddd4ff1188a6e4b43a586b62a",
+        "asset_id": "asset_e478b4d2-496b-4abe-a1d2-3cccad605002",
+        "tag": "boat",
+    }
+]
```

### Comparing `datature-1.6.0/test/fixture/data/error_fixture.py` & `datature-1.7.0/tests/unit/fixture/data/error_fixture.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   error_fixture.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Error Response Test Data
-'''
+"""
 
 forbidden_error_response = {
     "code": "ForbiddenError",
-    "message": "No Access Rights to Requested Resources"
+    "message": "No Access Rights to Requested Resources",
 }
 
 not_found_error_response = {
     "code": "ResourceNotFoundError",
-    "message": "Requested Project Resource Not Found"
+    "message": "Requested Project Resource Not Found",
 }
 
 too_many_requests_error_response = {
     "code": "TooManyRequestsError",
-    "message": "Too Many Requests"
+    "message": "Too Many Requests",
 }
 
 internal_server_error_response = {
     "code": "InternalServerError",
-    "message": "Internal Server Error"
+    "message": "Internal Server Error",
 }
```

### Comparing `datature-1.6.0/test/fixture/data/frame_fixture.py` & `datature-1.7.0/tests/unit/fixture/data/frame_fixture.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   frame_fixture.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Upload Session Test Data
-'''
+"""
 
 # pylint: disable=C0301
 register_frame_response = {
     "frame_format": "rectangle",
     "frame_id": "2fa565d3-27e2-4ee6-8362-bb4a3d8e7c12",
     "image_format": "pillow",
     "num_classes": 5,
```

### Comparing `datature-1.6.0/test/fixture/data/operation_fixture.py` & `datature-1.7.0/tests/unit/fixture/data/operation_fixture.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,185 +1,161 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   operation_fixture.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Operation Test Data
-'''
+"""
 
 pending_operation_response = {
-    'id': 'op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a',
-    'object': 'operation',
-    'kind': 'nexus.annotations.export',
-    'status': {
-        'overview': 'Running',
-        'message': 'Operation running',
-        'progress': {
-            'unit': 'asset',
-            'withStatus': {
-                'Queued': 10,
-                'Running': 0,
-                'Finished': 436,
-                'Errored': 0,
-                'Cancelled': 0
-            }
-        }
+    "id": "op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a",
+    "object": "operation",
+    "kind": "nexus.annotations.export",
+    "status": {
+        "overview": "Running",
+        "message": "Operation running",
+        "progress": {
+            "unit": "asset",
+            "withStatus": {
+                "Queued": 10,
+                "Running": 0,
+                "Finished": 436,
+                "Errored": 0,
+                "Cancelled": 0,
+            },
+        },
     },
-    'createDate': 1701755214003,
-    'updateDate': 1701755215476
+    "createDate": 1701755214003,
+    "updateDate": 1701755215476,
 }
 
 finished_operation_response = {
-    'id': 'op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a',
-    'object': 'operation',
-    'kind': 'nexus.annotations.export',
-    'status': {
-        'overview': 'Finished',
-        'message': 'Operation running',
-        'payload': '',
-        'progress': {
-            'unit': 'asset',
-            'withStatus': {
-                'Queued': 0,
-                'Running': 0,
-                'Finished': 436,
-                'Errored': 0,
-                'Cancelled': 0
-            }
-        }
+    "id": "op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a",
+    "object": "operation",
+    "kind": "nexus.annotations.export",
+    "status": {
+        "overview": "Finished",
+        "message": "Operation running",
+        "payload": "",
+        "progress": {
+            "unit": "asset",
+            "withStatus": {
+                "Queued": 0,
+                "Running": 0,
+                "Finished": 436,
+                "Errored": 0,
+                "Cancelled": 0,
+            },
+        },
     },
-    'createDate': 1701755214003,
-    'updateDate': 1701755215476
+    "createDate": 1701755214003,
+    "updateDate": 1701755215476,
 }
 
+
 errored_operation_response = {
-    'id': 'op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a',
-    'object': 'operation',
-    'kind': 'nexus.annotations.export',
-    'status': {
-        'overview': 'Errored',
-        'message': 'Operation running',
-        'payload': '',
-        'progress': {
-            'unit': 'asset',
-            'withStatus': {
-                'Queued': 0,
-                'Running': 0,
-                'Finished': 436,
-                'Errored': 0,
-                'Cancelled': 0
-            }
-        }
+    "id": "op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a",
+    "object": "operation",
+    "kind": "nexus.annotations.export",
+    "status": {
+        "overview": "Errored",
+        "message": "Operation running",
+        "payload": "",
+        "progress": {
+            "unit": "asset",
+            "withStatus": {
+                "Queued": 0,
+                "Running": 0,
+                "Finished": 436,
+                "Errored": 0,
+                "Cancelled": 0,
+            },
+        },
     },
-    'createDate': 1701755214003,
-    'updateDate': 1701755215476
+    "createDate": 1701755214003,
+    "updateDate": 1701755215476,
 }
 
+
 annotation_operation_response = {
     "opId": "op_8e794c4d-47b4-460c-bcd1-173ab5d109d7",
     "status": "Finished",
     "download": {
         "method": "GET",
         "url": "https://nexus.datature.io/projects",
-        "expiryDate": 1706183829833
-    }
+        "expiryDate": 1706183829833,
+    },
 }
 
 annotation_export_error_response = {
     "opId": "op_8e794c4d-47b4-460c-bcd1-173ab5d109d7",
-    "status": "Errored"
+    "status": "Errored",
 }
 
 annotation_import_finished_response = {
     "id": "annotsess_de40cabf-8275-4844-9d29-1ae3f7af5ca8",
     "object": "annotation_import_session",
     "projectId": "proj_cd067221d5a6e4007ccbb4afb5966535",
     "status": {
         "overview": "Finished",
         "message": "Annotation Imported successfully.",
         "updateDate": 1705465365932,
         "files": {
             "totalSizeBytes": 63368,
             "pageCount": 1,
-            "withStatus": {
-                "Processing": 0,
-                "Processed": 1,
-                "FailedProcess": 0
-            }
+            "withStatus": {"Processing": 0, "Processed": 1, "FailedProcess": 0},
         },
-        "annotations": {
-            "withStatus": {
-                "Processed": 1549,
-                "Committed": 1549
-            }
-        }
+        "annotations": {"withStatus": {"Processed": 1549, "Committed": 1549}},
     },
     "expiryDate": 1705468620676,
     "createDate": 1705465320781,
-    "updateDate": 1705465365945
+    "updateDate": 1705465365945,
 }
 
 annotation_import_errored_response = {
     "id": "annotsess_a2c771e8-6b85-47a2-b844-d25ee18e6ae3",
     "object": "annotation_import_session",
     "projectId": "proj_cd067221d5a6e4007ccbb4afb5966535",
     "status": {
         "overview": "Errored",
         "message": "AnnotationsCommitted errored, please contract support.",
         "updateDate": 1701772558131,
         "files": {
             "totalSizeBytes": 0,
             "pageCount": 1,
-            "withStatus": {
-                "Processing": 0,
-                "Processed": 0,
-                "FailedProcess": 0
-            }
+            "withStatus": {"Processing": 0, "Processed": 0, "FailedProcess": 0},
         },
-        "annotations": {
-            "withStatus": {
-                "Processed": 0,
-                "Committed": 0
-            }
-        }
+        "annotations": {"withStatus": {"Processed": 0, "Committed": 0}},
     },
     "expiryDate": 1701768467656,
     "createDate": 1701765173451,
-    "updateDate": 1701772558150
+    "updateDate": 1701772558150,
 }
 
+
 annotation_import_running_response = {
     "id": "annotsess_a2c771e8-6b85-47a2-b844-d25ee18e6ae3",
     "object": "annotation_import_session",
     "projectId": "proj_cd067221d5a6e4007ccbb4afb5966535",
     "status": {
         "overview": "Running",
         "message": "Running.",
         "updateDate": 1701772558131,
         "files": {
             "totalSizeBytes": 0,
             "pageCount": 1,
-            "withStatus": {
-                "Processing": 0,
-                "Processed": 0,
-                "FailedProcess": 0
-            }
+            "withStatus": {"Processing": 0, "Processed": 0, "FailedProcess": 0},
         },
-        "annotations": {
-            "withStatus": {
-                "Processed": 0,
-                "Committed": 0
-            }
-        }
+        "annotations": {"withStatus": {"Processed": 0, "Committed": 0}},
     },
     "expiryDate": 1701768467656,
     "createDate": 1701765173451,
-    "updateDate": 1701772558150
+    "updateDate": 1701772558150,
 }
```

### Comparing `datature-1.6.0/test/fixture/data/projects_fixture.py` & `datature-1.7.0/tests/unit/fixture/data/projects_fixture.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   projects_fixture.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Assets Test Data
-'''
+"""
 
 # pylint: disable=C0301
-list_projects_response = [{
-    "id":
-    "proj_b705a30ae26671657f1fd51eb2d4739d",
-    "object":
-    "project",
-    "name":
-    "New Test Nam",
-    "workspaceId":
-    "ws_1c8aab980f174b0296c7e35e88665b13",
-    "type":
-    "ObjectDetection",
-    "createDate":
-    1669185404836,
-    "localization":
-    "MULTI",
-    "tags": ["boat"],
-    "groups": ["main", "t", "group1", "gourp2", "1", "dataset"],
-    "statistic": {
-        "tagsCount": [{
-            "name": "boat",
-            "count": 240
-        }],
-        "totalAssets": 10272,
-        "annotatedAssets": 142,
-        "totalAnnotations": 240
+list_projects_response = [
+    {
+        "id": "proj_b705a30ae26671657f1fd51eb2d4739d",
+        "object": "project",
+        "name": "New Test Nam",
+        "workspaceId": "ws_1c8aab980f174b0296c7e35e88665b13",
+        "type": "ObjectDetection",
+        "createDate": 1669185404836,
+        "localization": "MULTI",
+        "tags": ["boat"],
+        "groups": ["main", "t", "group1", "gourp2", "1", "dataset"],
+        "statistic": {
+            "tagsCount": [{"name": "boat", "count": 240}],
+            "totalAssets": 10272,
+            "annotatedAssets": 142,
+            "totalAnnotations": 240,
+        },
     }
-}]
+]
 
 workspace_info_response = {
     "id": "ws_1c8aab980f174b0296c7e35e88665b13",
     "object": "workspace",
     "name": "Raighne's Workspace",
     "owner": "user_6323fea23e292439f31c58cd",
     "tier": "Developer",
-    "createDate": 1694771445182
+    "createDate": 1694771445182,
 }
```

### Comparing `datature-1.6.0/test/fixture/mock.py` & `datature-1.7.0/tests/unit/fixture/mock.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   mock.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Test Mock Cases
-'''
+"""
 
 
 class MockResponse:
     """Datature Mock Request Response."""
 
     def __init__(self, json_data, status_code):
         self.json_data = json_data
```

### Comparing `datature-1.6.0/test/test_file_signature.py` & `datature-1.7.0/tests/unit/test_file_signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_file_signature.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Utils Test Cases
-'''
+"""
 # pylint: disable=W0703,W0012,W0212
 
 import unittest
 
 from datature.nexus.utils import file_signature
 
 
 class TestFileSignature(unittest.TestCase):
     """Datature File Signature Test Cases."""
 
     def test_jpeg_file(self):
         """Test jpg files."""
 
         file_mine = file_signature.get_file_mime_by_signature(
-            b'\xff\xd8\xff\xe0\x00\x10JFIF\x00\x01\x01\x01\x01,\x01,\x00\x00\xff\xe2\x0cXICC_PROFILE\x00\x01\x01\x00\x00\x0cHLino\x02\x10\x00\x00mntrRGB XYZ \x07\xce\x00\x02\x00\t\x00\x06\x001\x00\x00acspMSFT\x00\x00\x00\x00IEC sRGB\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\xf6\xd6\x00\x01\x00\x00\x00\x00\xd3-HP  \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x11cprt\x00\x00\x01P\x00\x00\x003desc\x00\x00\x01\x84\x00\x00\x00lwtpt\x00\x00\x01\xf0\x00\x00\x00\x14bkpt\x00\x00\x02\x04\x00\x00\x00\x14rXYZ\x00\x00\x02\x18\x00\x00\x00\x14gXYZ\x00\x00\x02,\x00\x00\x00\x14bXYZ\x00\x00\x02@\x00\x00\x00\x14dmnd\x00\x00\x02T\x00\x00\x00pdmdd\x00\x00\x02\xc4\x00\x00\x00\x88vued\x00\x00\x03L\x00\x00\x00\x86view\x00\x00\x03\xd4\x00\x00\x00$lumi\x00\x00\x03\xf8\x00\x00\x00\x14meas\x00\x00\x04\x0c\x00\x00\x00$tech\x00\x00\x040\x00\x00\x00\x0crTRC\x00\x00\x04<\x00\x00\x08\x0cgTRC\x00\x00\x04<\x00\x00\x08\x0cbTRC\x00\x00\x04<\x00\x00\x08\x0ctext\x00\x00\x00\x00Copyright (c) 1998'
+            b"\xff\xd8\xff\xe0\x00\x10JFIF\x00\x01\x01\x01\x01,\x01,\x00\x00\xff\xe2\x0cXICC_PROFILE\x00\x01\x01\x00\x00\x0cHLino\x02\x10\x00\x00mntrRGB XYZ \x07\xce\x00\x02\x00\t\x00\x06\x001\x00\x00acspMSFT\x00\x00\x00\x00IEC sRGB\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\xf6\xd6\x00\x01\x00\x00\x00\x00\xd3-HP  \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x11cprt\x00\x00\x01P\x00\x00\x003desc\x00\x00\x01\x84\x00\x00\x00lwtpt\x00\x00\x01\xf0\x00\x00\x00\x14bkpt\x00\x00\x02\x04\x00\x00\x00\x14rXYZ\x00\x00\x02\x18\x00\x00\x00\x14gXYZ\x00\x00\x02,\x00\x00\x00\x14bXYZ\x00\x00\x02@\x00\x00\x00\x14dmnd\x00\x00\x02T\x00\x00\x00pdmdd\x00\x00\x02\xc4\x00\x00\x00\x88vued\x00\x00\x03L\x00\x00\x00\x86view\x00\x00\x03\xd4\x00\x00\x00$lumi\x00\x00\x03\xf8\x00\x00\x00\x14meas\x00\x00\x04\x0c\x00\x00\x00$tech\x00\x00\x040\x00\x00\x00\x0crTRC\x00\x00\x04<\x00\x00\x08\x0cgTRC\x00\x00\x04<\x00\x00\x08\x0cbTRC\x00\x00\x04<\x00\x00\x08\x0ctext\x00\x00\x00\x00Copyright (c) 1998"
         )
 
         assert file_mine == "image/jpeg"
 
     def test_not_supported_file(self):
         """Test not supported files."""
```

### Comparing `datature-1.6.0/test/test_medical.py` & `datature-1.7.0/tests/unit/test_medical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_medical.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Medical Test Cases
-'''
+"""
 # pylint: disable=W0703,W0012,W0212
 
 import os
 import unittest
 from pathlib import Path
 
 from datature.nexus.error import BadRequestError
@@ -48,29 +48,31 @@
             get_processor("../fixture/data/artifact_fixture.py")
         except Exception as e:
             assert isinstance(e, NotImplementedError)
 
     def test_dcm_file_output(self):
         """Test DCM files."""
         path = os.path.join(
-            Path(__file__).parent.resolve(), "fixture/data/medical/0002.DCM")
+            Path(__file__).parent.resolve(), "fixture/data/medical/0002.DCM"
+        )
 
         processor = get_processor(path)
 
         process_data = {"file": path}
 
         processor.valid(process_data)
         resp = processor.process(process_data)
 
         assert len(resp) == 1
 
     def test_single_file_dcm_file_output(self):
         """Test DCM files."""
         path = os.path.join(
-            Path(__file__).parent.resolve(), "fixture/data/medical/0015.DCM")
+            Path(__file__).parent.resolve(), "fixture/data/medical/0015.DCM"
+        )
 
         processor = get_processor(path)
 
         process_data = {"file": path}
 
         processor.valid(process_data)
         resp = processor.process(process_data)
@@ -91,29 +93,31 @@
             processor.valid({})
         except Exception as e:
             assert isinstance(e, BadRequestError)
 
     def test_nii_file_output(self):
         """Test NIfTI files."""
         path = os.path.join(
-            Path(__file__).parent.resolve(), "fixture/data/medical/MR_Gd.nii")
+            Path(__file__).parent.resolve(), "fixture/data/medical/MR_Gd.nii"
+        )
 
         processor = get_processor(path)
 
         process_data = {"file": path}
 
         processor.valid(process_data)
         resp = processor.process(process_data)
 
         assert len(resp) == 3
 
     def test_nii_file_output_with_orientation(self):
         """Test NIfTI files."""
         path = os.path.join(
-            Path(__file__).parent.resolve(), "fixture/data/medical/MR_Gd.nii")
+            Path(__file__).parent.resolve(), "fixture/data/medical/MR_Gd.nii"
+        )
 
         processor = get_processor(path)
 
         process_data = {"file": path, "options": {"nifti_orientation": "x"}}
 
         processor.valid(process_data)
         resp = processor.process(process_data)
```

### Comparing `datature-1.6.0/test/test_requester.py` & `datature-1.7.0/tests/unit/test_requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,175 +1,183 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_requester.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature HTTP Resource Test Cases
-'''
+"""
 
 import unittest
 from unittest.mock import MagicMock
-from test.fixture.mock import MockResponse
-from test.fixture.data import error_fixture, operation_fixture
+
 from datature.nexus import models
+from datature.nexus.error import (
+    BadRequestError,
+    ForbiddenError,
+    InternalServerError,
+    NotFoundError,
+    TooManyRequestsError,
+    UnauthorizedError,
+)
 from datature.nexus.requester import Requester
-from datature.nexus.error import (ForbiddenError, NotFoundError,
-                                  TooManyRequestsError, InternalServerError,
-                                  UnauthorizedError, BadRequestError)
+from tests.unit.fixture.data import error_fixture, operation_fixture
+from tests.unit.fixture.mock import MockResponse
 
 # pylint: disable=W0703,W0012,W0212
 
 
 class TestRequester(unittest.TestCase):
     """Datature HTTP Resource Test Cases."""
 
     def test_request_with_no_project_key(self):
         """Test resource request."""
 
         try:
-            Requester(secret_key=None,
-                      endpoint="")._request("GET",
-                                            "test_end_point",
-                                            response_type=models.Artifacts,
-                                            request_body={"test": "test"})
+            Requester(secret_key=None, endpoint="")._request(
+                "GET",
+                "test_end_point",
+                response_type=models.Artifacts,
+                request_body={"test": "test"},
+            )
 
         except Exception as exception:
             assert isinstance(exception, UnauthorizedError)
 
     def test_request_with_request_body(self):
         """Test resource request."""
         requester = Requester("secret-key", endpoint="")
         requester._session.request = MagicMock()
 
         requester._session.request.side_effect = [
             MockResponse(operation_fixture.pending_operation_response, 200)
         ]
         requester._interpret_response = MagicMock()
 
-        requester._request("POST",
-                           "test_end_point",
-                           response_type=models.Operation,
-                           request_body={"test": "test"})
+        requester._request(
+            "POST",
+            "test_end_point",
+            response_type=models.Operation,
+            request_body={"test": "test"},
+        )
 
     def test_request_with_query(self):
         """Test resource request."""
         requester = Requester("secret-key", endpoint="")
 
         requester._session.request = MagicMock()
         requester._session.request.side_effect = [
             MockResponse(operation_fixture.pending_operation_response, 200)
         ]
 
-        response = requester.GET("test_end_poimt",
-                                 query={"limit": 5},
-                                 response_type=models.Operation)
+        response = requester.GET(
+            "test_end_poimt", query={"limit": 5}, response_type=models.Operation
+        )
 
-        assert response.id == 'op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a'
+        assert response.id == "op_c26ea31d-599c-4a03-8b0d-b2bc9995fa8a"
 
     def test_make_headers_with_get_method(self):
         """Test make headers."""
 
-        headers = Requester("project_secret",
-                            endpoint="")._make_headers("GET", {})
+        headers = Requester("project_secret", endpoint="")._make_headers("GET", {})
 
         assert headers["Secret-Key"] == "project_secret"
 
     def test_make_headers_with_post_method(self):
         """Test make headers with post method."""
 
-        headers = Requester("project_secret",
-                            endpoint="")._make_headers("POST", {})
+        headers = Requester("project_secret", endpoint="")._make_headers("POST", {})
 
         assert headers["Secret-Key"] == "project_secret"
         assert headers["Content-Type"] == "application/json"
 
     def test_make_headers_with_supplied_headers(self):
         """Test make headers with supplied headers."""
 
-        headers = Requester("project_secret",
-                            endpoint="")._make_headers("GET", {
-                                "Connection": "keep-alive",
-                                "Accept": "*/*"
-                            })
+        headers = Requester("project_secret", endpoint="")._make_headers(
+            "GET", {"Connection": "keep-alive", "Accept": "*/*"}
+        )
 
         assert headers["Secret-Key"] == "project_secret"
         assert headers["Accept"] == "*/*"
 
     def test_interpret_response_with_400(self):
         """Test interpret response with 400 code."""
 
         try:
             Requester("secret-key", endpoint="")._interpret_response(
-                MockResponse(error_fixture.forbidden_error_response, 400))
+                MockResponse(error_fixture.forbidden_error_response, 400)
+            )
 
         except Exception as exception:
             assert isinstance(exception, BadRequestError)
 
     def test_interpret_response_with_403(self):
         """Test interpret response with 403 code."""
 
         try:
             Requester("secret-key", endpoint="")._interpret_response(
-                MockResponse(error_fixture.forbidden_error_response, 403))
+                MockResponse(error_fixture.forbidden_error_response, 403)
+            )
 
         except Exception as exception:
             assert isinstance(exception, ForbiddenError)
 
     def test_interpret_response_with_404(self):
         """Test interpret response with 404 code."""
 
         try:
             Requester("secret-key", endpoint="")._interpret_response(
-                MockResponse(error_fixture.not_found_error_response, 404))
+                MockResponse(error_fixture.not_found_error_response, 404)
+            )
 
         except Exception as exception:
             assert isinstance(exception, NotFoundError)
 
     def test_interpret_response_with_429(self):
         """Test interpret response with 429 code."""
 
         try:
             Requester("secret-key", endpoint="")._interpret_response(
-                MockResponse(error_fixture.too_many_requests_error_response,
-                             429))
+                MockResponse(error_fixture.too_many_requests_error_response, 429)
+            )
 
         except Exception as exception:
             assert isinstance(exception, TooManyRequestsError)
 
     def test_interpret_response_with_500(self):
         """Test interpret response with 500 code."""
 
         try:
             Requester("secret-key", endpoint="")._interpret_response(
-                MockResponse(error_fixture.internal_server_error_response,
-                             500))
+                MockResponse(error_fixture.internal_server_error_response, 500)
+            )
 
         except Exception as exception:
             assert isinstance(exception, InternalServerError)
 
     def test_make_query_string(self):
         """Test make querystring."""
 
-        none_res = Requester("secret-key",
-                             endpoint="")._make_query_string(None)
+        none_res = Requester("secret-key", endpoint="")._make_query_string(None)
 
         assert none_res == ""
 
-        res = Requester("secret-key", endpoint="")._make_query_string({
-            "limit":
-            5,
-            "offset":
-            0,
-            "group": ["group1", "group2"],
-            "includeExports":
-            True
-        })
-
-        assert res == "limit=5&offset=0&group[]=group1&group[]=group2&includeExports=true&"
+        res = Requester("secret-key", endpoint="")._make_query_string(
+            {
+                "limit": 5,
+                "offset": 0,
+                "group": ["group1", "group2"],
+                "includeExports": True,
+            }
+        )
+
+        assert (
+            res == "limit=5&offset=0&group[]=group1&group[]=group2&includeExports=true&"
+        )
```

### Comparing `datature-1.6.0/test/test_utils.py` & `datature-1.7.0/tests/unit/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python
 # -*-coding:utf-8 -*-
-'''
+"""
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   test_requester.py
 @Author  :   Raighne.Weng
-@Version :   1.6.0
+@Version :   1.7.0
 @Contact :   developers@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature HTTP Resource Test Cases
-'''
+"""
 # pylint: disable=W0703,W0012,W0212
 
 import json
 import unittest
 
 import msgspec
-from requests import Session
-
-from datature.nexus.utils import utils
 from datature.nexus import models
+from datature.nexus.utils import utils
+from requests import Session
 
 
 class TestUtils(unittest.TestCase):
     """Datature Utils Test Cases."""
 
     def test_find_all_annotations_files(self):
         """Test find_all_annotations_files."""
@@ -57,25 +56,28 @@
         assert isinstance(session, Session)
 
     def test_get_download_path(self):
         """Test get_download_path."""
 
         # test get download path
         path = utils.get_download_path("../test")
-        assert 'test' in str(path)
+        assert "test" in str(path)
 
         path = utils.get_download_path()
+        assert "datature" in str(path)
 
     def test_download_files_to_tempfile(self):
         """Test download_files_to_tempfile."""
 
         # test get download path
         utils.download_files_to_tempfile(
             msgspec.json.decode(
-                json.dumps({
-                    "method": "GET",
-                    "url":
-                    "https://cdn.jsdelivr.net/npm/bootstrap@3.3.7/dist/js/bootstrap.min.js",
-                    "expiryDate": 1701755214003,
-                }),
+                json.dumps(
+                    {
+                        "method": "GET",
+                        "url": "https://cdn.jsdelivr.net/npm/bootstrap@3.3.7/dist/js/bootstrap.min.js",
+                        "expiryDate": 1701755214003,
+                    }
+                ),
                 type=models.DownloadSignedUrl,
-            ))
+            )
+        )
```

