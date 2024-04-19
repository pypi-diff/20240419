# Comparing `tmp/martin_binance-3.0.5.tar.gz` & `tmp/martin_binance-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-3.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-3.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-3.0.5.tar` & `martin_binance-3.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1079 2024-04-16 12:48:01.803069 martin_binance-3.0.5/LICENSE
--rwxr-xr-x   0        0        0     3854 2024-04-16 12:48:01.803069 martin_binance-3.0.5/README.md
--rwxr-xr-x   0        0        0     1890 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/__init__.py
--rw-r--r--   0        0        0     5007 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2786 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    13214 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/exchange_simulator.py
--rwxr-xr-x   0        0        0     4165 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/optimizer.py
--rw-r--r--   0        0        0     4705 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/client.py
--rw-r--r--   0        0        0     6935 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/db_utils.py
--rwxr-xr-x   0        0        0   139919 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/executor.py
--rw-r--r--   0        0        0    15709 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/lib.py
--rw-r--r--   0        0        0     3287 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/params.py
--rw-r--r--   0        0        0      485 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    14650 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1269 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/relaunch.service
--rw-r--r--   0        0        0    82424 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/strategy_base.py
--rw-r--r--   0        0        0     7151 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/telegram_utils.py
--rw-r--r--   0        0        0     7217 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_0_BTCUSDT.py
--rw-r--r--   0        0        0     7219 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_1_BTCUSDT.py
--rw-r--r--   0        0        0     7223 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
--rwxr-xr-x   0        0        0     7212 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_3_BTCUSDT.py
--rw-r--r--   0        0        0   237568 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/funds_rate.db
--rw-r--r--   0        0        0     1723 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/ms_cfg.toml
--rw-r--r--   0        0        0      639 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/trial_params.json
--rw-r--r--   0        0        0     1425 2024-04-16 12:48:01.843069 martin_binance-3.0.5/pyproject.toml
--rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 martin_binance-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-19 15:23:47.148182 martin_binance-3.0.6/LICENSE
+-rwxr-xr-x   0        0        0     3854 2024-04-19 15:23:47.148182 martin_binance-3.0.6/README.md
+-rwxr-xr-x   0        0        0     1890 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/__init__.py
+-rw-r--r--   0        0        0     5007 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2786 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    13214 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/exchange_simulator.py
+-rwxr-xr-x   0        0        0     4165 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/backtest/optimizer.py
+-rw-r--r--   0        0        0     4781 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/client.py
+-rw-r--r--   0        0        0     6935 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/db_utils.py
+-rwxr-xr-x   0        0        0   139982 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/executor.py
+-rw-r--r--   0        0        0    15709 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/lib.py
+-rw-r--r--   0        0        0     3287 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/params.py
+-rw-r--r--   0        0        0      485 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    14650 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1269 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2024-04-19 15:23:47.184182 martin_binance-3.0.6/martin_binance/service/relaunch.service
+-rw-r--r--   0        0        0    83599 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/strategy_base.py
+-rw-r--r--   0        0        0     7151 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/telegram_utils.py
+-rw-r--r--   0        0        0     7217 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_0_BTCUSDT.py
+-rw-r--r--   0        0        0     7219 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_1_BTCUSDT.py
+-rw-r--r--   0        0        0     7223 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
+-rwxr-xr-x   0        0        0     7212 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/cli_3_BTCUSDT.py
+-rw-r--r--   0        0        0   237568 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/funds_rate.db
+-rw-r--r--   0        0        0     1723 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/ms_cfg.toml
+-rw-r--r--   0        0        0      639 2024-04-19 15:23:47.188182 martin_binance-3.0.6/martin_binance/templates/trial_params.json
+-rw-r--r--   0        0        0     1425 2024-04-19 15:23:47.188182 martin_binance-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 martin_binance-3.0.6/PKG-INFO
```

### Comparing `martin_binance-3.0.5/LICENSE` & `martin_binance-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/README.md` & `martin_binance-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/__init__.py` & `martin_binance-3.0.6/martin_binance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.5"
+__version__ = "3.0.6"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 from exchanges_wrapper.definitions import Interval
```

### Comparing `martin_binance-3.0.5/martin_binance/backtest/OoTSP.py` & `martin_binance-3.0.6/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/backtest/VCoSEL.py` & `martin_binance-3.0.6/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/backtest/exchange_simulator.py` & `martin_binance-3.0.6/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/backtest/optimizer.py` & `martin_binance-3.0.6/martin_binance/backtest/optimizer.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/client.py` & `martin_binance-3.0.6/martin_binance/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 gRPC async client for exchanges-wrapper
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.4"
+__version__ = "3.0.6"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import asyncio
 import random
 import logging
 
