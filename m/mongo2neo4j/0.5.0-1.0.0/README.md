# Comparing `tmp/mongo2neo4j-0.5.0.tar.gz` & `tmp/mongo2neo4j-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo2neo4j-0.5.0.tar", last modified: Thu Sep 28 10:20:22 2023, max compression
+gzip compressed data, was "mongo2neo4j-1.0.0.tar", last modified: Fri Apr 19 14:06:08 2024, max compression
```

## Comparing `mongo2neo4j-0.5.0.tar` & `mongo2neo4j-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2023-09-28 10:20:22.654936 mongo2neo4j-0.5.0/
--rw-r--r--   0 luther     (501) staff       (20)    35821 2023-08-05 21:05:58.000000 mongo2neo4j-0.5.0/LICENSE
--rw-r--r--   0 luther     (501) staff       (20)    45618 2023-09-28 10:20:22.654266 mongo2neo4j-0.5.0/PKG-INFO
--rw-r--r--   0 luther     (501) staff       (20)     4299 2023-09-28 10:15:01.000000 mongo2neo4j-0.5.0/README.md
--rw-r--r--   0 luther     (501) staff       (20)     5265 2023-09-27 09:11:14.000000 mongo2neo4j-0.5.0/pyproject.toml
--rw-r--r--   0 luther     (501) staff       (20)       38 2023-09-28 10:20:22.655107 mongo2neo4j-0.5.0/setup.cfg
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2023-09-28 10:20:22.642734 mongo2neo4j-0.5.0/src/
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2023-09-28 10:20:22.645778 mongo2neo4j-0.5.0/src/mongo2neo4j/
--rw-rw-r--   0 luther     (501) staff       (20)    47588 2023-09-28 08:27:12.000000 mongo2neo4j-0.5.0/src/mongo2neo4j/__init__.py
--rw-rw-r--   0 luther     (501) staff       (20)      137 2023-08-16 10:43:00.000000 mongo2neo4j-0.5.0/src/mongo2neo4j/__main__.py
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2023-09-28 10:20:22.650224 mongo2neo4j-0.5.0/src/mongo2neo4j.egg-info/
--rw-r--r--   0 luther     (501) staff       (20)    45618 2023-09-28 10:20:22.000000 mongo2neo4j-0.5.0/src/mongo2neo4j.egg-info/PKG-INFO
--rw-r--r--   0 luther     (501) staff       (20)      340 2023-09-28 10:20:22.000000 mongo2neo4j-0.5.0/src/mongo2neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 luther     (501) staff       (20)        1 2023-09-28 10:20:22.000000 mongo2neo4j-0.5.0/src/mongo2neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 luther     (501) staff       (20)       57 2023-09-28 10:20:22.000000 mongo2neo4j-0.5.0/src/mongo2neo4j.egg-info/entry_points.txt
--rw-r--r--   0 luther     (501) staff       (20)       12 2023-09-28 10:20:22.000000 mongo2neo4j-0.5.0/src/mongo2neo4j.egg-info/top_level.txt
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2023-09-28 10:20:22.652421 mongo2neo4j-0.5.0/tests/
--rw-rw-r--   0 luther     (501) staff       (20)       41 2023-07-06 07:53:53.000000 mongo2neo4j-0.5.0/tests/test_basic.py
--rw-rw-r--   0 luther     (501) staff       (20)     9859 2023-09-27 09:11:14.000000 mongo2neo4j-0.5.0/tests/test_flatten_and_cleanse.py
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.839669 mongo2neo4j-1.0.0/
+-rw-r--r--   0 luther     (501) staff       (20)    35821 2023-08-05 21:05:58.000000 mongo2neo4j-1.0.0/LICENSE
+-rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-19 14:06:08.839076 mongo2neo4j-1.0.0/PKG-INFO
+-rw-r--r--   0 luther     (501) staff       (20)     4347 2023-09-28 10:35:23.000000 mongo2neo4j-1.0.0/README.md
+-rw-r--r--   0 luther     (501) staff       (20)     6987 2024-02-12 16:48:54.000000 mongo2neo4j-1.0.0/pyproject.toml
+-rw-r--r--   0 luther     (501) staff       (20)      170 2024-04-19 13:47:32.000000 mongo2neo4j-1.0.0/requirements-dev.txt
+-rw-r--r--   0 luther     (501) staff       (20)       29 2024-04-16 11:28:39.000000 mongo2neo4j-1.0.0/requirements.txt
+-rw-r--r--   0 luther     (501) staff       (20)       38 2024-04-19 14:06:08.839778 mongo2neo4j-1.0.0/setup.cfg
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.828159 mongo2neo4j-1.0.0/src/
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.831901 mongo2neo4j-1.0.0/src/mongo2neo4j/
+-rw-rw-r--   0 luther     (501) staff       (20)    49265 2024-04-17 14:33:29.000000 mongo2neo4j-1.0.0/src/mongo2neo4j/__init__.py
+-rw-rw-r--   0 luther     (501) staff       (20)      138 2024-04-12 10:37:13.000000 mongo2neo4j-1.0.0/src/mongo2neo4j/__main__.py
+-rw-rw-r--   0 luther     (501) staff       (20)        0 2023-08-10 06:05:58.000000 mongo2neo4j-1.0.0/src/mongo2neo4j/py.typed
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.836621 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/
+-rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 luther     (501) staff       (20)      441 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 luther     (501) staff       (20)        1 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 luther     (501) staff       (20)       57 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/entry_points.txt
+-rw-r--r--   0 luther     (501) staff       (20)      206 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/requires.txt
+-rw-r--r--   0 luther     (501) staff       (20)       12 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/top_level.txt
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.835596 mongo2neo4j-1.0.0/tests/
+-rw-rw-r--   0 luther     (501) staff       (20)       41 2023-07-06 07:53:53.000000 mongo2neo4j-1.0.0/tests/test_basic.py
+-rw-rw-r--   0 luther     (501) staff       (20)     9949 2023-10-15 11:38:33.000000 mongo2neo4j-1.0.0/tests/test_flatten_and_cleanse.py
```

### Comparing `mongo2neo4j-0.5.0/LICENSE` & `mongo2neo4j-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo2neo4j-0.5.0/PKG-INFO` & `mongo2neo4j-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo2neo4j
-Version: 0.5.0
+Version: 1.0.0
 Summary: Imports object structures generated by MongoDB object relation mappers (like Mongoose) into Neo4j for exploration with SemSpect
 Author: Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,14 +684,28 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymongo>=4.6.3
