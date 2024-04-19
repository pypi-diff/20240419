# Comparing `tmp/barkshark-sql-0.1.3.post1.tar.gz` & `tmp/barkshark_sql-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barkshark-sql-0.1.3.post1.tar", last modified: Wed Apr 10 16:19:22 2024, max compression
+gzip compressed data, was "barkshark_sql-0.1.4.tar", last modified: Fri Apr 19 14:09:39 2024, max compression
```

## Comparing `barkshark-sql-0.1.3.post1.tar` & `barkshark_sql-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/
--rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-19 10:00:01.000000 barkshark-sql-0.1.3.post1/LICENSE.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2220 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-03-10 22:34:07.000000 barkshark-sql-0.1.3.post1/README.md
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2220 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      389 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-10 16:19:22.000000 barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/top_level.txt
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/bsql/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      540 2024-04-10 16:19:14.000000 barkshark-sql-0.1.3.post1/bsql/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     5350 2024-04-10 16:13:17.000000 barkshark-sql-0.1.3.post1/bsql/backends.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    18977 2024-04-02 20:23:43.000000 barkshark-sql-0.1.3.post1/bsql/database.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1178 2024-04-02 20:23:36.000000 barkshark-sql-0.1.3.post1/bsql/enums.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4174 2024-04-08 18:44:46.000000 barkshark-sql-0.1.3.post1/bsql/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-10 22:38:06.000000 barkshark-sql-0.1.3.post1/bsql/py.typed
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7209 2024-04-02 20:23:25.000000 barkshark-sql-0.1.3.post1/bsql/statement.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     7732 2024-04-01 17:49:07.000000 barkshark-sql-0.1.3.post1/bsql/table.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     2089 2024-04-01 18:22:58.000000 barkshark-sql-0.1.3.post1/pyproject.toml
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/setup.cfg
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-10 16:19:22.222621 barkshark-sql-0.1.3.post1/tests/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1880 2024-04-01 18:22:11.000000 barkshark-sql-0.1.3.post1/tests/test_statements.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)      654 2024-04-01 18:22:18.000000 barkshark-sql-0.1.3.post1/tests/test_tables.py
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-19 14:09:39.415125 barkshark_sql-0.1.4/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-19 10:00:01.000000 barkshark_sql-0.1.4/LICENSE.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-19 14:09:39.411125 barkshark_sql-0.1.4/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-03-10 22:34:07.000000 barkshark_sql-0.1.4/README.md
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-19 14:09:39.411125 barkshark_sql-0.1.4/barkshark_sql.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2214 2024-04-19 14:09:39.000000 barkshark_sql-0.1.4/barkshark_sql.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      389 2024-04-19 14:09:39.000000 barkshark_sql-0.1.4/barkshark_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-19 14:09:39.000000 barkshark_sql-0.1.4/barkshark_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-19 14:09:39.000000 barkshark_sql-0.1.4/barkshark_sql.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        5 2024-04-19 14:09:39.000000 barkshark_sql-0.1.4/barkshark_sql.egg-info/top_level.txt
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-19 14:09:39.411125 barkshark_sql-0.1.4/bsql/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      538 2024-04-19 14:06:24.000000 barkshark_sql-0.1.4/bsql/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     5350 2024-04-10 16:13:17.000000 barkshark_sql-0.1.4/bsql/backends.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    19046 2024-04-19 03:32:13.000000 barkshark_sql-0.1.4/bsql/database.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1178 2024-04-02 20:23:36.000000 barkshark_sql-0.1.4/bsql/enums.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4174 2024-04-08 18:44:46.000000 barkshark_sql-0.1.4/bsql/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-10 22:38:06.000000 barkshark_sql-0.1.4/bsql/py.typed
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7209 2024-04-02 20:23:25.000000 barkshark_sql-0.1.4/bsql/statement.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     7732 2024-04-01 17:49:07.000000 barkshark_sql-0.1.4/bsql/table.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     2089 2024-04-01 18:22:58.000000 barkshark_sql-0.1.4/pyproject.toml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-19 14:09:39.415125 barkshark_sql-0.1.4/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-19 14:09:39.411125 barkshark_sql-0.1.4/tests/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1880 2024-04-01 18:22:11.000000 barkshark_sql-0.1.4/tests/test_statements.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      654 2024-04-01 18:22:18.000000 barkshark_sql-0.1.4/tests/test_tables.py
```

### Comparing `barkshark-sql-0.1.3.post1/LICENSE.md` & `barkshark_sql-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/PKG-INFO` & `barkshark_sql-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-sql
-Version: 0.1.3.post1
+Version: 0.1.4
 Summary: Connection pool and query builder for dbapi 2.0 database drivers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/bsql
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/bsql/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/barkshark-sql
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/bsql
```

### Comparing `barkshark-sql-0.1.3.post1/README.md` & `barkshark_sql-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/barkshark_sql.egg-info/PKG-INFO` & `barkshark_sql-0.1.4/barkshark_sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barkshark-sql
-Version: 0.1.3.post1
+Version: 0.1.4
 Summary: Connection pool and query builder for dbapi 2.0 database drivers
 Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/bsql
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/bsql/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/barkshark-sql
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/bsql
```

### Comparing `barkshark-sql-0.1.3.post1/bsql/backends.py` & `barkshark_sql-0.1.4/bsql/backends.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/bsql/database.py` & `barkshark_sql-0.1.4/bsql/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 	"Manages a pool of database connections"
 
 	def __init__(self,
 				backend_name: str,
 				database: str,
 				host: str | Path = Path("/var/run/postgresql"),
 				port: int = 5432,
-				username: str = getuser(),
+				username: str | None = None,
 				password: str | None = None,
 				connection_class: type[T] = Connection, # type: ignore
 				pool_size: int = 5,
 				pool_timeout: int = 5,
 				tables: Tables | dict[str, Any] | str | None = None,
 				prepared_statements: dict[str, str] | None = None,
 				**kwargs: Any):