@@ -42,15 +42,16 @@
         self.wait_connection = True
         client = None
         while client is None:
             self.channel = Channel('127.0.0.1', 50051)
             self.stub = mr.MartinStub(self.channel)
             try:
                 client = await self.connect()
-            except UserWarning:
+            except UserWarning as ex:
+                logger.warning(ex)
                 client = None
                 self.channel.close()
                 await asyncio.sleep(random.randint(5, 30))
             else:
                 self.client = client
                 self.wait_connection = False
                 return True
@@ -62,15 +63,15 @@
                     trade_id=self.trade_id,
                     account_name=self.account_name,
                     rate_limiter=self.rate_limiter,
                     symbol=self.symbol
                 )
             )
         except asyncio.CancelledError:
-            pass  # Task cancellation should not be logged as an error.
+            pass  # Task cancellation should not be logged as an error
         except ConnectionRefusedError as ex:
             raise UserWarning(f"{ex}, reconnect...") from None
         except GRPCError as ex:
             status_code = ex.status
             logger.warning(f"Exception on register client: {status_code.name}, {ex.message}")
             if status_code == Status.FAILED_PRECONDITION:
                 raise SystemExit(1) from ex
@@ -81,15 +82,15 @@
 
     async def send_request(self, _request, _request_type, **kwargs):
         if not self.client:
             raise UserWarning("Send gRPC request failed, not active client session")
         kwargs['client_id'] = self.client.client_id
         kwargs['trade_id'] = self.trade_id
         try:
-            return await _request(_request_type(**kwargs))
+            res = await _request(_request_type(**kwargs))
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except grpclib.exceptions.StreamTerminatedError:
             raise UserWarning("Have not connection to gRPC server")
         except ConnectionRefusedError:
             raise UserWarning("Connection to gRPC server broken")
         except GRPCError as ex:
@@ -97,14 +98,16 @@
             logger.debug(f"Send request {_request}: {status_code.name}, {ex.message}")
             if status_code == Status.UNAVAILABLE:
                 self.client = None
                 raise UserWarning("Wait connection to gRPC server") from None
             raise
         except Exception as ex:
             logger.error(f"Exception on send request {ex}")
+        else:
+            return res
 
     async def for_request(self, _request, _request_type, **kwargs):
         if not self.client:
             raise UserWarning("Start gRPC request loop failed, not active client session")
         kwargs['client_id'] = self.client.client_id
         kwargs['trade_id'] = self.trade_id
         try:
```

### Comparing `martin_binance-3.0.5/martin_binance/db_utils.py` & `martin_binance-3.0.6/martin_binance/db_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/executor.py` & `martin_binance-3.0.6/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Cyclic grid strategy based on martingale
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.5"
+__version__ = "3.0.6"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import logging
 import sys
 import gc
 import statistics
@@ -65,19 +65,19 @@
         self.part_profit_first = O_DEC  # +
         self.part_profit_second = O_DEC  # +
         self.tp_was_filled = ()  # - Exist incomplete processing filled TP
         #
         self.sum_amount_first = O_DEC  # Sum buy/sell in first currency for current cycle
         self.sum_amount_second = O_DEC  # Sum buy/sell in second currency for current cycle
         self.part_amount = {}  # + {order_id: (Decimal(str(amount_f)), Decimal(str(amount_s)))} of partially filled
-    #
+        #
         self.deposit_first = AMOUNT_FIRST  # + Calculated operational deposit
         self.deposit_second = AMOUNT_SECOND  # + Calculated operational deposit
-        self.sum_profit_first = O_DEC  # + Sum profit from start to now()
-        self.sum_profit_second = O_DEC  # + Sum profit from start to now()
+        self.sum_profit_first = O_DEC  # + Sum profit from start
+        self.sum_profit_second = O_DEC  # + Sum profit from start
         self.cycle_buy_count = 0  # + Count for buy cycle
         self.cycle_sell_count = 0  # + Count for sale cycle
         self.shift_grid_threshold = None  # - Price level of shift grid threshold for current cycle
         self.f_currency = ''  # - First currency name
         self.s_currency = ''  # - Second currency name
         self.last_shift_time = None  # -
         self.avg_rate = O_DEC  # - Flow average rate for trading pair
@@ -371,28 +371,27 @@
                     order_sell = self.cycle_status[2]
                     order_hold = self.cycle_status[3]
                 else:
                     orders = self.get_buffered_open_orders()
                     order_buy = len([i for i in orders if i.buy is True])
                     order_sell = len([i for i in orders if i.buy is False])
                     order_hold = len(self.orders_hold)
