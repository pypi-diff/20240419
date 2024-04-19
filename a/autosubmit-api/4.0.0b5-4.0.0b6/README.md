# Comparing `tmp/autosubmit_api-4.0.0b5.tar.gz` & `tmp/autosubmit_api-4.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit_api-4.0.0b5.tar", last modified: Mon Mar 18 14:14:08 2024, max compression
+gzip compressed data, was "autosubmit_api-4.0.0b6.tar", last modified: Fri Apr 19 11:55:56 2024, max compression
```

## Comparing `autosubmit_api-4.0.0b5.tar` & `autosubmit_api-4.0.0b6.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.789579 autosubmit_api-4.0.0b5/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    35147 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/LICENSE
--rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     6833 2024-03-18 14:14:08.789579 autosubmit_api-4.0.0b5/PKG-INFO
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4306 2024-03-18 14:10:28.000000 autosubmit_api-4.0.0b5/README.md
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      910 2024-02-23 13:55:46.000000 autosubmit_api-4.0.0b5/autosubmit_api/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2542 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/app.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/auth/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2343 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/auth/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      293 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/auth/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/job/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/job/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    47286 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/job/job_list.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1995 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12421 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/job/job_utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1632 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/bgtask.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1232 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/scheduler.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/tasks/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/tasks/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4376 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/tasks/status_updater.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/blueprints/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/blueprints/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3008 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/blueprints/v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3213 2024-03-18 10:26:34.000000 autosubmit_api-4.0.0b5/autosubmit_api/blueprints/v4.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.773579 autosubmit_api-4.0.0b5/autosubmit_api/builders/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      468 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      570 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/basic_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2652 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/configuration_facade_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3038 2024-03-18 09:22:08.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/experiment_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3142 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/experiment_history_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2626 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/joblist_helper_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1521 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/joblist_loader_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2194 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/builders/pkl_organizer_builder.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3485 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/cli.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/common/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/common/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7779 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/common/utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      596 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/common/utils_for_testing.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/components/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11007 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/configuration_facade.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5840 2024-03-06 16:19:09.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/pkl_organizer.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4072 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/test.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12790 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/job_factory.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3127 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/job_support.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3557 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/joblist_helper.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8695 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/joblist_loader.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9703 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1321 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/edge.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    17156 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6951 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/test.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/tree/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/tree/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2688 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/tree/test.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13728 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/components/representations/tree/tree.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/config/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    19521 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/config/IConfigStrategy.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1345 2024-03-01 11:34:43.000000 autosubmit_api-4.0.0b5/autosubmit_api/config/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3507 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/config/basicConfig.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    49166 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/config/confConfigStrategy.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    24148 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/config/config_common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    14118 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/config/ymlConfigStrategy.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/database/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      772 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2677 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20319 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/db_common.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    45645 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/db_jobdata.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9115 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/db_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3589 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/db_structure.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1128 2024-03-06 16:20:05.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/models.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2501 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/queries.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1308 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/tables.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      461 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/database/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/experiment/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/experiment/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4665 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/experiment/common_db_requests.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    52385 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/experiment/common_requests.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      647 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/experiment/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/history/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/history/data_classes/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/data_classes/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7563 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/data_classes/experiment_run.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11544 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/data_classes/job_data.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5829 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/database_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5197 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/database_models.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    23141 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6124 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/experiment_history.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2041 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/internal_logging.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3090 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/history/utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1606 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/logger.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/monitor/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/monitor/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9896 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/monitor/monitor.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/performance/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/performance/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8010 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/performance/performance_metrics.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1081 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/performance/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/persistance/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/persistance/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1688 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/persistance/experiment.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2287 2024-03-06 16:27:51.000000 autosubmit_api-4.0.0b5/autosubmit_api/persistance/pkl_reader.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/statistics/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/statistics/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2791 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/statistics/job_stat.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6956 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/statistics/statistics.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2565 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/statistics/stats_summary.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      177 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/statistics/utils.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/views/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      476 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/views/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13529 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/autosubmit_api/views/v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    14815 2024-03-18 10:47:27.000000 autosubmit_api-4.0.0b5/autosubmit_api/views/v4.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.777578 autosubmit_api-4.0.0b5/autosubmit_api/workers/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/__init__.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.781578 autosubmit_api-4.0.0b5/autosubmit_api/workers/business/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/business/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3010 2024-02-26 11:08:40.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/business/process_graph_drawings.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.781578 autosubmit_api-4.0.0b5/autosubmit_api/workers/populate_details/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/populate_details/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4279 2024-02-28 09:41:42.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/populate_details/populate.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      135 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/populate_details_db.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      218 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/populate_graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      269 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/populate_running_experiments.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      158 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b5/autosubmit_api/workers/test_esarchive.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.785578 autosubmit_api-4.0.0b5/autosubmit_api.egg-info/
--rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     6833 2024-03-18 14:14:08.000000 autosubmit_api-4.0.0b5/autosubmit_api.egg-info/PKG-INFO
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4983 2024-03-18 14:14:08.000000 autosubmit_api-4.0.0b5/autosubmit_api.egg-info/SOURCES.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        1 2024-03-18 14:14:08.000000 autosubmit_api-4.0.0b5/autosubmit_api.egg-info/dependency_links.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       59 2024-03-18 14:14:08.000000 autosubmit_api-4.0.0b5/autosubmit_api.egg-info/entry_points.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      729 2024-03-18 14:14:08.000000 autosubmit_api-4.0.0b5/autosubmit_api.egg-info/requires.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       21 2024-03-18 14:14:08.000000 autosubmit_api-4.0.0b5/autosubmit_api.egg-info/top_level.txt
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       38 2024-03-18 14:14:08.789579 autosubmit_api-4.0.0b5/setup.cfg
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2188 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/setup.py
-drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-03-18 14:14:08.785578 autosubmit_api-4.0.0b5/tests/
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b5/tests/__init__.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1337 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/tests/conftest.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      228 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b5/tests/custom_utils.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3377 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/tests/test_auth.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      714 2024-02-28 10:06:07.000000 autosubmit_api-4.0.0b5/tests/test_bg_tasks.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2871 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/tests/test_config.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    18820 2024-03-05 11:35:39.000000 autosubmit_api-4.0.0b5/tests/test_endpoints_v3.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5762 2024-03-18 11:16:14.000000 autosubmit_api-4.0.0b5/tests/test_endpoints_v4.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b5/tests/test_graph.py
--rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      531 2024-03-06 16:49:06.000000 autosubmit_api-4.0.0b5/tests/test_persistance.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    35147 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/LICENSE
+-rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     6833 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/PKG-INFO
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4306 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/README.md
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      910 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2542 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/app.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/auth/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2343 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/auth/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      293 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/auth/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    43697 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_list.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12421 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1632 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/bgtask.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1232 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/scheduler.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.212231 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4376 2024-04-04 11:33:45.000000 autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/status_updater.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3008 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3381 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v4.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/builders/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      468 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      570 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/basic_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2652 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/configuration_facade_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3038 2024-04-09 11:09:40.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3142 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_history_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2626 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_helper_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1521 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_loader_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2194 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/builders/pkl_organizer_builder.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3485 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/cli.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/common/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/common/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7779 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/common/utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      596 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/common/utils_for_testing.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11007 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/configuration_facade.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5840 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/pkl_organizer.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4072 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/test.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    12790 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_factory.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3127 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_support.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3902 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_helper.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8695 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_loader.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9703 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1321 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/edge.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    17188 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6951 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/test.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2688 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/test.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13728 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/tree.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/config/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    19521 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/IConfigStrategy.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1345 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3507 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/basicConfig.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    49166 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/confConfigStrategy.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    24148 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/config_common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    14118 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/config/ymlConfigStrategy.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/database/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      772 2024-04-09 11:09:48.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2677 2024-04-12 10:56:16.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20348 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_common.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    45645 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_jobdata.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9115 2024-04-11 13:47:25.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3627 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/db_structure.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1128 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/models.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2645 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/queries.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3491 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/tables.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      461 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/database/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/experiment/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3999 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/common_db_requests.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    52746 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/common_requests.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      647 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/experiment/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/history/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     7563 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/experiment_run.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    11544 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/job_data.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5829 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     5197 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_models.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    23141 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6124 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/experiment_history.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2041 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/internal_logging.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3090 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/history/utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1606 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/logger.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/monitor/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/monitor/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     9896 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/monitor/monitor.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/performance/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/performance/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     8010 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/performance/performance_metrics.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1081 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/performance/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/persistance/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1688 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/experiment.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3743 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/job_package_reader.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2287 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/persistance/pkl_reader.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/statistics/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2791 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/job_stat.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6956 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/statistics.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2565 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/stats_summary.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      177 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/statistics/utils.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/views/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      476 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/views/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    13529 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/autosubmit_api/views/v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    15492 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/autosubmit_api/views/v4.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/workers/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/__init__.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/workers/business/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/business/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3010 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/business/process_graph_drawings.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.216231 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4279 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/populate.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      135 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details_db.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      218 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      269 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_running_experiments.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      158 2023-10-11 07:46:00.000000 autosubmit_api-4.0.0b6/autosubmit_api/workers/test_esarchive.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/
+-rw-r--r--   0 ltenorio  (1001) ltenorio  (1001)     6833 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/PKG-INFO
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     4968 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        1 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       59 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/entry_points.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      729 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/requires.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       21 2024-04-19 11:55:56.000000 autosubmit_api-4.0.0b6/autosubmit_api.egg-info/top_level.txt
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)       38 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/setup.cfg
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2188 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/setup.py
+drwxrwxr-x   0 ltenorio  (1001) ltenorio  (1001)        0 2024-04-19 11:55:56.220231 autosubmit_api-4.0.0b6/tests/
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)        0 2024-01-08 13:52:35.000000 autosubmit_api-4.0.0b6/tests/__init__.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     1337 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/conftest.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      228 2024-02-09 11:10:01.000000 autosubmit_api-4.0.0b6/tests/custom_utils.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     3377 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/test_auth.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      714 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/tests/test_bg_tasks.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2871 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/test_config.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)    20138 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/tests/test_endpoints_v3.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     6473 2024-04-19 11:53:24.000000 autosubmit_api-4.0.0b6/tests/test_endpoints_v4.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)     2504 2024-02-23 13:54:52.000000 autosubmit_api-4.0.0b6/tests/test_graph.py
+-rw-rw-r--   0 ltenorio  (1001) ltenorio  (1001)      531 2024-03-18 14:29:27.000000 autosubmit_api-4.0.0b6/tests/test_persistance.py
```

### Comparing `autosubmit_api-4.0.0b5/LICENSE` & `autosubmit_api-4.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/PKG-INFO` & `autosubmit_api-4.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 4.0.0b5
+Version: 4.0.0b6
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/es/autosubmit_api
 Author: Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi
 Author-email: support-autosubmit@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-4.0.0b5/README.md` & `autosubmit_api-4.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/__init__.py` & `autosubmit_api-4.0.0b6/autosubmit_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "4.0.0b5"
