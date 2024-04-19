# Comparing `tmp/tesseract_olap-0.9.3.tar.gz` & `tmp/tesseract_olap-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.9.3.tar", max compression
+gzip compressed data, was "tesseract_olap-0.9.4.tar", max compression
```

## Comparing `tesseract_olap-0.9.3.tar` & `tesseract_olap-0.9.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2589 2024-03-15 00:23:52.753141 tesseract_olap-0.9.3/PACKAGE.md
--rw-r--r--   0        0        0     1320 2024-04-16 19:20:26.872800 tesseract_olap-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      562 2024-04-16 18:43:02.221430 tesseract_olap-0.9.3/tesseract_olap/__init__.py
--rw-r--r--   0        0        0      397 2024-04-16 16:46:29.714821 tesseract_olap-0.9.3/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0     2815 2024-04-16 16:46:29.714821 tesseract_olap-0.9.3/tesseract_olap/backend/cache.py
--rw-r--r--   0        0        0       84 2023-12-12 19:31:05.053659 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     7219 2024-04-03 16:02:12.590243 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     2714 2024-03-21 19:13:55.671898 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0    20624 2024-04-02 20:13:34.560489 tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     3743 2024-04-02 16:29:24.355193 tesseract_olap-0.9.3/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0     2836 2024-04-16 16:46:29.730422 tesseract_olap-0.9.3/tesseract_olap/backend/valkey.py
--rw-r--r--   0        0        0      571 2024-04-02 15:44:57.403234 tesseract_olap-0.9.3/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0     2461 2024-04-02 17:20:54.212089 tesseract_olap-0.9.3/tesseract_olap/common/strings.py
--rw-r--r--   0        0        0      399 2023-12-12 19:31:05.137658 tesseract_olap-0.9.3/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      787 2024-03-28 19:35:52.289762 tesseract_olap-0.9.3/tesseract_olap/exceptions/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-03 00:40:34.602127 tesseract_olap-0.9.3/tesseract_olap/exceptions/backend.py
--rw-r--r--   0        0        0     3576 2024-04-16 19:11:41.156439 tesseract_olap-0.9.3/tesseract_olap/exceptions/query.py
--rw-r--r--   0        0        0     3712 2024-03-28 19:32:15.041429 tesseract_olap-0.9.3/tesseract_olap/exceptions/schema.py
--rw-r--r--   0        0        0      741 2024-03-28 19:33:42.379457 tesseract_olap-0.9.3/tesseract_olap/exceptions/server.py
--rw-r--r--   0        0        0      528 2023-12-12 19:31:05.153661 tesseract_olap-0.9.3/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0    11052 2024-04-16 18:30:11.173365 tesseract_olap-0.9.3/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     6326 2024-04-16 19:11:28.486182 tesseract_olap-0.9.3/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     4477 2024-04-16 18:35:36.963968 tesseract_olap-0.9.3/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1166 2024-04-02 17:32:08.076597 tesseract_olap-0.9.3/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     3318 2024-04-01 21:27:27.862280 tesseract_olap-0.9.3/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0    12543 2024-04-02 20:23:58.946279 tesseract_olap-0.9.3/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    13039 2024-04-16 19:09:01.435800 tesseract_olap-0.9.3/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0    10178 2024-04-02 16:17:50.023716 tesseract_olap-0.9.3/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1763 2024-04-16 18:36:26.257633 tesseract_olap-0.9.3/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-02 15:24:33.879569 tesseract_olap-0.9.3/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     3587 2024-03-25 21:23:44.777212 tesseract_olap-0.9.3/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     4744 2024-04-01 20:55:50.142052 tesseract_olap-0.9.3/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     2542 2024-03-14 23:53:07.076800 tesseract_olap-0.9.3/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     9528 2024-04-03 00:58:10.522977 tesseract_olap-0.9.3/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0    11992 2024-04-01 15:57:37.686893 tesseract_olap-0.9.3/tesseract_olap/schema/parser.py
--rw-r--r--   0        0        0     5306 2024-04-16 18:38:50.208477 tesseract_olap-0.9.3/tesseract_olap/schema/public.py
--rw-r--r--   0        0        0     4824 2024-03-07 16:34:52.541289 tesseract_olap-0.9.3/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23758 2024-04-16 19:07:35.244865 tesseract_olap-0.9.3/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    19086 2024-03-28 20:20:53.653136 tesseract_olap-0.9.3/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2024-03-21 21:10:19.073197 tesseract_olap-0.9.3/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0     4674 2024-03-28 19:25:27.542934 tesseract_olap-0.9.3/tesseract_olap/server/schema.py
--rw-r--r--   0        0        0     3713 2024-04-16 16:47:39.771505 tesseract_olap-0.9.3/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 tesseract_olap-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     2589 2024-04-19 21:02:01.618058 tesseract_olap-0.9.4/PACKAGE.md
+-rw-r--r--   0        0        0     1320 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      562 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0      377 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0     2707 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/cache.py
+-rw-r--r--   0        0        0       79 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     7219 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     2714 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0    20624 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     3743 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0     2761 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/backend/valkey.py
+-rw-r--r--   0        0        0      571 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0     2461 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      385 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      787 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/backend.py
+-rw-r--r--   0        0        0     3682 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/query.py
+-rw-r--r--   0        0        0     3712 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/schema.py
+-rw-r--r--   0        0        0      741 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/exceptions/server.py
+-rw-r--r--   0        0        0      511 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0    11052 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     6492 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     4550 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1166 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     3318 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0    12543 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    13039 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0    10178 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1763 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3587 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     4744 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     2542 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     9528 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0    11992 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/parser.py
+-rw-r--r--   0        0        0     5306 2024-04-19 21:02:01.622058 tesseract_olap-0.9.4/tesseract_olap/schema/public.py
+-rw-r--r--   0        0        0     4824 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23758 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    18520 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0     4674 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     3713 2024-04-19 21:02:01.626058 tesseract_olap-0.9.4/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 tesseract_olap-0.9.4/PKG-INFO
```

### Comparing `tesseract_olap-0.9.3/PACKAGE.md` & `tesseract_olap-0.9.4/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/pyproject.toml` & `tesseract_olap-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesseract-olap"
-version = "0.9.3"
+version = "0.9.4"
 description = "A simple OLAP library."
 authors = [
   "Francisco Abarzua <francisco@datawheel.us>",
   "Jelmy Hermosilla <jelmy@datawheel.us>",
 ]
 maintainers = [
   "Francisco Abarzua <francisco@datawheel.us>",
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/__init__.py` & `tesseract_olap-0.9.4/tesseract_olap/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __title__ = "tesseract-olap"
 __description__ = "A simple OLAP library."
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 __all__ = (
     "DataRequest",
     "DataRequestParams",
     "MembersRequest",
     "MembersRequestParams",
     "NotAuthorized",
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/backend/cache.py` & `tesseract_olap-0.9.4/tesseract_olap/backend/cache.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import abc
-from enum import Enum
-from typing import Union
-
-import polars as pl
-from lfudacache import LFUDACache
-
-from tesseract_olap.query import AnyQuery
-
-from .models import Result
-
-CacheConnectionStatus = Enum("CacheConnectionStatus", ["CLOSED", "CONNECTED"])
-
-
-class CacheProvider(abc.ABC):
-    """Base class for the implementation of a cache layer for the Backend."""
-
-    def __repr__(self):
-        return f"{type(self).__name__}"
-
-    @abc.abstractmethod
-    def connect(self) -> "CacheConnection":
-        raise NotImplementedError
-
-
-class CacheConnection(abc.ABC):
-    """Internal Base class for individual connections to the cache layer."""
-
-    @property
-    @abc.abstractmethod
-    def status(self) -> "CacheConnectionStatus":
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def close(self) -> None:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def ping(self) -> bool:
-        raise NotImplementedError
-
-
-class DummyProvider(CacheProvider):
-    """A CacheProvider used when the user doesn't set a valid one. Will always MISS."""
-
-    def connect(self):
-        return DummyConnection()
-
-
-class DummyConnection(CacheConnection):
-    """The CacheConnection associated to DummyProvider. Will always MISS."""
-
-    @property
-    def status(self):
-        return CacheConnectionStatus.CONNECTED
-
-    def close(self):
-        pass
-
-    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]"):
-        pass
-
-    def retrieve(self, query: "AnyQuery"):
-        return None
-
-    def ping(self):
-        return True
-
-
-class LfuProvider(CacheProvider):
-    """Stores elements in a dictionary under the Least Frequently Used caching stategy."""
-
-    def __init__(self, maxsize: int = 64) -> None:
-        self.store = LFUDACache(maxsize)
-
-    def connect(self):
-        return LfuConnection(self.store)
-
-
-class LfuConnection(CacheConnection):
-    """The CacheConnection associated to LfuProvider."""
-
-    def __init__(self, store: "LFUDACache") -> None:
-        self.storage = store
-
-    @property
-    def status(self):
-        return CacheConnectionStatus.CONNECTED
-
-    def close(self):
-        pass
-
-    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]"):
-        self.storage[query.key] = result
-
-    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
-        return self.storage.get(query.key)
-
-    def ping(self):
-        return True
+import abc
+from enum import Enum
+from typing import Union
+
+import polars as pl
+from lfudacache import LFUDACache
+
+from tesseract_olap.query import AnyQuery
+
+from .models import Result
+
+CacheConnectionStatus = Enum("CacheConnectionStatus", ["CLOSED", "CONNECTED"])
+
+
+class CacheProvider(abc.ABC):
+    """Base class for the implementation of a cache layer for the Backend."""
+
+    def __repr__(self):
+        return f"{type(self).__name__}"
+
+    @abc.abstractmethod
+    def connect(self) -> "CacheConnection":
+        raise NotImplementedError
+
+
+class CacheConnection(abc.ABC):
+    """Internal Base class for individual connections to the cache layer."""
+
+    @property
+    @abc.abstractmethod
+    def status(self) -> "CacheConnectionStatus":
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def close(self) -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def ping(self) -> bool:
+        raise NotImplementedError
+
+
+class DummyProvider(CacheProvider):
+    """A CacheProvider used when the user doesn't set a valid one. Will always MISS."""
+
+    def connect(self):
+        return DummyConnection()
+
+
+class DummyConnection(CacheConnection):
+    """The CacheConnection associated to DummyProvider. Will always MISS."""
+
+    @property
+    def status(self):
+        return CacheConnectionStatus.CONNECTED
+
+    def close(self):
+        pass
+
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]"):
+        pass
+
+    def retrieve(self, query: "AnyQuery"):
+        return None
+
+    def ping(self):
+        return True
+
+
+class LfuProvider(CacheProvider):
+    """Stores elements in a dictionary under the Least Frequently Used caching stategy."""
+
+    def __init__(self, maxsize: int = 64) -> None:
+        self.store = LFUDACache(maxsize)
+
+    def connect(self):
+        return LfuConnection(self.store)
+
+
+class LfuConnection(CacheConnection):
+    """The CacheConnection associated to LfuProvider."""
+
+    def __init__(self, store: "LFUDACache") -> None:
+        self.storage = store
+
+    @property
+    def status(self):
+        return CacheConnectionStatus.CONNECTED
+
+    def close(self):
+        pass
+
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]"):
+        self.storage[query.key] = result
+
+    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
+        return self.storage.get(query.key)
+
+    def ping(self):
+        return True
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/dialect.py` & `tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/dialect.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.9.4/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/backend/models.py` & `tesseract_olap-0.9.4/tesseract_olap/backend/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/backend/valkey.py` & `tesseract_olap-0.9.4/tesseract_olap/backend/valkey.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from io import BytesIO
-from typing import TYPE_CHECKING, Union
-
-import polars as pl
-import redis as valkey
-
-from tesseract_olap.backend import Result
-from tesseract_olap.common import hide_dsn_password
-from tesseract_olap.exceptions.backend import UpstreamInternalError, UpstreamNotPrepared
-
-from .cache import CacheConnection, CacheConnectionStatus, CacheProvider
-
-if TYPE_CHECKING:
-    from tesseract_olap.query import AnyQuery
-
-
-class ValkeyProvider(CacheProvider):
-    def __init__(self, dsn: str, **kwargs):
-        self.dsn = dsn
-        self.pool = valkey.ConnectionPool.from_url(dsn, **kwargs)
-
-    def __repr__(self):
-        return f"{type(self).__name__}(dsn='{hide_dsn_password(self.dsn)}')"
-
-    def connect(self):
-        try:
-            return ValkeyConnection(self.pool, single_connection_client=True)
-        except valkey.ConnectionError as exc:
-            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
-        except valkey.RedisError as exc:
-            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
-
-
-class ValkeyConnection(CacheConnection):
-    def __init__(self, pool: valkey.ConnectionPool, **kwargs):
-        self.valkey = valkey.Redis(connection_pool=pool, **kwargs)
-
-    @property
-    def status(self) -> CacheConnectionStatus:
-        return (
-            CacheConnectionStatus.CONNECTED
-            if self.valkey.connection is not None and self.valkey.ping()
-            else CacheConnectionStatus.CLOSED
-        )
-
-    def close(self) -> None:
-        return self.valkey.close()
-
-    def exists(self, query: "AnyQuery") -> bool:
-        return self.valkey.exists(query.key) == 1
-
-    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
-        dfio = result.data.write_ipc(file=None, compression="lz4")
-        try:
-            self.valkey.set(query.key, dfio.getvalue())
-        except valkey.ConnectionError as exc:
-            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
-        except valkey.RedisError as exc:
-            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
-
-    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
-        try:
-            res: bytes = self.valkey.get(query.key)  # type: ignore
-        except valkey.ConnectionError as exc:
-            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
-        except valkey.RedisError as exc:
-            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
-
-        if res is None:
-            return None
-
-        return Result(data=pl.read_ipc(BytesIO(res)), columns=query.columns)
-
-    def ping(self) -> bool:
-        return self.valkey.ping()  # type: ignore
+from io import BytesIO
+from typing import TYPE_CHECKING, Union
+
+import polars as pl
+import redis as valkey
+
+from tesseract_olap.backend import Result
+from tesseract_olap.common import hide_dsn_password
+from tesseract_olap.exceptions.backend import UpstreamInternalError, UpstreamNotPrepared
+
+from .cache import CacheConnection, CacheConnectionStatus, CacheProvider
+
+if TYPE_CHECKING:
+    from tesseract_olap.query import AnyQuery
+
+
+class ValkeyProvider(CacheProvider):
+    def __init__(self, dsn: str, **kwargs):
+        self.dsn = dsn
+        self.pool = valkey.ConnectionPool.from_url(dsn, **kwargs)
+
+    def __repr__(self):
+        return f"{type(self).__name__}(dsn='{hide_dsn_password(self.dsn)}')"
+
+    def connect(self):
+        try:
+            return ValkeyConnection(self.pool, single_connection_client=True)
+        except valkey.ConnectionError as exc:
+            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
+        except valkey.RedisError as exc:
+            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
+
+
+class ValkeyConnection(CacheConnection):
+    def __init__(self, pool: valkey.ConnectionPool, **kwargs):
+        self.valkey = valkey.Redis(connection_pool=pool, **kwargs)
+
+    @property
+    def status(self) -> CacheConnectionStatus:
+        return (
+            CacheConnectionStatus.CONNECTED
+            if self.valkey.connection is not None and self.valkey.ping()
+            else CacheConnectionStatus.CLOSED
+        )
+
+    def close(self) -> None:
+        return self.valkey.close()
+
+    def exists(self, query: "AnyQuery") -> bool:
+        return self.valkey.exists(query.key) == 1
+
+    def store(self, query: "AnyQuery", result: "Result[pl.DataFrame]") -> None:
+        dfio = result.data.write_ipc(file=None, compression="lz4")
+        try:
+            self.valkey.set(query.key, dfio.getvalue())
+        except valkey.ConnectionError as exc:
+            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
+        except valkey.RedisError as exc:
+            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
+
+    def retrieve(self, query: "AnyQuery") -> Union["Result[pl.DataFrame]", None]:
+        try:
+            res: bytes = self.valkey.get(query.key)  # type: ignore
+        except valkey.ConnectionError as exc:
+            raise UpstreamNotPrepared(*exc.args).with_traceback(exc.__traceback__)
+        except valkey.RedisError as exc:
+            raise UpstreamInternalError(*exc.args).with_traceback(exc.__traceback__)
+
+        if res is None:
+            return None
+
+        return Result(data=pl.read_ipc(BytesIO(res)), columns=query.columns)
+
+    def ping(self) -> bool:
+        return self.valkey.ping()  # type: ignore
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/common/__init__.py` & `tesseract_olap-0.9.4/tesseract_olap/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/common/strings.py` & `tesseract_olap-0.9.4/tesseract_olap/common/strings.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/exceptions/__init__.py` & `tesseract_olap-0.9.4/tesseract_olap/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/exceptions/backend.py` & `tesseract_olap-0.9.4/tesseract_olap/exceptions/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/exceptions/query.py` & `tesseract_olap-0.9.4/tesseract_olap/exceptions/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,10 +101,13 @@
 
     Should be raised before the query is executed against the upstream server.
     """
 
     code = 403
 
     def __init__(self, resource: str, roles: Iterable[str]) -> None:
-        super().__init__("You don't have authorization to access this resource.")
+        super().__init__(
+            f"Requested resource '{resource}' is not allowed for the roles "
+            f"provided by authorization credentials: '{', '.join(roles)}'"
+        )
         self.resource = resource
         self.request_roles = roles
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/exceptions/schema.py` & `tesseract_olap-0.9.4/tesseract_olap/exceptions/schema.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/exceptions/server.py` & `tesseract_olap-0.9.4/tesseract_olap/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/logiclayer/dependencies.py` & `tesseract_olap-0.9.4/tesseract_olap/logiclayer/dependencies.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.9.4/tesseract_olap/logiclayer/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,15 +101,21 @@
         roles = self.auth.get_roles(token)
         cube = self.server.schema.get_cube(cube_name)
         if not cube.is_authorized(roles):
             raise NotAuthorized(f"Cube({cube})", roles)
         locale = self.server.schema.default_locale if locale is None else locale
         return TesseractCube.from_entity(cube, locale=locale)
 
-    @ll.route("GET", "/data", name="redirect_data", response_class=RedirectResponse)
+    @ll.route(
+        "GET",
+        "/data",
+        deprecated=True,
+        name="redirect_data",
+        response_class=RedirectResponse,
+    )
     def query_data_redirect(self, request: Request):
         """Redirects the request to the canonical endpoint in jsonrecords format."""
         return f"{request.url.path}.jsonrecords?{request.url.query}"
 
     @ll.route("GET", "/data.{extension}", name="route_data")
     def query_data(
         self,
@@ -120,14 +126,25 @@
         """Executes a request for data from the server."""
         params.roles = self.auth.get_roles(token)
         query = DataQuery.from_request(self.server.schema, params)
         with self.server.session() as session:
             result = session.fetch_dataframe(query)
         return data_response(params, query, result, extension)
 
+    @ll.route(
+        "GET",
+        "/members.jsonrecords",
+        deprecated=True,
+        name="redirect_members",
+        response_class=RedirectResponse,
+    )
+    def query_members_redirect(self, request: Request):
+        path = request.url.path.replace("members.jsonrecords", "members")
+        return f"{path}?{request.url.query}"
+
     @ll.route("GET", "/members", name="route_members")
     def query_members(
         self,
         params: MembersRequest = Depends(membersquery_params),
         token: Optional[ll.AuthToken] = Depends(auth_token),
     ) -> MembersResModel:
         """Executes a request for the members of a level."""
@@ -140,22 +157,23 @@
     @ll.route("GET", "/debug/schema", debug=True)
     def debug_schema(self):
         """Returns the true internal schema, used to validate the requests."""
         return dataclasses.asdict(self.server.raw_schema)
 
     @ll.exception_handler(TesseractError)
     def exc_tesseracterror(self, request: Request, exc: TesseractError):
+        content = {"error": True, "detail": "Backend error"}
+
+        if self.debug:
+            content["type"] = type(exc).__name__
+
         if isinstance(exc, NotAuthorized):
-            if self.debug:
-                detail = (
-                    f"Requested resource '{exc.resource}' is not allowed for the roles "
-                    f"provided by authorization credentials: '{', '.join(exc.request_roles)}'"
-                )
-                content = {"error": True, "type": "NotAuthorized", "detail": detail}
-            else:
-                content = {"error": True, "detail": exc.message}
-
-        if self.debug or isinstance(exc, QueryError):
-            content = {"error": True, "type": type(exc).__name__, "detail": exc.message}
-        else:
-            content = {"error": True, "detail": "Backend error"}
+            content["detail"] = (
+                exc.message
+                if self.debug
+                else "You don't have authorization to access this resource."
+            )
+
+        elif isinstance(exc, QueryError):
+            content["detail"] = exc.message
+
         return JSONResponse(content, status_code=exc.code)
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.9.4/tesseract_olap/logiclayer/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 
     with tmp.NamedTemporaryFile(delete=False, suffix=f".{extension}") as tmp_file:
         if extension is ResponseFormat.csv:
             df.write_csv(tmp_file, separator=",", include_header=True)
 
         elif extension is ResponseFormat.excel:
             df.write_excel(tmp_file.name)
+            kwargs["filename"] = f"data_{query.key}.{extension}"
 
         elif extension is ResponseFormat.jsonarrays:
             res = df.to_dict(as_series=False)
             target = {"columns": columns, "data": zip(*(res[key] for key in columns))}
             tmp_file.write(orjson.dumps(target))
 
         elif extension is ResponseFormat.jsonrecords:
@@ -87,20 +88,20 @@
             tmp_file.write(orjson.dumps(target))
 
         elif extension is ResponseFormat.tsv:
             df.write_csv(tmp_file, separator="\t", include_header=True)
 
         elif extension is ResponseFormat.parquet:
             df.write_parquet(tmp_file.name)
+            kwargs["filename"] = f"data_{query.key}.{extension}"
 
         else:
             raise HTTPException(406, f"Requested format is not supported: {extension}")
 
     kwargs["background"] = BackgroundTask(os.unlink, tmp_file.name)
-    kwargs["filename"] = f"data_{query.key}.{extension}"
 
     return FileResponse(tmp_file.name, **kwargs)
 
 
 def members_response(
     params: MembersRequest,
     query: MembersQuery,
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/query/__init__.py` & `tesseract_olap-0.9.4/tesseract_olap/query/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/query/enums.py` & `tesseract_olap-0.9.4/tesseract_olap/query/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/query/models.py` & `tesseract_olap-0.9.4/tesseract_olap/query/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/query/queries.py` & `tesseract_olap-0.9.4/tesseract_olap/query/queries.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/query/requests.py` & `tesseract_olap-0.9.4/tesseract_olap/query/requests.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/aggregators.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/csv.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/csv.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/enums.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/json.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/json.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/models.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/parser.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/parser.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/public.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/public.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.9.4/tesseract_olap/schema/schema.xsd`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/traverse.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/schema/xml.py` & `tesseract_olap-0.9.4/tesseract_olap/schema/xml.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,566 +1,566 @@
-"""XML Schema parsing module
-
-Defines subclasses for the core Entity classes, parsed from an XML document.
-"""
-
-import logging
-from ast import literal_eval as eval_tuple
-from collections import OrderedDict
-from pathlib import Path
-from typing import (
-    Generator,
-    Iterable,
-    List,
-    Optional,
-    TextIO,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
-
-import immutables as immu
-from lxml import etree
-
-from tesseract_olap.common import is_numeric, numerify
-from tesseract_olap.exceptions.schema import (
-    InvalidXMLAttributeValue,
-    MissingXMLAttribute,
-    MissingXMLNode,
-)
-
-from . import models
-from .aggregators import Aggregator
-from .csv import parse_csv
-from .enums import AggregatorType, DimensionType, MemberType
-
-logger = logging.getLogger(__name__)
-
-XMLEntity = Union[
-    "XMLSharedDimension",
-    "XMLHierarchy",
-    "XMLLevel",
-    "XMLProperty",
-    "XMLInlineTable",
-    "XMLCube",
-    "XMLDimensionUsage",
-    "XMLHierarchyUsage",
-    "XMLLevelUsage",
-    "XMLPropertyUsage",
-    "XMLPrivateDimension",
-    "XMLMeasure",
-    "XMLCalculatedMeasure",
-]
-
-AnyXMLEntity = TypeVar("AnyXMLEntity", bound=XMLEntity)
-
-
-class XMLSchema(models.Schema):
-    tag = "Schema"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int = 0):
-        """Parse a <Schema> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        cube_gen = _yield_children_nodes(node, XMLCube)
-        shareddim_gen = _yield_children_nodes(node, XMLSharedDimension)
-        sharedtbl_gen = _yield_children_nodes(node, XMLInlineTable)
-
-        return cls(
-            name=name,
-            cube_map=OrderedDict(cube_gen),
-            shared_dimension_map=immu.Map(shareddim_gen),
-            shared_table_map=immu.Map(sharedtbl_gen),
-            default_locale=node.get("default_locale", "xx"),
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-
-class XMLAccessControl(models.AccessControl):
-    tag = "Access"
-
-    @classmethod
-    def parse(cls, node: etree._Element):
-        """Parse all <Access> XML node that are directly under this node."""
-
-        rules_gen = (
-            (role, _get_attr(item, "rule") == "allow")
-            for item in node.iterchildren(cls.tag)
-            for role in _get_attr(item, "roles").split(",")
-        )
-
-        return cls(
-            public=node.get("public", "true") == "true",
-            rules=immu.Map(rules_gen),
-        )
-
-
-class XMLCube(models.Cube):
-    tag = "Cube"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Cube> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        table = _find_table_ref(node)
-        if table is None:
-            raise MissingXMLNode(node.tag, name, "Table")
-
-        dimension_map = OrderedDict(
-            _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
-        )
-        if len(dimension_map) == 0:
-            raise MissingXMLNode(node.tag, name, "Dimension")
-
-        measure_map = OrderedDict(
-            _yield_children_nodes(node, XMLMeasure, XMLCalculatedMeasure)
-        )
-        if len(measure_map) == 0:
-            raise MissingXMLNode(node.tag, name, "Measure")
-
-        return cls(
-            name=name,
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            acl=XMLAccessControl.parse(node),
-            dimension_map=dimension_map,
-            measure_map=measure_map,
-            table=table,
-            annotations=immu.Map(_yield_annotations(node)),
-            subset_table=node.get("subset_table", "false").lower() != "false",
-            visible=node.get("visible", "true").lower() != "false",
-        )
-
-
-class XMLDimensionUsage(models.DimensionUsage):
-    tag = "DimensionUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <DimensionUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            foreign_key=_get_attr(node, "foreign_key"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            hierarchy_map=OrderedDict(
-                _yield_children_nodes(node, XMLHierarchyUsage, attr="source")
-            ),
-        )
-
-
-class XMLHierarchyUsage(models.HierarchyUsage):
-    tag = "HierarchyUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <HierarchyUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            level_map=OrderedDict(
-                _yield_children_nodes(node, XMLLevelUsage, attr="source")
-            ),
-        )
-
-
-class XMLLevelUsage(models.LevelUsage):
-    tag = "LevelUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <LevelUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            property_map=OrderedDict(
-                _yield_children_nodes(node, XMLPropertyUsage, attr="source")
-            ),
-        )
-
-
-class XMLPropertyUsage(models.PropertyUsage):
-    tag = "PropertyUsage"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <PropertyUsage> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            source=_get_attr(node, "source"),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-        )
-
-
-class XMLTable(models.Table):
-    tag = "Table"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Table> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            schema=node.get("schema"),
-            primary_key=node.get("primary_key", "id"),
-        )
-
-
-class XMLInlineTable(models.InlineTable):
-    tag = "InlineTable"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <InlineTable> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        node_format = _get_attr(node, "format")
-
-        if node_format == "csv":
-            node_format = "text/csv"
-
-        if node_format == "tuples":
-            headers, rows = cls.parse_tuples(node)
-        elif node_format.startswith("text/csv"):
-            content = [] if node.text is None else node.text.strip().splitlines()
-            headers, *rows = parse_csv(content, mimetype=node_format)
-            headers = tuple(str(item) for item in headers)
-        else:
-            raise InvalidXMLAttributeValue(node.tag, name, "format", node_format)
-
-        return cls(
-            name=name,
-            headers=headers,
-            types=cls.infer_types(rows),
-            rows=rows,
-        )
-
-    @staticmethod
-    def parse_tuples(
-        node: etree._Element,
-    ) -> Tuple[Tuple[str, ...], List[Tuple[Union[str, float], ...]]]:
-        """Parse the child nodes from an InlineTable with `tuples` format."""
-        try:
-            # try parsing literal tuples with ast.eval()
-            children: List[Tuple[Union[str, float], ...]] = [
-                eval_tuple(line)
-                for line in (item.text for item in node.iterchildren("Row"))
-                if line
-            ]
-        except SyntaxError:
-            # Python `tuples` looks similar to CSV, so let's try with it
-            row_iter = (
-                line[1:-1] if line.startswith("(") and line.endswith(")") else line
-                for line in (item.text for item in node.iterchildren("Row"))
-                if line is not None
-            )
-            children = parse_csv(row_iter, skipinitialspace=True)
-        # at least 2 rows must be present: a header list and a data row
-        if len(children) < 2:
-            raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Row")
-        headers = tuple(str(item) for item in children[0])
-        return headers, children[1:]
-
-
-class XMLSharedDimension(models.Dimension):
-    tag = "SharedDimension"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a Shared <Dimension> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        dim_type = node.get("type")
-
-        hierarchy_map = OrderedDict(_yield_children_nodes(node, XMLHierarchy))
-
-        default_hierarchy = node.get("default_hierarchy")
-        if default_hierarchy not in hierarchy_map:
-            default_hierarchy = next(iter(hierarchy_map.keys()))
-
-        return cls(
-            name=name,
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            default_hierarchy=default_hierarchy,
-            dim_type=DimensionType.from_str(dim_type),
-            foreign_key=node.get("foreign_key"),
-            hierarchy_map=hierarchy_map,
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-
-class XMLPrivateDimension(models.Dimension):
-    tag = "Dimension"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a Private <Dimension> XML node."""
-        dimension: cls = XMLSharedDimension.parse.__func__(cls, node, index)
-
-        # foreign keys are required in Private Dimensions
-        if dimension.foreign_key is None:
-            raise MissingXMLAttribute(node.tag, "foreign_key")
-
-        return dimension
-
-
-class XMLHierarchy(models.Hierarchy):
-    tag = "Hierarchy"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Hierarchy> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        level_map = OrderedDict(_yield_children_nodes(node, XMLLevel))
-        if len(level_map) == 0:
-            raise MissingXMLNode(node.tag, name, "Level")
-
-        default_pk = ""
-        for item in level_map.values():
-            default_pk = item.key_column
-
-        return cls(
-            name=name,
-            primary_key=node.get("primary_key", default_pk),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            table=_find_table_ref(node),
-            level_map=level_map,
-            default_member=cls._parse_default_member(node),
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-    @staticmethod
-    def _parse_default_member(node: etree._Element):
-        items: List[str] = node.get("default_member", "").split(".", maxsplit=1)
-        return (items[0], items[1]) if len(items) == 2 else None
-
-
-class XMLLevel(models.Level):
-    tag = "Level"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Level> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        key_type = node.get("key_type")
-
-        return cls(
-            name=name,
-            depth=index + 1,
-            key_column=_get_attr(node, "key_column"),
-            key_type=MemberType.from_str(key_type),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            name_column_map=immu.Map(_yield_locale_pairs(node, "name_column")),
-            property_map=OrderedDict(_yield_children_nodes(node, XMLProperty)),
-            annotations=immu.Map(_yield_annotations(node)),
-        )
-
-
-class XMLProperty(models.Property):
-    tag = "Property"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Property> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        key_type = node.get("key_type")
-
-        keycol_map = immu.Map(_yield_locale_pairs(node, "key_column"))
-        if len(keycol_map) == 0:
-            raise MissingXMLAttribute(node.tag, "key_column")
-
-        return cls(
-            name=name,
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            key_column_map=keycol_map,
-            key_type=MemberType.from_str(key_type),
-        )
-
-
-class XMLMeasure(models.Measure):
-    tag = "Measure"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <Measure> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            key_column=_get_attr(node, "key_column"),
-            aggregator=cls._get_aggregator(node),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            submeasures=immu.Map(_yield_children_nodes(node, cls)),
-        )
-
-    @staticmethod
-    def _get_aggregator(mea_node: etree._Element) -> Aggregator:
-        """
-        Raises:
-            :class:`MissingXMLAttribute` --
-                If the node doesn't have an `aggregator` attribute or an
-                `<Agregation>` child node.
-
-            :class:`InvalidXMLAttributeValue` --
-                If the aggregator defined for this node has an unexpected value.
-        """
-
-        agg_node = mea_node.find("Aggregation")
-
-        # if there's an <Aggregation> node, get its `type`
-        # else get the `<Measure>`'s `aggregator` attribute
-        node, attr = (mea_node, "aggregator") if agg_node is None else (agg_node, "type")
-        value = _get_attr(node, attr)
-
-        try:
-            agg_type = AggregatorType.from_str(value)
-        except ValueError:
-            node_name = _get_attr(mea_node, "name")
-            raise InvalidXMLAttributeValue(node.tag, node_name, attr, value)
-        else:
-            agg_cls = Aggregator.from_enum(agg_type)
-            agg_args = {
-                str(k).replace("-", "_"): numerify(v) if is_numeric(v) else str(v)
-                for k, v in node.attrib.items()
-            }
-            return agg_cls.new(agg_args)
-
-
-class XMLCalculatedMeasure(models.CalculatedMeasure):
-    tag = "CalculatedMeasure"
-
-    @classmethod
-    def parse(cls, node: etree._Element, index: int):
-        """Parse a <CalculatedMeasure> XML node."""
-        name = _get_attr(node, "name")
-        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
-
-        return cls(
-            name=name,
-            formula=cls._parse_formula(_get_attr(node, "formula")),
-            annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-        )
-
-
-def _find_table_ref(node: etree._Element):
-    gen_tables = (item for item in node.iterchildren("InlineTable", "Table", "TableUsage"))
-    table_node = next(gen_tables, None)
-
-    if table_node is None:
-        return None
-    elif table_node.tag == "InlineTable":
-        return XMLInlineTable.parse(table_node, 0)
-    elif table_node.tag == "Table":
-        return XMLTable.parse(table_node, 0)
-    elif table_node.tag == "TableUsage":
-        return _get_attr(table_node, "source")
-
-    raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Table")
-
-
-def _get_attr(node: etree._Element, attr: str) -> str:
-    """Retrieves an attribute from a node.
-
-    If the attribute is not present, raises :class:`MissingXMLAttribute`.
-    """
-    try:
-        value = node.attrib[attr]
-    except KeyError as exc:
-        raise MissingXMLAttribute(node.tag, attr) from exc
-    else:
-        return str(value)
-
-
-def _yield_annotations(node: etree._Element) -> Iterable[Tuple[str, Optional[str]]]:
-    """Yields a pair of (name, value) for each Annotation in the node."""
-    return (
-        (_get_attr(item, "name"), item.text)
-        for item in node.iterchildren("Annotation")
-    )
-
-
-def _yield_children_nodes(
-    node: etree._Element,
-    *children: Type[AnyXMLEntity],
-    attr: str = "name",
-) -> Generator[Tuple[str, AnyXMLEntity], None, None]:
-    tags = (item.tag for item in children)
-    parsers = {item.tag: item.parse for item in children}
-    for index, item in enumerate(node.iterchildren(*tags)):
-        reducer = parsers[item.tag]
-        yield _get_attr(item, attr), reducer(item, index)
-
-
-def _yield_locale_pairs(node: etree._Element,
-                        attribute: str) -> Generator[Tuple[str, str], None, None]:
-    attr_value = node.get(attribute)
-    if attr_value is not None:
-        yield ("xx", attr_value)
-
-    for child_node in node.iterchildren("LocalizedAttr"):
-        child_attr = _get_attr(child_node, "attr")
-        if child_attr != attribute:
-            continue
-
-        child_value = child_node.get("value", child_node.text)
-        if child_value is not None:
-            yield (_get_attr(child_node, "locale"), child_value)
-
-
-def parse_xml_schema(source: Union[str, Path, TextIO]) -> XMLSchema:
-    """Attempts to parse an object into a XMLSchema.
-
-    This function accepts:
-    - A raw XML :class:`str`
-    - A local path (as a :class:`pathlib.Path`) to a XML file
-    - A not-binary read-only :class:`TextIO` instance for a file-like object
-    """
-    parser = etree.XMLParser(encoding="utf-8",
-                             remove_blank_text=True,
-                             remove_comments=True)
-
-    # if argument is str, is assumed to be a raw XML string
-    if isinstance(source, str):
-        root = etree.fromstring(source, parser)
-        return XMLSchema.parse(root)
-
-    # if argument is pathlib.Path or TextIO, open it and parse contents
-    else:
-        tree = etree.parse(source, parser)
-        root = tree.getroot()
-        return XMLSchema.parse(root)
+"""XML Schema parsing module
+
+Defines subclasses for the core Entity classes, parsed from an XML document.
+"""
+
+import logging
+from ast import literal_eval as eval_tuple
+from collections import OrderedDict
+from pathlib import Path
+from typing import (
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    TextIO,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+
+import immutables as immu
+from lxml import etree
+
+from tesseract_olap.common import is_numeric, numerify
+from tesseract_olap.exceptions.schema import (
+    InvalidXMLAttributeValue,
+    MissingXMLAttribute,
+    MissingXMLNode,
+)
+
+from . import models
+from .aggregators import Aggregator
+from .csv import parse_csv
+from .enums import AggregatorType, DimensionType, MemberType
+
+logger = logging.getLogger(__name__)
+
+XMLEntity = Union[
+    "XMLSharedDimension",
+    "XMLHierarchy",
+    "XMLLevel",
+    "XMLProperty",
+    "XMLInlineTable",
+    "XMLCube",
+    "XMLDimensionUsage",
+    "XMLHierarchyUsage",
+    "XMLLevelUsage",
+    "XMLPropertyUsage",
+    "XMLPrivateDimension",
+    "XMLMeasure",
+    "XMLCalculatedMeasure",
+]
+
+AnyXMLEntity = TypeVar("AnyXMLEntity", bound=XMLEntity)
+
+
+class XMLSchema(models.Schema):
+    tag = "Schema"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int = 0):
+        """Parse a <Schema> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        cube_gen = _yield_children_nodes(node, XMLCube)
+        shareddim_gen = _yield_children_nodes(node, XMLSharedDimension)
+        sharedtbl_gen = _yield_children_nodes(node, XMLInlineTable)
+
+        return cls(
+            name=name,
+            cube_map=OrderedDict(cube_gen),
+            shared_dimension_map=immu.Map(shareddim_gen),
+            shared_table_map=immu.Map(sharedtbl_gen),
+            default_locale=node.get("default_locale", "xx"),
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+
+class XMLAccessControl(models.AccessControl):
+    tag = "Access"
+
+    @classmethod
+    def parse(cls, node: etree._Element):
+        """Parse all <Access> XML node that are directly under this node."""
+
+        rules_gen = (
+            (role, _get_attr(item, "rule") == "allow")
+            for item in node.iterchildren(cls.tag)
+            for role in _get_attr(item, "roles").split(",")
+        )
+
+        return cls(
+            public=node.get("public", "true") == "true",
+            rules=immu.Map(rules_gen),
+        )
+
+
+class XMLCube(models.Cube):
+    tag = "Cube"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Cube> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        table = _find_table_ref(node)
+        if table is None:
+            raise MissingXMLNode(node.tag, name, "Table")
+
+        dimension_map = OrderedDict(
+            _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
+        )
+        if len(dimension_map) == 0:
+            raise MissingXMLNode(node.tag, name, "Dimension")
+
+        measure_map = OrderedDict(
+            _yield_children_nodes(node, XMLMeasure, XMLCalculatedMeasure)
+        )
+        if len(measure_map) == 0:
+            raise MissingXMLNode(node.tag, name, "Measure")
+
+        return cls(
+            name=name,
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            acl=XMLAccessControl.parse(node),
+            dimension_map=dimension_map,
+            measure_map=measure_map,
+            table=table,
+            annotations=immu.Map(_yield_annotations(node)),
+            subset_table=node.get("subset_table", "false").lower() != "false",
+            visible=node.get("visible", "true").lower() != "false",
+        )
+
+
+class XMLDimensionUsage(models.DimensionUsage):
+    tag = "DimensionUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <DimensionUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            foreign_key=_get_attr(node, "foreign_key"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            hierarchy_map=OrderedDict(
+                _yield_children_nodes(node, XMLHierarchyUsage, attr="source")
+            ),
+        )
+
+
+class XMLHierarchyUsage(models.HierarchyUsage):
+    tag = "HierarchyUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <HierarchyUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            level_map=OrderedDict(
+                _yield_children_nodes(node, XMLLevelUsage, attr="source")
+            ),
+        )
+
+
+class XMLLevelUsage(models.LevelUsage):
+    tag = "LevelUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <LevelUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            property_map=OrderedDict(
+                _yield_children_nodes(node, XMLPropertyUsage, attr="source")
+            ),
+        )
+
+
+class XMLPropertyUsage(models.PropertyUsage):
+    tag = "PropertyUsage"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <PropertyUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            source=_get_attr(node, "source"),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+        )
+
+
+class XMLTable(models.Table):
+    tag = "Table"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Table> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            schema=node.get("schema"),
+            primary_key=node.get("primary_key", "id"),
+        )
+
+
+class XMLInlineTable(models.InlineTable):
+    tag = "InlineTable"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <InlineTable> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        node_format = _get_attr(node, "format")
+
+        if node_format == "csv":
+            node_format = "text/csv"
+
+        if node_format == "tuples":
+            headers, rows = cls.parse_tuples(node)
+        elif node_format.startswith("text/csv"):
+            content = [] if node.text is None else node.text.strip().splitlines()
+            headers, *rows = parse_csv(content, mimetype=node_format)
+            headers = tuple(str(item) for item in headers)
+        else:
+            raise InvalidXMLAttributeValue(node.tag, name, "format", node_format)
+
+        return cls(
+            name=name,
+            headers=headers,
+            types=cls.infer_types(rows),
+            rows=rows,
+        )
+
+    @staticmethod
+    def parse_tuples(
+        node: etree._Element,
+    ) -> Tuple[Tuple[str, ...], List[Tuple[Union[str, float], ...]]]:
+        """Parse the child nodes from an InlineTable with `tuples` format."""
+        try:
+            # try parsing literal tuples with ast.eval()
+            children: List[Tuple[Union[str, float], ...]] = [
+                eval_tuple(line)
+                for line in (item.text for item in node.iterchildren("Row"))
+                if line
+            ]
+        except SyntaxError:
+            # Python `tuples` looks similar to CSV, so let's try with it
+            row_iter = (
+                line[1:-1] if line.startswith("(") and line.endswith(")") else line
+                for line in (item.text for item in node.iterchildren("Row"))
+                if line is not None
+            )
+            children = parse_csv(row_iter, skipinitialspace=True)
+        # at least 2 rows must be present: a header list and a data row
+        if len(children) < 2:
+            raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Row")
+        headers = tuple(str(item) for item in children[0])
+        return headers, children[1:]
+
+
+class XMLSharedDimension(models.Dimension):
+    tag = "SharedDimension"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a Shared <Dimension> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        dim_type = node.get("type")
+
+        hierarchy_map = OrderedDict(_yield_children_nodes(node, XMLHierarchy))
+
+        default_hierarchy = node.get("default_hierarchy")
+        if default_hierarchy not in hierarchy_map:
+            default_hierarchy = next(iter(hierarchy_map.keys()))
+
+        return cls(
+            name=name,
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            default_hierarchy=default_hierarchy,
+            dim_type=DimensionType.from_str(dim_type),
+            foreign_key=node.get("foreign_key"),
+            hierarchy_map=hierarchy_map,
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+
+class XMLPrivateDimension(models.Dimension):
+    tag = "Dimension"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a Private <Dimension> XML node."""
+        dimension: cls = XMLSharedDimension.parse.__func__(cls, node, index)
+
+        # foreign keys are required in Private Dimensions
+        if dimension.foreign_key is None:
+            raise MissingXMLAttribute(node.tag, "foreign_key")
+
+        return dimension
+
+
+class XMLHierarchy(models.Hierarchy):
+    tag = "Hierarchy"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Hierarchy> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        level_map = OrderedDict(_yield_children_nodes(node, XMLLevel))
+        if len(level_map) == 0:
+            raise MissingXMLNode(node.tag, name, "Level")
+
+        default_pk = ""
+        for item in level_map.values():
+            default_pk = item.key_column
+
+        return cls(
+            name=name,
+            primary_key=node.get("primary_key", default_pk),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            table=_find_table_ref(node),
+            level_map=level_map,
+            default_member=cls._parse_default_member(node),
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+    @staticmethod
+    def _parse_default_member(node: etree._Element):
+        items: List[str] = node.get("default_member", "").split(".", maxsplit=1)
+        return (items[0], items[1]) if len(items) == 2 else None
+
+
+class XMLLevel(models.Level):
+    tag = "Level"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Level> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        key_type = node.get("key_type")
+
+        return cls(
+            name=name,
+            depth=index + 1,
+            key_column=_get_attr(node, "key_column"),
+            key_type=MemberType.from_str(key_type),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            name_column_map=immu.Map(_yield_locale_pairs(node, "name_column")),
+            property_map=OrderedDict(_yield_children_nodes(node, XMLProperty)),
+            annotations=immu.Map(_yield_annotations(node)),
+        )
+
+
+class XMLProperty(models.Property):
+    tag = "Property"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Property> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        key_type = node.get("key_type")
+
+        keycol_map = immu.Map(_yield_locale_pairs(node, "key_column"))
+        if len(keycol_map) == 0:
+            raise MissingXMLAttribute(node.tag, "key_column")
+
+        return cls(
+            name=name,
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            key_column_map=keycol_map,
+            key_type=MemberType.from_str(key_type),
+        )
+
+
+class XMLMeasure(models.Measure):
+    tag = "Measure"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <Measure> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            key_column=_get_attr(node, "key_column"),
+            aggregator=cls._get_aggregator(node),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            submeasures=immu.Map(_yield_children_nodes(node, cls)),
+        )
+
+    @staticmethod
+    def _get_aggregator(mea_node: etree._Element) -> Aggregator:
+        """
+        Raises:
+            :class:`MissingXMLAttribute` --
+                If the node doesn't have an `aggregator` attribute or an
+                `<Agregation>` child node.
+
+            :class:`InvalidXMLAttributeValue` --
+                If the aggregator defined for this node has an unexpected value.
+        """
+
+        agg_node = mea_node.find("Aggregation")
+
+        # if there's an <Aggregation> node, get its `type`
+        # else get the `<Measure>`'s `aggregator` attribute
+        node, attr = (mea_node, "aggregator") if agg_node is None else (agg_node, "type")
+        value = _get_attr(node, attr)
+
+        try:
+            agg_type = AggregatorType.from_str(value)
+        except ValueError:
+            node_name = _get_attr(mea_node, "name")
+            raise InvalidXMLAttributeValue(node.tag, node_name, attr, value)
+        else:
+            agg_cls = Aggregator.from_enum(agg_type)
+            agg_args = {
+                str(k).replace("-", "_"): numerify(v) if is_numeric(v) else str(v)
+                for k, v in node.attrib.items()
+            }
+            return agg_cls.new(agg_args)
+
+
+class XMLCalculatedMeasure(models.CalculatedMeasure):
+    tag = "CalculatedMeasure"
+
+    @classmethod
+    def parse(cls, node: etree._Element, index: int):
+        """Parse a <CalculatedMeasure> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
+
+        return cls(
+            name=name,
+            formula=cls._parse_formula(_get_attr(node, "formula")),
+            annotations=immu.Map(_yield_annotations(node)),
+            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+        )
+
+
+def _find_table_ref(node: etree._Element):
+    gen_tables = (item for item in node.iterchildren("InlineTable", "Table", "TableUsage"))
+    table_node = next(gen_tables, None)
+
+    if table_node is None:
+        return None
+    elif table_node.tag == "InlineTable":
+        return XMLInlineTable.parse(table_node, 0)
+    elif table_node.tag == "Table":
+        return XMLTable.parse(table_node, 0)
+    elif table_node.tag == "TableUsage":
+        return _get_attr(table_node, "source")
+
+    raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Table")
+
+
+def _get_attr(node: etree._Element, attr: str) -> str:
+    """Retrieves an attribute from a node.
+
+    If the attribute is not present, raises :class:`MissingXMLAttribute`.
+    """
+    try:
+        value = node.attrib[attr]
+    except KeyError as exc:
+        raise MissingXMLAttribute(node.tag, attr) from exc
+    else:
+        return str(value)
+
+
+def _yield_annotations(node: etree._Element) -> Iterable[Tuple[str, Optional[str]]]:
+    """Yields a pair of (name, value) for each Annotation in the node."""
+    return (
+        (_get_attr(item, "name"), item.text)
+        for item in node.iterchildren("Annotation")
+    )
+
+
+def _yield_children_nodes(
+    node: etree._Element,
+    *children: Type[AnyXMLEntity],
+    attr: str = "name",
+) -> Generator[Tuple[str, AnyXMLEntity], None, None]:
+    tags = (item.tag for item in children)
+    parsers = {item.tag: item.parse for item in children}
+    for index, item in enumerate(node.iterchildren(*tags)):
+        reducer = parsers[item.tag]
+        yield _get_attr(item, attr), reducer(item, index)
+
+
+def _yield_locale_pairs(node: etree._Element,
+                        attribute: str) -> Generator[Tuple[str, str], None, None]:
+    attr_value = node.get(attribute)
+    if attr_value is not None:
+        yield ("xx", attr_value)
+
+    for child_node in node.iterchildren("LocalizedAttr"):
+        child_attr = _get_attr(child_node, "attr")
+        if child_attr != attribute:
+            continue
+
+        child_value = child_node.get("value", child_node.text)
+        if child_value is not None:
+            yield (_get_attr(child_node, "locale"), child_value)
+
+
+def parse_xml_schema(source: Union[str, Path, TextIO]) -> XMLSchema:
+    """Attempts to parse an object into a XMLSchema.
+
+    This function accepts:
+    - A raw XML :class:`str`
+    - A local path (as a :class:`pathlib.Path`) to a XML file
+    - A not-binary read-only :class:`TextIO` instance for a file-like object
+    """
+    parser = etree.XMLParser(encoding="utf-8",
+                             remove_blank_text=True,
+                             remove_comments=True)
+
+    # if argument is str, is assumed to be a raw XML string
+    if isinstance(source, str):
+        root = etree.fromstring(source, parser)
+        return XMLSchema.parse(root)
+
+    # if argument is pathlib.Path or TextIO, open it and parse contents
+    else:
+        tree = etree.parse(source, parser)
+        root = tree.getroot()
+        return XMLSchema.parse(root)
```

### Comparing `tesseract_olap-0.9.3/tesseract_olap/server/schema.py` & `tesseract_olap-0.9.4/tesseract_olap/server/schema.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/tesseract_olap/server/server.py` & `tesseract_olap-0.9.4/tesseract_olap/server/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.3/PKG-INFO` & `tesseract_olap-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.9.3
+Version: 0.9.4
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us
```

