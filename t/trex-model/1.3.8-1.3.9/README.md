# Comparing `tmp/trex-model-1.3.8.tar.gz` & `tmp/trex-model-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-model-1.3.8.tar", last modified: Thu Mar 28 07:16:55 2024, max compression
+gzip compressed data, was "dist/trex-model-1.3.9.tar", last modified: Fri Apr 19 01:40:19 2024, max compression
```

## Comparing `trex-model-1.3.8.tar` & `trex-model-1.3.9.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2024-03-28 07:16:55.000000 trex-model-1.3.8/PKG-INFO
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)    29337 2024-01-27 11:17:47.000000 trex-model-1.3.8/trexmodel/program_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2287 2024-01-25 03:42:44.000000 trex-model-1.3.8/trexmodel/conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.3.8/trexmodel/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/trexmodel/utils/
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.3.8/trexmodel/utils/gcloud/datastore_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.8/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.8/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.3.8/trexmodel/utils/model/model_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.8/trexmodel/utils/model/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)     9261 2023-08-24 06:48:34.000000 trex-model-1.3.8/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.3.8/trexmodel/models/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.3.8/trexmodel/models/prepaid_helpers.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)     8552 2024-03-01 08:11:33.000000 trex-model-1.3.8/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8329 2023-12-27 03:18:38.000000 trex-model-1.3.8/trexmodel/models/datastore/import_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14671 2024-02-07 03:32:09.000000 trex-model-1.3.8/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4099 2024-01-25 06:53:38.000000 trex-model-1.3.8/trexmodel/models/datastore/message_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.3.8/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    34842 2023-11-07 09:43:31.000000 trex-model-1.3.8/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.3.8/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)    55190 2024-03-14 06:45:08.000000 trex-model-1.3.8/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22092 2024-01-30 05:47:01.000000 trex-model-1.3.8/trexmodel/models/datastore/message_model_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.3.8/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.3.8/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7135 2023-09-21 07:48:57.000000 trex-model-1.3.8/trexmodel/models/datastore/reward_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32185 2023-12-22 02:46:56.000000 trex-model-1.3.8/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2076 2024-03-28 07:14:43.000000 trex-model-1.3.8/trexmodel/models/datastore/recruit_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22417 2024-01-19 04:31:41.000000 trex-model-1.3.8/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    39078 2023-12-14 09:37:29.000000 trex-model-1.3.8/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17001 2024-01-02 05:38:53.000000 trex-model-1.3.8/trexmodel/models/datastore/redemption_catalogue_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1662 2023-08-16 15:50:05.000000 trex-model-1.3.8/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    39811 2024-01-30 09:18:08.000000 trex-model-1.3.8/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8555 2024-02-15 08:43:33.000000 trex-model-1.3.8/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19218 2024-01-01 16:01:07.000000 trex-model-1.3.8/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    20632 2023-12-01 03:25:17.000000 trex-model-1.3.8/trexmodel/models/datastore/rating_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.3.8/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    49135 2024-01-01 14:50:39.000000 trex-model-1.3.8/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.3.8/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    19899 2024-01-18 06:33:46.000000 trex-model-1.3.8/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.3.8/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    41297 2023-12-17 08:11:57.000000 trex-model-1.3.8/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12170 2024-03-06 03:28:38.000000 trex-model-1.3.8/trexmodel/models/datastore/marketing_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2397 2023-05-24 02:56:50.000000 trex-model-1.3.8/trexmodel/models/datastore/app_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15032 2024-03-14 09:02:34.000000 trex-model-1.3.8/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    74697 2024-01-15 09:30:14.000000 trex-model-1.3.8/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    28234 2024-01-30 09:33:33.000000 trex-model-1.3.8/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    41691 2024-02-05 10:11:10.000000 trex-model-1.3.8/trexmodel/models/datastore/lucky_draw_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.3.8/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.3.8/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.3.8/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.3.8/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.3.8/LICENSE
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-28 07:16:55.000000 trex-model-1.3.8/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2024-03-28 07:16:55.000000 trex-model-1.3.8/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     2273 2024-03-28 07:16:55.000000 trex-model-1.3.8/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2024-03-28 07:16:55.000000 trex-model-1.3.8/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2024-03-28 07:16:55.000000 trex-model-1.3.8/trex_model.egg-info/top_level.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-03-28 07:16:55.000000 trex-model-1.3.8/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.3.8/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.3.8/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2024-03-28 07:16:46.000000 trex-model-1.3.8/setup.py
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-03-28 07:16:55.000000 trex-model-1.3.8/setup.cfg
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2024-04-19 01:40:19.000000 trex-model-1.3.9/PKG-INFO
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:18.000000 trex-model-1.3.9/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)    32565 2024-04-17 15:19:03.000000 trex-model-1.3.9/trexmodel/program_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2287 2024-01-25 03:42:44.000000 trex-model-1.3.9/trexmodel/conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.3.9/trexmodel/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/utils/
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/gcloud/datastore_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.3.9/trexmodel/utils/model/model_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.3.9/trexmodel/utils/model/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:18.000000 trex-model-1.3.9/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)     9261 2023-08-24 06:48:34.000000 trex-model-1.3.9/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.3.9/trexmodel/models/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.3.9/trexmodel/models/prepaid_helpers.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:19.000000 trex-model-1.3.9/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)     8552 2024-03-01 08:11:33.000000 trex-model-1.3.9/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8329 2023-12-27 03:18:38.000000 trex-model-1.3.9/trexmodel/models/datastore/import_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14671 2024-02-07 03:32:09.000000 trex-model-1.3.9/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4099 2024-01-25 06:53:38.000000 trex-model-1.3.9/trexmodel/models/datastore/message_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.3.9/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    34842 2023-11-07 09:43:31.000000 trex-model-1.3.9/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.3.9/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    55190 2024-04-17 09:40:14.000000 trex-model-1.3.9/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22092 2024-01-30 05:47:01.000000 trex-model-1.3.9/trexmodel/models/datastore/message_model_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.3.9/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.3.9/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7135 2023-09-21 07:48:57.000000 trex-model-1.3.9/trexmodel/models/datastore/reward_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32185 2023-12-22 02:46:56.000000 trex-model-1.3.9/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2076 2024-03-28 07:14:43.000000 trex-model-1.3.9/trexmodel/models/datastore/recruit_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22417 2024-01-19 04:31:41.000000 trex-model-1.3.9/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    39078 2023-12-14 09:37:29.000000 trex-model-1.3.9/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17001 2024-04-13 08:31:55.000000 trex-model-1.3.9/trexmodel/models/datastore/redemption_catalogue_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1662 2023-08-16 15:50:05.000000 trex-model-1.3.9/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    39811 2024-01-30 09:18:08.000000 trex-model-1.3.9/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16394 2024-04-18 02:51:01.000000 trex-model-1.3.9/trexmodel/models/datastore/referral_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8555 2024-02-15 08:43:33.000000 trex-model-1.3.9/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19218 2024-01-01 16:01:07.000000 trex-model-1.3.9/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20632 2023-12-01 03:25:17.000000 trex-model-1.3.9/trexmodel/models/datastore/rating_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.3.9/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    49184 2024-04-17 11:58:10.000000 trex-model-1.3.9/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.3.9/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    19899 2024-01-18 06:33:46.000000 trex-model-1.3.9/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.3.9/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    41297 2023-12-17 08:11:57.000000 trex-model-1.3.9/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12170 2024-03-06 03:28:38.000000 trex-model-1.3.9/trexmodel/models/datastore/marketing_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2397 2023-05-24 02:56:50.000000 trex-model-1.3.9/trexmodel/models/datastore/app_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15032 2024-03-14 09:02:34.000000 trex-model-1.3.9/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    83773 2024-04-18 09:25:49.000000 trex-model-1.3.9/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    28234 2024-01-30 09:33:33.000000 trex-model-1.3.9/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    41800 2024-04-17 14:45:19.000000 trex-model-1.3.9/trexmodel/models/datastore/lucky_draw_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.3.9/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.3.9/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.3.9/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.3.9/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.3.9/LICENSE
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     2326 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/top_level.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-19 01:40:18.000000 trex-model-1.3.9/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.3.9/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.3.9/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2024-04-19 01:39:39.000000 trex-model-1.3.9/setup.py
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-19 01:40:19.000000 trex-model-1.3.9/setup.cfg
```

### Comparing `trex-model-1.3.8/trexmodel/program_conf.py` & `trex-model-1.3.9/trexmodel/program_conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 
 FEATURE_CODE_TIER_REWARD_PROGRAM            = 'tier_reward'
 
 FEATURE_CODE_REWARDING_PROGRAM              = 'rewarding'
 FEATURE_CODE_REDEMPTION_PROGRAM             = 'redemption'
 FEATURE_CODE_LUCKY_DRAW_PROGRAM             = 'lucky_draw'
