# Comparing `tmp/neptune_fetcher-0.1.0.tar.gz` & `tmp/neptune_fetcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_fetcher-0.1.0.tar", max compression
+gzip compressed data, was "neptune_fetcher-0.2.0.tar", max compression
```

## Comparing `neptune_fetcher-0.1.0.tar` & `neptune_fetcher-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      266 2024-04-11 15:47:41.324642 neptune_fetcher-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-11 15:47:41.324642 neptune_fetcher-0.1.0/LICENSE
--rw-r--r--   0        0        0     8944 2024-04-11 15:47:41.324642 neptune_fetcher-0.1.0/README.md
--rw-r--r--   0        0        0     2352 2024-04-11 15:47:51.224648 neptune_fetcher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      739 2024-04-11 15:47:41.328642 neptune_fetcher-0.1.0/src/neptune_fetcher/__init__.py
--rw-r--r--   0        0        0     5149 2024-04-11 15:47:41.328642 neptune_fetcher-0.1.0/src/neptune_fetcher/fetchable.py
--rw-r--r--   0        0        0     4223 2024-04-11 15:47:41.328642 neptune_fetcher-0.1.0/src/neptune_fetcher/fields.py
--rw-r--r--   0        0        0     8471 2024-04-11 15:47:41.328642 neptune_fetcher-0.1.0/src/neptune_fetcher/read_only_project.py
--rw-r--r--   0        0        0     3267 2024-04-11 15:47:41.328642 neptune_fetcher-0.1.0/src/neptune_fetcher/read_only_run.py
--rw-r--r--   0        0        0    10564 1970-01-01 00:00:00.000000 neptune_fetcher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      678 2024-04-19 12:25:59.982524 neptune_fetcher-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-19 12:25:59.982524 neptune_fetcher-0.2.0/LICENSE
+-rw-r--r--   0        0        0    10266 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/README.md
+-rw-r--r--   0        0        0     2352 2024-04-19 12:26:12.678558 neptune_fetcher-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      739 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/__init__.py
+-rw-r--r--   0        0        0     1597 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/cache.py
+-rw-r--r--   0        0        0     5219 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/fetchable.py
+-rw-r--r--   0        0        0     3990 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/fields.py
+-rw-r--r--   0        0        0     8471 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_project.py
+-rw-r--r--   0        0        0     3054 2024-04-19 12:25:59.986524 neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_run.py
+-rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 neptune_fetcher-0.2.0/PKG-INFO
```

### Comparing `neptune_fetcher-0.1.0/LICENSE` & `neptune_fetcher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.1.0/README.md` & `neptune_fetcher-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -289,10 +289,83 @@
 ```
 
 __Returns__:
 `str`
 
 ---
 
+### Datetime
+#### `fetch()`
+Retrieves value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+created_at = run["sys/creation_time"].fetch()
+```
+
+__Returns__:
+`datetime.datetime`
+
+---
+
+### Object state
+#### `fetch()`
+Retrieves value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+state = run["sys/state"].fetch()
+```
+
+__Returns__:
+`str`
+
+---
+
+### Boolean
+#### `fetch()`
+Retrieves value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+status = run["sys/failed"].fetch()
+```
+
+__Returns__:
+`bool`
+
+---
+
+### Float series
+#### `fetch()` or `fetch_last()`
+Retrieves last series value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+loss = run["loss"].fetch_last()
+```
+
+__Returns__:
+`Optional[float]`
+
+#### `fetch_values()`
+Retrieves all series values from the API.
+
+__Parameters__:
+
+| Name | Type   | Default | Description                |
+| ---- |--------|---------|----------------------------|
+| `include_timestamp` | `bool` | True    | Whether the fetched data should include the timestamp field. |
+
+__Example__:
+```python
+values = run["loss"].fetch_values()
+```
+
+__Returns__:
+`pandas.DataFrame`
+
+---
+
 ## License
 
 This project is licensed under the Apache License Version 2.0. For more details, see [Apache License Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
```