+Requires-Dist: neo4j>=5.19.0
+Provides-Extra: dev
+Requires-Dist: mypy>=1.9.0; extra == "dev"
+Requires-Dist: pyright>=1.1.359; extra == "dev"
+Requires-Dist: ruff>=0.3.7; extra == "dev"
+Requires-Dist: pylint>=3.1.0; extra == "dev"
+Requires-Dist: pytest>=8.1.1; extra == "dev"
+Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
+Requires-Dist: coverage-badge>=1.1.0; extra == "dev"
+Requires-Dist: pre-commit>=3.7.0; extra == "dev"
+Requires-Dist: twine>=5.0.0; extra == "dev"
+Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: codespell>=2.2.6; extra == "dev"
 
 # [mongo2neo4j](https://makomo.github.io/mongo2neo4j/)
 
 [MongoDB](https://www.mongodb.com/) [Mongoose](https://mongoosejs.com/) to [Neo4j](https://neo4j.com/) Importer
 
 ![License](https://img.shields.io/github/license/MAKOMO/mongo2neo4j.svg)
 [![Pylint](https://github.com/MAKOMO/mongo2neo4j/actions/workflows/pylint.yaml/badge.svg)](https://github.com/MAKOMO/mongo2neo4j/actions/workflows/pylint.yaml)
@@ -752,13 +766,13 @@
 
 Further configuration options are listed on calling
 
 ```sh
 % mongo2neo4j -h
 ```
 
-See [Script Arguments](https://github.com/MAKOMO/mongo2neo4j/wiki/Script-Arguments) for the full list of available arguments and the [example](example/README.md) documenting the workflow of mongo2neo4j using randomly generated sample data.
+See [Script Arguments](https://github.com/MAKOMO/mongo2neo4j/wiki/Script-Arguments) for the full list of available arguments and the [example](https://github.com/MAKOMO/mongo2neo4j/blob/main/example/README.md) documenting the workflow of mongo2neo4j using randomly generated sample data.
 
 
 
 
 NOTE: *if the [APOC plugin](https://neo4j.com/docs/apoc/) is installed in the Neo4j DB, the faster and memory-effective `apoc.periodic.iterate` method is used to generate nodes and sublabels.*
```

### Comparing `mongo2neo4j-0.5.0/README.md` & `mongo2neo4j-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,13 +61,13 @@
 
 Further configuration options are listed on calling
 
 ```sh
 % mongo2neo4j -h
 ```
 
-See [Script Arguments](https://github.com/MAKOMO/mongo2neo4j/wiki/Script-Arguments) for the full list of available arguments and the [example](example/README.md) documenting the workflow of mongo2neo4j using randomly generated sample data.
+See [Script Arguments](https://github.com/MAKOMO/mongo2neo4j/wiki/Script-Arguments) for the full list of available arguments and the [example](https://github.com/MAKOMO/mongo2neo4j/blob/main/example/README.md) documenting the workflow of mongo2neo4j using randomly generated sample data.
 
 
 
 
 NOTE: *if the [APOC plugin](https://neo4j.com/docs/apoc/) is installed in the Neo4j DB, the faster and memory-effective `apoc.periodic.iterate` method is used to generate nodes and sublabels.*
```

### Comparing `mongo2neo4j-0.5.0/src/mongo2neo4j/__init__.py` & `mongo2neo4j-1.0.0/src/mongo2neo4j/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
-"""
-Imports object structures generated by the ORM Mongoose <https://mongoosejs.com/> and
+"""Imports object structures generated by the ORM Mongoose <https://mongoosejs.com/> and
 stored in MongoDB <https://www.mongodb.com/> into Neo4j <https://neo4j.com/> for exploration with
 SemSpect <https://www.semspect.de/>.
 """
 
 # Changelog:
+#  v1.0.0 (04/12/2024) : minor rework and lib updates
 #  v0.5.0 (09/28/2023) : makes import idempotent
 #  v0.4.0 (09/26/2023) : pytests, fixes
 #  v0.3.0 (08/16/2023) : src layout, pypip package
 #  v0.2.0 (08/10/2023) :
 #     - adds recursive processing of list of objects
 #     - adds options to link nodes via relations on matching field values that are not MongoDB ObjectIds
 #     - allow simple patterns to specify excluded fields and collections using a * at the begin or end of entries
@@ -35,139 +35,151 @@
 from neo4j import GraphDatabase, Driver, Session
 from neo4j.time import DateTime
 from neo4j.exceptions import Neo4jError, AuthError
 
 if TYPE_CHECKING:
     from pymongo.database import Database
     from pymongo.cursor import Cursor
+    from neo4j import ManagedTransaction
 
-__author__  = 'Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard, Maximilian Wenzel'
-__license__ = 'GPLv3 <https://www.gnu.org/licenses/gpl-3.0.html>'
-__version__ = '0.5.0'
+__author__ = "Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard, Maximilian Wenzel"
+__license__ = "GPLv3 <https://www.gnu.org/licenses/gpl-3.0.html>"
+__version__ = "1.0.0"
 
 
 # Types
 
 Item = dict[str, Any]
 Items = list[Item]
-Link = tuple[str,str] # holds source and target IDs
+Link = tuple[str, str]  # holds source and target IDs
 Links = set[Link]
-Relations = dict[str, Links] # associates relation name to Links
+Relations = dict[str, Links]  # associates relation name to Links
 Collections = set[str]
 Fields = set[str]
-NodeLabels = dict[str, str] # associating node IDs to labels
-LabelRelations = dict[str, Relations] # associates labels to relations
-SubLabel = tuple[str,str,str,str] # collection, field, sublabel postfix, OTHERS-sublabel (last two can be the empty string)
+NodeLabels = dict[str, str]  # associating node IDs to labels
+LabelRelations = dict[str, Relations]  # associates labels to relations
+SubLabel = tuple[
+    str, str, str, str
+]  # collection, field, sublabel postfix, OTHERS-sublabel (last two can be the empty string)
 SubLabels = list[SubLabel]
-CollectionField = tuple[str,str] # collection and field
-RelationSpecification = tuple[CollectionField,CollectionField] # source collection-attrib tuple & target collection-attrib tuple
+CollectionField = tuple[str, str]  # collection and field
+RelationSpecification = tuple[
+    CollectionField, CollectionField
+]  # source collection-attrib tuple & target collection-attrib tuple
 RelationSpecifications = list[RelationSpecification]
 
 
 class SubSpec(TypedDict):
     """A subtype specification."""
+
     discriminator: str
-    value_type: type # one of {str, list, bool}
-    postfix: str # empty string by default
-    others: str # empty string by default
-    distinct_values: NotRequired[set[str]] # if value_type is bool, distinct_values is not available
+    value_type: type  # one of {str, list, bool}
+    postfix: str  # empty string by default
+    others: str  # empty string by default
+    distinct_values: NotRequired[
+        set[str]
+    ]  # if value_type is bool, distinct_values is not available
 
 
 # Globals
 
 # default MongoDB documents ID field
-mid: str = '_id'
+mid: str = "_id"
 
 default_fields_to_remove: Fields = {
-    '__v'  # the document version will always be ignored and never transferred
-}
-
-default_exclude_collections: Collections = {
-    'system.*'
+    "__v"  # the document version will always be ignored and never transferred
 }
 
+default_exclude_collections: Collections = {"system.*"}
 
 
 # Utility functions
 
 
 def split_excludes(suppress: Fields) -> tuple[Fields, Fields, Fields]:
-    """Splits the given exclude field specifications into equal, startswith and endswith field supress matchers"""
+    """Splits the given exclude field specifications into equal, startswith and endswith field suppress matchers"""
     res_suppress: Fields = set()
     res_suppress_startswith: Fields = set()
     res_suppress_endswith: Fields = set()
     for sup in suppress:
-        if sup.startswith('*'):
+        if sup.startswith("*"):
             res_suppress_endswith.add(sup[1:])
-        elif sup.endswith('*'):
+        elif sup.endswith("*"):
             res_suppress_startswith.add(sup[:-1])
         else:
             res_suppress.add(sup)
     return res_suppress, res_suppress_startswith, res_suppress_endswith
 
-def match_collection(collection: str, excluded_collections:Collections) -> bool:
+
+def match_collection(collection: str, excluded_collections: Collections) -> bool:
     """Returns True if the given <collection> matches any pattern in <excluded_collections>"""
-    for xc in excluded_collections:
-        if (xc == collection or
-                (xc.startswith('*') and collection.endswith(xc[1:])) or
-                (xc.endswith('*') and collection.startswith(xc[:-1]))):
-            return True
-    return False
+    return any(
+        xc == collection
+        or xc.startswith("*")
+        and collection.endswith(xc[1:])
+        or xc.endswith("*")
+        and collection.startswith(xc[:-1])
+        for xc in excluded_collections
+    )
+
 
-def remove_excluded_collections(collections: Collections, excluded_collections: Collections) -> Collections:
-    """Removes all collections from the given <collections> that matchs any pattern in excluded_collections"""
+def remove_excluded_collections(
+    collections: Collections, excluded_collections: Collections
+) -> Collections:
+    """Removes all collections from the given <collections> that matches any pattern in excluded_collections"""
     return {c for c in collections if not match_collection(c, excluded_collections)}
 
 
-def strlist2subLabels(sl:list[str]) -> SubLabels:
-    """Takes a list of sublabel string specifications of the form <collection>.<field>[.<postfix>][,<others>] and turns it into a SubLabels specification."""
+def strlist2subLabels(sl: list[str]) -> SubLabels:
+    """Takes a list of sublabel string specifications of the form <collection>.<field>[.<postfix>][,<others>] and turns it into a SubLabels specification <label=collection, discriminator=field, postfix=postfix, others=others>."""
     sublabels: SubLabels = []
     for subl in sl:
-        el:list[str] = subl.split(',')[:2]
-        others:str = ''
+        el: list[str] = subl.split(",")[:2]
+        others: str = ""
         if len(el) > 1:
             others = el[1]
         if len(el) > 0:
-            parts:list[str] = el[0].split('.')[:3]
+            parts: list[str] = el[0].split(".")[:3]
             if len(parts) == 2:
-                parts += ['']
+                parts += [""]
             if len(parts) == 3:
                 sublabels.append((parts[0], parts[1], parts[2], others))
     return sublabels
 
-def strlist2relationSpecifications(rl:list[str]) -> RelationSpecifications:
+
+def strlist2relationSpecifications(rl: list[str]) -> RelationSpecifications:
     relationspecs: RelationSpecifications = []
     for rel in rl:
-        rels:list[str] = rel.split(',')[:2]
+        rels: list[str] = rel.split(",")[:2]
         if len(rels) == 2:
-            source = rels[0].split('.')[:2]
-            target = rels[1].split('.')[:2]
+            source = rels[0].split(".")[:2]
+            target = rels[1].split(".")[:2]
             if len(source) == 2 and len(target) == 2:
                 source_cf: CollectionField = (source[0], source[1])
                 target_cf: CollectionField = (target[0], target[1])
-                rel_spec: RelationSpecification = (source_cf,target_cf)
+                rel_spec: RelationSpecification = (source_cf, target_cf)
                 relationspecs.append(rel_spec)
     return relationspecs
 
+
 # see https://stackoverflow.com/questions/24527006/split-a-generator-into-chunks-without-pre-walking-it/34935239#34935239
-def chunker(n:int, iterable:Any) -> Iterator[Any]:
+def chunker(n: int, iterable: Any) -> Iterator[Any]:
     """chunker(3, 'ABCDEFG') --> ('A', 'B', 'C'), ('D', 'E', 'F'),  ('G',)"""
     fillvalue = object()  # Anonymous sentinel object that can't possibly appear in input
     arguments = (iter(iterable),) * n
     for x in zip_longest(*arguments, fillvalue=fillvalue):
         if x[-1] is fillvalue:
-            yield x[:bisect(x, False, key=lambda v: v is fillvalue)]  # Python 3.10+ only!
+            yield x[: bisect(x, False, key=lambda v: v is fillvalue)]  # Python 3.10+ only!
         else:
             yield x
 
 
 # see https://stackoverflow.com/questions/54815892/pymongo-cursor-batch-size
-def yield_rows(cursor: 'Cursor[Any]', chunk_size: int) -> Iterator[Items]:
-    """
-    Generator to yield chunks from cursor
+def yield_rows(cursor: "Cursor[Any]", chunk_size: int) -> Iterator[Items]:
+    """Generator to yield chunks from cursor
     :param cursor:
     :param chunk_size:
     :return:
     """
     chunk: Items = []
     for i, row in enumerate(cursor):
         if i % chunk_size == 0 and i > 0:
@@ -199,134 +211,150 @@
 def add_relations(relations: Relations, rel: str, new_links: Links) -> None:
     """Adds destructively the source-target tuples of new links under key rel to the given relations map"""
     if rel in relations:
         relations[rel].update(new_links)
     else:
         relations[rel] = new_links
 
+
 def update_relations(relations: Relations, new_relations: Relations) -> None:
     """Adds destructively the new_relations to the given relations map"""
-    for (key, values) in new_relations.items():
+    for key, values in new_relations.items():
         add_relations(relations, key, values)
 
-def add_object(objects: dict[str, Items], collection: str, new_objects: Items):
+
+def add_object(objects: dict[str, Items], collection: str, new_objects: Items) -> None:
     if collection in objects:
         objects[collection].extend(new_objects)
     else:
         objects[collection] = new_objects
 
-def update_objects(objects: dict[str, Items], new_objects: dict[str, Items]):
+
+def update_objects(objects: dict[str, Items], new_objects: dict[str, Items]) -> None:
     """Adds destructively the new_objects to the given collection-objects map"""
-    for (collection, col_objects) in new_objects.items():
+    for collection, col_objects in new_objects.items():
         add_object(objects, collection, col_objects)
 
+
 # converts ObjectId(_) to string
-def flatten_and_cleanse(
-        collection: str,
-        dictionary: MutableMapping[str, Any],
-        suppress: Fields,
-        suppress_startswith: Fields,
-        suppress_endswith: Fields,
-        parent_key: str = '',
-        node_id: str = '',
-        separator: str = '_') -> tuple[Item, Relations, Fields, dict[str, Items]]:
+def flatten_and_cleanse(  # pylint: disable=too-complex, too-many-arguments, too-many-locals
+    collection: str,
+    dictionary: MutableMapping[str, Any],
+    suppress: Fields,
+    suppress_startswith: Fields,
+    suppress_endswith: Fields,
+    parent_key: str = "",
+    node_id: str = "",
+    separator: str = "_",
+) -> tuple[Item, Relations, Fields, dict[str, Items]]:
     """Returns the given dictionary with sub dictionaries flattened,
-        objectId(_) converted to strings and keys in the 'suppress', 'suppress_startswith', 'suppress_endswith' sets
-        removed. As second result a dictionary associating relation names
-        with list of tuples of source and target node ids.
-        As third result a set of attributes of type list.
-        As last result a dict associating labels with additional objects created."""
+    objectId(_) converted to strings and keys in the 'suppress', 'suppress_startswith', 'suppress_endswith' sets
+    removed. As second result a dictionary associating relation names
+    with list of tuples of source and target node ids.
+    As third result a set of attributes of type list.
+    As last result a dict associating labels with additional objects created."""
     res: Item = {}
     relations: Relations = {}
     array_fields: Fields = set()
-    additional_objects: dict[str, Items] = {} # additional objects associated to new labels
+    additional_objects: dict[str, Items] = {}  # additional objects associated to new labels
 
-    if parent_key == '' and mid in dictionary:
+    if parent_key == "" and mid in dictionary:
         node_id = str(dictionary[mid])
 
     for key, value in dictionary.items():
-        if (key not in suppress and
-                not key.startswith(tuple(suppress_startswith)) and
-                not key.endswith(tuple(suppress_endswith)) and
-                value is not None and
-                value != '' and value != []):
-            uuid_hex:str
+        if (
+            key not in suppress
+            and not key.startswith(tuple(suppress_startswith))
+            and not key.endswith(tuple(suppress_endswith))
+            and value is not None
+            and value != ""
+            and value != []
+        ):
+            uuid_hex: str
             new_key = parent_key + separator + key if parent_key else key
             if isinstance(value, MutableMapping):
                 if mid in value:
                     uuid_hex = str(value[mid])
                     value[mid] = uuid_hex
-                    new_label = f'{collection}_{new_key}'
+                    new_label = f"{collection}_{new_key}"
                     # we create a new object and link it
                     rec_res, rec_relations, rec_array_fields, rec_objects = flatten_and_cleanse(
-                                new_label,
-                                value,
-                                suppress,
-                                suppress_startswith,
-                                suppress_endswith,
-                                '',
-                                '',
-                                separator)
+                        new_label,
+                        value,
+                        suppress,
+                        suppress_startswith,
+                        suppress_endswith,
+                        "",
+                        "",
+                        separator,
+                    )
                     add_object(additional_objects, new_label, [rec_res])
                     update_relations(relations, rec_relations)
                     array_fields.update(rec_array_fields)
                     update_objects(additional_objects, rec_objects)
                     add_relation(relations, key, (node_id, uuid_hex))
                 else:
                     # we flatten the object
                     rec_res, rec_relations, rec_array_fields, rec_objects = flatten_and_cleanse(
-                            collection,
-                            value,
-                            suppress,
-                            suppress_startswith,
-                            suppress_endswith,
-                            new_key,
-                            node_id,
-                            separator)
+                        collection,
+                        value,
+                        suppress,
+                        suppress_startswith,
+                        suppress_endswith,
+                        new_key,
+                        node_id,
+                        separator,
+                    )
                     res.update(rec_res)
                     update_relations(relations, rec_relations)
                     array_fields.update(rec_array_fields)
                     update_objects(additional_objects, rec_objects)
             elif isinstance(value, ObjectId):
                 id_str: str = str(value)
-                if new_key != mid and node_id != '':
+                if new_key != mid and node_id != "":
                     add_relation(relations, new_key, (node_id, id_str))
                 else:
                     res[new_key] = id_str
             elif isinstance(value, MutableSequence):
                 if all(isinstance(v, str) for v in value):
                     # homogeneous list of strings
                     res[new_key] = value
-                    array_fields.add(new_key) # mark as field of type array, to have sublabels generated correctly on demand
-                elif (all(isinstance(v, int) for v in value) or
-                        all(isinstance(v, float) for v in value)):
+                    array_fields.add(
+                        new_key
+                    )  # mark as field of type array, to have sublabels generated correctly on demand
+                elif all(isinstance(v, int) for v in value) or all(
+                    isinstance(v, float) for v in value
+                ):
                     # homogeneous list of numbers (not marked as field of type array, to have field ignored on sublabel generation)
                     res[new_key] = value
-                elif all(isinstance(v, ObjectId) for v in value) and new_key != mid and node_id != '':
+                elif (
+                    all(isinstance(v, ObjectId) for v in value) and new_key != mid and node_id != ""
+                ):
                     # homogeneous list of ObjectIds
                     # we discard the field, but establish the relations
                     add_relations(relations, new_key, {(node_id, str(v)) for v in value})
                 elif all(isinstance(v, MutableMapping) for v in value):
                     # list of objects
-                    new_label = f'{collection}_{new_key}'
+                    new_label = f"{collection}_{new_key}"
                     uuids = []
                     for i, v in enumerate(value):
                         # if there is no unique object id we generate one
-                        uuid_hex = (str(v[mid]) if mid in v else f'{node_id}{new_label}{i}')
+                        uuid_hex = str(v[mid]) if mid in v else f"{node_id}{new_label}{i}"
                         uuids.append(uuid_hex)
                         v[mid] = uuid_hex
                         rec_res, rec_relations, rec_array_fields, rec_objects = flatten_and_cleanse(
-                                new_label,
-                                v,
-                                suppress,
-                                suppress_startswith,
-                                suppress_endswith,
-                                '',
-                                '',
-                                separator)
+                            new_label,
+                            v,
+                            suppress,
+                            suppress_startswith,
+                            suppress_endswith,
+                            "",
+                            "",
+                            separator,
+                        )
                         add_object(additional_objects, new_label, [rec_res])
                         update_relations(relations, rec_relations)
                         array_fields.update(rec_array_fields)
                         update_objects(additional_objects, rec_objects)
                     # add relations between this object and all generated ids
                     for uuid_hex in uuids:
                         add_relation(relations, new_key, (node_id, uuid_hex))
@@ -338,765 +366,823 @@
 def split_attributes(dictionary: Item) -> tuple[Item, Item]:
     """Splits the given attributes into those with primitive values and those with \
         non-primitive ones"""
     primitive: Item = {}
     non_primitive: Item = {}
     for key, value in dictionary.items():
         if isinstance(value, list) and not all(
-                isinstance(e, (str | bool | int | float)) for e in value):
+            isinstance(e, (str | bool | int | float)) for e in value
+        ):
             non_primitive[key] = value
         else:
             primitive[key] = value
     return primitive, non_primitive
 
 
 # see https://stackoverflow.com/a/34325723
 # Progress Bar Printing Function
-def printProgressBar(iteration, total = 100, prefix = '', suffix = '', decimals = 1, length = 70, fill = '█', printEnd = '\r'):
+def printProgressBar(  # pylint: disable=too-many-arguments
+    iteration: int,
+    total: int = 100,
+    prefix: str = "",
+    suffix: str = "",
+    decimals: int = 1,
+    length: int = 70,
+    fill: str = "█",
+    printEnd: str = "\r",
+) -> None:
     """Outputs a progress bar to stdout"""
-    percent = f'{100 * (iteration / float(total)):.{decimals}f}'
+    percent = f"{100 * (iteration / float(total)):.{decimals}f}"
     filledLength = int(length * iteration // total)
-    progbar = fill * filledLength + '-' * (length - filledLength)
-    print(f'\r{prefix} |{progbar}| {percent}% {suffix}', end = printEnd)
-
+    progbar = fill * filledLength + "-" * (length - filledLength)
+    print(f"\r{prefix} |{progbar}| {percent}% {suffix}", end=printEnd)
 
 
 # Neo4j communication
 
+
 def render_value(value: Any) -> str:
     """Render given value as str"""
     if isinstance(value, DateTime):
         return f"datetime('{value}')"
     if isinstance(value, datetime.datetime):
-        value_as_isoformat_datetime: str = value.isoformat(sep='T')
+        value_as_isoformat_datetime: str = value.isoformat(sep="T")
         return f"datetime('{value_as_isoformat_datetime}')"
     if isinstance(value, bool):
         return str(value).lower()
     if isinstance(value, (int | float)):
         return str(value)
     return f"'{value}'"
 
 
-def neo4j_output_query(query, **kwargs) -> None:
+def neo4j_output_query(query: str, **kwargs: Any) -> None:
     """Outputs the given Cypher query to stdout."""
     result = query
     for key, value in kwargs.items():
-        result = result.replace(
-            f'${key}', render_value(value))
+        result = result.replace(f"${key}", render_value(value))
     print(result)
 
 
-def neo4j_run_read_query(
-        session: None | Session, verbose: bool, query, **kwargs) -> None:
+def neo4j_run_read_query(session: None | Session, verbose: bool, query: str, **kwargs: Any) -> None:
     """Sends the given query to Neo4j and outputs it to stdout if verbose is True."""
 
-    def work(tx):  # pylint: disable=invalid-name
-        return tx.run(query, **kwargs)
+    def work(tx: "ManagedTransaction") -> Any:  # pylint: disable=invalid-name
+        return tx.run(query, **kwargs)  # pyright:ignore[reportGeneralTypeIssues, reportArgumentType]
 
     if verbose:
-        neo4j_output_query(query, **kwargs)
+        neo4j_output_query(query, **kwargs)  # pyright:ignore[reportGeneralTypeIssues, reportArgumentType]
     if session is not None:
         session.execute_read(work)
 
 
 def neo4j_run_write_query(
-        session: None | Session, verbose: bool, query, **kwargs) -> None:
+    session: None | Session, verbose: bool, query: str, **kwargs: Any
+) -> None:
     """Sends the given query to Neo4j and outputs it to stdout if verbose is True."""
 
-    def work(tx):  # pylint: disable=invalid-name
-        return tx.run(query, **kwargs)
+    def work(tx: "ManagedTransaction") -> Any:  # pylint: disable=invalid-name
+        return tx.run(query, **kwargs)  # pyright:ignore[reportGeneralTypeIssues, reportArgumentType]
 
     if verbose:
         neo4j_output_query(query, **kwargs)
     if session is not None:
         session.execute_write(work)
 
 
 def neo4j_create_index(session: None | Session, verbose: bool, label: str, field: str) -> None:
     """Creates an index on field <field> of <label>"""
     neo4j_run_write_query(
         session,
         verbose,
-        f'CREATE INDEX `{label.replace(" ", "_")}_{field.replace(" ", "_")}` IF NOT EXISTS FOR (l:`{label}`) ON l.`{field}`')
+        f'CREATE INDEX `{label.replace(" ", "_")}_{field.replace(" ", "_")}` IF NOT EXISTS FOR (l:`{label}`) ON l.`{field}`',
+    )
+
 
 def neo4j_create_constraint(session: None | Session, verbose: bool, label: str, field: str) -> None:
     """Creates a uniqueness constraint on field <field> of <label>"""
     neo4j_run_write_query(
         session,
         verbose,
-        f'CREATE CONSTRAINT `{label.replace(" ", "_")}_{field.replace(" ", "_")}` IF NOT EXISTS FOR (l:`{label}`) REQUIRE l.`{field}` IS UNIQUE')
+        f'CREATE CONSTRAINT `{label.replace(" ", "_")}_{field.replace(" ", "_")}` IF NOT EXISTS FOR (l:`{label}`) REQUIRE l.`{field}` IS UNIQUE',
+    )
 
-def neo4j_add_relations(
-        session: None | Session,
-        verbose: bool,
-        chunk_size: int,
-        apoc_installed: bool,
-        create: bool,
-        source: CollectionField,
-        target: CollectionField,
-        list_source: bool = False) -> None:
-    match_clause:str = (
-        f'MATCH (a:`{source[0]}`), (b:`{target[0]}`) '
-        f'WHERE b.`{target[1]}` {"IN" if list_source else "="} a.`{source[1]}`')
-    create_clause:str = f'{("CREATE" if create else "MERGE")} (a)-[:`{source[1]}`]->(b)'
+
+def neo4j_add_relations(  # pylint: disable=too-many-arguments
+    session: None | Session,
+    verbose: bool,
+    chunk_size: int,
+    apoc_installed: bool,
+    create: bool,
+    source: CollectionField,
+    target: CollectionField,
+    list_source: bool = False,
+) -> None:
+    match_clause: str = (
+        f"MATCH (a:`{source[0]}`), (b:`{target[0]}`) "
+        f'WHERE b.`{target[1]}` {"IN" if list_source else "="} a.`{source[1]}`'
+    )
+    create_clause: str = f'{("CREATE" if create else "MERGE")} (a)-[:`{source[1]}`]->(b)'
     if apoc_installed:
         neo4j_run_write_query(
             session,
             verbose,
-            (f'CALL apoc.periodic.iterate("{match_clause} RETURN a, b",'
-             f'"{create_clause}",'
-             f'{{batchSize:{chunk_size}, parallel:true}})'))
+            (
+                f'CALL apoc.periodic.iterate("{match_clause} RETURN a, b",'
+                f'"{create_clause}",'
+                f"{{batchSize:{chunk_size}, parallel:true}})"
+            ),
+        )
     else:
-        query = f'{match_clause} {create_clause}'
+        query = f"{match_clause} {create_clause}"
         neo4j_run_write_query(session, verbose, query)
 
-def neo4j_add_sublabel(
-        session: None | Session,
-        verbose: bool,
-        chunk_size: int,
-        apoc_installed: bool,
-        label: str,
-        field: str,
-        value: str,
-        sublabels: list[str],
-        isarray: bool = False) -> None:
+
+def neo4j_add_sublabel(  # pylint: disable=too-many-arguments
+    session: None | Session,
+    verbose: bool,
+    chunk_size: int,
+    apoc_installed: bool,
+    label: str,
+    field: str,
+    value: str,
+    sublabels: list[str],
+    isarray: bool = False,
+) -> None:
     """Adds <sublabel> to nodes in <label> where <value> is in list of <field> field values if isarray is True,
-       or if isarray is False and <field> value equals <value>."""
+    or if isarray is False and <field> value equals <value>."""
     if len(sublabels) > 0:
         if isarray:
-            match_clause = f'MATCH (n:`{label}`) WHERE {value} IN n.`{field}`'
+            match_clause = f"MATCH (n:`{label}`) WHERE {value} IN n.`{field}`"
         else:
-            match_clause = f'MATCH (n:`{label}` {{`{field}`: {value}}})'
-        quoted_sublabels = [f'`{sub}`' for sub in sublabels]
+            match_clause = f"MATCH (n:`{label}` {{`{field}`: {value}}})"
+        quoted_sublabels = [f"`{sub}`" for sub in sublabels]
         set_clause = f'SET n:{":".join(quoted_sublabels)}'
         if apoc_installed:
             neo4j_run_write_query(
                 session,
                 verbose,
-                (f'CALL apoc.periodic.iterate("{match_clause} RETURN n",'
-                 f'"{set_clause}",'
-                 f'{{batchSize:{chunk_size}, parallel:true}})'))
+                (
+                    f'CALL apoc.periodic.iterate("{match_clause} RETURN n",'
+                    f'"{set_clause}",'
+                    f"{{batchSize:{chunk_size}, parallel:true}})"
+                ),
+            )
         else:
-            neo4j_run_write_query(
-                session,
-                verbose,
-                f'{match_clause} {set_clause}')
+            neo4j_run_write_query(session, verbose, f"{match_clause} {set_clause}")
+
 
-def neo4j_add_sublabel_other(
-        session: None | Session,
-        verbose: bool,
-        chunk_size: int,
-        apoc_installed: bool,
-        label: str,
-        field: str,
-        others: str) -> None:
+def neo4j_add_sublabel_other(  # pylint: disable=too-many-arguments
+    session: None | Session,
+    verbose: bool,
+    chunk_size: int,
+    apoc_installed: bool,
+    label: str,
+    field: str,
+    others: str,
+) -> None:
     """Adds sublabel <others> to nodes in <label> where <value> of <field> is NULL"""
-    if others != '':
-        match_clause = f'MATCH (n:`{label}`) WHERE n.`{field}` is NULL'
-        set_clause = f'SET n:{others}'
+    if others != "":
+        match_clause = f"MATCH (n:`{label}`) WHERE n.`{field}` is NULL"
+        set_clause = f"SET n:{others}"
         if apoc_installed:
             neo4j_run_write_query(
                 session,
                 verbose,
-                (f'CALL apoc.periodic.iterate("{match_clause} RETURN n",'
-                 f'"{set_clause}",'
-                 f'{{batchSize:{chunk_size}, parallel:true}})'))
+                (
+                    f'CALL apoc.periodic.iterate("{match_clause} RETURN n",'
+                    f'"{set_clause}",'
+                    f"{{batchSize:{chunk_size}, parallel:true}})"
+                ),
+            )
         else:
-            neo4j_run_write_query(
-                session,
-                verbose,
-                f'{match_clause} {set_clause}')
+            neo4j_run_write_query(session, verbose, f"{match_clause} {set_clause}")
+
 
 # pylint: disable=too-many-arguments
-def process_data(
-        database: 'Database',
-        session: None | Session,
-        collections: Collections,
-        excluded_collections: Collections,
-        excluded_fields: Fields,
-        sublabels: SubLabels,
-        additional_relations: RelationSpecifications,
-        additional_list_relations: RelationSpecifications,
-        create: bool,
-        verbose: bool,
-        chunk_size: int) -> None:
+def process_data(  # pylint: disable=too-complex,too-many-locals
+    database: "Database[Any]",
+    session: None | Session,
+    collections: Collections,
+    excluded_collections: Collections,
+    excluded_fields: Fields,
+    sublabels: SubLabels,
+    additional_relations: RelationSpecifications,
+    additional_list_relations: RelationSpecifications,
+    create: bool,
+    verbose: bool,
+    chunk_size: int,
+) -> None:
     """Transfers all <collections> of the given MongoDB <db> via the <session> to Neo4j's \
         <neo4j_db> DB excluding the <excluded_collections> and the <excluded_fields>.
         If verbose, the generated Cypher queries are printed to stdout."""
 
-    node_label: NodeLabels = {} # associates the unique node _id to its label on creation of a node
-    all_relations: LabelRelations = {} # associates labels with relations given as association of relation names with list of tuples of source and target node ids
+    node_label: NodeLabels = {}  # associates the unique node _id to its label on creation of a node
+    all_relations: LabelRelations = (
+        {}
+    )  # associates labels with relations given as association of relation names with list of tuples of source and target node ids
     active_collections: Collections = remove_excluded_collections(collections, excluded_collections)
 
     array_fields = set()
 
     relations: Relations
     collection: str
 
     suppress: Fields
     suppress_startswith: Fields
     suppress_endswith: Fields
 
     suppress, suppress_startswith, suppress_endswith = split_excludes(excluded_fields)
 
-
     apoc_installed: bool = False
     if session is not None:
         try:
-            neo4j_run_read_query(
-                session,
-                verbose,
-                'RETURN apoc.version() AS output')
+            neo4j_run_read_query(session, verbose, "RETURN apoc.version() AS output")
             apoc_installed = True
-            print('Neo4j APOC plugin installed')
+            print("Neo4j APOC plugin installed")
         except Neo4jError:
-            # apoc plugin not installed
-            pass
+            print("Neo4j APOC plugin NOT installed")
 
     # add nodes
 
-    additional_objects: dict[str, Items] = {} # additional internal objects associated to new labels
+    additional_objects: dict[str, Items] = (
+        {}
+    )  # additional internal objects associated to new labels
 
     for collection in active_collections:
-        item_count: int = database[collection].count_documents({})
-        if item_count > 0:
+        if (item_count := database[collection].count_documents({})) > 0:
             print(f"*** processing {item_count} nodes of collection '{collection}'")
             relations = {}
             cursor: Cursor[Any] = database[collection].find({}, batch_size=chunk_size)
             chunk: Items
 
             # Establish constraints on '_id' attribute of label 'collection'
             # NOTE: the use of $ query parameters for constraint name and label
             #       does not work here, so we use Python fstring substitution
             neo4j_create_constraint(session, verbose, collection, mid)
 
             # Initial Progress Bar Call
             printProgressBar(0, item_count)
-            cnt:int = 0
+            cnt: int = 0
             for chunk in yield_rows(cursor, chunk_size):
                 cleansed_data: Items = []
                 # first we convert all objects in this chunk and extract its relations
                 for obj in chunk:
                     cnt += 1
-                    obj_data, obj_relations, obj_array_fields, obj_objects = flatten_and_cleanse(collection, obj, suppress, suppress_startswith, suppress_endswith)
-                    node_id: str = obj_data[mid]
-                    if node_id in node_label:
-                        print(f"ignoring object with duplicate ObjectId '{node_id}':{collection} (already registered as with label '{node_label[node_id]}').")
+                    obj_data, obj_relations, obj_array_fields, obj_objects = flatten_and_cleanse(
+                        collection, obj, suppress, suppress_startswith, suppress_endswith
+                    )
+                    if (node_id := obj_data[mid]) in node_label:
+                        print(
+                            f"ignoring object with duplicate ObjectId '{node_id}':{collection} (already registered with label '{node_label[node_id]}')."
+                        )
                     else:
                         cleansed_data.append(obj_data)
                         update_relations(relations, obj_relations)
                         node_label[node_id] = collection
                         array_fields.update(obj_array_fields)
                         update_objects(additional_objects, obj_objects)
                 # create the nodes per chunk
-                data: dict[str, Items] = {'batch': cleansed_data}
+                data: dict[str, Items] = {"batch": cleansed_data}
                 query = f"UNWIND $batch as row {('CREATE' if create else 'MERGE')} (n:`{collection}` {{{mid}: row.{mid}}}) SET n += row"
                 neo4j_run_write_query(session, verbose, query, **data)
                 # Update Progress Bar
                 printProgressBar(cnt, item_count)
             # print new line on complete
             print()
             all_relations[collection] = relations
 
-
     # add additional internal nodes
 
     for ao_label, ao_objects in additional_objects.items():
         if not match_collection(ao_label, excluded_collections):
             # register node_ids in node_label hash for new objects, skip others
-            new_objects:Items = []
+            new_objects: Items = []
             for ao_object in ao_objects:
-                node_id = ao_object[mid]
-                if node_id not in node_label:
+                if (node_id := ao_object[mid]) not in node_label:
                     node_label[node_id] = ao_label
                     new_objects.append(ao_object)
             # create nodes for new additional internal objects using the created composite labels
-            item_count = len(new_objects)
-            if item_count>0:
+            if (item_count := len(new_objects)) > 0:
                 neo4j_create_constraint(session, verbose, ao_label, mid)
                 print(f"*** processing {item_count} {ao_label} additional internal nodes'")
                 printProgressBar(0, item_count)
                 cnt = 0
                 for chunk in chunker(chunk_size, new_objects):
                     cnt += len(chunk)
-                    data = {'batch': chunk}
+                    data = {"batch": chunk}
                     query = f"UNWIND $batch as row {('CREATE' if create else 'MERGE')} (n:`{ao_label}` {{{mid}: row.{mid}}}) SET n += row"
                     neo4j_run_write_query(session, verbose, query, **data)
                     # Update Progress Bar
                     printProgressBar(cnt, item_count)
                 # print new line on complete
                 print()
 
-
     # add discovered relations
 
     for collection, relations in all_relations.items():
         # create relations (also per chunk)
         for rel, all_links in relations.items():
             # collected links by source and target label indexed by '<source_label>$<target_label>' with $ not allowed in MongoDB collection names
-            links_by_labels:dict[str, Links] = {}
+            links_by_labels: dict[str, Links] = {}
             for l in all_links:
                 if l[0] in node_label and l[1] in node_label:
-                    idx = f'{node_label[l[0]]}${node_label[l[1]]}'
-                    if idx in links_by_labels:
+                    if (idx := f"{node_label[l[0]]}${node_label[l[1]]}") in links_by_labels:
                         links_by_labels[idx].add(l)
                     else:
                         links_by_labels[idx] = {l}
                 elif l[0] not in node_label:
                     print(f'missing source object: ObjectId("{l[0]}")')
                 elif l[1] not in node_label:
-                    print(f'missing object linked from {node_label[l[0]]} ObjectId("{l[0]}") by attribute "{rel}": ObjectId("{l[1]}")')
+                    print(
+                        f'missing object linked from {node_label[l[0]]} ObjectId("{l[0]}") by attribute "{rel}": ObjectId("{l[1]}")'
+                    )
             for links in links_by_labels.values():
-                item_count = len(links)
-                if item_count > 0:
+                if (item_count := len(links)) > 0:
                     # Initial Progress Bar Call
                     printProgressBar(0, item_count)
                     cnt = 0
                     # assuming same source and target labels for all links
                     link = next(iter(links))
                     source_label: str = node_label[link[0]]
                     target_label: str = node_label[link[1]]
 
-                    print(f"*** processing {item_count} {rel} relation ({source_label}, {target_label}) of collection '{collection}'")
+                    print(
+                        f"*** processing {item_count} {rel} relation ({source_label}, {target_label}) of collection '{collection}'"
+                    )
 
                     for links_chunk in chunker(chunk_size, links):
                         cnt += len(links_chunk)
-                        data = {'links': links_chunk}
+                        data = {"links": links_chunk}
                         query = (
-                            f'UNWIND $links as row MATCH (a:`{source_label}`), (b:`{target_label}`) '
-                            f"WHERE a.{mid} = row[0] and b.{mid} = row[1] {('CREATE' if create else 'MERGE')} (a)-[:`{rel}`]->(b)")
+                            f"UNWIND $links as row MATCH (a:`{source_label}`), (b:`{target_label}`) "
+                            f"WHERE a.{mid} = row[0] and b.{mid} = row[1] {('CREATE' if create else 'MERGE')} (a)-[:`{rel}`]->(b)"
+                        )
                         neo4j_run_write_query(session, verbose, query, **data)
                         # Update Progress Bar
                         printProgressBar(cnt, item_count)
                     # print new line on complete
                     print()
 
+    # add specified relations
 
-   # add specified relations
-
-    # create indicies on sources and uniqueness constraint on targets of additional relations
+    # create indices on sources and uniqueness constraint on targets of additional relations
     if additional_relations:
         item_count = len(additional_relations)
-        print(f'*** processing {item_count} additional relations')
+        print(f"*** processing {item_count} additional relations")
         # Initial Progress Bar Call
         printProgressBar(0, item_count)
         cnt = 0
         for rel_source, rel_target in additional_relations:
             cnt += 1
             if rel_source[0] in node_label.values() and rel_target[0] in node_label.values():
                 # only process additional relation if nodes in source and target labels exist
-                neo4j_create_index(
-                    session,
-                    verbose,
-                    rel_source[0],
-                    rel_source[1])
-                neo4j_create_index(
-                    session,
-                    verbose,
-                    rel_target[0],
-                    rel_target[1])
-                neo4j_add_relations(session, verbose, chunk_size, apoc_installed, create, rel_source, rel_target)
+                neo4j_create_index(session, verbose, rel_source[0], rel_source[1])
+                neo4j_create_index(session, verbose, rel_target[0], rel_target[1])
+                neo4j_add_relations(
+                    session, verbose, chunk_size, apoc_installed, create, rel_source, rel_target
+                )
             # Update Progress Bar
             printProgressBar(cnt, item_count)
         # print new line on complete
         print()
 
     if additional_list_relations:
         item_count = len(additional_list_relations)
-        print(f'*** processing {item_count} additional list relations')
+        print(f"*** processing {item_count} additional list relations")
         # Initial Progress Bar Call
         printProgressBar(0, item_count)
         cnt = 0
         for rel_source, rel_target in additional_list_relations:
             cnt += 1
             if rel_source[0] in node_label.values() and rel_target[0] in node_label.values():
                 # only process additional list relation if nodes in source and target labels exist
-                neo4j_create_index(
-                    session,
-                    verbose,
-                    rel_source[0],
-                    rel_source[1])
-                neo4j_create_index(
+                neo4j_create_index(session, verbose, rel_source[0], rel_source[1])
+                neo4j_create_index(session, verbose, rel_target[0], rel_target[1])
+                neo4j_add_relations(
                     session,
                     verbose,
-                    rel_target[0],
-                    rel_target[1])
-                neo4j_add_relations(session, verbose, chunk_size, apoc_installed, create, rel_source, rel_target, list_source=True)
+                    chunk_size,
+                    apoc_installed,
+                    create,
+                    rel_source,
+                    rel_target,
+                    list_source=True,
+                )
             # Update Progress Bar
             printProgressBar(cnt, item_count)
         # print new line on complete
         print()
 
-
     # add sublabels
 
     # we only generate sublabels for active collections
     sublabels = [sl for sl in sublabels if sl[0] in active_collections]
     if len(sublabels) > 0:
         established_sublabels: set[str] = set()
         sub_label_specs: dict[str, list[SubSpec]] = {}
         # extract distinct values, type and postfix per sublabel item and associate it with label in sub_label_spec
-        for (label, discriminator, postfix, others) in sublabels:
+        for label, discriminator, postfix, others in sublabels:
             # distinct values, without None and the empty string
-            distinct_values: set[Any] = set(database[label].distinct(discriminator)).difference({None, ''})
-            sub_label_spec_item: None|SubSpec = None
-            if (all(isinstance(item, bool) for item in distinct_values) and
-                    True in distinct_values):
-                discriminator_postfix:str = discriminator + postfix
-                if (discriminator_postfix not in active_collections and
-                    discriminator_postfix not in established_sublabels):
+            distinct_values: set[Any] = set(database[label].distinct(discriminator)).difference(
+                {None, ""}
+            )
+            sub_label_spec_item: None | SubSpec = None
+            if all(isinstance(item, bool) for item in distinct_values) and True in distinct_values:
+                discriminator_postfix: str = discriminator + postfix
+                if (
+                    discriminator_postfix not in active_collections
+                    and discriminator_postfix not in established_sublabels
+                ):
                     # we use only the discriminator+prefix as sublabel for boolean typed discriminators
                     sub_label_spec_item = SubSpec(
-                        discriminator=discriminator,
-                        postfix=postfix,
-                        others=others,
-                        value_type=bool)
+                        discriminator=discriminator, postfix=postfix, others=others, value_type=bool
+                    )
                     # remember newly created (sub-)label
                     established_sublabels.add(discriminator_postfix)
                 else:
-                    print(f'sublabel {label}.{discriminator}{("" if postfix == "" else "."+postfix)} skipped')
-            elif (1 < len(distinct_values) < 50 and
-                    all(isinstance(item, str) for item in distinct_values)):
+                    print(
+                        f'sublabel {label}.{discriminator}{("" if postfix == "" else "."+postfix)} skipped'
+                    )
+            elif 1 < len(distinct_values) < 150 and all(
+                isinstance(item, str) for item in distinct_values
+            ):
                 distinct_values_postfix: list[str] = [str(s) + postfix for s in distinct_values]
-                if (not active_collections.intersection(distinct_values_postfix) and
-                    not established_sublabels.intersection(distinct_values_postfix)):
+                if not active_collections.intersection(
+                    distinct_values_postfix
+                ) and not established_sublabels.intersection(distinct_values_postfix):
                     sub_label_spec_item = SubSpec(
                         discriminator=discriminator,
                         postfix=postfix,
                         others=others,
                         value_type=(list if (discriminator in array_fields) else str),
-                        distinct_values=distinct_values)
+                        distinct_values=distinct_values,
+                    )
                     # remember newly created (sub-)label
-                    new_sublabels: list[str] = [item for sublist in [[f'{l}{postfix}' for l in sl.split('#')] for sl in distinct_values] for item in sublist]
+                    new_sublabels: list[str] = [
+                        item
+                        for sublist in [
+                            [f"{l}{postfix}" for l in sl.split("#")] for sl in distinct_values
+                        ]
+                        for item in sublist
+                    ]
                     new_sublabels.append(discriminator)
                     established_sublabels.update(new_sublabels)
                 else:
-                    print(f'sublabel {label}.{discriminator}{("" if postfix == "" else "."+postfix)} skipped')
-                    print('established_sublabels',established_sublabels)
+                    print(
+                        f'sublabel {label}.{discriminator}{("" if postfix == "" else "."+postfix)} skipped'
+                    )
             if sub_label_spec_item is not None:
                 if label in sub_label_specs:
                     sub_label_specs[label].append(sub_label_spec_item)
                 else:
                     sub_label_specs[label] = [sub_label_spec_item]
 
-        item_count = len(sub_label_specs.items())
-        if item_count > 0:
-            print(f'*** processing {item_count} sublabels')
+        if (item_count := len(sub_label_specs.items())) > 0:
+            print(f"*** processing {item_count} sublabels")
             # Initial Progress Bar Call
             printProgressBar(0, item_count)
             cnt = 0
             for label, sub_specs in sub_label_specs.items():
                 cnt += 1
-                multiple_sublabels: bool = len([ss for ss in sub_specs if ss['value_type'] != bool]) > 1
                 for sub_spec in sub_specs:
-                    if sub_spec['value_type'] is bool:
-                        discriminator = sub_spec['discriminator']
+                    if sub_spec["value_type"] is bool:
+                        discriminator = sub_spec["discriminator"]
                         neo4j_create_index(session, verbose, label, discriminator)
-                        neo4j_add_sublabel(session, verbose, chunk_size, apoc_installed, label, discriminator, 'true', [f'{discriminator}{sub_spec["postfix"]}'])
-                        neo4j_add_sublabel_other(session, verbose, chunk_size, apoc_installed, label, discriminator, sub_spec['others'])
-                    elif sub_spec['value_type'] in [str, list]:
+                        neo4j_add_sublabel(
+                            session,
+                            verbose,
+                            chunk_size,
+                            apoc_installed,
+                            label,
+                            discriminator,
+                            "true",
+                            [f'{discriminator}{sub_spec["postfix"]}'],
+                        )
+                        neo4j_add_sublabel_other(
+                            session,
+                            verbose,
+                            chunk_size,
+                            apoc_installed,
+                            label,
+                            discriminator,
+                            sub_spec["others"],
+                        )
+                    elif sub_spec["value_type"] in [str, list]:
                         # first establish index on the discriminator
-                        isarray: bool = sub_spec['value_type'] is list
-                        discriminator = sub_spec['discriminator']
+                        isarray: bool = sub_spec["value_type"] is list
+                        discriminator = sub_spec["discriminator"]
                         if not isarray:
                             # for fields of type list the index is not effective
                             neo4j_create_index(session, verbose, label, discriminator)
-                        if 'distinct_values' in sub_spec:
-                            for sl in sub_spec['distinct_values']:
+                        if "distinct_values" in sub_spec:
+                            for sl in sub_spec["distinct_values"]:
                                 # add sublabels
-                                labels: list[str] = [f'{l}{sub_spec["postfix"]}' for l in sl.split('#')]
-                                if multiple_sublabels:
-                                    labels.append(discriminator)
-                                neo4j_add_sublabel(session, verbose, chunk_size, apoc_installed, label, discriminator, f"'{sl}'", labels, isarray)
-                            neo4j_add_sublabel_other(session, verbose, chunk_size, apoc_installed, label, discriminator, sub_spec['others'])
+                                labels: list[str] = [
+                                    f'{l}{sub_spec["postfix"]}' for l in sl.split("#")
+                                ]
+                                neo4j_add_sublabel(
+                                    session,
+                                    verbose,
+                                    chunk_size,
+                                    apoc_installed,
+                                    label,
+                                    discriminator,
+                                    f"'{sl}'",
+                                    labels,
+                                    isarray,
+                                )
+                            neo4j_add_sublabel_other(
+                                session,
+                                verbose,
+                                chunk_size,
+                                apoc_installed,
+                                label,
+                                discriminator,
+                                sub_spec["others"],
+                            )
                 # Update Progress Bar
                 printProgressBar(cnt, item_count)
             # print new line on complete
             print()
 
 
 # pylint: disable=too-many-locals
 def main(
-        mongo_host: str,
-        mongo_port: int,
-        mongo_db: str,
-        neo4j_host: str,
-        neo4j_port: int,
-        neo4j_user: str,
-        neo4j_password: str,
-        neo4j_db: str,
-        chunk_size: int,
-        excluded_collections: Collections,
-        included_collections: None | Collections,
-        excluded_fields: Fields,
-        sublabels: SubLabels,
-        relations: RelationSpecifications,
-        list_relations: RelationSpecifications,
-        create: bool = False,
-        verbose: bool = False,
-        simulate: bool = False) -> int:
+    mongo_host: str,
+    mongo_port: int,
+    mongo_db: str,
+    neo4j_host: str,
+    neo4j_port: int,
+    neo4j_user: str,
+    neo4j_password: str,
+    neo4j_db: str,
+    chunk_size: int,
+    excluded_collections: Collections,
+    included_collections: None | Collections,
+    excluded_fields: Fields,
+    sublabels: SubLabels,
+    relations: RelationSpecifications,
+    list_relations: RelationSpecifications,
+    create: bool = False,
+    verbose: bool = False,
+    simulate: bool = False,
+) -> int:
     """The main mongo2neo4j function that takes MongoDB credential and DB name, Neo4j credentials \
         and DB name and a specification which MongoDB collections and attributes should be \
         transferred to Neo4j, if the Cypher queries should be printed to stdout (verbose=True) \
         and if the Neo4j engine should be connected to or not (simulate=True)."""
 
     # connect to MongDB
-    mongo_client: MongoClient = MongoClient(mongo_host, mongo_port)
+    mongo_client: MongoClient[Any] = MongoClient(mongo_host, mongo_port)
     # get MongoDB DB
-    database: 'Database' = mongo_client[mongo_db]
+    database: "Database[Any]" = mongo_client[mongo_db]
 
     try:
         db_collections: list[str] = database.list_collection_names()
         collections: Collections = (
             set(db_collections)
             if included_collections is None
-            else set(included_collections).intersection(db_collections))
+            else set(included_collections).intersection(db_collections)
+        )
 
         if simulate:
             process_data(
                 database,
                 None,
                 collections,
                 excluded_collections,
                 excluded_fields,
                 sublabels,
                 relations,
                 list_relations,
                 create,
                 verbose,
-                chunk_size)
+                chunk_size,
+            )
         else:
             driver: Driver
             with GraphDatabase.driver(  # pylint: disable=not-context-manager
-                    f'neo4j://{neo4j_host}:{neo4j_port}',
-                    auth=(neo4j_user, neo4j_password)) as driver:
+                f"neo4j://{neo4j_host}:{neo4j_port}",
+                auth=(neo4j_user, neo4j_password),
+                telemetry_disabled=True,
+            ) as driver:
                 session: Session
                 with driver.session(database=neo4j_db) as session:
                     process_data(
                         database,
                         session,
                         collections,
                         excluded_collections,
                         excluded_fields,
                         sublabels,
                         relations,
                         list_relations,
                         create,
                         verbose,
-                        chunk_size)
+                        chunk_size,
+                    )
         return 0
     except AuthError:
