# Comparing `tmp/fakesnow-0.9.7.tar.gz` & `tmp/fakesnow-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.9.7.tar", last modified: Wed Apr 17 21:12:47 2024, max compression
+gzip compressed data, was "fakesnow-0.9.8.tar", last modified: Fri Apr 19 06:37:41 2024, max compression
```

## Comparing `fakesnow-0.9.7.tar` & `fakesnow-0.9.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.081417 fakesnow-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 21:12:41.000000 fakesnow-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-17 21:12:47.081417 fakesnow-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-17 21:12:41.000000 fakesnow-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.073417 fakesnow-0.9.7/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    28929 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/global_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/info_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    48818 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.077417 fakesnow-0.9.7/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-17 21:12:41.000000 fakesnow-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:12:47.081417 fakesnow-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.077417 fakesnow-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    66139 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_info_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    32132 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.287021 fakesnow-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 06:37:31.000000 fakesnow-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-19 06:37:41.287021 fakesnow-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-19 06:37:31.000000 fakesnow-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.279021 fakesnow-0.9.8/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29442 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/global_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    49714 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.283021 fakesnow-0.9.8/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-19 06:37:31.000000 fakesnow-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:37:41.287021 fakesnow-0.9.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.283021 fakesnow-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67797 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33081 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_users.py
```

### Comparing `fakesnow-0.9.7/LICENSE` & `fakesnow-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/PKG-INFO` & `fakesnow-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.9.7
+Version: 0.9.8
 Summary: Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fakesnow-0.9.7/README.md` & `fakesnow-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/fakesnow/__init__.py` & `fakesnow-0.9.8/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/fakesnow/checks.py` & `fakesnow-0.9.8/fakesnow/checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/fakesnow/cli.py` & `fakesnow-0.9.8/fakesnow/cli.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/fakesnow/expr.py` & `fakesnow-0.9.8/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/fakesnow/fakes.py` & `fakesnow-0.9.8/fakesnow/fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 from collections.abc import Iterable, Iterator, Sequence
 from pathlib import Path
 from string import Template
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Literal, Optional, cast
 
 import duckdb
+from sqlglot import exp
 
 if TYPE_CHECKING:
     import pandas as pd
     import pyarrow.lib
 import pyarrow
 import snowflake.connector.converter
 import snowflake.connector.errors
 import sqlglot
 from duckdb import DuckDBPyConnection
 from snowflake.connector.cursor import DictCursor, ResultMetadata, SnowflakeCursor
 from snowflake.connector.result_batch import ResultBatch
-from sqlglot import exp, parse_one
+from sqlglot import parse_one
 from typing_extensions import Self
 
 import fakesnow.checks as checks
 import fakesnow.expr as expr
 import fakesnow.info_schema as info_schema
 import fakesnow.macros as macros
 import fakesnow.transforms as transforms
@@ -108,76 +109,57 @@
         self.execute(describe, *args, **kwargs)
         return FakeSnowflakeCursor._describe_as_result_metadata(self.fetchall())
 
     @property
     def description(self) -> list[ResultMetadata]:
         # use a separate cursor to avoid consuming the result set on this cursor
         with self._conn.cursor() as cur:
-            cur.execute(f"DESCRIBE {self._last_sql}", self._last_params)
+            # self._duck_conn.execute(sql, params)
+            expression = sqlglot.parse_one(f"DESCRIBE {self._last_sql}", read="duckdb")
+            cur._execute(expression, self._last_params)  # noqa: SLF001
             meta = FakeSnowflakeCursor._describe_as_result_metadata(cur.fetchall())
 
         return meta
 
     def execute(
         self,
         command: str,
         params: Sequence[Any] | dict[Any, Any] | None = None,
         *args: Any,
         **kwargs: Any,
     ) -> FakeSnowflakeCursor:
         try:
             self._sqlstate = None
-            return self._execute(command, params, *args, **kwargs)
+
+            if os.environ.get("FAKESNOW_DEBUG") == "snowflake":
+                print(f"{command};{params=}" if params else f"{command};", file=sys.stderr)
+
+            command, params = self._rewrite_with_params(command, params)
+            expression = parse_one(command, read="snowflake")
+            transformed = self._transform(expression)
+            return self._execute(transformed, params)
         except snowflake.connector.errors.ProgrammingError as e:
             self._sqlstate = e.sqlstate
             raise e
 