+__version__ = "4.0.0b6"
 __author__ = "Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi"
 __credits__ = "Barcelona Supercomputing Center"
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/app.py` & `autosubmit_api-4.0.0b6/autosubmit_api/app.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/auth/__init__.py` & `autosubmit_api-4.0.0b6/autosubmit_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/job/job_list.py` & `autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,25 +24,22 @@
 
 # Spectral imports
 # End Spectral imports
 
 from time import time, mktime
 from dateutil.relativedelta import *
 
-from bscearth.utils.log import Log
 from autosubmit_api.autosubmit_legacy.job.job_utils import SubJob
 from autosubmit_api.autosubmit_legacy.job.job_utils import SubJobManager, job_times_to_text
 from autosubmit_api.config.basicConfig import APIBasicConfig
 from autosubmit_api.performance.utils import calculate_ASYPD_perjob, calculate_SYPD_perjob
 from autosubmit_api.components.jobs import utils as JUtils
 from autosubmit_api.monitor.monitor import Monitor
 from autosubmit_api.common.utils import Status
 from bscearth.utils.date import date2str, parse_date
-from autosubmit_api.experiment import common_db_requests as DbRequests
-from autosubmit_api.autosubmit_legacy.job.job_package_persistence import JobPackagePersistence
 # from autosubmit_legacy.job.tree import Tree
 from autosubmit_api.database import db_structure as DbStructure
 from autosubmit_api.database.db_jobdata import JobDataStructure, JobRow
 from autosubmit_api.builders.experiment_history_builder import ExperimentHistoryDirector, ExperimentHistoryBuilder
 from autosubmit_api.history.data_classes.job_data import JobData
 
 from typing import List, Dict, Tuple