-        print('Neo4j authentication failed')
+        print("Neo4j authentication failed")
     except ServerSelectionTimeoutError:
-        print('MongoDB connection error')
+        print("MongoDB connection error")
     except PyMongoError as e:
-        print('MongoDB error', e)
+        print("MongoDB error", e)
     except Neo4jError as e:
-        print('Neo4j error', e)
+        print("Neo4j error", e)
     return -1
 
 
-def console_main() -> int:
+def console_main() -> int:  # pylint: disable=too-complex
     """The CLI entry point of mongo2neo4j.
 
     This function is not meant for programmable use; use `main()` instead.
     """
     # https://docs.python.org/3/library/signal.html#note-on-sigpipe
     try:
-        parser = argparse.ArgumentParser(description=f'mongo2neo4j v{__version__}: {__doc__}')
-        mongo_group = parser.add_argument_group('MongoDB connection')
+        parser = argparse.ArgumentParser(description=f"mongo2neo4j v{__version__}: {__doc__}")
+        mongo_group = parser.add_argument_group("MongoDB connection")
         mongo_group.add_argument(
-            '-mh',
-            '--mongo_host',
-            dest='mongo_host',
+            "-mh",
+            "--mongo_host",
+            dest="mongo_host",
             type=str,
-            default='localhost',
-            help='MongoDB simple hostname or a full MongoDB URI of the form mongodb://<user>:<password>@<host>:<port>. Unix domain sockets with percent encoded socket path in the URI.')
+            default="localhost",
+            help="MongoDB simple hostname or a full MongoDB URI of the form mongodb://<user>:<password>@<host>:<port>. Unix domain sockets with percent encoded socket path in the URI.",
+        )
         mongo_group.add_argument(
-            '-mp',
-            '--mongo_port',
-            dest='mongo_port',
-            type=int,
-            default='27017',
-            help='MongoDB port')
+            "-mp", "--mongo_port", dest="mongo_port", type=int, default="27017", help="MongoDB port"
+        )
 