-    def _execute(
-        self,
-        command: str,
-        params: Sequence[Any] | dict[Any, Any] | None = None,
-        *args: Any,
-        **kwargs: Any,
-    ) -> FakeSnowflakeCursor:
-        self._arrow_table = None
-        self._arrow_table_fetch_index = None
-        self._rowcount = None
-
-        command, params = self._rewrite_with_params(command, params)
-        expression = parse_one(command, read="snowflake")
-
-        cmd = expr.key_command(expression)
-
-        no_database, no_schema = checks.is_unqualified_table_expression(expression)
-
-        if no_database and not self._conn.database_set:
-            raise snowflake.connector.errors.ProgrammingError(
-                msg=f"Cannot perform {cmd}. This session does not have a current database. Call 'USE DATABASE', or use a qualified name.",  # noqa: E501
-                errno=90105,
-                sqlstate="22000",
-            )
-        elif no_schema and not self._conn.schema_set:
-            raise snowflake.connector.errors.ProgrammingError(
-                msg=f"Cannot perform {cmd}. This session does not have a current schema. Call 'USE SCHEMA', or use a qualified name.",  # noqa: E501
-                errno=90106,
-                sqlstate="22000",
-            )
-
-        transformed = (
+    def _transform(self, expression: exp.Expression) -> exp.Expression:
+        return (
             expression.transform(transforms.upper_case_unquoted_identifiers)
             .transform(transforms.set_schema, current_database=self._conn.database)
             .transform(transforms.create_database, db_path=self._conn.db_path)
             .transform(transforms.extract_comment_on_table)
             .transform(transforms.extract_comment_on_columns)
             .transform(transforms.information_schema_fs_columns_snowflake)
             .transform(transforms.information_schema_fs_tables_ext)
             .transform(transforms.drop_schema_cascade)
             .transform(transforms.tag)
             .transform(transforms.semi_structured_types)
             .transform(transforms.try_parse_json)
+            # NOTE: trim_cast_varchar must be before json_extract_cast_as_varchar
+            .transform(transforms.trim_cast_varchar)
             # indices_to_json_extract must be before regex_substr
             .transform(transforms.indices_to_json_extract)
             .transform(transforms.json_extract_cast_as_varchar)
             .transform(transforms.json_extract_cased_as_varchar)
             .transform(transforms.json_extract_precedence)
             .transform(transforms.flatten)
             .transform(transforms.regex_replace)
@@ -208,23 +190,48 @@
             .transform(lambda e: transforms.show_keys(e, self._conn.database, kind="PRIMARY"))
             .transform(lambda e: transforms.show_keys(e, self._conn.database, kind="UNIQUE"))
             .transform(lambda e: transforms.show_keys(e, self._conn.database, kind="FOREIGN"))
             .transform(transforms.show_users)
             .transform(transforms.create_user)
             .transform(transforms.sha256)
         )
+
+    def _execute(
+        self, transformed: exp.Expression, params: Sequence[Any] | dict[Any, Any] | None = None
+    ) -> FakeSnowflakeCursor:
+        self._arrow_table = None
+        self._arrow_table_fetch_index = None
+        self._rowcount = None
+
+        cmd = expr.key_command(transformed)
+
+        no_database, no_schema = checks.is_unqualified_table_expression(transformed)
+
+        if no_database and not self._conn.database_set:
+            raise snowflake.connector.errors.ProgrammingError(
+                msg=f"Cannot perform {cmd}. This session does not have a current database. Call 'USE DATABASE', or use a qualified name.",  # noqa: E501
+                errno=90105,
+                sqlstate="22000",
+            )
+        elif no_schema and not self._conn.schema_set:
+            raise snowflake.connector.errors.ProgrammingError(
+                msg=f"Cannot perform {cmd}. This session does not have a current schema. Call 'USE SCHEMA', or use a qualified name.",  # noqa: E501
+                errno=90106,
+                sqlstate="22000",
+            )
+
         sql = transformed.sql(dialect="duckdb")
-        result_sql = None
 
         if transformed.find(exp.Select) and (seed := transformed.args.get("seed")):
             sql = f"SELECT setseed({seed}); {sql}"
 
-        if fs_debug := os.environ.get("FAKESNOW_DEBUG"):
-            debug = command if fs_debug == "snowflake" else sql
-            print(f"{debug};{params=}" if params else f"{debug};", file=sys.stderr)
+        if (fs_debug := os.environ.get("FAKESNOW_DEBUG")) and fs_debug != "snowflake":
+            print(f"{sql};{params=}" if params else f"{sql};", file=sys.stderr)
+
+        result_sql = None
 
         try:
             self._duck_conn.execute(sql, params)
         except duckdb.BinderException as e:
             msg = e.args[0]
             raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2043, sqlstate="02000") from None
         except duckdb.CatalogException as e:
@@ -240,52 +247,27 @@
             else:
                 raise e
         except duckdb.ConnectionException as e:
             raise snowflake.connector.errors.DatabaseError(msg=e.args[0], errno=250002, sqlstate="08003") from None
 
         affected_count = None
 
-        if (maybe_ident := expression.find(exp.Identifier, bfs=False)) and isinstance(maybe_ident.this, str):
-            ident = maybe_ident.this if maybe_ident.quoted else maybe_ident.this.upper()
-        else:
-            ident = None
-
-        if cmd == "USE DATABASE" and ident:
-            self._conn.database = ident
+        if set_database := transformed.args.get("set_database"):
+            self._conn.database = set_database
             self._conn.database_set = True
 
-        elif cmd == "USE SCHEMA" and ident:
-            self._conn.schema = ident
+        elif set_schema := transformed.args.get("set_schema"):
+            self._conn.schema = set_schema
             self._conn.schema_set = True
 
         elif create_db_name := transformed.args.get("create_db_name"):
             # we created a new database, so create the info schema extensions
             self._duck_conn.execute(info_schema.creation_sql(create_db_name))
             result_sql = SQL_CREATED_DATABASE.substitute(name=create_db_name)
 
-        elif cmd == "CREATE SCHEMA" and ident:
-            result_sql = SQL_CREATED_SCHEMA.substitute(name=ident)
-
-        elif cmd == "CREATE TABLE" and ident:
-            result_sql = SQL_CREATED_TABLE.substitute(name=ident)
-
-        elif cmd == "CREATE VIEW" and ident:
-            result_sql = SQL_CREATED_VIEW.substitute(name=ident)
-
-        elif cmd.startswith("DROP") and ident:
-            result_sql = SQL_DROPPED.substitute(name=ident)
-
-            # if dropping the current database/schema then reset conn metadata
-            if cmd == "DROP DATABASE" and ident == self._conn.database:
-                self._conn.database = None
-                self._conn.schema = None
-
-            elif cmd == "DROP SCHEMA" and ident == self._conn.schema:
-                self._conn.schema = None
-
         elif cmd == "INSERT":
             (affected_count,) = self._duck_conn.fetchall()[0]
             result_sql = SQL_INSERTED_ROWS.substitute(count=affected_count)
 
         elif cmd == "UPDATE":
             (affected_count,) = self._duck_conn.fetchall()[0]
             result_sql = SQL_UPDATED_ROWS.substitute(count=affected_count)
@@ -297,14 +279,36 @@
         elif cmd == "DESCRIBE TABLE":
             # DESCRIBE TABLE has already been run above to detect and error if the table exists
             # We now rerun DESCRIBE TABLE but transformed with columns to match Snowflake
             result_sql = transformed.transform(
                 lambda e: transforms.describe_table(e, self._conn.database, self._conn.schema)
             ).sql(dialect="duckdb")
 
+        elif (eid := transformed.find(exp.Identifier, bfs=False)) and isinstance(eid.this, str):
+            ident = eid.this if eid.quoted else eid.this.upper()
+            if cmd == "CREATE SCHEMA" and ident:
+                result_sql = SQL_CREATED_SCHEMA.substitute(name=ident)
+
+            elif cmd == "CREATE TABLE" and ident:
+                result_sql = SQL_CREATED_TABLE.substitute(name=ident)
+
+            elif cmd == "CREATE VIEW" and ident:
+                result_sql = SQL_CREATED_VIEW.substitute(name=ident)
+
+            elif cmd.startswith("DROP") and ident:
+                result_sql = SQL_DROPPED.substitute(name=ident)
+
+                # if dropping the current database/schema then reset conn metadata
+                if cmd == "DROP DATABASE" and ident == self._conn.database:
+                    self._conn.database = None
+                    self._conn.schema = None
+
+                elif cmd == "DROP SCHEMA" and ident == self._conn.schema:
+                    self._conn.schema = None
+
         if table_comment := cast(tuple[exp.Table, str], transformed.args.get("table_comment")):
             # record table comment
             table, comment = table_comment
             catalog = table.catalog or self._conn.database
             schema = table.db or self._conn.schema
             assert catalog and schema
             self._duck_conn.execute(info_schema.insert_table_comment_sql(catalog, schema, table.name, comment))
