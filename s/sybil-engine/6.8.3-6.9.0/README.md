# Comparing `tmp/sybil_engine-6.8.3.tar.gz` & `tmp/sybil_engine-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil_engine-6.8.3.tar", last modified: Thu Apr 18 09:45:52 2024, max compression
+gzip compressed data, was "sybil_engine-6.9.0.tar", last modified: Thu Apr 18 13:07:23 2024, max compression
```

## Comparing `sybil_engine-6.8.3.tar` & `sybil_engine-6.9.0.tar`

### file list

```diff
@@ -1,105 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.528240 sybil_engine-6.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-18 09:45:52.528240 sybil_engine-6.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:45:52.528240 sybil_engine-6.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.512240 sybil_engine-6.8.3/sybil_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.512240 sybil_engine-6.8.3/sybil_engine/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/config/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.516240 sybil_engine-6.8.3/sybil_engine/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/contract/erc20_test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/contract/erc20contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/contract/send.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/contract/transaction_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/contract/weth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.516240 sybil_engine-6.8.3/sybil_engine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/data/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/data/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/data/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/data/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/data/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.516240 sybil_engine-6.8.3/sybil_engine/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/account_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.516240 sybil_engine-6.8.3/sybil_engine/domain/balance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/balance/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/balance/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/dex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/domain/generic_swap_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.516240 sybil_engine-6.8.3/sybil_engine/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/module/execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/module/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/module/module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/module/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.520240 sybil_engine-6.8.3/sybil_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/app_account_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/arguments_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/binance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/cex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/configuration_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/fee_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/gas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/google_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/l0_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/okx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/scal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/validation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/wallet_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/sybil_engine/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.524240 sybil_engine-6.8.3/sybil_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-18 09:45:52.000000 sybil_engine-6.8.3/sybil_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-18 09:45:52.000000 sybil_engine-6.8.3/sybil_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:45:52.000000 sybil_engine-6.8.3/sybil_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-18 09:45:52.000000 sybil_engine-6.8.3/sybil_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 09:45:52.000000 sybil_engine-6.8.3/sybil_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.520240 sybil_engine-6.8.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.524240 sybil_engine-6.8.3/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/data/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/data/test_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.524240 sybil_engine-6.8.3/test/module/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.524240 sybil_engine-6.8.3/test/module/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/contract/mock_router.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/mock_fail_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/mock_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/mock_not_enoguth_native_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/repeatable_mock_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.524240 sybil_engine-6.8.3/test/module/swap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/swap/mock_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/swap/mock_test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/swap/test_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/swap/test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/test_execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/test_module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/module/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:52.524240 sybil_engine-6.8.3/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/utils/test_binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/utils/test_create_app_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-18 09:45:48.000000 sybil_engine-6.8.3/test/utils/test_validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.866283 sybil_engine-6.9.0/sybil_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.866283 sybil_engine-6.9.0/sybil_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/config/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.870283 sybil_engine-6.9.0/sybil_engine/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/contract/erc20_test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/contract/erc20contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/contract/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/contract/transaction_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/contract/weth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.870283 sybil_engine-6.9.0/sybil_engine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/data/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/data/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/data/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/data/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/data/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.870283 sybil_engine-6.9.0/sybil_engine/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/account_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.870283 sybil_engine-6.9.0/sybil_engine/domain/balance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/balance/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/balance/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/domain/generic_swap_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.870283 sybil_engine-6.9.0/sybil_engine/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/module/execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/module/module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/module/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.874283 sybil_engine-6.9.0/sybil_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/app_account_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/arguments_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/binance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/cex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/configuration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/fee_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/gas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/l0_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/okx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/scan_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/validation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/wallet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/sybil_engine/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/sybil_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-18 13:07:23.000000 sybil_engine-6.9.0/sybil_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-18 13:07:23.000000 sybil_engine-6.9.0/sybil_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:07:23.000000 sybil_engine-6.9.0/sybil_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-18 13:07:23.000000 sybil_engine-6.9.0/sybil_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 13:07:23.000000 sybil_engine-6.9.0/sybil_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.874283 sybil_engine-6.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.874283 sybil_engine-6.9.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/data/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/data/test_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/test/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/test/module/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/contract/mock_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/mock_fail_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/mock_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/mock_not_enoguth_native_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/repeatable_mock_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/test/module/swap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/swap/mock_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/swap/mock_test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/swap/test_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/swap/test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/test_execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/test_module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/module/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:23.878283 sybil_engine-6.9.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/utils/test_create_app_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 13:07:19.000000 sybil_engine-6.9.0/test/utils/test_validation_utils.py
```

### Comparing `sybil_engine-6.8.3/PKG-INFO` & `sybil_engine-6.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.8.3
+Version: 6.9.0
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.5.1
@@ -18,14 +18,16 @@
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: bumpversion==0.6.0
 Requires-Dist: binance-connector==3.6.0
 Requires-Dist: base58==2.1.1
 Requires-Dist: google-api-python-client==2.126.0
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
+Requires-Dist: eth-tester==0.10.0b4
+Requires-Dist: py-evm==0.10.0b6
 
 # Sybil Engine
 
 ## Introduction
 Sybil Engine is a powerful Python library designed for testing web3 contracts. It facilitates seamless interactions with blockchain networks and smart contracts, providing developers with efficient tools to execute, plan, and manage web3 transactions.
 
 ## Key Features