-        neo4j_group = parser.add_argument_group('Neo4j connection')
+        neo4j_group = parser.add_argument_group("Neo4j connection")
         neo4j_group.add_argument(
-            '-nh',
-            '--neo4j_host',
-            dest='neo4j_host',
+            "-nh",
+            "--neo4j_host",
+            dest="neo4j_host",
             type=str,
-            default='localhost',
-            help='Neo4j hostname')
+            default="localhost",
+            help="Neo4j hostname",
+        )
         neo4j_group.add_argument(
-            '-np',
-            '--neo4j_port',
-            dest='neo4j_port',
-            type=int,
-            default='7687',
-            help='Neo4j port')
+            "-np", "--neo4j_port", dest="neo4j_port", type=int, default="7687", help="Neo4j port"
+        )
         neo4j_group.add_argument(
-            '-nu',
-            '--neo4j_user',
-            dest='neo4j_user',
-            type=str,
-            default='neo4j',
-            help='Neo4j user')
+            "-nu", "--neo4j_user", dest="neo4j_user", type=str, default="neo4j", help="Neo4j user"
+        )
         neo4j_group.add_argument(
-            '-npw',
-            '--neo4j_password',
-            dest='neo4j_password',
-            type=str,
-            help='Neo4j password')
+            "-npw", "--neo4j_password", dest="neo4j_password", type=str, help="Neo4j password"
+        )
         neo4j_group.add_argument(
-            '-nd', '--neo4j_db',
-            dest='neo4j_db',
-            type=str,
-            help='Neo4j DB to import into')
+            "-nd", "--neo4j_db", dest="neo4j_db", type=str, help="Neo4j DB to import into"
+        )
 