```

### Comparing `fakesnow-0.9.7/fakesnow/global_database.py` & `fakesnow-0.9.8/fakesnow/global_database.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/fakesnow/info_schema.py` & `fakesnow-0.9.8/fakesnow/info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/fakesnow/transforms.py` & `fakesnow-0.9.8/fakesnow/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,29 +562,32 @@
     """Return raw unquoted string when casting json extraction to varchar.
 
     Returns a raw string using the Duckdb ->> operator, aka the json_extract_string function, see
     https://duckdb.org/docs/extensions/json#json-extraction-functions
     """
     if (
         isinstance(expression, exp.Cast)
+        and (to := expression.to)
+        and isinstance(to, exp.DataType)
+        and to.this in {exp.DataType.Type.VARCHAR, exp.DataType.Type.TEXT}
         and (je := expression.this)
         and isinstance(je, exp.JSONExtract)
         and (path := je.expression)
         and isinstance(path, exp.JSONPath)
     ):
         return exp.JSONExtractScalar(this=je.this, expression=path)
     return expression
 
 
 def json_extract_precedence(expression: exp.Expression) -> exp.Expression:
     """Associate json extract operands to avoid duckdb operators of higher precedence transforming the expression.
 
     See https://github.com/tekumara/fakesnow/issues/53
     """
-    if isinstance(expression, exp.JSONExtract):
+    if isinstance(expression, (exp.JSONExtract, exp.JSONExtractScalar)):
         return exp.Paren(this=expression)
     return expression
 
 
 def random(expression: exp.Expression) -> exp.Expression:
     """Convert random() and random(seed).
 
@@ -775,26 +778,30 @@
         and kind.name
         and kind.name.upper() in ["SCHEMA", "DATABASE"]
     ):
         assert expression.this, f"No identifier for USE expression {expression}"
 
         if kind.name.upper() == "DATABASE":
             # duckdb's default schema is main
-            name = f"{expression.this.name}.main"
+            database = expression.this.name
+            return exp.Command(
+                this="SET", expression=exp.Literal.string(f"schema = '{database}.main'"), set_database=database
+            )
         else:
             # SCHEMA
             if db := expression.this.args.get("db"):  # noqa: SIM108
                 db_name = db.name
             else:
                 # isn't qualified with a database
                 db_name = current_database or MISSING_DATABASE
 
-            name = f"{db_name}.{expression.this.name}"
-
-        return exp.Command(this="SET", expression=exp.Literal.string(f"schema = '{name}'"))
+            schema = expression.this.name
+            return exp.Command(
+                this="SET", expression=exp.Literal.string(f"schema = '{db_name}.{schema}'"), set_schema=schema
+            )
 
     return expression
 
 
 def show_objects_tables(expression: exp.Expression, current_database: str | None = None) -> exp.Expression:
     """Transform SHOW OBJECTS/TABLES to a query against the information_schema.tables table.
 
@@ -1091,14 +1098,29 @@
         new = expression.copy()
         del new.args["expressions"]
         return new
 
     return expression
 
 