```

### Comparing `sybil_engine-6.8.3/README.md` & `sybil_engine-6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/setup.py` & `sybil_engine-6.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = file.readlines()
 
 setup(
     name='sybil_engine',
-    version='6.8.3',
+    version='6.9.0',
     py_modules=['sybil_engine'],
     packages=find_packages(),
     install_requires=requirements,
     data_files=[('', ['requirements.txt'])],
     author='Indeoo',
     author_email='indeooars@gmail.com',
     description='Engine for web3 smart contracts automatization.',
```

### Comparing `sybil_engine-6.8.3/sybil_engine/app.py` & `sybil_engine-6.9.0/sybil_engine/app.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/config/app_config.py` & `sybil_engine-6.9.0/sybil_engine/config/app_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/contract/contract.py` & `sybil_engine-6.9.0/sybil_engine/contract/contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/contract/erc20_test_contract.py` & `sybil_engine-6.9.0/sybil_engine/contract/erc20_test_contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/contract/erc20contract.py` & `sybil_engine-6.9.0/sybil_engine/contract/erc20contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/contract/send.py` & `sybil_engine-6.9.0/sybil_engine/contract/send.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/contract/transaction_executor.py` & `sybil_engine-6.9.0/sybil_engine/contract/transaction_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/contract/weth.py` & `sybil_engine-6.9.0/sybil_engine/contract/weth.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/data/contracts.py` & `sybil_engine-6.9.0/sybil_engine/data/contracts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/data/networks.py` & `sybil_engine-6.9.0/sybil_engine/data/networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/data/pairs.py` & `sybil_engine-6.9.0/sybil_engine/data/pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/data/tokens.py` & `sybil_engine-6.9.0/sybil_engine/data/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/domain/balance/balance.py` & `sybil_engine-6.9.0/sybil_engine/domain/balance/balance.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/domain/balance/balance_utils.py` & `sybil_engine-6.9.0/sybil_engine/domain/balance/balance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/domain/balance/tokens.py` & `sybil_engine-6.9.0/sybil_engine/domain/balance/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/domain/dex.py` & `sybil_engine-6.9.0/sybil_engine/domain/dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/domain/generic_swap_facade.py` & `sybil_engine-6.9.0/sybil_engine/domain/generic_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/module/execution_planner.py` & `sybil_engine-6.9.0/sybil_engine/module/execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/module/module.py` & `sybil_engine-6.9.0/sybil_engine/module/module.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/module/module_executor.py` & `sybil_engine-6.9.0/sybil_engine/module/module_executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from loguru import logger
 from sybil_engine.data.contracts import get_contracts_for_chain
 
 from sybil_engine.data.networks import get_chain_instance
 
 from sybil_engine.utils.accumulator import add_accumulator_str, remove_accumulator_str
-from sybil_engine.utils.scal_utils import find_interacted_contracts
+from sybil_engine.utils.scan_utils import find_interacted_contracts
 from sybil_engine.utils.utils import randomized_sleeping, ModuleException, print_exception_chain, \
     ConfigurationException, RetryException
 
 
 class ModuleExecutor:
     def execute_modules(self, modules, account, sleep_interval):
         try:
@@ -22,20 +22,22 @@
             logger.error(f'Error, skip {account}:')
             print_exception_chain(e)
             add_accumulator_str("Failed accounts: ", account)
 
     def execute_module(self, module_args, account, module, sleep_interval):
         try:
             args = list(module_args.keys())
-            if 'unique' in args and 'chain' in args and 'api_key' in args and module_args['unique']:
+            if 'unique' in args and 'chain' in args and module_args['unique']:
                 chain = module_args['chain']
+                chain_instance = get_chain_instance(chain)
+
                 interactions = find_interacted_contracts(
                     account.address,
-                    get_chain_instance(chain)['scan_api'],
-                    module_args['api_key']
+                    chain_instance['api_scan'],
+                    chain_instance['api_scan_key']
                 )
 
                 if 'contract' in args:
                     contract_address = module_args['contract']
                 elif module.module_name == 'SEND_TO_CEX':
                     contract_address = account.cex_address
                 else:
```

### Comparing `sybil_engine-6.8.3/sybil_engine/module/modules.py` & `sybil_engine-6.9.0/sybil_engine/module/modules.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/accumulator.py` & `sybil_engine-6.9.0/sybil_engine/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/app_account_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/app_account_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
         app_accounts = app_accounts + [AppAccount(index, proxy, account, cex_address, starknet_address)]
 
     logger.info(f"Loaded {len(app_accounts)} accounts")
     random.shuffle(app_accounts)
 
     return app_accounts
 
+
 def validate_cex_addresses(app_accounts, cex_addresses):
     missing_addresses_accounts = []
 
     for account in app_accounts:
         if account.cex_address not in cex_addresses:
             missing_addresses_accounts.append(account)
 
@@ -178,15 +179,15 @@
         for missing_addresses_account in missing_addresses_accounts:
             error_log += f"{missing_addresses_account} has wrong CEX {missing_addresses_account.cex_address}. "
 
         raise Exception({error_log})
 
 
 class AppAccount(Account):
-    def __init__(self, app_id, proxy, account, cex_address, starknet_address, notes):
+    def __init__(self, app_id, proxy, account, cex_address, starknet_address, notes=None):
         self.app_id = app_id
         self.proxy = proxy
         self.address = account.address
         self.key = account.key
         self.cex_address = cex_address
         self.starknet_address = starknet_address
         self.notes = notes
```

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/arguments_parser.py` & `sybil_engine-6.9.0/sybil_engine/utils/arguments_parser.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/binance_prices.py` & `sybil_engine-6.9.0/sybil_engine/utils/binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/binance_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/binance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/configuration_loader.py` & `sybil_engine-6.9.0/sybil_engine/utils/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/decryptor.py` & `sybil_engine-6.9.0/sybil_engine/utils/decryptor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/fee_storage.py` & `sybil_engine-6.9.0/sybil_engine/utils/fee_storage.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/gas_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/gas_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/google_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/logs.py` & `sybil_engine-6.9.0/sybil_engine/utils/logs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/okx_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/okx_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/retry.py` & `sybil_engine-6.9.0/sybil_engine/utils/retry.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/scal_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/scan_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/telegram.py` & `sybil_engine-6.9.0/sybil_engine/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/validation_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine/utils/web3_utils.py` & `sybil_engine-6.9.0/sybil_engine/utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/sybil_engine.egg-info/PKG-INFO` & `sybil_engine-6.9.0/sybil_engine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.8.3
+Version: 6.9.0
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.5.1
@@ -18,14 +18,16 @@
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: bumpversion==0.6.0
 Requires-Dist: binance-connector==3.6.0
 Requires-Dist: base58==2.1.1
 Requires-Dist: google-api-python-client==2.126.0
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
+Requires-Dist: eth-tester==0.10.0b4
+Requires-Dist: py-evm==0.10.0b6
 
 # Sybil Engine
 
 ## Introduction
 Sybil Engine is a powerful Python library designed for testing web3 contracts. It facilitates seamless interactions with blockchain networks and smart contracts, providing developers with efficient tools to execute, plan, and manage web3 transactions.
 
 ## Key Features
```

### Comparing `sybil_engine-6.8.3/sybil_engine.egg-info/SOURCES.txt` & `sybil_engine-6.9.0/sybil_engine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 sybil_engine/utils/file_loader.py
 sybil_engine/utils/gas_utils.py
 sybil_engine/utils/google_utils.py
 sybil_engine/utils/l0_utils.py
 sybil_engine/utils/logs.py
 sybil_engine/utils/okx_utils.py
 sybil_engine/utils/retry.py
-sybil_engine/utils/scal_utils.py
+sybil_engine/utils/scan_utils.py
 sybil_engine/utils/telegram.py
 sybil_engine/utils/utils.py
 sybil_engine/utils/validation_utils.py
 sybil_engine/utils/wallet_loader.py
 sybil_engine/utils/web3_utils.py
 test/__init__.py
 test/test_config.py
@@ -77,11 +77,10 @@
 test/module/contract/mock_router.py
 test/module/swap/__init__.py
 test/module/swap/mock_dex.py
 test/module/swap/mock_test_swap_facade.py
 test/module/swap/test_dex.py
 test/module/swap/test_swap_facade.py
 test/utils/__init__.py
-test/utils/test_binance_prices.py
 test/utils/test_create_app_accounts.py
 test/utils/test_utils.py
 test/utils/test_validation_utils.py
```

### Comparing `sybil_engine-6.8.3/test/__init__.py` & `sybil_engine-6.9.0/test/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,37 @@
 import importlib
 import pkgutil
 
 from sybil_engine.config.app_config import set_network, set_dex_retry_interval, set_gas_prices
 from sybil_engine.domain.balance.balance_utils import interval_to_eth_balance
 from sybil_engine.utils.app_account_utils import create_app_account_with_proxies
 
-zksync_test_account = create_app_account_with_proxies(
-    ['0xb98308D11E2B578858Fbe65b793e71C7a0CAa43e'],
-    False,
-    'password',
-    ['0x7726827caac94a7f9e1b160f7ea819f172f7b6f9d2a97f992c38edeab82d4110'],
-    [],
-    'RANDOM',
-    ['0x6317842385f344acf68561f4e65f0f39e4fb4f1ad104b92bd007361aed39d8'],
-)[0]
-
-zksync_min_native_balance = interval_to_eth_balance({'from': 1, 'to': 1}, zksync_test_account, None, None)
 
-base_test_account = create_app_account_with_proxies(
+test_account = create_app_account_with_proxies(
     ['0xb98308D11E2B578858Fbe65b793e71C7a0CAa43e'],
     False,
     'password',
     ['0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80'],
     [],
     'RANDOM',
     ['0x6317842385f344acf68561f4e65f0f39e4fb4f1ad104b92bd007361aed39d8'],
 )[0]
 
-base_min_native_balance = interval_to_eth_balance({'from': 1, 'to': 1}, base_test_account, None, None)
+min_native_balance = interval_to_eth_balance({'from': 1, 'to': 1}, test_account, None, None)
 
 global_vars = globals()
 
 for loader, module_name, is_pkg in pkgutil.iter_modules(['core/contract']):
     module = importlib.import_module('.' + module_name, package='core.contract')
     global_vars[module_name] = module
 
 
 gas_prices_gwei_test = {
     'ETH_MAINNET': 100,
-    'ZKSYNC': 0.26,
-    'BASE': 0.5,
-    'LINEA': 2,
-    'ARBITRUM': 0.2,
-    'AVALANCHE': 26,
-    'BSC': 5,
-    'FANTOM': 750,
-    'OPTIMISM': 0.5,
-    'POLYGON': 150
+    'MOCK_CHAIN': 100
 }
 
 
 def init_set_test_config():
     set_network('LOCAL')
     set_dex_retry_interval({'from': 0, 'to': 0})
     set_gas_prices(gas_prices_gwei_test)
```

### Comparing `sybil_engine-6.8.3/test/data/test_networks.py` & `sybil_engine-6.9.0/test/data/test_networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/test/data/test_pairs.py` & `sybil_engine-6.9.0/test/data/test_pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/test/module/contract/mock_router.py` & `sybil_engine-6.9.0/test/module/contract/mock_router.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/test/module/swap/mock_dex.py` & `sybil_engine-6.9.0/test/module/swap/mock_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/test/module/swap/mock_test_swap_facade.py` & `sybil_engine-6.9.0/test/module/swap/mock_test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.8.3/test/module/swap/test_dex.py` & `sybil_engine-6.9.0/test/module/swap/test_dex.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import unittest
 
+from eth_tester import EthereumTester, PyEVMBackend
+from eth_utils import to_wei
+from web3 import Web3, EthereumTesterProvider
 from sybil_engine.data.networks import get_chain_instance
 from sybil_engine.domain.balance.balance import NativeBalance
 from sybil_engine.domain.balance.balance_utils import from_eth_to_wei
 from sybil_engine.utils.utils import SwapException
-from sybil_engine.utils.web3_utils import init_web3
-from test import zksync_test_account, init_set_test_config, base_test_account
+from test import init_set_test_config, test_account
 from test.module.swap.mock_dex import MockFailDex
+from test.test_config import setup_mock_eth_provider
 
 
 class TestDex(unittest.TestCase):
     init_set_test_config()
 
-    def test_succeed_after_3_retries(self, chain='LINEA'):
+    def test_succeed_after_3_retries(self, chain='MOCK_CHAIN'):
         chain_instance = get_chain_instance(chain)
-        web3 = init_web3(chain_instance, None)
+
+        web3 = Web3(setup_mock_eth_provider())
+
         from_token = 'ETH'
         to_token = 'USDC'
         slippage = 0.99
         amount_to_swap = NativeBalance(from_eth_to_wei(1), chain, 'ETH')
 
         test_dex = MockFailDex(chain_instance, web3, 2, {'from': 0, 'to': 0})
 
-        test_dex.swap_with_retry(amount_to_swap, from_token, to_token, slippage, base_test_account)
+        test_dex.swap_with_retry(amount_to_swap, from_token, to_token, slippage, test_account)
 
-    def test_fail_after_3_retries(self, chain='LINEA'):
+    def test_fail_after_3_retries(self, chain='MOCK_CHAIN'):
         chain_instance = get_chain_instance(chain)
-        web3 = init_web3(chain_instance, None)
+
+        web3 = Web3(setup_mock_eth_provider())
+
         from_token = 'ETH'
         to_token = 'USDC'
         slippage = 0.99
         amount_to_swap = NativeBalance(from_eth_to_wei(1), chain, 'ETH')
 
         test_dex = MockFailDex(chain_instance, web3, 3, {'from': 0, 'to': 0})
 
         with self.assertRaises(SwapException):
-            test_dex.swap_with_retry(amount_to_swap, from_token, to_token, slippage, zksync_test_account)
+            test_dex.swap_with_retry(amount_to_swap, from_token, to_token, slippage, test_account)
```

### Comparing `sybil_engine-6.8.3/test/module/swap/test_swap_facade.py` & `sybil_engine-6.9.0/test/module/swap/test_swap_facade.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 class TestSwapFacade(unittest.TestCase):
     init_set_test_config()
 
     def test_shouldGetDex(self):
         logger.info("Test swap facade")
 
-        dex_apps = swap_facade.get_swap_apps_by_chain('BASE')
-        chain_instance = get_chain_instance('BASE')
-        pairs = Pairs(swap_facade).get_pairs_by_tokens('ETH', 'USDC', 'ZKSYNC')
+        dex_apps = swap_facade.get_swap_apps_by_chain('MOCK_CHAIN')
+        chain_instance = get_chain_instance('MOCK_CHAIN')
+        pairs = Pairs(swap_facade).get_pairs_by_tokens('ETH', 'USDC', 'MOCK_CHAIN')
         web3 = init_web3(chain_instance, None)
 
         try:
             for swap_app in dex_apps:
                 for pair in pairs:
                     print(swap_facade.get_dex(pair, swap_app, chain_instance, web3))
         except Exception as e:
```

### Comparing `sybil_engine-6.8.3/test/module/test_execution_planner.py` & `sybil_engine-6.9.0/test/module/test_execution_planner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
 from sybil_engine.module.execution_planner import create_execution_plans
-from test import zksync_test_account
+from test import test_account
 from test.test_config import create_config
 
 mock_scenario = {
     'scenario_name': 'TEST_module_0_config',
     'scenario': [
         {
             'module': 'MockModule',
@@ -26,27 +26,27 @@
         }
     ]
 }
 
 
 class TestExecutionPlanner(unittest.TestCase):
 
-    def test_should_form_execution_planner(self, account=zksync_test_account):
+    def test_should_form_execution_planner(self, account=test_account):
         modules, encryption, min_native_interval, proxy_config, okx_config, sleep_interval, swap_retry_sleep_interval, gas_prices_gwei = create_config()
 
         execution_plans = create_execution_plans([account], min_native_interval, mock_scenario, modules)
 
         index, (plan_account, modules) = execution_plans[0]
 
         self.assertEqual(1, index)
         self.assertEqual(plan_account, account)
         self.assertEqual(5, len(modules))
         self.assertEqual(2000000000000000, modules[1][0].min_native_balance.wei)
 
-    def test_should_form_execution_planner_with_min_native_interval(self, account=zksync_test_account):
+    def test_should_form_execution_planner_with_min_native_interval(self, account=test_account):
         modules, encryption, min_native_interval, proxy_config, okx_config, sleep_interval, swap_retry_sleep_interval, gas_prices_gwei = create_config()
 
         execution_plans = create_execution_plans([account], min_native_interval, mock_scenario, modules)
 
         index, (plan_account, modules) = execution_plans[0]
 
         self.assertEqual(1, index)
```

### Comparing `sybil_engine-6.8.3/test/module/test_module_executor.py` & `sybil_engine-6.9.0/test/module/test_module_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import unittest
 
 from sybil_engine.module.module_executor import ModuleExecutor
 from sybil_engine.utils.accumulator import get_value
 from sybil_engine.utils.utils import AccountException
-from test import zksync_test_account
+from test import test_account
 from test.module.mock_fail_module import MockFailModule
 from test.module.mock_module import MockModule
 from test.module.mock_not_enoguth_native_module import MockNotEnoughNativeModule
 from test.module.repeatable_mock_module import RepeatableMockModule
 
 
 class TestModuleExecutor(unittest.TestCase):
 
     def test_execute_module(self):
         sleep_interval = {'from': 0, 'to': 0}
-        account = zksync_test_account
+        account = test_account
         min_native_balance = {'from': 0.001, 'to': 0.001}
         modules = [
             (MockModule(min_native_balance, None), {}),
             (MockModule(min_native_balance, None), {}),
             (MockModule(min_native_balance, None), {})
         ]
 
         ModuleExecutor().execute_modules(modules, account, sleep_interval)
 
-        self.assertEqual(get_value("Finished accounts: "), [zksync_test_account])
+        self.assertEqual(get_value("Finished accounts: "), [test_account])
 
     def test_shouldThrowNotEnoughNativeBalance(self):
         sleep_interval = {'from': 0, 'to': 0}
-        account = zksync_test_account
+        account = test_account
         min_native_balance = {'from': 0.001, 'to': 0.001}
         modules = [
             (MockModule(min_native_balance, None), {}),
             (MockModule(min_native_balance, None), {}),
             (MockNotEnoughNativeModule(min_native_balance, None), {})
         ]
 
         ModuleExecutor().execute_modules(modules, account, sleep_interval)
 
         self.assertEqual(len(get_value("Failed accounts: ")), 1)
 
     def test_should_throwAccountExceptionOnModuleException(self):
         sleep_interval = {'from': 0, 'to': 0}
-        account = zksync_test_account
+        account = test_account
         min_native_balance = {'from': 0.001, 'to': 0.001}
 
         module = MockFailModule(min_native_balance, None)
 
         with self.assertRaises(AccountException):
-            ModuleExecutor().execute_module([], account, module, sleep_interval)
+            ModuleExecutor().execute_module({}, account, module, sleep_interval)
 
     def test_should_throwHandleExceptionOnRepeatableModuleException(self):
         sleep_interval = {'from': 0, 'to': 0}
-        account = zksync_test_account
+        account = test_account
         min_native_balance = {'from': 0.001, 'to': 0.001}
 
         module = RepeatableMockModule(min_native_balance, None, 1)
 
-        ModuleExecutor().execute_module([], account, module, sleep_interval)
+        ModuleExecutor().execute_module({}, account, module, sleep_interval)
```

### Comparing `sybil_engine-6.8.3/test/utils/test_create_app_accounts.py` & `sybil_engine-6.9.0/test/utils/test_create_app_accounts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import unittest
 
+from sybil_engine.utils.csv_reader import read_csv_rows
+
 from sybil_engine.domain.balance.balance_utils import interval_to_eth_balance
 from sybil_engine.utils.app_account_utils import create_app_account_with_proxies, create_app_accounts_from_table, \
     validate_cex_addresses, AppAccount
-from test import zksync_test_account
+from test import test_account
 
 
 class TestCreateAppAccounts(unittest.TestCase):
 
     def test_create_zksync(self):
-        zksync_test_account = create_app_account_with_proxies(
+        test_account = create_app_account_with_proxies(
             ['0xb98308D11E2B578858Fbe65b793e71C7a0CAa43e'],
             False,
             'password',
             ['0x7726827caac94a7f9e1b160f7ea819f172f7b6f9d2a97f992c38edeab82d4110'],
             [],
             'RANDOM',
             ['0x6317842385f344acf68561f4e65f0f39e4fb4f1ad104b92bd007361aed39d8'],
         )[0]
 
-        zksync_min_native_balance = interval_to_eth_balance({'from': 1, 'to': 1}, zksync_test_account, None, None)
+        zksync_min_native_balance = interval_to_eth_balance({'from': 1, 'to': 1}, test_account, None, None)
 
     def test_create_base_account(self):
         base_test_account = create_app_account_with_proxies(
             ['0xb98308D11E2B578858Fbe65b793e71C7a0CAa43e'],
             False,
             'password',
             ['0xac0974bec39a17e36ba4a6b4d238ff944bacb478cbed5efcae784d7bf4f2ff80'],
@@ -31,37 +33,39 @@
             'RANDOM',
             ['0x6317842385f344acf68561f4e65f0f39e4fb4f1ad104b92bd007361aed39d8'],
         )[0]
 
         base_min_native_balance = interval_to_eth_balance({'from': 1, 'to': 1}, base_test_account, None, None)
 
     def test_create_zksync_from_csv(self):
+        rows = read_csv_rows('test/data/wallets/accounts.csv')
+
         accounts = create_app_accounts_from_table(
-            'test/data/wallets/accounts.csv',
+            rows,
             'password',
             False
         )
 
         self.assertEqual(
             len(accounts),
             2
         )
         print(accounts)
 
     def test_validate_cex_addresses(self):
         app_accounts = [
-            AppAccount(1, None, zksync_test_account, '1', None, None),
-            AppAccount(2, None, zksync_test_account, '2', None, None)
+            AppAccount(1, None, test_account, '1', None, None),
+            AppAccount(2, None, test_account, '2', None, None)
         ]
         cex_addresses = ['1', '2']
 
         validate_cex_addresses(app_accounts, cex_addresses)
 
     def test_validate_cex_addresses_fail(self):
         app_accounts = [
-            AppAccount(1, None, zksync_test_account, '1', None, None),
-            AppAccount(2, None, zksync_test_account, '2', None, None)
+            AppAccount(1, None, test_account, '1', None, None),
+            AppAccount(2, None, test_account, '2', None, None)
         ]
         cex_addresses = ['1', '3']
 
         with self.assertRaises(Exception):
             validate_cex_addresses(app_accounts, cex_addresses)
```

### Comparing `sybil_engine-6.8.3/test/utils/test_validation_utils.py` & `sybil_engine-6.9.0/test/utils/test_validation_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class TestValidation(unittest.TestCase):
 
     def test_shouldValidateValidChain(self):
         set_module_data(test_modules)
 
         try:
-            validate_chain('ZKSYNC')
-            validate_chain('OPTIMISM')
+            #validate_chain('ZKSYNC')
+            validate_chain('MOCK_CHAIN')
         except Exception as e:
             self.fail(e)
 
     def test_shouldFailInInvalidChain(self):
         set_module_data(test_modules)
 
         with self.assertRaises(Exception):
```

