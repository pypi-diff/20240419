# Comparing `tmp/isagog_ai-0.8.5.tar.gz` & `tmp/isagog_ai-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.8.5.tar", max compression
+gzip compressed data, was "isagog_ai-0.8.6.tar", max compression
```

## Comparing `isagog_ai-0.8.5.tar` & `isagog_ai-0.8.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.5/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.5/isagog/client/__init__.py
--rw-r--r--   0        0        0    10003 2024-04-16 08:17:48.784662 isagog_ai-0.8.5/isagog/client/kg_client.py
--rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.8.5/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.5/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.5/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.5/isagog/model/__init__.py
--rw-r--r--   0        0        0    23276 2024-04-16 14:14:33.202407 isagog_ai-0.8.5/isagog/model/kg_model.py
--rw-r--r--   0        0        0    26878 2024-04-16 07:29:03.592734 isagog_ai-0.8.5/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.5/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.5/LICENSE
--rw-r--r--   0        0        0      588 2024-04-16 08:35:19.804960 isagog_ai-0.8.5/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.5/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.6/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.6/isagog/client/__init__.py
+-rw-r--r--   0        0        0    10003 2024-04-16 08:17:48.784662 isagog_ai-0.8.6/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     6456 2024-04-16 08:17:48.810054 isagog_ai-0.8.6/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.6/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.6/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.6/isagog/model/__init__.py
+-rw-r--r--   0        0        0    26806 2024-04-19 09:17:25.151550 isagog_ai-0.8.6/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    26878 2024-04-16 07:29:03.592734 isagog_ai-0.8.6/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.6/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.6/LICENSE
+-rw-r--r--   0        0        0      588 2024-04-16 14:15:47.037432 isagog_ai-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.6/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.6/PKG-INFO
```

### Comparing `isagog_ai-0.8.5/isagog/client/kg_client.py` & `isagog_ai-0.8.6/isagog/client/kg_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.5/isagog/client/nlp_client.py` & `isagog_ai-0.8.6/isagog/client/nlp_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.5/isagog/generator/sparql_generator.py` & `isagog_ai-0.8.6/isagog/generator/sparql_generator.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.5/isagog/model/kg_model.py` & `isagog_ai-0.8.6/isagog/model/kg_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,37 @@
     (c) Isagog S.r.l. 2024, MIT License
 """
 import logging
 from typing import IO, TextIO, Any, Callable, Dict
 
 from rdflib import OWL, Graph, RDF, URIRef, RDFS
 
-# Type definitions
+import re
 
-Reference = URIRef | str
+
+class Identifier(str):
+    def __new__(cls, _id):
+        if not cls.is_valid_id(_id):
+            raise ValueError(f"Invalid ID format: {_id}")
+        return str.__new__(cls, _id)
+
+    @staticmethod
+    def is_valid_id(_id):
+        pattern = re.compile(
+            r'^[a-zA-Z][a-zA-Z0-9+.-]*:'  # Scheme: Any valid URI scheme
+            r'[a-zA-Z0-9-._~:/?#\[\]@!$&\'()*+,;=%]*$'  # Path: Any valid URI character
+        )
+        return re.match(pattern, _id)
+
+
+Reference = URIRef | Identifier
 
 OWL_ENTITY_TYPES = [OWL.Class, OWL.NamedIndividual, OWL.ObjectProperty, OWL.DatatypeProperty, OWL.AnnotationProperty]
 
-PROFILE_ATTRIBUTE = "https://isagog.com/ontology#profile"
+PROFILE_ATTRIBUTE = Identifier("http://isagog.com/ontology#profile")
 
 
 def _uri_label(uri: str) -> str:
     """
     Extracts a label from a URI
     :param uri:
     :return:
@@ -49,14 +65,15 @@
                      if not callable(value) and not key.startswith('_')])
         if not data:
             return str(obj)
         if classkey is not None and hasattr(obj, "__class__"):
             data[classkey] = obj.__class__.__name__
         return data
     else:
