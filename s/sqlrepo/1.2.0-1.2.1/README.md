# Comparing `tmp/sqlrepo-1.2.0.tar.gz` & `tmp/sqlrepo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-1.2.0.tar", last modified: Thu Apr 18 13:55:37 2024, max compression
+gzip compressed data, was "sqlrepo-1.2.1.tar", last modified: Fri Apr 19 14:09:09 2024, max compression
```

## Comparing `sqlrepo-1.2.0.tar` & `sqlrepo-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     8166 2024-04-18 08:40:57.394211 sqlrepo-1.2.0/README.md
--rw-r--r--   0        0        0     3039 2024-04-18 13:55:37.619599 sqlrepo-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.2.0/sqlrepo/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.2.0/sqlrepo/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.2.0/sqlrepo/.pytest_cache/README.md
--rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.2.0/sqlrepo/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.2.0/sqlrepo/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.2.0/sqlrepo/__init__.py
--rw-r--r--   0        0        0      491 2024-04-15 09:17:35.411159 sqlrepo-1.2.0/sqlrepo/exc.py
--rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.2.0/sqlrepo/logging.py
--rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.2.0/sqlrepo/py.typed
--rw-r--r--   0        0        0    32700 2024-04-18 13:55:06.255867 sqlrepo-1.2.0/sqlrepo/queries.py
--rw-r--r--   0        0        0    22475 2024-04-18 13:46:54.885073 sqlrepo-1.2.0/sqlrepo/repositories.py
--rw-r--r--   0        0        0     3540 2024-04-16 08:43:46.475848 sqlrepo-1.2.0/sqlrepo/uow.py
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0    14674 2024-04-18 09:54:00.067553 sqlrepo-1.2.0/tests/test_async_queries.py
--rw-r--r--   0        0        0    17011 2024-04-18 08:27:43.006148 sqlrepo-1.2.0/tests/test_base_queries.py
--rw-r--r--   0        0        0     2825 2024-04-18 13:50:35.586184 sqlrepo-1.2.0/tests/test_base_repositories.py
--rw-r--r--   0        0        0    13875 2024-04-18 09:57:20.991582 sqlrepo-1.2.0/tests/test_sync_queries.py
--rw-r--r--   0        0        0        0 2024-04-05 11:56:33.229687 sqlrepo-1.2.0/tests/test_uow.py
--rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.2.0/tests/types.py
--rw-r--r--   0        0        0     7107 2024-04-15 06:16:49.991950 sqlrepo-1.2.0/tests/utils.py
--rw-r--r--   0        0        0     8519 1970-01-01 00:00:00.000000 sqlrepo-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-04-19 13:48:52.688101 sqlrepo-1.2.1/README.md
+-rw-r--r--   0        0        0     3039 2024-04-19 14:09:09.193136 sqlrepo-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/README.md
+-rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.2.1/sqlrepo/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.2.1/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-15 09:17:35.411159 sqlrepo-1.2.1/sqlrepo/exc.py
+-rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.2.1/sqlrepo/logging.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.2.1/sqlrepo/py.typed
+-rw-r--r--   0        0        0    32857 2024-04-19 14:00:18.076644 sqlrepo-1.2.1/sqlrepo/queries.py
+-rw-r--r--   0        0        0    22638 2024-04-19 13:36:14.622268 sqlrepo-1.2.1/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     3540 2024-04-16 08:43:46.475848 sqlrepo-1.2.1/sqlrepo/uow.py
+-rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.2.1/tests/test_async_queries.py
+-rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.2.1/tests/test_async_repositories.py
+-rw-r--r--   0        0        0    17011 2024-04-18 08:27:43.006148 sqlrepo-1.2.1/tests/test_base_queries.py
+-rw-r--r--   0        0        0     2825 2024-04-18 13:50:35.586184 sqlrepo-1.2.1/tests/test_base_repositories.py
+-rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.2.1/tests/test_sync_queries.py
+-rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.2.1/tests/test_sync_repositories.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:56:33.229687 sqlrepo-1.2.1/tests/test_uow.py
+-rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.2.1/tests/types.py
+-rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.2.1/tests/utils.py
+-rw-r--r--   0        0        0     9933 1970-01-01 00:00:00.000000 sqlrepo-1.2.1/PKG-INFO
```

### Comparing `sqlrepo-1.2.0/README.md` & `sqlrepo-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 # sqlrepo
 
 ![coverage](./coverage.svg)
 
 >SQLAlchemy repository pattern.
 
