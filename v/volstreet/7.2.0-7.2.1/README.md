# Comparing `tmp/volstreet-7.2.0.tar.gz` & `tmp/volstreet-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.2.0.tar", last modified: Thu Apr 18 03:26:44 2024, max compression
+gzip compressed data, was "volstreet-7.2.1.tar", last modified: Fri Apr 19 03:41:58 2024, max compression
```

## Comparing `volstreet-7.2.0.tar` & `volstreet-7.2.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.146103 volstreet-7.2.0/
--rw-rw-rw-   0        0        0     1293 2024-04-18 03:26:44.146103 volstreet-7.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.2.0/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1104 2024-04-18 03:26:44.146103 volstreet-7.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.036402 volstreet-7.2.0/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.2.0/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.067592 volstreet-7.2.0/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.2.0/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.2.0/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    17998 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.2.0/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30608 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.2.0/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.083283 volstreet-7.2.0/volstreet/backtests/
--rw-rw-rw-   0        0        0      157 2024-04-13 05:28:03.000000 volstreet-7.2.0/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.2.0/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    46315 2024-04-13 06:57:57.000000 volstreet-7.2.0/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-7.2.0/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0      972 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0       66 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/backtests/state.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-7.2.0/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     2441 2024-04-13 07:18:24.000000 volstreet-7.2.0/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20783 2024-04-09 13:24:35.000000 volstreet-7.2.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6134 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.101845 volstreet-7.2.0/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-7.2.0/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-7.2.0/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.2.0/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.101845 volstreet-7.2.0/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18674 2024-04-13 07:50:10.000000 volstreet-7.2.0/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.2.0/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.101845 volstreet-7.2.0/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.114848 volstreet-7.2.0/volstreet/strategies/
--rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    56285 2024-04-18 03:26:14.000000 volstreet-7.2.0/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.2.0/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    90364 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-7.2.0/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26268 2024-04-18 03:26:18.000000 volstreet-7.2.0/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    18789 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    19897 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.2.0/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.2.0/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.2.0/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2584 2024-04-18 03:26:44.000000 volstreet-7.2.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.730476 volstreet-7.2.1/
+-rw-rw-rw-   0        0        0     1293 2024-04-19 03:41:58.730476 volstreet-7.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.2.1/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1104 2024-04-19 03:41:58.730476 volstreet-7.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.644511 volstreet-7.2.1/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.2.1/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.665516 volstreet-7.2.1/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.2.1/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.2.1/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    17998 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.2.1/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30608 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.2.1/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.675588 volstreet-7.2.1/volstreet/backtests/
+-rw-rw-rw-   0        0        0      157 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.2.1/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    46315 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-7.2.1/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0      972 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0       66 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/state.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-7.2.1/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     2441 2024-04-13 07:18:24.000000 volstreet-7.2.1/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20783 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6134 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.690998 volstreet-7.2.1/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-7.2.1/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-7.2.1/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.2.1/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.690998 volstreet-7.2.1/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18674 2024-04-13 07:50:10.000000 volstreet-7.2.1/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.2.1/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.690998 volstreet-7.2.1/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.707443 volstreet-7.2.1/volstreet/strategies/
+-rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    56285 2024-04-18 03:26:14.000000 volstreet-7.2.1/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.2.1/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    90356 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-7.2.1/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.710445 volstreet-7.2.1/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26268 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    18977 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    19897 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.720302 volstreet-7.2.1/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.2.1/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.729474 volstreet-7.2.1/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.2.1/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.2.1/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.730476 volstreet-7.2.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2584 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.2.0/PKG-INFO` & `volstreet-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.2.0
+Version: 7.2.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.2.0/setup.cfg` & `volstreet-7.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 322e 300d 0a61  rsion = 7.2.0..a
+00000020: 7273 696f 6e20 3d20 372e 322e 310d 0a61  rsion = 7.2.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-7.2.0/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.2.1/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/angel_interface/async_interface.py` & `volstreet-7.2.1/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/angel_interface/base_websocket.py` & `volstreet-7.2.1/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/angel_interface/interface.py` & `volstreet-7.2.1/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/angel_interface/login.py` & `volstreet-7.2.1/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/angel_interface/order_websocket.py` & `volstreet-7.2.1/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/angel_interface/price_websocket.py` & `volstreet-7.2.1/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/angel_interface/smart_connect.py` & `volstreet-7.2.1/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/database.py` & `volstreet-7.2.1/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/delta_hedging.py` & `volstreet-7.2.1/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/delta_optimizer.py` & `volstreet-7.2.1/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/framework.py` & `volstreet-7.2.1/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.2.1/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/proxy_functions.py` & `volstreet-7.2.1/volstreet/backtests/proxy_functions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/tools.py` & `volstreet-7.2.1/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/trend.py` & `volstreet-7.2.1/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/backtests/underlying_info.py` & `volstreet-7.2.1/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/blackscholes.py` & `volstreet-7.2.1/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/config.py` & `volstreet-7.2.1/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/database_connection.py` & `volstreet-7.2.1/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/analysis.py` & `volstreet-7.2.1/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/archive.py` & `volstreet-7.2.1/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/data_handling.py` & `volstreet-7.2.1/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/eod_client.py` & `volstreet-7.2.1/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/gambling.py` & `volstreet-7.2.1/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/intraday_data.py` & `volstreet-7.2.1/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/stockmock.py` & `volstreet-7.2.1/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/datamodule/trading_assistance.py` & `volstreet-7.2.1/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/dealingroom.py` & `volstreet-7.2.1/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/decorators.py` & `volstreet-7.2.1/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/discord_bot.py` & `volstreet-7.2.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/exceptions.py` & `volstreet-7.2.1/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.2.1/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/parallelization.py` & `volstreet-7.2.1/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/performance_tracking.py` & `volstreet-7.2.1/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/position_dashboard/app.py` & `volstreet-7.2.1/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/position_dashboard/formatting.py` & `volstreet-7.2.1/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/strategies/deployment.py` & `volstreet-7.2.1/volstreet/strategies/deployment.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/strategies/error_handling.py` & `volstreet-7.2.1/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/strategies/helpers.py` & `volstreet-7.2.1/volstreet/strategies/helpers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/strategies/monitoring.py` & `volstreet-7.2.1/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/strategies/optimization.py` & `volstreet-7.2.1/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/strategies/strats.py` & `volstreet-7.2.1/volstreet/strategies/strats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1161,15 +1161,15 @@
 
         # Placing the trend option order
         exec_details = execute_instructions(
             {
                 trend_option: {
                     "action": Action.SELL,
                     "quantity_in_lots": qty_in_lots,
-                    "order_tag": f"Intraday Strangle Trend Catcher",
+                    "order_tag": f"{strategy_tag} Trend Catcher",
                 }
             }
         )
         sell_avg_price = exec_details[trend_option]
 
         # Setting up the stop losses on underlying and trend option
 