### Comparing `neptune_fetcher-0.1.0/pyproject.toml` & `neptune_fetcher-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 style = "semver"
 pattern = "default-unprefixed"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # Base neptune package
-neptune = "2.0.0a1"
+neptune = "2.0.0a2"
 
 # Optional for default progress update handling
 tqdm = { version = ">=4.66.0", optional = true }
 
 
 [tool.poetry]
 authors = ["neptune.ai <contact@neptune.ai>"]
@@ -24,15 +24,15 @@
 repository = "https://github.com/neptune-ai/neptune-fetcher"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-fetcher"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_fetcher-0.1.0/src/neptune_fetcher/__init__.py` & `neptune_fetcher-0.2.0/src/neptune_fetcher/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.1.0/src/neptune_fetcher/fetchable.py` & `neptune_fetcher-0.2.0/src/neptune_fetcher/fetchable.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 __all__ = [
     "which_fetchable",
     "Fetchable",
     "FetchableAtom",
     "FetchableSeries",
     "SUPPORTED_TYPES",
     "FieldToFetchableVisitor",
@@ -25,15 +27,14 @@
 from abc import (
     ABC,
     abstractmethod,
 )
 from typing import (
     TYPE_CHECKING,
     Any,
-    Dict,
     Union,
 )
 
 from neptune.api.models import (
     ArtifactField,
     BoolField,
     DateTimeField,
@@ -51,136 +52,145 @@
     ObjectStateField,
     StringField,
     StringSeriesField,
     StringSetField,
 )
 from neptune.internal.container_type import ContainerType
 from neptune.internal.utils.logger import get_logger
-from neptune.internal.warnings import NeptuneUnsupportedType
 
 from neptune_fetcher.fields import (
+    Bool,
+    DateTime,
     Field,
     Float,
+    FloatSeries,
     Integer,
+    ObjectState,
     Series,
     String,
+    StringSet,
 )
 
 if TYPE_CHECKING:
     from neptune.internal.backends.hosted_neptune_backend import HostedNeptuneBackend
     from pandas import DataFrame
 
+    from neptune_fetcher.cache import FieldsCache
+
 
 logger = get_logger()
 
 
 SUPPORTED_ATOMS = {
     FieldType.INT,
     FieldType.FLOAT,
     FieldType.STRING,
+    FieldType.BOOL,
+    FieldType.DATETIME,
+    FieldType.STRING_SET,
+    FieldType.OBJECT_STATE,
+}
+SUPPORTED_SERIES_TYPES = {
+    FieldType.FLOAT_SERIES,
 }
-SUPPORTED_SERIES_TYPES = set()
 SUPPORTED_TYPES = {*SUPPORTED_ATOMS, *SUPPORTED_SERIES_TYPES}
 
 
 class Fetchable(ABC):
     def __init__(
         self,
         field: FieldDefinition,
         backend: "HostedNeptuneBackend",
         container_id: str,
-        cache: Dict[str, Union[Field, Series]],
+        cache: FieldsCache,
     ) -> None:
         self._field = field
         self._backend = backend
         self._container_id = container_id
-        self._cache = cache
+        self._cache: FieldsCache = cache
 
     @abstractmethod
     def fetch(self):
         ...
 
 
 class NoopFetchable(Fetchable):
     def fetch(self) -> None:
         logger.info("Unsupported type: %s", self._field.type)
         return None
 
 
 class FetchableAtom(Fetchable):
     def fetch(self):
