# Comparing `tmp/odp_sdk-0.4.6.tar.gz` & `tmp/odp_sdk-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_sdk-0.4.6.tar", max compression
+gzip compressed data, was "odp_sdk-0.4.7.tar", max compression
```

## Comparing `odp_sdk-0.4.6.tar` & `odp_sdk-0.4.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1052 2024-03-18 11:15:46.721698 odp_sdk-0.4.6/LICENSE
--rw-r--r--   0        0        0      836 2024-03-18 11:15:46.721698 odp_sdk-0.4.6/README.md
--rw-r--r--   0        0        0       30 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/__init__.py
--rw-r--r--   0        0        0    12249 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/auth.py
--rw-r--r--   0        0        0     1941 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/client.py
--rw-r--r--   0        0        0       84 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/dto/__init__.py
--rw-r--r--   0        0        0      857 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/dto/file_dto.py
--rw-r--r--   0        0        0     1938 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/dto/resource_dto.py
--rw-r--r--   0        0        0      846 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/dto/table_spec.py
--rw-r--r--   0        0        0     1391 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/dto/tabular_store.py
--rw-r--r--   0        0        0     1012 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/exc.py
--rw-r--r--   0        0        0     7724 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/http_client.py
--rw-r--r--   0        0        0     8303 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/raw_storage_client.py
--rw-r--r--   0        0        0     6759 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/resource_client.py
--rw-r--r--   0        0        0    17200 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/tabular_storage_client.py
--rw-r--r--   0        0        0        0 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1789 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/utils/json.py
--rw-r--r--   0        0        0     4249 2024-03-18 11:15:46.725698 odp_sdk-0.4.6/odp_sdk/utils/ndjson.py
--rw-r--r--   0        0        0     1172 2024-03-18 11:16:00.449615 odp_sdk-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 odp_sdk-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-04-19 12:03:58.957894 odp_sdk-0.4.7/LICENSE
+-rw-r--r--   0        0        0      836 2024-04-19 12:03:58.957894 odp_sdk-0.4.7/README.md
+-rw-r--r--   0        0        0       30 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/__init__.py
+-rw-r--r--   0        0        0    12698 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/auth.py
+-rw-r--r--   0        0        0     1941 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/client.py
+-rw-r--r--   0        0        0       84 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/dto/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/dto/file_dto.py
+-rw-r--r--   0        0        0     1938 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/dto/resource_dto.py
+-rw-r--r--   0        0        0      846 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/dto/table_spec.py
+-rw-r--r--   0        0        0     1391 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/dto/tabular_store.py
+-rw-r--r--   0        0        0     1012 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/exc.py
+-rw-r--r--   0        0        0     7933 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/http_client.py
+-rw-r--r--   0        0        0     8303 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/raw_storage_client.py
+-rw-r--r--   0        0        0     6759 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/resource_client.py
+-rw-r--r--   0        0        0    17200 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/tabular_storage_client.py
+-rw-r--r--   0        0        0       39 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1789 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/utils/json.py
+-rw-r--r--   0        0        0     4249 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/utils/ndjson.py
+-rw-r--r--   0        0        0      437 2024-04-19 12:03:58.961894 odp_sdk-0.4.7/odp_sdk/utils/package_utils.py
+-rw-r--r--   0        0        0     1189 2024-04-19 12:04:18.170056 odp_sdk-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 odp_sdk-0.4.7/PKG-INFO
```

### Comparing `odp_sdk-0.4.6/LICENSE` & `odp_sdk-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/README.md` & `odp_sdk-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/auth.py` & `odp_sdk-0.4.7/odp_sdk/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,24 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicNumbers
 from pydantic import BaseModel, PrivateAttr, SecretStr
 from requests.auth import AuthBase
 
 from .exc import OdpAuthError
+from .utils import get_version
 
 LOG = logging.getLogger(__name__)
 
 
 class TokenProvider(AuthBase, BaseModel, ABC):
     """Base class for token providers"""
 