@@ -586,19 +583,14 @@
 
         :return: job running to min (queue, run, status), job running to text (text)
         """
         # Getting information
         path_local_root = basic_config.LOCAL_ROOT_DIR
         path_structure = basic_config.STRUCTURES_DIR
         db_file = os.path.join(path_local_root, basic_config.DB_FILE)
-        conn = DbRequests.create_connection(db_file)
-        # job_data = None
-        # Job information from worker database
-        # job_times = dict() # REMOVED: DbRequests.get_times_detail_by_expid(conn, expid)
-        conn.close()
         # Job information from job historic data
         # print("Get current job data structure...")
         experiment_history = ExperimentHistoryDirector(ExperimentHistoryBuilder(expid)).build_reader_experiment_history()
         job_data = experiment_history.manager.get_all_last_job_data_dcs() if experiment_history.is_header_ready() else None
         # Result variables
         job_running_time_seconds = dict()
         job_running_to_runtext = dict()
@@ -842,76 +834,7 @@
                     status,
                     energy,
                     int(submit_time),
                     int(start_time),
                     int(finish_time),
                     None,
                     None)
-
-    @staticmethod
-    def retrieve_packages(basic_config, expid, current_jobs=None):
-        """
-        Retrieves dictionaries that map the collection of packages in the experiment
-
-        :param basic_config: Basic configuration
-        :type basic_config: Configuration Object
-        :param expid: Experiment Id
-        :type expid: String
-        :param current_jobs: list of names of current jobs
-        :type current_jobs: list
-        :return: job to package, package to jobs, package to package_id, package to symbol
-        :rtype: Dictionary(Job Object, Package_name), Dictionary(Package_name, List of Job Objects), Dictionary(String, String), Dictionary(String, String)
-        """
-        monitor = Monitor()
-        packages = None
-        exp_paths = ExperimentPaths(expid)
-        try:
-            packages = JobPackagePersistence(exp_paths.job_packages_db).load(wrapper=False)
-
-            # if the main table exist but is empty, we try the other one
-            if not (any(packages.keys()) or any(packages.values())):
-                Log.info("Wrapper table empty, trying packages.")
-                packages = JobPackagePersistence(exp_paths.job_packages_db).load(wrapper=True)
-
-
-        except Exception as ex:
-            print("Wrapper table not found, trying packages.")
-            packages = None
-            try:
-                packages = JobPackagePersistence(exp_paths.job_packages_db).load(wrapper=True)
-            except Exception as exp2:
-                packages = None
-                pass
-            pass
-
-        job_to_package = dict()
-        package_to_jobs = dict()
-        package_to_package_id = dict()
-        package_to_symbol = dict()
-        if (packages):
-            try:
-                for exp, package_name, job_name in packages:
-                    if len(str(package_name).strip()) > 0:
-                        if (current_jobs):
-                            if job_name in current_jobs:
-                                job_to_package[job_name] = package_name
-                        else:
-                            job_to_package[job_name] = package_name
-                    # list_packages.add(package_name)
-                for name in job_to_package:
-                    package_name = job_to_package[name]
-                    package_to_jobs.setdefault(package_name, []).append(name)
-                    # if package_name not in package_to_jobs.keys():
-                    #     package_to_jobs[package_name] = list()
-                    # package_to_jobs[package_name].append(name)
-                for key in package_to_jobs:
-                    package_to_package_id[key] = key.split("_")[2]
-                list_packages = list(job_to_package.values())
-                for i in range(len(list_packages)):
-                    if i % 2 == 0:
-                        package_to_symbol[list_packages[i]] = 'square'
-                    else:
-                        package_to_symbol[list_packages[i]] = 'hexagon'
-            except Exception as ex:
-                print((traceback.format_exc()))
-
-        return (job_to_package, package_to_jobs, package_to_package_id, package_to_symbol)
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/autosubmit_legacy/job/job_utils.py` & `autosubmit_api-4.0.0b6/autosubmit_api/autosubmit_legacy/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/bgtask.py` & `autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/bgtask.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/scheduler.py` & `autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/scheduler.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/bgtasks/tasks/status_updater.py` & `autosubmit_api-4.0.0b6/autosubmit_api/bgtasks/tasks/status_updater.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/blueprints/v3.py` & `autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/blueprints/v4.py` & `autosubmit_api-4.0.0b6/autosubmit_api/blueprints/v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     )
 
     blueprint.add_url_rule(
         "/experiments/<string:expid>/jobs",
         view_func=v4_views.ExperimentJobsView.as_view("ExperimentJobsView"),
     )
 
+    blueprint.add_url_rule(
+        "/experiments/<string:expid>/wrappers",
+        view_func=v4_views.ExperimentWrappersView.as_view("ExperimentWrappersView"),
+    )
+
     # blueprint.route("/experiments/<string:expid>/runs")(v3_views.get_runs)
     # blueprint.route("/experiments/<string:expid>/check-running")(
     #     v3_views.get_if_running
     # )
     # blueprint.route("/experiments/<string:expid>/running-detail")(
     #     v3_views.get_running_detail
     # )
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/builders/basic_builder.py` & `autosubmit_api-4.0.0b6/autosubmit_api/builders/basic_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/builders/configuration_facade_builder.py` & `autosubmit_api-4.0.0b6/autosubmit_api/builders/configuration_facade_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/builders/experiment_builder.py` & `autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/builders/experiment_history_builder.py` & `autosubmit_api-4.0.0b6/autosubmit_api/builders/experiment_history_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/builders/joblist_helper_builder.py` & `autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_helper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/builders/joblist_loader_builder.py` & `autosubmit_api-4.0.0b6/autosubmit_api/builders/joblist_loader_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/builders/pkl_organizer_builder.py` & `autosubmit_api-4.0.0b6/autosubmit_api/builders/pkl_organizer_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/cli.py` & `autosubmit_api-4.0.0b6/autosubmit_api/cli.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/common/utils.py` & `autosubmit_api-4.0.0b6/autosubmit_api/common/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/common/utils_for_testing.py` & `autosubmit_api-4.0.0b6/autosubmit_api/common/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/configuration_facade.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/configuration_facade.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/pkl_organizer.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/pkl_organizer.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/experiment/test.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/experiment/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/job_factory.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/job_support.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/job_support.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/joblist_helper.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from autosubmit_api.common.utils import datechunk_to_year
 from autosubmit_api.database.db_jobdata import JobDataStructure, JobRow
 from autosubmit_api.components.experiment.configuration_facade import AutosubmitConfigurationFacade
 from autosubmit_api.components.experiment.pkl_organizer import PklOrganizer
 from autosubmit_api.config.basicConfig import APIBasicConfig
 from typing import List, Dict
 from autosubmit_api.components.jobs.job_factory import Job
+from autosubmit_api.persistance.job_package_reader import JobPackageReader
 
 class JobListHelper(object):
   """ Loads time (queuing runnning) and packages. Applies the fix for queue time of jobs in wrappers. """
   def __init__(self, expid, configuration_facade, pkl_organizer, basic_config):
     # type: (str, AutosubmitConfigurationFacade, PklOrganizer, APIBasicConfig) -> None
     self.basic_config = basic_config # type: APIBasicConfig
     self.configuration_facade = configuration_facade # type: AutosubmitConfigurationFacade
@@ -24,16 +25,24 @@
     self._run_id_to_run_object = {} # type: Dict
     self.warning_messages = [] # type: List
     self.expid = expid # type: str
     self.simple_jobs = self.pkl_organizer.get_simple_jobs(self.configuration_facade.tmp_path)
     self._initialize_main_values()
 
   def _initialize_main_values(self):
-    # type: () -> None
-    self.job_to_package, self.package_to_jobs, self.package_to_package_id, self.package_to_symbol = JobList.retrieve_packages(self.basic_config, self.expid)
+    job_package_reader = JobPackageReader(self.expid)
+    try:
+      job_package_reader.read()
+      self.job_to_package = job_package_reader.job_to_package
+      self.package_to_jobs = job_package_reader.package_to_jobs
+      self.package_to_package_id = job_package_reader.package_to_package_id
+      self.package_to_symbol = job_package_reader.package_to_symbol
+    except:
+      self.warning_messages.append("Failed to read job_packages")
+      
     self.job_name_to_job_row, self.job_running_time_to_text, self.warning_messages  = JobList.get_job_times_collection(
                 self.basic_config, self.simple_jobs, self.expid, self.job_to_package, self.package_to_jobs, timeseconds=True)
 
   def update_with_timedata(self, section_jobs):
     # type: (List[Job]) -> None
     """ Update Job information with JobRow (time) data from Historical Database (Or as_times information) """
     for job in section_jobs:
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/joblist_loader.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/joblist_loader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/jobs/utils.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/edge.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/edge.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/graph.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,15 @@
         "label": job.name,
         "status": job.status_text,
         "status_code": job.status,
         "status_color": job.status_color,
         "platform_name": job.platform,
         "chunk": job.chunk,
         "package": job.package,
+        "wrapper": job.package,
         "member": job.member,
         "date": ini_date,
         "date_plus": end_date,
         "SYPD": PUtils.calculate_SYPD_perjob(self.joblist_loader.chunk_unit, self.joblist_loader.chunk_size, job.chunk, job.run_time, job.status),
         "ASYPD": PUtils.calculate_ASYPD_perjob(self.joblist_loader.chunk_unit, self.joblist_loader.chunk_size, job.chunk, job.total_time, self.average_post_time, job.status),
         "minutes_queue": job.queue_time,
         "minutes": job.run_time,
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/representations/graph/test.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/graph/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/representations/tree/test.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/components/representations/tree/tree.py` & `autosubmit_api-4.0.0b6/autosubmit_api/components/representations/tree/tree.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/config/IConfigStrategy.py` & `autosubmit_api-4.0.0b6/autosubmit_api/config/IConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/config/__init__.py` & `autosubmit_api-4.0.0b6/autosubmit_api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/config/basicConfig.py` & `autosubmit_api-4.0.0b6/autosubmit_api/config/basicConfig.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/config/confConfigStrategy.py` & `autosubmit_api-4.0.0b6/autosubmit_api/config/confConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/config/config_common.py` & `autosubmit_api-4.0.0b6/autosubmit_api/config/config_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/config/ymlConfigStrategy.py` & `autosubmit_api-4.0.0b6/autosubmit_api/config/ymlConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/__init__.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/common.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/db_common.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/db_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,14 +378,15 @@
     if not check_db():
         return result
     (conn, cursor) = open_conn()
     query = "SELECT id, name, description, autosubmit_version FROM experiment WHERE name ='" + expid + "'"
     cursor.execute(query)
     headers = get_headers_sqlite(cursor)
     row = cursor.fetchone()
+    close_conn(conn, cursor)
     if row is not None:
         obj = map_row_result_to_dict_sqlite(row, headers)
         result['id'] = obj["id"]
         result['name'] = obj["name"]
         result['description'] = obj["description"]
         result['version'] = obj["autosubmit_version"]
     return result
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/db_jobdata.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/db_jobdata.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/db_manager.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/db_structure.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/db_structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,23 @@
         if os.path.exists(db_structure_path):
             # Create file
             os.umask(0)
             if not os.path.exists(db_structure_path):
                 os.open(db_structure_path, os.O_WRONLY | os.O_CREAT, 0o777)
                 # open(db_structure_path, "w")
             # print(db_structure_path)
-            conn = create_connection(db_structure_path)
             create_table_query = textwrap.dedent(
                 '''CREATE TABLE
             IF NOT EXISTS experiment_structure (
             e_from text NOT NULL,
             e_to text NOT NULL,
             UNIQUE(e_from,e_to)
             );''')
-            create_table(conn, create_table_query)
+            with create_connection(db_structure_path) as conn:
+                create_table(conn, create_table_query)
             current_table = _get_exp_structure(db_structure_path)
             # print("Current table: ")
             # print(current_table)
             current_table_structure = dict()
             for item in current_table:
                 _from, _to = item
                 current_table_structure.setdefault(_from, []).append(_to)
@@ -88,17 +88,17 @@
 def _get_exp_structure(path):
     """
     Get all registers from experiment_status.\n
     :return: row content: exp_id, name, status, seconds_diff
     :rtype: 4-tuple (int, str, str, int)
     """
     try:
-        conn = create_connection(path)
-        conn.text_factory = str
-        cur = conn.cursor()
-        cur.execute(
-            "SELECT e_from, e_to FROM experiment_structure")
-        rows = cur.fetchall()
+        with create_connection(path) as conn:
+            conn.text_factory = str
+            cur = conn.cursor()
+            cur.execute(
+                "SELECT e_from, e_to FROM experiment_structure")
+            rows = cur.fetchall()
         return rows
     except Exception as exp:
         print((traceback.format_exc()))
         return dict()
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/models.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/database/queries.py` & `autosubmit_api-4.0.0b6/autosubmit_api/database/queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 def generate_query_listexp_extended(
     query: str = None,
     only_active: bool = False,
     owner: str = None,
     exp_type: str = None,
+    autosubmit_version: str = None,
     order_by: str = None,
     order_desc: bool = False,
 ):
     """
     Query listexp without accessing the view with status and total/completed jobs.
     """
 
@@ -57,15 +58,19 @@
         filter_stmts.append(tables.experiment_table.c.name.like(f"t%"))
     elif exp_type == "operational":
         filter_stmts.append(tables.experiment_table.c.name.like(f"o%"))
     elif exp_type == "experiment":
         filter_stmts.append(tables.experiment_table.c.name.not_like(f"t%"))
         filter_stmts.append(tables.experiment_table.c.name.not_like(f"o%"))
 
-    # logger.debug(str(filter_stmts))
+    if autosubmit_version:
+        filter_stmts.append(
+            tables.experiment_table.c.autosubmit_version == autosubmit_version
+        )
+
     statement = statement.where(*filter_stmts)
 
     # Order by
     ORDER_OPTIONS = {
         "expid": tables.experiment_table.c.name,
         "created": tables.details_table.c.created,
         "description": tables.experiment_table.c.description,
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/experiment/common_requests.py` & `autosubmit_api-4.0.0b6/autosubmit_api/experiment/common_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from autosubmit_api.autosubmit_legacy.job.job_list import JobList
 from autosubmit_api.logger import logger
 
 from autosubmit_api.performance.utils import calculate_SYPD_perjob
 from autosubmit_api.monitor.monitor import Monitor
 from autosubmit_api.persistance.experiment import ExperimentPaths
 
+from autosubmit_api.persistance.job_package_reader import JobPackageReader
 from autosubmit_api.statistics.statistics import Statistics
 
 from autosubmit_api.config.basicConfig import APIBasicConfig
 from autosubmit_api.config.config_common import AutosubmitConfigResolver
 from bscearth.utils.config_parser import ConfigParserFactory
 
 from autosubmit_api.components.representations.tree.tree import TreeRepresentation
@@ -305,20 +306,19 @@
     error_message = ""
     try:
         # Basic paths
         APIBasicConfig.read()
         tmp_path = os.path.join(
             APIBasicConfig.LOCAL_ROOT_DIR, expid, APIBasicConfig.LOCAL_TMP_DIR)
         # Try to get packages
-        job_to_package = dict()
-        package_to_jobs = dict()
-        package_to_package_id = dict()
-        package_to_symbol = dict()
-        job_to_package, package_to_jobs, package_to_package_id, package_to_symbol = JobList.retrieve_packages(
-            APIBasicConfig, expid)
+        job_package_reader = JobPackageReader(expid)
+        try:
+            job_package_reader.read()
+        except:
+            logger.warning("Failed to read job_packages")
         # Basic data
         job_running_to_seconds = dict()
         job_running_to_runtext = dict()
         jobs_in_pkl = dict()
         fakeAllJobs = list()
 
         # Read PKL
@@ -334,17 +334,25 @@
             err = job_item.err_path_local
             status_color = Monitor.color_status(status_code)
             status_text = str(common_utils.Status.VALUE_TO_KEY[status_code])
             jobs_in_pkl[job_name] = (
                 status_code, status_color, status_text, out, err, priority, id_number)
             fakeAllJobs.append(
                 SimpleJob(job_name, tmp_path, status_code))
-            
-        job_running_to_seconds, job_running_to_runtext, _ = JobList.get_job_times_collection(
-            APIBasicConfig, fakeAllJobs, expid, job_to_package, package_to_jobs, timeseconds=True)
+
+        job_running_to_seconds, job_running_to_runtext, _ = (
+            JobList.get_job_times_collection(
+                APIBasicConfig,
+                fakeAllJobs,
+                expid,
+                job_package_reader.job_to_package,
+                job_package_reader.package_to_jobs,
+                timeseconds=True,
+            )
+        )
 
         # Main Loop
         if len(list(job_running_to_seconds.keys())) > 0:
             for job_name in list(jobs_in_pkl.keys()):
                 # print(value)
                 job_info = job_running_to_seconds[job_name] if job_name in list(job_running_to_seconds.keys(
                 )) else None
@@ -820,16 +828,25 @@
     try:
         APIBasicConfig.read()
         exp_paths = ExperimentPaths(expid)
         path_to_logs = exp_paths.tmp_log_dir
 
         # Retrieving packages
         now_ = time.time()
-        job_to_package, package_to_jobs, package_to_package_id, package_to_symbol = JobList.retrieve_packages(
-            APIBasicConfig, expid)
+        job_to_package = {}
+        package_to_package_id = {}
+
+        job_package_reader = JobPackageReader(expid)
+        try:
+            job_package_reader.read()
+            job_to_package = job_package_reader.job_to_package
+            package_to_package_id = job_package_reader.package_to_package_id
+        except:
+            logger.warning("Failed to read job_packages")
+        
         logger.debug(("Retrieving packages {0} seconds.".format(
             str(time.time() - now_))))
         
         # Reading PKL
         try:
             autosubmit_config_facade = ConfigurationFacadeDirector(
                 AutosubmitConfigurationFacadeBuilder(expid)).build_autosubmit_configuration_facade()
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/experiment/utils.py` & `autosubmit_api-4.0.0b6/autosubmit_api/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/data_classes/experiment_run.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/data_classes/job_data.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/database_manager.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/database_models.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/database_managers/experiment_history_db_manager.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/experiment_history.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/internal_logging.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/history/utils.py` & `autosubmit_api-4.0.0b6/autosubmit_api/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/logger.py` & `autosubmit_api-4.0.0b6/autosubmit_api/logger.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/monitor/monitor.py` & `autosubmit_api-4.0.0b6/autosubmit_api/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/performance/performance_metrics.py` & `autosubmit_api-4.0.0b6/autosubmit_api/performance/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/performance/utils.py` & `autosubmit_api-4.0.0b6/autosubmit_api/performance/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/persistance/experiment.py` & `autosubmit_api-4.0.0b6/autosubmit_api/persistance/experiment.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/persistance/pkl_reader.py` & `autosubmit_api-4.0.0b6/autosubmit_api/persistance/pkl_reader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/statistics/job_stat.py` & `autosubmit_api-4.0.0b6/autosubmit_api/statistics/job_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/statistics/statistics.py` & `autosubmit_api-4.0.0b6/autosubmit_api/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/statistics/stats_summary.py` & `autosubmit_api-4.0.0b6/autosubmit_api/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/views/v3.py` & `autosubmit_api-4.0.0b6/autosubmit_api/views/v3.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/views/v4.py` & `autosubmit_api-4.0.0b6/autosubmit_api/views/v4.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from collections import deque
 from datetime import datetime, timedelta
 from enum import Enum
 from http import HTTPStatus
 import math
 import traceback
-from typing import Optional
+from typing import Dict, List, Optional
 from flask import redirect, request
 from flask.views import MethodView
 import jwt
 import requests
 from autosubmit_api.auth import ProtectionLevels, with_auth_token
 from autosubmit_api.auth.utils import validate_client
 from autosubmit_api.builders.experiment_builder import ExperimentBuilder
 from autosubmit_api.builders.experiment_history_builder import (
     ExperimentHistoryBuilder,
     ExperimentHistoryDirector,
 )
 from autosubmit_api.common.utils import Status
 from autosubmit_api.database import tables
 from autosubmit_api.database.common import (
-    create_autosubmit_db_engine,
     create_main_db_conn,
     execute_with_limit_offset,
 )
-from autosubmit_api.database.models import ExperimentModel
 from autosubmit_api.database.queries import generate_query_listexp_extended
 from autosubmit_api.logger import logger, with_log_run_times
 from cas import CASClient
 from autosubmit_api import config
+from autosubmit_api.persistance.job_package_reader import JobPackageReader
 from autosubmit_api.persistance.pkl_reader import PklReader
 
 
 PAGINATION_LIMIT_DEFAULT = 12
 
 
 class CASV2Login(MethodView):
@@ -213,14 +212,15 @@
         # Parse args
         logger.debug("Search args: " + str(request.args))
 
         query = request.args.get("query")
         only_active = request.args.get("only_active") == "true"
         owner = request.args.get("owner")
         exp_type = request.args.get("exp_type")
+        autosubmit_version = request.args.get("autosubmit_version")
 
         order_by = request.args.get("order_by")
         order_desc = request.args.get("order_desc") == "true"
 
         try:
             page = max(request.args.get("page", default=1, type=int), 1)
             page_size = request.args.get(
@@ -236,14 +236,15 @@
 
         # Query
         statement = generate_query_listexp_extended(
             query=query,
             only_active=only_active,
             owner=owner,
             exp_type=exp_type,
+            autosubmit_version=autosubmit_version,
             order_by=order_by,
             order_desc=order_desc,
         )
         with create_main_db_conn() as conn:
             query_result, total_rows = execute_with_limit_offset(
                 statement=statement,
                 conn=conn,
@@ -401,7 +402,25 @@
 
             if job_item.status in [Status.COMPLETED, Status.WAITING, Status.READY]:
                 pkl_jobs.append(resp_job)
             else:
                 pkl_jobs.appendleft(resp_job)
 
         return {"jobs": list(pkl_jobs)}, HTTPStatus.OK
+
+
+class ExperimentWrappersView(MethodView):
+    decorators = [with_auth_token(), with_log_run_times(logger, "WRAPPERS")]
+
+    def get(self, expid: str, user_id: Optional[str] = None):
+
+        job_package_reader = JobPackageReader(expid)
+        job_package_reader.read()
+
+        wrappers_dict: Dict[str, List[str]] = job_package_reader.package_to_jobs
+
+        wrappers = []
+        for key, val in wrappers_dict.items():
+            wrappers.append({"wrapper_name": key, "job_names": val})
+
+        logger.debug(wrappers)
+        return {"wrappers": wrappers}
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/workers/business/process_graph_drawings.py` & `autosubmit_api-4.0.0b6/autosubmit_api/workers/business/process_graph_drawings.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api/workers/populate_details/populate.py` & `autosubmit_api-4.0.0b6/autosubmit_api/workers/populate_details/populate.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api.egg-info/PKG-INFO` & `autosubmit_api-4.0.0b6/autosubmit_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 4.0.0b5
+Version: 4.0.0b6
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/es/autosubmit_api
 Author: Luiggi Tenorio, Bruno P. Kinoshita, Cristian Gutiérrez, Julian Berlin, Wilmer Uruchi
 Author-email: support-autosubmit@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api.egg-info/SOURCES.txt` & `autosubmit_api-4.0.0b6/autosubmit_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 autosubmit_api.egg-info/requires.txt
 autosubmit_api.egg-info/top_level.txt
 autosubmit_api/auth/__init__.py
 autosubmit_api/auth/utils.py
 autosubmit_api/autosubmit_legacy/__init__.py
 autosubmit_api/autosubmit_legacy/job/__init__.py
 autosubmit_api/autosubmit_legacy/job/job_list.py
-autosubmit_api/autosubmit_legacy/job/job_package_persistence.py
 autosubmit_api/autosubmit_legacy/job/job_utils.py
 autosubmit_api/bgtasks/__init__.py
 autosubmit_api/bgtasks/bgtask.py
 autosubmit_api/bgtasks/scheduler.py
 autosubmit_api/bgtasks/tasks/__init__.py
 autosubmit_api/bgtasks/tasks/status_updater.py
 autosubmit_api/blueprints/__init__.py
@@ -90,14 +89,15 @@
 autosubmit_api/monitor/__init__.py
 autosubmit_api/monitor/monitor.py
 autosubmit_api/performance/__init__.py
 autosubmit_api/performance/performance_metrics.py
 autosubmit_api/performance/utils.py
 autosubmit_api/persistance/__init__.py
 autosubmit_api/persistance/experiment.py
+autosubmit_api/persistance/job_package_reader.py
 autosubmit_api/persistance/pkl_reader.py
 autosubmit_api/statistics/__init__.py
 autosubmit_api/statistics/job_stat.py
 autosubmit_api/statistics/statistics.py
 autosubmit_api/statistics/stats_summary.py
 autosubmit_api/statistics/utils.py
 autosubmit_api/views/__init__.py
```

### Comparing `autosubmit_api-4.0.0b5/autosubmit_api.egg-info/requires.txt` & `autosubmit_api-4.0.0b6/autosubmit_api.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/setup.py` & `autosubmit_api-4.0.0b6/setup.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/tests/conftest.py` & `autosubmit_api-4.0.0b6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/tests/test_auth.py` & `autosubmit_api-4.0.0b6/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/tests/test_bg_tasks.py` & `autosubmit_api-4.0.0b6/tests/test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/tests/test_config.py` & `autosubmit_api-4.0.0b6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/tests/test_endpoints_v3.py` & `autosubmit_api-4.0.0b6/tests/test_endpoints_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,31 @@
         assert resp_obj["total"] == len(resp_obj["jobs"])
         assert (
             len([job for job in resp_obj["jobs"] if job["status"] == "COMPLETED"]) == 24
         )
         for job in resp_obj["jobs"]:
             assert job["id"][:4] == expid
 
+    def test_wrappers(self, fixture_client: FlaskClient):
+        expid = "a6zj"
+        response = fixture_client.get(self.endpoint.format(expid=expid))
+        resp_obj: dict = response.get_json()
+
+        assert len(resp_obj["jobs"]) == 10
+
+        for job in resp_obj["jobs"]:
+            if job["section"] == "SIM":
+                assert isinstance(job["wrapper"], str) and len(job["wrapper"]) > 0
+            else:
+                assert job["wrapper"] == None
+
+        assert (
+            resp_obj["tree"][2]["title"] == "Wrappers" and resp_obj["tree"][2]["folder"]
+        )
+
 
 class TestRunsList:
     endpoint = "/v3/runs/{expid}"
 
     def test_runs_list(self, fixture_client: FlaskClient):
         expid = "a003"
 
@@ -306,14 +323,34 @@
             query_string={"loggedUser": random_user},
         )
         resp_obj: dict = response.get_json()
         assert resp_obj["error_message"] == ""
         assert resp_obj["error"] == False
         assert resp_obj["total_jobs"] == len(resp_obj["nodes"])
 
+    def test_wrappers(self, fixture_client: FlaskClient):
+        expid = "a6zj"
+        random_user = str(uuid4())
+        response = fixture_client.get(
+            self.endpoint.format(expid=expid, graph_type="standard", grouped="none"),
+            query_string={"loggedUser": random_user},
+        )
+        resp_obj: dict = response.get_json()
+
+        assert len(resp_obj["nodes"]) == 10
+
+        for node in resp_obj["nodes"]:
+            if node["section"] == "SIM":
+                assert isinstance(node["wrapper"], str) and len(node["wrapper"]) > 0
+            else:
+                assert node["wrapper"] == None
+
+        assert "packages" in list(resp_obj.keys())
+        assert len(resp_obj["packages"].keys()) > 0
+
 
 class TestExpCount:
     endpoint = "/v3/expcount/{expid}"
 
     def test_exp_count(self, fixture_client: FlaskClient):
         expid = "a003"
         response = fixture_client.get(self.endpoint.format(expid=expid))
@@ -522,14 +559,15 @@
         expid = "a3tb"
         response = fixture_client.get(self.endpoint.format(expid=expid))
         resp_obj: dict = response.get_json()
 
         assert isinstance(resp_obj["experiment"], list)
         assert len(resp_obj["experiment"]) > 0
 
+
 class TestRunningExps:
     endpoint = "/v3/running/"
 
     def test_search_by_expid(self, fixture_client: FlaskClient):
         expid = "a3tb"
         response = fixture_client.get(self.endpoint)
         resp_obj: dict = response.get_json()
```

### Comparing `autosubmit_api-4.0.0b5/tests/test_endpoints_v4.py` & `autosubmit_api-4.0.0b6/tests/test_endpoints_v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,7 +158,28 @@
 
         assert len(resp_obj["jobs"]) == 8
 
         for job in resp_obj["jobs"]:
             assert isinstance(job, dict) and len(job.keys()) > 2
             assert isinstance(job["name"], str) and job["name"].startswith(expid)
             assert isinstance(job["status"], str)
+
+
+class TestExperimentWrappers:
+    endpoint = "/v4/experiments/{expid}/wrappers"
+
+    def test_wrappers(self, fixture_client: FlaskClient):
+        expid = "a6zj"
+
+        response = fixture_client.get(self.endpoint.format(expid=expid))
+        resp_obj: dict = response.get_json()
+
+        assert isinstance(resp_obj, dict)
+        assert isinstance(resp_obj["wrappers"], list)
+        assert len(resp_obj["wrappers"]) == 1
+
+        for wrapper in resp_obj["wrappers"]:
+            assert isinstance(wrapper, dict)
+            assert isinstance(wrapper["job_names"], list)
+            assert isinstance(wrapper["wrapper_name"], str) and wrapper[
+                "wrapper_name"
+            ].startswith(expid)
```

### Comparing `autosubmit_api-4.0.0b5/tests/test_graph.py` & `autosubmit_api-4.0.0b6/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-4.0.0b5/tests/test_persistance.py` & `autosubmit_api-4.0.0b6/tests/test_persistance.py`

 * *Files identical despite different names*