-        if self._field.path in self._cache:
-            return self._cache[self._field.path].val
-        if self._field.type == FieldType.STRING:
-            attr = String(self._field.type)
-        elif self._field.type == FieldType.INT:
-            attr = Integer(self._field.type)
-        elif self._field.type == FieldType.FLOAT:
-            attr = Float(self._field.type)
-        else:
-            raise NeptuneUnsupportedType()
-        attr.val = attr.fetch(self._backend, self._container_id, ContainerType.RUN, [self._field.path])
-        self._cache[self._field.path] = attr
-        return attr.val
+        return self._cache[self._field.path].val
 
 
 class FetchableSeries(Fetchable):
     def fetch(self):
-        raise NeptuneUnsupportedType()
+        return self._cache[self._field.path].last
+
+    def fetch_last(self):
+        return self.fetch()
 
     def fetch_values(self, *, include_timestamp: bool = True) -> "DataFrame":
-        raise NeptuneUnsupportedType()
+        return self._cache[self._field.path].fetch_values(
+            backend=self._backend,
+            container_id=self._container_id,
+            container_type=ContainerType.RUN,
+            path=self._field.path,
+            include_timestamp=include_timestamp,
+        )
 
 
 def which_fetchable(field: FieldDefinition, *args: Any, **kwargs: Any) -> Fetchable:
     if field.type in SUPPORTED_ATOMS:
         return FetchableAtom(field, *args, **kwargs)
     elif field.type in SUPPORTED_SERIES_TYPES:
         return FetchableSeries(field, *args, **kwargs)
     return NoopFetchable(field, *args, **kwargs)
 
 
-class FieldToFetchableVisitor(FieldVisitor[Field]):
+class FieldToFetchableVisitor(FieldVisitor[Union[Field, Series]]):
     def visit_float(self, field: FloatField) -> Field:
         return Float(field.type, val=field.value)
 
     def visit_int(self, field: IntField) -> Field:
         return Integer(field.type, val=field.value)
 
     def visit_bool(self, field: BoolField) -> Field:
-        raise NotImplementedError
+        return Bool(field.type, val=field.value)
 
     def visit_string(self, field: StringField) -> Field:
         return String(field.type, val=field.value)
 
     def visit_datetime(self, field: DateTimeField) -> Field:
-        raise NotImplementedError
+        return DateTime(field.type, val=field.value)
 
     def visit_file(self, field: FileField) -> Field:
         raise NotImplementedError
 
     def visit_file_set(self, field: FileSetField) -> Field:
         raise NotImplementedError
 
-    def visit_float_series(self, field: FloatSeriesField) -> Field:
-        raise NotImplementedError
+    def visit_float_series(self, field: FloatSeriesField) -> Series:
+        return FloatSeries(field.type, last=field.last)
 
     def visit_string_series(self, field: StringSeriesField) -> Field:
         raise NotImplementedError
 
     def visit_image_series(self, field: ImageSeriesField) -> Field:
         raise NotImplementedError
 
     def visit_string_set(self, field: StringSetField) -> Field:
-        raise NotImplementedError
+        return StringSet(field.type, val=field.values)
 
     def visit_git_ref(self, field: GitRefField) -> Field:
         raise NotImplementedError
 
     def visit_object_state(self, field: ObjectStateField) -> Field:
-        raise NotImplementedError
+        return ObjectState(field.type, val=field.value)
 
     def visit_notebook_ref(self, field: NotebookRefField) -> Field:
         raise NotImplementedError
 
     def visit_artifact(self, field: ArtifactField) -> Field:
         raise NotImplementedError
```

### Comparing `neptune_fetcher-0.1.0/src/neptune_fetcher/read_only_project.py` & `neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_project.py`

 * *Files identical despite different names*

### Comparing `neptune_fetcher-0.1.0/src/neptune_fetcher/read_only_run.py` & `neptune_fetcher-0.2.0/src/neptune_fetcher/read_only_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 )
 
 from neptune.internal.container_type import ContainerType
 from neptune.internal.id_formats import QualifiedName
 from neptune.internal.utils import verify_type
 from neptune.table import TableEntry
 