-
-        mapping_group = parser.add_argument_group('Mapping')
+        mapping_group = parser.add_argument_group("Mapping")
         mapping_group.add_argument(
-            '-i',
-            '--include',
-            dest='included_collections',
-            action='append',
-            help='Comma separated collections to be transferred. If not specified, transfer all not excluded ones')
+            "-i",
+            "--include",
+            dest="included_collections",
+            action="append",
+            help="Comma separated collections to be transferred. If not specified, transfer all not excluded ones",
+        )
         mapping_group.add_argument(
-            '-x',
-            '--exclude',
-            dest='excluded_collections',
-            action='append',
+            "-x",
+            "--exclude",
+            dest="excluded_collections",
+            action="append",
             default=[],
-            help='Comma separated collections to be excluded. Collection names can have a * at the begin or end to match multiple collections.')
+            help="Comma separated collections to be excluded. Collection names can have a * at the begin or end to match multiple collections.",
+        )
         mapping_group.add_argument(
-            '-f',
-            '--exclude_fields',
-            dest='excluded_fields',
-            action='append',
+            "-f",
+            "--exclude_fields",
+            dest="excluded_fields",
+            action="append",
             default=[],
-            help='Comma separated fields to be ignored. Field names can have a * at the begin or end to match multiple fields.')
+            help="Comma separated fields to be ignored. Field names can have a * at the begin or end to match multiple fields.",
+        )
         mapping_group.add_argument(
-            '-sl',
-            '--sublabels',
-            dest='sublabels',
-            action='append',
+            "-sl",
+            "--sublabels",
+            dest="sublabels",
+            action="append",
             default=[],
-            help='List of <collection>.<attrib>[.<postfix>][,<others>] fields of type string or list of strings to create sublabels. The optional <postfix> is added to the generated sublabel and if <others> is given it is used to collect nodes without proper value.')
+            help="List of <collection>.<attrib>[.<postfix>][,<others>] fields of type string or list of strings to create sublabels. The optional <postfix> is added to the generated sublabel and if <others> is given it is used to collect nodes without proper value.",
+        )
         mapping_group.add_argument(
-            '-r',
-            '--relations',
-            dest='relations',
-            action='append',
+            "-r",
+            "--relations",
+            dest="relations",
+            action="append",
             default=[],
-            help='List of <Collection>.<attrib>,<collection>.<attrib> tuples to relations between nodes of equal str/number values')
+            help="List of <Collection>.<attrib>,<collection>.<attrib> tuples to relations between nodes of equal str/number values",
+        )
         mapping_group.add_argument(
-            '-lr',
-            '--list_relations',
-            dest='list_relations',
-            action='append',
+            "-lr",
+            "--list_relations",
+            dest="list_relations",
+            action="append",
             default=[],
-            help='List of <collection>.<attrib>,<collection>.<attrib> tuples to relations between nodes of list of str/number values and str/number values')
+            help="List of <collection>.<attrib>,<collection>.<attrib> tuples to relations between nodes of list of str/number values and str/number values",
+        )
 
