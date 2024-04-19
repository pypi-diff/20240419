# Comparing `tmp/pyflocker-0.4.1.tar.gz` & `tmp/pyflocker-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflocker-0.4.1.tar", max compression
+gzip compressed data, was "pyflocker-0.4.2.tar", last modified: Fri Apr 19 11:34:20 2024, max compression
```

## Comparing `pyflocker-0.4.1.tar` & `pyflocker-0.4.2.tar`

### file list

```diff
@@ -1,43 +1,56 @@
--rw-r--r--   0        0        0     1073 2023-02-23 06:11:56.062059 pyflocker-0.4.1/LICENSE
--rw-r--r--   0        0        0     4933 2023-02-23 06:11:56.062059 pyflocker-0.4.1/README.md
--rw-r--r--   0        0        0     3776 2023-02-23 06:11:56.066058 pyflocker-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      142 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/__init__.py
--rw-r--r--   0        0        0      512 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/__init__.py
--rw-r--r--   0        0        0     2523 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/__init__.py
--rw-r--r--   0        0        0     2849 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/asymmetric.py
--rw-r--r--   0        0        0     8848 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/AES.py
--rw-r--r--   0        0        0     2357 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/ChaCha20.py
--rw-r--r--   0        0        0    17033 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/ECC.py
--rw-r--r--   0        0        0     7617 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/Hash.py
--rw-r--r--   0        0        0    13231 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/RSA.py
--rw-r--r--   0        0        0       70 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/__init__.py
--rw-r--r--   0        0        0     5599 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/asymmetric.py
--rw-r--r--   0        0        0     1404 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/misc.py
--rw-r--r--   0        0        0     3926 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/symmetric.py
--rw-r--r--   0        0        0    12636 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/AES.py
--rw-r--r--   0        0        0     4288 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/Camellia.py
--rw-r--r--   0        0        0     5563 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/ChaCha20.py
--rw-r--r--   0        0        0    11252 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/DH.py
--rw-r--r--   0        0        0    23459 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/ECC.py
--rw-r--r--   0        0        0     6415 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/Hash.py
--rw-r--r--   0        0        0    12153 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/RSA.py
--rw-r--r--   0        0        0       74 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/__init__.py
--rw-r--r--   0        0        0     4278 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/asymmetric.py
--rw-r--r--   0        0        0     1964 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/misc.py
--rw-r--r--   0        0        0     3492 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/symmetric.py
--rw-r--r--   0        0        0     8917 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/backends/symmetric.py
--rw-r--r--   0        0        0    26613 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/base.py
--rw-r--r--   0        0        0      931 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/exc.py
--rw-r--r--   0        0        0     3539 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/AES.py
--rw-r--r--   0        0        0     3099 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/Camellia.py
--rw-r--r--   0        0        0     1438 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/ChaCha20.py
--rw-r--r--   0        0        0     3181 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/DH.py
--rw-r--r--   0        0        0     2540 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/ECC.py
--rw-r--r--   0        0        0     2124 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/Hash.py
--rw-r--r--   0        0        0     2600 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/RSA.py
--rw-r--r--   0        0        0        0 2023-02-23 06:11:56.066058 pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/__init__.py
--rw-r--r--   0        0        0      706 2023-02-23 06:11:56.070059 pyflocker-0.4.1/src/pyflocker/ciphers/modes.py
--rw-r--r--   0        0        0    19717 2023-02-23 06:11:56.070059 pyflocker-0.4.1/src/pyflocker/locker.py
--rw-r--r--   0        0        0        0 2023-02-23 06:11:56.070059 pyflocker-0.4.1/src/pyflocker/py.typed
--rw-r--r--   0        0        0     6043 1970-01-01 00:00:00.000000 pyflocker-0.4.1/setup.py
--rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 pyflocker-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-19 11:33:58.399529 pyflocker-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4933 2024-04-19 11:33:58.399529 pyflocker-0.4.2/README.md
+-rw-r--r--   0        0        0     3219 2024-04-19 11:34:20.035698 pyflocker-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-19 11:34:20.027698 pyflocker-0.4.2/src/pyflocker/_version.py
+-rw-r--r--   0        0        0      512 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/__init__.py
+-rw-r--r--   0        0        0     2570 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/__init__.py
+-rw-r--r--   0        0        0     2898 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/asymmetric.py
+-rw-r--r--   0        0        0     9116 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/AES.py
+-rw-r--r--   0        0        0     2383 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/ChaCha20.py
+-rw-r--r--   0        0        0    17508 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/ECC.py
+-rw-r--r--   0        0        0     7701 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/Hash.py
+-rw-r--r--   0        0        0    13689 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/RSA.py
+-rw-r--r--   0        0        0       70 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/__init__.py
+-rw-r--r--   0        0        0     5743 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/asymmetric.py
+-rw-r--r--   0        0        0     1437 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/misc.py
+-rw-r--r--   0        0        0     3962 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/symmetric.py
+-rw-r--r--   0        0        0    12773 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/AES.py
+-rw-r--r--   0        0        0     4304 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/Camellia.py
+-rw-r--r--   0        0        0     5665 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/ChaCha20.py
+-rw-r--r--   0        0        0    11678 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/DH.py
+-rw-r--r--   0        0        0    23939 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/ECC.py
+-rw-r--r--   0        0        0     6465 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/Hash.py
+-rw-r--r--   0        0        0    12387 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/RSA.py
+-rw-r--r--   0        0        0       74 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/__init__.py
+-rw-r--r--   0        0        0     4413 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/asymmetric.py
+-rw-r--r--   0        0        0     1979 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/misc.py
+-rw-r--r--   0        0        0     3532 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/symmetric.py
+-rw-r--r--   0        0        0     9068 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/backends/symmetric.py
+-rw-r--r--   0        0        0    26612 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/base.py
+-rw-r--r--   0        0        0      930 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/exc.py
+-rw-r--r--   0        0        0     3619 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/AES.py
+-rw-r--r--   0        0        0     3154 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/Camellia.py
+-rw-r--r--   0        0        0     1502 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/ChaCha20.py
+-rw-r--r--   0        0        0     3204 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/DH.py
+-rw-r--r--   0        0        0     2588 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/ECC.py
+-rw-r--r--   0        0        0     2148 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/Hash.py
+-rw-r--r--   0        0        0     2649 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/RSA.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/__init__.py
+-rw-r--r--   0        0        0      706 2024-04-19 11:33:58.403529 pyflocker-0.4.2/src/pyflocker/ciphers/modes.py
+-rw-r--r--   0        0        0    19758 2024-04-19 11:33:58.407529 pyflocker-0.4.2/src/pyflocker/locker.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:33:58.407529 pyflocker-0.4.2/src/pyflocker/py.typed
+-rw-r--r--   0        0        0        0 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/base.py
+-rw-r--r--   0        0        0      292 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0    29729 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_AES.py
+-rw-r--r--   0        0        0    15952 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_Camellia.py
+-rw-r--r--   0        0        0    14761 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_ChaCha20.py
+-rw-r--r--   0        0        0     9678 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_DH.py
+-rw-r--r--   0        0        0    17385 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_ECC.py
+-rw-r--r--   0        0        0    12019 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_Hash.py
+-rw-r--r--   0        0        0    16507 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_RSA.py
+-rw-r--r--   0        0        0    11921 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_locker.py
+-rw-r--r--   0        0        0     1891 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_misc.py
+-rw-r--r--   0        0        0     2173 2024-04-19 11:33:58.407529 pyflocker-0.4.2/tests/test_symmetric.py
+-rw-r--r--   0        0        0     6200 1970-01-01 00:00:00.000000 pyflocker-0.4.2/PKG-INFO
```

### Comparing `pyflocker-0.4.1/LICENSE` & `pyflocker-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflocker-0.4.1/README.md` & `pyflocker-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/__init__.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/__init__.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import enum
 import typing
 from importlib import import_module
 
-from .. import exc
+from pyflocker.ciphers import exc
 
 _DEFAULT_BACKEND = None
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import types
     from types import ModuleType
 
@@ -36,17 +36,16 @@
         UnsupportedAlgorithm:
             This is raised if the algorithm is not found in the backend.
     """
     _backend = load_backend(backend)
     try:
         return import_module(f".{name}", _backend.__name__)
     except ImportError as e:
-        raise exc.UnsupportedAlgorithm(
-            f"{name} is not implemented by backend {backend}."
-        ) from e
+        msg = f"{name} is not implemented by backend {backend}."
+        raise exc.UnsupportedAlgorithm(msg) from e
 
 
 def load_backend(
     backend: Backends | None = None,
 ) -> types.ModuleType:
     """Load a backend.
 
@@ -68,15 +67,16 @@
     if backend is None:
         if _DEFAULT_BACKEND is None:
             _DEFAULT_BACKEND = _find_backend()
         return _DEFAULT_BACKEND  # type: ignore
 
     # backend is not None
     if not isinstance(backend, Backends):
-        raise TypeError("argument backend must be of type Backends.")
+        msg = "argument backend must be of type Backends."
+        raise TypeError(msg)
 
     if _DEFAULT_BACKEND is None:
         _DEFAULT_BACKEND = _import_helper(backend)
         return _DEFAULT_BACKEND  # noqa: PIE781
 
     return _import_helper(backend)
 
@@ -94,10 +94,11 @@
     for i in list(Backends):
         try:
             return _import_helper(i)
         except ImportError:
             errors += 1
 
     if errors == len(Backends):
-        raise ImportError("No backends found.")
+        msg = "No backends found."
+        raise ImportError(msg)
 
     return None
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/asymmetric.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/asymmetric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Tools for asymmetric ciphers common to all the backends."""
+
 from __future__ import annotations
 
 import typing
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
-from ..base import (
+from pyflocker.ciphers.base import (
     BaseAsymmetricPadding,
     BaseEllepticCurveExchangeAlgorithm,
     BaseEllepticCurveSignatureAlgorithm,
     BaseMGF,
 )
-from ..interfaces import Hash
+from pyflocker.ciphers.interfaces import Hash
 
 if TYPE_CHECKING:  # pragma: no cover
-    from ..base import BaseHash
+    from pyflocker.ciphers.base import BaseHash
 
 
 def _default_hash_factory() -> BaseHash:
     """SHA-256 Hash object factory.
 
     The import is delayed because we want the backends to be loaded
     only when they are explicitly called by user or loaded by the
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/AES.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/AES.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Implementation of AES cipher."""
+
 from __future__ import annotations
 
 import contextlib
 import typing
 from types import MappingProxyType
 from typing import TYPE_CHECKING
 
 from Cryptodome.Cipher import AES
 
-from ... import exc, modes
-from ...base import BaseAEADOneShotCipher
-from ...modes import Modes
-from ..symmetric import FileCipherWrapper, HMACWrapper
+from pyflocker.ciphers import base, exc, modes
+from pyflocker.ciphers.backends.symmetric import FileCipherWrapper, HMACWrapper
+from pyflocker.ciphers.base import BaseAEADOneShotCipher
+from pyflocker.ciphers.modes import Modes
+
 from . import Hash
 from .misc import derive_hkdf_key
 from .symmetric import (
     AEADCipherTemplate,
     AuthenticationMixin,
     NonAEADCipherTemplate,
 )
 
 if TYPE_CHECKING:  # pragma: no cover
     import io
 
-    from ... import base
-
 SUPPORTED = MappingProxyType(
     {
         # classic modes
         Modes.MODE_CTR: AES.MODE_CTR,
         Modes.MODE_CFB: AES.MODE_CFB,
         Modes.MODE_CFB8: AES.MODE_CFB,  # compat with pyca/cryptography
         Modes.MODE_OFB: AES.MODE_OFB,
@@ -70,15 +70,15 @@
 class AEAD(AEADCipherTemplate):
     def __init__(
         self,
         encrypting: bool,
         key: bytes,
         mode: Modes,
         nonce: bytes,
-    ):
+    ) -> None:
         self._cipher = _get_aes_cipher(key, mode, nonce)
         self._updated = False
         self._encrypting = encrypting
         self._mode = mode
         self._tag = None
         # creating a context is relatively expensive here
         self._update_func = (
@@ -94,15 +94,15 @@
 class NonAEAD(NonAEADCipherTemplate):
     def __init__(
         self,
         encrypting: bool,
         key: bytes,
         mode: Modes,
         nonce: bytes,
-    ):
+    ) -> None:
         self._cipher = _get_aes_cipher(key, mode, nonce)
         self._updated = False
         self._encrypting = encrypting
         self._mode = mode
 
         # creating a context is relatively expensive here
         self._update_func = (
@@ -120,15 +120,15 @@
 
     def __init__(
         self,
         encrypting: bool,
         key: bytes,
         mode: Modes,
         nonce: bytes,
-    ):
+    ) -> None:
         self._cipher = _get_aes_cipher(key, mode, nonce)
         self._updated = False
         self._encrypting = encrypting
         self._mode = mode
 
         # creating a context is relatively expensive here
         self._update_func = self._get_update_func(encrypting, self._cipher)
@@ -167,22 +167,22 @@
         if self._update_func is None:
             raise exc.AlreadyFinalized
 
         update_func_kwargs = {}
         if self.mode in self._write_into_buffer_unsupported:
             # the mode does not support writing into mutable buffers.
             if out is not None:
-                raise NotImplementedError(
-                    f"writing into buffer unsupported by {self.mode.name}"
-                )
+                msg = f"writing into buffer unsupported by {self.mode.name}"
+                raise NotImplementedError(msg)
         else:
             update_func_kwargs = {"output": out}
 
         if not self.is_encrypting() and tag is None:
-            raise ValueError("tag is required for decryption")
+            msg = "tag is required for decryption"
+            raise ValueError(msg)
 
         result: bytes | None = None
         with contextlib.suppress(ValueError):
             result = self._update_func(data, tag, **update_func_kwargs)
 
         self.finalize(tag)
         return result
@@ -248,47 +248,52 @@
         NotImplementedError:
             if the ``mode`` does not support encryption/decryption of files or
             the mode is not supported by the backend.
 
     Note:
         Any other error that is raised is from the backend itself.
     """
-    crp: typing.Any
-
-    if file is not None:
-        use_hmac = True
+    cipher: base.BaseAEADCipher | base.BaseNonAEADCipher | FileCipherWrapper
 
     if mode not in supported_modes():
