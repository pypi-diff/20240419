# Comparing `tmp/cognitojwt-1.4.0.tar.gz` & `tmp/cognitojwt-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cognitojwt-1.4.0.tar", last modified: Mon Jun  7 11:55:06 2021, max compression
+gzip compressed data, was "dist/cognitojwt-1.4.1.tar", last modified: Mon Jun  7 15:27:36 2021, max compression
```

## Comparing `cognitojwt-1.4.0.tar` & `cognitojwt-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2289 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1596 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt/
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/cognitojwt/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/cognitojwt/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1082 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/cognitojwt/token_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/cognitojwt/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1867 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/cognitojwt/jwt_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2074 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/cognitojwt/jwt_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1046 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2021-06-07 11:54:36.000000 cognitojwt-1.4.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2289 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      373 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-06-07 11:55:06.000000 cognitojwt-1.4.0/cognitojwt.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2672 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1979 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       91 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/cognitojwt/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/cognitojwt/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/cognitojwt/token_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/cognitojwt/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1928 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/cognitojwt/jwt_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2135 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/cognitojwt/jwt_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1046 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2021-06-07 15:27:05.000000 cognitojwt-1.4.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2672 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      373 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      164 2021-06-07 15:27:36.000000 cognitojwt-1.4.1/cognitojwt.egg-info/requires.txt
```

### Comparing `cognitojwt-1.4.0/PKG-INFO` & `cognitojwt-1.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitojwt
-Version: 1.4.0
+Version: 1.4.1
 Summary: Decode and verify Amazon Cognito JWT tokens
 Home-page: http://github.com/borisrozumnuk/cognitojwt
 Author: Boris Rozumniuk
 Author-email: borisrozumnuk@gmail.com
 License: MIT
 Keywords: Amazon Cognito JWT
 Platform: Any
@@ -63,8 +63,21 @@
 )
 
 ```
 
 Note: if the application is deployed inside a private vpc without internet gateway, the application will not be able to download the JWKS file.
 In this case set the `AWS_COGNITO_JWKS_PATH` environment variable referencing the absolute or relative path of the jwks.json file.
 
+It is possible to allow multiple app client ids by passing the value as a Container instance such as a list or tuple:
+```python
+ALLOWED_CLIENT_IDS = ('client_one', 'client_two')
+
+verified_claims: dict = cognitojwt.decode(
+    id_token,
+    REGION,
+    USERPOOL_ID,
+    app_client_id=ALLOWED_CLIENT_IDS,
+    testmode=True  # Disable token expiration check for testing purposes
+)
+```
+
```

### Comparing `cognitojwt-1.4.0/README.md` & `cognitojwt-1.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,7 +40,20 @@
     testmode=True  # Disable token expiration check for testing purposes
 )
 
 ```
 
 Note: if the application is deployed inside a private vpc without internet gateway, the application will not be able to download the JWKS file.
 In this case set the `AWS_COGNITO_JWKS_PATH` environment variable referencing the absolute or relative path of the jwks.json file.
+
+It is possible to allow multiple app client ids by passing the value as a Container instance such as a list or tuple:
+```python
+ALLOWED_CLIENT_IDS = ('client_one', 'client_two')
+
+verified_claims: dict = cognitojwt.decode(
+    id_token,
+    REGION,
+    USERPOOL_ID,
+    app_client_id=ALLOWED_CLIENT_IDS,
+    testmode=True  # Disable token expiration check for testing purposes
+)
+```
```

### Comparing `cognitojwt-1.4.0/cognitojwt/token_utils.py` & `cognitojwt-1.4.1/cognitojwt/token_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
+from typing import Dict, Union, Container
 