+        parser.add_argument("--conf_export", action="store_true", help="Dump config and exit")
+        parser.add_argument("--conf", action="append", help="Read config file")
+        parser.add_argument("-v", "--verbose", action="store_true", help="Output Cypher")
+        parser.add_argument("-s", "--simulate", action="store_true", help="Don't connect to Neo4j")
         parser.add_argument(
-            '--conf_export',
-            action='store_true',
-            help='Dump config and exit')
-        parser.add_argument(
-            '--conf',
-            action='append',
-            help='Read config file')
-        parser.add_argument('-v', '--verbose', action='store_true', help='Output Cypher')
-        parser.add_argument(
-            '-s', '--simulate', action='store_true', help="Don't connect to Neo4j")
-        parser.add_argument(
-            '-c',
-            '--create',
-            action='store_true',
-            help='Use CREATE instead of MERGE to create objects in Neo4j')
+            "-c",
+            "--create",
+            action="store_true",
+            help="Use CREATE instead of MERGE to create objects in Neo4j",
+        )
 
         parser.add_argument(
-            '-k',
-            '--chunk_size',
-            dest='chunk_size',
+            "-k",
+            "--chunk_size",
+            dest="chunk_size",
             type=int,
-            default='500',
-            help='processing objects chunk size')
+            default="500",
+            help="processing objects chunk size",
+        )
 
