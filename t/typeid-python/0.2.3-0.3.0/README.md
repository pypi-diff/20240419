# Comparing `tmp/typeid_python-0.2.3.tar.gz` & `tmp/typeid_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeid_python-0.2.3.tar", max compression
+gzip compressed data, was "typeid_python-0.3.0.tar", max compression
```

## Comparing `typeid_python-0.2.3.tar` & `typeid_python-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-10-02 11:51:12.457900 typeid_python-0.2.3/LICENSE
--rw-r--r--   0        0        0     3137 2023-10-02 11:51:12.458085 typeid_python-0.2.3/README.md
--rw-r--r--   0        0        0     1533 2024-03-27 15:08:45.248159 typeid_python-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      149 2023-10-02 11:51:12.459201 typeid_python-0.2.3/typeid/__init__.py
--rw-r--r--   0        0        0     6504 2023-10-02 11:51:12.459389 typeid_python-0.2.3/typeid/base32.py
--rw-r--r--   0        0        0      872 2023-10-02 11:51:12.459463 typeid_python-0.2.3/typeid/cli.py
--rw-r--r--   0        0        0       37 2023-10-02 11:51:12.459530 typeid_python-0.2.3/typeid/constants.py
--rw-r--r--   0        0        0      207 2023-10-02 11:51:12.459605 typeid_python-0.2.3/typeid/errors.py
--rw-r--r--   0        0        0     2927 2024-03-27 15:08:26.864050 typeid_python-0.2.3/typeid/typeid.py
--rw-r--r--   0        0        0      899 2023-10-02 11:51:12.459777 typeid_python-0.2.3/typeid/validation.py
--rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 typeid_python-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-10-02 11:51:12.457900 typeid_python-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3137 2023-10-02 11:51:12.458085 typeid_python-0.3.0/README.md
+-rw-r--r--   0        0        0     1533 2024-04-19 13:18:18.643545 typeid_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-10-02 11:51:12.459201 typeid_python-0.3.0/typeid/__init__.py
+-rw-r--r--   0        0        0     6504 2023-10-02 11:51:12.459389 typeid_python-0.3.0/typeid/base32.py
+-rw-r--r--   0        0        0      872 2023-10-02 11:51:12.459463 typeid_python-0.3.0/typeid/cli.py
+-rw-r--r--   0        0        0       37 2023-10-02 11:51:12.459530 typeid_python-0.3.0/typeid/constants.py
+-rw-r--r--   0        0        0      207 2023-10-02 11:51:12.459605 typeid_python-0.3.0/typeid/errors.py
+-rw-r--r--   0        0        0     3009 2024-04-19 13:18:00.088577 typeid_python-0.3.0/typeid/typeid.py
+-rw-r--r--   0        0        0      910 2024-04-19 13:18:00.088801 typeid_python-0.3.0/typeid/validation.py
+-rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 typeid_python-0.3.0/PKG-INFO
```

### Comparing `typeid_python-0.2.3/LICENSE` & `typeid_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typeid_python-0.2.3/README.md` & `typeid_python-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `typeid_python-0.2.3/pyproject.toml` & `typeid_python-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typeid-python"
-version = "0.2.3"
+version = "0.3.0"
 description = "Python implementation of TypeIDs: type-safe, K-sortable, and globally unique identifiers inspired by Stripe IDs"
 authors = ["Murad Akhundov <akhundov1murad@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/akhundMurad/typeid-python"
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `typeid_python-0.2.3/typeid/base32.py` & `typeid_python-0.3.0/typeid/base32.py`

 * *Files identical despite different names*

### Comparing `typeid_python-0.2.3/typeid/cli.py` & `typeid_python-0.3.0/typeid/cli.py`

 * *Files identical despite different names*

### Comparing `typeid_python-0.2.3/typeid/typeid.py` & `typeid_python-0.3.0/typeid/typeid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import warnings
 from typing import Optional
-from uuid import UUID
 
-from uuid6 import uuid7
+import uuid6
 
 from typeid import base32
 from typeid.errors import InvalidTypeIDStringException
 from typeid.validation import validate_prefix, validate_suffix
 
 
 class TypeID:
     def __init__(self, prefix: Optional[str] = None, suffix: Optional[str] = None) -> None:
-        suffix = _convert_uuid_to_b32(uuid7()) if not suffix else suffix
+        suffix = _convert_uuid_to_b32(uuid6.uuid7()) if not suffix else suffix
         validate_suffix(suffix=suffix)
         if prefix:
             validate_prefix(prefix=prefix)
 
         self._prefix = prefix or ""
         self._suffix = suffix
 
     @classmethod
     def from_string(cls, string: str):
         prefix, suffix = get_prefix_and_suffix(string=string)
         return cls(suffix=suffix, prefix=prefix)
 
     @classmethod