-                sum_profit = self.round_truncate(self.sum_profit_first * self.avg_rate + self.sum_profit_second,
-                                                 base=False)
+
                 command = bool(self.command in ('end', 'stop'))
                 if GRID_ONLY:
                     header = (f"{'Buy' if self.cycle_buy else 'Sell'} assets Grid only mode\n"
                               f"{('Waiting funding for convert' + chr(10)) if self.grid_only_restart else ''}"
                               f"{self.get_free_assets()[3]}"
                               )
                 else:
                     header = (f"Complete {self.cycle_buy_count} buy cycle and {self.cycle_sell_count} sell cycle\n"
                               f"For all cycles profit:\n"
                               f"First: {self.sum_profit_first}\n"
                               f"Second: {self.sum_profit_second}\n"
-                              f"Summary: {sum_profit}\n"
+                              f"Summary: {self.get_sum_profit()}\n"
                               f"{self.get_free_assets(mode='free')[3]}"
                               )
                 self.message_log(f"{header}\n"
                                  f"{'*** Shift grid mode ***' if self.shift_grid_threshold else '* **  **  ** *'}\n"
                                  f"{'Buy' if self.cycle_buy else 'Sell'}{' Reverse' if self.reverse else ''}"
                                  f"{' Hold reverse' if self.reverse_hold else ''} "
                                  f"{MODE}{'-SO' if MODE == 'TC' and SELF_OPTIMIZATION else ''}-cycle with"
@@ -459,15 +458,16 @@
                 self.start()
 
     def _common_stable_conditions(self):
         """
         Checks the common conditions for stability in both live and backtest modes.
         """
         return (
-            self.grid_remove is None
+            self.operational_status
+            and self.grid_remove is None
             and not GRID_ONLY
             and not self.grid_update_started
             and not self.start_after_shift
             and not self.tp_hold
             and not self.tp_order_hold
             and not self.orders_init
             and self.command != 'stopped'
@@ -691,15 +691,15 @@
                 self.message_log("Waiting for conditions for conversion", color=Style.B_WHITE)
                 return
         if not self.first_run and not self.start_after_shift and not self.reverse and not GRID_ONLY:
             self.message_log(f"Complete {self.cycle_buy_count} buy cycle and {self.cycle_sell_count} sell cycle\n"
                              f"For all cycles profit:\n"
                              f"First: {self.sum_profit_first}\n"
                              f"Second: {self.sum_profit_second}\n"
-                             f"Summary: {self.sum_profit_first * self.avg_rate + self.sum_profit_second:f}\n")
+                             f"Summary: {self.get_sum_profit()}\n")
         if self.first_run or MODE in ('T', 'TC'):
             self.cycle_time = datetime.now(timezone.utc).replace(tzinfo=None)
         #
         memory = psutil.virtual_memory()
         swap = psutil.swap_memory()
         total_used_percent = 100 * float(swap.used + memory.used) / (swap.total + memory.total)
         if total_used_percent > 85:
@@ -2113,15 +2113,15 @@
             buy: bool,
             amount: Decimal,
             price: Decimal,
             check=False,
             price_limit_rules=False
     ) -> int:
         """
-        Before place limit order check trade conditions and correct price
+        Before place limit order checking trade conditions and correct price
         """
         if self.command == 'stopped':
             return 0
         if price_limit_rules:
             tcm = self.get_trading_capability_manager()
             _price = self.get_buffered_ticker().last_price or self.avg_rate
             if ((buy and price < tcm.get_min_buy_price(_price)) or
@@ -2210,14 +2210,20 @@
         restart = False
         delta = self.round_truncate(
             delta,
             bool(asset == self.f_currency),
             _rounding=ROUND_FLOOR if delta > 0 else ROUND_CEILING
         )
         #
+        if delta < 0 and not GRID_ONLY:
+            if asset == self.f_currency:
+                self.sum_profit_first += abs(delta)
+            elif asset == self.s_currency:
+                self.sum_profit_second += abs(delta)
+        #
         if self.cycle_buy:
             if asset == self.s_currency:
                 restart = True
                 if self.reverse:
                     if delta < 0 and abs(delta) > self.initial_reverse_second - self.deposit_second:
                         self.deposit_second = self.initial_reverse_second + delta
                     elif delta > 0:
```

### Comparing `martin_binance-3.0.5/martin_binance/lib.py` & `martin_binance-3.0.6/martin_binance/lib.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/params.py` & `martin_binance-3.0.6/martin_binance/params.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/service/funds_rate_exporter.py` & `martin_binance-3.0.6/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/service/grafana.json` & `martin_binance-3.0.6/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/service/relaunch.py` & `martin_binance-3.0.6/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/strategy_base.py` & `martin_binance-3.0.6/martin_binance/strategy_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 martin-binance base class and methods definitions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.4"
+__version__ = "3.0.6"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import csv
 import logging
@@ -303,107 +303,111 @@
         self.trades[:] = [i for i in self.trades if i.order_id != _order_id]
 
     #
     async def backtest_control(self):
         """
         Managing backtest and optimization cycles
         """
-        while not self.operational_status:
-            await asyncio.sleep(HEARTBEAT)
         delay = HEARTBEAT * 30  # 1 min
         ts = time.time()
         restart = False
         _prm_best = {}
         prm_best = {}
-        while self.operational_status:
-            if self.start_collect and time.time() - ts > prm.SAVE_PERIOD:
-                self.start_collect = False
-                self.session_data_handler()
-                self.reset_backtest_vars()
-                if prm.SELF_OPTIMIZATION and self.command != 'stopped':
-                    _ts = datetime.now(timezone.utc).replace(tzinfo=None)
-                    storage_name = Path(self.session_root, "_study.db")
-                    try:
-                        self.backtest_process = await asyncio.create_subprocess_exec(
-                            OPTIMIZER,
-                            f"{self.exchange}_{self.symbol}",
-                            Path(self.session_root, Path(prm.PARAMS).name),
-                            str(prm.N_TRIALS),
-                            f"sqlite:///{storage_name}",
-                            json.dumps(prm_best or _prm_best),
-                            f"{prm.ID_EXCHANGE}_{prm.SYMBOL}_S.log",
-
-                            stdout=asyncio.subprocess.PIPE
-                        )
-                        stdout, _ = await self.backtest_process.communicate()
-                        _res = stdout.splitlines()
-                        if _res:
-                            prm_best = orjson.loads(_res[0])
+        _res = None
+        while True:
+            await asyncio.sleep(delay)
+            try:
+                if self.operational_status and self.start_collect and time.time() - ts > prm.SAVE_PERIOD:
+                    self.start_collect = False
+                    self.session_data_handler()
+                    self.reset_backtest_vars()
+                    if prm.SELF_OPTIMIZATION and self.command != 'stopped':
+                        _ts = datetime.now(timezone.utc).replace(tzinfo=None)
+                        storage_name = Path(self.session_root, "_study.db")
+                        try:
+                            self.backtest_process = await asyncio.create_subprocess_exec(
+                                OPTIMIZER,
+                                f"{self.exchange}_{self.symbol}",
+                                Path(self.session_root, Path(prm.PARAMS).name),
+                                str(prm.N_TRIALS),
+                                f"sqlite:///{storage_name}",
+                                json.dumps(prm_best or _prm_best),
+                                f"{prm.ID_EXCHANGE}_{prm.SYMBOL}_S.log",
+                                stdout=asyncio.subprocess.PIPE
+                            )
+                            stdout, _ = await self.backtest_process.communicate()
+                        except Exception as ex:
+                            self.message_log(f"Backtest process: {ex}", log_level=logging.ERROR)
                         else:
-                            self.message_log("Backtest control: result is empty", log_level=logging.WARNING)
-                            break
-                    except (asyncio.CancelledError, KeyboardInterrupt):
-                        break
-                    except Exception as err:
-                        self.message_log(f"Backtest control: {err}", log_level=logging.ERROR)
-                        self.message_log(f"Exception traceback: {traceback.format_exc()}", log_level=logging.DEBUG)
-                        break
-                    #
-                    self.backtest_process = None
-                    storage_name.replace(storage_name.with_name('study.db'))
-                    if prm_best:
-                        _prm_best = dict(prm_best)
+                            _res = stdout.splitlines()
+                        if _res:
+                            try:
+                                prm_best = orjson.loads(_res[0])
+                            except orjson.JSONDecodeError:
+                                self.message_log(f"Backtest control: response {_res}", log_level=logging.ERROR)
+                        #
+                        self.backtest_process = None
+                        storage_name.replace(storage_name.with_name('study.db'))
+                        if prm_best:
+                            _prm_best = dict(prm_best)
+                            self.message_log(
+                                f"Updating parameters from backtest,"
+                                f" predicted value {prm_best.pop('_value')} -> {prm_best.pop('new_value')}",
+                                color=Style.B_WHITE,
+                                tlg=True
+                            )
+                            for key, value in prm_best.items():
+                                self.message_log(f"{key}: {getattr(prm, key)} -> {value}")
+                                setattr(
+                                    prm, key,
+                                    value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}")
+                                )
+                        l_m = str(
+                            datetime.now(timezone.utc).replace(tzinfo=None) - _ts + timedelta(seconds=prm.SAVE_PERIOD)
+                        ).rsplit('.')[0]
                         self.message_log(
-                            f"Updating parameters from backtest,"
-                            f" predicted value {prm_best.pop('_value')} -> {prm_best.pop('new_value')}",
+                            f"Strategy parameters are optimal now. Optimization cycle duration {l_m}",
                             color=Style.B_WHITE,
                             tlg=True
                         )
