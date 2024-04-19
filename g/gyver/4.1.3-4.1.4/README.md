# Comparing `tmp/gyver-4.1.3.tar.gz` & `tmp/gyver-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-4.1.3.tar", max compression
+gzip compressed data, was "gyver-4.1.4.tar", max compression
```

## Comparing `gyver-4.1.3.tar` & `gyver-4.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1079 2024-03-28 22:08:41.323819 gyver-4.1.3/LICENSE
--rw-r--r--   0        0        0      610 2024-03-28 22:08:41.323819 gyver-4.1.3/README.md
--rw-r--r--   0        0        0      158 2024-03-28 22:28:31.846253 gyver-4.1.3/gyver/__init__.py
--rw-r--r--   0        0        0      795 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1315 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1065 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     7939 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1043 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     6716 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/helpers.py
--rw-r--r--   0        0        0     2111 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     2014 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     2105 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0      419 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     3880 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2358 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     2734 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5447 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/context.py
--rw-r--r--   0        0        0      102 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1984 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/context/typedef.py
--rw-r--r--   0        0        0     2667 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/exc.py
--rw-r--r--   0        0        0      225 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/filetree/__init__.py
--rw-r--r--   0        0        0     1748 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/filetree/filetree.py
--rw-r--r--   0        0        0      348 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/filetree/helpers.py
--rw-r--r--   0        0        0     3248 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/filetree/interface.py
--rw-r--r--   0        0        0     2865 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/filetree/typedef.py
--rw-r--r--   0        0        0     2808 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/filetree/virtual.py
--rw-r--r--   0        0        0      111 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/model/__init__.py
--rw-r--r--   0        0        0     1804 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/model/v1.py
--rw-r--r--   0        0        0     1793 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/model/v2.py
--rw-r--r--   0        0        0      101 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/py.typed
--rw-r--r--   0        0        0      186 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/__init__.py
--rw-r--r--   0        0        0     6994 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/core.py
--rw-r--r--   0        0        0      423 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/encode.py
--rw-r--r--   0        0        0     1505 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/fragment.py
--rw-r--r--   0        0        0     4784 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/netloc.py
--rw-r--r--   0        0        0     4749 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/path.py
--rw-r--r--   0        0        0     3926 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/query.py
--rw-r--r--   0        0        0     1186 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/url/utils.py
--rw-r--r--   0        0        0      579 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/utils/__init__.py
--rw-r--r--   0        0        0     1041 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/utils/exc.py
--rw-r--r--   0        0        0    12855 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/utils/finder.py
--rw-r--r--   0        0        0     4941 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/utils/helpers.py
--rw-r--r--   0        0        0     1669 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/utils/json.py
--rw-r--r--   0        0        0     2749 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/utils/strings.py
--rw-r--r--   0        0        0     1100 2024-03-28 22:08:41.327153 gyver-4.1.3/gyver/utils/timezone.py
--rw-r--r--   0        0        0     1623 2024-03-28 22:28:31.856253 gyver-4.1.3/pyproject.toml
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 gyver-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-28 22:08:41.323819 gyver-4.1.4/LICENSE
+-rw-r--r--   0        0        0      610 2024-03-28 22:08:41.323819 gyver-4.1.4/README.md
+-rw-r--r--   0        0        0      158 2024-04-19 02:04:59.979793 gyver-4.1.4/gyver/__init__.py
+-rw-r--r--   0        0        0      795 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1315 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1065 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     7939 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1043 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     6716 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/helpers.py
+-rw-r--r--   0        0        0     2111 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     2014 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     2105 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0      419 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     3880 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2358 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     2734 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5447 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1984 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/context/typedef.py
+-rw-r--r--   0        0        0     2667 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/exc.py
+-rw-r--r--   0        0        0      225 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/__init__.py
+-rw-r--r--   0        0        0     1748 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/filetree.py
+-rw-r--r--   0        0        0      348 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/helpers.py
+-rw-r--r--   0        0        0     3248 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/interface.py
+-rw-r--r--   0        0        0     2865 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/typedef.py
+-rw-r--r--   0        0        0     2808 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/filetree/virtual.py
+-rw-r--r--   0        0        0      111 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/model/__init__.py
+-rw-r--r--   0        0        0     1804 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/model/v1.py
+-rw-r--r--   0        0        0     1793 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/model/v2.py
+-rw-r--r--   0        0        0      101 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/py.typed
+-rw-r--r--   0        0        0      186 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/url/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-18 22:41:50.880985 gyver-4.1.4/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2024-04-18 20:01:32.234522 gyver-4.1.4/gyver/url/encode.py
+-rw-r--r--   0        0        0     1631 2024-04-18 22:41:41.627434 gyver-4.1.4/gyver/url/fragment.py
+-rw-r--r--   0        0        0     5027 2024-04-19 02:03:56.058338 gyver-4.1.4/gyver/url/netloc.py
+-rw-r--r--   0        0        0     4830 2024-04-18 22:40:58.819756 gyver-4.1.4/gyver/url/path.py
+-rw-r--r--   0        0        0     4022 2024-04-18 22:42:15.161559 gyver-4.1.4/gyver/url/query.py
+-rw-r--r--   0        0        0     1186 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/url/utils.py
+-rw-r--r--   0        0        0      579 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/__init__.py
+-rw-r--r--   0        0        0     1041 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/exc.py
+-rw-r--r--   0        0        0    12855 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/finder.py
+-rw-r--r--   0        0        0     4941 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/helpers.py
+-rw-r--r--   0        0        0     1669 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/json.py
+-rw-r--r--   0        0        0     2749 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/strings.py
+-rw-r--r--   0        0        0     1100 2024-03-28 22:08:41.327153 gyver-4.1.4/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     1623 2024-04-19 02:04:59.993127 gyver-4.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 gyver-4.1.4/PKG-INFO
```

### Comparing `gyver-4.1.3/LICENSE` & `gyver-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/README.md` & `gyver-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/__init__.py` & `gyver-4.1.4/gyver/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/attrs.py` & `gyver-4.1.4/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/dataclass.py` & `gyver-4.1.4/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/factory.py` & `gyver-4.1.4/gyver/config/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/gattrs.py` & `gyver-4.1.4/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/helpers.py` & `gyver-4.1.4/gyver/config/adapter/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/interface.py` & `gyver-4.1.4/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/mark.py` & `gyver-4.1.4/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/config/adapter/pydantic.py` & `gyver-4.1.4/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/context/atomic_/bound.py` & `gyver-4.1.4/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/context/atomic_/core.py` & `gyver-4.1.4/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/context/atomic_/resolver.py` & `gyver-4.1.4/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/context/context.py` & `gyver-4.1.4/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/context/interfaces/adapter.py` & `gyver-4.1.4/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/exc.py` & `gyver-4.1.4/gyver/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/filetree/filetree.py` & `gyver-4.1.4/gyver/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/filetree/interface.py` & `gyver-4.1.4/gyver/filetree/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/filetree/typedef.py` & `gyver-4.1.4/gyver/filetree/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/filetree/virtual.py` & `gyver-4.1.4/gyver/filetree/virtual.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/model/v1.py` & `gyver-4.1.4/gyver/model/v1.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/model/v2.py` & `gyver-4.1.4/gyver/model/v2.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/pools/asyncio.py` & `gyver-4.1.4/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/pools/resource.py` & `gyver-4.1.4/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/pools/thread.py` & `gyver-4.1.4/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/url/core.py` & `gyver-4.1.4/gyver/url/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -163,15 +163,21 @@
 
     def copy(self) -> "URL":
         """Create a copy of the URL object.
 
         Returns:
             URL: The copied URL object.
         """
