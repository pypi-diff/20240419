# Comparing `tmp/Py-SPW-1.5.3.tar.gz` & `tmp/Py-SPW-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Py-SPW-1.5.3.tar", last modified: Wed Dec 13 21:29:54 2023, max compression
+gzip compressed data, was "/home/stepan/projects/spworlds/Py-SPW/dist/.tmp-wvgxggar/Py-SPW-2.0.0.tar", last modified: Fri Apr 19 20:35:33 2024, max compression
```

## Comparing `Py-SPW-1.5.3.tar` & `Py-SPW-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,45 @@
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-12-13 21:29:54.962476 Py-SPW-1.5.3/
--rwxrwxr-x   0 stepan    (1000) stepan    (1000)     1085 2023-05-09 10:37:44.000000 Py-SPW-1.5.3/LICENSE
--rw-r--r--   0 stepan    (1000) stepan    (1000)       58 2023-07-13 13:18:30.000000 Py-SPW-1.5.3/MANIFEST.in
--rw-r--r--   0 stepan    (1000) stepan    (1000)     1516 2023-12-13 21:29:54.962476 Py-SPW-1.5.3/PKG-INFO
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-12-13 21:29:54.961476 Py-SPW-1.5.3/Py_SPW.egg-info/
--rw-r--r--   0 stepan    (1000) stepan    (1000)     1516 2023-12-13 21:29:54.000000 Py-SPW-1.5.3/Py_SPW.egg-info/PKG-INFO
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      285 2023-12-13 21:29:54.000000 Py-SPW-1.5.3/Py_SPW.egg-info/SOURCES.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        1 2023-12-13 21:29:54.000000 Py-SPW-1.5.3/Py_SPW.egg-info/dependency_links.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       86 2023-12-13 21:29:54.000000 Py-SPW-1.5.3/Py_SPW.egg-info/requires.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        6 2023-12-13 21:29:54.000000 Py-SPW-1.5.3/Py_SPW.egg-info/top_level.txt
--rw-r--r--   0 stepan    (1000) stepan    (1000)      945 2023-05-09 10:37:44.000000 Py-SPW-1.5.3/README.md
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-12-13 21:29:54.962476 Py-SPW-1.5.3/pyspw/
--rw-r--r--   0 stepan    (1000) stepan    (1000)     2661 2023-05-09 10:37:42.000000 Py-SPW-1.5.3/pyspw/Parameters.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     3694 2023-12-13 21:27:42.000000 Py-SPW-1.5.3/pyspw/User.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)       42 2023-12-13 21:27:21.000000 Py-SPW-1.5.3/pyspw/__init__.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     9976 2023-07-17 21:58:25.000000 Py-SPW-1.5.3/pyspw/api.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     1728 2023-05-09 10:37:41.000000 Py-SPW-1.5.3/pyspw/errors.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)       85 2023-12-13 21:27:42.000000 Py-SPW-1.5.3/requirements.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       38 2023-12-13 21:29:54.962476 Py-SPW-1.5.3/setup.cfg
--rw-r--r--   0 stepan    (1000) stepan    (1000)     1061 2023-12-13 21:27:42.000000 Py-SPW-1.5.3/setup.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)     1085 2023-05-09 10:37:44.000000 Py-SPW-2.0.0/LICENSE
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)       58 2023-07-13 13:18:30.000000 Py-SPW-2.0.0/MANIFEST.in
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1890 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/PKG-INFO
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/Py_SPW.egg-info/
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)     1890 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/Py_SPW.egg-info/PKG-INFO
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)      868 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/Py_SPW.egg-info/SOURCES.txt
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)        1 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/Py_SPW.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)       86 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/Py_SPW.egg-info/requires.txt
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)       38 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/Py_SPW.egg-info/top_level.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1481 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/README.md
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/docs/
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/docs/source/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    20236 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/docs/source/conf.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/examples/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      446 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/examples/check_access.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      177 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/examples/check_api_work.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1673 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/examples/create_payment_link.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      307 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/examples/get_selfcard_info.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1124 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/examples/send_transaction.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1143 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/examples/users_actions.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      449 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/examples/validate_webhook.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/pyspw/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      152 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)    10950 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/api.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1696 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/errors.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/pyspw/methods/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      456 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     2288 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/base.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      652 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/create_payment.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      650 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/create_transaction.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      564 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/get_me.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      502 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/get_selfcard_info.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      632 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/get_user.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      599 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/get_user_cards.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      904 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/methods/set_transaction_webhook.py
+drwxr-xr-x   0 stepan    (1000) stepan    (1000)        0 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/pyspw/models/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      249 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/models/Card.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      222 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/models/ServerAnswers.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     2826 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/models/Transaction.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     3724 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/models/User.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      421 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/pyspw/models/__init__.py
+-rwxrwxrwx   0 stepan    (1000) stepan    (1000)       85 2023-12-13 21:27:42.000000 Py-SPW-2.0.0/requirements.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       38 2024-04-19 20:35:33.000000 Py-SPW-2.0.0/setup.cfg
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1118 2024-04-19 20:35:20.000000 Py-SPW-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `Py-SPW-1.5.3/LICENSE` & `Py-SPW-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.3/PKG-INFO` & `Py-SPW-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: Py-SPW
-Version: 1.5.3
+Version: 2.0.0
 Summary: Python library for spworlds API
 Home-page: https://github.com/teleportx/Py-SPW
 Author: Stepan Khozhempo
 Author-email: stepan@xstl.ru
 License: MIT License
 Project-URL: Docs, https://pyspw.xstl.ru/en/latest/
 Project-URL: GitHub, https://github.com/teleport2/Py-SPW/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.28.2
-Requires-Dist: mojang==1.1.0
-Requires-Dist: pydantic>=1.10.7
-Requires-Dist: setuptools>=65.5.1
-Requires-Dist: validators>=0.20.0
 
-[![Documentation Status](https://readthedocs.org/projects/py-spw/badge/?version=latest)](https://pyspw.xstl.ru/ru/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/Py-SPW.svg)](https://pypi.org/project/Py-SPW/)
+[![python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/Py-SPW/)
+
+[![Documentation Status](https://github.com/teleportx/Py-SPW/actions/workflows/docs-publish.yml/badge.svg)](https://pyspw.xstl.ru/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/teleportx/Py-SPW/blob/main/LICENSE)
+[![Downloads](https://img.shields.io/pypi/dm/Py-SPW)](https://pypi.org/project/Py-SPW/)
+
+**Follow [telegram channel](https://t.me/xstl_devblog) to receive a notification about new version.**
 
 # Py SPW
 Library for work with [SPWorlds](https://spworlds.ru) API in Python.
 
 ## Installation
 **You need python >=3.7**
 
@@ -45,9 +47,9 @@
 * See the code [examples](https://github.com/teleportx/Py-SPW/tree/main/examples)
 * If you found a bug in a library report it to [issue tracker](https://github.com/teleportx/Py-SPW/issues)
 * Get help with your code using Py-SPW [discussions](https://github.com/teleportx/Py-SPW/discussions)
 
 
 ## Links
 - [PyPi](https://pypi.org/project/Py-SPW)
-- [Documentation](https://pyspw.xstl.ru/en/latest/)
+- [Documentation](https://pyspw.xstl.ru/)
 - [API](https://github.com/sp-worlds/api-docs)
```