@@ -1239,15 +1239,15 @@
         if square_off:
             # Buying the trend option back
             exec_details = execute_instructions(
                 {
                     trend_option: {
                         "action": Action.BUY,
                         "quantity_in_lots": qty_in_lots,
-                        "order_tag": f"Intraday Strangle Trend Catcher",
+                        "order_tag": f"{strategy_tag} Trend Catcher",
                     }
                 }
             )
             square_up_avg_price = exec_details[trend_option]
         else:
             square_up_avg_price = trend_option.fetch_ltp()
 
@@ -1416,15 +1416,15 @@
                 )
                 info_dict[f"{other_side}_stop_loss_order_ids"] = (
                     place_option_order_and_notify(
                         instrument=option_to_repair,
                         action="BUY",
                         qty_in_lots=quantity_in_lots,
                         prices=info_dict[f"{other_side}_stop_loss_price"],
-                        order_tag=f"{other_side.capitalize()} SL move to cost",
+                        order_tag=f"{other_side.capitalize()} stop loss {strategy_tag}",
                         webhook_url=notification_url,
                         stop_loss_order=True,
                         target_status="trigger pending",
                         return_avg_price=False,
                     )
                 )
 
@@ -1626,26 +1626,26 @@
 
     if place_sl_orders:
         call_stop_loss_order_ids = place_option_order_and_notify(
             instrument=strangle.call_option,
             action="BUY",
             qty_in_lots=quantity_in_lots,
             prices=call_stop_loss_price,
-            order_tag="Call SL Strangle",
+            order_tag=strategy_tag,
             webhook_url=notification_url,
             stop_loss_order=True,
             target_status="trigger pending",
             return_avg_price=False,
         )
         put_stop_loss_order_ids = place_option_order_and_notify(
             instrument=strangle.put_option,
             action="BUY",
             qty_in_lots=quantity_in_lots,
             prices=put_stop_loss_price,
-            order_tag="Put SL Strangle",
+            order_tag=strategy_tag,
             webhook_url=notification_url,
             stop_loss_order=True,
             target_status="trigger pending",
             return_avg_price=False,
         )
     else:
         call_stop_loss_order_ids = None
