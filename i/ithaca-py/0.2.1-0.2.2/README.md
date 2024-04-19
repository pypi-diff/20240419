# Comparing `tmp/ithaca_py-0.2.1.tar.gz` & `tmp/ithaca_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.2.1.tar", max compression
+gzip compressed data, was "ithaca_py-0.2.2.tar", max compression
```

## Comparing `ithaca_py-0.2.1.tar` & `ithaca_py-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-04-12 05:58:28.073315 ithaca_py-0.2.1/README.md
--rw-r--r--   0        0        0     5147 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/calculation.py
--rw-r--r--   0        0        0     3206 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/market.py
--rw-r--r--   0        0        0     6650 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/protocol.py
--rw-r--r--   0        0        0     2210 2024-04-12 05:58:28.077315 ithaca_py-0.2.1/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-04-12 05:58:28.081315 ithaca_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/README.md
+-rw-r--r--   0        0        0     5147 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/calculation.py
+-rw-r--r--   0        0        0     3206 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/market.py
+-rw-r--r--   0        0        0     7370 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/protocol.py
+-rw-r--r--   0        0        0     2210 2024-04-19 12:36:32.430024 ithaca_py-0.2.2/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-04-19 12:36:32.430024 ithaca_py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.2/PKG-INFO
```

### Comparing `ithaca_py-0.2.1/README.md` & `ithaca_py-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/__init__.py` & `ithaca_py-0.2.2/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/analytics.py` & `ithaca_py-0.2.2/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/auth.py` & `ithaca_py-0.2.2/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/calculation.py` & `ithaca_py-0.2.2/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/client.py` & `ithaca_py-0.2.2/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/constants.py` & `ithaca_py-0.2.2/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/fundlock.py` & `ithaca_py-0.2.2/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/market.py` & `ithaca_py-0.2.2/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/orders.py` & `ithaca_py-0.2.2/ithaca/orders.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Orders Module."""
-
+from collections import namedtuple
 from datetime import datetime, timezone
 
 
 class Orders:
     """Orders class."""
 
+    TIME_IN_FORCE_OPTIONS = ["DAY", "GOOD_TILL_CANCEL", "IMMEDIATE_OR_CANCEL", "GOOD_TILL_DATE", "AT_AUCTION_ONLY"]
+    OrderInfo = namedtuple('OrderInfo', 'legs price time_in_force order_descr client_order_id',
+                           defaults=("GOOD_TILL_CANCEL", "", None))
+
     def __init__(self, parent):
         """Class constructor."""
         self.parent = parent
 
     def create_client_order_id(self, value=101) -> int:
         """Create a 'random' client order id."""
         return int(
@@ -122,28 +126,31 @@
         res = self.parent.post("/clientapi/newOrder", json=body)
 
         try:
             return {**res, "clientOrderId": client_order_id}
         except TypeError:
             return {"result": "ERROR", "clientOrderId": client_order_id}
 
-    def new_orders(self, orders, order_descr=""):
+    def new_orders(self, orders):
         """Send new orders request to Ithaca backend."""
         payload = []
-        for legs, price,client_order_id in orders:
-            legs = sorted(legs, key=lambda x: x[0])
-            if client_order_id is None:
-                client_order_id = self.create_client_order_id()
+        for order_info in orders:
+            order_info = self.OrderInfo(*order_info)
+            time_in_force = order_info.time_in_force if self._is_time_in_force_valid(order_info.time_in_force) else "GOOD_TILL_CANCEL"
+            legs = sorted(order_info.legs, key=lambda x: x[0])
+            price = order_info.price
+            client_order_id = order_info.client_order_id if order_info.client_order_id else self.create_client_order_id()
+            order_descr = order_info.order_descr
 
             order = {
                 "clientOrderId": client_order_id,
                 "totalNetPrice": f"{price:.4f}",
                 "legs": legs,
                 "orderType": "LIMIT",
-                "timeInForce": "GOOD_TILL_CANCEL",
+                "timeInForce": time_in_force,
                 "clientEthAddress": self.parent.address.lower(),
                 "singlePrice": True,
             }
 
             signature = self.sign_order(order)
             del order["singlePrice"]
 
@@ -180,7 +187,12 @@
             "clientOrderId": client_order_id,
         }
         return self.parent.post("/clientapi/orderCancel", json=body)
 
     def order_cancel_all(self):
         """Cancel all orders."""
         return self.parent.post("/clientapi/allOrdersCancel")
+
+    def _is_time_in_force_valid(self, value):
+        if value in self.TIME_IN_FORCE_OPTIONS:
+            return True
+        return False
```

### Comparing `ithaca_py-0.2.1/ithaca/protocol.py` & `ithaca_py-0.2.2/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/ithaca/socket.py` & `ithaca_py-0.2.2/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.1/pyproject.toml` & `ithaca_py-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.2.1"
+version = "0.2.2"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.2.1/PKG-INFO` & `ithaca_py-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

