# Comparing `tmp/kitetrader-2.1.0.tar.gz` & `tmp/kitetrader-2.2.0.tar.gz`

## Comparing `kitetrader-2.1.0.tar` & `kitetrader-2.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 kitetrader-2.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kitetrader-2.1.0/src/__init__.py
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 kitetrader-2.1.0/src/kitetrader/Kite.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kitetrader-2.1.0/src/kitetrader/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kitetrader-2.1.0/tests/Dockerfile
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 kitetrader-2.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kitetrader-2.1.0/LICENSE
--rw-r--r--   0        0        0    11172 2020-02-02 00:00:00.000000 kitetrader-2.1.0/README.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 kitetrader-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 kitetrader-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 kitetrader-2.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kitetrader-2.2.0/src/__init__.py
+-rw-r--r--   0        0        0    15207 2020-02-02 00:00:00.000000 kitetrader-2.2.0/src/kitetrader/Kite.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kitetrader-2.2.0/src/kitetrader/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kitetrader-2.2.0/tests/Dockerfile
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 kitetrader-2.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kitetrader-2.2.0/LICENSE
+-rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 kitetrader-2.2.0/README.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 kitetrader-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 kitetrader-2.2.0/PKG-INFO
```

### Comparing `kitetrader-2.1.0/.github/workflows/python-publish.yml` & `kitetrader-2.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kitetrader-2.1.0/src/kitetrader/Kite.py` & `kitetrader-2.2.0/src/kitetrader/Kite.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections.abc import Collection
 from typing import Optional, Union, Any
 from requests import Session
 from requests.exceptions import ReadTimeout
 from urllib3.util import Retry
 from requests.adapters import HTTPAdapter
 from pathlib import Path
-import pickle
 from mthrottle import Throttle
 from datetime import datetime
+import pickle, hashlib, logging
+
 
 throttle_config = {
     "quote": {
         "rps": 1,
     },
     "historical": {
         "rps": 3,
@@ -24,14 +25,23 @@
         "rps": 8,
     },
 }
 
 th = Throttle(throttle_config, 15)
 
 
+def configure_default_logger(name):
+    logging.basicConfig(
+        level=logging.INFO,
+        format="%(levelname)s: %(message)s",
+    )
+
+    return logging.getLogger(name)
+
+
 class Kite:
     """Unofficial implementation of Zerodha Kite api"""
 
     # Exchanges
     EXCHANGE_NSE = "NSE"
     EXCHANGE_BSE = "BSE"
     EXCHANGE_NFO = "NFO"
@@ -76,33 +86,53 @@
     MARGIN_EQUITY = "equity"
     MARGIN_COMMODITY = "commodity"
 
     # GTT order type
     GTT_TYPE_OCO = "two-leg"
     GTT_TYPE_SINGLE = "single"
 
+    # Status constants
+    STATUS_COMPLETE = "COMPLETE"
+    STATUS_REJECTED = "REJECTED"
+    STATUS_CANCELLED = "CANCELLED"
+
+    # GTT order status
+    GTT_STATUS_ACTIVE = "active"
+    GTT_STATUS_TRIGGERED = "triggered"
+    GTT_STATUS_DISABLED = "disabled"
+    GTT_STATUS_EXPIRED = "expired"
+    GTT_STATUS_CANCELLED = "cancelled"
+    GTT_STATUS_REJECTED = "rejected"
+    GTT_STATUS_DELETED = "deleted"
+
     base_dir = Path(__file__).parent
     base_url = "https://api.kite.trade"
     cookies = None
     config = None
 
     def __init__(
         self,
         user_id: Optional[str] = None,
         password: Optional[str] = None,
         twofa: Optional[str] = None,
         enctoken: Optional[str] = None,
+        access_token: Optional[str] = None,
+        api_key: Optional[str] = None,
+        api_secret: Optional[str] = None,
+        request_token: Optional[str] = None,
+        logger: Optional[logging.Logger] = None,
     ):
 
         self.cookie_path = self.base_dir / "kite_cookies"
 
         self.session = Session()
         self.session.headers.update({"X-Kite-version": "3"})
 
         self.enctoken = enctoken