+## Current state
+
+Now, some features of repository pattern works incorrect or some parts of it is hard to understand
+or use. I want to simplify work with repositories, so this is TODO for my project:
+
+* [ ] Add more test cases for main functionality. Now, tested only base cases of repository
+    method use.
+* [ ] Add wrapper for all non sqlrepo exceptions. Now, some functionality could raise
+      "raw" SQLAlchemy error. I want to avoid the situation, when developer make
+      try-except with all possible exceptions, when works with my package.
+* [ ] Add more use-cases of `specific_column_mapping` option. Now it only works with
+      `search_by` and `order_by` params. I want to add it for filters, joins and other
+      parts, where it can be used.
+* [ ] Integrate sqlrepo with FastAPI or some other web-frameworks.
+* [ ] Add pydantic-like configuration. Current implementation works on ClassVar. I want to separate
+      configuration and main repository code.
+
+If all these todo items are finished, it means, that all, what I want, is implemented.
+If you want to give me advice or feedback, you are welcome.
+
 ## Install
 
 sqlrepo project doesn't has optional dependencies, so you can install it just as regular:
 
 With pip:
 
 ```bash
@@ -160,22 +180,28 @@
 
 Uses as choice of used defined disable field.
 
 By default, None. Needs to be set manually, because this option depends on user custom
 implementation of disable_field. If None and `disable` method was evaluated, there will be
 RepositoryAttributeError exception raised by Repository class.
 
+Now only works with string fields, because otherwise sqlalchemy think that Repository class is
+sqlalchemy model without mapping, and raise error.
+
 ### `disable_id_field`
 
 Uses as choice of used defined id field in model, which supports disable.
 
 By default, None. Needs to be set manually, because this option depends on user custom
 implementation of disable_field. If None and `disable` method was evaluated, there will be
 RepositoryAttributeError exception raised by Repository class.
 
+Now only works with string fields, because otherwise sqlalchemy think that Repository class is
+sqlalchemy model without mapping, and raise error.
+
 ### `unique_list_items`
 
 __Warning!__ Ambiguous option!
 
 Current version of `sqlrepo` works with load strategies with user configured option
 `load_strategy`. In order to make `list` method works stable, this option is used.
 If you don't work with relationships in your model or you don't need unique (for example,
```