+    user_agent: str = "odp-sdk/" + get_version()
+
     @abstractmethod
     def get_token(self) -> str:
         """Returns the token to be used for authentication
 
         Returns:
             str: The token to be used for authentication
 
@@ -46,28 +49,34 @@
 
 class OdpWorkspaceTokenProvider(TokenProvider):
     """Token provider for ODP workspaces"""
 
     token_uri: str = "http://localhost:8000/access_token"
     """Token endpoint."""
 
+    def __init__(self, **data):
+        super().__init__(**data)
+        self.user_agent = self.user_agent + " (Workspaces)"
+
     def get_token(self) -> str:
         res = requests.post(self.token_uri)
         res.raise_for_status()
 
         return "Bearer " + res.json()["token"]
 
 
 class HardcodedTokenProvider(TokenProvider):
-    _token: PrivateAttr()
     """Token provider for hardcoded tokens"""
 
+    _token: PrivateAttr()
+
     def __init__(self, token: str, **data):
         super().__init__(**data)
         self._token = token
+        self.user_agent = self.user_agent + " (Hardcoded)"
 
     def get_token(self) -> str:
         return self._token
 
 
 class JwtTokenProvider(TokenProvider, ABC):
     """Token provider for JWT tokens"""
@@ -243,14 +252,18 @@
 
     token_uri: str = "https://oceandataplatform.b2clogin.com/oceandataplatform.onmicrosoft.com/b2c_1a_signup_signin_custom/oauth2/v2.0/token"  # noqa: E501
     """Token endpoint. Will default to 'https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token'"""
 
     jwks_uri: str = "https://oceandataplatform.b2clogin.com/oceandataplatform.onmicrosoft.com/b2c_1a_signup_signin_custom/discovery/v2.0/keys"  # noqa: E501
     """JWKS endpoint."""
 
+    def __init__(self, **data):
+        super().__init__(**data)
+        self.user_agent = self.user_agent + " (Azure)"
+
     def get_jwks_uri(self) -> str:
         return self.jwks_uri
 
     def authenticate(self) -> dict[str, str]:
         res = requests.post(
             self.token_uri,
             data={
@@ -302,14 +315,15 @@
         cache = msal_extensions.PersistedTokenCache(persistence)
 
         self._app = msal.PublicClientApplication(
             client_id=self.client_id.get_secret_value(),
             authority=self.authority,
             token_cache=cache,
         )
+        self.user_agent = self.user_agent + " (Interactive)"
 
     def get_jwks_uri(self) -> str:
         return self.jwks_uri
 
     def authenticate(self) -> dict[str, str]:
         accounts = self._app.get_accounts()
         if accounts and len(accounts) == 1:
```

### Comparing `odp_sdk-0.4.6/odp_sdk/client.py` & `odp_sdk-0.4.7/odp_sdk/client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/dto/resource_dto.py` & `odp_sdk-0.4.7/odp_sdk/dto/resource_dto.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/dto/table_spec.py` & `odp_sdk-0.4.7/odp_sdk/dto/table_spec.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/dto/tabular_store.py` & `odp_sdk-0.4.7/odp_sdk/dto/tabular_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/exc.py` & `odp_sdk-0.4.7/odp_sdk/exc.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/http_client.py` & `odp_sdk-0.4.7/odp_sdk/http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .auth import TokenProvider
 from .exc import OdpForbiddenError, OdpUnauthorizedError
 
 
 class OdpHttpClient(BaseModel):
     base_url: str = "https://api.hubocean.earth"
     token_provider: TokenProvider
+    custom_user_agent: str = None
 
     @field_validator("base_url")
     @classmethod
     def _validate_url(cls, v: str) -> str:
         m = re.match(
             r"https?:\/\/(www\.|localhost)?[-a-zA-Z0-9@:%._\+~#=]"
             r"{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*|:\d+)",
@@ -225,14 +226,18 @@
         elif url.startswith(self.base_url):
             url = url[len(self.base_url) :]
             base_url = self.base_url
         else:
             base_url = ""
 
         headers = headers or {}
+        if self.custom_user_agent:
+            headers["User-Agent"] = self.custom_user_agent
+        else:
+            headers["User-Agent"] = self.token_provider.user_agent
 
         if isinstance(content, (dict, list)):
             body = json.dumps(content)
             headers["Content-Type"] = "application/json"
         elif isinstance(content, BaseModel):
             body = content.model_dump_json()
             headers["Content-Type"] = "application/json"
```

### Comparing `odp_sdk-0.4.6/odp_sdk/raw_storage_client.py` & `odp_sdk-0.4.7/odp_sdk/raw_storage_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/resource_client.py` & `odp_sdk-0.4.7/odp_sdk/resource_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/tabular_storage_client.py` & `odp_sdk-0.4.7/odp_sdk/tabular_storage_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/utils/json.py` & `odp_sdk-0.4.7/odp_sdk/utils/json.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/odp_sdk/utils/ndjson.py` & `odp_sdk-0.4.7/odp_sdk/utils/ndjson.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.6/pyproject.toml` & `odp_sdk-0.4.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "odp-sdk"
-version = "0.4.6"
+version = "0.4.7"
 description = "ODP Python SDK"
 authors = ["Thomas Li Fredriksen <thomas.fredriksen@oceandata.earth>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "odp_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.4.2"
 cryptography = ">=41.0.5,<43.0.0"
 pyjwt = "^2.8.0"
 msal = "^1.24.1"
 msal-extensions = "^1.1.0"
 pandas = { version = "^2.1.4", optional = true}
+tomli = "^2.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 coverage = "^7.3.2"
 flake8-pyproject = "^1.2.2"
 responses = "^0.23.1"
```

### Comparing `odp_sdk-0.4.6/PKG-INFO` & `odp_sdk-0.4.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp-sdk
-Version: 0.4.6
+Version: 0.4.7
 Summary: ODP Python SDK
 License: MIT
 Author: Thomas Li Fredriksen
 Author-email: thomas.fredriksen@oceandata.earth
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Provides-Extra: pandas
 Requires-Dist: cryptography (>=41.0.5,<43.0.0)
 Requires-Dist: msal (>=1.24.1,<2.0.0)
 Requires-Dist: msal-extensions (>=1.1.0,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0) ; extra == "pandas"
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://www.oceandata.earth/">
     <img src="assets/ODP-SDK.png" alt="ODP SDK logo" title="ODP" align="right" height="100" />
 </a>
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: odp-sdk Version: 0.4.6 Summary: ODP Python SDK
+Metadata-Version: 2.1 Name: odp-sdk Version: 0.4.7 Summary: ODP Python SDK
 License: MIT Author: Thomas Li Fredriksen Author-email:
 thomas.fredriksen@oceandata.earth Requires-Python: >=3.10,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: pandas Requires-Dist: cryptography
 (>=41.0.5,<43.0.0) Requires-Dist: msal (>=1.24.1,<2.0.0) Requires-Dist: msal-
 extensions (>=1.1.0,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) ; extra ==
 "pandas" Requires-Dist: pydantic (>=2.4.2,<3.0.0) Requires-Dist: pyjwt
-(>=2.8.0,<3.0.0) Description-Content-Type: text/markdown _[_O_D_P_ _S_D_K_ _l_o_g_o_]# ODP
-Python SDK Connect to the Ocean Data Platform with Python through the Python
-SDK. Download queried ocean data easily and efficiently into data frames, for
-easy exploring and further processing in your data science project. ##
-Documentation [WIP] ## Installation Use the package manager [pip](https://
-pip.pypa.io/en/stable/) to install the Ocean Data Platform Python SDK. ```bash
-pip3 install odp_sdk ``` ## Usage *Note: Accessing the Ocean Data Platform
-requires an authorzed account. Contact ODP to require one.* ```python from
-odp_sdk.client import OdpClient client = OdpClient() for item in
-client.catalog.list(): print(item) ``` Examples can be found in /examples.
+(>=2.8.0,<3.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0) Description-Content-
+Type: text/markdown _[_O_D_P_ _S_D_K_ _l_o_g_o_]# ODP Python SDK Connect to the Ocean Data
+Platform with Python through the Python SDK. Download queried ocean data easily
+and efficiently into data frames, for easy exploring and further processing in
+your data science project. ## Documentation [WIP] ## Installation Use the
+package manager [pip](https://pip.pypa.io/en/stable/) to install the Ocean Data
+Platform Python SDK. ```bash pip3 install odp_sdk ``` ## Usage *Note: Accessing
+the Ocean Data Platform requires an authorzed account. Contact ODP to require
+one.* ```python from odp_sdk.client import OdpClient client = OdpClient() for
+item in client.catalog.list(): print(item) ``` Examples can be found in /
+examples.
```