+from neptune_fetcher.cache import FieldsCache
 from neptune_fetcher.fetchable import (
     SUPPORTED_TYPES,
     Fetchable,
     FetchableSeries,
-    FieldToFetchableVisitor,
     which_fetchable,
 )
 
 if TYPE_CHECKING:
     from neptune_fetcher.read_only_project import ReadOnlyProject
 
 
@@ -50,20 +50,23 @@
         return None
 
 
 class ReadOnlyRun:
     def __init__(self, read_only_project: "ReadOnlyProject", with_id: str) -> None:
         self.project = read_only_project
         self.with_id = with_id
-        self._field_to_fetchable_visitor = FieldToFetchableVisitor()
 
         verify_type("with_id", with_id, str)
 
         self._container_id = QualifiedName(f"{self.project.project_identifier}/{with_id}")
-        self._cache = dict()
+        self._cache = FieldsCache(
+            backend=self.project._backend,
+            container_id=self._container_id,
+            container_type=ContainerType.RUN,
+        )
         self._structure = {
             field_definition.path: which_fetchable(
                 field_definition,
                 self.project._backend,
                 self._container_id,
                 self._cache,
             )
@@ -91,15 +94,8 @@
 
     def prefetch(self, paths: List[str]) -> None:
         """Prefetches values of a list of fields and stores them in local cache.
 
         Args:
             paths: List of field paths to prefetch.
         """
-        data = self.project._backend.get_fields_with_paths_filter(
-            container_id=self._container_id,
-            container_type=ContainerType.RUN,
-            paths=paths,
-            use_proto=True,
-        )
-        fetched = {field.path: self._field_to_fetchable_visitor.visit(field) for field in data}
-        self._cache.update(fetched)
+        self._cache.prefetch(paths=paths)
```

### Comparing `neptune_fetcher-0.1.0/PKG-INFO` & `neptune_fetcher-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-fetcher
-Version: 0.1.0
+Version: 0.2.0
 Summary: Neptune Fetcher
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: neptune (==2.0.0a1)
+Requires-Dist: neptune (==2.0.0a2)
 Requires-Dist: tqdm (>=4.66.0)
 Project-URL: Documentation, https://docs.neptune.ai/
 Project-URL: Repository, https://github.com/neptune-ai/neptune-fetcher
 Project-URL: Tracker, https://github.com/neptune-ai/neptune-fetcher/issues
 Description-Content-Type: text/markdown
 
 # Neptune Fetcher
@@ -326,11 +326,84 @@
 ```
 
 __Returns__:
 `str`
 
 ---
 
+### Datetime
+#### `fetch()`
+Retrieves value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+created_at = run["sys/creation_time"].fetch()
+```
+
+__Returns__:
+`datetime.datetime`
+
+---
+
+### Object state
+#### `fetch()`
+Retrieves value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+state = run["sys/state"].fetch()
+```
+
+__Returns__:
+`str`
+
+---
+
+### Boolean
+#### `fetch()`
+Retrieves value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+status = run["sys/failed"].fetch()
+```
+
+__Returns__:
+`bool`
+
+---
+
+### Float series
+#### `fetch()` or `fetch_last()`
+Retrieves last series value either from the internal cache (see [`prefetch()`](#prefetch)) or from the API.
+
+__Example__:
+```python
+loss = run["loss"].fetch_last()
+```
+
+__Returns__:
+`Optional[float]`
+
+#### `fetch_values()`
+Retrieves all series values from the API.
+
+__Parameters__:
+
+| Name | Type   | Default | Description                |
+| ---- |--------|---------|----------------------------|
+| `include_timestamp` | `bool` | True    | Whether the fetched data should include the timestamp field. |
+
+__Example__:
+```python
+values = run["loss"].fetch_values()
+```
+
+__Returns__:
+`pandas.DataFrame`
+
+---
+
 ## License
 
 This project is licensed under the Apache License Version 2.0. For more details, see [Apache License Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
```