-                        for key, value in prm_best.items():
-                            self.message_log(f"{key}: {getattr(prm, key)} -> {value}")
-                            setattr(
-                                prm, key,
-                                value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}")
-                            )
-                    l_m = str(
-                        datetime.now(timezone.utc).replace(tzinfo=None) - _ts + timedelta(seconds=prm.SAVE_PERIOD)
-                    ).rsplit('.')[0]
-                    self.message_log(
-                        f"Strategy parameters are optimal now. Optimization cycle duration {l_m}",
-                        color=Style.B_WHITE,
-                        tlg=True
-                    )
-                    restart = True
-                else:
-                    break
+                        restart = True
+                    else:
+                        break
 
-            if restart and self.stable_state_backtest():
-                restart = False
-                self.parquet_declare(Path(self.session_root, "raw"))
-                # Refresh klines init
-                for i in KLINES_INIT:
+                if restart and self.stable_state_backtest():
+                    restart = False
+                    # Refresh klines init
                     try:
-                        res = await self.send_request(self.stub.fetch_klines, mr.FetchKlinesRequest,
-                                                      symbol=self.symbol,
-                                                      interval=i.value,
-                                                      limit=KLINES_LIM)
+                        for i in KLINES_INIT:
+                            res = await self.send_request(self.stub.fetch_klines, mr.FetchKlinesRequest,
+                                                          symbol=self.symbol,
+                                                          interval=i.value,
+                                                          limit=KLINES_LIM)
+                            self.klines[i.value] = list(map(json.loads, res.items))
                     except Exception as ex:
+                        restart = True
                         self.message_log(f"FetchKlines: {ex}", log_level=logging.WARNING)
-                    else:
-                        self.klines[i.value] = list(map(json.loads, res.items))
-                # Save current strategy state for backtesting
-                last_state = self.save_strategy_state()
-                self.last_state_update(last_state)
-                with self.state_file.open(mode='w') as outfile:
-                    json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
-                #
-                self.start_collect = True
-                ts = time.time()
-                self.message_log("Start data collect", tlg=True)
-            await asyncio.sleep(delay)
+                        continue
+
+                    self.parquet_declare(Path(self.session_root, "raw"))
+                    # Save current strategy state for backtesting
+                    last_state = self.save_strategy_state()
+                    self.last_state_update(last_state)
+                    with self.state_file.open(mode='w') as outfile:
+                        json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
+                    #
+                    self.start_collect = True
+                    ts = time.time()
+                    self.message_log("Start data collect", tlg=True)
+            except (asyncio.CancelledError, KeyboardInterrupt):
+                break
+            except Exception as err:
+                self.message_log(f"Backtest control: {err}", log_level=logging.ERROR)
+                self.message_log(f"Exception traceback: {traceback.format_exc()}", log_level=logging.DEBUG)
+                break
         self.message_log("Backtest data collect and optimize session ended", tlg=True)
 
     def session_data_handler(self):
         """
         Save raw data for back testing and session snapshot for compare.
         """
         # Finalize ticker file
@@ -475,14 +479,17 @@
             print(f"Session profit: {s_profit}, free: {s_free}, total: {float(s_profit) + float(s_free)}")
             test_time = datetime.now(timezone.utc).replace(tzinfo=None) - self.cycle_time
             original_time = (self.backtest['ticker_index_last'] - self.backtest['ticker_index_first']) / 1000
             original_time = timedelta(seconds=original_time)
             print(f"Original time: {original_time}, test time: {test_time}, x = {original_time / test_time:.2f}")
         if prm.SAVE_DS:
             self._back_test_handler_ext()
+
+        self.session.channel.close()
+        self.task_cancel()
         asyncio.get_event_loop().stop()
 
     def _back_test_handler_ext(self):
         # Save test data
         session_path = Path(BACKTEST_PATH,
                             f"{self.exchange}_{self.symbol}_{datetime.now().strftime('%m%d-%H-%M-%S')}")
         session_path.mkdir(parents=True)