+        self.access_token = access_token
 
         retries = Retry(
             total=None,
             connect=3,
             read=3,
             redirect=0,
             status=3,
@@ -110,35 +140,58 @@
             backoff_factor=0.1,
             status_forcelist=[502, 503, 504],
             raise_on_status=False,
         )
 
         self.session.mount("https://", HTTPAdapter(max_retries=retries))
 
+        self.log = logger if logger else configure_default_logger(__name__)
+
+        if self.enctoken:
+            return self._set_enc_token(self.enctoken)
+
+        if self.access_token:
+            if not api_key:
+                raise ValueError(
+                    "api_key is required, when access_token is passed"
+                )
+
+            return self._set_access_token(api_key, self.access_token)
+
         if self.cookie_path.exists():
             self.cookies = self._get_cookie()
 
             # get enctoken from cookies
             self.enctoken = self.cookies.get("enctoken")
 
-        if self.enctoken:
-            self.session.headers.update(
-                {"Authorization": f"enctoken {self.enctoken}"}
-            )
-        else:
-            # initiate login
-            self._authorize(user_id, password, twofa)
+            if self.enctoken:
+                return self._set_enc_token(self.enctoken)
+
+        # initiate login
+        self._authorize(
+            user_id, password, twofa, api_key, request_token, api_secret
+        )
 
     def __enter__(self):
         return self
 
     def __exit__(self, *_):
         self.session.close()
         return False
 
+    def _set_enc_token(self, token):
+        self.session.headers.update({"Authorization": f"enctoken {token}"})
+        self.log.info("Auth headers updated with enctoken")
+
+    def _set_access_token(self, api_key, token):
+        self.session.headers.update(
+            {"Authorization": f"token {api_key}:{token}"}
+        )
+        self.log.info("Auth headers updated with access_token")
+
     def close(self):
         """Close the Requests session"""
 
         self.session.close()
 
     def _get_cookie(self):
         """Load the pickle format cookie file"""
@@ -189,57 +242,85 @@
         raise ConnectionError(f"{hint} | {code}: {r.reason}")
 
     def _authorize(
         self,
         user_id: Optional[str] = None,
         password: Optional[str] = None,
         twofa: Optional[str] = None,
+        api_key: Optional[str] = None,
+        request_token: Optional[str] = None,
+        secret: Optional[str] = None,
     ):
         """Authenthicate the user"""
 
+        login_url = "https://kite.zerodha.com"
+
+        if request_token and secret:
+            # API LOGIN
+            if not api_key:
+                raise ValueError("No api_key provided during initialization")
+
+            checksum = hashlib.sha256(
+                f"{api_key}{request_token}{secret}".encode("utf-8")
+            ).hexdigest()
+
+            response = self._req(
+                f"{login_url}/session/token",
+                "POST",
+                payload={
+                    "api_key": api_key,
+                    "request_token": request_token,
+                    "checksum": checksum,
+                },
+                hint="API_LOGIN",
+            ).json()
+
+            self.access_token = response["access_token"]
+            self.log.info("KiteConnect login success")
+            return self._set_access_token(api_key, self.access_token)
+
+        # WEB LOGIN
         if not user_id:
             user_id = input("Enter User id\n> ")
 
         if not password:
             password = input("Enter Password\n> ")
 
-        base_url = "https://kite.zerodha.com"
-
         response = self._req(
-            f"{base_url}/api/login",
+            f"{login_url}/api/login",
             "POST",
             payload=dict(user_id=user_id, password=password),
-            hint="Login",
+            hint="WEB_LOGIN",
         ).json()
 
         request_id = response["data"]["request_id"]
         twofa_type = response["data"]["twofa_type"]
 
         if not twofa:
             twofa = input(f"Please enter {twofa_type} code\n> ")
 
         response = self._req(
-            f"{base_url}/api/twofa",
+            f"{login_url}/api/twofa",
             "POST",
             payload=dict(
                 user_id=user_id,
                 request_id=request_id,
                 twofa_value=twofa,
                 twofa_type=twofa_type,
                 skip_session="",
             ),
             hint="TwoFA",
         )
 
