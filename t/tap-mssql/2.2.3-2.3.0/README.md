# Comparing `tmp/tap_mssql-2.2.3.tar.gz` & `tmp/tap_mssql-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_mssql-2.2.3.tar", max compression
+gzip compressed data, was "tap_mssql-2.3.0.tar", max compression
```

## Comparing `tap_mssql-2.2.3.tar` & `tap_mssql-2.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0    33005 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/LICENSE
--rwxr-xr-x   0        0        0    20762 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/README.md
--rw-r--r--   0        0        0     1177 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/pyproject.toml
--rw-r--r--   0        0        0    29147 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/tap_mssql/__init__.py
--rwxr-xr-x   0        0        0     1723 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/tap_mssql/connection.py
--rwxr-xr-x   0        0        0        0 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/tap_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0    10933 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/tap_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2221 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/tap_mssql/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0     2751 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/tap_mssql/sync_strategies/incremental.py
--rw-r--r--   0        0        0    15642 2024-02-28 05:26:46.164627 tap_mssql-2.2.3/tap_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0    21856 1970-01-01 00:00:00.000000 tap_mssql-2.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0    33005 2024-04-18 22:19:08.962562 tap_mssql-2.3.0/LICENSE
+-rwxr-xr-x   0        0        0    20762 2024-04-18 22:19:08.962562 tap_mssql-2.3.0/README.md
+-rw-r--r--   0        0        0     1177 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    29147 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/tap_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1723 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/tap_mssql/connection.py
+-rwxr-xr-x   0        0        0        0 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/tap_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0    10933 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/tap_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2221 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/tap_mssql/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0     2888 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/tap_mssql/sync_strategies/incremental.py
+-rw-r--r--   0        0        0    15642 2024-04-18 22:19:08.966562 tap_mssql-2.3.0/tap_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0    21856 1970-01-01 00:00:00.000000 tap_mssql-2.3.0/PKG-INFO
```

### Comparing `tap_mssql-2.2.3/LICENSE` & `tap_mssql-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_mssql-2.2.3/README.md` & `tap_mssql-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_mssql-2.2.3/pyproject.toml` & `tap_mssql-2.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-mssql"
-version = "2.2.3"
+version = "2.3.0"
 description = "A pipelinewise compatible tap for connecting Microsoft SQL Server"
 authors = ["Rob Winters <wintersrd@gmail.com>"]
 license = "GNU Affero"
 readme = "README.md"
 homepage = "https://robertwinters.nl"
 repository = "https://github.com/wintersrd/pipelinewise-tap-mssql"
 keywords = ["singer", "meltano", "pipelinewise", "mssql"]
```

### Comparing `tap_mssql-2.2.3/tap_mssql/__init__.py` & `tap_mssql-2.3.0/tap_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `tap_mssql-2.2.3/tap_mssql/connection.py` & `tap_mssql-2.3.0/tap_mssql/connection.py`

 * *Files identical despite different names*

### Comparing `tap_mssql-2.2.3/tap_mssql/sync_strategies/common.py` & `tap_mssql-2.3.0/tap_mssql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `tap_mssql-2.2.3/tap_mssql/sync_strategies/full_table.py` & `tap_mssql-2.3.0/tap_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `tap_mssql-2.2.3/tap_mssql/sync_strategies/incremental.py` & `tap_mssql-2.3.0/tap_mssql/sync_strategies/incremental.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # pylint: disable=duplicate-code
 
 import pendulum
 import singer
+from datetime import datetime
 from singer import metadata
 
 import tap_mssql.sync_strategies.common as common
 from tap_mssql.connection import MSSQLConnection, connect_with_backoff
 
 LOGGER = singer.get_logger()
 
@@ -49,15 +50,18 @@
     with connect_with_backoff(mssql_conn) as open_conn:
         with open_conn.cursor() as cur:
             select_sql = common.generate_select_sql(catalog_entry, columns)
             params = {}
 
             if replication_key_value is not None:
                 if catalog_entry.schema.properties[replication_key_metadata].format == "date-time":
-                    replication_key_value = pendulum.parse(replication_key_value)
+                    replication_key_value = datetime.fromtimestamp(
+                        pendulum.parse(replication_key_value).timestamp()
+                    )
+                    
 
                 select_sql += ' WHERE "{}" >= %(replication_key_value)s ORDER BY "{}" ASC'.format(
                     replication_key_metadata, replication_key_metadata
                 )
 
                 params["replication_key_value"] = replication_key_value
             elif replication_key_metadata is not None:
```

### Comparing `tap_mssql-2.2.3/tap_mssql/sync_strategies/log_based.py` & `tap_mssql-2.3.0/tap_mssql/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `tap_mssql-2.2.3/PKG-INFO` & `tap_mssql-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-mssql
-Version: 2.2.3
+Version: 2.3.0
 Summary: A pipelinewise compatible tap for connecting Microsoft SQL Server
 Home-page: https://robertwinters.nl
 License: GNU Affero
 Keywords: singer,meltano,pipelinewise,mssql
 Author: Rob Winters
 Author-email: wintersrd@gmail.com
 Requires-Python: >=3.7,<4.0
```