@@ -541,28 +548,31 @@
                             self.message_log(f"Exception on check WSS: {ex}", log_level=logging.ERROR)
                         else:
                             if not res.success:
                                 self.message_log(f"Not active WSS for {self.symbol} on {self.exchange},"
                                                  f" restart request sent", log_level=logging.WARNING)
                                 update_max_queue_size = True
                                 self.wss_fire_up = True
+                        finally:
+                            if self.wss_fire_up:
+                                self.operational_status = False
                     #
                     if self.wss_fire_up:
                         try:
                             if await self.session.get_client():
                                 self.update_vars(self.session)
                                 await self.send_request(
                                     self.stub.stop_stream,
                                     mr.MarketRequest,
                                     symbol=self.symbol
                                 )
                                 await self.wss_init(update_max_queue_size=update_max_queue_size)
-                                self.wss_fire_up = False
                         except Exception as ex:
                             self.message_log(f"Exception on fire up WSS: {ex}", log_level=logging.WARNING)
+                            self.message_log(traceback.format_exc(), log_level=logging.DEBUG)
                             self.wss_fire_up = True
                 await asyncio.sleep(HEARTBEAT)
             except (KeyboardInterrupt, asyncio.CancelledError):
                 break
 
     async def save_asset(self):
         """
@@ -571,19 +581,22 @@
         connection_analytic = None
         balances = []
         while connection_analytic is None:
             connection_analytic = self.connection_analytic
             await asyncio.sleep(HEARTBEAT)
         delay = 600  # 10 min
         max_use_update = 25 * 60  # 25 min if the row has not been updated that the instance is down
-        while self.operational_status:
+        while True:
+            if not self.operational_status:
+                await asyncio.sleep(HEARTBEAT * 30)
+                continue
             try:
                 res = await self.send_request(self.stub.fetch_account_information, mr.OpenClientConnectionId)
-            except asyncio.CancelledError:
-                pass
+            except (asyncio.CancelledError, KeyboardInterrupt):
+                break
             except Exception as _ex:
                 self.message_log(f"Exception save_asset: {_ex}", log_level=logging.WARNING)
             else:
                 if res:
                     balances = list(map(json.loads, res.items))
                 # Refresh actual balance
                 try:
@@ -600,16 +613,16 @@
                 }
                 # Get asset balances from Funding Wallet
                 funding_wallet = []
                 assets_fw = {}
                 if self.exchange not in ('bitfinex', 'huobi'):
                     try:
                         res = await self.send_request(self.stub.fetch_funding_wallet, mr.FetchFundingWalletRequest)
-                    except asyncio.CancelledError:
-                        pass
+                    except (asyncio.CancelledError, KeyboardInterrupt):
+                        break
                     except Exception as _ex:
                         logger.warning(f"FetchFundingWallet: {_ex}")
                     else:
                         funding_wallet = list(map(json.loads, res.items))
                     for fw in funding_wallet:
                         assets_fw[fw['asset']] = Decimal(fw['free']) + Decimal(fw['locked']) + Decimal(fw['freeze'])
                 # Create list of cumulative asset from SPOT and Funding wallet
@@ -949,42 +962,43 @@
                     break
             await asyncio.sleep(600)
 
     async def buffered_candle(self):
         Klines.klines_lim = KLINES_LIM
         klines = {}
         klines_from_file = {}
+        kline = []
         if prm.MODE == 'S':
             klines_from_file = json.load(open(Path(self.session_root, "raw/klines.json")))
         for i in KLINES_INIT:
             if prm.MODE in ('T', 'TC'):
                 try:
                     res = await self.send_request(
                         self.stub.fetch_klines, mr.FetchKlinesRequest,
                         symbol=self.symbol,
                         interval=i.value,
                         limit=KLINES_LIM
                     )
                 except Exception as ex:
-                    kline = []
                     self.message_log(f"FetchKlines: {ex}", log_level=logging.WARNING)
                 else:
-                    kline = list(map(json.loads, res.items))
-                    if prm.MODE == 'TC' and (self.start_collect or self.start_collect is None):
-                        self.klines[i.value] = kline
+                    if res:
+                        kline = list(map(json.loads, res.items))
+                        if prm.MODE == 'TC' and (self.start_collect or self.start_collect is None):
+                            self.klines[i.value] = kline
             else:
                 kline = klines_from_file.get(i.value, [])
 
             kline_i = Klines(i.value)
             for candle in kline:
                 kline_i.refresh(candle)
             klines[i.value] = kline_i
 
         if len(klines) == len(KLINES_INIT):
-            self.tasks_manage(self.on_klines_update(klines))
+            self.tasks_manage(self.on_klines_update(klines), name='wss')
         else:
             self.message_log("Init buffered candle failed. try one else...", log_level=logging.WARNING)
             await asyncio.sleep(random.uniform(1, 5))
             self.wss_fire_up = True
 
     async def on_klines_update(self, _klines: {str: Klines}):
         _intervals = list(_klines.keys())
@@ -1008,15 +1022,15 @@
                         )
             except Exception as ex:
                 self.message_log(f"Exception on WSS, on_klines_update loop closed: {ex}", log_level=logging.WARNING)
                 self.message_log(f"Exception traceback: {traceback.format_exc()}", log_level=logging.DEBUG)
                 self.wss_fire_up = True
         else:
             for i in _intervals:
-                self.tasks_manage(self.aiter_candles(_klines, i))
+                self.tasks_manage(self.aiter_candles(_klines, i), name='wss')
 
     async def create_limit_order(self, _id: int, buy: bool, amount: str, price: str) -> None:
         self.wait_order_id.append(_id)
         _fetch_order = False
         try:
             if prm.MODE in ('T', 'TC'):
                 ts = time.time()
@@ -1300,15 +1314,18 @@
                     break
             self.message_log("Backtest *** order_book *** timeSeries ended")
 
     async def buffered_orders(self):
         exch_orders = []
         diff_id = set()
         restore = False
-        while self.operational_status:
+        while True:
+            if not self.operational_status:
+                await asyncio.sleep(HEARTBEAT)
+                continue
             try:
                 _orders = await self.send_request(self.stub.fetch_open_orders, mr.MarketRequest, symbol=self.symbol)
                 if _orders is None:
                     raise UserWarning("Can't fetch open orders")
 
                 self.rate_limiter = max(self.rate_limiter, _orders.rate_limiter)
 
@@ -1346,17 +1363,16 @@
                         json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
                     self.start_collect = True
                 exch_orders.clear()
                 diff_id.clear()
                 self.last_state = None
                 restore = False
 
-            except asyncio.CancelledError:
-                # print("buffered_orders.Cancelled")
-                self.operational_status = False
+            except (asyncio.CancelledError, KeyboardInterrupt):
+                break
             except UserWarning as ex_2:
                 self.message_log(f"Exception buffered_orders 2: {ex_2}", log_level=logging.WARNING)
                 restore = True
             except GRPCError as ex_3:
                 status_code = ex_3.status
                 self.message_log(f"Exception buffered_orders 3: {status_code.name}, {ex_3.message}",
                                  log_level=logging.WARNING, color=Style.B_RED, tlg=True)
@@ -1386,31 +1402,30 @@
                 res = await self.send_request(self.stub.check_stream, mr.MarketRequest, symbol=self.symbol)
             except Exception as ex_1:
                 self.message_log(f"Exception on Check WSS: {ex_1}", log_level=logging.WARNING)
             else:
                 if res.success:
                     self.operational_status = True
 
-    def tasks_manage(self, coro):
-        _t = asyncio.create_task(coro)
+    def tasks_manage(self, coro, name=None, add_done_callback=True):
+        _t = asyncio.create_task(coro, name=name)
         self.tasks.add(_t)
-        _t.add_done_callback(self.tasks.discard)
+        if add_done_callback:
+            _t.add_done_callback(self.tasks.discard)
 
     async def wss_declare(self):
         # Market stream
-        self.tasks_manage(self.on_ticker_update())
+        self.tasks_manage(self.on_ticker_update(), name='wss')
         await self.buffered_candle()
-        self.tasks_manage(self.on_order_book_update())
+        self.tasks_manage(self.on_order_book_update(), name='wss')
         if prm.MODE in ('T', 'TC'):
             # User Stream
-            self.tasks_manage(self.on_funds_update())
-            self.tasks_manage(self.on_order_update())
-            self.tasks_manage(self.on_balance_update())
-            if prm.MODE == 'TC':
-                self.tasks_manage(self.backtest_control())
+            self.tasks_manage(self.on_funds_update(), name='wss')
+            self.tasks_manage(self.on_order_update(), name='wss')
+            self.tasks_manage(self.on_balance_update(), name='wss')
 
     async def wss_init(self, update_max_queue_size=False):
         if self.client_id:
             self.message_log(f"Init WSS, client_id: {self.client_id}")
             self.task_cancel()
             await self.wss_declare()
             # WSS start
@@ -1425,22 +1440,22 @@
                                         market_stream_count=5,
                                         update_max_queue_size=update_max_queue_size)
             except UserWarning:
                 self.message_log("Start WSS failed, retry", log_level=logging.WARNING)
                 self.wss_fire_up = True
             else:
                 self.wss_fire_up = False
+                await self.wait_wss_init()
         else:
             self.message_log("Init WSS failed, retry", log_level=logging.WARNING)
             await asyncio.sleep(random.randint(HEARTBEAT, HEARTBEAT * 5))
             self.wss_fire_up = True
 
     def task_cancel(self):
-        [task.cancel() for task in self.tasks if not task.done()]
-        self.tasks.clear()
+        [task.cancel() for task in self.tasks if not task.done() and task.get_name() == 'wss']
 
     async def main(self, _symbol):
         restore_state = None
         last_state = {}
         active_orders = []
         exch_orders_ids = []
         try:
@@ -1648,23 +1663,24 @@
                         self.start_collect = True
                     else:
                         self.init()
                         self.start()
 
             if prm.MODE in ('T', 'TC'):
                 await self.wss_init()
-                await self.wait_wss_init()
                 self.tasks_manage(save_to_csv())
-                self.tasks_manage(self.buffered_orders())
+                self.tasks_manage(self.buffered_orders(), add_done_callback=False)
                 if self.session.client.real_market:
-                    self.tasks_manage(self.save_asset())
+                    self.tasks_manage(self.save_asset(), add_done_callback=False)
+                if prm.MODE == 'TC':
+                    self.tasks_manage(self.backtest_control(), add_done_callback=False)
                 if not restore_state:
                     self.start()
 
-            self.tasks_manage(self.heartbeat(self.session))
+            self.tasks_manage(self.heartbeat(self.session), add_done_callback=False)
 
         except (KeyboardInterrupt, SystemExit):
             # noinspection PyProtectedMember, PyUnresolvedReferences
             os._exit(1)
 
     # region AbstractMethod
     @abstractmethod
```

### Comparing `martin_binance-3.0.5/martin_binance/telegram_utils.py` & `martin_binance-3.0.6/martin_binance/telegram_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/templates/cli_0_BTCUSDT.py` & `martin_binance-3.0.6/martin_binance/templates/cli_0_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/templates/cli_1_BTCUSDT.py` & `martin_binance-3.0.6/martin_binance/templates/cli_1_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py` & `martin_binance-3.0.6/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/templates/cli_3_BTCUSDT.py` & `martin_binance-3.0.6/martin_binance/templates/cli_3_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/templates/funds_rate.db` & `martin_binance-3.0.6/martin_binance/templates/funds_rate.db`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/templates/ms_cfg.toml` & `martin_binance-3.0.6/martin_binance/templates/ms_cfg.toml`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/martin_binance/templates/trial_params.json` & `martin_binance-3.0.6/martin_binance/templates/trial_params.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.5/pyproject.toml` & `martin_binance-3.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 
 dependencies = [
-    "exchanges-wrapper==2.1.10",
+    "exchanges-wrapper==2.1.11",
     "jsonpickle==3.0.2",
     "psutil==5.9.6",
     "requests==2.31.0",
     "libtmux==0.23.2",
     "colorama==0.4.6",
     "prometheus-client==0.18.0",
     "optuna==3.4.0",
```

### Comparing `martin_binance-3.0.5/PKG-INFO` & `martin_binance-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 3.0.5
+Version: 3.0.6
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==2.1.10
+Requires-Dist: exchanges-wrapper==2.1.11
 Requires-Dist: jsonpickle==3.0.2
 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: libtmux==0.23.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: prometheus-client==0.18.0
 Requires-Dist: optuna==3.4.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 3.0.5 Summary: Free trading
+Metadata-Version: 2.1 Name: martin-binance Version: 3.0.6 Summary: Free trading
 system for Binance SPOT API Author-email: Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist: exchanges-
-wrapper==2.1.10 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
+wrapper==2.1.11 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0 Requires-Dist: libtmux==0.23.2 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.18.0 Requires-Dist:
 optuna==3.4.0 Requires-Dist: plotly==5.18.0 Requires-Dist: pandas==2.1.2
 Requires-Dist: dash>=2.15.0 Requires-Dist: future==0.18.3 Requires-Dist:
 inquirer==3.1.3 Requires-Dist: scikit-learn==1.3.2 Requires-Dist: tqdm==4.66.1
 Requires-Dist: ujson~=5.9.0 Requires-Dist: orjson~=3.9.15 Requires-Dist:
 pyarrow~=14.0.2 Requires-Dist: shortuuid~=1.0.11 Requires-Dist: numpy~=1.23.4
```

