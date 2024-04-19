# Comparing `tmp/hilcat-1.0.6.tar.gz` & `tmp/hilcat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilcat-1.0.6.tar", last modified: Mon Nov 20 04:54:29 2023, max compression
+gzip compressed data, was "hilcat-1.1.0.tar", last modified: Fri Apr 19 02:16:15 2024, max compression
```

## Comparing `hilcat-1.0.6.tar` & `hilcat-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 04:54:29.642695 hilcat-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-20 04:54:29.642695 hilcat-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-20 04:54:18.000000 hilcat-1.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 04:54:29.638695 hilcat-1.0.6/hilcat/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-20 04:54:29.000000 hilcat-1.0.6/hilcat/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 04:54:29.642695 hilcat-1.0.6/hilcat/db/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/db/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/db/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    23487 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/db/relational.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/db/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-11-20 04:54:18.000000 hilcat-1.0.6/hilcat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 04:54:29.642695 hilcat-1.0.6/hilcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-20 04:54:29.000000 hilcat-1.0.6/hilcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-11-20 04:54:29.000000 hilcat-1.0.6/hilcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 04:54:29.000000 hilcat-1.0.6/hilcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-11-20 04:54:18.000000 hilcat-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 04:54:29.642695 hilcat-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.053067 hilcat-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-19 02:16:15.053067 hilcat-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-19 02:16:09.000000 hilcat-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.049067 hilcat-1.1.0/hilcat/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 02:16:14.000000 hilcat-1.1.0/hilcat/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.053067 hilcat-1.1.0/hilcat/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/relational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/db/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 02:16:09.000000 hilcat-1.1.0/hilcat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:16:15.053067 hilcat-1.1.0/hilcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-19 02:16:15.000000 hilcat-1.1.0/hilcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 02:16:15.000000 hilcat-1.1.0/hilcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:16:15.000000 hilcat-1.1.0/hilcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-19 02:16:09.000000 hilcat-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:16:15.053067 hilcat-1.1.0/setup.cfg
```

### Comparing `hilcat-1.0.6/hilcat/db/__init__.py` & `hilcat-1.1.0/hilcat/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.0.6/hilcat/db/mysql.py` & `hilcat-1.1.0/hilcat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.0.6/hilcat/db/postgresql.py` & `hilcat-1.1.0/hilcat/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.0.6/hilcat/db/relational.py` & `hilcat-1.1.0/hilcat/db/relational.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,49 +3,138 @@
 """
 Relational database can be used as a cache or a persistence storage.
 Actually, implement a cache is enough.
 """
 
 from typing import (
     Any, Iterable, Dict,
-    Optional, List,
+    List, Type,
     Sequence, Callable,
     Literal, Union,
-    Tuple, Hashable
+    Tuple, Hashable,
 )
 from abc import ABC, abstractmethod
 from types import ModuleType
 import dataclasses
 from ..core import Cache
 
 _FETCH_SIZE_TYPE = Union[Literal['one', 'all'], int]
 _EXECUTE_PARAM_TYPE = Union[Sequence[Any], Dict[str, Any]]
 _KEY_TYPE = Union[str, int]
 
+class ValueAdapter(ABC):
+    """
+    Method `build_column_values` and `parse_column_values` should be reversed one-to-one mapping.
+    That is to say:
+        parse_column_values(build_column_values(x)) == x
+        build_column_values(parse_column_values(x)) == x
+    """
+    @abstractmethod
+    def build_column_values(self, value: Any) -> Dict[str, Any]:
+        """
+        Used in method `RelationalDbCache.set()` to build column values
+        """
+    @abstractmethod
+    def parse_column_values(self, value: Dict[str, Any]) -> Any:
+        """
+        Used in method `RelationalDbCache.fetch()` to parse column values.
+        """
+
+class DefaultAdapter(ValueAdapter):
+    """
+    Cache value should be exactly column values and thus nothing should do.
+    """
+
+    def build_column_values(self, value: Dict[str, Any]) -> Dict[str, Any]:
+        return value
+
+    def parse_column_values(self, value: Dict[str, Any]) -> Dict[str, Any]:
+        return value
+
+class SingleAdapter(ValueAdapter):
+    """
+    Cache value is exactly one column.
+    """
+
+    def __init__(self, col: str):
+        self.col = col
+
+    def build_column_values(self, value: Any) -> Dict[str, Any]:
+        return {self.col: value}
+
+    def parse_column_values(self, value: Dict[str, Any]) -> Any:
+        return value[self.col]
+
+class SequenceAdapter(ValueAdapter):
+    """
+    Cache value is a list or tuple, corresponding to some columns.
+    """
+
+    def __init__(self, cols: Sequence[str], return_type: Type[Union[list, tuple]] = tuple):
+        self.cols = cols
+        self.return_type = return_type
+
+    def build_column_values(self, value: Sequence[Any]) -> Dict[str, Any]:
+        return dict(zip(self.cols, value))
+
+    def parse_column_values(self, value: Dict[str, Any]) -> Sequence[Any]:
+        return self.return_type(map(value.get, self.cols))
+
 @dataclasses.dataclass
 class RelationalDbScopeConfig:
     scope: Hashable
     table: str = None
     uniq_column: str = 'id'     # unique column to identify rows