### Comparing `sqlrepo-1.2.0/pyproject.toml` & `sqlrepo-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -172,24 +172,24 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "1.2.0"
+version = "1.2.1"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "sqlalchemy>=2.0.29",
-    "python-dev-utils[sqlalchemy_filters]>=1.3.0",
+    "python-dev-utils[sqlalchemy_filters]>=1.3.1",
 ]
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `sqlrepo-1.2.0/sqlrepo/logging.py` & `sqlrepo-1.2.1/sqlrepo/logging.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.0/sqlrepo/queries.py` & `sqlrepo-1.2.1/sqlrepo/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import re
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, Literal, NotRequired, TypedDict, TypeVar, overload
 
 from dev_utils.core.utils import get_utc_now
 from dev_utils.sqlalchemy.filters.converters import BaseFilterConverter
 from dev_utils.sqlalchemy.utils import apply_joins, apply_loads, get_sqlalchemy_attribute
-from sqlalchemy import CursorResult, and_, delete
+from sqlalchemy import CursorResult, and_, delete, func, insert, or_, select, text, update
 from sqlalchemy import exc as sqlalchemy_exc
-from sqlalchemy import func, insert, or_, select, text, update
 from sqlalchemy.orm import joinedload
 
 from sqlrepo.exc import QueryError
 from sqlrepo.logging import logger as default_logger
 
 
 class JoinKwargs(TypedDict):
@@ -51,26 +50,27 @@
     Join = str | Model | ModelWithOnclause | CompleteModel
     Filter = dict[str, Any] | Sequence[dict[str, Any] | ColumnElement[bool]] | ColumnElement[bool]
     Load = str | _AbstractLoad
     SearchParam = str | QueryableAttribute[Any]
     ColumnParam = str | QueryableAttribute[Any]
     OrderByParam = _ColumnExpressionOrStrLabelArgument[Any]
     DataDict = dict[str, Any]
+    StrField = str
 
 
 class BaseQuery:
     """Base query class.
 
     Implements base logic for queries like generating statements or filters. Don't use it directly.
     """
 
     def __init__(
         self,
         filter_converter_class: type[BaseFilterConverter],
-        specific_column_mapping: dict[str, "ColumnElement[Any]"] | None = None,
+        specific_column_mapping: dict[str, "InstrumentedAttribute[Any]"] | None = None,
         load_strategy: Callable[..., "_AbstractLoad"] = joinedload,
         logger: "Logger" = default_logger,
     ) -> None:
         self.specific_column_mapping = specific_column_mapping
         self.filter_converter_class = filter_converter_class
         self.load_strategy = load_strategy
         self.logger = logger
@@ -346,15 +346,15 @@
 class BaseSyncQuery(BaseQuery):
     """Base query class with sync interface."""
 
     def __init__(
         self,
         session: "Session",
         filter_converter_class: type[BaseFilterConverter],
-        specific_column_mapping: dict[str, "ColumnElement[Any]"] | None = None,
+        specific_column_mapping: dict[str, "InstrumentedAttribute[Any]"] | None = None,
         load_strategy: Callable[[Any], "_AbstractLoad"] = joinedload,
         logger: "Logger" = default_logger,
     ) -> None:
         self.session = session
         super().__init__(filter_converter_class, specific_column_mapping, load_strategy, logger)
 
     def get_item(
@@ -611,27 +611,27 @@
         return True
 
     def disable_items(
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         ids_to_disable: set[Any],
-        id_field: "InstrumentedAttribute[Any]",
-        disable_field: "InstrumentedAttribute[Any]",
+        id_field: "StrField",
+        disable_field: "StrField",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
         extra_filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Count":
         """Disable model instances with given ids and extra_filters."""
         stmt = self._disable_items_stmt(
             model=model,
             ids_to_disable=ids_to_disable,
-            id_field=id_field,
-            disable_field=disable_field,
+            id_field=get_sqlalchemy_attribute(model, id_field, only_columns=True),
+            disable_field=get_sqlalchemy_attribute(model, disable_field, only_columns=True),
             field_type=field_type,
             allow_filter_by_value=allow_filter_by_value,
             extra_filters=extra_filters,
         )
         if isinstance(stmt, int):  # pragma: no coverage
             return stmt
         result = self.session.execute(stmt)
@@ -647,15 +647,15 @@
 class BaseAsyncQuery(BaseQuery):
     """Base query class with async interface."""
 
     def __init__(
         self,
         session: "AsyncSession",
         filter_converter_class: type[BaseFilterConverter],
-        specific_column_mapping: dict[str, "ColumnElement[Any]"] | None = None,
+        specific_column_mapping: dict[str, "InstrumentedAttribute[Any]"] | None = None,
         load_strategy: Callable[..., "_AbstractLoad"] = joinedload,
         logger: "Logger" = default_logger,
     ) -> None:
         self.session = session
         super().__init__(filter_converter_class, specific_column_mapping, load_strategy, logger)
 
     async def get_item(
@@ -912,27 +912,27 @@
         return True
 
     async def disable_items(
         self,
         *,
         model: type["BaseSQLAlchemyModel"],
         ids_to_disable: set[Any],
-        id_field: "InstrumentedAttribute[Any]",
-        disable_field: "InstrumentedAttribute[Any]",
+        id_field: "StrField",
+        disable_field: "StrField",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
         extra_filters: "Filter | None" = None,
         use_flush: bool = False,
     ) -> "Count":
         """Disable model instances with given ids and extra_filters."""
         stmt = self._disable_items_stmt(
             model=model,
             ids_to_disable=ids_to_disable,
-            id_field=id_field,
-            disable_field=disable_field,
+            id_field=get_sqlalchemy_attribute(model, id_field, only_columns=True),
+            disable_field=get_sqlalchemy_attribute(model, disable_field, only_columns=True),
             field_type=field_type,
             allow_filter_by_value=allow_filter_by_value,
             extra_filters=extra_filters,
         )
         if isinstance(stmt, int):  # pragma: no coverage
             return stmt
         result = await self.session.execute(stmt)
```

