# Comparing `tmp/uagents-0.9.2.tar.gz` & `tmp/uagents-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents-0.9.2.tar", max compression
+gzip compressed data, was "uagents-0.9.3.tar", max compression
```

## Comparing `uagents-0.9.2.tar` & `uagents-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      442 2023-12-14 11:40:20.485416 uagents-0.9.2/README.md
--rw-r--r--   0        0        0     1176 2023-12-14 11:40:20.493416 uagents-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      119 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/__init__.py
--rw-r--r--   0        0        0    37798 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/agent.py
--rw-r--r--   0        0        0    10413 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/asgi.py
--rw-r--r--   0        0        0     3531 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/config.py
--rw-r--r--   0        0        0    20464 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/context.py
--rw-r--r--   0        0        0        0 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/contrib/protocols/__init__.py
--rw-r--r--   0        0        0      751 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/contrib/protocols/protocol_query.py
--rw-r--r--   0        0        0     6280 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/crypto/__init__.py
--rw-r--r--   0        0        0     1369 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/dispatch.py
--rw-r--r--   0        0        0     3367 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/envelope.py
--rw-r--r--   0        0        0     8824 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/mailbox.py
--rw-r--r--   0        0        0      464 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/models.py
--rw-r--r--   0        0        0    14175 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/network.py
--rw-r--r--   0        0        0    11560 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/protocol.py
--rw-r--r--   0        0        0     4109 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/query.py
--rw-r--r--   0        0        0     9197 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/resolver.py
--rw-r--r--   0        0        0     1860 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/setup.py
--rw-r--r--   0        0        0     3855 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/storage/__init__.py
--rw-r--r--   0        0        0     2891 2023-12-14 11:40:20.493416 uagents-0.9.2/src/uagents/wallet_messaging.py
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 uagents-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      430 2024-01-12 09:43:03.430566 uagents-0.9.3/README.md
+-rw-r--r--   0        0        0     1176 2024-01-12 09:43:03.434566 uagents-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      119 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/__init__.py
+-rw-r--r--   0        0        0    37798 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/agent.py
+-rw-r--r--   0        0        0    10413 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/asgi.py
+-rw-r--r--   0        0        0     3531 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/config.py
+-rw-r--r--   0        0        0    20464 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/context.py
+-rw-r--r--   0        0        0        0 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/contrib/protocols/__init__.py
+-rw-r--r--   0        0        0      751 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/contrib/protocols/protocol_query.py
+-rw-r--r--   0        0        0     6280 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/crypto/__init__.py
+-rw-r--r--   0        0        0     1369 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/dispatch.py
+-rw-r--r--   0        0        0     3367 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/envelope.py
+-rw-r--r--   0        0        0     8824 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/mailbox.py
+-rw-r--r--   0        0        0      464 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/models.py
+-rw-r--r--   0        0        0    14175 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/network.py
+-rw-r--r--   0        0        0    11560 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/protocol.py
+-rw-r--r--   0        0        0     4109 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/query.py
+-rw-r--r--   0        0        0     9197 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/resolver.py
+-rw-r--r--   0        0        0     1860 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/setup.py
+-rw-r--r--   0        0        0     3855 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/storage/__init__.py
+-rw-r--r--   0        0        0     2891 2024-01-12 09:43:03.434566 uagents-0.9.3/src/uagents/wallet_messaging.py
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 uagents-0.9.3/PKG-INFO
```

### Comparing `uagents-0.9.2/pyproject.toml` & `uagents-0.9.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "uagents"
-version = "0.9.2"
+version = "0.9.3"
 description = "Lightweight framework for rapid agent-based development"
 authors = ["Ed FitzGerald <edward.fitzgerald@fetch.ai>", "James Riehl <james.riehl@fetch.ai>", "Alejandro Morales <alejandro.madrigal@fetch.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8,<3.13"
 pydantic = "^1.10.2"
 msgpack = "^1.0.4"
 bech32 = "^1.2.0"
 ecdsa = "^0.18.0"
 apispec = "^6.0.2"
 uvicorn = "^0.20.0"
 aiohttp = "^3.8.3"
-cosmpy = "^0.9.1"
+cosmpy = "^0.9.2"
 websockets = "^10.4"
 
 # extras
 fetchai-babble = {version = "^0.4.0", optional = true}
 tortoise-orm = {version = "^0.19.2", optional = true}
 geopy = {version = "^2.3.0", optional = true}
 pyngrok = {version = "^5.2.3", optional = true}
```

### Comparing `uagents-0.9.2/src/uagents/agent.py` & `uagents-0.9.3/src/uagents/agent.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/asgi.py` & `uagents-0.9.3/src/uagents/asgi.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/config.py` & `uagents-0.9.3/src/uagents/config.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/context.py` & `uagents-0.9.3/src/uagents/context.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/contrib/protocols/protocol_query.py` & `uagents-0.9.3/src/uagents/contrib/protocols/protocol_query.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/crypto/__init__.py` & `uagents-0.9.3/src/uagents/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/dispatch.py` & `uagents-0.9.3/src/uagents/dispatch.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/envelope.py` & `uagents-0.9.3/src/uagents/envelope.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/mailbox.py` & `uagents-0.9.3/src/uagents/mailbox.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/network.py` & `uagents-0.9.3/src/uagents/network.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/protocol.py` & `uagents-0.9.3/src/uagents/protocol.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/query.py` & `uagents-0.9.3/src/uagents/query.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/resolver.py` & `uagents-0.9.3/src/uagents/resolver.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/setup.py` & `uagents-0.9.3/src/uagents/setup.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/storage/__init__.py` & `uagents-0.9.3/src/uagents/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/src/uagents/wallet_messaging.py` & `uagents-0.9.3/src/uagents/wallet_messaging.py`

 * *Files identical despite different names*

### Comparing `uagents-0.9.2/PKG-INFO` & `uagents-0.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: uagents
-Version: 0.9.2
+Version: 0.9.3
 Summary: Lightweight framework for rapid agent-based development
 License: Apache 2.0
 Author: Ed FitzGerald
 Author-email: edward.fitzgerald@fetch.ai
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: geo
 Provides-Extra: orm
 Provides-Extra: remote-agents
 Provides-Extra: wallet
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: apispec (>=6.0.2,<7.0.0)
 Requires-Dist: bech32 (>=1.2.0,<2.0.0)
-Requires-Dist: cosmpy (>=0.9.1,<0.10.0)
+Requires-Dist: cosmpy (>=0.9.2,<0.10.0)
 Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
 Requires-Dist: fetchai-babble (>=0.4.0,<0.5.0) ; extra == "all" or extra == "wallet"
 Requires-Dist: geopy (>=2.3.0,<3.0.0) ; extra == "all" or extra == "geo"
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyngrok (>=5.2.3,<6.0.0) ; extra == "all" or extra == "remote-agents"
 Requires-Dist: tortoise-orm (>=0.19.2,<0.20.0) ; extra == "all" or extra == "orm"
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Description-Content-Type: text/markdown
 
 ## Installation (Python)
 
-Install μAgents for Python 3.8, 3.9, 3.10, or 3.11:
+Install μAgents for Python 3.8 to 3.12:
 
 ```bash
 poetry install
 poetry shell
 ```
 
 ## Documentation
```