-    columns: Sequence[str] = ('id', 'data')
+    columns: Sequence[str] = ('data', )
     columns_with_id: List[str] = dataclasses.field(init=False)
 
     # if column not specified here, type should be str
     column_types: Dict[str, str] = dataclasses.field(default_factory=dict)
 
+    # convert value when fetch and set
+    value_adapter: Union[Literal['auto', 'default', 'single', 'tuple', 'list'], ValueAdapter] = 'auto'
+
+    def _check_value_adapter(self, adapter) -> ValueAdapter:
+        if adapter == 'auto':
+            if len(self.columns) == 1:
+                return SingleAdapter(self.columns[0])
+            return DefaultAdapter()
+        elif adapter == 'default':
+            return DefaultAdapter()
+        elif adapter == 'single':
+            if len(self.columns) != 1:
+                raise ValueError(f"columns length should be 1 when value_adapter is 'single'.")
+            return SingleAdapter(self.columns[0])
+        elif adapter == 'tuple':
+            return SequenceAdapter(self.columns, return_type=tuple)
+        elif adapter == 'list':
+            return SequenceAdapter(self.columns, return_type=list)
+
+        if isinstance(adapter, ValueAdapter):
+            return adapter
+
+        if isinstance(adapter, str):
+            msg = f"Unexpected value_adapter: {adapter}"
+        else:
+            msg = f"Unexpected value_adapter type: {type(adapter)}"
+        raise ValueError(msg)
+
     def __post_init__(self):
         if self.uniq_column in self.columns:
             self.columns_with_id = list(self.columns)
         else:
             self.columns_with_id = [self.uniq_column] + list(self.columns)
+
         if not self.table:
             if not isinstance(self.scope, str):
                 raise ValueError("Arg scope must be a str when table not given.")
             self.table = self.scope
 
+        self.value_adapter = self._check_value_adapter(self.value_adapter)
+
     def get_column_type(self, col: str) -> str:
         # this method should be overwritten for certain database
         return self.column_types.get(col, 'text')
 
 @dataclasses.dataclass
 class Operation:
     """
@@ -174,15 +263,16 @@
                 return [variable_values[x] for x in variable_names]
             return list(variable_values.values())
         return variable_values
 
     def build_select_operation(self, config: RelationalDbScopeConfig, key: _KEY_TYPE = None, limit: int = -1,
                                select_columns: Sequence[str] = None) -> Operation:
         if select_columns is None:
-            select_columns = config.columns_with_id
+            # only select configured columns; if id not configured, ignore it
+            select_columns = config.columns
         elif isinstance(select_columns, str):
             select_columns = [select_columns]
         stmt = f"SELECT {','.join(select_columns)} FROM {config.table}"
         variable_values = {}
         if key is not None:
             name = config.uniq_column
             placeholder = self.config_variable(name=name, order=1, value=key, variable_mapping=variable_values)
@@ -501,29 +591,37 @@
     def _check_key(self, key: _KEY_TYPE):
         if key is None:
             raise ValueError("Arg key should not be None.")
 
     def exists(self, key: _KEY_TYPE, scope: str = None, **kwargs) -> bool:
         self._check_key(key)
         config = self._get_scope_config(scope)
-        operation = self.sql_builder.build_select_operation(config=config, key=key, limit=1)
+        operation = self.sql_builder.build_select_operation(
+            config=config, key=key, limit=1,
+            select_columns=[config.uniq_column],
+        )
         return self._execute(operation, fetch_size=1) is not None
 
-    def fetch(self, key: _KEY_TYPE, default: Any = None, scope: Any = None, **kwargs) -> Optional[Dict[str, Any]]:
+    def fetch(self, key: _KEY_TYPE, default: Any = None, scope: Any = None, **kwargs) -> Any:
         self._check_key(key)
         config = self._get_scope_config(scope)
-        operation = self.sql_builder.build_select_operation(config=config, key=key, limit=1)
+        operation = self.sql_builder.build_select_operation(
+            config=config, key=key, limit=1,
+            select_columns=config.columns,
+        )
         row = self._execute(operation, fetch_size=1)
         if row is None:
             return default
-        return dict(zip(config.columns, row))
+        value = dict(zip(config.columns, row))
+        return config.value_adapter.parse_column_values(value)
 
-    def set(self, key: _KEY_TYPE, value: Dict[str, Any], scope: Any = None, **kwargs) -> bool:
+    def set(self, key: _KEY_TYPE, value: Any, scope: Any = None, **kwargs) -> bool:
         self._check_key(key)
         config = self._get_scope_config(scope)
+        value = config.value_adapter.build_column_values(value)
         if config.uniq_column in value:
             if key != value[config.uniq_column]:
                 raise ValueError(f"key {key} is different from value {value[config.uniq_column]}")
             row = {name: value[name] for name in config.columns_with_id if name in value}
         else:
             row = {config.uniq_column: key}
             row.update((name, value[name]) for name in config.columns if name in value)
```

### Comparing `hilcat-1.0.6/hilcat/db/sqlite.py` & `hilcat-1.1.0/hilcat/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.0.6/hilcat/es.py` & `hilcat-1.1.0/hilcat/es.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.0.6/hilcat/redis.py` & `hilcat-1.1.0/hilcat/redis.py`

 * *Files identical despite different names*

### Comparing `hilcat-1.0.6/pyproject.toml` & `hilcat-1.1.0/pyproject.toml`

 * *Files identical despite different names*