### Comparing `Py-SPW-1.5.3/Py_SPW.egg-info/PKG-INFO` & `Py-SPW-2.0.0/Py_SPW.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: Py-SPW
-Version: 1.5.3
+Version: 2.0.0
 Summary: Python library for spworlds API
 Home-page: https://github.com/teleportx/Py-SPW
 Author: Stepan Khozhempo
 Author-email: stepan@xstl.ru
 License: MIT License
 Project-URL: Docs, https://pyspw.xstl.ru/en/latest/
 Project-URL: GitHub, https://github.com/teleport2/Py-SPW/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.28.2
-Requires-Dist: mojang==1.1.0
-Requires-Dist: pydantic>=1.10.7
-Requires-Dist: setuptools>=65.5.1
-Requires-Dist: validators>=0.20.0
 
-[![Documentation Status](https://readthedocs.org/projects/py-spw/badge/?version=latest)](https://pyspw.xstl.ru/ru/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/Py-SPW.svg)](https://pypi.org/project/Py-SPW/)
+[![python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/Py-SPW/)
+
+[![Documentation Status](https://github.com/teleportx/Py-SPW/actions/workflows/docs-publish.yml/badge.svg)](https://pyspw.xstl.ru/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/teleportx/Py-SPW/blob/main/LICENSE)
+[![Downloads](https://img.shields.io/pypi/dm/Py-SPW)](https://pypi.org/project/Py-SPW/)
+
+**Follow [telegram channel](https://t.me/xstl_devblog) to receive a notification about new version.**
 
 # Py SPW
 Library for work with [SPWorlds](https://spworlds.ru) API in Python.
 
 ## Installation
 **You need python >=3.7**
 
@@ -45,9 +47,9 @@
 * See the code [examples](https://github.com/teleportx/Py-SPW/tree/main/examples)
 * If you found a bug in a library report it to [issue tracker](https://github.com/teleportx/Py-SPW/issues)
 * Get help with your code using Py-SPW [discussions](https://github.com/teleportx/Py-SPW/discussions)
 
 
 ## Links
 - [PyPi](https://pypi.org/project/Py-SPW)
-- [Documentation](https://pyspw.xstl.ru/en/latest/)
+- [Documentation](https://pyspw.xstl.ru/)
 - [API](https://github.com/sp-worlds/api-docs)
```

### Comparing `Py-SPW-1.5.3/pyspw/User.py` & `Py-SPW-2.0.0/pyspw/models/User.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,57 @@
+from datetime import datetime
 from enum import Enum
-from typing import Optional
+from typing import Optional, List
+from warnings import warn
 
 import requests as rq
 from mojang import API as MAPI
 from mojang._types import UserProfile
+from pydantic import BaseModel, computed_field, Field
 
-from . import errors as err
-from .errors import MojangAccountNotFound
+from . import Card
+from .. import errors as err
 
 mapi = MAPI()
 
-headers = {
-    'User-Agent': f'Py-SPW'
-}
-
 
 class SkinVariant(Enum):
     """
     Варианты скинов.
     """
     SLIM = 'slim'
     CLASSIC = 'classic'
 
 
-class _SkinPart:
+class SkinPart:
     def __init__(self, url: str):
         self.__skin_part_url = url
 
-    def __str__(self):
-        return self.get_url()
+    @property
+    def url(self) -> str:
+        """
+        Адрес изображения части скина.
+        """
 
-    def __bytes__(self):
-        return self.get_image()
+        return self.__skin_part_url
 
     def get_url(self) -> str:
-        """
-        Получения ссылки на изображение части скина.
+        warn('Use .url', DeprecationWarning)
 
-        :return: Ссылка на изображение части скина.
-        """
-        return self.__skin_part_url
+        return self.url
 
     def get_image(self) -> bytes:
         """
         Получения изображения части скина.
 
         :return: Изображения части скина.
         """
 
         try:
-            visage_surgeplay_response = rq.get(self.__skin_part_url, headers=headers)
+            visage_surgeplay_response = rq.get(self.__skin_part_url)
             if visage_surgeplay_response.status_code != 200:
                 raise err.SurgeplayApiError(f'HTTP status: {visage_surgeplay_response.status_code}')
             return visage_surgeplay_response.content
 
         except rq.exceptions.ConnectionError as error:
             raise err.SurgeplayApiError(error)
 
@@ -65,59 +63,76 @@
         self._profile = profile
         self._variant = SkinVariant(profile.skin_variant)
 
     @property
     def variant(self) -> SkinVariant:
         return self._variant
 
-    def get_face(self, image_size: int = 64) -> _SkinPart:
-        return _SkinPart(f'https://visage.surgeplay.com/face/{image_size}/{self._profile.id}')
+    @property
+    def cape(self) -> Optional[SkinPart]:
+        if self._profile.cape_url is None:
+            return None
+        return SkinPart(self._profile.cape_url)
 
-    def get_front(self, image_size: int = 64) -> _SkinPart:
-        return _SkinPart(f'https://visage.surgeplay.com/front/{image_size}/{self._profile.id}')
+    def get_face(self, image_size: int = 64) -> SkinPart:
+        return SkinPart(f'https://visage.surgeplay.com/face/{image_size}/{self._profile.id}')
 
-    def get_front_full(self, image_size: int = 64) -> _SkinPart:
-        return _SkinPart(f'https://visage.surgeplay.com/frontfull/{image_size}/{self._profile.id}')
+    def get_front(self, image_size: int = 64) -> SkinPart:
+        return SkinPart(f'https://visage.surgeplay.com/front/{image_size}/{self._profile.id}')
 
-    def get_head(self, image_size: int = 64) -> _SkinPart:
-        return _SkinPart(f'https://visage.surgeplay.com/head/{image_size}/{self._profile.id}')
+    def get_front_full(self, image_size: int = 64) -> SkinPart:
+        return SkinPart(f'https://visage.surgeplay.com/frontfull/{image_size}/{self._profile.id}')
 
-    def get_bust(self, image_size: int = 64) -> _SkinPart:
-        return _SkinPart(f'https://visage.surgeplay.com/bust/{image_size}/{self._profile.id}')
+    def get_head(self, image_size: int = 64) -> SkinPart:
+        return SkinPart(f'https://visage.surgeplay.com/head/{image_size}/{self._profile.id}')
 
-    def get_full(self, image_size: int = 64) -> _SkinPart:
-        return _SkinPart(f'https://visage.surgeplay.com/full/{image_size}/{self._profile.id}')
+    def get_bust(self, image_size: int = 64) -> SkinPart:
+        return SkinPart(f'https://visage.surgeplay.com/bust/{image_size}/{self._profile.id}')
 
-    def get_skin(self, image_size: int = 64) -> _SkinPart:
-        return _SkinPart(f'https://visage.surgeplay.com/skin/{image_size}/{self._profile.id}')
+    def get_full(self, image_size: int = 64) -> SkinPart:
+        return SkinPart(f'https://visage.surgeplay.com/full/{image_size}/{self._profile.id}')
 
-    def get_cape(self) -> Optional[_SkinPart]:
-        if self._profile.cape_url is None:
-            return None
-        return _SkinPart(self._profile.cape_url)
+    def get_skin(self, image_size: int = 64) -> SkinPart:
+        return SkinPart(f'https://visage.surgeplay.com/skin/{image_size}/{self._profile.id}')
 
 
-class User:
-    def __init__(self, nickname: str):
-        self._nickname = nickname
-        self._uuid = mapi.get_uuid(nickname)
-        if self._uuid is None:
-            raise MojangAccountNotFound(self._nickname)
-        self._profile = mapi.get_profile(self._uuid)
+class City(BaseModel):
+    id: str
+    name: str
+    description: str
 
-    @property
-    def nickname(self) -> str:
-        return self._nickname
+    x: int
+    z: int
+    isMayor: bool
 
-    @property
-    def uuid(self) -> str:
-        return self._uuid
+
+class User(BaseModel):
+    username: Optional[str]
+    uuid: Optional[str]
 
     @property
-    def profile(self) -> UserProfile:
-        return self._profile
+    def nickname(self) -> Optional[str]:
+        warn('Use .username', DeprecationWarning)
+        return self.username
+
+    def get_profile(self) -> Optional[UserProfile]:
+        if self.uuid is None:
+            return
+
+        return mapi.get_profile(self.uuid)
 
     def get_skin(self) -> Skin:
-        """
-        Получения объекта скина пользователя.
-        """
-        return Skin(self._profile)
+        return Skin(self.get_profile())
+
+
+class SelfUser(BaseModel):
+    id: str
+    username: str
+    uuid: Optional[str] = Field(validation_alias='minecraftUUID')
+
+    status: str
+    city: Optional[City]
+
+    roles: List[str]
+    cards: List[Card]
+
+    createdAt: datetime
```

### Comparing `Py-SPW-1.5.3/pyspw/api.py` & `Py-SPW-2.0.0/pyspw/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,183 +1,221 @@
-import json
-import platform
-from base64 import b64encode
-from dataclasses import dataclass
-from enum import Enum
-from hashlib import sha256
 import hmac
-import requests as rq
-import time
-from typing import List, Callable
 import logging
-from mojang import API as MAPI
-
-from . import errors as err
-from .User import User
-from .Parameters import Payment, Transaction
-
-mapi = MAPI()
+import time
+from base64 import b64encode
+from hashlib import sha256
+from typing import List, Callable, Optional
+from warnings import warn
 
+from pydantic import BaseModel, computed_field
 
-class _RequestTypes(Enum):
-    POST = 'POST'
-    GET = 'GET'
+from . import errors as err
+from . import models
+from .methods import GetUser, CreatePayment, CreateTransaction, GetSelfCardInfo, SetTransactionWebhook, GetMe, \
+    GetUserCards
 
 
-@dataclass
-class _Card:
+class AuthorizationPair(BaseModel):
     id: str
     token: str
 
+    @computed_field
+    @property
+    def authorization(self) -> str:
+        return f'Bearer ' + str(b64encode(str(f'{self.id}:{self.token}').encode('utf-8')), 'utf-8')
+
+    def verify_webhook(self, webhook_data: str, X_Body_Hash: str):
+        hmac_data = hmac.new(self.token.encode('utf-8'), webhook_data.encode('utf-8'), sha256).digest()
+        base64_data = b64encode(hmac_data)
+        return hmac.compare_digest(base64_data, X_Body_Hash.encode('utf-8'))
+
 
 class SpApi:
     """
-    API класс для работы с spworlds api
+    **API класс для работы с spworlds api**
 
     :param card_id: Индефикатор карты
     :type card_id: str
 
     :param card_token: Секретный ключ доступа карты
     :type card_token: str
     """
 
-    _spworlds_api_url = 'https://spworlds.ru/api/public'
-
     def __init__(self, card_id: str, card_token: str):
-        self._card = _Card(card_id, card_token)
-        self._authorization = f"Bearer {str(b64encode(str(f'{card_id}:{card_token}').encode('utf-8')), 'utf-8')}"
-
-    def _request(self, method: _RequestTypes, path: str = '', body: dict = None, *,
-                 ignore_codes: list = []) -> rq.Response:
-        headers = {
-            'Authorization': self._authorization,
-            'User-Agent': f'Py-SPW (Python {platform.python_version()})'
-        }
-        try:
-            response = rq.request(method.value, url=self._spworlds_api_url + path, headers=headers, json=body)
-
-        except rq.exceptions.ConnectionError as error:
-            raise err.SpwApiError(error)
-
-        try:
-            response.json()
-
-        except json.JSONDecodeError:
-            raise err.SpwApiDDOS()
-
-        if response.ok or response.status_code in ignore_codes:
-            return response
-
-        elif response.status_code == 401:
-            raise err.SpwUnauthorized()
-
-        elif response.status_code >= 500:
-            raise err.SpwApiError(f'HTTP: {response.status_code}, Server Error.')
-
-        else:
-            raise err.SpwApiError(
-                f'HTTP: {response.status_code} {response.json()["error"]}. Message: {response.json()["message"]}')
+        self._auth = AuthorizationPair(
+            id=card_id,
+            token=card_token
+        )
 
     def ping(self) -> bool:
         """
             Проверка работоспособности API.
 
             :return: Состояние API.
         """
         try:
-            self.get_balance()
+            self.card()
             return True
 
         except err.SpwApiError:
             return False
 
-    def get_user(self, discord_id: str) -> User:
+    def get_user(self, discord_id: str) -> models.User:
         """
             Получение пользователя.
 
             :param discord_id: ID пользователя дискорда.
             :type discord_id: bool
 
             :return: Объект пользователя.
 
             :raises SpwUserNotFound: Пользователь не был найден.
         """
 
-        response = self._request(_RequestTypes.GET, f'/users/{discord_id}', ignore_codes=[404])
-        if response.status_code == 404:
-            raise err.SpwUserNotFound(discord_id)
+        try:
+            return GetUser(
+                discord_id=int(discord_id)
+            )(self._auth.authorization)
+
+        except err.SpwApiError as e:
+            if e.status_code == 404:
+                raise err.SpwUserNotFound(discord_id)
 
-        return User(response.json()['username'])
+            raise e
 
     def check_access(self, discord_id: str) -> bool:
         """
             Получение статуса проходки.
 
             :param discord_id: ID пользователя дискорда.
             :type discord_id: bool
 
             :return: Состояние проходки пользователя.
         """
-        response = self._request(_RequestTypes.GET, f'/users/{discord_id}', ignore_codes=[404])
-        return response.status_code != 404
+
+        try:
+            GetUser(
+                discord_id=int(discord_id)
+            )(self._auth.authorization)
+            return True
+
+        except err.SpwApiError as e:
+            if e.status_code == 404:
+                return False
+
+            raise e
 
     def check_webhook(self, webhook_data: str, X_Body_Hash: str) -> bool:
         """
             Валидирует webhook.
 
             :param webhook_data: Тело webhook'а.
             :type webhook_data: str
 
             :param X_Body_Hash: Хэдер X-Body-Hash из webhook.
             :type X_Body_Hash: str
 
             :return: Верефецирован или нет вебхук.
         """
 
-        hmac_data = hmac.new(self._card.token.encode('utf-8'), webhook_data.encode('utf-8'), sha256).digest()
-        base64_data = b64encode(hmac_data)
-        return hmac.compare_digest(base64_data, X_Body_Hash.encode('utf-8'))
+        return self._auth.verify_webhook(webhook_data, X_Body_Hash)
 
-    def create_payment(self, payment: Payment) -> str:
+    def create_payment(self, payment: models.Payment) -> str:
         """
             Создание ссылки на оплату.
 
             :param payment: Параметры оплаты.
             :type payment: Payment
 
             :return: Ссылку на страницу оплаты, на которую стоит перенаправить пользователя.
         """
-        return self._request(_RequestTypes.POST, '/payment', payment.dict()).json()['url']
 
-    def send_transaction(self, transaction: Transaction) -> None:
+        return CreatePayment(
+            payment=payment
+        )(self._auth.authorization).url
+
+    def send_transaction(self, transaction: models.Transaction):
         """
             Отправка транзакции.
             
             :param transaction: Параметры транзакции.
             :type transaction: Transaction
 
             :raises SpwInsufficientFunds: Недостаточно средств на карте.
             :raises SpwCardNotFound: Карта получателя не найдена.
         """
-        response = self._request(_RequestTypes.POST, '/transactions', transaction.dict(), ignore_codes=[400])
-        if response.status_code == 400:
-            msg = response.json()["message"]
-            if msg == 'Недостаточно средств на карте':
-                raise err.SpwInsufficientFunds()
 
-            elif msg == 'Карты не существует':
-                raise err.SpwCardNotFound()
+        try:
+            CreateTransaction(
+                transaction=transaction
+            )(self._auth.authorization)
+
+        except err.SpwApiError as e:
+            if e.status_code == 400:
+                if e.extra_info == 'Недостаточно средств на карте':
+                    raise err.SpwInsufficientFunds()
+
+                elif e.extra_info == 'Карты не существует':
+                    raise err.SpwCardNotFound()
+
+            raise e
+
+    def card(self) -> models.SelfCard:
+        """
+            Получение информации о токен-карте.
+
+            :return: Card класс с информации о карте.
+        """
+
+        return GetSelfCardInfo()(self._auth.authorization)
 
     def get_balance(self) -> int:
         """
             Получение баланса.
 
             :return: Значения баланса карты.
         """
-        return self._request(_RequestTypes.GET, '/card').json()['balance']
+        warn('Use .card().balance', DeprecationWarning)
+
+        return self.card().balance
+
+    def set_transaction_webhook(self, url: Optional[str]):
+        """
+            Установка адреса для получения вебхуков о транзакциях по карте.
+
+            :param url: Адрес вебхука.
+            :type url: Optional[str]
+        """
+
+        SetTransactionWebhook(
+            url=url
+        )(self._auth.authorization)
+
+    def me(self) -> models.SelfUser:
+        """
+            Получения пользователя владельца карты.
+
+            :return: Пользователь владельца карты.
+        """
+
+        return GetMe()(self._auth.authorization)
+
+    def get_user_cards(self, username: str) -> List[models.Card]:
+        """
+            Получения карта пользователя.
+
+            :param username: Имя пользователя у которого надо получить карты.
+            :type username: str
+
+            :return: Список карт пользователя.
+        """
+
+        return GetUserCards(
+            username=username
+        )(self._auth.authorization)
 
     # ---------------------------------
     # ------------- Manys -------------
     # ---------------------------------
 
     def _many_req(self, iterable: List, method: Callable, delay: float) -> List:
         users = []
@@ -187,15 +225,15 @@
 
         for i in iterable:
             users.append(method(i))
             time.sleep(delay)
 
         return users
 
-    def get_users(self, discord_ids: List[str], delay: float = 0.3) -> List[User]:
+    def get_users(self, discord_ids: List[str], delay: float = 0.3) -> List[models.User]:
         """
             Получение пользователей.
 
             :param delay: Значение задержки между запросами, указывается в секундах.
             :type delay: float
 
             :param discord_ids: Список discord id пользователей, которых вы бы хотели получить.
@@ -217,46 +255,49 @@
             :param discord_ids: Список discord id пользователей статусы проходок, которых вы бы хотели получить.
             :type discord_ids: List[str]
 
             :return: Список со статусами проходок.
         """
         return self._many_req(discord_ids, self.check_access, delay)
 
-    def create_payments(self, payments: List[Payment], delay: float = 0.5) -> List[str]:
+    def create_payments(self, payments: List[models.Payment], delay: float = 0.5) -> List[str]:
         """
             Создание ссылок на оплату.
 
             :param delay: Значение задержки между запросами, указывается в секундах.
             :type delay: float
 
             :param payments: Список параметров оплаты.
             :type payments: List[Payment]
 
             :return: Список ссылок на оплату.
         """
         return self._many_req(payments, self.create_payment, delay)
 
-    def send_transactions(self, transactions: List[Transaction], delay: float = 0.5) -> None:
+    def send_transactions(self, transactions: List[models.Transaction], delay: float = 0.5, safe: bool = True) -> None:
         """
             Отправка транзакций.
 
             .. warning::
-                **Важно: Перед множетсвенной отправки транзаций проводится дополнительная проверка на количество средств на карте.
+                **Важно: Если safe=true, то перед множетсвенной отправки транзаций проводится дополнительная проверка на количество средств на карте.
                 В случае если во время совершения транзакций кто-либо еще спишет с этой карты сумму, после которой
                 остаток на карте не будет достаточен для проведения транзакции, то выполнение транзакций прервется,
                 а предыдущие транзации не откатятся.**
 
+            :param safe: Значение задержки между запросами, указывается в секундах.
+            :type safe: bool
+
             :param delay: Значение задержки между запросами, указывается в секундах.
             :type delay: float
 
             :param transactions: Список параметров транзакций
             :type transactions: List[Transaction]
 
             :raises SpwInsufficientFunds: Недостаточно средств на карте.
             :raises SpwCardNotFound: Карта получателя не найдена.
         """
 
         # Additional balance verify
-        if self.get_balance() < sum([tr.amount for tr in transactions]):
+        if safe and self.card().balance < sum([tr.amount for tr in transactions]):
             raise err.SpwInsufficientFunds()
 
         self._many_req(transactions, self.send_transaction, delay)
```

### Comparing `Py-SPW-1.5.3/pyspw/errors.py` & `Py-SPW-2.0.0/pyspw/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,45 +3,59 @@
 
 
 class _ApiError(_Error):
     pass
 
 
 class SpwApiError(_ApiError):
-    pass
+    def __init__(self, status_code: int, text: str = None, extra_info: str = None):
+        if extra_info is not None:
+            extra_info = ' ' + extra_info
+
+        else:
+            extra_info = ''
+
+        if text is None:
+            text = f'Raised not OK status. HTTP: {status_code}.'
+
+        self.status_code = status_code
+        self.text = text
+        self.extra_info = extra_info
+
+        super().__init__(text + extra_info)
 
 
 class SpwApiDDOS(SpwApiError):
     def __init__(self):
-        super().__init__("SPWorlds DDOS protection block your request")
+        super().__init__(429, "SPWorlds DDOS protection block your request")
 
 
 class SpwUserNotFound(SpwApiError):
     def __init__(self, discord_id: str):
         self._discord_id = discord_id
-        super().__init__(f"User with discord id `{discord_id}` not found in spworlds")
+        super().__init__(404, f"User with discord id `{discord_id}` not found in spworlds")
 
     @property
     def discord_id(self) -> str:
         return self._discord_id
 
 
 class SpwUnauthorized(SpwApiError):
     def __init__(self):
-        super().__init__("Access details are invalid")
+        super().__init__(401, "Access details are invalid")
 
 
 class SpwInsufficientFunds(SpwApiError):
     def __init__(self):
-        super().__init__("Insufficient funds on the card")
+        super().__init__(400, "Insufficient funds on the card")
 
 
 class SpwCardNotFound(SpwApiError):
     def __init__(self):
-        super().__init__("Receiver card not found")
+        super().__init__(404, "Receiver card not found")
 
 
 class MojangApiError(_ApiError):
     pass
 
 
 class MojangAccountNotFound(MojangApiError):
@@ -52,27 +66,7 @@
     @property
     def nickname(self) -> str:
         return self._nickname
 
 
 class SurgeplayApiError(_ApiError):
     pass
-
-
-class LengthError(ValueError):
-    def __init__(self, max_length: int):
-        super().__init__(f"length must be <= {max_length}.")
-
-
-class BigAmountError(ValueError):
-    def __init__(self):
-        super().__init__(f"amount must be <= 1728.")
-
-
-class IsNotURLError(ValueError):
-    def __init__(self):
-        super().__init__(f"is not url.")
-
-
-class IsNotCardError(ValueError):
-    def __init__(self, card: str):
-        super().__init__(f"Receiver card (`{card}`) number not valid")
```

### Comparing `Py-SPW-1.5.3/setup.py` & `Py-SPW-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from os import path, environ
 
 from setuptools import setup
+from setuptools.config.expand import find_packages
 
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     description_md = f.read()
 
 requirements = open('requirements.txt', 'r').read().split('\n')
@@ -13,15 +14,15 @@
 
 if environ.get('version') is not None:
     __version__ = environ.get('version')
 
 setup(
     name='Py-SPW',
     version=__version__,
-    packages=['pyspw'],
+    packages=find_packages(),
     url='https://github.com/teleportx/Py-SPW',
     license='MIT License',
     author='Stepan Khozhempo',
     author_email='stepan@xstl.ru',
     description='Python library for spworlds API',
     long_description=description_md,
     long_description_content_type='text/markdown',
```