+def trim_cast_varchar(expression: exp.Expression) -> exp.Expression:
+    """Snowflake's TRIM casts input to VARCHAR implicitly."""
+
+    if not (isinstance(expression, exp.Trim)):
+        return expression
+
+    operand = expression.this
+    if isinstance(operand, exp.Cast) and operand.to.this in [exp.DataType.Type.VARCHAR, exp.DataType.Type.TEXT]:
+        return expression
+
+    return exp.Trim(
+        this=exp.Cast(this=operand, to=exp.DataType(this=exp.DataType.Type.VARCHAR, nested=False, prefix=False))
+    )
+
+
 def try_parse_json(expression: exp.Expression) -> exp.Expression:
     """Convert TRY_PARSE_JSON() to TRY_CAST(... as JSON).
 
     Example:
         >>> import sqlglot
         >>> sqlglot.parse_one("select try_parse_json('{}')").transform(parse_json).sql()
         "SELECT TRY_CAST('{}' AS JSON)"
```

### Comparing `fakesnow-0.9.7/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.9.8/fakesnow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.9.7
+Version: 0.9.8
 Summary: Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `fakesnow-0.9.7/fakesnow.egg-info/SOURCES.txt` & `fakesnow-0.9.8/fakesnow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/pyproject.toml` & `fakesnow-0.9.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally."
-version = "0.9.7"
+version = "0.9.8"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.10.0",
```

### Comparing `fakesnow-0.9.7/tests/test_checks.py` & `fakesnow-0.9.8/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/tests/test_cli.py` & `fakesnow-0.9.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/tests/test_expr.py` & `fakesnow-0.9.8/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/tests/test_fakes.py` & `fakesnow-0.9.8/tests/test_fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -608,14 +608,25 @@
     # fmt: off
     assert dcur.description == [
         ResultMetadata(name='number of rows deleted', type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True),
     ]
     # fmt: on
 
 
+def test_description_select(dcur: snowflake.connector.cursor.DictCursor):
+    dcur.execute("SELECT DATEDIFF( DAY, '2023-04-02'::DATE, '2023-04-05'::DATE) as days")
+    assert dcur.fetchall() == [{"DAYS": 3}]
+    # TODO: Snowflake is actually precision=9, is_nullable=False
+    # fmt: off
+    assert dcur.description == [
+        ResultMetadata(name='DAYS', type_code=0, display_size=None, internal_size=None, precision=38, scale=0, is_nullable=True),
+    ]
+    # fmt: on
+
+
 def test_equal_null(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("select equal_null(NULL, NULL), equal_null(1, 1), equal_null(1, 2), equal_null(1, NULL)")
     assert cur.fetchall() == [(True, True, False, False)]
 
 
 def test_executemany(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
@@ -788,14 +799,19 @@
     assert cur.fetchall() == [("42",)]
 
 
 def test_get_path_precedence(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("select {'K1': {'K2': 1}} as col where col:K1:K2 > 0")
     assert indent(cur.fetchall()) == [('{\n  "K1": {\n    "K2": 1\n  }\n}',)]
 
+    cur.execute(
+        """select parse_json('{"K1": "a", "K2": "b"}') as col, case when col:K1::VARCHAR = 'a' and col:K2::VARCHAR = 'b' then 'yes' end"""
+    )
+    assert indent(cur.fetchall()) == [('{\n  "K1": "a",\n  "K2": "b"\n}', "yes")]
+
 
 def test_get_result_batches(cur: snowflake.connector.cursor.SnowflakeCursor):
     # no result set
     assert cur.get_result_batches() is None
 
     cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
     cur.execute("insert into customers values (1, 'Jenny', 'P')")
@@ -1389,14 +1405,22 @@
         assert cur.fetchall() == [("Statement executed successfully.",)]
 
         cur.execute("ROLLBACK")
         assert cur.description == [ResultMetadata(name='status', type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True)]  # fmt: skip
         assert cur.fetchall() == [("Statement executed successfully.",)]
 
 
+def test_trim_cast_varchar(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute("select trim(1), trim('  name 1  ')")
+    assert cur.fetchall() == [("1", "name 1")]
+
+    cur.execute("""select trim(parse_json('{"k1": "   v11  "}'):k1), trim(parse_json('{"k1": 21}'):k1)""")
+    assert cur.fetchall() == [("v11", "21")]
+
+
 def test_unquoted_identifiers_are_upper_cased(dcur: snowflake.connector.cursor.SnowflakeCursor):
     dcur.execute("create table customers (id int, first_name varchar, last_name varchar)")
     dcur.execute("insert into customers values (1, 'Jenny', 'P')")
     dcur.execute("select first_name, first_name as fname from customers")
 
     assert dcur.fetchall() == [
         {"FIRST_NAME": "Jenny", "FNAME": "Jenny"},
@@ -1446,14 +1470,25 @@
 
         assert cur.fetchall() == [
             {"COLUMN2": 1, "COLUMN1": "Amsterdam", "PJ": "[]"},
             {"COLUMN2": 2, "COLUMN1": "London", "PJ": "{}"},
         ]
 
 
+def test_json_extract_cast_as_varchar(dcur: snowflake.connector.cursor.DictCursor):
+    dcur.execute("CREATE TABLE example (j VARIANT)")
+    dcur.execute("""INSERT INTO example SELECT PARSE_JSON('{"str": "100", "number" : 100}')""")
+
+    dcur.execute("SELECT j:str::varchar as c_str_varchar, j:number::varchar as c_num_varchar  FROM example")
+    assert dcur.fetchall() == [{"C_STR_VARCHAR": "100", "C_NUM_VARCHAR": "100"}]
+
+    dcur.execute("SELECT j:str::number as c_str_number, j:number::number as c_num_number  FROM example")
+    assert dcur.fetchall() == [{"C_STR_NUMBER": 100, "C_NUM_NUMBER": 100}]
+
+
 def test_write_pandas_quoted_column_names(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor(snowflake.connector.cursor.DictCursor) as dcur:
         # colunmn names with spaces
         dcur.execute('create table customers (id int, "first name" varchar)')
         df = pd.DataFrame.from_records(
             [
                 {"ID": 1, "first name": "Jenny"},
```

### Comparing `fakesnow-0.9.7/tests/test_info_schema.py` & `fakesnow-0.9.8/tests/test_info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/tests/test_patch.py` & `fakesnow-0.9.8/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/tests/test_sqlalchemy.py` & `fakesnow-0.9.8/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.7/tests/test_transforms.py` & `fakesnow-0.9.8/tests/test_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     show_schemas,
     tag,
     timestamp_ntz_ns,
     to_date,
     to_decimal,
     to_timestamp,
     to_timestamp_ntz,
+    trim_cast_varchar,
     try_parse_json,
     try_to_decimal,
     upper_case_unquoted_identifiers,
     values_columns,
 )
 
 
@@ -442,14 +443,24 @@
             read="snowflake",
         )
         .transform(json_extract_cast_as_varchar)
         .sql(dialect="duckdb")
         == """SELECT JSON('{"fruit":"banana"}') ->> '$.fruit'"""
     )
 
+    assert (
+        sqlglot.parse_one(
+            """select parse_json('{"fruit":"9000"}'):fruit::number""",
+            read="snowflake",
+        )
+        .transform(json_extract_cast_as_varchar)
+        .sql(dialect="duckdb")
+        == """SELECT CAST(JSON('{"fruit":"9000"}') -> '$.fruit' AS DECIMAL)"""
+    )
+
 
 def test_json_extract_precedence() -> None:
     assert (
         sqlglot.parse_one(
             """select {'K1': {'K2': 1}} as col where col:K1:K2 > 0""",
             read="snowflake",
         )
@@ -766,14 +777,31 @@
         sqlglot.parse_one("""INSERT INTO table1 (name) SELECT TRY_PARSE_JSON('{"first":"foo", "last":"bar"}')""")
         .transform(try_parse_json)
         .sql(dialect="duckdb")
         == """INSERT INTO table1 (name) SELECT TRY_CAST('{"first":"foo", "last":"bar"}' AS JSON)"""
     )
 
 
+def test_trim_cast_varchar() -> None:
+    assert (
+        sqlglot.parse_one("SELECT TRIM(col) FROM table1").transform(trim_cast_varchar).sql(dialect="duckdb")
+        == "SELECT TRIM(CAST(col AS TEXT)) FROM table1"
+    )
+
+    assert (
+        sqlglot.parse_one("SELECT TRIM(col::varchar) FROM table1").transform(trim_cast_varchar).sql(dialect="duckdb")
+        == "SELECT TRIM(CAST(col AS TEXT)) FROM table1"
+    )
+
+    assert (
+        sqlglot.parse_one("SELECT TRIM(col::TEXT) FROM table1").transform(trim_cast_varchar).sql(dialect="duckdb")
+        == "SELECT TRIM(CAST(col AS TEXT)) FROM table1"
+    )
+
+
 def test_upper_case_unquoted_identifiers() -> None:
     assert (
         sqlglot.parse_one("select name, name as fname from table1").transform(upper_case_unquoted_identifiers).sql()
         == "SELECT NAME, NAME AS FNAME FROM TABLE1"
     )
```

### Comparing `fakesnow-0.9.7/tests/test_users.py` & `fakesnow-0.9.8/tests/test_users.py`

 * *Files identical despite different names*