-    def from_uuid(cls, suffix: UUID, prefix: Optional[str] = None):
+    def from_uuid(cls, suffix: uuid6.UUID, prefix: Optional[str] = None):
         suffix_str = _convert_uuid_to_b32(suffix)
-        return TypeID(suffix=suffix_str, prefix=prefix)
+        return cls(suffix=suffix_str, prefix=prefix)
 
     @property
     def suffix(self) -> str:
         return self._suffix
 
     @property
     def prefix(self) -> str:
         return self._prefix
 
     @property
-    def uuid(self) -> UUID:
+    def uuid(self) -> uuid6.UUID:
         return _convert_b32_to_uuid(self.suffix)
 
     def __str__(self) -> str:
         value = ""
         if self.prefix:
             value += f"{self.prefix}_"
         value += self.suffix
@@ -71,33 +70,34 @@
 
 
 def from_string(string: str) -> TypeID:
     warnings.warn("Consider TypeID.from_string instead.", DeprecationWarning)
     return TypeID.from_string(string=string)
 
 
-def from_uuid(suffix: UUID, prefix: Optional[str] = None) -> TypeID:
+def from_uuid(suffix: uuid6.UUID, prefix: Optional[str] = None) -> TypeID:
     warnings.warn("Consider TypeID.from_uuid instead.", DeprecationWarning)
     return TypeID.from_uuid(suffix=suffix, prefix=prefix)
 
 
 def get_prefix_and_suffix(string: str) -> tuple:
     parts = string.split("_")
-    suffix = None
     prefix = None
     if len(parts) == 1:
         suffix = parts[0]
     elif len(parts) == 2 and parts[0] != "":
         suffix = parts[1]
         prefix = parts[0]
     else:
         raise InvalidTypeIDStringException(f"Invalid TypeID: {string}")
 
     return prefix, suffix
 
 
-def _convert_uuid_to_b32(uuid_instance: UUID) -> str:
+def _convert_uuid_to_b32(uuid_instance: uuid6.UUID) -> str:
     return base32.encode(list(uuid_instance.bytes))
 
 
-def _convert_b32_to_uuid(b32: str) -> UUID:
-    return UUID(bytes=bytes(base32.decode(b32)))
+def _convert_b32_to_uuid(b32: str) -> uuid6.UUID:
+    uuid_bytes = bytes(base32.decode(b32))
+    uuid_int = int.from_bytes(uuid_bytes, byteorder="big")
+    return uuid6.UUID(int=uuid_int, version=7)
```

### Comparing `typeid_python-0.2.3/typeid/validation.py` & `typeid_python-0.3.0/typeid/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import re
+
 from typeid import base32
-from typeid.constants import PREFIX_MAX_LEN, SUFFIX_LEN
+from typeid.constants import SUFFIX_LEN
 from typeid.errors import PrefixValidationException, SuffixValidationException
 
 
 def validate_prefix(prefix: str) -> None:
-    if not prefix.islower() or not prefix.isascii() or len(prefix) > PREFIX_MAX_LEN or not prefix.isalpha():
+    # See https://github.com/jetify-com/typeid/tree/main/spec
+    if not re.match("^([a-z]([a-z_]{0,61}[a-z])?)?$", prefix):
         raise PrefixValidationException(f"Invalid prefix: {prefix}.")
 
 
 def validate_suffix(suffix: str) -> None:
     if (
         len(suffix) != SUFFIX_LEN
         or suffix == ""
```

### Comparing `typeid_python-0.2.3/PKG-INFO` & `typeid_python-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeid-python
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python implementation of TypeIDs: type-safe, K-sortable, and globally unique identifiers inspired by Stripe IDs
 Home-page: https://github.com/akhundMurad/typeid-python
 License: MIT
 Keywords: typeid,uuid,uuid6,guid
 Author: Murad Akhundov
 Author-email: akhundov1murad@gmail.com
 Requires-Python: >=3.8,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: typeid-python Version: 0.2.3 Summary: Python
+Metadata-Version: 2.1 Name: typeid-python Version: 0.3.0 Summary: Python
 implementation of TypeIDs: type-safe, K-sortable, and globally unique
 identifiers inspired by Stripe IDs Home-page: https://github.com/akhundMurad/
 typeid-python License: MIT Keywords: typeid,uuid,uuid6,guid Author: Murad
 Akhundov Author-email: akhundov1murad@gmail.com Requires-Python: >=3.8,<4
 Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