-from typing import Dict
 from jose import jwt
 
 from .exceptions import CognitoJWTException
 
 
 CLIENT_ID_KEYS: Dict[str, str] = {
     'access': 'client_id',
@@ -21,22 +21,25 @@
 
 
 def check_expired(exp: int, testmode: bool = False) -> None:
     if time.time() > exp and not testmode:
         raise CognitoJWTException('Token is expired')
 
 
-def check_client_id(claims: Dict, app_client_id: str) -> None:
+def check_client_id(claims: Dict, app_client_id: Union[str, Container[str]]) -> None:
     token_use = claims['token_use']
 
     client_id_key: str = CLIENT_ID_KEYS.get(token_use)
     if not client_id_key:
         raise CognitoJWTException(f'Invalid token_use: {token_use}. Valid values: {list(CLIENT_ID_KEYS.keys())}')
 
-    if claims[client_id_key] != app_client_id:
+    if isinstance(app_client_id, str):
+        app_client_id = (app_client_id,)
+
+    if claims[client_id_key] not in app_client_id:
         raise CognitoJWTException('Token was not issued for this client id audience')
 
 
 __all__ = [
     'get_unverified_headers',
     'get_unverified_claims',
     'check_expired',
```

### Comparing `cognitojwt-1.4.0/cognitojwt/jwt_sync.py` & `cognitojwt-1.4.1/cognitojwt/jwt_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 from functools import lru_cache
-from typing import List, Dict
+from typing import List, Dict, Optional, Union, Container
 import requests
 
 
 from jose import jwk
 from jose.utils import base64url_decode
 
 from .constants import PUBLIC_KEYS_URL_TEMPLATE
@@ -39,15 +39,15 @@
     return jwk.construct(key)
 
 
 def decode(
         token: str,
         region: str,
         userpool_id: str,
-        app_client_id: str = None,
+        app_client_id: Optional[Union[str, Container[str]]] = None,
         testmode: bool = False
 ) -> Dict:
     message, encoded_signature = str(token).rsplit('.', 1)
 
     decoded_signature = base64url_decode(encoded_signature.encode('utf-8'))
 
     public_key = get_public_key(token, region, userpool_id)
```

### Comparing `cognitojwt-1.4.0/cognitojwt/jwt_async.py` & `cognitojwt-1.4.1/cognitojwt/jwt_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import List, Dict
+from typing import List, Dict, Optional, Union, Container
 
 from aiofile import AIOFile
 import aiohttp
 from async_lru import alru_cache
 from jose import jwk
 from jose.utils import base64url_decode
 
@@ -41,15 +41,15 @@
     return jwk.construct(key)
 
 
 async def decode_async(
         token: str,
         region: str,
         userpool_id: str,
-        app_client_id: str = None,
+        app_client_id: Optional[Union[str, Container[str]]] = None,
         testmode: bool = False
 ) -> Dict:
     message, encoded_signature = str(token).rsplit('.', 1)
 
     decoded_signature = base64url_decode(encoded_signature.encode('utf-8'))
 
     public_key = await get_public_key_async(token, region, userpool_id)
```

### Comparing `cognitojwt-1.4.0/LICENSE` & `cognitojwt-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitojwt-1.4.0/setup.py` & `cognitojwt-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     'pytest-asyncio==0.12.0',
     'attrs==19.1.0'
 }
 
 
 setup(
     name='cognitojwt',
-    version='1.4.0',
+    version='1.4.1',
     description='Decode and verify Amazon Cognito JWT tokens',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/borisrozumnuk/cognitojwt',
     author='Boris Rozumniuk',
     author_email='borisrozumnuk@gmail.com',
     license='MIT',
```

### Comparing `cognitojwt-1.4.0/cognitojwt.egg-info/PKG-INFO` & `cognitojwt-1.4.1/cognitojwt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitojwt
-Version: 1.4.0
+Version: 1.4.1
 Summary: Decode and verify Amazon Cognito JWT tokens
 Home-page: http://github.com/borisrozumnuk/cognitojwt
 Author: Boris Rozumniuk
 Author-email: borisrozumnuk@gmail.com
 License: MIT
 Keywords: Amazon Cognito JWT
 Platform: Any
@@ -63,8 +63,21 @@
 )
 
 ```
 
 Note: if the application is deployed inside a private vpc without internet gateway, the application will not be able to download the JWKS file.
 In this case set the `AWS_COGNITO_JWKS_PATH` environment variable referencing the absolute or relative path of the jwks.json file.
 
+It is possible to allow multiple app client ids by passing the value as a Container instance such as a list or tuple:
+```python
+ALLOWED_CLIENT_IDS = ('client_one', 'client_two')
+
+verified_claims: dict = cognitojwt.decode(
+    id_token,
+    REGION,
+    USERPOOL_ID,
+    app_client_id=ALLOWED_CLIENT_IDS,
+    testmode=True  # Disable token expiration check for testing purposes
+)
+```
+
```