-        return URL(self.encode())
+        url = object.__new__(type(self))
+        url.scheme = self.scheme
+        url.netloc = self.netloc.copy()
+        url.path = self.path.copy()
+        url.query = self.query.copy()
+        url.fragment = self.fragment.copy()
+        return url
 
     @classmethod
     def from_netloc(
         cls,
         netloc: Optional[Netloc] = None,
         *,
         username: Optional[str] = None,
```

### Comparing `gyver-4.1.3/gyver/url/fragment.py` & `gyver-4.1.4/gyver/url/fragment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from urllib.parse import quote
 
-from gyver.attrs import mutable
 from typing_extensions import Self
 
+from gyver.attrs import mutable
 from gyver.url.encode import Encodable
-from gyver.url.utils import is_valid_encoded_path
-from gyver.url.utils import utf8
+from gyver.url.utils import is_valid_encoded_path, utf8
 
 
 @mutable(eq=False)
 class Fragment(Encodable):
     """Represents an encodable URL fragment.
 
     Attributes:
@@ -55,7 +54,12 @@
         """
         Return the fragment string when converting the object to a string.
 
         Returns:
             str: The fragment string.
         """
         return self.fragment_str
+
+    def copy(self) -> "Fragment":
+        fragment = object.__new__(Fragment)
+        fragment.fragment_str = self.fragment_str
+        return fragment
```

### Comparing `gyver-4.1.3/gyver/url/netloc.py` & `gyver-4.1.4/gyver/url/netloc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 from urllib.parse import quote
 
-from gyver.attrs import mutable
 from typing_extensions import Self
 
+from gyver.attrs import mutable
 from gyver.url.encode import Encodable
 from gyver.url.utils import utf8
 
 
 @mutable(eq=False)
 class Netloc(Encodable):
     """Represents the network location portion of a URL.
@@ -151,7 +151,15 @@
             port (Optional[int], optional): The port number.
 
         Returns:
             Netloc: The created `Netloc` object.
         """
         netloc = cls("")
         return netloc.set(host, username, password, port)
+
+    def copy(self) -> "Netloc":
+        netloc = object.__new__(type(self))
+        netloc.host = self.host
+        netloc.username = self.username
+        netloc.password = self.password
+        netloc.port = self.port
+        return netloc
```

### Comparing `gyver-4.1.3/gyver/url/path.py` & `gyver-4.1.4/gyver/url/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import re
 from typing import Union
-from urllib.parse import quote
-from urllib.parse import unquote
+from urllib.parse import quote, unquote
 
-from gyver.attrs import mutable
 from typing_extensions import Self
 
+from gyver.attrs import mutable
 from gyver.url.encode import Encodable
-from gyver.url.utils import is_valid_encoded_path
-from gyver.url.utils import utf8
+from gyver.url.utils import is_valid_encoded_path, utf8
 
 PERCENT_REGEX = r"\%[a-fA-F\d][a-fA-F\d]"
 
 SAFE_SEGMENT_CHARS = ":@-._~!$&'()*+,;="
 
 
 @mutable(eq=False)
@@ -138,14 +136,19 @@
             Path: The normalized Path object.
         """
         if resolved := self.encode():
             normalized = normalize(resolved)
             self.segments = self._load(normalized)
         return self
 
+    def copy(self) -> "Path":
+        path = object.__new__(Path)
+        path.segments = self.segments.copy()
+        return path
+
 
 _duplicates_regex = re.compile(r"/+")
 
 
 def normalize(path: str) -> str:
     """Normalize a path string by removing redundant segments.
```

### Comparing `gyver-4.1.3/gyver/url/query.py` & `gyver-4.1.4/gyver/url/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from collections import defaultdict
-from typing import Mapping
-from typing import Optional
-from urllib.parse import parse_qs
-from urllib.parse import quote
+from typing import Mapping, Optional
+from urllib.parse import parse_qs, quote
 
-from gyver.attrs import mutable
 from typing_extensions import Self
 
+from gyver.attrs import mutable
 from gyver.url.encode import Encodable
 
 
 @mutable(eq=False)
 class Query(Encodable):
     """Represents a query string and provides methods to manipulate and encode it.
 
@@ -120,7 +118,12 @@
         """Sorts the query parameters in lexicographic order based on the parameter names.
 
         Returns:
             Query: The modified Query object.
         """
         self.params = defaultdict(list, sorted(self.params.items()))
         return self
+
+    def copy(self) -> "Query":
+        query = object.__new__(type(self))
+        query.params = self.params.copy()
+        return query
```

### Comparing `gyver-4.1.3/gyver/url/utils.py` & `gyver-4.1.4/gyver/url/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/utils/__init__.py` & `gyver-4.1.4/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/utils/exc.py` & `gyver-4.1.4/gyver/utils/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/utils/finder.py` & `gyver-4.1.4/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/utils/helpers.py` & `gyver-4.1.4/gyver/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/utils/json.py` & `gyver-4.1.4/gyver/utils/json.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/utils/strings.py` & `gyver-4.1.4/gyver/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/gyver/utils/timezone.py` & `gyver-4.1.4/gyver/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.3/pyproject.toml` & `gyver-4.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "4.1.3"
+version = "4.1.4"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver-4.1.3/PKG-INFO` & `gyver-4.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 4.1.3
+Version: 4.1.4
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

