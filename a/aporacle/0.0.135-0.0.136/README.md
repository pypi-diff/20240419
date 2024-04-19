# Comparing `tmp/aporacle-0.0.135.tar.gz` & `tmp/aporacle-0.0.136.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporacle-0.0.135.tar", max compression
+gzip compressed data, was "aporacle-0.0.136.tar", max compression
```

## Comparing `aporacle-0.0.135.tar` & `aporacle-0.0.136.tar`

### file list

```diff
@@ -1,96 +1,26 @@
--rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.135/README.md
--rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.135/aporacle/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.135/aporacle/broadcast/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.135/aporacle/conf/__init__.py
--rw-r--r--   0        0        0      279 2024-03-20 16:45:48.324259 aporacle-0.0.135/aporacle/connectors/__init__.py
--rw-r--r--   0        0        0      113 2024-03-12 14:57:44.334437 aporacle-0.0.135/aporacle/connectors/evm_chain.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.924041 aporacle-0.0.135/aporacle/connectors/oracle/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.916041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.912041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/flare_system_manager/__init__.py
--rw-r--r--   0        0        0      658 2024-03-20 16:59:16.255639 aporacle-0.0.135/aporacle/connectors/oracle/contracts/flare_system_manager/flare_systems_manager_contract.py
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.895289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/flare_system_manager/flare_systems_manager_contract_abi.coston.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.903289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/flare_system_manager/flare_systems_manager_contract_abi.coston2.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.911289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/flare_system_manager/flare_systems_manager_contract_abi.flare.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.887289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/flare_system_manager/flare_systems_manager_contract_abi.songbird.json
--rw-r--r--   0        0        0     3497 2024-03-20 16:59:16.275639 aporacle-0.0.135/aporacle/connectors/oracle/contracts/flare_system_manager/flare_systems_manager_watcher.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.912041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_decimals/__init__.py
--rw-r--r--   0        0        0      659 2024-03-14 07:08:33.216905 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_decimals/ftso_feed_decimals_contract.py
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.895289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_decimals/ftso_feed_decimals_contract_abi.coston.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.903289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_decimals/ftso_feed_decimals_contract_abi.coston2.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.911289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_decimals/ftso_feed_decimals_contract_abi.flare.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.887289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_decimals/ftso_feed_decimals_contract_abi.songbird.json
--rw-r--r--   0        0        0     3834 2024-03-14 07:15:16.171822 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_decimals/ftso_feed_decimals_watcher.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.912041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_publisher/__init__.py
--rw-r--r--   0        0        0      750 2024-03-20 17:55:31.607772 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_publisher/ftso_feed_publisher_contract.py
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.895289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_publisher/ftso_feed_publisher_contract_abi.coston.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.903289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_publisher/ftso_feed_publisher_contract_abi.coston2.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.911289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_publisher/ftso_feed_publisher_contract_abi.flare.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.887289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_publisher/ftso_feed_publisher_contract_abi.songbird.json
--rw-r--r--   0        0        0     3764 2024-03-20 17:33:35.863356 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_feed_publisher/ftso_feed_publisher_watcher.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.912041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_inflation_configurations/__init__.py
--rw-r--r--   0        0        0      681 2024-03-14 07:01:38.248492 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_inflation_configurations/ftso_inflation_configurations_contract.py
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.895289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_inflation_configurations/ftso_inflation_configurations_contract_abi.coston.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.903289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_inflation_configurations/ftso_inflation_configurations_contract_abi.coston2.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.911289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_inflation_configurations/ftso_inflation_configurations_contract_abi.flare.json
--rw-r--r--   0        0        0    22067 2024-03-04 15:59:28.887289 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_inflation_configurations/ftso_inflation_configurations_contract_abi.songbird.json
--rw-r--r--   0        0        0     3867 2024-03-14 07:01:38.240492 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_inflation_configurations/ftso_inflation_configurations_watcher.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.912041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_reward_offers_manager/__init__.py
--rw-r--r--   0        0        0      660 2024-03-20 16:59:16.247639 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_reward_offers_manager/ftso_reward_offers_manager_contract.py
--rw-r--r--   0        0        0     8333 2024-03-14 06:36:52.007377 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_reward_offers_manager/ftso_reward_offers_manager_contract_abi.coston.json
--rw-r--r--   0        0        0     8333 2024-03-14 06:36:52.023377 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_reward_offers_manager/ftso_reward_offers_manager_contract_abi.coston2.json
--rw-r--r--   0        0        0     8333 2024-03-14 06:36:52.015377 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_reward_offers_manager/ftso_reward_offers_manager_contract_abi.flare.json
--rw-r--r--   0        0        0     8333 2024-03-14 06:36:52.011377 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_reward_offers_manager/ftso_reward_offers_manager_contract_abi.songbird.json
--rw-r--r--   0        0        0     3860 2024-03-20 16:59:16.263639 aporacle-0.0.135/aporacle/connectors/oracle/contracts/ftso_reward_offers_manager/ftso_reward_offers_manager_watcher.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.912041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/relay/__init__.py
--rw-r--r--   0        0        0      635 2024-03-14 07:16:47.885312 aporacle-0.0.135/aporacle/connectors/oracle/contracts/relay/relay_contract.py
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.974591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/relay/relay_contract_abi.coston.json
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.958591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/relay/relay_contract_abi.coston2.json
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.966591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/relay/relay_contract_abi.flare.json
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.982591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/relay/relay_contract_abi.songbird.json
--rw-r--r--   0        0        0     3823 2024-03-14 07:16:47.797311 aporacle-0.0.135/aporacle/connectors/oracle/contracts/relay/relay_watcher.py
--rw-r--r--   0        0        0        0 2024-03-02 14:39:29.912041 aporacle-0.0.135/aporacle/connectors/oracle/contracts/submission/__init__.py
--rw-r--r--   0        0        0      645 2024-03-13 05:05:56.964219 aporacle-0.0.135/aporacle/connectors/oracle/contracts/submission/submission_contract.py
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.974591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/submission/submission_contract_abi.coston.json
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.958591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/submission/submission_contract_abi.coston2.json
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.966591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/submission/submission_contract_abi.flare.json
--rw-r--r--   0        0        0     6501 2024-03-04 16:51:08.982591 aporacle-0.0.135/aporacle/connectors/oracle/contracts/submission/submission_contract_abi.songbird.json
--rw-r--r--   0        0        0     4064 2024-03-15 17:56:38.466252 aporacle-0.0.135/aporacle/connectors/oracle/contracts/submission/submission_watcher.py
--rw-r--r--   0        0        0     2513 2024-03-20 16:59:16.155638 aporacle-0.0.135/aporacle/connectors/oracle/contracts/tso_contract_base.py
--rw-r--r--   0        0        0     4799 2024-03-12 18:37:33.073939 aporacle-0.0.135/aporacle/connectors/oracle/oracle_wallet.py
--rw-r--r--   0        0        0        0 2024-02-05 13:16:28.308617 aporacle-0.0.135/aporacle/connectors/rpc/__init__.py
--rw-r--r--   0        0        0        0 2024-01-24 12:48:57.904850 aporacle-0.0.135/aporacle/connectors/rpc/flarepy/__init__.py
--rw-r--r--   0        0        0        0 2024-02-08 08:20:45.544302 aporacle-0.0.135/aporacle/connectors/rpc/flarepy/api/__init__.py
--rw-r--r--   0        0        0    43477 2024-01-24 13:21:09.144003 aporacle-0.0.135/aporacle/connectors/rpc/flarepy/api/apimeta.py
--rw-r--r--   0        0        0      353 2024-02-08 08:19:46.495663 aporacle-0.0.135/aporacle/connectors/rpc/flarepy/api/flareconfig.py
--rw-r--r--   0        0        0     1785 2024-03-20 16:30:40.435366 aporacle-0.0.135/aporacle/connectors/rpc/flarepy/api/flarerpc.py
--rw-r--r--   0        0        0      179 2024-03-20 16:30:40.427366 aporacle-0.0.135/aporacle/connectors/rpc/flarepy/api/health.py
--rw-r--r--   0        0        0      331 2024-03-20 16:30:40.419366 aporacle-0.0.135/aporacle/connectors/rpc/flarepy/api/platform.py
--rw-r--r--   0        0        0      787 2024-03-12 14:57:44.350437 aporacle-0.0.135/aporacle/connectors/wallet_base.py
--rw-r--r--   0        0        0      507 2024-03-21 17:41:59.128025 aporacle-0.0.135/aporacle/connectors/watcher/__init__.py
--rw-r--r--   0        0        0      949 2024-03-20 16:45:48.312259 aporacle-0.0.135/aporacle/connectors/watcher/base_watcher.py
--rw-r--r--   0        0        0     5585 2024-03-20 16:45:48.344259 aporacle-0.0.135/aporacle/connectors/watcher/contract_event_logs.py
--rw-r--r--   0        0        0     8426 2024-03-20 16:45:48.352259 aporacle-0.0.135/aporacle/connectors/watcher/websocket_watcher.py
--rw-r--r--   0        0        0     1922 2024-03-20 17:10:58.230130 aporacle-0.0.135/aporacle/connectors/web3_wallet.py
--rw-r--r--   0        0        0     5796 2024-03-20 16:41:05.665563 aporacle-0.0.135/aporacle/connectors/web3_wallet_backend.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.135/aporacle/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.135/aporacle/core/utils/__init__.py
--rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.135/aporacle/core/utils/async_call_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.135/aporacle/data/__init__.py
--rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.135/aporacle/data/asset/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-25 05:26:42.304279 aporacle-0.0.135/aporacle/data/combination.py
--rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.135/aporacle/data/db/__init__.py
--rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.135/aporacle/data/db/crud.py
--rw-r--r--   0        0        0    10174 2024-03-22 09:49:57.935682 aporacle-0.0.135/aporacle/data/gcp/__init__.py
--rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.135/aporacle/data/symbols/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.135/aporacle/execution/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-27 10:53:43.099151 aporacle-0.0.135/aporacle/execution/executables.py
--rw-r--r--   0        0        0        0 2024-03-10 10:09:16.424282 aporacle-0.0.135/aporacle/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 10:09:56.392617 aporacle-0.0.135/aporacle/ml/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 10:09:40.520484 aporacle-0.0.135/aporacle/ml/train/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 10:41:27.060572 aporacle-0.0.135/aporacle/ml/train/base/__init__.py
--rw-r--r--   0        0        0     4327 2024-03-25 03:23:22.081532 aporacle-0.0.135/aporacle/ml/train/base/training_runner.py
--rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.135/aporacle/network/__init__.py
--rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.135/aporacle/network/network_base.py
--rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.135/aporacle/shared_setup.py
--rw-r--r--   0        0        0      531 2024-04-19 05:10:06.899603 aporacle-0.0.135/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 aporacle-0.0.135/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.136/README.md
+-rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.136/aporacle/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.136/aporacle/broadcast/__init__.py
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.136/aporacle/conf/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.136/aporacle/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.136/aporacle/core/utils/__init__.py
+-rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.136/aporacle/core/utils/async_call_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.136/aporacle/data/__init__.py
+-rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.136/aporacle/data/asset/__init__.py
+-rw-r--r--   0        0        0     1459 2024-03-25 05:26:42.304279 aporacle-0.0.136/aporacle/data/combination.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.136/aporacle/data/db/__init__.py
+-rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.136/aporacle/data/db/crud.py
+-rw-r--r--   0        0        0    10174 2024-03-22 09:49:57.935682 aporacle-0.0.136/aporacle/data/gcp/__init__.py
+-rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.136/aporacle/data/symbols/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.136/aporacle/execution/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-27 10:53:43.099151 aporacle-0.0.136/aporacle/execution/executables.py
+-rw-r--r--   0        0        0        0 2024-03-10 10:09:16.424282 aporacle-0.0.136/aporacle/ml/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-10 10:09:56.392617 aporacle-0.0.136/aporacle/ml/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-10 10:09:40.520484 aporacle-0.0.136/aporacle/ml/train/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-10 10:41:27.060572 aporacle-0.0.136/aporacle/ml/train/base/__init__.py
+-rw-r--r--   0        0        0     4327 2024-03-25 03:23:22.081532 aporacle-0.0.136/aporacle/ml/train/base/training_runner.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.136/aporacle/network/__init__.py
+-rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.136/aporacle/network/network_base.py
+-rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.136/aporacle/shared_setup.py
+-rw-r--r--   0        0        0      447 2024-04-19 05:22:52.676114 aporacle-0.0.136/pyproject.toml
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 aporacle-0.0.136/PKG-INFO
```

### Comparing `aporacle-0.0.135/aporacle/broadcast/__init__.py` & `aporacle-0.0.136/aporacle/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/conf/__init__.py` & `aporacle-0.0.136/aporacle/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/core/utils/async_call_scheduler.py` & `aporacle-0.0.136/aporacle/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/data/asset/__init__.py` & `aporacle-0.0.136/aporacle/data/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/data/combination.py` & `aporacle-0.0.136/aporacle/data/combination.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/data/db/crud.py` & `aporacle-0.0.136/aporacle/data/db/crud.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/data/gcp/__init__.py` & `aporacle-0.0.136/aporacle/data/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/data/symbols/__init__.py` & `aporacle-0.0.136/aporacle/data/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/execution/executables.py` & `aporacle-0.0.136/aporacle/execution/executables.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/ml/train/base/training_runner.py` & `aporacle-0.0.136/aporacle/ml/train/base/training_runner.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/network/network_base.py` & `aporacle-0.0.136/aporacle/network/network_base.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/aporacle/shared_setup.py` & `aporacle-0.0.136/aporacle/shared_setup.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.135/PKG-INFO` & `aporacle-0.0.136/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: aporacle
-Version: 0.0.135
+Version: 0.0.136
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cachetools (>=5.3.3,<6.0.0)
-Requires-Dist: eth-abi (>=5.0.1,<6.0.0)
-Requires-Dist: eth-bloom (>=3.0.0,<4.0.0)
-Requires-Dist: eth-utils (>=4.0.0,<5.0.0)
 Requires-Dist: google-cloud-storage (>=2.16.0,<3.0.0)
 Requires-Dist: komoutils (>=0.0.224,<0.0.225)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
-Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
-Requires-Dist: statsmodels (>=0.14.1,<0.15.0)
-Requires-Dist: web3 (>=6.15.1,<7.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
 Description-Content-Type: text/markdown
```