### Comparing `sqlrepo-1.2.0/sqlrepo/repositories.py` & `sqlrepo-1.2.1/sqlrepo/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Any,
     ClassVar,
     Final,
     ForwardRef,
     Generic,
     Literal,
     NotRequired,
+    TypeAlias,
     TypedDict,
     TypeVar,
     get_args,
     overload,
 )
 
 from dev_utils.sqlalchemy.filters.converters import (
@@ -60,16 +61,17 @@
     Filter = dict[str, Any] | Sequence[dict[str, Any] | ColumnElement[bool]] | ColumnElement[bool]
     Load = str | _AbstractLoad
     SearchParam = str | QueryableAttribute[Any]
     OrderByParam = _ColumnExpressionOrStrLabelArgument[Any]
     DataDict = dict[str, Any]
 
 
-StrField = str
+StrField: TypeAlias = str
 BaseSQLAlchemyModel = TypeVar("BaseSQLAlchemyModel", bound=Base)
+IsUpdated: TypeAlias = bool
 
 
 class RepositoryModelClassIncorrectUseWarning(Warning):
     """Warning about Repository model_class attribute incorrect usage."""
 
 
 class BaseRepository(Generic[BaseSQLAlchemyModel]):
@@ -103,15 +105,15 @@
 
     # So, when you will use AdminRepository, model_class attribute will be set with Admin
     # automatically.
     ```
     """
 
     # TODO: add specific_column_mapping to filters, joins and loads.
-    specific_column_mapping: ClassVar["dict[str, ColumnElement[Any]]"] = {}
+    specific_column_mapping: ClassVar["dict[str, InstrumentedAttribute[Any]]"] = {}
     """
     Warning! Current version of sqlrepo doesn't support this mapping for filters, joins and loads.
 
     Uses as mapping for some attributes, that you need to alias or need to specify column
     from other models.
 
     Warning: if you specify column from other model, it may cause errors. For example, update
@@ -164,23 +166,23 @@
     """
     Uses as choice of type of disable field.
 
     By default, None. Needs to be set manually, because this option depends on user custom
     implementation of disable_field. If None and ``disable`` method was evaluated, there will be
     RepositoryAttributeError exception raised by Repository class.
     """
-    disable_field: ClassVar["InstrumentedAttribute[Any] | None"] = None
+    disable_field: ClassVar["StrField | None"] = None
     """
     Uses as choice of used defined disable field.
 
     By default, None. Needs to be set manually, because this option depends on user custom
     implementation of disable_field. If None and ``disable`` method was evaluated, there will be
     RepositoryAttributeError exception raised by Repository class.
     """
-    disable_id_field: ClassVar["InstrumentedAttribute[Any] | None"] = None
+    disable_id_field: ClassVar["StrField | None"] = None
     """
     Uses as choice of used defined id field in model, which supports disable.
 
     By default, None. Needs to be set manually, because this option depends on user custom
     implementation of disable_field. If None and ``disable`` method was evaluated, there will be
     RepositoryAttributeError exception raised by Repository class.
     """
@@ -325,14 +327,15 @@
         self.session = session
         self.logger = logger
         self.queries = self.query_class(
             session,
             self.get_filter_convert_class(),
             self.specific_column_mapping,
             self.load_strategy,
+            logger,
         )
 
     async def get(
         self,
         filters: "Filter",
         *,
         joins: "Sequence[Join] | None" = None,
@@ -430,15 +433,15 @@
         return result
 
     async def update_instance(
         self,
         *,
         instance: "BaseSQLAlchemyModel",
         data: "DataDict",
-    ) -> "tuple[bool, BaseSQLAlchemyModel]":
+    ) -> "tuple[IsUpdated, BaseSQLAlchemyModel]":
         """Update model_class instance from given data.
 
         Returns tuple with boolean (was instance updated or not) and updated instance.
         """
         result = await self.queries.change_item(
             data=data,
             item=instance,
@@ -491,21 +494,23 @@
 
     __inheritance_check_model_class__ = False
     query_class: type["BaseSyncQuery"] = BaseSyncQuery
 
     def __init__(
         self,
         session: "Session",
+        logger: "Logger" = default_logger,
     ) -> None:
         self.session = session
         self.queries = self.query_class(
             session,
             self.get_filter_convert_class(),
             self.specific_column_mapping,
             self.load_strategy,
+            logger,
         )
 
     def get(
         self,
         *,
         filters: "Filter",
         joins: "Sequence[Join] | None" = None,
@@ -519,16 +524,16 @@
             filters=filters,
         )
         return result
 
     def count(
         self,
         *,
-        joins: "Sequence[Join] | None" = None,
         filters: "Filter | None" = None,
+        joins: "Sequence[Join] | None" = None,
     ) -> int:
         """Get count of instances of model_class by given filters."""
         result = self.queries.get_items_count(
             model=self.model_class,
             joins=joins,
             filters=filters,
         )
@@ -603,15 +608,15 @@
         return result
 
     def update_instance(
         self,
         *,
         instance: "BaseSQLAlchemyModel",
         data: "DataDict",
-    ) -> "tuple[bool, BaseSQLAlchemyModel]":
+    ) -> "tuple[IsUpdated, BaseSQLAlchemyModel]":
         """Update model_class instance from given data.
 
         Returns tuple with boolean (was instance updated or not) and updated instance.
         """
         result = self.queries.change_item(
             data=data,
             item=instance,
@@ -637,14 +642,15 @@
     def disable(
         self,
         *,
         ids_to_disable: set[Any],
         extra_filters: "Filter | None" = None,
     ) -> "Count":
         """Disable model_class instances with given ids and extra_filters."""
+        self._validate_disable_attributes()
         result = self.queries.disable_items(
             model=self.model_class,
             ids_to_disable=ids_to_disable,
             id_field=self.disable_id_field,  # type: ignore
             disable_field=self.disable_field,  # type: ignore
             field_type=self.disable_field_type,  # type: ignore
             allow_filter_by_value=self.allow_disable_filter_by_value,
```

### Comparing `sqlrepo-1.2.0/sqlrepo/uow.py` & `sqlrepo-1.2.1/sqlrepo/uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.0/tests/conftest.py` & `sqlrepo-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.0/tests/test_async_queries.py` & `sqlrepo-1.2.1/tests/test_async_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,16 +428,16 @@
     mymodel_async_factory: "AsyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     item = await mymodel_async_factory(db_async_session, bl=False)
     query_obj = BaseAsyncQuery(db_async_session, SimpleFilterConverter)
     disable_count = await query_obj.disable_items(
         model=MyModel,
         ids_to_disable={item.id},
-        id_field=MyModel.id,
-        disable_field=MyModel.bl,
+        id_field="id",
+        disable_field="bl",
         field_type=bool,
         allow_filter_by_value=False,
         extra_filters={"id": item.id},
         use_flush=use_flush,
     )
     assert disable_count == 1
     assert (
```

### Comparing `sqlrepo-1.2.0/tests/test_base_queries.py` & `sqlrepo-1.2.1/tests/test_base_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.0/tests/test_base_repositories.py` & `sqlrepo-1.2.1/tests/test_base_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.0/tests/test_sync_queries.py` & `sqlrepo-1.2.1/tests/test_sync_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,16 +414,16 @@
     mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     item = mymodel_sync_factory(db_sync_session, bl=False)
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     disable_count = query_obj.disable_items(
         model=MyModel,
         ids_to_disable={item.id},
-        id_field=MyModel.id,
-        disable_field=MyModel.bl,
+        id_field="id",
+        disable_field="bl",
         field_type=bool,
         allow_filter_by_value=False,
         extra_filters={"id": item.id},
         use_flush=use_flush,
     )
     assert disable_count == 1
     assert (
```

### Comparing `sqlrepo-1.2.0/tests/types.py` & `sqlrepo-1.2.1/tests/types.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.2.0/tests/utils.py` & `sqlrepo-1.2.1/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import random
-from typing import TYPE_CHECKING, Any, Sequence, TypeVar
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Any, TypeVar
 
 from sqlalchemy import ForeignKey, inspect
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.hybrid import hybrid_method, hybrid_property
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
@@ -70,14 +71,15 @@
     items2: Sequence["DeclarativeBase"],
 ) -> None:
     """Assert if 2 model lists not compare to each other."""
     assert len(items1) == len(items2), f"Different lists count: {len(items1)} != {len(items2)}"
     for item1, item2 in zip(
         sorted(items1, key=lambda x: x.id),  # type: ignore
         sorted(items2, key=lambda x: x.id),  # type: ignore
+        strict=True,
     ):
         assert_compare_db_items(item1, item2)
 
 
 def assert_compare_db_item_with_dict(
     item: "DeclarativeBase",
     data: dict[str, Any],
```

### Comparing `sqlrepo-1.2.0/PKG-INFO` & `sqlrepo-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 Metadata-Version: 2.1
 Name: sqlrepo
-Version: 1.2.0
+Version: 1.2.1
 Summary: sqlalchemy repositories with crud operations and other utils for it.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: sqlalchemy>=2.0.29
-Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.3.0
+Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.3.1
 Description-Content-Type: text/markdown
 
 # sqlrepo
 
 ![coverage](./coverage.svg)
 
 >SQLAlchemy repository pattern.
 
+## Current state
+
+Now, some features of repository pattern works incorrect or some parts of it is hard to understand
+or use. I want to simplify work with repositories, so this is TODO for my project:
+
+* [ ] Add more test cases for main functionality. Now, tested only base cases of repository
+    method use.
+* [ ] Add wrapper for all non sqlrepo exceptions. Now, some functionality could raise
+      "raw" SQLAlchemy error. I want to avoid the situation, when developer make
+      try-except with all possible exceptions, when works with my package.
+* [ ] Add more use-cases of `specific_column_mapping` option. Now it only works with
+      `search_by` and `order_by` params. I want to add it for filters, joins and other
+      parts, where it can be used.
+* [ ] Integrate sqlrepo with FastAPI or some other web-frameworks.
+* [ ] Add pydantic-like configuration. Current implementation works on ClassVar. I want to separate
+      configuration and main repository code.
+
+If all these todo items are finished, it means, that all, what I want, is implemented.
+If you want to give me advice or feedback, you are welcome.
+
 ## Install
 
 sqlrepo project doesn't has optional dependencies, so you can install it just as regular:
 
 With pip:
 
 ```bash
@@ -171,22 +191,28 @@
 
 Uses as choice of used defined disable field.
 
 By default, None. Needs to be set manually, because this option depends on user custom
 implementation of disable_field. If None and `disable` method was evaluated, there will be
 RepositoryAttributeError exception raised by Repository class.
 
+Now only works with string fields, because otherwise sqlalchemy think that Repository class is
+sqlalchemy model without mapping, and raise error.
+
 ### `disable_id_field`
 
 Uses as choice of used defined id field in model, which supports disable.
 
 By default, None. Needs to be set manually, because this option depends on user custom
 implementation of disable_field. If None and `disable` method was evaluated, there will be
 RepositoryAttributeError exception raised by Repository class.
 
+Now only works with string fields, because otherwise sqlalchemy think that Repository class is
+sqlalchemy model without mapping, and raise error.
+
 ### `unique_list_items`
 
 __Warning!__ Ambiguous option!
 
 Current version of `sqlrepo` works with load strategies with user configured option
 `load_strategy`. In order to make `list` method works stable, this option is used.
 If you don't work with relationships in your model or you don't need unique (for example,
```