+        # can't convert to dict
         return obj
 
 
 class Entity(object):
     """
     Any identified knowledge entity, either predicative (property) or individual
     Every entity has a string identifier and an optional meta type, which can be an OWL type
@@ -65,15 +82,23 @@
     def __init__(self, _id: Reference, **kwargs):
         """
 
         :param _id: the entity identifier, will be converted to a string
         :param kwargs:
         """
         assert _id
-        self.id = str(_id).strip("<>")
+        if isinstance(_id, URIRef):
+            _id = Identifier(str(_id))
+        elif isinstance(_id, Identifier):
+            pass
+        elif isinstance(_id, str):
+            _id = Identifier(_id)
+        else:
+            raise ValueError("bad id object")
+        self.id = _id  # str(_id).strip("<>")
         owl_type = kwargs.get('owl')
         if owl_type:
             if owl_type in OWL_ENTITY_TYPES:
                 self.__meta__ = owl_type
             else:
                 logging.warning("bad owl type %s", owl_type)
         else:
@@ -87,23 +112,34 @@
         )
 
     def __hash__(self):
         return self.id.__hash__()
 
     def to_dict(self, **kwargs) -> dict:
         """
-        Converts the entity to a json serializable dictionary
-        :param serializer:
-        :param kwargs:
-        :return:
+        Converts the entity to a json serializable dictionary.
+        :param kwargs: format (a string to specify the output format, 'api' for API output,
+                               default: object to dict conversion)
+                       serializer (a custom function to use for serialization, overrides format if present)
+        :return: a serializable dictionary representation of the entity
         """
         if 'serializer' in kwargs:
             serializer = kwargs.get('serializer')
             if not isinstance(serializer, Callable):
                 raise ValueError("bad serializer")
+        elif 'format' in kwargs:
+            if kwargs.get('format') == 'api':
+                rt = {
+                    "id": self.id,
+                }
+                if hasattr(self, '__meta__'):
+                    rt['meta'] = self.__meta__
+                return rt
+            else:
+                serializer = _todict
         else:
             serializer = _todict
         return serializer(self)
 
 
 class Concept(Entity):
     """
@@ -208,14 +244,28 @@
         return not self.values
 
     def to_dict(self, **kwargs) -> dict:
         if 'serializer' in kwargs:
             serializer = kwargs.get('serializer')
             if not isinstance(serializer, Callable):
                 raise ValueError("bad serializer")
+        elif 'format' in kwargs:
+            if kwargs.get('format') == 'api':
+                rt = {
+                    "id": self.predicate,
+                    "subject": self.subject,
+                    "values": self.values
+                }
+                if hasattr(self, 'label'):
+                    rt['label'] = self.label
+                if hasattr(self, 'comment'):
+                    rt['comment'] = self.comment
+                return rt
+            else:
+                serializer = _todict
         else:
             serializer = _todict
         return serializer(self)
 
 
 class Ontology(Graph):
     """
@@ -383,29 +433,30 @@
     def first_value(self, default=None) -> str | int | float | bool | None:
         if len(self.values) > 0:
             return self.values[0]
         else:
             return default
 
     def to_dict(self, **kwargs) -> dict:
-        nested = kwargs.get('nested', False)
+        if 'serializer' in kwargs:
+            return super().to_dict(serializer=kwargs.get('serializer'))
         rt = {}
-        if nested:
+        if 'format' in kwargs and kwargs.get('format') == 'api':
             rt["id"] = self.predicate
             if hasattr(self, 'label'):
                 rt['label'] = self.label
             if hasattr(self, 'type'):
                 rt['type'] = self.type
             rt['values'] = self.values
         else:
             return super().to_dict()
         return rt
 
 
-VOID_ATTRIBUTE = AttributeInstance(predicate='https://isagog.com/attribute#void')
+VOID_ATTRIBUTE = AttributeInstance(predicate='http://isagog.com/attribute#void')
 
 
 class RelationInstance(Assertion):
     """
     Relational assertion
     """
 
@@ -471,30 +522,34 @@
             for kind in individual.kind:
                 if kind not in kind_map:
                     kind_map[kind] = []
                 kind_map[kind].append(individual)
         return kind_map
 
     def to_dict(self, **kwargs) -> dict:
-
-        nested = kwargs.get('nested', False)
+        if 'serializer' in kwargs:
+            return super().to_dict(serializer=kwargs.get('serializer'))
         rt = {}
-        if nested:
-            rt["id"] = self.predicate
-            if hasattr(self, 'label'):
-                rt['label'] = self.label
-            if hasattr(self, 'type'):
-                rt['type'] = self.type
-            rt['values'] = [ind.to_dict(nested=True) for ind in self.values]
+        if 'format' in kwargs:
+            if kwargs.get('format') == 'api':
+                rt["id"] = str(self.predicate)
+                if hasattr(self, 'label'):
+                    rt['label'] = str(self.label)
+                if hasattr(self, 'type'):
+                    rt['type'] = str(self.type)
+                rt['values'] = [ind.to_dict(format='api') for ind in self.values]
+            else:
+                logging.warning("unknown format %s", kwargs.get('format'))
+                rt = super().to_dict()
         else:
             rt = super().to_dict()
         return rt
 
 
-VOID_RELATION = RelationInstance(predicate='https://isagog.com/relation#void')
+VOID_RELATION = RelationInstance(predicate='http://isagog.com/relation#void')
 
 
 class Individual(Entity):
     """
     Individual entity
 
     """
@@ -592,27 +647,40 @@
         """
         Gets all assertions about the individual
         :return:
         """
         return self.attributes + self.relations
 
     def set_score(self, score: float):
+        """
+        Sets the individual score, i.e. the relevance of the individual in a given context (e.g. a search result)
+        :param score:
+        :return:
+        """
         self.score = score
 
     def get_score(self) -> float | None:
+        """
+        Gets the individual score, i.e. the relevance of the individual in a given context (e.g. a search result)
+        :return:
+        """
         if hasattr(self, 'score'):
             return self.score
         else:
             return None
 
     def has_score(self) -> bool:
+        """
+        Tells if the individual has a score
+        :return:
+        """
         return hasattr(self, 'score')
 
     def add_attribute(self,
-                      predicate: Reference | str = None,
+                      predicate: Reference = None,
                       values: list[str | int | float | bool] = None,
                       instance: AttributeInstance = None):
         """
         Adds an attribute to the individual
         One of predicate or instance must be provided (but not both: in that case, instance is preferred)
         :param values:
         :param predicate:
@@ -628,15 +696,15 @@
             if not existing or existing.is_empty():
                 self.attributes.append(instance)
             else:
                 existing.values.extend([value for value in instance.values if value not in existing.values])
         else:
             if not predicate:
                 raise ValueError("missing property")
-            if not isinstance(predicate, (Reference, str)):
+            if not isinstance(predicate, Reference):
                 raise ValueError("bad property")
             self.add_attribute(instance=AttributeInstance(predicate=predicate, values=values))
         self._refresh = True
 
     def add_relation(self,
                      predicate: Reference | str = None,
                      values: list[Reference | str] = None,
@@ -671,18 +739,31 @@
     def need_update(self):
         return self._refresh
 
     def updated(self):
         self._refresh = False
 
     def to_dict(self, **kwargs) -> dict:
-        nested = kwargs.get('nested', False)
-        if nested:
-            rt = {
-                "id": self.id,
-                "kind": [k for k in self.kind],
-                "label": self.label,
-                "comment": self.comment,
-            }
+        if 'serializer' in kwargs:
+            return super().to_dict(serializer=kwargs.get('serializer'))
+        rt = {}
+        if 'format' in kwargs:
+            if kwargs.get('format') == 'api':
+                rt['id'] = str(self.id)
+                if self.kind:
+                    rt['kind'] = [str(k) for k in self.kind],  # [str(c.id) for c in self.get_kind()],
+                if self.label:
+                    rt['label'] = self.label
+                if self.comment:
+                    rt['comment'] = self.comment
+                if self.attributes:
+                    rt['attributes'] = [att.to_dict(format='api') for att in self.attributes]
+                if self.relations:
+                    rt['relations'] = [rel.to_dict(format='api') for rel in self.relations]
+                if hasattr(self, 'score'):
+                    rt['score'] = self.score
+            else:
+                logging.warning("unknown format %s", kwargs.get('format'))
+                rt = super().to_dict()
         else:
             rt = super().to_dict()
         return rt
```

### Comparing `isagog_ai-0.8.5/isagog/model/kg_query.py` & `isagog_ai-0.8.6/isagog/model/kg_query.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.5/LICENSE` & `isagog_ai-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.5/pyproject.toml` & `isagog_ai-0.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 382e 3522 0d0a 6465 7363 7269 7074 696f  8.5"..descriptio
+00000030: 382e 3622 0d0a 6465 7363 7269 7074 696f  8.6"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
```

### Comparing `isagog_ai-0.8.5/PKG-INFO` & `isagog_ai-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.8.5
+Version: 0.8.6
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