```

### Comparing `volstreet-7.2.0/volstreet/trade_interface/instruments.py` & `volstreet-7.2.1/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/trade_interface/order_execution.py` & `volstreet-7.2.1/volstreet/trade_interface/order_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,44 +117,46 @@
     Returns the average price of all executed orders.
     """
     if session is None:
         async with ActiveSession.obj.async_session() as session:
             return await execute_orders_per_symbol(orders, symbol, session)
 
     order_ids = await place_orders(orders, session)
+    await asyncio.sleep(0.25)
     statuses = await fetch_statuses(order_ids, session)
     check_for_rejection(statuses)
     open_orders = filter_for_open_orders(statuses)
 
-    iteration = 0
+    iteration = 1
     while open_orders:
-        iteration += 1
-        if iteration == 10:
+        if iteration == 3:
             notifier(
                 f"Max modification iterations reached for symbol {symbol}.",
                 config.ERROR_NOTIFICATION_SETTINGS["url"],
                 "ERROR",
             )
             break  # todo: Can we add get_ltp_async here to return the ltp as the avg price? think about it
         additional_buffer = iteration / 100
         quotes = await get_quotes_async(
             [order["symboltoken"] for order in open_orders], session=session
         )
         await modify_open_orders(open_orders, quotes, additional_buffer, session)
+        await asyncio.sleep(0.25)
         statuses = await fetch_statuses(order_ids, session)
         check_for_rejection(statuses)
         open_orders = filter_for_open_orders(statuses)
+        iteration += 1
 
     logger.info(f"Orders successfully executed for symbol {symbol}.")
 
     avg_price = calculate_average_price(statuses, order_ids)
     return avg_price
 
 
-async def _execute_orders(orders: list[dict]) -> dict:
+async def execute_orders(orders: list[dict]) -> dict:
     """The difference between this function and execute_order_per_symbol is that this function
     can take in orders of different action types and symbols. It groups the orders
     into transaction types and symbol tokens and executes them in parallel, prioritizing
     buy orders to be executed first.
     """
     master_dict = {}
     orders.sort(key=lambda x: x["transactiontype"])
@@ -182,21 +184,14 @@
                 # then this will overwrite the avg_price for that token with the sell avg_price
                 # This is a limitation of the current implementation. It will be fixed in the future.
                 master_dict[symbol] = avg_price
 
     return master_dict
 
 
-async def execute_orders(orders: list[dict]) -> dict:
-    with order_placement_lock:
-        logger.info(f"{threading.current_thread().name} is executing orders.")
-        result = await _execute_orders(orders)
-        return result
-
-
 def generate_bulk_params(
     instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict]
 ) -> list[dict]:
 
     def fetch_market_depth(instruments):
         option_tokens = {
             instrument.token
@@ -265,15 +260,15 @@
                 instr.generate_order_params(**params, price=(call_price, put_price))
             )
 
     return order_params
 
 
 @timeit()
-def execute_instructions(
+def _execute_instructions(
     instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict]
 ) -> dict[Option | Strangle | Straddle | SyntheticFuture, float]:
     """Executes orders for a given set of instructions.
     Instructions is a dictionary where the keys are Instrument objects and
     the values are dictionaries containing the order parameters.
     The order parameters MUST contain the following keys:
     - action: Action.BUY or Action.SELL
@@ -326,14 +321,23 @@
             for instr in og_instructions
             if instr not in instructions
         }
     )
     return average_prices
 
 
+def execute_instructions(
+    instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict]
+) -> dict[Option | Strangle | Straddle | SyntheticFuture, float]:
+    with order_placement_lock:
+        logger.info(f"{threading.current_thread().name} is executing orders.")
+        result = _execute_instructions(instructions)
+        return result
+
+
 @timeit()
 def place_option_order_and_notify(
     instrument: Option | Strangle | Straddle | SyntheticFuture,
     action: Action | str,
     qty_in_lots: int,
     prices: str | int | float | tuple | list | np.ndarray = "LIMIT",
     order_tag: str = "",
```

### Comparing `volstreet-7.2.0/volstreet/trade_interface/underlyings.py` & `volstreet-7.2.1/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/utils/change_config.py` & `volstreet-7.2.1/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/utils/communication.py` & `volstreet-7.2.1/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/utils/core.py` & `volstreet-7.2.1/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/utils/data_io.py` & `volstreet-7.2.1/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/utils/scrip_processing.py` & `volstreet-7.2.1/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/vectorized_blackscholes.py` & `volstreet-7.2.1/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/vslogging/formatters.py` & `volstreet-7.2.1/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/vslogging/logging_config.json` & `volstreet-7.2.1/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/vslogging/logging_setup.py` & `volstreet-7.2.1/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet/vslogging/parsing.py` & `volstreet-7.2.1/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.0/volstreet.egg-info/PKG-INFO` & `volstreet-7.2.1/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.2.0
+Version: 7.2.1
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.2.0/volstreet.egg-info/SOURCES.txt` & `volstreet-7.2.1/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