-        raise exc.UnsupportedMode(f"{mode.name} not supported.")
+        msg = f"{mode.name} not supported."
+        raise exc.UnsupportedMode(msg)
+
+    is_mode_aead = mode in modes.AEAD
+    is_file = file is not None
+    use_hmac = (is_file and not is_mode_aead) or (use_hmac and not is_mode_aead)
 
     if mode in modes.SPECIAL:
-        if file is not None:
-            raise NotImplementedError(
-                f"{mode} does not support encryption/decryption of files."
+        if is_file:
+            msg = (
+                f"{mode.name} does not support encryption/decryption of files."
             )
-        crp = AEADOneShot(encrypting, key, mode, iv_or_nonce)
-    elif mode in modes.AEAD:
-        crp = AEAD(encrypting, key, mode, iv_or_nonce)
+            raise NotImplementedError(msg)
+        return AEADOneShot(encrypting, key, mode, iv_or_nonce)
+
+    if is_mode_aead:
+        cipher = AEAD(encrypting, key, mode, iv_or_nonce)
     else:
-        if use_hmac:
-            crp = _wrap_hmac(
-                encrypting,
-                key,
-                mode,
-                iv_or_nonce,
-                digestmod if digestmod is not None else Hash.new("sha256"),
-                tag_length,
-            )
-        else:
-            crp = NonAEAD(encrypting, key, mode, iv_or_nonce)
+        cipher = NonAEAD(encrypting, key, mode, iv_or_nonce)
+
+    if use_hmac:
+        cipher = _wrap_hmac(
+            encrypting,
+            key,
+            mode,
+            iv_or_nonce,
+            digestmod or Hash.new("sha256"),
+            tag_length,
+        )
 
     if file:
-        crp = FileCipherWrapper(crp, file)
+        assert isinstance(cipher, base.BaseAEADCipher)
+        cipher = FileCipherWrapper(cipher, file)
 
-    return crp
+    return cipher
 
 
 def supported_modes() -> set[Modes]:
     """Lists all modes supported by AES cipher of this backend.
 
     Returns:
         set of :any:`Modes` object supported by backend.
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/ChaCha20.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/ChaCha20.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from __future__ import annotations
 
 import typing
 
-from Cryptodome.Cipher import ChaCha20 as _ChaCha20
-from Cryptodome.Cipher import ChaCha20_Poly1305 as _ChaCha20_Poly1305
+from Cryptodome.Cipher import (
+    ChaCha20 as _ChaCha20,
+    ChaCha20_Poly1305 as _ChaCha20_Poly1305,
+)
+
+from pyflocker.ciphers.backends.symmetric import FileCipherWrapper
 
-from ..symmetric import FileCipherWrapper
 from .symmetric import AEADCipherTemplate, NonAEADCipherTemplate
 
 if typing.TYPE_CHECKING:
     import io
 
 
 class ChaCha20(NonAEADCipherTemplate):
     """ChaCha20 Cipher class.
 
     This class alone does not provide any authentication. For AEAD purposes,
     wrap ``ChaCha20`` object with a class that implements ``BaseAEADCipher`` or
     use ``ChaCha20Poly1305``.
     """
 
-    def __init__(self, encrypting: bool, key: bytes, nonce: bytes):
+    def __init__(self, encrypting: bool, key: bytes, nonce: bytes) -> None:
         self._cipher = _ChaCha20.new(key=key, nonce=nonce)
         self._encrypting = encrypting
         self._update_func = (
             self._cipher.encrypt if encrypting else self._cipher.decrypt
         )
 
 
 class ChaCha20Poly1305(AEADCipherTemplate):
     """ChaCha20Poly1305 Cipher class."""
 
-    def __init__(self, encrypting: bool, key: bytes, nonce: bytes):
+    def __init__(self, encrypting: bool, key: bytes, nonce: bytes) -> None:
         self._cipher = _ChaCha20_Poly1305.new(key=key, nonce=nonce)
         self._encrypting = encrypting
         self._update_func = (
             self._cipher.encrypt if encrypting else self._cipher.decrypt
         )
         self._tag = None
         self._updated = False
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/ECC.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/ECC.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import typing
 
 from Cryptodome.PublicKey import ECC
 from Cryptodome.Signature import eddsa
 
-from ... import base, exc
-from ..asymmetric import ECDSA, EdDSA
+from pyflocker.ciphers import base, exc
+from pyflocker.ciphers.backends.asymmetric import ECDSA, EdDSA
+
 from .asymmetric import PROTECTION_SCHEMES, get_ec_signature_algorithm
 
 
 class _Curves:
     NIST_CURVES = {
         # p192 and aliases
         "NIST P-192": "p192",
@@ -72,19 +73,21 @@
         curve: str | None,
         _key: ECC.EccKey | None = None,
     ) -> None:
         if _key is not None:
             self._key = _key
         else:
             if not isinstance(curve, str):
-                raise TypeError("curve name must be a string")
+                msg = "curve name must be a string"
+                raise TypeError(msg)
             try:
                 self._key = ECC.generate(curve=_Curves.CURVES[curve])
             except KeyError as e:
-                raise ValueError(f"Invalid curve: {curve}") from e
+                msg = f"Invalid curve: {curve}"
+                raise ValueError(msg) from e
 
         self._key_size = self._key.pointQ.size_in_bits()
         self._curve = self._key.curve
 
     @property
     def key_size(self) -> int:
         return self._key_size
@@ -133,34 +136,37 @@
             TypeError:
                 if the passphrase is not a bytes-like object when protection
                 is supplied.
         """
         try:
             encoding, format = self._ENCODINGS[encoding], self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(f"Invalid encoding or format: {e}") from e
+            msg = f"Invalid encoding or format: {e}"
+            raise ValueError(msg) from e
 
         if (
             protection is not None and protection not in PROTECTION_SCHEMES
         ):  # pragma: no cover
-            raise ValueError(f"invalid protection scheme: {protection!r}")
+            msg = f"invalid protection scheme: {protection!r}"
+            raise ValueError(msg)
 
         if passphrase:
             passphrase = memoryview(passphrase).tobytes()
 
         kwargs: dict[str, typing.Any] = {}
         if encoding == "PEM":
             self._set_pem_args(format, passphrase, protection, kwargs)
         elif encoding == "DER":
             self._set_der_args(format, passphrase, protection, kwargs)
 
         try:
             key = self._key.export_key(**kwargs)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
         return key if isinstance(key, bytes) else key.encode()
 
     @classmethod
     def _set_pem_args(
         cls,
         format: str,
         passphrase: bytes | None,
@@ -171,15 +177,16 @@
         if format == "PKCS8":
             kwargs["use_pkcs8"] = True
             cls._set_pkcs8_passphrase_args(passphrase, protection, kwargs)
         elif format == "PKCS1":
             kwargs["use_pkcs8"] = False
             cls._set_pkcs1_passphrase_args(passphrase, protection, kwargs)
         else:
-            raise ValueError(f"Invalid format for PEM: {format!r}")
+            msg = f"Invalid format for PEM: {format!r}"
+            raise ValueError(msg)
 
     @classmethod
     def _set_der_args(
         cls,
         format: str,
         passphrase: bytes | None,
         protection: str | None,
@@ -189,38 +196,41 @@
         if format == "PKCS8":
             kwargs["use_pkcs8"] = True
             cls._set_pkcs8_passphrase_args(passphrase, protection, kwargs)
         elif format == "PKCS1":
             kwargs["use_pkcs8"] = False
             cls._set_pkcs1_passphrase_args(passphrase, protection, kwargs)
         else:
-            raise ValueError(f"Invalid format for DER: {format!r}")
+            msg = f"Invalid format for DER: {format!r}"
+            raise ValueError(msg)
 
     @classmethod
     def _set_pkcs8_passphrase_args(
         cls,
         passphrase: bytes | None,
         protection: str | None,
         kwargs: dict,
     ) -> None:
         if not passphrase and protection:
-            raise ValueError("Using protection without passphrase is invalid")
+            msg = "Using protection without passphrase is invalid"
+            raise ValueError(msg)
         kwargs["passphrase"] = passphrase
         kwargs["protection"] = (
             protection if protection else cls._DEFAULT_PROTECTION
         )
 
     @staticmethod
     def _set_pkcs1_passphrase_args(
         passphrase: bytes | None,
         protection: str | None,
         kwargs: dict,
     ) -> None:
         if protection is not None:  # pragma: no cover
-            raise ValueError("protection is meaningful only for PKCS8")
+            msg = "protection is meaningful only for PKCS8"
+            raise ValueError(msg)
         if passphrase is not None:
             kwargs["passphrase"] = passphrase
 
     def signer(
         self,
         algorithm: None | base.BaseEllepticCurveSignatureAlgorithm = None,
     ) -> SignerContext | EdDSASignerContext:
@@ -241,36 +251,36 @@
 
     def exchange(
         self,
         peer_public_key: bytes | ECCPublicKey | base.BaseECCPublicKey,
         algorithm: None | base.BaseEllepticCurveExchangeAlgorithm = None,
     ) -> bytes:
         del peer_public_key, algorithm
-        raise NotImplementedError(
-            "key exchange is currently not supported by the backend."
-        )
+        msg = "key exchange is currently not supported by the backend."
+        raise NotImplementedError(msg)
 
     @classmethod
     def load(
         cls,
         data: bytes,
         passphrase: bytes | None = None,
         *,
         curve: str | None = None,
     ) -> ECCPrivateKey:
         if curve is not None:
-            raise NotImplementedError(
-                "Cryptodome does not support Raw encoded private keys yet."
-            )
+            msg = "Cryptodome does not support Raw encoded private keys yet."
+            raise NotImplementedError(msg)
         try:
             key = ECC.import_key(data, passphrase)  # type: ignore
             if not key.has_private():
-                raise ValueError("The key is not a private key")
+                msg = "The key is not a private key"
+                raise ValueError(msg)
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
         return cls(None, _key=key)
 
 
 class ECCPublicKey(base.BaseECCPublicKey):
     """Represents ECC public key."""
 
     # Encodings supported by this key.
@@ -335,76 +345,82 @@
 
         Raises:
             ValueError: if the encoding or format is invalid.
         """
         try:
             encoding, format = self._ENCODINGS[encoding], self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(f"Invalid encoding or format: {e}") from e
+            msg = f"Invalid encoding or format: {e}"
+            raise ValueError(msg) from e
 
         kwargs: dict[str, typing.Any] = {}
         if encoding == "SEC1":
             self._set_sec1_args(format, kwargs)
         elif encoding == "OpenSSH":
             self._set_openssh_args(format, kwargs)
         elif encoding == "raw":
             if self.curve in _Curves.NIST_CURVES:
-                raise ValueError(
-                    "Failed to serialize key: NIST curves do not support Raw "
-                    "encoding. Use SEC1 instead."
-                )
+                msg = "Failed to serialize key: NIST curves do not support Raw"
+                "encoding. Use SEC1 instead."
+                raise ValueError(msg)
             self._set_raw_args(format, kwargs)
         elif encoding == "PEM":
             self._set_pem_args(format, kwargs)
         elif encoding == "DER":
             self._set_der_args(format, kwargs)
 
         try:
             data = self._key.export_key(**kwargs)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
         return data if isinstance(data, bytes) else data.encode("utf-8")
 
     @staticmethod
     def _set_sec1_args(format: str, kwargs: dict) -> None:
         kwargs["format"] = "SEC1"
         if format == "UncompressedPoint":
             kwargs["compress"] = False
         elif format == "CompressedPoint":
             kwargs["compress"] = True
         else:
-            raise ValueError(f"Invalid format for SEC1: {format!r}")
+            msg = f"Invalid format for SEC1: {format!r}"
+            raise ValueError(msg)
 
     @staticmethod
     def _set_openssh_args(format: str, kwargs: dict) -> None:
         if format == "OpenSSH":
             kwargs["format"] = "OpenSSH"
             return
-        raise ValueError(f"Invalid format for OpenSSH: {format!r}")
+        msg = f"Invalid format for OpenSSH: {format!r}"
+        raise ValueError(msg)
 
     @staticmethod
     def _set_raw_args(format: str, kwargs: dict) -> None:
         if format == "raw":
             kwargs["format"] = "raw"
             return
-        raise ValueError(f"Invalid format for Raw: {format!r}")
+        msg = f"Invalid format for Raw: {format!r}"
+        raise ValueError(msg)
 
     @staticmethod
     def _set_pem_args(format: str, kwargs: dict) -> None:
         if format == "SubjectPublicKeyInfo":
             kwargs["format"] = "PEM"
             return
-        raise ValueError(f"Invalid format for PEM: {format!r}")
+        msg = f"Invalid format for PEM: {format!r}"
+        raise ValueError(msg)
 
     @staticmethod
     def _set_der_args(format: str, kwargs: dict) -> None:
         if format == "SubjectPublicKeyInfo":
             kwargs["format"] = "DER"
             return
-        raise ValueError(f"Invalid format for DER: {format!r}")
+        msg = f"Invalid format for DER: {format!r}"
+        raise ValueError(msg)
 
     def verifier(
         self,
         algorithm: None | base.BaseEllepticCurveSignatureAlgorithm = None,
     ) -> VerifierContext | EdDSAVerifierContext:
         if self.curve.lower().startswith("ed"):
             algorithm = EdDSA() if algorithm is None else algorithm
@@ -442,17 +458,19 @@
         """
         try:
             if curve in _Curves.EDWARDS_CURVES:
                 key = eddsa.import_public_key(data)
             else:
                 key = ECC.import_key(data, curve_name=curve)
                 if key.has_private():
-                    raise ValueError("The key is not a private key")
+                    msg = "The key is not a private key"
+                    raise ValueError(msg)
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
         return cls(key)
 
 
 class SignerContext(base.BaseSignerContext):
     def __init__(self, ctx: typing.Any) -> None:
         self._ctx = ctx
 
@@ -491,14 +509,15 @@
         # catch is that Cryptodome requires its own hash object. It's too much
         # of an hassle. We will use PureEdDSA only.
         if isinstance(msghash, bytes):
             try:
                 return self._ctx.verify(msghash, signature)
             except ValueError as e:
                 raise exc.SignatureError from e
+        return None
 
 
 def generate(curve: str) -> ECCPrivateKey:
     """
     Generate a private key with given curve ``curve``.
 
     Args:
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/Hash.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/Hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     KangarooTwelve,
     TupleHash128,
     TupleHash256,
     cSHAKE128,
     cSHAKE256,
 )
 
-from ... import base, exc
+from pyflocker.ciphers import base, exc
 
 HASHES = {
     "sha224": SHA224.new,
     "sha256": SHA256.new,
     "sha384": SHA384.new,
     "sha512": SHA512.new,
     "sha512_224": lambda data=b"": SHA512.new(data, "224"),
@@ -150,15 +150,16 @@
     def name(self) -> str:
         return self._name
 
     @property
     def oid(self) -> str:  # pragma: no cover
         """The ASN.1 Object ID."""
         if self._oid is NotImplemented:
-            raise AttributeError(f"OID not available for {self.name!r}")
+            msg = f"OID not available for {self.name!r}"
+            raise AttributeError(msg)
         return self._oid  # type: ignore
 
     def update(self, data: bytes) -> None:
         if self._ctx is None:
             raise exc.AlreadyFinalized
         self._ctx.update(data)
 
@@ -178,15 +179,16 @@
     def copy(self) -> Hash:
         if self._ctx is None:
             raise exc.AlreadyFinalized
 
         try:
             hashobj = self._ctx.copy()
         except AttributeError as e:
-            raise ValueError(f"copying not supported by {self.name!r}") from e
+            msg = f"copying not supported by {self.name!r}"
+            raise ValueError(msg) from e
 
         return type(self)(
             self.name,
             digest_size=self.digest_size,
             _copy=hashobj,
         )
 
@@ -221,15 +223,16 @@
         Creates a Cryptodome based hash function object.
         """
         hashfunc = HASHES[name]
 
         digest_size_kwargs = {}
         if name in VAR_DIGEST_SIZE:
             if digest_size is None:
-                raise ValueError("digest_size is required")
+                msg = "digest_size is required"
+                raise ValueError(msg)
             # XOFs have the `read()` API, which is frustrating!
             if name not in XOFS:
                 digest_size_kwargs = {"digest_bytes": digest_size}
 
         custom_kwargs = {}
         if name in SUPPORTS_CUSTOM and custom is not None:
             custom_kwargs = {"custom": custom}
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/RSA.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/RSA.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import typing
 
 from Cryptodome.PublicKey import RSA
 
-from ... import base, exc
-from ..asymmetric import OAEP, PSS
+from pyflocker.ciphers import base, exc
+from pyflocker.ciphers.backends.asymmetric import OAEP, PSS
+
 from .asymmetric import PROTECTION_SCHEMES, get_padding_algorithm
 
 
 class RSAPrivateKey(base.BaseRSAPrivateKey):
     # Encodings supported by this key.
     _ENCODINGS = {
         "PEM": "PEM",
@@ -32,15 +33,16 @@
         e: int = 65537,
         _key: RSA.RsaKey | None = None,
     ) -> None:
         if _key is not None:
             self._key = _key
         else:
             if not isinstance(n, int):  # pragma: no cover
-                raise TypeError("n must be an integer value")
+                msg = "n must be an integer value"
+                raise TypeError(msg)
             self._key = RSA.generate(n, e=e)
 
     @property
     def p(self) -> int:
         return self._key.p
 
     @property
@@ -119,34 +121,37 @@
                 If the encoding or format is incorrect or,
                 if DER is used with PKCS1 or,
                 protection value is supplied with PKCS1 format.
         """
         try:
             encoding, format = self._ENCODINGS[encoding], self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(f"Invalid encoding or format: {e}") from e
+            msg = f"Invalid encoding or format: {e}"
+            raise ValueError(msg) from e
 
         if (
             protection is not None and protection not in PROTECTION_SCHEMES
         ):  # pragma: no cover
-            raise ValueError(f"invalid protection scheme: {protection!r}")
+            msg = f"invalid protection scheme: {protection!r}"
+            raise ValueError(msg)
 
         if passphrase:
             passphrase = memoryview(passphrase).tobytes()
 
         kwargs: dict[str, typing.Any] = {}
         if encoding == "PEM":
             self._set_pem_args(format, passphrase, protection, kwargs)
         elif encoding == "DER":
             self._set_der_args(format, passphrase, protection, kwargs)
 
         try:
             key: str | bytes = self._key.export_key(**kwargs)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
         return key if isinstance(key, bytes) else key.encode()
 
     @classmethod
     def _set_pem_args(
         cls,
         format: str,
         passphrase: bytes | None,
@@ -157,15 +162,16 @@
         if format == "PKCS8":
             kwargs["pkcs"] = 8
             cls._set_pkcs8_passphrase_args(passphrase, protection, kwargs)
         elif format == "PKCS1":
             kwargs["pkcs"] = 1
             cls._set_pkcs1_passphrase_args(passphrase, protection, kwargs)
         else:
-            raise ValueError(f"Invalid format for PEM: {format!r}")
+            msg = f"Invalid format for PEM: {format!r}"
+            raise ValueError(msg)
 
     @classmethod
     def _set_der_args(
         cls,
         format: str,
         passphrase: bytes | None,
         protection: str | None,
@@ -175,63 +181,70 @@
         if format == "PKCS8":
             kwargs["pkcs"] = 8
             cls._set_pkcs8_passphrase_args(passphrase, protection, kwargs)
         elif format == "PKCS1":
             kwargs["pkcs"] = 1
             cls._set_pkcs1_passphrase_args(passphrase, protection, kwargs)
         else:
-            raise ValueError(f"Invalid format for DER: {format!r}")
+            msg = f"Invalid format for DER: {format!r}"
+            raise ValueError(msg)
 
     @classmethod
     def _set_pkcs8_passphrase_args(
         cls,
         passphrase: bytes | None,
         protection: str | None,
         kwargs: dict,
     ) -> None:
         if not passphrase and protection:
-            raise ValueError("Using protection without passphrase is invalid")
+            msg = "Using protection without passphrase is invalid"
+            raise ValueError(msg)
         kwargs["passphrase"] = passphrase
         kwargs["protection"] = (
             protection if protection else cls._DEFAULT_PROTECTION
         )
 
     @staticmethod
     def _set_pkcs1_passphrase_args(
         passphrase: bytes | None,
         protection: str | None,
         kwargs: dict,
     ) -> None:
         if protection is not None:  # pragma: no cover
-            raise ValueError("protection is meaningful only for PKCS8")
+            msg = "protection is meaningful only for PKCS8"
+            raise ValueError(msg)
         if passphrase is not None:
             kwargs["passphrase"] = passphrase
 
     @staticmethod
     def _validate_pkcs1_args(
         encoding: str,
         protection: str | None,
     ) -> None:
         if protection is not None:  # pragma: no cover
-            raise ValueError("protection is meaningful only for PKCS8")
+            msg = "protection is meaningful only for PKCS8"
+            raise ValueError(msg)
         if encoding == "DER":
-            raise ValueError("cannot use DER with PKCS1 format")
+            msg = "cannot use DER with PKCS1 format"
+            raise ValueError(msg)
 
     @classmethod
     def load(
         cls,
         data: bytes,
         passphrase: bytes | None = None,
     ) -> RSAPrivateKey:
         try:
             key = RSA.import_key(data, passphrase)  # type: ignore
             if not key.has_private():
-                raise ValueError("The key is not a private key")
+                msg = "The key is not a private key"
+                raise ValueError(msg)
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
         return cls(None, _key=key)
 
 
 class RSAPublicKey(base.BaseRSAPublicKey):
     # Encodings supported by this key.
     _ENCODINGS = {
         "PEM": "PEM",
@@ -306,59 +319,66 @@
             ValueError:
                 if the encoding or format is not supported or invalid,
                 or OpenSSH encoding is not used with OpenSSH format.
         """
         try:
             encoding, format = self._ENCODINGS[encoding], self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(f"Invalid encoding or format: {e}") from e
+            msg = f"Invalid encoding or format: {e}"
+            raise ValueError(msg) from e
 
         kwargs: dict[str, typing.Any] = {}
         if encoding == "OpenSSH":
             self._set_openssh_args(format, kwargs)
         elif encoding == "PEM":
             self._set_pem_args(format, kwargs)
         elif encoding == "DER":
             self._set_der_args(format, kwargs)
 
         try:
             data: str | bytes = self._key.export_key(**kwargs)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
         return data if isinstance(data, bytes) else data.encode("utf-8")
 
     @staticmethod
     def _set_openssh_args(format: str, kwargs: dict) -> None:
         if format == "OpenSSH":
             kwargs["format"] = "OpenSSH"
             return
-        raise ValueError(f"Invalid format for OpenSSH: {format!r}")
+        msg = f"Invalid format for OpenSSH: {format!r}"
+        raise ValueError(msg)
 
     @staticmethod
     def _set_pem_args(format: str, kwargs: dict) -> None:
         if format == "SubjectPublicKeyInfo":
             kwargs["format"] = "PEM"
             return
-        raise ValueError(f"Invalid format for PEM: {format!r}")
+        msg = f"Invalid format for PEM: {format!r}"
+        raise ValueError(msg)
 
     @staticmethod
     def _set_der_args(format: str, kwargs: dict) -> None:
         if format == "SubjectPublicKeyInfo":
             kwargs["format"] = "DER"
             return
-        raise ValueError(f"Invalid format for DER: {format!r}")
+        msg = f"Invalid format for DER: {format!r}"
+        raise ValueError(msg)
 
     @classmethod
     def load(cls, data: bytes) -> RSAPublicKey:
         try:
             key = RSA.import_key(data)
             if key.has_private():
-                raise ValueError("The key is not a private key")
+                msg = "The key is not a private key"
+                raise ValueError(msg)
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
         return cls(key)
 
 
 class EncryptorContext(base.BaseEncryptorContext):
     def __init__(self, ctx: typing.Any) -> None:
         self._ctx = ctx
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/asymmetric.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/asymmetric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import typing
 
 from Cryptodome.Cipher import PKCS1_OAEP
 from Cryptodome.Signature import DSS, eddsa, pss
 
-from .. import asymmetric
+from pyflocker.ciphers.backends import asymmetric
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     from Cryptodome.PublicKey.ECC import EccKey
     from Cryptodome.PublicKey.RSA import RsaKey
 
-    from ... import base
+    from pyflocker.ciphers import base
 
 
 def get_OAEP(
     key: RsaKey,
     padding: base.BaseAsymmetricPadding,
 ) -> PKCS1_OAEP.PKCS1OAEP_Cipher:
     """Construct a Cryptodome specific OAEP object.
@@ -25,17 +25,19 @@
         padding: An OAEP object.
 
     Returns:
         An OAEP encryptor/decryptor object depending on the key, from the
         Cryptodome backend.
     """
     if not isinstance(padding, asymmetric.OAEP):  # pragma: no cover
-        raise TypeError("padding must be an OAEP object")
+        msg = "padding must be an OAEP object"
+        raise TypeError(msg)
     if not isinstance(padding.mgf, asymmetric.MGF1):
-        raise TypeError("mgf must be an MGF1 instance")
+        msg = "mgf must be an MGF1 instance"
+        raise TypeError(msg)
 
     return PKCS1_OAEP.new(
         key,
         padding.hashfunc.new(),  # type: ignore
         lambda x, y: pss.MGF1(
             x,
             y,
@@ -52,17 +54,19 @@
         key: Public/Private key (from the Cryptodome backend).
         padding: A PSS object.
 
     Returns:
         An PSS signer/verifier object, depending on the key.
     """
     if not isinstance(padding, asymmetric.PSS):  # pragma: no cover
-        raise TypeError("padding must be a PSS object")
+        msg = "padding must be a PSS object"
+        raise TypeError(msg)
     if not isinstance(padding.mgf, asymmetric.MGF1):
-        raise TypeError("mgf must be an MGF1 instance")
+        msg = "mgf must be an MGF1 instance"
+        raise TypeError(msg)
 
     if padding.salt_length is None:
         return _SaltLengthMaximizer(key, padding)
 
     return pss.new(
         key,
         mask_func=lambda x, y: pss.MGF1(  # type: ignore
@@ -86,27 +90,29 @@
     Args:
         key: An ECC key object from ``Cryptodome`` backend.
         algorithm: The algorithm to use.
 
     Returns: Signer/Verifier instance.
     """
     if not isinstance(algorithm, asymmetric.ECDSA):  # pragma: no cover
-        raise TypeError("algorithm must be an instance of ECDSA")
+        msg = "algorithm must be an instance of ECDSA"
+        raise TypeError(msg)
     return DSS.new(key, mode="fips-186-3", encoding="der")  # type: ignore
 
 
 def get_EdDSA(
     key: EccKey,
     algorithm: asymmetric.BaseEllepticCurveSignatureAlgorithm,
 ) -> eddsa.EdDSASigScheme:
     if not isinstance(algorithm, asymmetric.EdDSA):
-        raise TypeError("algorithm must be an instance of EdDSA")
+        msg = "algorithm must be an instance of EdDSA"
+        raise TypeError(msg)
     return eddsa.new(
         key,
-        mode=algorithm.mode,  # type: ignore
+        mode=algorithm.mode,
         context=algorithm.context,
     )
 
 
 class _SaltLengthMaximizer:
     """
     Custom sign/verify wrapper over PSS to preserve consistency.
@@ -131,15 +137,16 @@
         )
         if signature is None:
             return pss.sign(msghash)
         return pss.verify(msghash, signature)
 
     def sign(self, msghash: typing.Any) -> bytes:
         if not self._key.has_private():
-            raise TypeError("The key is not a private key.")
+            msg = "The key is not a private key."
+            raise TypeError(msg)
         return self._sign_or_verify(msghash)
 
     def verify(self, msghash: typing.Any, signature: bytes) -> None:
         return self._sign_or_verify(msghash, signature)
 
 
 PADDINGS: dict[type[base.BaseAsymmetricPadding], typing.Callable] = {
@@ -171,23 +178,21 @@
     padding: base.BaseAsymmetricPadding,
     *args: typing.Any,
     **kwargs: typing.Any,
 ) -> typing.Any:
     try:
         return PADDINGS[type(padding)](*args, **kwargs)
     except KeyError as e:
-        raise TypeError(
-            f"Invalid padding algorithm type: {type(padding)}"
-        ) from e
+        msg = f"Invalid padding algorithm type: {type(padding)}"
+        raise TypeError(msg) from e
 
 
 def get_ec_signature_algorithm(
     algorithm: base.BaseEllepticCurveSignatureAlgorithm,
     *args: typing.Any,
     **kwargs: typing.Any,
 ) -> typing.Any:
     try:
         return EC_SIGNATURE_ALGORITHMS[type(algorithm)](*args, **kwargs)
     except KeyError as e:
-        raise TypeError(
-            f"Invalid signature algorithm type: {type(algorithm)}"
-        ) from e
+        msg = f"Invalid signature algorithm type: {type(algorithm)}"
+        raise TypeError(msg) from e
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/misc.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Miscellaneous Tools: Tools that are not common to symmetric or asymmetric.
 """
 
 from __future__ import annotations
 
 from Cryptodome.Protocol import KDF
 
-from ...base import BaseHash
+from pyflocker.ciphers.base import BaseHash
 
 
 def derive_hkdf_key(
     master_key: bytes,
     dklen: int,
     hashalgo: BaseHash,
     salt: bytes,
@@ -27,15 +27,16 @@
         cipher_ctx: Context for cipher.
         auth_ctx: Context for HMAC.
 
     Returns:
         A pair of *cipher key* and *MAC key*.
     """
     if not isinstance(hashalgo, BaseHash):
-        raise TypeError("hashalgo must be an object implementing BaseHash.")
+        msg = "hashalgo must be an object implementing BaseHash."
+        raise TypeError(msg)
 
     hash_ = hashalgo.new()
 
     key = KDF.HKDF(
         master=master_key,
         key_len=dklen,
         salt=salt,
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptodome_/symmetric.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptodome_/symmetric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Cryptodome backend specific templates and tools for symmetric ciphers."""
 
 from __future__ import annotations
 
 import typing
 
-from ... import base, exc
+from pyflocker.ciphers import base, exc
 
 
 class NonAEADCipherTemplate(base.BaseNonAEADCipher):
     """
     Template class to provide the default behavior of BaseNonAEADCipher.
 
     Subclasses need to provide:
@@ -84,15 +84,16 @@
 
         if self.is_encrypting():  # type: ignore
             self._tag, self._cipher = self._cipher.digest(), None
             self._update_func = None  # type: ignore
             return
 
         if tag is None:
-            raise ValueError("tag is required for finalization")
+            msg = "tag is required for finalization"
+            raise ValueError(msg)
 
         cipher, self._cipher = self._cipher, None
         self._update_func = None  # type: ignore
         try:
             cipher.verify(tag)
         except ValueError as e:
             raise exc.DecryptionError from e
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/AES.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/AES.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,34 @@
 import struct
 import typing
 from types import MappingProxyType
 
 import cryptography.exceptions as bkx
 from cryptography.hazmat.backends import default_backend as defb
 from cryptography.hazmat.primitives import cmac
-from cryptography.hazmat.primitives.ciphers import Cipher as CrCipher
-from cryptography.hazmat.primitives.ciphers import aead
-from cryptography.hazmat.primitives.ciphers import algorithms as algo
-from cryptography.hazmat.primitives.ciphers import modes
-
-from ... import base, exc
-from ... import modes as modes_
-from ...modes import Modes
-from ..symmetric import (
+from cryptography.hazmat.primitives.ciphers import (
+    Cipher as CrCipher,
+    aead,
+    algorithms as algo,
+    modes,
+)
+
+from pyflocker.ciphers import (
+    base,
+    exc,
+    modes as modes_,
+)
+from pyflocker.ciphers.backends.symmetric import (
     FileCipherWrapper,
     HMACWrapper,
     _DecryptionCtx,
     _EncryptionCtx,
 )
+from pyflocker.ciphers.modes import Modes
+
 from . import Hash
 from .misc import derive_hkdf_key
 from .symmetric import AEADCipherTemplate, NonAEADCipherTemplate
 
 if typing.TYPE_CHECKING:
     import io
 
@@ -49,15 +55,15 @@
 class AEAD(AEADCipherTemplate):
     def __init__(
         self,
         encrypting: bool,
         key: bytes,
         mode: Modes,
         nonce: bytes,
-    ):
+    ) -> None:
         self._encrypting = encrypting
         self._updated = False
         self._tag = None
         self._mode = mode
 
         cipher = _aes_cipher(key, mode, nonce)
         # cryptography already provides a context
@@ -75,15 +81,15 @@
 class NonAEAD(NonAEADCipherTemplate):
     def __init__(
         self,
         encrypting: bool,
         key: bytes,
         mode: Modes,
         nonce: bytes,
-    ):
+    ) -> None:
         self._encrypting = encrypting
         self._mode = mode
 
         cipher = _aes_cipher(key, mode, nonce)
         # cryptography already provides a context
         if encrypting:
             self._ctx = cipher.encryptor()
@@ -99,15 +105,15 @@
 class AEADOneShot(base.BaseAEADOneShotCipher):
     def __init__(
         self,
         encrypting: bool,
         key: bytes,
         mode: Modes,
         nonce: bytes,
-    ):
+    ) -> None:
         cipher = _aes_cipher(key, mode, nonce)
 
         self._mode = mode
         self._encrypting = encrypting
         self._aad = b""
         self._tag = None
         self._nonce = nonce
@@ -140,15 +146,16 @@
         if self.is_encrypting():
             ctxt_tag = self._update_func(self._nonce, data, self._aad)
             self._tag = ctxt_tag[-self._tag_length :]
             self.finalize(tag)
             return ctxt_tag[: -self._tag_length]
 
         if tag is None:
-            raise ValueError("tag is required for decryption.")
+            msg = "tag is required for decryption."
+            raise ValueError(msg)
 
         try:
             data = self._update_func(self._nonce, data + tag, self._aad)
         except bkx.InvalidTag:
             self._raise_on_tag_err = True
         finally:
             self.finalize(tag)
@@ -164,15 +171,16 @@
         raise NotImplementedError
 
     def finalize(self, tag: bytes | None = None) -> None:
         if self._update_func is None:
             raise exc.AlreadyFinalized
 
         if not self.is_encrypting() and tag is None:
-            raise ValueError("tag is required for decryption.")
+            msg = "tag is required for decryption."
+            raise ValueError(msg)
 
         self._update_func = None
         if self._raise_on_tag_err:
             raise exc.DecryptionError
 
     def calculate_tag(self) -> bytes | None:
         if self._update_func is not None:
@@ -181,15 +189,15 @@
 
 
 class _AuthWrapper:
     """Wrapper class for objects that do not support memoryview objects."""
 
     __slots__ = ("_auth",)
 
-    def __init__(self, auth: typing.Any):
+    def __init__(self, auth: typing.Any) -> None:
         self._auth = auth
 
     def update(self, data: bytes) -> None:
         self._auth.update(bytes(data))
 
     def __getattr__(self, name: str) -> typing.Any:
         return getattr(self._auth, name)
@@ -205,30 +213,29 @@
         "_omac_cache",
         "_cipher",
         "_updated",
         "__ctx",
         "__tag",
     )
 
-    def __init__(self, key: bytes, nonce: bytes, mac_len: int = 16):
+    def __init__(self, key: bytes, nonce: bytes, mac_len: int = 16) -> None:
         self._mac_len = mac_len
         self._omac = [cmac.CMAC(algo.AES(key), defb()) for _ in range(3)]
 
         for i in range(3):
             self._omac[i].update(
-                bytes(1) * (algo.AES.block_size // 8 - 1)
-                + struct.pack("B", i)  # noqa: W503
+                bytes(1) * (algo.AES.block_size // 8 - 1) + struct.pack("B", i)  # noqa: W503
             )
 
         self._omac[0].update(nonce)
         self._auth = _AuthWrapper(self._omac[1])
 
         # create a cache since cryptography allows us to calculate tag
         # only once... why...
-        self._omac_cache = []
+        self._omac_cache: list[bytes] = []
         self._omac_cache.append(self._omac[0].finalize())
 
         self._cipher = CrCipher(
             algo.AES(key),
             modes.CTR(self._omac_cache[0]),
             defb(),
         )
@@ -288,19 +295,17 @@
     def finalize(self) -> None:
         """Finalizes the cipher."""
         if self.__ctx is None:  # pragma: no cover
             raise bkx.AlreadyFinalized
 
         tag = bytes(typing.cast("int", algo.AES.block_size) // 8)
         for i in range(3):
-            try:
-                tag = strxor(tag, self._omac_cache[i])
-            except IndexError:
+            if i >= len(self._omac_cache):
                 self._omac_cache.append(self._omac[i].finalize())
-                tag = strxor(tag, self._omac_cache[i])
+            tag = strxor(tag, self._omac_cache[i])
         self.__tag, self.__ctx = tag[: self._mac_len], None
 
     def finalize_with_tag(self, tag: bytes) -> None:
         self.finalize()
         assert self.__tag is not None
         if not hmac.compare_digest(tag, self.__tag):
             raise bkx.InvalidTag  # pragma: no cover
@@ -323,15 +328,15 @@
     mode: Modes,
     iv_or_nonce: bytes,
     *,
     use_hmac: bool = False,
     tag_length: int | None = 16,
     digestmod: None | base.BaseHash = None,
     file: io.BufferedReader | None = None,
-) -> AEAD | NonAEAD | FileCipherWrapper | HMACWrapper:
+) -> AEAD | NonAEAD | AEADOneShot | FileCipherWrapper | HMACWrapper:
     """Create a new backend specific AES cipher.
 
     Args:
         encrypting: True is encryption and False is decryption.
         key: The key for the cipher.
         mode: The mode to use for AES cipher.
         iv_or_nonce:
@@ -368,47 +373,52 @@
     Raises:
         NotImplementedError:
             if the ``mode`` does not support encryption/decryption of files.
 
     Note:
         Any other error that is raised is from the backend itself.
     """
-    crp: typing.Any
+    cipher: base.BaseAEADCipher | base.BaseNonAEADCipher | FileCipherWrapper
 
     if mode not in supported_modes():
-        raise exc.UnsupportedMode(f"{mode.name} not supported.")
+        msg = f"{mode.name} not supported."
+        raise exc.UnsupportedMode(msg)
 
-    if file is not None:
-        use_hmac = True
+    is_mode_aead = mode in modes_.AEAD
+    is_file = file is not None
+    use_hmac = (is_file and not is_mode_aead) or (use_hmac and not is_mode_aead)
 
     if mode in modes_.SPECIAL:
-        if file is not None:
-            raise NotImplementedError(
-                f"{mode} does not support encryption/decryption of files."
+        if is_file:
+            msg = (
+                f"{mode.name} does not support encryption/decryption of files."
             )
-        crp = AEADOneShot(encrypting, key, mode, iv_or_nonce)
-    elif mode in modes_.AEAD:
-        crp = AEAD(encrypting, key, mode, iv_or_nonce)
+            raise NotImplementedError(msg)
+        return AEADOneShot(encrypting, key, mode, iv_or_nonce)
+
+    if is_mode_aead:
+        cipher = AEAD(encrypting, key, mode, iv_or_nonce)
     else:
-        if use_hmac:
-            crp = _wrap_hmac(
-                encrypting,
-                key,
-                mode,
-                iv_or_nonce,
-                digestmod if digestmod is not None else Hash.new("sha256"),
-                tag_length,
-            )
-        else:
-            crp = NonAEAD(encrypting, key, mode, iv_or_nonce)
+        cipher = NonAEAD(encrypting, key, mode, iv_or_nonce)
+
+    if use_hmac:
+        cipher = _wrap_hmac(
+            encrypting,
+            key,
+            mode,
+            iv_or_nonce,
+            digestmod or Hash.new("sha256"),
+            tag_length,
+        )
 
     if file:
-        crp = FileCipherWrapper(crp, file, offset=15)
+        assert isinstance(cipher, base.BaseAEADCipher)
+        cipher = FileCipherWrapper(cipher, file, offset=15)
 
-    return crp
+    return cipher
 
 
 def supported_modes() -> set[Modes]:
     """Lists all modes supported by AES cipher of this backend.
 
     Returns:
         set of :any:`Modes` object supported by backend.
@@ -419,17 +429,18 @@
 def _aes_cipher(key: bytes, mode: Modes, nonce_or_iv: bytes) -> typing.Any:
     if mode == Modes.MODE_EAX:
         return _EAX(key, nonce_or_iv)
 
     backend_mode = SUPPORTED[mode]
     assert backend_mode is not None
 
-    if mode in modes_.SPECIAL and mode == Modes.MODE_CCM:
+    if mode == Modes.MODE_CCM:
         if not 7 <= len(nonce_or_iv) <= 13:
-            raise ValueError("Length of nonce must be between 7 and 13 bytes")
+            msg = "Length of nonce must be between 7 and 13 bytes"
+            raise ValueError(msg)
         return backend_mode(key)
 
     assert not issubclass(backend_mode, aead.AESCCM)
     return CrCipher(algo.AES(key), backend_mode(nonce_or_iv))
 
 
 def _wrap_hmac(
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/Camellia.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/Camellia.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
 import typing
 
-from cryptography.hazmat.primitives.ciphers import Cipher
-from cryptography.hazmat.primitives.ciphers import algorithms as algo
-from cryptography.hazmat.primitives.ciphers import modes
-
-from ... import exc
-from ...modes import Modes
-from ..symmetric import FileCipherWrapper, HMACWrapper
+from cryptography.hazmat.primitives.ciphers import (
+    Cipher,
+    algorithms as algo,
+    modes,
+)
+
+from pyflocker.ciphers import exc
+from pyflocker.ciphers.backends.symmetric import FileCipherWrapper, HMACWrapper
+from pyflocker.ciphers.modes import Modes
+
 from . import Hash
 from .misc import derive_hkdf_key
 from .symmetric import NonAEADCipherTemplate
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import io
 
-    from ... import base
+    from pyflocker.ciphers import base
 
 SUPPORTED = {
     Modes.MODE_CFB: modes.CFB,
     Modes.MODE_CTR: modes.CTR,
     Modes.MODE_OFB: modes.OFB,
 }
 
@@ -30,17 +33,18 @@
 
     def __init__(
         self,
         encrypting: bool,
         key: bytes,
         mode: Modes,
         iv_or_nonce: bytes,
-    ):
+    ) -> None:
         if mode not in supported_modes():
-            raise exc.UnsupportedMode(f"{mode.name} not supported.")
+            msg = f"{mode.name} not supported."
+            raise exc.UnsupportedMode(msg)
 
         cipher = Cipher(
             algo.Camellia(key),
             SUPPORTED[mode](iv_or_nonce),  # type: ignore
         )
         self._ctx = (
             cipher.encryptor()  # type: ignore[misc]
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/ChaCha20.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/ChaCha20.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,33 +2,41 @@
 
 from __future__ import annotations
 
 import typing
 
 from cryptography import exceptions as bkx
 from cryptography.hazmat.backends import default_backend as defb
-from cryptography.hazmat.primitives.ciphers import Cipher
-from cryptography.hazmat.primitives.ciphers import algorithms as algo
+from cryptography.hazmat.primitives.ciphers import (
+    Cipher,
+    algorithms as algo,
+)
 from cryptography.hazmat.primitives.poly1305 import Poly1305
 
-from ... import base, exc
-from ..symmetric import FileCipherWrapper, _DecryptionCtx, _EncryptionCtx
+from pyflocker.ciphers import base, exc
+from pyflocker.ciphers.backends.symmetric import (
+    FileCipherWrapper,
+    _DecryptionCtx,
+    _EncryptionCtx,
+)
+
 from .misc import derive_poly1305_key
 from .symmetric import NonAEADCipherTemplate
 
 if typing.TYPE_CHECKING:
     import io
 
 
 class ChaCha20Poly1305(base.BaseAEADCipher):
     """ChaCha20Poly1305 Cipher class."""
 
-    def __init__(self, encrypting: bool, key: bytes, nonce: bytes):
-        if not len(nonce) in (8, 12):
-            raise ValueError("A 8 or 12 byte nonce is required")
+    def __init__(self, encrypting: bool, key: bytes, nonce: bytes) -> None:
+        if len(nonce) not in (8, 12):
+            msg = "A 8 or 12 byte nonce is required"
+            raise ValueError(msg)
         if len(nonce) == 8:
             nonce = bytes(4) + nonce
 
         cipher = Cipher(
             algo.ChaCha20(key, (1).to_bytes(4, "little") + nonce),
             None,
         )
@@ -86,15 +94,16 @@
         self._len_ct += len(out)
         self._ctx.update_into(data, out)
 
     def finalize(self, tag: bytes | None = None) -> None:
         if self._ctx is None:
             raise exc.AlreadyFinalized
         if not self.is_encrypting() and tag is None:
-            raise ValueError("tag is required for decryption")
+            msg = "tag is required for decryption"
+            raise ValueError(msg)
 
         self._pad_aad()
 
         if self._len_ct & 0x0F:
             self._auth.update(bytes(16 - (self._len_ct & 0x0F)))
 
         self._auth.update(self._len_aad.to_bytes(8, "little"))
@@ -123,17 +132,18 @@
     """ChaCha20 Cipher class.
 
     This class alone does not provide any authentication. For AEAD purposes,
     wrap ``ChaCha20`` object with a class that implements ``BaseAEADCipher`` or
     use ``ChaCha20Poly1305``.
     """
 
-    def __init__(self, encrypting: bool, key: bytes, nonce: bytes):
-        if not len(nonce) in (8, 12):
-            raise ValueError("A 8 or 12 byte nonce is required")
+    def __init__(self, encrypting: bool, key: bytes, nonce: bytes) -> None:
+        if len(nonce) not in (8, 12):
+            msg = "A 8 or 12 byte nonce is required"
+            raise ValueError(msg)
         if len(nonce) == 8:
             nonce = bytes(4) + nonce
 
         cipher = Cipher(
             algo.ChaCha20(
                 key,
                 bytes(4) + nonce,
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/DH.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/DH.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     ParameterFormat,
     PrivateFormat,
     PublicFormat,
 )
 
-from ... import base
+from pyflocker.ciphers import base
 
 
 class DHParameters(base.BaseDHParameters):
     _ENCODINGS = {
         "PEM": Encoding.PEM,
         "DER": Encoding.DER,
     }
@@ -35,15 +35,16 @@
         generator: int = 2,
         _params: dh.DHParameters | None = None,
     ) -> None:
         if _params is not None:
             self._params = _params
         else:
             if not isinstance(key_size, int):  # pragma: no cover
-                raise TypeError("key_size must be an integer")
+                msg = "key_size must be an integer"
+                raise TypeError(msg)
             self._params = dh.generate_parameters(generator, key_size)
 
         numbers = self._params.parameter_numbers()
         self._g = numbers.g
         self._p = numbers.p
         self._q = numbers.q
 
@@ -76,45 +77,49 @@
         Raises:
             ValueError: if the encoding of format is invalid.
         """
         try:
             encd = self._ENCODINGS[encoding]
             fmt = self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(
-                f"The encoding or format is invalid: {e.args[0]!r}"
-            ) from e
+            msg = f"The encoding or format is invalid: {e.args[0]!r}"
+            raise ValueError(msg) from e
 
         try:
             return self._params.parameter_bytes(encd, fmt)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
 
     @classmethod
     def load(cls, data: bytes) -> DHParameters:
+        data = memoryview(data).tobytes()
         loader = cls._get_loader(data)
         try:
-            params = loader(memoryview(data))
+            params = loader(data)
             if not isinstance(params, dh.DHParameters):
-                raise ValueError("Data is not a DH parameter.")
+                msg = "Data is not a DH parameter."
+                raise ValueError(msg)
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
 
         return cls(None, _params=params)
 
     @classmethod
     def _get_loader(cls, data: bytes) -> typing.Callable:
         """
         Returns a loader function depending on the initial bytes of the
         parameter.
         """
         try:
             return cls._LOADERS[next(filter(data.startswith, cls._LOADERS))]
         except StopIteration:
-            raise ValueError("Invalid format.") from None
+            msg = "Invalid format."
+            raise ValueError(msg) from None
 
     @classmethod
     def load_from_parameters(
         cls,
         p: int,
         g: int = 2,
         q: int | None = None,
@@ -135,15 +140,16 @@
     _LOADERS = {
         b"-----": serial.load_pem_private_key,
         b"0": serial.load_der_private_key,
     }
 
     def __init__(self, key: dh.DHPrivateKey) -> None:
         if not isinstance(key, dh.DHPrivateKey):  # pragma: no cover
-            raise ValueError("The key is not a DH private key.")
+            msg = "The key is not a DH private key."
+            raise ValueError(msg)
         self._key = key
 
         numbers = key.private_numbers()
         self._x = numbers.x
 
     def parameters(self) -> DHParameters:
         return DHParameters(None, _params=self._key.parameters())
@@ -176,64 +182,68 @@
         format: str = "PKCS8",
         passphrase: bytes | None = None,
     ) -> bytes:
         try:
             encd = self._ENCODINGS[encoding]
             fmt = self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(
-                f"The encoding or format is invalid: {e.args[0]!r}"
-            ) from e
+            msg = f"The encoding or format is invalid: {e.args[0]!r}"
+            raise ValueError(msg) from e
 
         protection: serial.KeySerializationEncryption
         if passphrase is None:
             protection = serial.NoEncryption()
         else:
             protection = serial.BestAvailableEncryption(
                 memoryview(passphrase).tobytes()
             )
 
         try:
             return self._key.private_bytes(encd, fmt, protection)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
 
     @property
     def x(self) -> int:
         return self._x
 
     @classmethod
     def load(
         cls,
         data: bytes,
         passphrase: bytes | None = None,
     ) -> DHPrivateKey:
+        data = memoryview(data).tobytes()
         loader = cls._get_loader(data)
 
         if passphrase is not None:
             passphrase = memoryview(passphrase).tobytes()
 
         try:
-            key = loader(memoryview(data), passphrase)
+            key = loader(data, passphrase)
             if not isinstance(key, dh.DHPrivateKey):
-                raise ValueError("Key is not a DH private key.")
+                msg = "Key is not a DH private key."
+                raise ValueError(msg)
         except (ValueError, TypeError) as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
 
         return cls(key)
 
     @classmethod
     def _get_loader(cls, data: bytes) -> typing.Callable:
         """
         Returns a loader function depending on the initial bytes of the key.
         """
         try:
             return cls._LOADERS[next(filter(data.startswith, cls._LOADERS))]
         except StopIteration:
-            raise ValueError("Invalid format") from None
+            msg = "Invalid format"
+            raise ValueError(msg) from None
 
 
 class DHPublicKey(base.BaseDHPublicKey):
     _ENCODINGS = {
         "PEM": Encoding.PEM,
         "DER": Encoding.DER,
     }
@@ -245,15 +255,16 @@
     _LOADERS = {
         b"-----": serial.load_pem_public_key,
         b"0": serial.load_der_public_key,
     }
 
     def __init__(self, key: dh.DHPublicKey) -> None:
         if not isinstance(key, dh.DHPublicKey):  # pragma: no cover
-            raise ValueError("The key is not a DH public key.")
+            msg = "The key is not a DH public key."
+            raise ValueError(msg)
         self._key = key
         self._y = key.public_numbers().y
 
     def parameters(self) -> DHParameters:
         return DHParameters(None, _params=self._key.parameters())
 
     @property
@@ -277,48 +288,52 @@
         Raises:
             ValueError: if the encoding or format is invalid.
         """
         try:
             encd = self._ENCODINGS[encoding]
             fmt = self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(
-                f"Invalid encoding or format: {e.args[0]!r}"
-            ) from e
+            msg = f"Invalid encoding or format: {e.args[0]!r}"
+            raise ValueError(msg) from e
 
         try:
             return self._key.public_bytes(encd, fmt)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
 
     @property
     def y(self) -> int:
         return self._y
 
     @classmethod
     def load(cls, data: bytes) -> DHPublicKey:
+        data = memoryview(data).tobytes()
         loader = cls._get_loader(data)
         try:
-            key = loader(memoryview(data))
+            key = loader(data)
             if not isinstance(key, dh.DHPublicKey):
-                raise ValueError("Key is not a DH public key.")
+                msg = "Key is not a DH public key."
+                raise ValueError(msg)
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
 
         return cls(key)
 
     @classmethod
     def _get_loader(cls, data: bytes) -> typing.Callable:
         """
         Returns a loader function depending on the initial bytes of the key.
         """
         try:
             return cls._LOADERS[next(filter(data.startswith, cls._LOADERS))]
         except StopIteration:
-            raise ValueError("Invalid format.") from None
+            msg = "Invalid format."
+            raise ValueError(msg) from None
 
 
 def generate(key_size: int, g: int = 2) -> DHParameters:
     """
     Generate DHE parameter with prime number's bit size ``bits`` and
     generator ``g`` (default 2). Recommended size of ``bits`` > 1024.
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/ECC.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/ECC.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from cryptography.hazmat.primitives.asymmetric import ec, ed448, ed25519, utils
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     PrivateFormat,
     PublicFormat,
 )
 
-from ... import base, exc
-from ..asymmetric import ECDH, ECDSA, EdDSA
+from pyflocker.ciphers import base, exc
+from pyflocker.ciphers.backends.asymmetric import ECDH, ECDSA, EdDSA
+
 from . import Hash
 from .asymmetric import get_ec_exchange_algorithm, get_ec_signature_algorithm
 
 
 class _Curves:
     """Group curve names under one namespace."""
 
@@ -127,19 +128,21 @@
         _key: ec.EllipticCurvePrivateKey | None = None,
     ) -> None:
         if _key is not None:
             self._key = _key
             self._curve = _key.curve.name
         else:
             if not isinstance(curve, str):  # pragma: no cover
-                raise TypeError("curve name must be a string")
+                msg = "curve name must be a string"
+                raise TypeError(msg)
             try:
                 curve_obj = _Curves.CURVES[curve]()
             except KeyError as e:
-                raise ValueError(f"Invalid curve: {e.args[0]!r}") from e
+                msg = f"Invalid curve: {e.args[0]!r}"
+                raise ValueError(msg) from e
 
             if isinstance(curve_obj, ec.EllipticCurve):
                 self._key = ec.generate_private_key(curve_obj)
             else:
                 self._key = curve_obj
 
         self._key_size = self._key.key_size
@@ -158,15 +161,16 @@
 
     def exchange(
         self,
         peer_public_key: bytes | ECCPublicKey | base.BaseECCPublicKey,
         algorithm: None | base.BaseEllepticCurveExchangeAlgorithm = None,
     ) -> bytes:
         if isinstance(self._key, _EdDSAPrivateKeyAdapter):
-            raise NotImplementedError("EdDSA keys cannot perform key exchange")
+            msg = "EdDSA keys cannot perform key exchange"
+            raise NotImplementedError(msg)
 
         if algorithm is None:  # pragma: no cover
             algorithm = ECDH()
         algo = get_ec_exchange_algorithm(algorithm, algorithm)
         if isinstance(peer_public_key, bytes):
             return self._key.exchange(
                 algo,
@@ -200,15 +204,16 @@
 
         Warning:
             If the key is an ``EdDSA`` key, then the ``EdDSA`` parameters are
             ignored.
         """
         if self.curve.lower().startswith("ed"):
             if algorithm is not None and not isinstance(algorithm, EdDSA):
-                raise TypeError(f"Invalid signature algorithm: {algorithm}")
+                msg = f"Invalid signature algorithm: {algorithm}"
+                raise TypeError(msg)
             assert isinstance(self._key, _EdDSAPrivateKeyAdapter)
             return EdDSASignerContext(self._key)
 
         algorithm = ECDSA() if algorithm is None else algorithm
         return SignerContext(
             self._key,
             get_ec_signature_algorithm(algorithm, algorithm),
@@ -248,30 +253,30 @@
             ValueError: If the encoding or format is incorrect, or
             serialization failed.
         """
         try:
             encd = self._ENCODINGS[encoding]
             fmt = self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(
-                f"The encoding or format is invalid: {e.args[0]!r}"
-            ) from e
+            msg = f"The encoding or format is invalid: {e.args[0]!r}"
+            raise ValueError(msg) from e
 
         protection: serial.KeySerializationEncryption
         if passphrase is None:
             protection = serial.NoEncryption()
         else:
             protection = serial.BestAvailableEncryption(
                 memoryview(passphrase).tobytes()
             )
 
         try:
             return self._key.private_bytes(encd, fmt, protection)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
 
     @classmethod
     def load(
         cls,
         data: bytes,
         passphrase: bytes | None = None,
         *,
@@ -284,52 +289,56 @@
 
         if passphrase is not None:
             passphrase = memoryview(passphrase).tobytes()
 
         try:
             key = cls._validate_key_type(loader(memoryview(data), passphrase))
         except (ValueError, TypeError) as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
 
         return cls(None, _key=key)
 
     @classmethod
     def _get_loader(
         cls,
         data: bytes,
     ) -> typing.Callable[[bytes, bytes | None], ec.EllipticCurvePrivateKey]:
         """
         Returns a loader function depending on the initial bytes of the key.
         """
         try:
             return cls._LOADERS[next(filter(data.startswith, cls._LOADERS))]
         except StopIteration:
-            raise ValueError("Invalid format") from None
+            msg = "Invalid format"
+            raise ValueError(msg) from None
 
     @classmethod
     def _validate_key_type(cls, key: typing.Any) -> ec.EllipticCurvePrivateKey:
         """
         Working principle: The loader will return a private key of certain
         type. We will use the knowledge of the type to wrap the key. This
         helps in handling Edwards keys (or any other key that might be added
         in the future).
         """
         try:
             klass = next(
                 filter(lambda t: isinstance(key, t), cls._KEY_TYPE_WRAPPERS)
             )
         except StopIteration:
-            raise ValueError("The key is not an EC private key.") from None
+            msg = "The key is not an EC private key."
+            raise ValueError(msg) from None
 
         return cls._KEY_TYPE_WRAPPERS[klass](key)
 
     @classmethod
     def _load_raw(cls, data: bytes, curve: str) -> ECCPrivateKey:
         if curve not in _Curves.EDWARDS_CURVES:
-            raise ValueError(f"Curve {curve!r} does not support Raw encoding.")
+            msg = f"Curve {curve!r} does not support Raw encoding."
+            raise ValueError(msg)
         return cls(
             None,
             _key=_EdDSAPrivateKeyAdapter.from_private_bytes(data, curve),
         )
 
 
 class ECCPublicKey(base.BaseECCPublicKey):
@@ -373,15 +382,16 @@
             key,
             _name="ed448",
         ),
     }
 
     def __init__(self, key: ec.EllipticCurvePublicKey) -> None:
         if not isinstance(key, ec.EllipticCurvePublicKey):  # pragma: no cover
-            raise TypeError("key is not an EC public key")
+            msg = "key is not an EC public key"
+            raise TypeError(msg)
         self._key = key
         self._key_size = key.key_size
         self._curve = key.curve.name
 
     @property
     def key_size(self) -> int:
         return self._key_size
@@ -392,15 +402,16 @@
 
     def verifier(
         self,
         algorithm: None | base.BaseEllepticCurveSignatureAlgorithm = None,
     ) -> VerifierContext | EdDSAVerifierContext:
         if self.curve.startswith("ed"):
             if algorithm is not None and not isinstance(algorithm, EdDSA):
-                raise TypeError(f"Invalid signature algorithm: {algorithm}")
+                msg = f"Invalid signature algorithm: {algorithm}"
+                raise TypeError(msg)
             assert isinstance(self._key, _EdDSAPublicKeyAdapter)
             return EdDSAVerifierContext(self._key)
 
         algorithm = ECDSA() if algorithm is None else algorithm
         return VerifierContext(
             self._key,
             get_ec_signature_algorithm(algorithm, algorithm),
@@ -438,48 +449,50 @@
             ValueError: If the encoding or format is incorrect, or
             serialization failed.
         """
         try:
             encd = self._ENCODINGS[encoding]
             fmt = self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(
-                f"Invalid encoding or format: {e.args[0]!r}"
-            ) from e
+            msg = f"Invalid encoding or format: {e.args[0]!r}"
+            raise ValueError(msg) from e
 
         try:
             return self._key.public_bytes(encd, fmt)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
 
     @classmethod
     def load(cls, data: bytes, *, curve: str | None = None) -> ECCPublicKey:
         if curve is not None:
             return cls._load_raw_or_sec1(data, curve)
 
         loader = cls._get_loader(data)
         try:
             key = cls._validate_key_type(loader(memoryview(data)))
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
 
         assert isinstance(key, ec.EllipticCurvePublicKey)
         return cls(key)
 
     @classmethod
     def _load_raw_or_sec1(cls, data: bytes, curve: str) -> ECCPublicKey:
         if curve in _Curves.NIST_CURVES:
             return cls(
                 ec.EllipticCurvePublicKey.from_encoded_point(
                     _Curves.NIST_CURVES[curve](),
                     data,
                 )
             )
         if curve not in _Curves.EDWARDS_CURVES:
-            raise ValueError(f"Curve {curve!r} does not support Raw encoding.")
+            msg = f"Curve {curve!r} does not support Raw encoding."
+            raise ValueError(msg)
         return cls(_EdDSAPublicKeyAdapter.from_public_bytes(data, curve))
 
     @classmethod
     def _validate_key_type(cls, key: typing.Any) -> ec.EllipticCurvePublicKey:
         """
         Working principle: The loader will return a public key of certain
         type. We will use the knowledge of the type to wrap the key. This
@@ -488,25 +501,27 @@
         """
         try:
             klass = next(
                 filter(lambda t: isinstance(key, t), cls._KEY_TYPE_WRAPPERS)
             )
             return cls._KEY_TYPE_WRAPPERS[klass](key)
         except StopIteration:
-            raise ValueError("The key is not an EC public key.") from None
+            msg = "The key is not an EC public key."
+            raise ValueError(msg) from None
 
     @classmethod
     def _get_loader(cls, data: bytes) -> typing.Callable:
         """
         Returns a loader function depending on the initial bytes of the key.
         """
         try:
             return cls._LOADERS[next(filter(data.startswith, cls._LOADERS))]
         except StopIteration:
-            raise ValueError("Invalid format.") from None
+            msg = "Invalid format."
+            raise ValueError(msg) from None
 
 
 class VerifierContext(base.BaseVerifierContext):
     def __init__(
         self,
         key: ec.EllipticCurvePublicKey,
         signature_algorithm: typing.Any,
@@ -567,15 +582,15 @@
         try:
             return self._key.verify(signature, message, None)
         except bkx.InvalidSignature as e:
             raise exc.SignatureError from e
 
 
 class _EllepticCurve(ec.EllipticCurve):
-    def __init__(self, name: str, key_size: int):
+    def __init__(self, name: str, key_size: int) -> None:
         self._name = name
         self._key_size = key_size
 
     @property
     def name(self) -> str:
         return self._name
 
@@ -717,14 +732,17 @@
         key = cls._LOADERS[curve](data)
         assert isinstance(
             key,
             (ed25519.Ed25519PublicKey, ed448.Ed448PublicKey),
         )
         return cls(key, _name=curve)
 
+    def __eq__(self, other: object) -> bool:
+        return self._key == other
+
 
 def generate(curve: str) -> ECCPrivateKey:
     """
     Generate a private key with given curve ``curve``.
 
     Args:
         curve: The name of the curve to use.
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/Hash.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/Hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import typing
 from types import MappingProxyType
 
 from cryptography.hazmat.primitives import hashes
 
-from ... import base, exc
+from pyflocker.ciphers import base, exc
 
 HASHES = MappingProxyType(
     {
         "sha1": hashes.SHA1,
         "sha224": hashes.SHA224,
         "sha256": hashes.SHA256,
         "sha384": hashes.SHA384,
@@ -114,24 +114,24 @@
     def name(self) -> str:
         return self._name
 
     @property
     def oid(self) -> str:  # pragma: no cover
         """The ASN.1 Object ID."""
         if self._oid is NotImplemented:
-            raise AttributeError(f"OID not available for {self.name!r}")
+            msg = f"OID not available for {self.name!r}"
+            raise AttributeError(msg)
 
         if self.name in ("blake2b", "blake2s") and self.digest_size not in (
             32,
             64,
         ):
-            raise AttributeError(
-                f"OID not available for {self.name!r} with digest size"
-                f" {self.digest_size}"
-            )
+            msg = f"OID not available for {self.name!r} with digest size "
+            f"{self.digest_size}"
+            raise AttributeError(msg)
 
         return self._oid
 
     def update(self, data: bytes) -> None:
         if self._ctx is None:
             raise exc.AlreadyFinalized
         self._ctx.update(data)
@@ -178,15 +178,16 @@
         Creates a pyca/cryptography based hash function object.
         """
         hashfunc = HASHES[name]
 
         digest_size_kwargs = {}
         if name in VAR_DIGEST_SIZE:
             if digest_size is None:
-                raise ValueError("digest_size is required")
+                msg = "digest_size is required"
+                raise ValueError(msg)
             digest_size_kwargs = {"digest_size": digest_size}
 
         hashobj = hashes.Hash(hashfunc(**digest_size_kwargs))
 
         if data is not None:
             hashobj.update(data)
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/RSA.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/RSA.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from cryptography.hazmat.primitives.asymmetric import rsa, utils
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     PrivateFormat,
     PublicFormat,
 )
 
-from ... import base, exc
-from ..asymmetric import OAEP, PSS
+from pyflocker.ciphers import base, exc
+from pyflocker.ciphers.backends.asymmetric import OAEP, PSS
+
 from . import Hash
 from .asymmetric import get_padding_algorithm
 
 if typing.TYPE_CHECKING:
     from cryptography.hazmat.primitives.asymmetric import padding as _padding
 
 
@@ -52,15 +53,16 @@
         e: int = 65537,
         _key: rsa.RSAPrivateKey | None = None,
     ) -> None:
         if _key is not None:
             self._key = _key
         else:
             if not isinstance(n, int):  # pragma: no cover
-                raise TypeError("n must be an integer value")
+                msg = "n must be an integer value"
+                raise TypeError(msg)
             self._key = rsa.generate_private_key(e, n)
 
         # numbers
         priv_nos = self._key.private_numbers()
         self._p = priv_nos.p
         self._q = priv_nos.q
         self._d = priv_nos.d
@@ -145,30 +147,30 @@
         Raises:
            ValueError: if the format or encoding is invalid or not supported.
         """
         try:
             encd = self._ENCODINGS[encoding]
             fmt = self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(
-                f"The encoding or format is invalid: {e.args[0]!r}"
-            ) from e
+            msg = f"The encoding or format is invalid: {e.args[0]!r}"
+            raise ValueError(msg) from e
 
         protection: serial.KeySerializationEncryption
         if passphrase is None:
             protection = serial.NoEncryption()
         else:
             protection = serial.BestAvailableEncryption(
                 memoryview(passphrase).tobytes()
             )
 
         try:
             return self._key.private_bytes(encd, fmt, protection)
         except ValueError as e:
-            raise ValueError(f"Failed to serialize key: {e!s}") from e
+            msg = f"Failed to serialize key: {e!s}"
+            raise ValueError(msg) from e
 
     @classmethod
     def load(
         cls,
         data: bytes,
         passphrase: bytes | None = None,
     ) -> RSAPrivateKey:
@@ -176,32 +178,35 @@
 
         if passphrase is not None:
             passphrase = memoryview(passphrase).tobytes()
 
         try:
             key = loader(memoryview(data), passphrase)
             if not isinstance(key, rsa.RSAPrivateKey):
-                raise ValueError("Key is not an RSA Private key")
+                msg = "Key is not an RSA Private key"
+                raise ValueError(msg)
         except (ValueError, TypeError) as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
 
         return cls(None, _key=key)
 
     @classmethod
     def _get_loader(
         cls,
         data: bytes,
     ) -> typing.Callable[[bytes, bytes | None], rsa.RSAPrivateKey]:
         """
         Returns a loader function depending on the initial bytes of the key.
         """
         try:
             return cls._LOADERS[next(filter(data.startswith, cls._LOADERS))]
         except StopIteration:
-            raise ValueError("Invalid format") from None
+            msg = "Invalid format"
+            raise ValueError(msg) from None
 
 
 class RSAPublicKey(base.BaseRSAPublicKey):
     # Encodings supported by this key.
     _ENCODINGS = {
         "PEM": Encoding.PEM,
         "DER": Encoding.DER,
@@ -220,15 +225,16 @@
         b"ssh-rsa ": serial.load_ssh_public_key,
         b"-----": serial.load_pem_public_key,
         b"0": serial.load_der_public_key,
     }
 
     def __init__(self, key: rsa.RSAPublicKey) -> None:
         if not isinstance(key, rsa.RSAPublicKey):  # pragma: no cover
-            raise ValueError("The key is not an RSA public key.")
+            msg = "The key is not an RSA public key."
+            raise ValueError(msg)
         self._key = key
 
         # numbers
         pub_nos = self._key.public_numbers()
         self._e = pub_nos.e
         self._n = pub_nos.n
 
@@ -287,41 +293,43 @@
         Raises:
             ValueError: if the encoding or format is incorrect or unsupported.
         """
         try:
             encd = self._ENCODINGS[encoding]
             fmt = self._FORMATS[format]
         except KeyError as e:
-            raise ValueError(
-                f"Invalid encoding or format: {e.args[0]!r}"
-            ) from e
+            msg = f"Invalid encoding or format: {e.args[0]!r}"
+            raise ValueError(msg) from e
         return self._key.public_bytes(encd, fmt)
 
     @classmethod
     def load(cls, data: bytes) -> RSAPublicKey:
         loader = cls._get_loader(data)
         try:
             key = loader(memoryview(data))
             if not isinstance(key, rsa.RSAPublicKey):
-                raise ValueError("Key is not an RSA public key.")
+                msg = "Key is not an RSA public key."
+                raise ValueError(msg)
         except ValueError as e:
-            raise ValueError(f"Failed to load key: {e!s}") from e
+            msg = f"Failed to load key: {e!s}"
+            raise ValueError(msg) from e
 
         assert isinstance(key, rsa.RSAPublicKey)
         return cls(key)
 
     @classmethod
     def _get_loader(cls, data: bytes) -> typing.Callable:
         """
         Returns a loader function depending on the initial bytes of the key.
         """
         try:
             return cls._LOADERS[next(filter(data.startswith, cls._LOADERS))]
         except StopIteration:
-            raise ValueError("Invalid format.") from None
+            msg = "Invalid format."
+            raise ValueError(msg) from None
 
 
 class EncryptorContext(base.BaseEncryptorContext):
     def __init__(
         self,
         key: rsa.RSAPublicKey,
         padding: _padding.AsymmetricPadding,
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/asymmetric.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/asymmetric.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 
 import typing
 from typing import TYPE_CHECKING
 
 from cryptography.hazmat.primitives.asymmetric import padding as padding_
 from cryptography.hazmat.primitives.asymmetric.ec import ECDH, ECDSA
 
-from .. import asymmetric
+from pyflocker.ciphers.backends import asymmetric
+
 from . import Hash
 
 if TYPE_CHECKING:  # pragma: no cover
-    from ... import base
+    from pyflocker.ciphers import base
 
 
 def get_OAEP(padding: base.BaseAsymmetricPadding) -> padding_.OAEP:
     """Construct a pyca/cryptography specific OAEP object.
 
     Args:
         padding (OAEP): An OAEP object.
 
     Returns:
         OAEP object:
             An OAEP encryptor/decryptor object depending on the key, from the
             cryptography backend.
     """
     if not isinstance(padding, asymmetric.OAEP):  # pragma: no cover
-        raise TypeError("padding must be an instance of OAEP.")
+        msg = "padding must be an instance of OAEP."
+        raise TypeError(msg)
     if not isinstance(padding.mgf, asymmetric.MGF1):
-        raise TypeError("MGF must be an instance of MGF1.")
+        msg = "MGF must be an instance of MGF1."
+        raise TypeError(msg)
     return padding_.OAEP(
         mgf=padding_.MGF1(
             Hash._get_hash_algorithm(padding.mgf.hashfunc),
         ),
         algorithm=Hash._get_hash_algorithm(padding.hashfunc),
         label=padding.label,
     )
@@ -43,17 +46,19 @@
     Args:
         padding (PSS): A PSS object.
 
     Returns:
         PSS object: An PSS signer/verifier object, depending on the key.
     """
     if not isinstance(padding, asymmetric.PSS):  # pragma: no cover
-        raise TypeError("padding must be an instance of PSS.")
+        msg = "padding must be an instance of PSS."
+        raise TypeError(msg)
     if not isinstance(padding.mgf, asymmetric.MGF1):
-        raise TypeError("MGF must be an instance of MGF1.")
+        msg = "MGF must be an instance of MGF1."
+        raise TypeError(msg)
     return padding_.PSS(
         mgf=padding_.MGF1(Hash._get_hash_algorithm(padding.mgf.hashfunc)),
         salt_length=padding_.PSS.MAX_LENGTH
         if padding.salt_length is None
         else padding.salt_length,
     )
 
@@ -63,15 +68,16 @@
 
     Args:
         algorithm: The algorithm to use.
 
     Returns: ECDH key exchange object.
     """
     if not isinstance(algorithm, asymmetric.ECDH):  # pragma: no cover
-        raise TypeError("algorithm must be an instance of ECDH")
+        msg = "algorithm must be an instance of ECDH"
+        raise TypeError(msg)
     return ECDH()
 
 
 def get_ECDSA(
     algorithm: base.BaseEllepticCurveSignatureAlgorithm,
 ) -> type[ECDSA]:
     """Return an ECDSA callable for signing/verification.
@@ -80,15 +86,16 @@
 
     Args:
         algorithm: The algorithm to use.
 
     Returns: Signer/Verifier callable.
     """
     if not isinstance(algorithm, asymmetric.ECDSA):  # pragma: no cover
-        raise TypeError("algorithm must be an instance of ECDSA")
+        msg = "algorithm must be an instance of ECDSA"
+        raise TypeError(msg)
     return ECDSA
 
 
 PADDINGS: dict[type[base.BaseAsymmetricPadding], typing.Callable] = {
     asymmetric.OAEP: get_OAEP,
     asymmetric.PSS: get_PSS,
 }
@@ -114,36 +121,33 @@
     padding: base.BaseAsymmetricPadding,
     *args: typing.Any,
     **kwargs: typing.Any,
 ) -> padding_.AsymmetricPadding:
     try:
         return PADDINGS[type(padding)](*args, **kwargs)
     except KeyError as e:
-        raise TypeError(
-            f"Invalid padding algorithm type: {type(padding)}"
-        ) from e
+        msg = f"Invalid padding algorithm type: {type(padding)}"
+        raise TypeError(msg) from e
 
 
 def get_ec_exchange_algorithm(
     algorithm: base.BaseEllepticCurveExchangeAlgorithm,
     *args: typing.Any,
     **kwargs: typing.Any,
 ) -> typing.Any:
     try:
         return EC_EXCHANGE_ALGORITHMS[type(algorithm)](*args, **kwargs)
     except KeyError as e:
-        raise TypeError(
-            f"Invalid exchange algorithm type: {type(algorithm)}"
-        ) from e
+        msg = f"Invalid exchange algorithm type: {type(algorithm)}"
+        raise TypeError(msg) from e
 
 
 def get_ec_signature_algorithm(
     algorithm: base.BaseEllepticCurveSignatureAlgorithm,
     *args: typing.Any,
     **kwargs: typing.Any,
 ) -> typing.Any:
     try:
         return EC_SIGNATURE_ALGORITHMS[type(algorithm)](*args, **kwargs)
     except KeyError as e:
-        raise TypeError(
-            f"Invalid signature algorithm type: {type(algorithm)}"
-        ) from e
+        msg = f"Invalid signature algorithm type: {type(algorithm)}"
+        raise TypeError(msg) from e
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/misc.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Miscellaneous Tools: Tools that are not common to symmetric or asymmetric.
 """
 
 from __future__ import annotations
 
-from cryptography.hazmat.primitives.ciphers import Cipher
-from cryptography.hazmat.primitives.ciphers import algorithms as algo
+from cryptography.hazmat.primitives.ciphers import (
+    Cipher,
+    algorithms as algo,
+)
 from cryptography.hazmat.primitives.kdf.hkdf import HKDF
 
-from ...base import BaseHash
+from pyflocker.ciphers.base import BaseHash
+
 from .Hash import _get_hash_algorithm
 
 
 def derive_hkdf_key(
     master_key: bytes,
     dklen: int,
     hashalgo: BaseHash,
@@ -30,15 +33,16 @@
         cipher_ctx: Context for cipher.
         auth_ctx: Context for HMAC.
 
     Returns:
         A pair of *cipher key* and *MAC key*.
     """
     if not isinstance(hashalgo, BaseHash):
-        raise TypeError("hashalgo must be an object implementing BaseHash")
+        msg = "hashalgo must be an object implementing BaseHash"
+        raise TypeError(msg)
 
     hash_ = _get_hash_algorithm(hashalgo)
     key = HKDF(hash_, dklen, salt, cipher_ctx).derive(master_key)
     hkey = HKDF(hash_, hash_.digest_size, salt, auth_ctx).derive(master_key)
     return key, hkey
 
 
@@ -52,14 +56,15 @@
     Returns:
         bytes: A Poly1305 key.
 
     Raises:
         ValueError: If the length of nonce is not equal to 8 or 12 bytes.
     """
     if len(nonce) not in (8, 12):
-        raise ValueError("Poly1305 nonce must be 8 or 12 bytes long.")
+        msg = "Poly1305 nonce must be 8 or 12 bytes long."
+        raise ValueError(msg)
 
     if len(nonce) == 8:  # pragma: no cover
         nonce = bytes(4) + nonce
 
     crp = Cipher(algo.ChaCha20(ckey, bytes(4) + nonce), None).encryptor()
     return crp.update(bytes(32))
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/cryptography_/symmetric.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/cryptography_/symmetric.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import typing
 
 from cryptography import exceptions as bkx
 
-from ... import base, exc
+from pyflocker.ciphers import base, exc
 
 
 class NonAEADCipherTemplate(base.BaseNonAEADCipher):
     """
     Template class to provide the default behavior if BaseNonAEADCipher.
 
     Subclasses need to provide:
@@ -76,15 +76,16 @@
 
     def finalize(self, tag: bytes | None = None) -> None:
         if self._ctx is None:
             raise exc.AlreadyFinalized
 
         if not self.is_encrypting():
             if tag is None:
-                raise ValueError("tag is required for finalization")
+                msg = "tag is required for finalization"
+                raise ValueError(msg)
 
             ctx, self._ctx = self._ctx, None
             try:
                 ctx.finalize_with_tag(tag)
             except bkx.InvalidTag as e:
                 raise exc.DecryptionError from e
         else:
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/backends/symmetric.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/backends/symmetric.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import hmac
 import typing
 from functools import partial
 
-from .. import base, exc
+from pyflocker.ciphers import base, exc
 
 if typing.TYPE_CHECKING:
     import io
 
 
 class FileCipherWrapper:
     """
@@ -18,29 +18,30 @@
     """
 
     def __init__(
         self,
         cipher: base.BaseAEADCipher,
         file: io.BufferedIOBase,
         offset: int = 0,
-    ):
+    ) -> None:
         """Initialize a file cipher wrapper.
 
         Args:
             cipher:
                 A cipher that supports :py:class:`BaseAEADCipher` interface.
             file: A file or file-like object.
             offset:
                 The difference between the length of ``in`` buffer and ``out``
                 buffer in ``update_into`` method of a BaseAEADCipher. This is
                 required because backend like ``pyca/cryptography`` needs an
                 output buffer that is bigger than the input buffer.
         """
         if not isinstance(cipher, base.BaseAEADCipher):
-            raise TypeError("cipher must implement BaseAEADCipher interface.")
+            msg = "cipher must implement BaseAEADCipher interface."
+            raise TypeError(msg)
 
         # the cipher already has an internal context
         self._ctx = cipher
         self._file = file
         self._tag: bytes | None = None
         self._encrypting = self._ctx.is_encrypting()
         self._offset = offset
@@ -98,15 +99,16 @@
         Raises:
             AlreadyFinalized: if the cipher has been finalized.
             ValueError: if the file is being decrypted and tag is not supplied.
         """
         if self._ctx is None:
             raise exc.AlreadyFinalized
         if not self._encrypting and tag is None:
-            raise ValueError("tag is required for decryption")
+            msg = "tag is required for decryption"
+            raise ValueError(msg)
 
         buf = memoryview(bytearray(blocksize + self._offset))
         rbuf = buf[:blocksize]
 
         # localize variables for better performance
         offset = self._offset
         write = file.write
@@ -132,15 +134,16 @@
             self._tag, self._ctx = (
                 self._ctx.calculate_tag(),
                 None,  # type: ignore
             )
 
     def calculate_tag(self) -> bytes | None:
         if self._ctx is not None:
-            raise exc.NotFinalized("Cipher has not been finalized yet.")
+            msg = "Cipher has not been finalized yet."
+            raise exc.NotFinalized(msg)
         return self._tag
 
 
 StreamCipherWrapper = FileCipherWrapper
 
 
 class HMACWrapper(base.BaseAEADCipher):
@@ -153,17 +156,18 @@
         self,
         cipher: base.BaseNonAEADCipher,
         hmac_key: bytes,
         hmac_random: bytes,
         hashfunc: str | base.BaseHash = "sha256",
         offset: int = 0,
         tag_length: int | None = 16,
-    ):
+    ) -> None:
         if not isinstance(cipher, base.BaseNonAEADCipher):
-            raise TypeError("Only NonAEAD ciphers can be wrapped.")
+            msg = "Only NonAEAD ciphers can be wrapped."
+            raise TypeError(msg)
 
         if isinstance(hashfunc, base.BaseHash):
             # always use a fresh hash object.
             hashfunc = hashfunc.new()
         self._auth = hmac.new(hmac_key, digestmod=hashfunc)  # type: ignore
 
         self._auth.update(hmac_random)
@@ -183,18 +187,17 @@
     def is_encrypting(self) -> bool:
         return self._encrypting
 
     def authenticate(self, data: bytes) -> None:
         if self._ctx is None:
             raise exc.AlreadyFinalized
         if self._updated:
-            raise TypeError(
-                "Cannot call authenticate after update/update_into has been"
-                " called"
-            )
+            msg = "Cannot call authenticate after update/update_into has been "
+            "called"
+            raise TypeError(msg)
         self._auth.update(data)
         self._len_aad += len(data)
 
     def update(self, data: bytes) -> bytes:
         if self._ctx is None:
             raise exc.AlreadyFinalized
         self._updated = True
@@ -214,19 +217,19 @@
 
     def finalize(self, tag: bytes | None = None) -> None:
         if self._ctx is None:
             raise exc.AlreadyFinalized
 
         if not self.is_encrypting():
             if tag is None:
-                raise ValueError("tag is required for decryption")
+                msg = "tag is required for decryption"
+                raise ValueError(msg)
             if len(tag) != self._tag_length:
-                raise ValueError(
-                    f"Invalid tag length: (required {self._tag_length})"
-                )
+                msg = f"Invalid tag length: (required {self._tag_length})"
+                raise ValueError(msg)
 
         self._auth.update(self._len_aad.to_bytes(8, "little"))
         self._auth.update(self._len_ct.to_bytes(8, "little"))
 
         self._ctx = None
 
         if not self._encrypting and not hmac.compare_digest(
@@ -256,15 +259,15 @@
 
 class _EncryptionCtx:
     def __init__(
         self,
         cipher: base.BaseNonAEADCipher,
         auth: typing.Any,
         offset: int,
-    ):
+    ) -> None:
         self._ctx = cipher
         self._auth = auth
         self._offset = -offset or None
 
     def update(self, data: bytes) -> bytes:
         ctxt = self._ctx.update(data)
         self._auth.update(ctxt)
@@ -276,15 +279,17 @@
         out: bytearray | memoryview,
     ) -> None:
         self._ctx.update_into(data, out)
         self._auth.update(out[: self._offset])
 
 
 class _DecryptionCtx:
-    def __init__(self, cipher: base.BaseNonAEADCipher, auth: typing.Any):
+    def __init__(
+        self, cipher: base.BaseNonAEADCipher, auth: typing.Any
+    ) -> None:
         self._ctx = cipher
         self._auth = auth
 
     def update(self, data: bytes) -> bytes:
         self._auth.update(data)
         return self._ctx.update(data)
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/base.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Base classes for pyflocker. """
+"""Base classes for pyflocker."""
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 
 
 class BaseSymmetricCipher(metaclass=ABCMeta):
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/exc.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/exc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Exceptions raised by the ciphers are defined here."""
 
-
 from __future__ import annotations
 
 
 class DecryptionError(Exception):
     """
     Can be raised in two cases:
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/AES.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/Camellia.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,68 @@
-"""Interface to AES cipher"""
+"""Interface to Camellia cipher"""
+
 from __future__ import annotations
 
 import typing
 
-from ..backends import load_algorithm as _load_algo
-from ..modes import Modes
+from pyflocker.ciphers.backends import (
+    Backends,
+    load_algorithm as _load_algo,
+)
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import io
 
-    from .. import base
-    from ..backends import Backends
-    from ..backends.symmetric import FileCipherWrapper
-
-
-# Prevent type checking errors from being raised.
-MODE_GCM = Modes.MODE_GCM
-MODE_CTR = Modes.MODE_CTR
-MODE_CFB = Modes.MODE_CFB
-MODE_CFB8 = Modes.MODE_CFB8
-MODE_OFB = Modes.MODE_OFB
-MODE_CCM = Modes.MODE_CCM
-MODE_EAX = Modes.MODE_EAX
-MODE_SIV = Modes.MODE_SIV
-MODE_OCB = Modes.MODE_OCB
+    from pyflocker.ciphers import base
+    from pyflocker.ciphers.backends.symmetric import FileCipherWrapper
+    from pyflocker.ciphers.modes import Modes
 
 
 def supported_modes(backend: Backends) -> set[Modes]:
     """
     Lists all modes supported by the cipher. It is limited to backend's
     implementation and capability, and hence, varies from backend to backend.
 
     Args:
         backend: The backend to inspect.
 
     Returns:
         Set of :any:`Modes` supported by the backend.
     """
-    return _load_algo("AES", backend).supported_modes()
+    return _load_algo("Camellia", backend).supported_modes()
 
 
 def new(
     encrypting: bool,
     key: bytes,
     mode: Modes,
     iv_or_nonce: bytes,
     *,
     use_hmac: bool = False,
     tag_length: int | None = 16,
     digestmod: None | base.BaseHash = None,
     file: io.BufferedIOBase | None = None,
-    backend: Backends | None = None,
-) -> (
-    base.BaseAEADCipher
-    | base.BaseNonAEADCipher
-    | base.BaseAEADOneShotCipher
-    | FileCipherWrapper
-):
-    """Instantiate a new AES cipher object.
+    backend: Backends = Backends.CRYPTOGRAPHY,
+) -> base.BaseAEADCipher | base.BaseNonAEADCipher | FileCipherWrapper:
+    """Instantiate a new Camellia cipher object.
 
     Args:
         encrypting: True is encryption and False is decryption.
         key: The key for the cipher.
         mode:
-            The mode to use for AES cipher. All backends may not support that
-            particular mode.
+            The mode to use for Camellia cipher. All backends may not support
+            that particular mode.
         iv_or_nonce:
             The Initialization Vector or Nonce for the cipher. It must not be
             repeated with the same key.
 
     Keyword Arguments:
         use_hmac:
-            Should the cipher use HMAC as authentication or not, if it does not
-            support AEAD. (Default: False)
+            Should the cipher use HMAC as authentication or not. Default is
+            False.
         tag_length:
             Length of HMAC tag. By default, a **16 byte tag** is generated. If
             ``tag_length`` is ``None``, a **non-truncated** tag is generated.
             Length of non-truncated tag depends on the digest size of the
             underlying hash algorithm used by HMAC.
         digestmod:
             The algorithm to use for HMAC. If ``None``, defaults to ``sha256``.
@@ -91,28 +77,26 @@
         The following arguments are ignored if the mode is an AEAD mode:
 
         - ``use_hmac``
         - ``tag_length``
         - ``digestmod``
 
     Returns:
-        AES cipher wrapper from the appropriate backend module.
+        Camellia cipher from the appropriate backend module.
 
     Raises:
-        NotImplementedError:
-            if the mode does not support encryption/decryption of files.
-        UnsupportedAlgorithm: if the backend does not support AES.
-        UnsupportedMode: if the mode does not support the given ``mode``.
+        UnsupportedMode: if backend does not support that mode.
+        UnsupportedAlgorithm: if the backend does not support Camellia.
 
     Note:
         Any other error that is raised is from the backend itself.
     """
-    return _load_algo("AES", backend).new(
+    return _load_algo("Camellia", backend).new(
         encrypting,
         key,
         mode,
         iv_or_nonce,
+        file=file,
         use_hmac=use_hmac,
         tag_length=tag_length,
         digestmod=digestmod,
-        file=file,
     )
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/ChaCha20.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/ChaCha20.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Interface to ChaCha20(-Poly1305) cipher"""
+
 from __future__ import annotations
 
 import typing
 
-from ..backends import load_algorithm as _load_algo
+from pyflocker.ciphers.backends import load_algorithm as _load_algo
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     import io
 
-    from .. import base
-    from ..backends import Backends
-    from ..backends.symmetric import FileCipherWrapper
+    from pyflocker.ciphers import base
+    from pyflocker.ciphers.backends import Backends
+    from pyflocker.ciphers.backends.symmetric import FileCipherWrapper
 
 
 def new(
     encrypting: bool,
     key: bytes,
     nonce: bytes,
     *,
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/DH.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/DH.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Interface to DH key exchange"""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from ..backends import Backends as _Backends
-from ..backends import load_algorithm as _load_algo
+from pyflocker.ciphers.backends import (
+    Backends as _Backends,
+    load_algorithm as _load_algo,
+)
 
 if TYPE_CHECKING:  # pragma: no cover
     from types import ModuleType
 
-    from .. import base
+    from pyflocker.ciphers import base
 
 
 def _load_dhe(backend: _Backends) -> ModuleType:
     return _load_algo("DH", backend)
 
 
 def generate(
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/ECC.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/ECC.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Interface to ECC signature algorithm and key-exchange."""
+
 from __future__ import annotations
 
 import typing
 
-from ..backends import load_algorithm as _load_algo
+from pyflocker.ciphers.backends import load_algorithm as _load_algo
 
 if typing.TYPE_CHECKING:
     from types import ModuleType
 
-    from .. import base
-    from ..backends import Backends
+    from pyflocker.ciphers import base
+    from pyflocker.ciphers.backends import Backends
 
 
 def _load_ecc_cpr(backend: Backends | None) -> ModuleType:
     """Load the cipher module from the backend."""
     return _load_algo("ECC", backend)
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/Hash.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/Hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Interface to hashing algorithms."""
+
 from __future__ import annotations
 
 import typing
 
-from ..backends import Backends as _Backends
-from ..backends import load_algorithm as _load_algo
+from pyflocker.ciphers.backends import (
+    Backends as _Backends,
+    load_algorithm as _load_algo,
+)
 
 if typing.TYPE_CHECKING:  # pragma: no cover
-    from ..base import BaseHash
+    from pyflocker.ciphers.base import BaseHash
 
 
 def algorithms_available(
     backend: _Backends | None = None,
 ) -> set[str]:
     """Returns all available hashes supported by backend."""
     if backend is not None:
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/interfaces/RSA.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/interfaces/RSA.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Interface to RSA cipher and signature algorithm"""
+
 from __future__ import annotations
 
 import typing
 from typing import TYPE_CHECKING
 
-from ..backends import load_algorithm as _load_algo
+from pyflocker.ciphers.backends import load_algorithm as _load_algo
 
 if TYPE_CHECKING:  # pragma: no cover
     from types import ModuleType
 
-    from ..backends import Backends
-    from ..base import BaseRSAPrivateKey, BaseRSAPublicKey
+    from pyflocker.ciphers.backends import Backends
+    from pyflocker.ciphers.base import BaseRSAPrivateKey, BaseRSAPublicKey
 
 
 def _load_rsa(backend: Backends | None) -> ModuleType:
     """Load the cipher module from the backend."""
     return _load_algo("RSA", backend)
```

### Comparing `pyflocker-0.4.1/src/pyflocker/ciphers/modes.py` & `pyflocker-0.4.2/src/pyflocker/ciphers/modes.py`

 * *Files identical despite different names*

### Comparing `pyflocker-0.4.1/src/pyflocker/locker.py` & `pyflocker-0.4.2/src/pyflocker/locker.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 ~~~~~~~~~~~~
 
 After completion of the entire operation, the tag created by the authenticator
 of the cipher is written to the file as a part of ``Header``. If the file is
 being decrypted, it is read from the ``Header`` for verifying the file
 integrity and correct decryption.
 """
+
 from __future__ import annotations
 
 import os
 import struct
 import typing
 from collections import namedtuple
 from functools import partial
@@ -213,18 +214,20 @@
             Raised if ``aes_mode`` is not amongst the supported modes.
         OverflowError:
             Raised if length of metadata exceeded :py:const:`MAX_METADATA_LEN`.
     """
     _assert_unique_files(infile, outfile)
 
     if aes_mode in SPECIAL:
-        raise NotImplementedError(f"{aes_mode} is not supported.")
+        msg = f"{aes_mode} is not supported."
+        raise NotImplementedError(msg)
 
     if len(metadata) > MAX_METADATA_LEN:
-        raise OverflowError("maximum metadata length exceeded (limit: 32).")
+        msg = "maximum metadata length exceeded (limit: 32)."
+        raise OverflowError(msg)
 
     # create the salt and nonce...
     salt = os.urandom(32)
     nonce = os.urandom(12) if aes_mode == AES.MODE_GCM else os.urandom(16)
 
     # ...and pack it into header and write it to the outfile
     header = _Header(MAGIC, aes_mode.value, nonce, b"", metadata, salt)
@@ -533,29 +536,27 @@
         The removal of file is **NOT** secure, because it uses
         :py:func:`os.remove` to remove the file. With enough expertise and
         time, the original file can be restored. If you want to remove the
         original file securely, consider using ``shred`` or ``srm`` or some
         other secure file deletion tools.
     """
     if newfile and ext:
-        raise ValueError("newfile and ext are mutually exclusive")
+        msg = "newfile and ext are mutually exclusive"
+        raise ValueError(msg)
 
     ext = ext or EXTENSION
     file = os.fspath(file)
 
     # guess encrypting if not provided
     if encrypting is None:
         encrypting = not file.endswith(ext)
 
     # make newfile name if not provided
     if newfile is None:
-        if encrypting:
-            newfile = file + ext
-        else:
-            newfile = os.path.splitext(file)[0]
+        newfile = file + ext if encrypting else os.path.splitext(file)[0]
 
     if encrypting:
         encrypt(file, newfile, password, remove, **kwargs)
     else:
         kwargs.pop("aes_mode", None)
         decrypt(file, newfile, password, remove, **kwargs)
 
@@ -579,15 +580,16 @@
 
 def _assert_unique_files(
     infile: typing.IO[bytes],
     outfile: typing.IO[bytes],
 ) -> None:
     """Check if files are unique, else raise ValueError."""
     if os.path.samefile(infile.fileno(), outfile.fileno()):
-        raise ValueError("infile and outfile are the same")
+        msg = "infile and outfile are the same"
+        raise ValueError(msg)
 
 
 def _encrypt_or_decrypt(
     callable: typing.Callable[..., None],
     infile: str | os.PathLike,
     outfile: str | os.PathLike,
     password: bytes,
@@ -606,39 +608,39 @@
         if remove:
             os.remove(infile)
 
 
 def _check_key_length(n: int) -> int:
     if n in (128, 192, 256):
         return n // 8
-    elif n in (16, 24, 32):
+    if n in (16, 24, 32):
         return n
-    else:
-        raise ValueError("invalid key length")
+    msg = "invalid key length"
+    raise ValueError(msg)
 
 
 def _get_header(data: bytes, metadata: bytes = METADATA) -> _Header:
     try:
         (
             magic,
             mode,
             nonce,
             tag,
             metadata_h,
             salt,
         ) = HEADER_PAYLOAD.unpack(data)
     except struct.error as e:
-        raise TypeError("The file format is invalid (Header mismatch).") from e
+        msg = "The file format is invalid (Header mismatch)."
+        raise TypeError(msg) from e
 
     if (
         magic != MAGIC
         or metadata != metadata_h[: len(metadata) - MAX_METADATA_LEN]
     ):
-        raise TypeError(
-            "The file format is invalid (Metadata/magic number mismatch)."
-        )
+        msg = "The file format is invalid (Metadata/magic number mismatch)."
+        raise TypeError(msg)
 
     if mode == Modes.MODE_GCM.value:
         nonce = nonce[:12]
     if Modes(mode) in AEAD:
         tag = tag[:16]
     return _Header(magic, mode, nonce, tag, metadata, salt)
```

### Comparing `pyflocker-0.4.1/PKG-INFO` & `pyflocker-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 Metadata-Version: 2.1
-Name: pyflocker
-Version: 0.4.1
+Name: PyFLocker
+Version: 0.4.2
 Summary: Python Cryptographic (File Locking) Library
-Home-page: https://github.com/arunanshub/pyflocker
+Keywords: cryptography,encryption,python,pypi,symmetric key,asymmetric key,aes,chacha20,camellia,rsa,dsa,ecc,file encryption,secure communication,cryptography library
+Author-Email: Arunanshu Biswas <mydellpc07@gmail.com>
 License: MIT
-Keywords: cryptography,symmetric,asymmetric,aead,rsa
-Author: Arunanshu Biswas
-Author-email: mydellpc07@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security :: Cryptography
-Requires-Dist: cryptography[ssh] (>=35.0.0,!=37.0.0)
-Requires-Dist: pycryptodomex (>=3.9.8,<4.0.0)
-Project-URL: Bug Tracker, https://github.com/arunanshub/pyflocker/issues
+Project-URL: Bug tracker, https://github.com/arunanshub/pyflocker/issues
 Project-URL: Changelog, https://github.com/arunanshub/pyflocker/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://pyflocker.readthedocs.io
 Project-URL: Repository, https://github.com/arunanshub/pyflocker
+Requires-Python: >=3.9
+Requires-Dist: pycryptodomex>=3.9.8
+Requires-Dist: cryptography[ssh]!=37.0.0,>=35.0.0
 Description-Content-Type: text/markdown
 
 # PyFLocker
 
 [![CI](https://github.com/arunanshub/pyflocker/actions/workflows/ci.yml/badge.svg)](https://github.com/arunanshub/pyflocker/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/arunanshub/pyflocker/badge.svg?branch=master)](https://coveralls.io/github/arunanshub/pyflocker?branch=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -179,8 +173,7 @@
 [MIT](https://choosealicense.com/licenses/mit/)
 
 [docs]: https://pyflocker.readthedocs.io/en/latest/
 [examples]: https://pyflocker.readthedocs.io/en/latest/examples
 [pycrypto]: https://github.com/Legrandin/pycryptodome
 [pyca]: https://github.com/pyca/cryptography
 [pyca_vs_self]: https://cryptography.io/en/latest/hazmat/primitives/asymmetric/rsa.html#key-serialization
-
```