+FEATURE_CODE_REFERRAL_PROGRAM               = 'referral'
 
 PRODUCT_CODE_POINT_OF_SALES                 = 'pos'
 PRODUCT_CODE_LOYALTY                        = 'loyalty'
 
 
 
 
@@ -110,15 +111,15 @@
                                                 FEATURE_CODE_REDEMPTION_PROGRAM,
                                                 ],
                                        
                                        LOYALTY_PACKAGE_SCALE:[
                                                 FEATURE_CODE_REWARDING_PROGRAM,
                                                 FEATURE_CODE_REDEMPTION_PROGRAM,
                                                 FEATURE_CODE_LUCKY_DRAW_PROGRAM,
-                                                
+                                                FEATURE_CODE_REFERRAL_PROGRAM,
                                                 ],
                                        
                                        }
 
 PACKAGE_FEATURE_MEMBERSHIP_MAP = {
                                        LOYALTY_PACKAGE_LITE:[
                                                 FEATURE_CODE_BASIC_MEMBERSHIP,
@@ -193,20 +194,25 @@
 PROGRAM_STATUS_PROGRAM_BASE             = 'program_base'
 PROGRAM_STATUS_REWARD_SCHEME            = 'reward_scheme'
 PROGRAM_STATUS_REWARD_DETAILS           = 'reward_details'
 PROGRAM_STATUS_DEFINE_TIER              = 'define_program_tier'
 PROGRAM_STATUS_DEFINE_REWARD            = 'define_reward'
 PROGRAM_STATUS_DEFINE_CONDITION         = 'define_condition'
 PROGRAM_STATUS_UPLOAD_TICKET_IMAGE      = 'upload_material'
+PROGRAM_STATUS_UPLOAD_MATERIAL          = 'upload_material'
 PROGRAM_STATUS_DEFINE_PRIZE             = 'define_prize'
 PROGRAM_STATUS_DEFINE_PRIZE_POSSIBILITY = 'define_prize_possibility'
 PROGRAM_STATUS_EXCLUSIVITY              = 'exclusivity'
 PROGRAM_STATUS_REVIEW                   = 'review'
 PROGRAM_STATUS_PUBLISH                  = 'published'
 PROGRAM_STATUS_DEFINE_ITEM              = 'define_item'
+PROGRAM_STATUS_DEFINE_PROMOTE_TEXT      = 'define_promote_text'
+
+PROGRAM_STATUS_DEFINE_REFERRER_REWARD   = 'define_program_referrer_reward'
+PROGRAM_STATUS_DEFINE_REFEREE_REWARD    = 'define_program_referee_reward'
 
 ACTION_AFTER_UNLOCK_TIER_NO_ACTION          = 'no_action'
 ACTION_AFTER_UNLOCK_TIER_CONSUME_REWARD     = 'consume_reward'
 
 
 PROGRAM_REWARD_GIVEAWAY_METHOD_AUTO     = 'auto'
 PROGRAM_REWARD_GIVEAWAY_METHOD_MANUAL   = 'manual'
@@ -239,14 +245,22 @@
 BASIC_REWARD_PROGRAM_STATUS                          = [PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   PROGRAM_STATUS_REWARD_SCHEME, 
                                                                   PROGRAM_STATUS_EXCLUSIVITY,
                                                                   PROGRAM_STATUS_REVIEW,
                                                                   PROGRAM_STATUS_PUBLISH
                                                                   ]
 
+REFERRAL_REWARD_PROGRAM_STATUS                          = [PROGRAM_STATUS_PROGRAM_BASE, 
+                                                                  PROGRAM_STATUS_DEFINE_REFERRER_REWARD, 
+                                                                  PROGRAM_STATUS_DEFINE_REFEREE_REWARD,
+                                                                  PROGRAM_STATUS_REVIEW,
+                                                                  PROGRAM_STATUS_PUBLISH
+                                                                  ]
+
+
 LITE_BASIC_REWARD_PROGRAM_STATUS                     = [PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   PROGRAM_STATUS_REWARD_SCHEME, 
                                                                   PROGRAM_STATUS_REVIEW,
                                                                   PROGRAM_STATUS_PUBLISH
                                                                   ]
 
 TIER_REWARD_PROGRAM_STATUS                          = [PROGRAM_STATUS_PROGRAM_BASE, 
@@ -256,28 +270,37 @@
                                                                   PROGRAM_STATUS_REVIEW,
                                                                   PROGRAM_STATUS_PUBLISH,
                                                                   ]
 
 LUCKY_DRAW_PROGRAM_STATUS                          = [
                                                                   PROGRAM_STATUS_PROGRAM_BASE, 
                                                                   #PROGRAM_STATUS_DEFINE_CONDITION,
-                                                                  PROGRAM_STATUS_UPLOAD_TICKET_IMAGE,  
-                                                                  PROGRAM_STATUS_DEFINE_PRIZE,  
+                                                                  PROGRAM_STATUS_DEFINE_PRIZE,
                                                                   PROGRAM_STATUS_DEFINE_PRIZE_POSSIBILITY,
                                                                   PROGRAM_STATUS_EXCLUSIVITY,
+                                                                  PROGRAM_STATUS_UPLOAD_TICKET_IMAGE,  
+                                                                  PROGRAM_STATUS_PUBLISH,
+                                                                  ]
+
+REFERRAL_PROGRAM_STATUS                            = [PROGRAM_STATUS_PROGRAM_BASE, 
+                                                                  PROGRAM_STATUS_DEFINE_REFERRER_REWARD, 
+                                                                  PROGRAM_STATUS_DEFINE_REFEREE_REWARD,
+                                                                  #PROGRAM_STATUS_DEFINE_PROMOTE_TEXT,
+                                                                  #PROGRAM_STATUS_UPLOAD_MATERIAL,
+                                                                  #PROGRAM_STATUS_REVIEW,
                                                                   PROGRAM_STATUS_PUBLISH,
                                                                   ]
 
 ALL_PROGRAM_STATUS                            = (PROGRAM_STATUS_PROGRAM_BASE,
                                                  PROGRAM_STATUS_REWARD_SCHEME,
                                                  PROGRAM_STATUS_DEFINE_TIER,
                                                  PROGRAM_STATUS_DEFINE_REWARD,
                                                  PROGRAM_STATUS_EXCLUSIVITY,
                                                  PROGRAM_STATUS_REVIEW,
-                                                 PROGRAM_STATUS_PUBLISH
+                                                 PROGRAM_STATUS_PUBLISH,
                                                  )
 
 REDEMPTION_CATALOGUE_STATUS_DEFINED_CATALOGUE       = 'define_catalogue'
 REDEMPTION_CATALOGUE_STATUS_DEFINE_ITEM             = 'define_item'
 REDEMPTION_CATALOGUE_STATUS_UPLOAD_MATERIAL         = 'upload_material'
 REDEMPTION_CATALOGUE_STATUS_DEFINE_EXCLUSIVITY      = 'define_exclusivity'
 REDEMPTION_CATALOGUE_STATUS_REVIEW                  = 'review'
@@ -364,14 +387,15 @@
 
 
 REWARD_EXPIRATION_TYPE_SPECIFIC_DATE     = 'date'
 REWARD_EXPIRATION_TYPE_AFTER_YEAR        = 'year'
 REWARD_EXPIRATION_TYPE_AFTER_MONTH       = 'month'
 REWARD_EXPIRATION_TYPE_AFTER_WEEK        = 'week'
 REWARD_EXPIRATION_TYPE_AFTER_DAY         = 'day'
+REWARD_EXPIRATION_TYPE_END_OF_MONTH      = 'eom'
 
 FIRST_DAY_OF_MONTH                       = 'month_start'
 ON_DOB_DATE                              = 'dob_date'
 ADVANCE_IN_DAY                           = 'advance_in_day'
 
 REWARD_LIMIT_TYPE_NO_LIMIT                  = 'no_limit'
 REWARD_LIMIT_TYPE_BY_MONTH                  = 'limit_by_month'
@@ -447,23 +471,35 @@
 
 def get_lucky_draw_program_completed_status_index(completed_status):
     return LUCKY_DRAW_PROGRAM_STATUS.index(completed_status)
 
 def get_redemption_catalogue_completed_status_index(completed_status):
     return REDEMPTION_CATALOGUE_STATUS.index(completed_status)
 
+def get_referral_program_completed_status_index(completed_status):
+    return REFERRAL_PROGRAM_STATUS.index(completed_status)
+
 def is_program_current_status_reach(checking_status, completed_status):
     completed_status_index  = get_program_completed_status_index(completed_status)
     checking_status_index   = get_program_completed_status_index(checking_status)
     
     print('completed_status_index=%s'%completed_status_index)
     print('checking_status_index=%s'%checking_status_index)
     
     return checking_status_index<=completed_status_index+1
 
+def is_referral_program_current_status_reach(checking_status, completed_status):
+    completed_status_index  = get_referral_program_completed_status_index(completed_status)
+    checking_status_index   = get_referral_program_completed_status_index(checking_status)
+    
+    print('completed_status_index=%s'%completed_status_index)
+    print('checking_status_index=%s'%checking_status_index)
+    
+    return checking_status_index<=completed_status_index+1
+
 def is_voucher_current_status_reach(checking_status, completed_status):
     completed_status_index  = get_voucher_completed_status_index(completed_status)
     checking_status_index   = get_voucher_completed_status_index(checking_status)
     
     print('completed_status_index=%s'%completed_status_index)
     print('checking_status_index=%s'%checking_status_index)
     
@@ -490,14 +526,20 @@
 
 def is_valid_to_update_program_status(checking_status, completed_status):
     completed_status_index  = get_program_completed_status_index(completed_status)
     checking_status_index   = get_program_completed_status_index(checking_status)
     
     return checking_status_index<=completed_status_index+1
 
+def is_valid_to_update_referral_program_status(checking_status, completed_status):
+    completed_status_index  = get_referral_program_completed_status_index(completed_status)
+    checking_status_index   = get_referral_program_completed_status_index(checking_status)
+    
+    return checking_status_index<=completed_status_index+1
+
 def is_valid_to_update_voucher_status(checking_status, completed_status):
     completed_status_index  = get_voucher_completed_status_index(completed_status)
     checking_status_index   = get_voucher_completed_status_index(checking_status)
     
     return checking_status_index<=completed_status_index+1
 
 
@@ -520,14 +562,19 @@
     return checking_status_index<completed_status_index
 
 def is_existing_program_status_final_state(completed_status):
     completed_status_index  = get_program_completed_status_index(completed_status)
     
     return completed_status_index==len(BASIC_REWARD_PROGRAM_STATUS)-1
 
+def is_existing_referral_program_status_final_state(completed_status):
+    completed_status_index  = get_referral_program_completed_status_index(completed_status)
+    
+    return completed_status_index==len(BASIC_REWARD_PROGRAM_STATUS)-1
+
 def is_existing_tier_reward_program_status_final_state(completed_status):
     completed_status_index  = get_tier_reward_program_completed_status_index(completed_status)
     
     return completed_status_index==len(TIER_REWARD_PROGRAM_STATUS)-1
 
 def is_existing_voucher_status_final_state(completed_status):
     completed_status_index  = get_voucher_completed_status_index(completed_status)
@@ -555,7 +602,12 @@
 def redemption_catalogue_completed_progress_percentage(completed_status, loyalty_package):
     completed_status_index  = get_redemption_catalogue_completed_status_index(completed_status)
     print('redemption_catalogue_completed_progress_percentage: completed_status_index(%s)=%s'% (completed_status,completed_status_index))
     if loyalty_package == LOYALTY_PACKAGE_LITE:
         return int((completed_status_index+1)/len(LITE_REDEMPTION_CATALOGUE_STATUS) * 100)
     else:
         return int((completed_status_index+1)/len(REDEMPTION_CATALOGUE_STATUS) * 100)
+
+def referral_program_completed_progress_percentage(completed_status):
+    completed_status_index  = get_referral_program_completed_status_index(completed_status)
+    print('referral_program_completed_progress_percentage: completed_status_index(%s)=%s'% (completed_status,completed_status_index))
+    return int((completed_status_index+1)/len(REFERRAL_PROGRAM_STATUS) * 100)
```

### Comparing `trex-model-1.3.8/trexmodel/conf.py` & `trex-model-1.3.9/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/utils/model/model_util.py` & `trex-model-1.3.9/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/merchant_helpers.py` & `trex-model-1.3.9/trexmodel/models/merchant_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/loyalty_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/import_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/import_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/membership_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/membership_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/message_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/message_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/task_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/reward_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/reward_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.3.9/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/customer_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/customer_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/message_model_helper.py` & `trex-model-1.3.9/trexmodel/models/datastore/message_model_helper.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/coporate_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/reward_model_helpers.py` & `trex-model-1.3.9/trexmodel/models/datastore/reward_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/pos_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/pos_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/recruit_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/recruit_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/user_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/user_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/product_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/product_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/redemption_catalogue_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/redemption_catalogue_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     
     loyalty_package                    = ndb.StringProperty(required=False, default=program_conf.LOYALTY_PACKAGE_SCALE)
     
     dict_properties = [
                         "label","desc","completed_status","start_date","end_date","created_datetime",
                         "redeem_reward_format","catalogue_settings", "image_storage_filename", "image_public_url",
                         "exclusive_tags_list", "exclusive_memberships_list", "exclusive_tier_memberships_list",
-                        "completed_prograss_in_percentage","completed_status_index", "catalogue_items",
+                        "completed_progress_in_percentage","completed_status_index", "catalogue_items",
                         "is_enabled", "is_disabled", "is_archived", "is_published", "loyalty_package",
                         ]
     
     @property
     def is_enabled(self):
         return self.enabled
     
@@ -89,15 +89,15 @@
             return self.catalogue_settings.get('exclusivity').get('tier_memberships') or []
     
     @property
     def catalogue_items(self):
         return self.catalogue_settings.get('items') or []
     
     @property
-    def completed_prograss_in_percentage(self):
+    def completed_progress_in_percentage(self):
         return program_conf.redemption_catalogue_completed_progress_percentage(self.completed_status, self.loyalty_package)
     
     @property
     def completed_status_index(self):
         return program_conf.get_redemption_catalogue_completed_status_index(self.completed_status)
     
     @staticmethod
```

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/redeem_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/system_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/voucher_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/rating_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/rating_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/test_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/program_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/program_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,18 +248,19 @@
                 modified_by_username = modified_by.username
                 program.modified_by            = modified_by.create_ndb_key()
                 
         program.modified_by_username   = modified_by_username
         
         program.put()  
         
-        merchant_acct = program.merchant_acct
-        merchant_acct.remove_program_from_published_program_configuration(program.key_in_str)
-        
-        cls.__remove_schedule_program(program)
+        if program.is_published:
+            merchant_acct = program.merchant_acct
+            merchant_acct.remove_program_from_published_program_configuration(program.key_in_str)
+            
+            cls.__remove_schedule_program(program)
         
     def to_configuration(self):
         program_configuration = {
                                 'merchant_acct_key'                 : self.parent_key,
                                 'program_key'                       : self.key_in_str,
                                 'label'                             : self.label,
                                 'desc'                              : self.desc,
@@ -275,15 +276,15 @@
         
         return program_configuration
     
 
 class BasicRewardProgram(BaseProgram):
     
     @property
-    def completed_prograss_in_percentage(self):
+    def completed_progress_in_percentage(self):
         
         return program_conf.program_completed_progress_percentage(self.completed_status, self.loyalty_package)
     
     @property
     def completed_status_index(self):
         return program_conf.get_program_completed_status_index(self.completed_status)
     
@@ -556,15 +557,15 @@
         program.put()    
     
     
     
 class MerchantProgram(BasicRewardProgram):
     dict_properties                     = ['reward_base', 'giveaway_method', 'reward_format', 'completed_status', 'start_date', 'end_date', 'label','desc', 'program_settings', 
                                            'created_datetime', 'modified_datetime',  'enabled','completed_status','is_enabled', 'is_disabled', 'is_review_state', 
-                                           'is_published', 'archived', 'is_reward_amount_required', 'completed_prograss_in_percentage', 'completed_status_index',
+                                           'is_published', 'archived', 'is_reward_amount_required', 'completed_progress_in_percentage', 'completed_status_index',
                                            'exclusive_tags_list', 'exclusive_memberships_list', 'exclusive_tier_memberships_list',
                                            'is_recurring_scheme', 
                                            'expiration_type', 'expiration_date', 'expiration_value', 'is_expiration_date_type',
                                            'giveaway_reward_when', 'giveaway_reward_advance_in_day',
                                            'giveaway_system_condition', 'giveaway_system_condition_memberships_list', 'giveaway_system_condition_tier_memberships_list',
                                            'remarks', 'loyalty_package',
                                            'created_by_username', 'modified_by_username']
@@ -657,21 +658,21 @@
     
     is_tier_recycle                     = ndb.BooleanProperty(required=True, default=True)
     max_unlock_tier_count_per_trax      = ndb.IntegerProperty(required=False, default=999)
     is_show_progress                    = ndb.BooleanProperty(required=True, default=True)
     
     dict_properties                     = ['completed_status', 'start_date', 'end_date', 'label', 'desc', 'program_settings', 'reward_format',
                                            'created_datetime', 'modified_datetime',  'enabled','completed_status','is_enabled', 'is_disabled', 'is_review_state', 
-                                           'is_published', 'archived', 'completed_prograss_in_percentage', 'completed_status_index',
+                                           'is_published', 'archived', 'completed_progress_in_percentage', 'completed_status_index',
                                            'exclusive_tags_list', 'exclusive_memberships_list', 'exclusive_tier_memberships_list',
                                            'is_tier_recycle', 'is_show_progress', 'max_unlock_tier_count_per_trax',
                                            'created_by_username', 'modified_by_username', 'loyalty_package']
     
     @property
-    def completed_prograss_in_percentage(self):
+    def completed_progress_in_percentage(self):
         return program_conf.tier_reward_program_completed_progress_percentage(self.completed_status)
     
     @property
     def completed_status_index(self):
         return program_conf.get_tier_reward_program_completed_status_index(self.completed_status)
     
     @property
```

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.3.9/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/ndb_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/ndb_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/analytic_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/transaction_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/marketing_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/marketing_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/app_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/app_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.3.9/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/merchant_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,38 +63,40 @@
     timezone                                = ndb.StringProperty(required=False, default='Asia/Kuala_Lumpur')
     api_key                                 = ndb.StringProperty(required=False)
     
     account_plan                            = ndb.JsonProperty()
     outlet_count                            = ndb.IntegerProperty(default=0)
     
     published_program_configuration                 = ndb.JsonProperty()
+    published_referral_program_configuration        = ndb.JsonProperty()
     published_voucher_configuration                 = ndb.JsonProperty()
     published_redemption_catalogue_configuration    = ndb.JsonProperty()
     
     membership_configuration                        = ndb.JsonProperty()
     tier_membership_configuration                   = ndb.JsonProperty()
     
-    reward_naming_configuration             = ndb.JsonProperty()
+    reward_naming_configuration                     = ndb.JsonProperty()
     
-    prepaid_configuration                   = ndb.JsonProperty()
+    prepaid_configuration                           = ndb.JsonProperty()
     
-    lucky_draw_configuration                = ndb.JsonProperty(required=False)
+    lucky_draw_configuration                        = ndb.JsonProperty(required=False)
     
-    product_modifier_configuration          = ndb.JsonProperty()
+    product_modifier_configuration                  = ndb.JsonProperty()
     
-    program_settings                        = ndb.JsonProperty()
+    program_settings                                = ndb.JsonProperty()
     
-    stat_figure_update_interval_in_minutes  = conf.MERCHANT_STAT_FIGURE_UPDATE_INTERVAL_IN_MINUTES
-    stat_figure_update_datetime_format      = '%d-%m-%Y %H:%M:%S'
+    stat_figure_update_interval_in_minutes          = conf.MERCHANT_STAT_FIGURE_UPDATE_INTERVAL_IN_MINUTES
+    stat_figure_update_datetime_format              = '%d-%m-%Y %H:%M:%S'
     
     dict_properties = ['company_name', 'brand_name', 'contact_name', 'business_reg_no', 'mobile_phone', 
                        'office_phone', 'fax_phone', 'email', 'account_code', 'country',
                        'registered_datetime', 'modified_datetime', 'plan_start_date', 'plan_end_date', 'currency_code', 
                        'timezone',
-                       'published_program_configuration', 'published_voucher_configuration', 'membership_configuration', 
+                       'published_program_configuration', 'published_referral_program_configuration', 
+                       'published_voucher_configuration', 'membership_configuration', 
                        'tier_membership_configuration', 'prepaid_configuration', 'lucky_draw_configuration', 'product_modifier_configuration',
                        'dashboard_stat_figure', 'program_settings', 'is_tier_membership_configured', 'website', 
                        'product_package', 'loyalty_package','account_plan','outlet_count', 'outlet_limit',
                        'published_redemption_catalogue_configuration',
                        ]
     
     
@@ -209,24 +211,162 @@
         return 0
     
     @property
     def lucky_draw_ticket_image_url(self):
         if self.lucky_draw_configuration.get('settings'):
             return self.lucky_draw_configuration['settings']['ticket_image_url']
     
+    @property
+    def referrer_promote_title(self):
+        if is_not_empty(self.program_settings):
+            if self.program_settings.get('referral_program'):
+                return self.program_settings.get('referral_program').get('referrer_promote_title', '')
+        return ''
+        
+    @property
+    def referee_promote_title(self):
+        if is_not_empty(self.program_settings):
+            if self.program_settings.get('referral_program'):
+                return self.program_settings.get('referral_program').get('referee_promote_title', '')      
+        return ''
+        
+    @property
+    def referrer_promote_desc(self):
+        if is_not_empty(self.program_settings):
+            if self.program_settings.get('referral_program'):
+                return self.program_settings.get('referral_program').get('referrer_promote_desc', '')
+        return ''
+            
+    @property
+    def referee_promote_desc(self):
+        if is_not_empty(self.program_settings):
+            if self.program_settings.get('referral_program'):
+                return self.program_settings.get('referral_program').get('referee_promote_desc', '')            
+        return ''
+        
+    @property
+    def referrer_promote_image(self):
+        if is_not_empty(self.program_settings):
+            if self.program_settings.get('referral_program'):
+                return self.program_settings.get('referral_program').get('referrer_promote_image')
+            
+    @property
+    def referee_promote_image(self):
+        if is_not_empty(self.program_settings):
+            if self.program_settings.get('referral_program'):
+                return self.program_settings.get('referral_program').get('referee_promote_image')        
+        
+    
     @staticmethod
     def default_program_settings():
         return {
                 'days_of_return_policy'                 : 3,
                 'days_of_repeat_purchase_measurement'   : 7,
                 'membership_renew_advance_day'          : 7,
                 'membership_renew_late_day'             : 30,
                 
                 }
+    
+    def update_referrer_program_promote_text(self, 
+                                             promote_title=None, 
+                                             promote_desc=None,
+                                             modified_by=None):
+        modified_by_username = None
+        
+        if is_not_empty(modified_by):
+            if isinstance(modified_by, MerchantUser):
+                modified_by_username = modified_by.username
+        
+        if is_empty(self.program_settings):
+            self.program_settings = {
+                                    'referral_program':{}
+                                    }
+        else:
+            if is_empty(self.program_settings.get('referral_program')):
+                self.program_settings['referral_program'] = {}
+        
+        self.modified_by            = modified_by.create_ndb_key()
+        self.modified_by_username   = modified_by_username
+            
+        self.program_settings['referral_program']['referrer_promote_title'] =  promote_title
+        self.program_settings['referral_program']['referrer_promote_desc']  =  promote_desc
+        self.put() 
+        
+    def update_referee_program_promote_text(self, 
+                                             promote_title=None, 
+                                             promote_desc=None, 
+                                             modified_by=None):
+        modified_by_username = None
+        
+        if is_not_empty(modified_by):
+            if isinstance(modified_by, MerchantUser):
+                modified_by_username = modified_by.username
+        
+        if is_empty(self.program_settings):
+            self.program_settings = {
+                                    'referral_program':{}
+                                    }
+        else:
+            if is_empty(self.program_settings.get('referral_program')):
+                self.program_settings['referral_program'] = {}
+        
+        self.modified_by            = modified_by.create_ndb_key()
+        self.modified_by_username   = modified_by_username
+            
+        self.program_settings['referral_program']['referee_promote_title'] =  promote_title
+        self.program_settings['referral_program']['referee_promote_desc']  =  promote_desc
+        self.put()       
+        
+    def upload_referrer_program_promote_image(self, image_public_url=None, image_storage_filename=None, modified_by=None):
+        
+        modified_by_username = None
+        
+        if is_not_empty(modified_by):
+            if isinstance(modified_by, MerchantUser):
+                modified_by_username = modified_by.username
+        
+        if is_empty(self.program_settings):
+            self.program_settings = {
+                                    'referral_program':{}
+                                    }
+        else:
+            if is_empty(self.program_settings.get('referral_program')):
+                self.program_settings['referral_program'] = {}
+        
+        self.program_settings['referral_program']['referrer_promote_image']             = image_public_url
+        self.program_settings['referral_program']['referrer_promote_image_filename']    = image_storage_filename
+        
+        self.modified_by            = modified_by.create_ndb_key()
+        self.modified_by_username   = modified_by_username
+        
+        self.put()
+        
+    def upload_referee_program_promote_image(self, image_public_url=None, image_storage_filename=None, modified_by=None):
+        
+        modified_by_username = None
         
+        if is_not_empty(modified_by):
+            if isinstance(modified_by, MerchantUser):
+                modified_by_username = modified_by.username
+        
+        if is_empty(self.program_settings):
+            self.program_settings = {
+                                    'referral_program':{}
+                                    }
+        else:
+            if is_empty(self.program_settings.get('referral_program')):
+                self.program_settings['referral_program'] = {}
+        
+        self.program_settings['referral_program']['referee_promote_image']          = image_public_url
+        self.program_settings['referral_program']['referee_promote_image_filename'] = image_storage_filename
+        
+        self.modified_by            = modified_by.create_ndb_key()
+        self.modified_by_username   = modified_by_username
+        
+        self.put()        
     
     @staticmethod
     def update_details(merchant_acct, company_name=None, brand_name=None, business_reg_no=None, contact_name=None, 
                        email=None, mobile_phone=None, office_phone=None, currency_code=None,
                        country=None, timezone=None, website=None):
         
         
@@ -404,14 +544,40 @@
             existing_programs_list.append(program_configuration)
             
             self.published_program_configuration['programs']    = existing_programs_list
             self.published_program_configuration['count']       = len(existing_programs_list) 
             
         self.put()
         
+    def update_published_referral_program(self, program_configuration):
+        if is_empty(self.published_referral_program_configuration):
+            self.published_referral_program_configuration = {
+                                                'programs'  :[program_configuration],
+                                                'count'     : 1,
+                                                } 
+                                            
+        else:
+            self.flush_dirty_program_configuration()
+            existing_programs_list  = self.published_referral_program_configuration.get('programs')
+            
+            program_key = program_configuration.get('program_key')
+            index = 0
+            for p in existing_programs_list:
+                if p.get('program_key') == program_key:
+                    existing_programs_list.pop(index)
+                
+                index = index+1
+            
+            existing_programs_list.append(program_configuration)
+            
+            self.published_referral_program_configuration['programs']    = existing_programs_list
+            self.published_referral_program_configuration['count']       = len(existing_programs_list) 
+            
+        self.put()    
+        
     def add_voucher(self, voucher_configuration):
         if is_empty(self.published_voucher_configuration):
             self.published_voucher_configuration = {
                                                 'vouchers'  :[voucher_configuration],
                                                 'count'     : 1,
                                                 } 
                                             
@@ -674,14 +840,50 @@
         logger.debug('program_count after remove=%s', program_count)
         
         self.published_program_configuration['programs']    = existing_programs_list
         self.published_program_configuration['count']       = program_count
             
         self.put() 
         
+    def remove_program_from_published_referral_program_configuration(self, program_key_to_remove):
+        
+        logger.debug('remove_program_from_published_referral_program_configuration: program_key_to_remove=%s', program_key_to_remove)
+        
+        #self.flush_dirty_program_configuration()
+        existing_programs_list  = self.published_referral_program_configuration['programs']
+        program_count           = len(existing_programs_list)
+        
+        logger.debug('program_count before remove=%s', program_count)
+        
+        index = 0
+        
+        for program in existing_programs_list:
+            
+            logger.debug('program_key=%s', program.get('program_key'))
+            
+            is_same_program_key = program.get('program_key') == program_key_to_remove
+            
+            logger.debug('is_same_program_key=%s', is_same_program_key)
+            
+            if is_same_program_key:
+                existing_programs_list.pop(index)
+                
+                logger.debug('Found program to be remove')
+                
+            index = index+1
+        
+        program_count = len(existing_programs_list)
+        
+        logger.debug('program_count after remove=%s', program_count)
+        
+        self.published_referral_program_configuration['programs']    = existing_programs_list
+        self.published_referral_program_configuration['count']       = program_count
+            
+        self.put()     
+        
     
         
     def remove_redeption_catalogue(self, catalogue_key):
         existing_catalogues_list = self.published_redemption_catalogue_configuration['catalogues']
         
         new_catalogues_list = []
         for catalogue in existing_catalogues_list:
```

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/prepaid_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/lucky_draw_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/lucky_draw_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     image_storage_filename  = ndb.StringProperty(required=False)
     image_public_url        = ndb.StringProperty(required=False)
     
     dict_properties                     = ['label', 'desc', 'start_date', 'end_date', 'archived', 'is_recurring_scheme',
                                            'created_datetime', 'modified_datetime','archived_datetime', 'completed_status',
                                            'condition_settings', 'exclusivity_settings', 'prize_settings',
                                            'exclusive_tags_list', 'exclusive_memberships_list', 'exclusive_tier_memberships_list',  
-                                           'created_by_username', 'modified_by_username', 'completed_prograss_in_percentage',
+                                           'created_by_username', 'modified_by_username', 'completed_progress_in_percentage',
                                            'is_published', 'is_enabled','is_disabled', 'totalPrizePossibility',
-                                           'image_storage_filename', 'image_public_url', 'test_result', 
+                                           'image_storage_filename', 'image_public_url', 'test_result', 'is_expired',
                                            ]
     
     
     def to_configuration(self):
         program_configuration = {
                                 'merchant_acct_key'                 : self.parent_key,
                                 'program_key'                       : self.key_in_str,
@@ -92,14 +92,18 @@
         return self.enabled
     
     @property
     def is_disabled(self):
         return self.enabled==False
     
     @property
+    def is_expired(self):
+        return self.end_date<datetime.now().date()
+    
+    @property
     def is_archived(self):
         return self.archived
     
     @property
     def is_published(self):
         return self.completed_status == program_conf.PROGRAM_STATUS_PUBLISH
     
@@ -115,15 +119,15 @@
         
     @property
     def exclusive_tier_memberships_list(self):
         if self.exclusivity_settings and self.exclusivity_settings.get('tier_memberships'):
             return ','.join(self.exclusivity_settings.get('tier_memberships')) or ''
     
     @property
-    def completed_prograss_in_percentage(self):
+    def completed_progress_in_percentage(self):
         return program_conf.lucky_draw_program_completed_progress_percentage(self.completed_status)
     
     @property
     def is_recurring_scheme(self):
         if self.condition_settings:
             return self.condition_settings.get('is_recurring_scheme') or False
         return False
```

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/inventory_model.py` & `trex-model-1.3.9/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trexmodel/models/datastore/admin_models.py` & `trex-model-1.3.9/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/LICENSE` & `trex-model-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-1.3.8/trex_model.egg-info/SOURCES.txt` & `trex-model-1.3.9/trex_model.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 trexmodel/models/datastore/prepaid_models.py
 trexmodel/models/datastore/product_models.py
 trexmodel/models/datastore/program_models.py
 trexmodel/models/datastore/rating_models.py
 trexmodel/models/datastore/recruit_models.py
 trexmodel/models/datastore/redeem_models.py
 trexmodel/models/datastore/redemption_catalogue_models.py
+trexmodel/models/datastore/referral_program_model.py
 trexmodel/models/datastore/reward_model_helpers.py
 trexmodel/models/datastore/reward_models.py
 trexmodel/models/datastore/spending_base_program_model.py
 trexmodel/models/datastore/system_models.py
 trexmodel/models/datastore/task_models.py
 trexmodel/models/datastore/test_models.py
 trexmodel/models/datastore/transaction_models.py
```

### Comparing `trex-model-1.3.8/setup.py` & `trex-model-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='1.3.8',
+     version='1.3.9',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