-        enctoken = response.cookies["enctoken"]
+        self.enctoken = response.cookies["enctoken"]
         self._set_cookie(response.cookies)
 
-        self.session.headers.update({"Authorization": f"enctoken {enctoken}"})
+        self._set_enc_token(self.enctoken)
 
-        print("Authorization Succces")
+        self.log.info("Web Login Success")
 
     def instruments(self, exchange: Optional[str] = None):
         """return a CSV dump of all tradable instruments"""
 
         th.check()
         url = f"{self.base_url}/instruments"
```

### Comparing `kitetrader-2.1.0/.gitignore` & `kitetrader-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kitetrader-2.1.0/LICENSE` & `kitetrader-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kitetrader-2.1.0/README.md` & `kitetrader-2.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,38 +27,75 @@
 
 # close the requests session
 kite.close()
 ```
 
 ## Login
 
-**Update v2.1.0**
+**Update v2.2.0 - 19th April 2024** - Support both KiteConnect login and Web login
 
-- You can pass the user_id, password and OTP during class initialization. This allows full automation of script for those requiring it. See #notes below for details.
+**For KiteConnect login:**
 
-On first initialization, Kite will check for user authentication. If no arguments are provided, the script prompts for username, password, and OTP.
+1. Pass the api_key, api_secret and request_token during initialization. Once authorized the `access_token` can be accessed as `kite.access_token`
 
-On successful login, an `enctoken` is generated and stored in a cookie file.
+```python
+kite = Kite(
+    api_key=credentials['api_key'],
+    api_secret=credentials['api_secret'],
+    request_token=credentials['request_token'],
+)
+
+# On successful authentication, save the kite.access_token to database or file
+# for future use
+print(kite.access_token)
+```
+
+2. On subsequent attempts, simply pass the `access_token` and `api_key`
+
+```python
+kite = Kite(
+    access_token=credentials["access_token"],
+    api_key=credentials["api_key"],
+)
+```
+
+**For Web Login:**
+
+1. Web login is the default, if no arguments are passed. It will start an interactive prompt requesting `user_id`, `password` and `twofa`.
 
-If the cookie file exists on subsequent initialization, the `enctoken` is reused, eliminating the need to log in again.
+```python
+# Interactive prompt
+kite = Kite()
 
-This method will logout all Kite web (browser) sessions. (You can continue to use the Kite Mobile App).
+# Once auth is completed, save the enctoken for later use
+print(kite.enctoken)
+```
+
+2. You may pass some or all three arguments. Any missing info, will need to be entered when prompted.
+
+```python
+kite = Kite(
+    user_id: credentials['user_id'],
+    password: credentials['password'],
+    twofa: twofa,
+)
+```
+
+3. On successful authorization, the enctoken is saved to a cookie file. On subsequent attempts, the `enctoken` is loaded from the cookie file.
 
-You can reuse the browser `enctoken`, passing it to Kite. This way, you can use Kite without getting logged out.
+4. Using the web login, will log you out of any Kite web browser sessions. You can reuse the browser `enctoken`, passing it to Kite. This way, you can use Kite Web, without getting logged out.
 
-`kite = Kite(enctoken='<token string>')`
+`kite = Kite(enctoken=credentials['enctoken'])`
 
 To access the browser `enctoken`, login to kite.zerodha.com and press `SHIFT + F9` to open the Storage inspector (On Firefox). You will find the info under cookies.
 
 ## NOTES
 
 - Hard coding password and credentials can be risky. Take appropriate measure to safeguard your credentials from accidental uploads or exposure on shared computers. Stick to defaults or use enctoken if unsure.
 
-- Starting `v1.1.0`, kitetrader no longer exits on error. You must handle the error appropriately.
-
 - Methods may raise the following errors:
   - A `RuntimeError` is raised if too many (>15) 429 reponse codes are returned.
   - A `TimeoutError` is raised if server takes too long to respond.
   - A `ConnectionError` is raised if:
     - Session expired
     - Bad request or invalid parameters
     - Internal server error
```

