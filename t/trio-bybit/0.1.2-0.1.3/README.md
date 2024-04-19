# Comparing `tmp/trio_bybit-0.1.2.tar.gz` & `tmp/trio_bybit-0.1.3.tar.gz`

## Comparing `trio_bybit-0.1.2.tar` & `trio_bybit-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/pytest.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/tests/test_async_client.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/trio_bybit/__init__.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/trio_bybit/client.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/trio_bybit/helpers.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/README.md
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/pytest.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/tests/test_async_client.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/tests/test_streams.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/README.md
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.3/PKG-INFO
```

### Comparing `trio_bybit-0.1.2/tests/test_async_client.py` & `trio_bybit-0.1.3/tests/test_async_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,19 +23,27 @@
         assert symbol_info["result"]["category"] == "linear"
         assert symbol_info["result"]["list"][0]["symbol"] == "BTCUSDT"
         assert symbol_info["result"]["list"][0]["contractType"] == "LinearPerpetual"
         assert symbol_info["result"]["list"][0]["status"] == "Trading"
         assert symbol_info["result"]["list"][0]["baseCoin"] == "BTC"
         assert symbol_info["result"]["list"][0]["quoteCoin"] == "USDT"
 
+        orderbook = await client.get_orderbook(category="linear", symbol="BTCUSDT")
+        assert orderbook["retCode"] == 0
+        assert orderbook["retMsg"] == "OK"
+
 
 async def test_get_private():
     client = await AsyncClient.create(
         api_key=os.getenv("BYBIT_API_KEY"),
         api_secret=os.getenv("BYBIT_API_SECRET"),
+        # alternative_net="demo",
     )
 
     async with client:
         wallet = await client.get_wallet_balance(accountType="UNIFIED")
         assert wallet["retCode"] == 0
         assert wallet["retMsg"] == "OK"
         assert wallet["result"]["list"][0]["accountType"] == "UNIFIED"
+        position = await client.get_position_info(category="linear", settleCoin="USDT")
+        assert position["retCode"] == 0
+        assert position["retMsg"] == "OK"
```

### Comparing `trio_bybit-0.1.2/tests/test_streams.py` & `trio_bybit-0.1.3/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.2/trio_bybit/client.py` & `trio_bybit-0.1.3/trio_bybit/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,55 +7,63 @@
 
 import orjson
 
 from .exceptions import BybitAPIException, BybitRequestException
 
 
 class BaseClient:
-    API_URL = "https://api.bybit.com"
-    # SECONDARY_API_URL = "https://api.bytick.com"
-    # TEST_NET = "https://api-testnet.bybit.com"
+    API_URL = "https://api.bybit.com/"
+    # SECONDARY_API_URL = "https://api.bytick.com/"
+    TEST_NET_API_URL = "https://api-testnet.bybit.com/"
+    DEMO_NET_API_URL = "https://api-demo.bybit.com/"
     API_VERSION = "v5"
 
     REQUEST_TIMEOUT: float = 5
 
     def __init__(
         self,
         api_key: str | None = None,
         api_secret: str | None = None,
         receive_window: int = 5000,
         sign_style: str = "HMAC",
+        alternative_net: str = "",
     ):
         """API Client constructor
-
         :param api_key: Api Key
-        :type api_key: str.
         :param api_secret: Api Secret
-        :type api_secret: str.
+        :param receive_window: Receive Window
+        :param sign_style: Sign Style. Default HMAC. RSA not implemented yet.
+        :param alternative_net: Alternative network. Default empty to use mainnet. Choices: "test", "demo"
         """
         self.API_KEY = api_key
         self.API_SECRET = api_secret
         self.response = None
         self.receive_window = receive_window
         self.sign_style = sign_style  # RSA not implemented yet
         self.timestamp_offset = 0
-        self.base_url = self.API_URL + self.API_VERSION + "/"
+        if alternative_net == "test":
+            self.base = self.TEST_NET_API_URL
+        elif alternative_net == "demo":
+            self.base = self.DEMO_NET_API_URL
+        else:
+            self.base = self.API_URL
+        self.base_url = self.base + self.API_VERSION + "/"
         self.session = httpx.AsyncClient(http2=True, base_url=self.base_url)
 
     def _get_headers(self, timestamp_milli: int, signed=False, timeout: int = None) -> dict:
         headers = {
             "X-BAPI-TIMESTAMP": str(timestamp_milli),
             "X-BAPI-RECV-WINDOW": str(self.receive_window),
         }
         if signed:
             headers["X-BAPI-API-KEY"] = self.API_KEY
         return headers
 
     def _create_api_uri(self, path: str) -> httpx.URL:
-        return httpx.URL(os.path.join(self.API_URL, self.API_VERSION, path))
+        return httpx.URL(os.path.join(self.base, self.API_VERSION, path))
 
     def _generate_signature(self, request: httpx.Request, timestamp_milli: int) -> str:
         if request.method == "GET":
             prepared_str = str(timestamp_milli) + self.API_KEY + str(self.receive_window) + str(request.url.params)
         else:
             prepared_str = (
                 str(timestamp_milli) + self.API_KEY + str(self.receive_window) + request.content.decode("utf-8")
@@ -76,25 +84,31 @@
 
 
 class AsyncClient(BaseClient):
     def __init__(
         self,
         api_key: str | None = None,
         api_secret: str | None = None,
+        receive_window: int = 5000,
+        sign_style: str = "HMAC",
+        alternative_net: str = "",
     ):
-        super().__init__(api_key, api_secret)
+        super().__init__(api_key, api_secret, receive_window, sign_style, alternative_net)
         self.session: httpx.AsyncClient = httpx.AsyncClient(http2=True)
 
     @classmethod
     async def create(
         cls,
         api_key: str | None = None,
         api_secret: str | None = None,
+        receive_window: int = 5000,
+        sign_style: str = "HMAC",
+        alternative_net: str = "",
     ) -> "AsyncClient":
-        self = cls(api_key, api_secret)
+        self = cls(api_key, api_secret, receive_window, sign_style, alternative_net)
 
         try:
             # calculate timestamp offset between local and coinex server
             res = await self.get_server_time()
             self.timestamp_offset = 1000 * (int(res["result"]["timeSecond"]) - int(time.time()))
 
             return self
```

### Comparing `trio_bybit-0.1.2/trio_bybit/exceptions.py` & `trio_bybit-0.1.3/trio_bybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.2/trio_bybit/helpers.py` & `trio_bybit-0.1.3/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.2/trio_bybit/streams.py` & `trio_bybit-0.1.3/trio_bybit/streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.2/.gitignore` & `trio_bybit-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.2/LICENSE` & `trio_bybit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.2/README.md` & `trio_bybit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.2/pyproject.toml` & `trio_bybit-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trio-bybit"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.0",
     "httpx[http2]>=0.27.0",
```

### Comparing `trio_bybit-0.1.2/PKG-INFO` & `trio_bybit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
```