-        parser.add_argument('mongo_db', help='MongoDB DB to be imported')
+        parser.add_argument("mongo_db", help="MongoDB DB to be imported")
         args = parser.parse_args()
 
-        print(f'mongo2neo4j v{__version__}')
+        print(f"mongo2neo4j v{__version__}")
 
         # load config file
-        if args.conf is None and os.path.isfile('mongo2neo4j.conf'):
+        if args.conf is None and os.path.isfile("mongo2neo4j.conf"):
             # by default we load a config from mongo2neo4j.conf if nothing else is specified and that file exists
-            args.conf = ['mongo2neo4j.conf']
+            args.conf = ["mongo2neo4j.conf"]
         if args.conf is not None:
             for conf_fname in args.conf:
                 try:
-                    with open(conf_fname, encoding='utf-8') as f:
+                    with open(conf_fname, encoding="utf-8") as f:
                         parser.set_defaults(**json.load(f))
                 except FileNotFoundError:
                     print(f'config file "{conf_fname}" not found')
                     sys.exit(-1)
 
         # Reload arguments to override config file values with command line values
         args = parser.parse_args()
 
         # dump config
         if args.conf_export:
             tmp_args = vars(args).copy()
-            del tmp_args['conf_export']  # Do not dump value of conf_export flag
-            del tmp_args['conf']  # Values already loaded
-            print(json.dumps(tmp_args,  indent=4, sort_keys=True))
+            del tmp_args["conf_export"]  # Do not dump value of conf_export flag
+            del tmp_args["conf"]  # Values already loaded
+            print(json.dumps(tmp_args, indent=4, sort_keys=True))
             sys.exit(-1)
 
         requested_collections: None | Collections = None
         if args.included_collections is not None:
             requested_collections = set()
             for c in args.included_collections:
-                for s in c.split(','):
+                for s in c.split(","):
                     requested_collections.add(s)
         args_excluded_collections: Collections = default_exclude_collections
         for c in args.excluded_collections:
-            for s in c.split(','):
+            for s in c.split(","):
                 args_excluded_collections.add(s)
         args_excluded_fields: Fields = default_fields_to_remove
         if args.excluded_fields is not None:
             for fields in args.excluded_fields:
-                for f in fields.split(','):
+                for f in fields.split(","):
                     args_excluded_fields.add(str(f))
 
         start = time.perf_counter()
         res = main(
-                args.mongo_host,
-                args.mongo_port,
-                args.mongo_db,
-                args.neo4j_host,
-                args.neo4j_port,
-                args.neo4j_user,
-                args.neo4j_password,
-                args.neo4j_db,
-                args.chunk_size,
-                args_excluded_collections,
-                requested_collections,
-                args_excluded_fields,
-                strlist2subLabels(args.sublabels),
-                strlist2relationSpecifications(args.relations),
-                strlist2relationSpecifications(args.list_relations),
-                args.create,
-                args.verbose,
-                args.simulate)
+            args.mongo_host,
+            args.mongo_port,
+            args.mongo_db,
+            args.neo4j_host,
+            args.neo4j_port,
+            args.neo4j_user,
+            args.neo4j_password,
+            args.neo4j_db,
+            args.chunk_size,
+            args_excluded_collections,
+            requested_collections,
+            args_excluded_fields,
+            strlist2subLabels(args.sublabels),
+            strlist2relationSpecifications(args.relations),
+            strlist2relationSpecifications(args.list_relations),
+            args.create,
+            args.verbose,
+            args.simulate,
+        )
         end = time.perf_counter()
-        print(f'total runtime: {str(datetime.timedelta(seconds=end-start)).split(".", maxsplit=1)[0]}')
+        print(
+            f'total runtime: {str(datetime.timedelta(seconds=end-start)).split(".", maxsplit=1)[0]}'
+        )
         sys.stdout.flush()
         return res
     except BrokenPipeError:
         # Python flushes standard streams on exit; redirect remaining output
         # to devnull to avoid another BrokenPipeError at shutdown
         devnull = os.open(os.devnull, os.O_WRONLY)
         os.dup2(devnull, sys.stdout.fileno())
         return 1  # Python exits with error code 1 on EPIPE
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     sys.exit(console_main())
```

### Comparing `mongo2neo4j-0.5.0/src/mongo2neo4j.egg-info/PKG-INFO` & `mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo2neo4j
-Version: 0.5.0
+Version: 1.0.0
 Summary: Imports object structures generated by MongoDB object relation mappers (like Mongoose) into Neo4j for exploration with SemSpect
 Author: Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,14 +684,28 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymongo>=4.6.3