### Comparing `kitetrader-2.1.0/pyproject.toml` & `kitetrader-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kitetrader"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
   { name="Benny Thadikaran" },
 ]
 description = "Unofficial Python Client for Zerodha Kite"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kitetrader-2.1.0/PKG-INFO` & `kitetrader-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kitetrader
-Version: 2.1.0
+Version: 2.2.0
 Summary: Unofficial Python Client for Zerodha Kite
 Project-URL: Homepage, https://github.com/BennyThadikaran/Kite-Trader
 Project-URL: Bug Tracker, https://github.com/BennyThadikaran/Kite-Trader/issues
 Author: Benny Thadikaran
 License-File: LICENSE
 Keywords: algo-trading,historical-data,intraday-data,kiteconnect,stock-data,stock-market,zerodha,zerodha-kite
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -44,38 +44,75 @@
 
 # close the requests session
 kite.close()
 ```
 
 ## Login
 
-**Update v2.1.0**
+**Update v2.2.0 - 19th April 2024** - Support both KiteConnect login and Web login
 
-- You can pass the user_id, password and OTP during class initialization. This allows full automation of script for those requiring it. See #notes below for details.
+**For KiteConnect login:**
 
-On first initialization, Kite will check for user authentication. If no arguments are provided, the script prompts for username, password, and OTP.
+1. Pass the api_key, api_secret and request_token during initialization. Once authorized the `access_token` can be accessed as `kite.access_token`
 
-On successful login, an `enctoken` is generated and stored in a cookie file.
+```python
+kite = Kite(
+    api_key=credentials['api_key'],
+    api_secret=credentials['api_secret'],
+    request_token=credentials['request_token'],
+)
+
+# On successful authentication, save the kite.access_token to database or file
+# for future use
+print(kite.access_token)
+```
+
+2. On subsequent attempts, simply pass the `access_token` and `api_key`
 
-If the cookie file exists on subsequent initialization, the `enctoken` is reused, eliminating the need to log in again.
+```python
+kite = Kite(
+    access_token=credentials["access_token"],
+    api_key=credentials["api_key"],
+)
+```
 
-This method will logout all Kite web (browser) sessions. (You can continue to use the Kite Mobile App).
+**For Web Login:**
 
-You can reuse the browser `enctoken`, passing it to Kite. This way, you can use Kite without getting logged out.
+1. Web login is the default, if no arguments are passed. It will start an interactive prompt requesting `user_id`, `password` and `twofa`.
 
-`kite = Kite(enctoken='<token string>')`
+```python
+# Interactive prompt
+kite = Kite()
+
+# Once auth is completed, save the enctoken for later use
+print(kite.enctoken)
+```
+
+2. You may pass some or all three arguments. Any missing info, will need to be entered when prompted.
+
+```python
+kite = Kite(
+    user_id: credentials['user_id'],
+    password: credentials['password'],
+    twofa: twofa,
+)
+```
+
+3. On successful authorization, the enctoken is saved to a cookie file. On subsequent attempts, the `enctoken` is loaded from the cookie file.
+
+4. Using the web login, will log you out of any Kite web browser sessions. You can reuse the browser `enctoken`, passing it to Kite. This way, you can use Kite Web, without getting logged out.
+
+`kite = Kite(enctoken=credentials['enctoken'])`
 
 To access the browser `enctoken`, login to kite.zerodha.com and press `SHIFT + F9` to open the Storage inspector (On Firefox). You will find the info under cookies.
 
 ## NOTES
 
 - Hard coding password and credentials can be risky. Take appropriate measure to safeguard your credentials from accidental uploads or exposure on shared computers. Stick to defaults or use enctoken if unsure.
 
-- Starting `v1.1.0`, kitetrader no longer exits on error. You must handle the error appropriately.
-
 - Methods may raise the following errors:
   - A `RuntimeError` is raised if too many (>15) 429 reponse codes are returned.
   - A `TimeoutError` is raised if server takes too long to respond.
   - A `ConnectionError` is raised if:
     - Session expired
     - Bad request or invalid parameters
     - Internal server error
```