@@ -367,15 +367,15 @@
 
 		self.host: str | Path = host
 		"Address or unix socket for connecting to the server"
 
 		self.port: int = port
 		"Port the server is listening on"
 
-		self.username: str = username
+		self.username: str = username or getuser(z)
 		"User to connect to the server with"
 
 		self.password: str | None = password
 		"Password of the user"
 
 		self.arguments: dict[str, Any] = kwargs
 		"Arguments to pass to the backend connection function"
@@ -512,14 +512,16 @@
 
 			:param start_trans: Start a transaction on the connection
 		"""
 
 		if not self.connected:
 			self.connect()
 
+		conn: T | None = None
+
 		try:
 			conn = self._pool.get(block = True, timeout = self.pool_timeout)
 
 			if start_trans:
 				conn.begin()
 
 			elif not conn.connected:
@@ -536,19 +538,20 @@
 		except Exception as e:
 			if conn and conn.in_transaction:
 				conn.rollback()
 
 			raise e
 
 		finally:
-			if self.connected:
-				self._pool.put(conn)
+			if conn is not None:
+				if self.connected:
+					self._pool.put(conn)
 
-			else:
-				conn.disconnect()
+				else:
+					conn.disconnect()
 
 
 	def connect(self) -> None:
 		"Create connections up to the amount specified by :attr:`Database.pool_size`"
 
 		if self.connected:
 			return
```

### Comparing `barkshark-sql-0.1.3.post1/bsql/enums.py` & `barkshark_sql-0.1.4/bsql/enums.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/bsql/misc.py` & `barkshark_sql-0.1.4/bsql/misc.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/bsql/statement.py` & `barkshark_sql-0.1.4/bsql/statement.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/bsql/table.py` & `barkshark_sql-0.1.4/bsql/table.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/pyproject.toml` & `barkshark_sql-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/tests/test_statements.py` & `barkshark_sql-0.1.4/tests/test_statements.py`

 * *Files identical despite different names*

### Comparing `barkshark-sql-0.1.3.post1/tests/test_tables.py` & `barkshark_sql-0.1.4/tests/test_tables.py`

 * *Files identical despite different names*