+Requires-Dist: neo4j>=5.19.0
+Provides-Extra: dev
+Requires-Dist: mypy>=1.9.0; extra == "dev"
+Requires-Dist: pyright>=1.1.359; extra == "dev"
+Requires-Dist: ruff>=0.3.7; extra == "dev"
+Requires-Dist: pylint>=3.1.0; extra == "dev"
+Requires-Dist: pytest>=8.1.1; extra == "dev"
+Requires-Dist: pytest-cov>=5.0.0; extra == "dev"
+Requires-Dist: coverage-badge>=1.1.0; extra == "dev"
+Requires-Dist: pre-commit>=3.7.0; extra == "dev"
+Requires-Dist: twine>=5.0.0; extra == "dev"
+Requires-Dist: build>=1.2.1; extra == "dev"
+Requires-Dist: codespell>=2.2.6; extra == "dev"
 
 # [mongo2neo4j](https://makomo.github.io/mongo2neo4j/)
 
 [MongoDB](https://www.mongodb.com/) [Mongoose](https://mongoosejs.com/) to [Neo4j](https://neo4j.com/) Importer
 
 ![License](https://img.shields.io/github/license/MAKOMO/mongo2neo4j.svg)
 [![Pylint](https://github.com/MAKOMO/mongo2neo4j/actions/workflows/pylint.yaml/badge.svg)](https://github.com/MAKOMO/mongo2neo4j/actions/workflows/pylint.yaml)
@@ -752,13 +766,13 @@
 
 Further configuration options are listed on calling
 
 ```sh
 % mongo2neo4j -h
 ```
 
-See [Script Arguments](https://github.com/MAKOMO/mongo2neo4j/wiki/Script-Arguments) for the full list of available arguments and the [example](example/README.md) documenting the workflow of mongo2neo4j using randomly generated sample data.
+See [Script Arguments](https://github.com/MAKOMO/mongo2neo4j/wiki/Script-Arguments) for the full list of available arguments and the [example](https://github.com/MAKOMO/mongo2neo4j/blob/main/example/README.md) documenting the workflow of mongo2neo4j using randomly generated sample data.
 
 
 
 
 NOTE: *if the [APOC plugin](https://neo4j.com/docs/apoc/) is installed in the Neo4j DB, the faster and memory-effective `apoc.periodic.iterate` method is used to generate nodes and sublabels.*
```

### Comparing `mongo2neo4j-0.5.0/tests/test_flatten_and_cleanse.py` & `mongo2neo4j-1.0.0/tests/test_flatten_and_cleanse.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,109 +4,109 @@
 
 class TestFlattenAndCleanseSubObjects:
 
     mid = '_id'
 
     def test_simple_values(self):
         """the sub object is flattend"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'sub': {
                 'a': 1,
                 'b': 2
             }
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == { self.mid: '6477dcd14ff2e36571d60890', 'sub_a': 1, 'sub_b': 2}
-        assert relations == {}
+        assert not relations
         assert array_fields == set()
-        assert objects == {}
+        assert not objects
 
     def test_simple_values_with_id(self):
         """the sub object is generated and linked"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'k': 0,
             'sub': {
                 self.mid: ObjectId('6477dcd14ff2e36571d60891'),
                 'a': 1,
                 'b': 2
             }
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == { self.mid: '6477dcd14ff2e36571d60890', 'k': 0}
         assert relations == { 'sub': {('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60891')}}
         assert array_fields == set()
         assert objects == {'super_sub': [{self.mid: '6477dcd14ff2e36571d60891', 'a': 1, 'b': 2}]}
 
     def test_sequence_numbers(self):
         """the sub object is flattend"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'k': 0,
             'sub': {
                 'l': [0, 1, 2],
                 'm': 1
             }
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == {self.mid: '6477dcd14ff2e36571d60890', 'k': 0, 'sub_l': [0, 1, 2], 'sub_m': 1}
-        assert relations == {}
+        assert not relations
         assert array_fields == set()
-        assert objects == {}
+        assert not objects
 
     def test_sequence_strings(self):
         """the sub object is flattend and sub_l is marked as array field to allow for generation of sublabels"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'k': 0,
             'sub': {
                 'l': ['a', 'b', 'c'],
                 'm': 1
             }
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == {self.mid: '6477dcd14ff2e36571d60890', 'k': 0, 'sub_l': ['a', 'b', 'c'], 'sub_m': 1}
-        assert relations == {}
+        assert not relations
         assert array_fields == {'sub_l'}
-        assert objects == {}
+        assert not objects
 
     def test_sequence_ids(self):
         """the sub objects are generated and linked"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'k': 0,
             'sub': {
                 'l': [ObjectId('6477dcd14ff2e36571d60892'), ObjectId('6477dcd14ff2e36571d60894')],
                 'm': 1
             }
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == {self.mid: '6477dcd14ff2e36571d60890', 'k': 0, 'sub_m': 1}
         assert relations == {'sub_l': {('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60892'), ('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60894')}}
         assert array_fields == set()
-        assert objects == {}
+        assert not objects
 
     def test_sequence_objects(self):
         """sub sub objects are generated with fresh ids and linked"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'k': 0,
             'sub': {
                 'l': [
                     { 'x': 0 },
                     { 'x': 1 }
                 ],
                 'm': 1
             }
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == {self.mid: '6477dcd14ff2e36571d60890', 'k': 0, 'sub_m': 1}
         # relations: {'sub_l': [('6477dcd14ff2e36571d60890', '0303b7e9b84f41e9bdb09db2e187a8d8'), ('6477dcd14ff2e36571d60890', '8e8cbc0d44d349c88f1f2df20f8458aa')]}
-        assert ('sub_l' in relations) == True
+        assert ('sub_l' in relations) is True
         links = relations['sub_l']
         assert len(links) == 2
         assert {l[0] for l in links} == {'6477dcd14ff2e36571d60890'}
         assert array_fields == set()
         # objects: {'super_sub_l': [{'x': 0, '_id': '0303b7e9b84f41e9bdb09db2e187a8d8'}, {'x': 1, '_id': '8e8cbc0d44d349c88f1f2df20f8458aa'}]}
         assert 'super_sub_l' in objects
         sub_objects = objects['super_sub_l']
@@ -115,26 +115,26 @@
         assert sub_objects[1]['x'] == 1
         linked_objects = [l[1] for l in links]
         assert sub_objects[0][self.mid] in linked_objects
         assert sub_objects[1][self.mid] in linked_objects
 
     def test_sequence_id_objects(self):
         """sub sub objects are generated using the given ids and linked"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'k': 0,
             'sub': {
                 'l': [
                     { self.mid: ObjectId('6477dcd14ff2e36571d60892'), 'x': 0 },
                     { self.mid: ObjectId('6477dcd14ff2e36571d60894'), 'x': 1 }
                 ],
                 'm': 1
             }
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == {self.mid: '6477dcd14ff2e36571d60890', 'k': 0, 'sub_m': 1}
         # relations: {'sub_l': [('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60892'), ('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60894')]}
         links = relations['sub_l']
         assert len(links) == 2
         assert {l[0] for l in links} == {'6477dcd14ff2e36571d60890'}
         assert array_fields == set()
         # {'super_sub_l': [{'_id': '6477dcd14ff2e36571d60892', 'x': 0}, {'_id': '6477dcd14ff2e36571d60894', 'x': 1}]}
@@ -151,46 +151,46 @@
 
 class TestFlattenAndCleanseSubSequences:
 
     mid = '_id'
 
     def test_simple_values(self):
         """the sub object is flattend"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'l': [0, 1, 2]
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == { self.mid: '6477dcd14ff2e36571d60890', 'l': [0, 1, 2]}
-        assert relations == {}
+        assert not relations
         assert array_fields == set()
-        assert objects == {}
+        assert not objects
 
     def test_ids(self):
         """the sub object is flattend"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'l': [ObjectId('6477dcd14ff2e36571d60892'), ObjectId('6477dcd14ff2e36571d60894')]
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == { self.mid: '6477dcd14ff2e36571d60890' }
         assert relations == {'l': {('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60892'), ('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60894')}}
         assert array_fields == set()
-        assert objects == {}
+        assert not objects
 
     def test_objects(self):
         """the sub object is flattend"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'l': [ {'x': 0 }, {'x': 1}]
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == { self.mid: '6477dcd14ff2e36571d60890' }
         # relations: {'l': [('6477dcd14ff2e36571d60890', '0bbed9a55ca1409088521b7927b615e9'), ('6477dcd14ff2e36571d60890', '3eebc1d7b1c14485a85e53ef05734749')]}
-        assert ('l' in relations) == True
+        assert ('l' in relations) is True
         links = relations['l']
         assert len(links) == 2
         assert {l[0] for l in links} == {'6477dcd14ff2e36571d60890'}
         assert array_fields == set()
         # objects: {'super_l': [{self.mid: '0bbed9a55ca1409088521b7927b615e9', 'x': 0}, {self.mid: '3eebc1d7b1c14485a85e53ef05734749', 'x': 1}]}
         assert 'super_l' in objects
         sub_objects = objects['super_l']
@@ -199,21 +199,21 @@
         assert sub_objects[1]['x'] == 1
         linked_objects = [l[1] for l in links]
         assert sub_objects[0][self.mid] in linked_objects
         assert sub_objects[1][self.mid] in linked_objects
 
     def test_objects_with_ids(self):
         """the sub object is flattend"""
-        super = {
+        super_dict = {
             self.mid: ObjectId('6477dcd14ff2e36571d60890'),
             'l': [ {self.mid: ObjectId('6477dcd14ff2e36571d60892'), 'x': 0 }, {self.mid: ObjectId('6477dcd14ff2e36571d60894'), 'x': 1}]
         }
-        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super, [], [], [])
+        res, relations, array_fields, objects = mongo2neo4j.flatten_and_cleanse('super', super_dict, [], [], [])
         assert res == { self.mid: '6477dcd14ff2e36571d60890' }
         # relations: {'l': [('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60892'), ('6477dcd14ff2e36571d60890', '6477dcd14ff2e36571d60894')]}
-        assert ('l' in relations) == True
+        assert ('l' in relations) is True
         links = relations['l']
         assert len(links) == 2
         assert {l[0] for l in links} == {'6477dcd14ff2e36571d60890'}
         assert array_fields == set()
         # objects: {'super_l': [{'_id': '6477dcd14ff2e36571d60892', 'x': 0}, {'_id': '6477dcd14ff2e36571d60894', 'x': 1}]}
         assert objects == {'super_l': [{'_id': '6477dcd14ff2e36571d60892', 'x': 0}, {'_id': '6477dcd14ff2e36571d60894', 'x': 1}]}
```

