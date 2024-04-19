# Comparing `tmp/ariadne_graphql_proxy-0.3.0.tar.gz` & `tmp/ariadne_graphql_proxy-0.4.0.dev1.tar.gz`

## Comparing `ariadne_graphql_proxy-0.3.0.tar` & `ariadne_graphql_proxy-0.4.0.dev1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/context_value.py
--rw-r--r--   0        0        0    12810 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/copy.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/errors.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/foreign_key_resolver.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/get_operation.py
--rw-r--r--   0        0        0    20423 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/merge.py
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/narrow_graphql_query.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/proxy_resolver.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/proxy_root_value.py
--rw-r--r--   0        0        0    16255 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/proxy_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/py.typed
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/query_filter.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/remote_schema.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/resolvers.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/selections.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/standard_types.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/str_to_field.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/backend.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/cache_key.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/cached_resolver.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/serializer.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/simple_cached_resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/aws/__init__.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/aws/cache_backend.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/cloudflare/__init__.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/cloudflare/cache_backend.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/imgix/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/imgix/query_params_resolver.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/LICENSE
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/README.md
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/context_value.py
+-rw-r--r--   0        0        0    26909 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/copy.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/errors.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/foreign_key_resolver.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/get_operation.py
+-rw-r--r--   0        0        0    20423 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/merge.py
+-rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/narrow_graphql_query.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/proxy_resolver.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/proxy_root_value.py
+-rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/proxy_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/py.typed
+-rw-r--r--   0        0        0    14202 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/query_filter.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/remote_schema.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/resolvers.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/selections.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/standard_types.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/str_to_field.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/unwrap_type.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/backend.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/cache_key.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/cached_resolver.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/serializer.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/simple_cached_resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/aws/__init__.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/aws/cache_backend.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/cloudflare/__init__.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/cloudflare/cache_backend.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/imgix/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/imgix/query_params_resolver.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/LICENSE
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/README.md
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ariadne_graphql_proxy-0.4.0.dev1/PKG-INFO
```

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/__init__.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from .proxy_resolver import ProxyResolver
 from .proxy_root_value import ProxyRootValue
 from .proxy_schema import ProxySchema
 from .query_filter import QueryFilter, QueryFilterContext
 from .remote_schema import get_remote_schema
 from .resolvers import set_resolver, unset_resolver
 from .selections import merge_selection_sets, merge_selections
+from .unwrap_type import unwrap_graphql_type
 
 __all__ = [
     "ForeignKeyResolver",
     "ProxyResolver",
     "ProxyRootValue",
     "ProxySchema",
     "QueryFilter",
@@ -91,8 +92,9 @@
     "merge_types",
     "merge_unions",
     "narrow_graphql_query",
     "raise_upstream_error",
     "set_resolver",
     "setup_root_resolver",
     "unset_resolver",
+    "unwrap_graphql_type",
 ]
```

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/errors.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/errors.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/foreign_key_resolver.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/foreign_key_resolver.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/get_operation.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/get_operation.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/merge.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/merge.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/narrow_graphql_query.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/narrow_graphql_query.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/proxy_resolver.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/proxy_resolver.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/proxy_root_value.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/proxy_root_value.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/proxy_schema.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/proxy_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         self.root_value: Optional[RootValue] = root_value
 
     def add_remote_schema(
         self,
         url: str,
         headers: Optional[ProxyHeaders] = None,
         *,
+        queries: Optional[List[str]] = None,
+        mutations: Optional[List[str]] = None,
         exclude_types: Optional[List[str]] = None,
         exclude_args: Optional[Dict[str, Dict[str, List[str]]]] = None,
         exclude_fields: Optional[Dict[str, List[str]]] = None,
         exclude_directives: Optional[List[str]] = None,
         exclude_directives_args: Optional[Dict[str, List[str]]] = None,
         extra_fields: Optional[Dict[str, List[str]]] = None,
         label: Optional[str] = None,
@@ -81,14 +83,16 @@
 
         schema_id = len(self.schemas)
 
         return self.add_schema(
             remote_schema,
             url,
             headers,
+            queries=queries,
+            mutations=mutations,
             exclude_types=exclude_types,
             exclude_args=exclude_args,
             exclude_fields=exclude_fields,
             exclude_directives=exclude_directives,
             exclude_directives_args=exclude_directives_args,
             extra_fields=extra_fields,
             label=label or f"remote_{schema_id}",
@@ -98,33 +102,39 @@
 
     def add_schema(
         self,
         schema: GraphQLSchema,
         url: Optional[str] = None,
         headers: Optional[ProxyHeaders] = None,
         *,
+        queries: Optional[List[str]] = None,
+        mutations: Optional[List[str]] = None,
         exclude_types: Optional[List[str]] = None,
         exclude_args: Optional[Dict[str, Dict[str, List[str]]]] = None,
         exclude_fields: Optional[Dict[str, List[str]]] = None,
         exclude_directives: Optional[List[str]] = None,
         exclude_directives_args: Optional[Dict[str, List[str]]] = None,
         extra_fields: Optional[Dict[str, List[str]]] = None,
         label: Optional[str] = None,
         proxy_errors: bool = True,
         proxy_extensions: bool = True,
     ) -> int:
         if (
-            exclude_types
+            queries
+            or mutations
+            or exclude_types
             or exclude_args
             or exclude_fields
             or exclude_directives
             or exclude_directives_args
         ):
             schema = copy_schema(
                 schema,
+                queries=queries,
+                mutations=mutations,
                 exclude_types=exclude_types,
                 exclude_args=exclude_args,
                 exclude_fields=exclude_fields,
                 exclude_directives=exclude_directives,
                 exclude_directives_args=exclude_directives_args,
             )
 
@@ -408,15 +418,14 @@
                 and self.proxy_errors[schema_id]
             ):
                 root_errors += self.clean_errors(label, subquery_data["errors"])
             if (
                 isinstance(subquery_data.get("extensions"), dict)
                 and self.proxy_extensions[schema_id]
             ):
-                print("HERE")
                 root_extensions[label] = subquery_data["extensions"]
 
         if root_errors or root_extensions:
             return self.proxy_root_value(
                 root_value,
                 root_errors or None,
                 root_extensions or None,
```

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/query_filter.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/query_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from graphql import (
     DocumentNode,
     FieldNode,
     FragmentDefinitionNode,
     FragmentSpreadNode,
     GraphQLSchema,
     InlineFragmentNode,
+    ListValueNode,
     NameNode,
+    ObjectValueNode,
     OperationDefinitionNode,
     SelectionNode,
     SelectionSetNode,
     VariableNode,
 )
 
 from .selections import merge_selections
@@ -149,20 +151,15 @@
 
     def filter_field_node(
         self,
         field_node: FieldNode,
         schema_obj: str,
         context: QueryFilterContext,
     ) -> Optional[FieldNode]:
-        context.variables.update(
-            argument.value.name.value
-            for argument in field_node.arguments
-            if isinstance(argument.value, VariableNode)
-        )
-
+        self.update_context_variables(field_node, context)
         if not field_node.selection_set:
             return field_node
 
         field_name = field_node.name.value
 
         if (
             schema_obj in self.foreign_keys
@@ -387,7 +384,27 @@
         schema_id: int,
         type_name: str,
     ) -> Optional[Dict[str, SelectionSetNode]]:
         if schema_id in self.dependencies and type_name in self.dependencies[schema_id]:
             return self.dependencies[schema_id][type_name]
 
         return None
+
+    def update_context_variables(
+        self, field_node: FieldNode, context: QueryFilterContext
+    ):
+        for argument in field_node.arguments:
+            self.extract_variables(argument.value, context)  # type: ignore
+
+    def extract_variables(
+        self,
+        value: VariableNode | ListValueNode | ObjectValueNode,
+        context: QueryFilterContext,
+    ):
+        if isinstance(value, VariableNode):
+            context.variables.add(value.name.value)
+        elif isinstance(value, ObjectValueNode):
+            for field in value.fields:
+                self.extract_variables(field.value, context)  # type: ignore
+        elif isinstance(value, ListValueNode):
+            for item in value.values:
+                self.extract_variables(item, context)  # type: ignore
```

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/remote_schema.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/remote_schema.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/resolvers.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/resolvers.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/selections.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/selections.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/standard_types.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/standard_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from graphql import GraphQLBoolean, GraphQLFloat, GraphQLID, GraphQLInt, GraphQLString
 
+STANDARD_DIRECTIVES = (
+    "skip",
+    "include",
+    "deprecated",
+    "specifiedBy",
+)
+
 STANDARD_TYPES = (
     "ID",
     "Boolean",
     "Float",
     "Int",
     "String",
     "__Schema",
```

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/str_to_field.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/str_to_field.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/__init__.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/backend.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/backend.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/cache_key.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/cache_key.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/cached_resolver.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/cached_resolver.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/serializer.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/serializer.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/cache/simple_cached_resolver.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/cache/simple_cached_resolver.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/aws/cache_backend.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/aws/cache_backend.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/cloudflare/cache_backend.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/cloudflare/cache_backend.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/ariadne_graphql_proxy/contrib/imgix/query_params_resolver.py` & `ariadne_graphql_proxy-0.4.0.dev1/ariadne_graphql_proxy/contrib/imgix/query_params_resolver.py`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/.gitignore` & `ariadne_graphql_proxy-0.4.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/LICENSE` & `ariadne_graphql_proxy-0.4.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/README.md` & `ariadne_graphql_proxy-0.4.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ariadne_graphql_proxy-0.3.0/pyproject.toml` & `ariadne_graphql_proxy-0.4.0.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.3.0"
+version = "0.4.0.dev1"
 dependencies = [
   "graphql-core>=3.2.0,<3.3",
   "httpx",
   "ariadne>=0.23.0",
 ]
 
 [project.optional-dependencies]
```

### Comparing `ariadne_graphql_proxy-0.3.0/PKG-INFO` & `ariadne_graphql_proxy-0.4.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ariadne-graphql-proxy
-Version: 0.3.0
+Version: 0.4.0.dev1
 Summary: Ariadne toolkit for building GraphQL proxies.
 Project-URL: Homepage, https://ariadnegraphql.org/
 Project-URL: Repository, https://github.com/mirumee/ariadne-graphql-proxy
 Project-URL: Bug Tracker, https://github.com/mirumee/ariadne-graphql-proxy/issues
 Project-URL: Community, https://github.com/mirumee/ariadne/discussions
 Project-URL: Twitter, https://twitter.com/AriadneGraphQL
 Author-email: Mirumee Software <hello@mirumee.com>
```

