# Comparing `tmp/owlapy-0.1.3.tar.gz` & `tmp/owlapy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlapy-0.1.3.tar", last modified: Wed Apr 10 10:55:17 2024, max compression
+gzip compressed data, was "owlapy-1.0.0.tar", last modified: Fri Apr 19 11:40:23 2024, max compression
```

## Comparing `owlapy-0.1.3.tar` & `owlapy-1.0.0.tar`

### file list

```diff
@@ -1,55 +1,51 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/
--rw-rw-r--   0 demir     (1000) demir     (1000)     1056 2024-03-25 12:18:36.000000 owlapy-0.1.3/LICENSE
--rw-r--r--   0 demir     (1000) demir     (1000)     3602 2024-04-10 10:55:17.138621 owlapy-0.1.3/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     2922 2024-04-10 10:54:54.000000 owlapy-0.1.3/README.md
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.134621 owlapy-0.1.3/owlapy/
--rw-rw-r--   0 demir     (1000) demir     (1000)       22 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      419 2024-03-25 12:18:36.000000 owlapy-0.1.3/owlapy/_utils.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.134621 owlapy-0.1.3/owlapy/class_expression/
--rw-rw-r--   0 demir     (1000) demir     (1000)     2206 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     3206 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/class_expression.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1473 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/nary_boolean_expression.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1483 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/owl_class.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    25473 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/restriction.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/data_ranges/
--rw-rw-r--   0 demir     (1000) demir     (1000)     2683 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/data_ranges/__init__.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/entities/
--rw-rw-r--   0 demir     (1000) demir     (1000)      485 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/entities/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      290 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/has.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     5347 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/iri.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1771 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/meta_classes.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/model/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35363 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/model/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2784 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/model/providers.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1288 2024-03-25 12:18:36.000000 owlapy-0.1.3/owlapy/namespaces.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/owl2sparql/
--rw-rw-r--   0 demir     (1000) demir     (1000)       31 2024-04-08 17:49:23.000000 owlapy-0.1.3/owlapy/owl2sparql/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    24053 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl2sparql/converter.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1443 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_annotation.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    43211 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_axiom.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1115 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_individual.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    15935 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_literal.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     6005 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_property.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2466 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owlobject.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    36488 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/parser.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    15925 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/render.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      795 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/types.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    21630 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/util.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     4389 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/vocab.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.134621 owlapy-0.1.3/owlapy.egg-info/
--rw-r--r--   0 demir     (1000) demir     (1000)     3602 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     1087 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       62 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        7 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/top_level.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       80 2024-03-28 12:08:04.000000 owlapy-0.1.3/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)       38 2024-04-10 10:55:17.138621 owlapy-0.1.3/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)      920 2024-04-10 10:54:54.000000 owlapy-0.1.3/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/tests/
--rw-rw-r--   0 demir     (1000) demir     (1000)     1191 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_class_expression_semantics.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1330 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_examples.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1613 2024-04-08 17:49:23.000000 owlapy-0.1.3/tests/test_owlapy.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    11198 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_cnf_dnf.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    18196 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_nnf.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    30062 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_parser.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     8674 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_render.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.397060 owlapy-1.0.0/
+-rw-rw-rw-   0        0        0     1077 2023-05-27 17:20:12.000000 owlapy-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3808 2024-04-19 11:40:23.396046 owlapy-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3144 2024-04-17 13:17:23.000000 owlapy-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.375542 owlapy-1.0.0/owlapy/
+-rw-rw-rw-   0        0        0      216 2024-04-18 12:50:47.000000 owlapy-1.0.0/owlapy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.384502 owlapy-1.0.0/owlapy/class_expression/
+-rw-rw-rw-   0        0        0     2258 2024-04-17 12:42:17.000000 owlapy-1.0.0/owlapy/class_expression/__init__.py
+-rw-rw-rw-   0        0        0     3657 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/class_expression/class_expression.py
+-rw-rw-rw-   0        0        0     1889 2024-04-15 18:25:40.000000 owlapy-1.0.0/owlapy/class_expression/nary_boolean_expression.py
+-rw-rw-rw-   0        0        0     1653 2024-04-17 12:30:02.000000 owlapy-1.0.0/owlapy/class_expression/owl_class.py
+-rw-rw-rw-   0        0        0    31671 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/class_expression/restriction.py
+-rw-rw-rw-   0        0        0    24825 2024-04-17 11:25:38.000000 owlapy-1.0.0/owlapy/converter.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.386542 owlapy-1.0.0/owlapy/entities/
+-rw-rw-rw-   0        0        0      493 2024-04-10 12:11:02.000000 owlapy-1.0.0/owlapy/entities/__init__.py
+-rw-rw-rw-   0        0        0     5514 2024-04-17 12:42:17.000000 owlapy-1.0.0/owlapy/iri.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 12:42:17.000000 owlapy-1.0.0/owlapy/meta_classes.py
+-rw-rw-rw-   0        0        0     1501 2024-04-11 16:18:42.000000 owlapy-1.0.0/owlapy/namespaces.py
+-rw-rw-rw-   0        0        0     1518 2024-04-17 11:21:40.000000 owlapy-1.0.0/owlapy/owl_annotation.py
+-rw-rw-rw-   0        0        0    56408 2024-04-17 12:10:21.000000 owlapy-1.0.0/owlapy/owl_axiom.py
+-rw-rw-rw-   0        0        0     3402 2024-04-17 14:26:54.000000 owlapy-1.0.0/owlapy/owl_data_ranges.py
+-rw-rw-rw-   0        0        0     1396 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/owl_datatype.py
+-rw-rw-rw-   0        0        0     1306 2024-04-17 12:30:02.000000 owlapy-1.0.0/owlapy/owl_individual.py
+-rw-rw-rw-   0        0        0    16664 2024-04-17 12:48:36.000000 owlapy-1.0.0/owlapy/owl_literal.py
+-rw-rw-rw-   0        0        0     2548 2024-04-17 12:48:36.000000 owlapy-1.0.0/owlapy/owl_object.py
+-rw-rw-rw-   0        0        0     8206 2024-04-17 11:21:41.000000 owlapy-1.0.0/owlapy/owl_ontology.py
+-rw-rw-rw-   0        0        0     5102 2024-04-17 14:11:30.000000 owlapy-1.0.0/owlapy/owl_ontology_manager.py
+-rw-rw-rw-   0        0        0     6334 2024-04-18 14:19:00.000000 owlapy-1.0.0/owlapy/owl_property.py
+-rw-rw-rw-   0        0        0    19537 2024-04-15 19:10:09.000000 owlapy-1.0.0/owlapy/owl_reasoner.py
+-rw-rw-rw-   0        0        0    37465 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/parser.py
+-rw-rw-rw-   0        0        0     2882 2024-04-15 19:24:04.000000 owlapy-1.0.0/owlapy/providers.py
+-rw-rw-rw-   0        0        0    16389 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/render.py
+-rw-rw-rw-   0        0        0    22897 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/util.py
+-rw-rw-rw-   0        0        0     4601 2024-04-17 12:10:21.000000 owlapy-1.0.0/owlapy/vocab.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.394013 owlapy-1.0.0/owlapy.egg-info/
+-rw-rw-rw-   0        0        0     3808 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-11-14 15:09:44.000000 owlapy-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:40:23.397060 owlapy-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-04-18 12:44:58.000000 owlapy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.392823 owlapy-1.0.0/tests/
+-rw-rw-rw-   0        0        0     1045 2024-04-15 19:24:04.000000 owlapy-1.0.0/tests/test_class_expression_semantics.py
+-rw-rw-rw-   0        0        0     1318 2024-04-15 19:24:04.000000 owlapy-1.0.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0     1693 2024-04-15 19:50:32.000000 owlapy-1.0.0/tests/test_owlapy.py
+-rw-rw-rw-   0        0        0    11461 2024-04-15 19:50:32.000000 owlapy-1.0.0/tests/test_owlapy_cnf_dnf.py
+-rw-rw-rw-   0        0        0    18720 2024-04-17 14:24:48.000000 owlapy-1.0.0/tests/test_owlapy_nnf.py
+-rw-rw-rw-   0        0        0    30821 2024-04-17 14:24:48.000000 owlapy-1.0.0/tests/test_owlapy_parser.py
+-rw-rw-rw-   0        0        0     8940 2024-04-17 14:24:48.000000 owlapy-1.0.0/tests/test_owlapy_render.py
```

### Comparing `owlapy-0.1.3/LICENSE` & `owlapy-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `owlapy-0.1.3/owlapy/class_expression/__init__.py` & `owlapy-1.0.0/owlapy/class_expression/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-"""https://www.w3.org/TR/owl2-syntax/#Class_Expressions
-ClassExpression :=
-    owl_class.py:
-    Class
-    nary_boolean_expression.py:
-    ObjectIntersectionOf, ObjectUnionOf
-    class_expression.py: ObjectComplementOf
-
-    restriction.py:
-    ObjectOneOf, ObjectSomeValuesFrom, ObjectAllValuesFrom, ObjectHasValue,ObjectHasSelf,
-    ObjectMinCardinality, ObjectMaxCardinality, ObjectExactCardinality, DataSomeValuesFrom, DataAllValuesFrom,
-    DataHasValue, DataMinCardinality, DataMaxCardinality, DataExactCardinality
-"""
-from .class_expression import OWLClassExpression, OWLAnonymousClassExpression, OWLBooleanClassExpression, \
-    OWLObjectComplementOf
-from .owl_class import OWLClass
-from .nary_boolean_expression import OWLNaryBooleanClassExpression, OWLObjectUnionOf, OWLObjectIntersectionOf
-from .restriction import (OWLRestriction, OWLQuantifiedRestriction, OWLQuantifiedObjectRestriction,
-                          OWLObjectRestriction,
-                          OWLHasValueRestriction, OWLDataRestriction, OWLCardinalityRestriction,
-                          OWLObjectCardinalityRestriction, OWLObjectHasSelf,
-                          OWLDataOneOf, OWLQuantifiedDataRestriction, OWLDataCardinalityRestriction,
-                          OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, OWLObjectHasValue,
-                          OWLDatatypeRestriction, OWLFacet, OWLFacetRestriction,
-                          OWLObjectMinCardinality,
-                          OWLObjectMaxCardinality,
-                          OWLObjectExactCardinality,
-                          OWLDataSomeValuesFrom,
-                          OWLDataAllValuesFrom,
-                          OWLDataHasValue,
-                          OWLDataMinCardinality,
-                          OWLDataMaxCardinality,
-                          OWLDataExactCardinality,
-                          OWLObjectOneOf
-                          )
-from typing import Final
-from ..vocab import OWLRDFVocabulary
-
-OWLThing: Final = OWLClass(OWLRDFVocabulary.OWL_THING.get_iri())  #: : :The OWL Class corresponding to owl:Thing
-OWLNothing: Final = OWLClass(OWLRDFVocabulary.OWL_NOTHING.get_iri())  #: : :The OWL Class corresponding to owl:Nothing
+""" OWL Class Expressions
+https://www.w3.org/TR/owl2-syntax/#Class_Expressions
+ClassExpression :=
+    owl_class.py:
+    Class
+    nary_boolean_expression.py:
+    ObjectIntersectionOf, ObjectUnionOf
+    class_expression.py: ObjectComplementOf
+
+    restriction.py:
+    ObjectOneOf, ObjectSomeValuesFrom, ObjectAllValuesFrom, ObjectHasValue,ObjectHasSelf,
+    ObjectMinCardinality, ObjectMaxCardinality, ObjectExactCardinality, DataSomeValuesFrom, DataAllValuesFrom,
+    DataHasValue, DataMinCardinality, DataMaxCardinality, DataExactCardinality
+"""
+from .class_expression import OWLClassExpression, OWLAnonymousClassExpression, OWLBooleanClassExpression, \
+    OWLObjectComplementOf
+from .owl_class import OWLClass
+from .nary_boolean_expression import OWLNaryBooleanClassExpression, OWLObjectUnionOf, OWLObjectIntersectionOf
+from .restriction import (OWLRestriction, OWLQuantifiedRestriction, OWLQuantifiedObjectRestriction,
+                          OWLObjectRestriction,
+                          OWLHasValueRestriction, OWLDataRestriction, OWLCardinalityRestriction,
+                          OWLObjectCardinalityRestriction, OWLObjectHasSelf,
+                          OWLDataOneOf, OWLQuantifiedDataRestriction, OWLDataCardinalityRestriction,
+                          OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, OWLObjectHasValue,
+                          OWLDatatypeRestriction, OWLFacet, OWLFacetRestriction,
+                          OWLObjectMinCardinality,
+                          OWLObjectMaxCardinality,
+                          OWLObjectExactCardinality,
+                          OWLDataSomeValuesFrom,
+                          OWLDataAllValuesFrom,
+                          OWLDataHasValue,
+                          OWLDataMinCardinality,
+                          OWLDataMaxCardinality,
+                          OWLDataExactCardinality,
+                          OWLObjectOneOf
+                          )
+from typing import Final
+from ..vocab import OWLRDFVocabulary
+
+OWLThing: Final = OWLClass(OWLRDFVocabulary.OWL_THING.iri)  #: : :The OWL Class corresponding to owl:Thing
+OWLNothing: Final = OWLClass(OWLRDFVocabulary.OWL_NOTHING.iri)  #: : :The OWL Class corresponding to owl:Nothing
```

### Comparing `owlapy-0.1.3/owlapy/class_expression/class_expression.py` & `owlapy-1.0.0/owlapy/class_expression/class_expression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,114 @@
-from abc import abstractmethod, ABCMeta
-from ..data_ranges import OWLPropertyRange, OWLDataRange
-from ..meta_classes import HasOperands
-
-from typing import Final, Iterable
-class OWLClassExpression(OWLPropertyRange):
-    """An OWL 2 Class Expression (https://www.w3.org/TR/owl2-syntax/#Class_Expressions) """
-    __slots__ = ()
-
-    @abstractmethod
-    def is_owl_thing(self) -> bool:
-        """Determines if this expression is the built in class owl:Thing. This method does not determine if the class
-        is equivalent to owl:Thing.
-
-        Returns:
-            True if this expression is owl:Thing.
-        """
-        pass
-
-    @abstractmethod
-    def is_owl_nothing(self) -> bool:
-        """Determines if this expression is the built in class owl:Nothing. This method does not determine if the class
-        is equivalent to owl:Nothing.
-        """
-        pass
-
-    @abstractmethod
-    def get_object_complement_of(self) -> 'OWLObjectComplementOf':
-        """Gets the object complement of this class expression.
-
-        Returns:
-            A class expression that is the complement of this class expression.
-        """
-        pass
-
-    @abstractmethod
-    def get_nnf(self) -> 'OWLClassExpression':
-        """Gets the negation normal form of the complement of this expression.
-
-        Returns:
-            A expression that represents the NNF of the complement of this expression.
-        """
-        pass
-
-
-class OWLAnonymousClassExpression(OWLClassExpression, metaclass=ABCMeta):
-    """A Class Expression which is not a named Class."""
-
-    def is_owl_nothing(self) -> bool:
-        # documented in parent
-        return False
-
-    def is_owl_thing(self) -> bool:
-        # documented in parent
-        return False
-
-    def get_object_complement_of(self) -> 'OWLObjectComplementOf':
-        # documented in parent
-        return OWLObjectComplementOf(self)
-
-    def get_nnf(self) -> 'OWLClassExpression':
-        # documented in parent
-        from owlapy.util import NNF
-        return NNF().get_class_nnf(self)
-
-
-class OWLBooleanClassExpression(OWLAnonymousClassExpression, metaclass=ABCMeta):
-    """Represent an anonymous boolean class expression."""
-    __slots__ = ()
-    pass
-
-
-class OWLObjectComplementOf(OWLBooleanClassExpression, HasOperands[OWLClassExpression]):
-    """Represents an ObjectComplementOf class expression in the OWL 2 Specification."""
-    __slots__ = '_operand'
-    type_index: Final = 3003
-
-    _operand: OWLClassExpression
-
-    def __init__(self, op: OWLClassExpression):
-        """
-        Args:
-            op: Class expression to complement.
-        """
-        self._operand = op
-
-    def get_operand(self) -> OWLClassExpression:
-        """
-        Returns:
-            The wrapped expression.
-        """
-        return self._operand
-
-    def operands(self) -> Iterable[OWLClassExpression]:
-        # documented in parent
-        yield self._operand
-
-    def __repr__(self):
-        return f"OWLObjectComplementOf({repr(self._operand)})"
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._operand == other._operand
-        return NotImplemented
-
-    def __hash__(self):
-        return hash(self._operand)
+"""OWL Base Classes Expressions"""
+from abc import abstractmethod, ABCMeta
+from ..owl_data_ranges import OWLPropertyRange
+from ..meta_classes import HasOperands
+
+from typing import Final, Iterable
+
+
+class OWLClassExpression(OWLPropertyRange):
+    """OWL Class expressions represent sets of individuals by formally specifying conditions on the individuals' properties;
+     individuals satisfying these conditions are said to be instances of the respective class expressions.
+     In the structural specification of OWL 2, class expressions are represented by ClassExpression.
+     (https://www.w3.org/TR/owl2-syntax/#Class_Expressions)
+     """
+    __slots__ = ()
+
+    @abstractmethod
+    def is_owl_thing(self) -> bool:
+        """Determines if this expression is the built in class owl:Thing. This method does not determine if the class
+        is equivalent to owl:Thing.
+
+        Returns:
+            True if this expression is owl:Thing.
+        """
+        pass
+
+    @abstractmethod
+    def is_owl_nothing(self) -> bool:
+        """Determines if this expression is the built in class owl:Nothing. This method does not determine if the class
+        is equivalent to owl:Nothing.
+        """
+        pass
+
+    @abstractmethod
+    def get_object_complement_of(self) -> 'OWLObjectComplementOf':
+        """Gets the object complement of this class expression.
+
+        Returns:
+            A class expression that is the complement of this class expression.
+        """
+        pass
+
+    @abstractmethod
+    def get_nnf(self) -> 'OWLClassExpression':
+        """Gets the negation normal form of the complement of this expression.
+
+        Returns:
+            A expression that represents the NNF of the complement of this expression.
+        """
+        pass
+
+
+class OWLAnonymousClassExpression(OWLClassExpression, metaclass=ABCMeta):
+    """A Class Expression which is not a named Class."""
+
+    def is_owl_nothing(self) -> bool:
+        # documented in parent
+        return False
+
+    def is_owl_thing(self) -> bool:
+        # documented in parent
+        return False
+
+    def get_object_complement_of(self) -> 'OWLObjectComplementOf':
+        # documented in parent
+        return OWLObjectComplementOf(self)
+
+    def get_nnf(self) -> 'OWLClassExpression':
+        # documented in parent
+        from owlapy.util import NNF
+        return NNF().get_class_nnf(self)
+
+
+class OWLBooleanClassExpression(OWLAnonymousClassExpression, metaclass=ABCMeta):
+    """Represent an anonymous boolean class expression."""
+    __slots__ = ()
+    pass
+
+
+class OWLObjectComplementOf(OWLBooleanClassExpression, HasOperands[OWLClassExpression]):
+    """Represents an ObjectComplementOf class expression in the OWL 2 Specification."""
+    __slots__ = '_operand'
+    type_index: Final = 3003
+
+    _operand: OWLClassExpression
+
+    def __init__(self, op: OWLClassExpression):
+        """
+        Args:
+            op: Class expression to complement.
+        """
+        self._operand = op
+
+    def get_operand(self) -> OWLClassExpression:
+        """
+        Returns:
+            The wrapped expression.
+        """
+        return self._operand
+
+    def operands(self) -> Iterable[OWLClassExpression]:
+        # documented in parent
+        yield self._operand
+
+    def __repr__(self):
+        return f"OWLObjectComplementOf({repr(self._operand)})"
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._operand == other._operand
+        return NotImplemented
+
+    def __hash__(self):
+        return hash(self._operand)
```

### Comparing `owlapy-0.1.3/owlapy/iri.py` & `owlapy-1.0.0/owlapy/iri.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,180 +1,181 @@
-import weakref
-from abc import ABCMeta, abstractmethod
-from typing import Final, Union, overload
-from weakref import WeakKeyDictionary
-
-from owlapy import namespaces
-from .owl_annotation import OWLAnnotationSubject, OWLAnnotationValue
-from owlapy.namespaces import Namespaces
-
-
-class _WeakCached(type):
-    __slots__ = ()
-
-    def __init__(cls, what, bases, dct):
-        super().__init__(what, bases, dct)
-        cls._cache = WeakKeyDictionary()
-
-    def __call__(cls, *args, **kwargs):
-        _temp = super().__call__(*args, **kwargs)
-        ret = cls._cache.get(_temp)
-        if ret is None:
-            cls._cache[_temp] = weakref.ref(_temp)
-            return _temp
-        else:
-            return ret()
-
-
-class _meta_IRI(ABCMeta, _WeakCached):
-    __slots__ = ()
-    pass
-
-
-class IRI(OWLAnnotationSubject, OWLAnnotationValue, metaclass=_meta_IRI):
-    """An IRI, consisting of a namespace and a remainder."""
-    __slots__ = '_namespace', '_remainder', '__weakref__'
-    type_index: Final = 0
-
-    _namespace: str
-    _remainder: str
-
-    def __init__(self, namespace: Union[str, Namespaces], remainder: str):
-        if isinstance(namespace, Namespaces):
-            namespace = namespace.ns
-        else:
-            assert namespace[-1] in ("/", ":", "#")
-        import sys
-        self._namespace = sys.intern(namespace)
-        self._remainder = remainder
-
-    @overload
-    @staticmethod
-    def create(namespace: Namespaces, remainder: str) -> 'IRI':
-        ...
-
-    @overload
-    @staticmethod
-    def create(namespace: str, remainder: str) -> 'IRI':
-        """Creates an IRI by concatenating two strings. The full IRI is an IRI that contains the characters in
-        namespace + remainder.
-
-        Args:
-            namespace: The first string.
-            remainder: The second string.
-
-        Returns:
-            An IRI whose characters consist of prefix + suffix.
-        """
-        ...
-
-    @overload
-    @staticmethod
-    def create(string: str) -> 'IRI':
-        """Creates an IRI from the specified String.
-
-        Args:
-            string: The String that specifies the IRI.
-
-        Returns:
-            The IRI that has the specified string representation.
-        """
-        ...
-
-    @staticmethod
-    def create(string, remainder=None) -> 'IRI':
-        if remainder is not None:
-            return IRI(string, remainder)
-        index = 1 + max(string.rfind("/"), string.rfind(":"), string.rfind("#"))
-        return IRI(string[0:index], string[index:])
-
-    def __repr__(self):
-        return f"IRI({repr(self._namespace)},{repr(self._remainder)})"
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._namespace is other._namespace and self._remainder == other._remainder
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._namespace, self._remainder))
-
-    def is_nothing(self):
-        """Determines if this IRI is equal to the IRI that owl:Nothing is named with.
-
-        Returns:
-            :True if this IRI is equal to <http://www.w3.org/2002/07/owl#Nothing> and otherwise False.
-        """
-        from owlapy.vocab import OWLRDFVocabulary
-        return self == OWLRDFVocabulary.OWL_NOTHING.get_iri()
-
-    def is_thing(self):
-        """Determines if this IRI is equal to the IRI that owl:Thing is named with.
-
-        Returns:
-            :True if this IRI is equal to <http://www.w3.org/2002/07/owl#Thing> and otherwise False.
-        """
-        from owlapy.vocab import OWLRDFVocabulary
-        return self == OWLRDFVocabulary.OWL_THING.get_iri()
-
-    def is_reserved_vocabulary(self) -> bool:
-        """Determines if this IRI is in the reserved vocabulary. An IRI is in the reserved vocabulary if it starts with
-        <http://www.w3.org/1999/02/22-rdf-syntax-ns#> or <http://www.w3.org/2000/01/rdf-schema#> or
-        <http://www.w3.org/2001/XMLSchema#> or <http://www.w3.org/2002/07/owl#>.
-
-        Returns:
-            True if the IRI is in the reserved vocabulary, otherwise False.
-        """
-        return (self._namespace == namespaces.OWL or self._namespace == namespaces.RDF
-                or self._namespace == namespaces.RDFS or self._namespace == namespaces.XSD)
-
-    def as_iri(self) -> 'IRI':
-        # documented in parent
-        return self
-
-    def as_str(self) -> str:
-        """
-        CD: Should be deprecated.
-        Returns:
-            The string that specifies the IRI.
-        """
-        return self._namespace + self._remainder
-
-    @property
-    def str(self) -> str:
-        """
-
-        Returns:
-            The string that specifies the IRI.
-        """
-        return self.as_str()
-
-    @property
-    def reminder(self) -> str:
-        """
-
-        Returns:
-            The string corresponding to the reminder of the IRI.
-        """
-        return self.reminder()
-
-    def get_short_form(self) -> str:
-        """Gets the short form.
-
-        Returns:
-            A string that represents the short form.
-        """
-        return self._remainder
-
-    def get_namespace(self) -> str:
-        """
-        Returns:
-            The namespace as string.
-        """
-        return self._namespace
-
-    def get_remainder(self) -> str:
-        """
-        Returns:
-            The remainder (coincident with NCName usually) for this IRI.
-        """
-        return self._remainder
+"""OWL IRI"""
+import weakref
+from abc import ABCMeta
+from typing import Final, Union, overload
+from weakref import WeakKeyDictionary
+
+from owlapy import namespaces
+from .owl_annotation import OWLAnnotationSubject, OWLAnnotationValue
+from owlapy.namespaces import Namespaces
+
+
+class _WeakCached(type):
+    __slots__ = ()
+
+    def __init__(cls, what, bases, dct):
+        super().__init__(what, bases, dct)
+        cls._cache = WeakKeyDictionary()
+
+    def __call__(cls, *args, **kwargs):
+        _temp = super().__call__(*args, **kwargs)
+        ret = cls._cache.get(_temp)
+        if ret is None:
+            cls._cache[_temp] = weakref.ref(_temp)
+            return _temp
+        else:
+            return ret()
+
+
+class _meta_IRI(ABCMeta, _WeakCached):
+    __slots__ = ()
+    pass
+
+
+class IRI(OWLAnnotationSubject, OWLAnnotationValue, metaclass=_meta_IRI):
+    """An IRI, consisting of a namespace and a remainder."""
+    __slots__ = '_namespace', '_remainder', '__weakref__'
+    type_index: Final = 0
+
+    _namespace: str
+    _remainder: str
+
+    def __init__(self, namespace: Union[str, Namespaces], remainder: str):
+        if isinstance(namespace, Namespaces):
+            namespace = namespace.ns
+        else:
+            assert namespace[-1] in ("/", ":", "#")
+        import sys
+        self._namespace = sys.intern(namespace)
+        self._remainder = remainder
+
+    @overload
+    @staticmethod
+    def create(namespace: Namespaces, remainder: str) -> 'IRI':
+        ...
+
+    @overload
+    @staticmethod
+    def create(namespace: str, remainder: str) -> 'IRI':
+        """Creates an IRI by concatenating two strings. The full IRI is an IRI that contains the characters in
+        namespace + remainder.
+
+        Args:
+            namespace: The first string.
+            remainder: The second string.
+
+        Returns:
+            An IRI whose characters consist of prefix + suffix.
+        """
+        ...
+
+    @overload
+    @staticmethod
+    def create(string: str) -> 'IRI':
+        """Creates an IRI from the specified String.
+
+        Args:
+            string: The String that specifies the IRI.
+
+        Returns:
+            The IRI that has the specified string representation.
+        """
+        ...
+
+    @staticmethod
+    def create(string, remainder=None) -> 'IRI':
+        if remainder is not None:
+            return IRI(string, remainder)
+        index = 1 + max(string.rfind("/"), string.rfind(":"), string.rfind("#"))
+        return IRI(string[0:index], string[index:])
+
+    def __repr__(self):
+        return f"IRI({repr(self._namespace)},{repr(self._remainder)})"
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._namespace is other._namespace and self._remainder == other._remainder
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._namespace, self._remainder))
+
+    def is_nothing(self):
+        """Determines if this IRI is equal to the IRI that owl:Nothing is named with.
+
+        Returns:
+            :True if this IRI is equal to <http://www.w3.org/2002/07/owl#Nothing> and otherwise False.
+        """
+        from owlapy.vocab import OWLRDFVocabulary
+        return self == OWLRDFVocabulary.OWL_NOTHING.iri
+
+    def is_thing(self):
+        """Determines if this IRI is equal to the IRI that owl:Thing is named with.
+
+        Returns:
+            :True if this IRI is equal to <http://www.w3.org/2002/07/owl#Thing> and otherwise False.
+        """
+        from owlapy.vocab import OWLRDFVocabulary
+        return self == OWLRDFVocabulary.OWL_THING.iri
+
+    def is_reserved_vocabulary(self) -> bool:
+        """Determines if this IRI is in the reserved vocabulary. An IRI is in the reserved vocabulary if it starts with
+        <http://www.w3.org/1999/02/22-rdf-syntax-ns#> or <http://www.w3.org/2000/01/rdf-schema#> or
+        <http://www.w3.org/2001/XMLSchema#> or <http://www.w3.org/2002/07/owl#>.
+
+        Returns:
+            True if the IRI is in the reserved vocabulary, otherwise False.
+        """
+        return (self._namespace == namespaces.OWL or self._namespace == namespaces.RDF
+                or self._namespace == namespaces.RDFS or self._namespace == namespaces.XSD)
+
+    def as_iri(self) -> 'IRI':
+        # documented in parent
+        return self
+
+    def as_str(self) -> str:
+        """
+        CD: Should be deprecated.
+        Returns:
+            The string that specifies the IRI.
+        """
+        return self._namespace + self._remainder
+
+    @property
+    def str(self) -> str:
+        """
+
+        Returns:
+            The string that specifies the IRI.
+        """
+        return self.as_str()
+
+    @property
+    def reminder(self) -> str:
+        """
+
+        Returns:
+            The string corresponding to the reminder of the IRI.
+        """
+        return self.reminder()
+
+    def get_short_form(self) -> str:
+        """Gets the short form.
+
+        Returns:
+            A string that represents the short form.
+        """
+        return self._remainder
+
+    def get_namespace(self) -> str:
+        """
+        Returns:
+            The namespace as string.
+        """
+        return self._namespace
+
+    def get_remainder(self) -> str:
+        """
+        Returns:
+            The remainder (coincident with NCName usually) for this IRI.
+        """
+        return self._remainder
```

### Comparing `owlapy-0.1.3/owlapy/model/providers.py` & `owlapy-1.0.0/owlapy/providers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""OWL Datatype restriction constructors."""
-from typing import Union
-from datetime import datetime, date
-from owlapy.owl_literal import OWLLiteral
-from owlapy.class_expression import OWLDatatypeRestriction, OWLFacet, OWLFacetRestriction
-from pandas import Timedelta
-
-Restriction_Literals = Union[OWLLiteral, int, float, Timedelta, datetime, date]
-
-
-def OWLDatatypeMaxExclusiveRestriction(max_: Restriction_Literals) -> OWLDatatypeRestriction:
-    """Create a max exclusive restriction."""
-    r = OWLFacetRestriction(OWLFacet.MAX_EXCLUSIVE, max_)
-    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
-
-
-def OWLDatatypeMinExclusiveRestriction(min_: Restriction_Literals) -> OWLDatatypeRestriction:
-    """Create a min exclusive restriction."""
-    r = OWLFacetRestriction(OWLFacet.MIN_EXCLUSIVE, min_)
-    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
-
-
-def OWLDatatypeMaxInclusiveRestriction(max_: Restriction_Literals) -> OWLDatatypeRestriction:
-    """Create a max inclusive restriction."""
-    r = OWLFacetRestriction(OWLFacet.MAX_INCLUSIVE, max_)
-    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
-
-
-def OWLDatatypeMinInclusiveRestriction(min_: Restriction_Literals) -> OWLDatatypeRestriction:
-    """Create a min inclusive restriction."""
-    r = OWLFacetRestriction(OWLFacet.MIN_INCLUSIVE, min_)
-    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
-
-
-def OWLDatatypeMinMaxExclusiveRestriction(min_: Restriction_Literals,
-                                          max_: Restriction_Literals) -> OWLDatatypeRestriction:
-    """Create a min-max exclusive restriction."""
-    if isinstance(min_, float) and isinstance(max_, int):
-        max_ = float(max_)
-    if isinstance(max_, float) and isinstance(min_, int):
-        min_ = float(min_)
-    assert type(min_) == type(max_)
-
-    r_min = OWLFacetRestriction(OWLFacet.MIN_EXCLUSIVE, min_)
-    r_max = OWLFacetRestriction(OWLFacet.MAX_EXCLUSIVE, max_)
-    restrictions = (r_min, r_max)
-    return OWLDatatypeRestriction(r_min.get_facet_value().get_datatype(), restrictions)
-
-
-def OWLDatatypeMinMaxInclusiveRestriction(min_: Restriction_Literals,
-                                          max_: Restriction_Literals) -> OWLDatatypeRestriction:
-    """Create a min-max inclusive restriction."""
-    if isinstance(min_, float) and isinstance(max_, int):
-        max_ = float(max_)
-    if isinstance(max_, float) and isinstance(min_, int):
-        min_ = float(min_)
-    assert type(min_) == type(max_)
-
-    r_min = OWLFacetRestriction(OWLFacet.MIN_INCLUSIVE, min_)
-    r_max = OWLFacetRestriction(OWLFacet.MAX_INCLUSIVE, max_)
-    restrictions = (r_min, r_max)
-    return OWLDatatypeRestriction(r_min.get_facet_value().get_datatype(), restrictions)
+"""OWL Datatype restriction constructors."""
+from typing import Union
+from datetime import datetime, date
+from owlapy.owl_literal import OWLLiteral
+from owlapy.class_expression import OWLDatatypeRestriction, OWLFacet, OWLFacetRestriction
+from pandas import Timedelta
+
+Restriction_Literals = Union[OWLLiteral, int, float, Timedelta, datetime, date]
+
+
+def owl_datatype_max_exclusive_restriction(max_: Restriction_Literals) -> OWLDatatypeRestriction:
+    """Create a max exclusive restriction."""
+    r = OWLFacetRestriction(OWLFacet.MAX_EXCLUSIVE, max_)
+    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
+
+
+def owl_datatype_min_exclusive_restriction(min_: Restriction_Literals) -> OWLDatatypeRestriction:
+    """Create a min exclusive restriction."""
+    r = OWLFacetRestriction(OWLFacet.MIN_EXCLUSIVE, min_)
+    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
+
+
+def owl_datatype_max_inclusive_restriction(max_: Restriction_Literals) -> OWLDatatypeRestriction:
+    """Create a max inclusive restriction."""
+    r = OWLFacetRestriction(OWLFacet.MAX_INCLUSIVE, max_)
+    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
+
+
+def owl_datatype_min_inclusive_restriction(min_: Restriction_Literals) -> OWLDatatypeRestriction:
+    """Create a min inclusive restriction."""
+    r = OWLFacetRestriction(OWLFacet.MIN_INCLUSIVE, min_)
+    return OWLDatatypeRestriction(r.get_facet_value().get_datatype(), r)
+
+
+def owl_datatype_min_max_exclusive_restriction(min_: Restriction_Literals,
+                                               max_: Restriction_Literals) -> OWLDatatypeRestriction:
+    """Create a min-max exclusive restriction."""
+    if isinstance(min_, float) and isinstance(max_, int):
+        max_ = float(max_)
+    if isinstance(max_, float) and isinstance(min_, int):
+        min_ = float(min_)
+    assert type(min_) == type(max_)
+
+    r_min = OWLFacetRestriction(OWLFacet.MIN_EXCLUSIVE, min_)
+    r_max = OWLFacetRestriction(OWLFacet.MAX_EXCLUSIVE, max_)
+    restrictions = (r_min, r_max)
+    return OWLDatatypeRestriction(r_min.get_facet_value().get_datatype(), restrictions)
+
+
+def owl_datatype_min_max_inclusive_restriction(min_: Restriction_Literals,
+                                               max_: Restriction_Literals) -> OWLDatatypeRestriction:
+    """Create a min-max inclusive restriction."""
+    if isinstance(min_, float) and isinstance(max_, int):
+        max_ = float(max_)
+    if isinstance(max_, float) and isinstance(min_, int):
+        min_ = float(min_)
+    assert type(min_) == type(max_)
+
+    r_min = OWLFacetRestriction(OWLFacet.MIN_INCLUSIVE, min_)
+    r_max = OWLFacetRestriction(OWLFacet.MAX_INCLUSIVE, max_)
+    restrictions = (r_min, r_max)
+    return OWLDatatypeRestriction(r_min.get_facet_value().get_datatype(), restrictions)
```

### Comparing `owlapy-0.1.3/owlapy/namespaces.py` & `owlapy-1.0.0/owlapy/namespaces.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-"""Namespaces."""
-from typing import Final
-
-
-class Namespaces:
-    """A Namespace and its prefix."""
-    __slots__ = '_prefix', '_ns'
-
-    _prefix: str
-    _ns: str
-
-    def __init__(self, prefix: str, ns: str):
-        """Create a new namespace.
-
-        Args:
-            prefix: Typical prefix associated with this namespace.
-            ns: Namespace IRI as string.
-        """
-        assert ns[-1] in ("/", ":", "#")
-        self._prefix = prefix
-        self._ns = ns
-
-    @property
-    def ns(self) -> str:
-        return self._ns
-
-    @property
-    def prefix(self) -> str:
-        return self._prefix
-
-    def __repr__(self):
-        return f'Namespaces({repr(self._prefix)}, {repr(self._ns)})'
-
-    def __hash__(self):
-        return hash((self._prefix, self._ns))
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._ns == other._ns
-        elif type(other) is str:
-            return self._ns == other
-        return NotImplemented
-
-
-OWL: Final = Namespaces("owl", "http://www.w3.org/2002/07/owl#")  #:
-RDFS: Final = Namespaces("rdfs", "http://www.w3.org/2000/01/rdf-schema#")  #:
-RDF: Final = Namespaces("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")  #:
-XSD: Final = Namespaces("xsd", "http://www.w3.org/2001/XMLSchema#")  #:
+"""Namespaces."""
+from typing import Final
+
+
+class Namespaces:
+    """Namespaces provide a simple method for qualifying element and attribute names used in Extensible Markup
+    Language documents by associating them with namespaces identified by URI references"""
+    __slots__ = '_prefix', '_ns'
+
+    _prefix: str
+    _ns: str
+
+    def __init__(self, prefix: str, ns: str):
+        """Create a new namespace.
+
+        Args:
+            prefix: Typical prefix associated with this namespace.
+            ns: Namespace IRI as string.
+        """
+        assert ns[-1] in ("/", ":", "#")
+        self._prefix = prefix
+        self._ns = ns
+
+    @property
+    def ns(self) -> str:
+        return self._ns
+
+    @property
+    def prefix(self) -> str:
+        return self._prefix
+
+    def __repr__(self):
+        return f'Namespaces({repr(self._prefix)}, {repr(self._ns)})'
+
+    def __hash__(self):
+        return hash((self._prefix, self._ns))
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._ns == other._ns
+        elif type(other) is str:
+            return self._ns == other
+        return NotImplemented
+
+
+OWL: Final = Namespaces("owl", "http://www.w3.org/2002/07/owl#")  #:
+RDFS: Final = Namespaces("rdfs", "http://www.w3.org/2000/01/rdf-schema#")  #:
+RDF: Final = Namespaces("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")  #:
+XSD: Final = Namespaces("xsd", "http://www.w3.org/2001/XMLSchema#")  #:
```

### Comparing `owlapy-0.1.3/owlapy/owl2sparql/converter.py` & `owlapy-1.0.0/owlapy/converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,601 +1,603 @@
-"""Format converter."""
-from collections import defaultdict
-from contextlib import contextmanager
-from functools import singledispatchmethod
-from types import MappingProxyType
-from typing import Set, List, Dict, Optional, Iterable
-
-from rdflib.plugins.sparql.parser import parseQuery
-
-from owlapy.model import OWLClassExpression, OWLClass, OWLEntity, OWLObjectProperty, \
-    OWLObjectUnionOf, OWLObjectComplementOf, OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, \
-    OWLNamedIndividual, OWLObjectCardinalityRestriction, OWLObjectMinCardinality, OWLObjectExactCardinality, \
-    OWLObjectMaxCardinality, OWLDataCardinalityRestriction, OWLDataProperty, OWLObjectHasSelf, \
-    OWLDataSomeValuesFrom, OWLDataAllValuesFrom, OWLDataHasValue, OWLDatatype, TopOWLDatatype, OWLDataOneOf, OWLObjectIntersectionOf
-from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf, OWLDatatypeRestriction
-from owlapy.owl_literal import OWLLiteral
-from owlapy.vocab import OWLFacet, OWLRDFVocabulary
-
-_Variable_facet_comp = MappingProxyType({
-    OWLFacet.MIN_INCLUSIVE: ">=",
-    OWLFacet.MIN_EXCLUSIVE: ">",
-    OWLFacet.MAX_INCLUSIVE: "<=",
-    OWLFacet.MAX_EXCLUSIVE: "<"
-})
-
-
-def peek(x):
-    """Peek the last element of an array.
-
-    Returns:
-        The last element arr[-1].
-
-    """
-    return x[-1]
-
-
-class VariablesMapping:
-    """Helper class for owl-to-sparql conversion."""
-    __slots__ = 'class_cnt', 'prop_cnt', 'ind_cnt', 'dict'
-
-    def __init__(self):
-        self.class_cnt = 0
-        self.prop_cnt = 0
-        self.ind_cnt = 0
-        self.dict = dict()
-
-    def get_variable(self, e: OWLEntity) -> str:
-        if e in self.dict:
-            return self.dict[e]
-
-        if isinstance(e, OWLClass):
-            self.class_cnt += 1
-            var = f"?cls_{self.class_cnt}"
-        elif isinstance(e, OWLObjectProperty) or isinstance(e, OWLDataProperty):
-            self.prop_cnt += 1
-            var = f"?p_{self.prop_cnt}"
-        elif isinstance(e, OWLNamedIndividual):
-            self.ind_cnt += 1
-            var = f"?ind_{self.ind_cnt}"
-        else:
-            raise ValueError(e)
-
-        self.dict[e] = var
-        return var
-
-    def new_individual_variable(self) -> str:
-        self.ind_cnt += 1
-        return f"?s_{self.ind_cnt}"
-
-    def new_property_variable(self) -> str:
-        self.prop_cnt += 1
-        return f"?p_{self.prop_cnt}"
-
-    def __contains__(self, item: OWLEntity) -> bool:
-        return item in self.dict
-
-    def __getitem__(self, item: OWLEntity) -> str:
-        return self.dict[item]
-
-
-class Owl2SparqlConverter:
-    """Convert owl (owlapy model class expressions) to SPARQL."""
-    __slots__ = 'ce', 'sparql', 'variables', 'parent', 'parent_var', 'properties', 'variable_entities', 'cnt', \
-                'mapping', 'grouping_vars', 'having_conditions', '_intersection'
-    # @TODO:CD: We need to document this class. The computation behind the mapping is not clear.
-
-    ce: OWLClassExpression
-    sparql: List[str]
-    variables: List[str]
-    parent: List[OWLClassExpression]
-    parent_var: List[str]
-    variable_entities: Set[OWLEntity]
-    properties: Dict[int, List[OWLEntity]]
-    _intersection: Dict[int, bool]
-    mapping: VariablesMapping
-    grouping_vars: Dict[OWLClassExpression, Set[str]]
-    having_conditions: Dict[OWLClassExpression, Set[str]]
-    cnt: int
-
-    def convert(self, root_variable: str, ce: OWLClassExpression, named_individuals: bool = False):
-        """Used to convert owl class expression to SPARQL syntax.
-
-        Args:
-            root_variable (str): Root variable name that will be used in SPARQL query.
-            ce (OWLClassExpression): The owl class expression to convert.
-            named_individuals (bool): If 'True' return only entities that are instances of owl:NamedIndividual.
-
-        Returns:
-            list[str]: The SPARQL query.
-        """
-        self.ce = ce
-        self.sparql = []
-        self.variables = []
-        self.parent = []
-        self.parent_var = []
-        self.properties = defaultdict(list)
-        self.variable_entities = set()
-        self._intersection = defaultdict(bool)
-        self.cnt = 0
-        self.mapping = VariablesMapping()
-        self.grouping_vars = defaultdict(set)
-        self.having_conditions = defaultdict(set)
-        # if named_individuals is True, we return only entities that are instances of owl:NamedIndividual
-        if named_individuals:
-            self.append_triple(root_variable, 'a', f"<{OWLRDFVocabulary.OWL_NAMED_INDIVIDUAL.as_str()}>")
-        with self.stack_variable(root_variable):
-            with self.stack_parent(ce):
-                self.process(ce)
-        return self.sparql
-
-    @property
-    def modal_depth(self):
-        return len(self.variables)
-
-    @singledispatchmethod
-    def render(self, e):
-        raise NotImplementedError(e)
-
-    @render.register
-    def _(self, lit: OWLLiteral):
-        return f'"{lit.get_literal()}"^^<{lit.get_datatype().to_string_id()}>'
-
-    @render.register
-    def _(self, e: OWLEntity):
-        if e in self.variable_entities:
-            s = self.mapping.get_variable(e)
-        else:
-            s = f"<{e.to_string_id()}>"
-        if isinstance(e, OWLObjectProperty):
-            self.properties[self.modal_depth].append(e)
-        return s
-
-    def _maybe_quote(self, e):
-        assert isinstance(e, str)
-        if e.startswith("?"):
-            return e
-        else:
-            return f"<{e}>"
-
-    def _maybe_quote_p(self, p):
-        if isinstance(p, str):
-            if p.startswith("?") or p == "a" or p.startswith("<"):
-                return p
-            else:
-                return f"<{p}>"
-        else:
-            return self.render(p)
-
-    def _maybe_render(self, o):
-        if isinstance(o, str):
-            return o
-        else:
-            return self.render(o)
-
-
-    @contextmanager
-    def stack_variable(self, var):
-        self.variables.append(var)
-        try:
-            yield
-        finally:
-            self.variables.pop()
-
-    @contextmanager
-    def stack_parent(self, parent: OWLClassExpression):
-        self.parent.append(parent)
-        self.parent_var.append(self.current_variable)
-        try:
-            yield
-        finally:
-            self.parent.pop()
-            self.parent_var.pop()
-
-    @property
-    def current_variable(self):
-        return peek(self.variables)
-
-    # this method is responsible for translating class expressions to SPARQL queries
-    # the decorator "@singledispatchmethod" denotes that the method is overload
-    # each overload of the method is responsible for processing a different type of class expressions (e.g., ⊔ or ⊓)
-    @singledispatchmethod
-    def process(self, ce: OWLClassExpression):
-        raise NotImplementedError(ce)
-
-    # an overload of process function
-    # this overload is responsible for handling single concepts (e.g., Brother)
-    # general case: C
-    # this is the final step of the recursion
-    @process.register
-    def _(self, ce: OWLClass):
-        if self.ce == ce or not ce.is_owl_thing():
-            self.append_triple(self.current_variable, "a", self.render(ce))
-            # old_var = self.current_variable
-            # new_var = self.mapping.new_individual_variable()
-            # with self.stack_variable(new_var):
-            #     self.append_triple(old_var, "a", new_var)
-            #     self.append_triple(new_var, "<http://www.w3.org/2000/01/rdf-schema#subClassOf>*", self.render(ce))
-        elif ce.is_owl_thing():
-            self.append_triple(self.current_variable, "a", "<http://www.w3.org/2002/07/owl#Thing>")
-
-    # an overload of process function
-    # this overload is responsible for handling intersections of concepts (e.g., Brother ⊓ Father)
-    # general case: C1 ⊓ ... ⊓ Cn
-    @process.register
-    def _(self, ce: OWLObjectIntersectionOf):
-        # we iterate over the concepts that appear in the intersection
-        for op in ce.operands():
-            self.process(op)
-
-    # an overload of process function
-    # this overload is responsible for handling unions of concepts (e.g., Brother ⊔ Sister)
-    # general case: C1 ⊔ ... ⊔ Cn
-    @process.register
-    def _(self, ce: OWLObjectUnionOf):
-        first = True
-        # we iterate over the concepts that appear in the union
-        for op in ce.operands():
-            # SPARQL's UNION comes after the first concept
-            if first:
-                first = False
-            else:
-                self.append(" UNION ")
-            self.append("{ ")
-            with self.stack_parent(op):
-                self.process(op)
-            self.append(" }")
-
-    # an overload of process function
-    # this overload is responsible for handling complements of concepts (e.g., ¬Brother)
-    # general case: ¬C
-    @process.register
-    def _(self, ce: OWLObjectComplementOf):
-        subject = self.current_variable
-        self.append_triple(subject, self.mapping.new_individual_variable(), self.mapping.new_individual_variable())
-
-        self.append("FILTER NOT EXISTS { ")
-        # process the concept after the ¬
-        self.process(ce.get_operand())
-        self.append(" }")
-
-    # an overload of process function
-    # this overload is responsible for handling the exists operator (e.g., ∃hasChild.Male)
-    # general case: ∃r.C
-    @process.register
-    def _(self, ce: OWLObjectSomeValuesFrom):
-        object_variable = self.mapping.new_individual_variable()
-        # property expression holds the role of the class expression (hasChild in our example)
-        property_expression = ce.get_property()
-        if property_expression.is_anonymous():
-            # property expression is inverse of a property
-            self.append_triple(object_variable, property_expression.get_named_property(), self.current_variable)
-        else:
-            self.append_triple(self.current_variable, property_expression.get_named_property(), object_variable)
-        # filler holds the concept of the expression (Male in our example) and is processed recursively
-        filler = ce.get_filler()
-        with self.stack_variable(object_variable):
-            self.process(filler)
-
-    # an overload of process function
-    # this overload is responsible for handling the forAll operator (e.g., ∀hasChild.Male)
-    # general case: ∀r.C
-    @process.register
-    def _(self, ce: OWLObjectAllValuesFrom):
-        subject = self.current_variable
-        object_variable = self.mapping.new_individual_variable()
-        # property expression holds the role of the class expression (hasChild in our example)
-        property_expression = ce.get_property()
-        predicate = property_expression.get_named_property()
-        # filler holds the concept of the expression (Male in our example) and is processed recursively
-        filler = ce.get_filler()
-
-
-        self.append("{")
-
-        if property_expression.is_anonymous():
-            # property expression is inverse of a property
-            self.append_triple(object_variable, predicate, self.current_variable)
-        else:
-            self.append_triple(self.current_variable, predicate, object_variable)
-
-        # restrict filler
-        var = self.mapping.new_individual_variable()
-        cnt_var1 = self.new_count_var()
-        # the count needs to use distinct
-        self.append(f"{{ SELECT {subject} ( COUNT( DISTINCT {var} ) AS {cnt_var1} ) WHERE {{ ")
-        self.append_triple(subject, predicate, var)
-        # here, we recursively process the filler (Male in our example)
-        with self.stack_variable(var):
-            self.process(filler)
-        self.append(f" }} GROUP BY {subject} }}")
-
-        var = self.mapping.new_individual_variable()
-        cnt_var2 = self.new_count_var()
-        # the count needs to use distinct
-        self.append(f"{{ SELECT {subject} ( COUNT( DISTINCT {var} ) AS {cnt_var2} ) WHERE {{ ")
-        self.append_triple(subject, predicate, var)
-        self.append(f" }} GROUP BY {subject} }}")
-
-        self.append(f" FILTER( {cnt_var1} = {cnt_var2} )")
-        self.append("} UNION { ")
-
-        # here, the second group graph pattern starts
-        # the second group graph pattern returns all those entities that do not appear in a triple with the property
-        self.append_triple(subject, self.mapping.new_individual_variable(), self.mapping.new_individual_variable())
-        self.append("FILTER NOT EXISTS { ")
-        if property_expression.is_anonymous():
-            # property expression is inverse of a property
-            self.append_triple(self.mapping.new_individual_variable(), predicate, self.current_variable)
-        else:
-            self.append_triple(self.current_variable, predicate, self.mapping.new_individual_variable())
-        self.append(" } }")
-
-    # an overload of process function
-    # this overload is responsible for handling the exists operator combined with an individual (e.g., ∃hasChild.{john})
-    # general case: ∃r.{a}
-    @process.register
-    def _(self, ce: OWLObjectHasValue):
-        property_expression = ce.get_property()
-        value = ce.get_filler()
-        # we ensure that the value is an individual
-        assert isinstance(value, OWLNamedIndividual)
-        if property_expression.is_anonymous():
-            self.append_triple(value.to_string_id(), property_expression.get_named_property(), self.current_variable)
-        else:
-            self.append_triple(self.current_variable, property_expression.get_named_property(), value)
-
-    # an overload of process function
-    # this overload is responsible for handling the exists operator combined with an individual(e.g., >=3 hasChild.Male)
-    # general case: \theta n r.C
-    @process.register
-    def _(self, ce: OWLObjectCardinalityRestriction):
-        subject_variable = self.current_variable
-        object_variable = self.mapping.new_individual_variable()
-        property_expression = ce.get_property()
-        cardinality = ce.get_cardinality()
-
-        if isinstance(ce, OWLObjectMinCardinality):
-            comparator = ">="
-        elif isinstance(ce, OWLObjectMaxCardinality):
-            comparator = "<="
-        elif isinstance(ce, OWLObjectExactCardinality):
-            comparator = "="
-        else:
-            raise ValueError(ce)
-
-        # if the comparator is ≤ or the cardinality is 0, we need an additional group graph pattern
-        # the additional group graph pattern will take care the cases where an individual is not associated with the
-        # property expression
-        if comparator == "<=" or cardinality == 0:
-            self.append("{")
-
-        self.append(f"{{ SELECT {subject_variable} WHERE {{ ")
-        if property_expression.is_anonymous():
-            # property expression is inverse of a property
-            self.append_triple(object_variable, property_expression.get_named_property(), subject_variable)
-        else:
-            self.append_triple(subject_variable, property_expression.get_named_property(), object_variable)
-
-        filler = ce.get_filler()
-        with self.stack_variable(object_variable):
-            self.process(filler)
-
-        self.append(f" }} GROUP BY {subject_variable}"
-                    f" HAVING ( COUNT ( {object_variable} ) {comparator} {cardinality} ) }}")
-
-        # here, the second group graph pattern starts
-        if comparator == "<=" or cardinality == 0:
-            self.append("} UNION {")
-            self.append_triple(subject_variable, self.mapping.new_individual_variable(),
-                               self.mapping.new_individual_variable())
-            self.append("FILTER NOT EXISTS { ")
-            object_variable = self.mapping.new_individual_variable()
-            if property_expression.is_anonymous():
-                # property expression is inverse of a property
-                self.append_triple(object_variable, property_expression.get_named_property(), self.current_variable)
-            else:
-                self.append_triple(self.current_variable, property_expression.get_named_property(), object_variable)
-            with self.stack_variable(object_variable):
-                self.process(filler)
-            self.append(" } }")
-
-    @process.register
-    def _(self, ce: OWLDataCardinalityRestriction):
-        subject_variable = self.current_variable
-        object_variable = self.mapping.new_individual_variable()
-        property_expression = ce.get_property()
-        assert isinstance(property_expression, OWLDataProperty)
-        cardinality = ce.get_cardinality()
-
-        if isinstance(ce, OWLObjectMinCardinality):
-            comparator = ">="
-        elif isinstance(ce, OWLObjectMaxCardinality):
-            comparator = "<="
-        elif isinstance(ce, OWLObjectExactCardinality):
-            comparator = "="
-        else:
-            raise ValueError(ce)
-
-        self.append(f"{{ SELECT {subject_variable} WHERE {{ ")
-        self.append_triple(subject_variable, property_expression, object_variable)
-
-        filler = ce.get_filler()
-        with self.stack_variable(object_variable):
-            self.process(filler)
-
-        self.append(f" }} GROUP BY {subject_variable}"
-                    f" HAVING ( COUNT ( {object_variable} ) {comparator} {cardinality} ) }}")
-
-    # an overload of process function
-    # this overload is responsible for handling the exists operator combined with SELF
-    # general case: ∃r.SELF
-    @process.register
-    def _(self, ce: OWLObjectHasSelf):
-        subject = self.current_variable
-        property = ce.get_property()
-        self.append_triple(subject, property.get_named_property(), subject)
-
-    # an overload of process function
-    # this overload is responsible for handling the one of case (e.g., { john, jane }
-    # general case: { a1, ..., an }
-    @process.register
-    def _(self, ce: OWLObjectOneOf):
-        subject = self.current_variable
-        if self.modal_depth == 1:
-            self.append_triple(subject, "?p", "?o")
-
-        self.append(f" FILTER ( {subject} IN ( ")
-        first = True
-        for ind in ce.individuals():
-            if first:
-                first = False
-            else:
-                self.append(",")
-            assert isinstance(ind, OWLNamedIndividual)
-            self.append(f"<{ind.to_string_id()}>")
-        self.append(f" ) )")
-
-    @process.register
-    def _(self, ce: OWLDataSomeValuesFrom):
-        object_variable = self.mapping.new_individual_variable()
-        property_expression = ce.get_property()
-        assert isinstance(property_expression, OWLDataProperty)
-        self.append_triple(self.current_variable, property_expression, object_variable)
-        filler = ce.get_filler()
-        with self.stack_variable(object_variable):
-            self.process(filler)
-
-    @process.register
-    def _(self, ce: OWLDataAllValuesFrom):
-        subject = self.current_variable
-        object_variable = self.mapping.new_individual_variable()
-        property_expression = ce.get_property()
-        assert isinstance(property_expression, OWLDataProperty)
-        predicate = property_expression.to_string_id()
-        filler = ce.get_filler()
-
-        self.append_triple(self.current_variable, predicate, object_variable)
-
-        var = self.mapping.new_individual_variable()
-        cnt_var1 = self.new_count_var()
-        self.append(f"{{ SELECT {subject} ( COUNT( {var} ) AS {cnt_var1} ) WHERE {{ ")
-        self.append_triple(subject, predicate, var)
-        with self.stack_variable(var):
-            self.process(filler)
-        self.append(f" }} GROUP BY {subject} }}")
-
-        var = self.mapping.new_individual_variable()
-        cnt_var2 = self.new_count_var()
-        self.append(f"{{ SELECT {subject} ( COUNT( {var} ) AS {cnt_var2} ) WHERE {{ ")
-        self.append_triple(subject, predicate, var)
-        self.append(f" }} GROUP BY {subject} }}")
-
-        self.append(f" FILTER( {cnt_var1} = {cnt_var2} )")
-
-    @process.register
-    def _(self, ce: OWLDataHasValue):
-        property_expression = ce.get_property()
-        value = ce.get_filler()
-        assert isinstance(value, OWLDataProperty)
-        self.append_triple(self.current_variable, property_expression, value)
-
-    @process.register
-    def _(self, node: OWLDatatype):
-        if node != TopOWLDatatype:
-            self.append(f" FILTER ( DATATYPE ( {self.current_variable} = <{node.to_string_id()}> ) ) ")
-
-    @process.register
-    def _(self, node: OWLDataOneOf):
-        subject = self.current_variable
-        if self.modal_depth == 1:
-            self.append_triple(subject, "?p", "?o")
-        self.append(f" FILTER ( {subject} IN ( ")
-        first = True
-        for value in node.values():
-            if first:
-                first = False
-            else:
-                self.append(",")
-            if value:
-                self.append(self.render(value))
-        self.append(f" ) ) ")
-
-    @process.register
-    def _(self, node: OWLDatatypeRestriction):
-        frs = node.get_facet_restrictions()
-
-        for fr in frs:
-            facet = fr.get_facet()
-            value = fr.get_facet_value()
-
-            if facet in _Variable_facet_comp:
-                self.append(f' FILTER ( {self.current_variable} {_Variable_facet_comp[facet]}'
-                            f' "{value.get_literal()}"^^<{value.get_datatype().to_string_id()}> ) ')
-
-    def new_count_var(self) -> str:
-        self.cnt += 1
-        return f"?cnt_{self.cnt}"
-
-    def append_triple(self, subject, predicate, object_):
-        self.append(self.triple(subject, predicate, object_))
-
-    def append(self, frag):
-        self.sparql.append(frag)
-
-    def triple(self, subject, predicate, object_):
-        return f"{self._maybe_quote(subject)} {self._maybe_quote_p(predicate)} {self._maybe_render(object_)} . "
-
-    def as_query(self,
-                 root_variable: str,
-                 ce: OWLClassExpression,
-                 count: bool = False,
-                 values: Optional[Iterable[OWLNamedIndividual]] = None,
-                 named_individuals: bool = False)->str:
-        """
-        root variable: the variable that will be projected
-        ce: the class expression to be transformed to a SPARQL query
-        count: True, counts the results ; False, projects the individuals
-        values: positive or negative examples from a class expression problem
-        named_individuals: if set to True, the generated SPARQL query will return only entities that are instances
-        of owl:NamedIndividual
-
-        """
-
-        qs = ["SELECT"]
-        tp = self.convert(root_variable, ce, named_individuals)
-        if count:
-            qs.append(f" ( COUNT ( DISTINCT {root_variable} ) AS ?cnt ) WHERE {{ ")
-        else:
-            qs.append(f" DISTINCT {root_variable} WHERE {{ ")
-        if values is not None and root_variable.startswith("?"):
-            q = [f"VALUES {root_variable} {{ "]
-            for x in values:
-                q.append(f"<{x.to_string_id()}>")
-            q.append(f"}} . ")
-            qs.extend(q)
-        qs.extend(tp)
-        qs.append(f" }}")
-
-
-        query = "\n".join(qs)
-        parseQuery(query)
-        return query
-
-
-converter = Owl2SparqlConverter()
-
-
-def owl_expression_to_sparql(root_variable: str = "?x",
-                             expression: OWLClassExpression = None,
-                             values: Optional[Iterable[OWLNamedIndividual]] = None,
-                             named_individuals: bool = False)->str:
-    """Convert an OWL Class Expression (https://www.w3.org/TR/owl2-syntax/#Class_Expressions) into a SPARQL query
-     root variable: the variable that will be projected
-     expression: the class expression to be transformed to a SPARQL query
-
-     values: positive or negative examples from a class expression problem. Unclear
-     named_individuals: if set to True, the generated SPARQL query will return only entities
-     that are instances of owl:NamedIndividual
-    """
-    assert expression is not None, "expression cannot be None"
-    return converter.as_query(root_variable, expression, False, values, named_individuals)
+"""Format converter."""
+from collections import defaultdict
+from contextlib import contextmanager
+from functools import singledispatchmethod
+from types import MappingProxyType
+from typing import Set, List, Dict, Optional, Iterable
+
+from rdflib.plugins.sparql.parser import parseQuery
+
+from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf, OWLDatatypeRestriction, OWLDataMinCardinality, \
+    OWLDataMaxCardinality, OWLDataExactCardinality, OWLClass, OWLClassExpression, OWLObjectIntersectionOf, \
+    OWLObjectUnionOf, OWLObjectComplementOf, OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, \
+    OWLObjectCardinalityRestriction, OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, \
+    OWLDataCardinalityRestriction, OWLObjectHasSelf, OWLDataSomeValuesFrom, OWLDataAllValuesFrom, OWLDataHasValue, \
+    OWLDataOneOf
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import OWLLiteral, TopOWLDatatype
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty
+from owlapy.owl_object import OWLEntity
+from owlapy.owl_datatype import OWLDatatype
+from owlapy.vocab import OWLFacet, OWLRDFVocabulary
+
+_Variable_facet_comp = MappingProxyType({
+    OWLFacet.MIN_INCLUSIVE: ">=",
+    OWLFacet.MIN_EXCLUSIVE: ">",
+    OWLFacet.MAX_INCLUSIVE: "<=",
+    OWLFacet.MAX_EXCLUSIVE: "<"
+})
+
+
+def peek(x):
+    """Peek the last element of an array.
+
+    Returns:
+        The last element arr[-1].
+
+    """
+    return x[-1]
+
+
+class VariablesMapping:
+    """Helper class for owl-to-sparql conversion."""
+    __slots__ = 'class_cnt', 'prop_cnt', 'ind_cnt', 'dict'
+
+    def __init__(self):
+        self.class_cnt = 0
+        self.prop_cnt = 0
+        self.ind_cnt = 0
+        self.dict = dict()
+
+    def get_variable(self, e: OWLEntity) -> str:
+        if e in self.dict:
+            return self.dict[e]
+
+        if isinstance(e, OWLClass):
+            self.class_cnt += 1
+            var = f"?cls_{self.class_cnt}"
+        elif isinstance(e, OWLObjectProperty) or isinstance(e, OWLDataProperty):
+            self.prop_cnt += 1
+            var = f"?p_{self.prop_cnt}"
+        elif isinstance(e, OWLNamedIndividual):
+            self.ind_cnt += 1
+            var = f"?ind_{self.ind_cnt}"
+        else:
+            raise ValueError(e)
+
+        self.dict[e] = var
+        return var
+
+    def new_individual_variable(self) -> str:
+        self.ind_cnt += 1
+        return f"?s_{self.ind_cnt}"
+
+    def new_property_variable(self) -> str:
+        self.prop_cnt += 1
+        return f"?p_{self.prop_cnt}"
+
+    def __contains__(self, item: OWLEntity) -> bool:
+        return item in self.dict
+
+    def __getitem__(self, item: OWLEntity) -> str:
+        return self.dict[item]
+
+
+class Owl2SparqlConverter:
+    """Convert owl (owlapy model class expressions) to SPARQL."""
+    __slots__ = 'ce', 'sparql', 'variables', 'parent', 'parent_var', 'properties', 'variable_entities', 'cnt', \
+                'mapping', 'grouping_vars', 'having_conditions', '_intersection'
+    # @TODO:CD: We need to document this class. The computation behind the mapping is not clear.
+
+    ce: OWLClassExpression
+    sparql: List[str]
+    variables: List[str]
+    parent: List[OWLClassExpression]
+    parent_var: List[str]
+    variable_entities: Set[OWLEntity]
+    properties: Dict[int, List[OWLEntity]]
+    _intersection: Dict[int, bool]
+    mapping: VariablesMapping
+    grouping_vars: Dict[OWLClassExpression, Set[str]]
+    having_conditions: Dict[OWLClassExpression, Set[str]]
+    cnt: int
+
+    def convert(self, root_variable: str, ce: OWLClassExpression, named_individuals: bool = False):
+        """Used to convert owl class expression to SPARQL syntax.
+
+        Args:
+            root_variable (str): Root variable name that will be used in SPARQL query.
+            ce (OWLClassExpression): The owl class expression to convert.
+            named_individuals (bool): If 'True' return only entities that are instances of owl:NamedIndividual.
+
+        Returns:
+            list[str]: The SPARQL query.
+        """
+        self.ce = ce
+        self.sparql = []
+        self.variables = []
+        self.parent = []
+        self.parent_var = []
+        self.properties = defaultdict(list)
+        self.variable_entities = set()
+        self._intersection = defaultdict(bool)
+        self.cnt = 0
+        self.mapping = VariablesMapping()
+        self.grouping_vars = defaultdict(set)
+        self.having_conditions = defaultdict(set)
+        # if named_individuals is True, we return only entities that are instances of owl:NamedIndividual
+        if named_individuals:
+            self.append_triple(root_variable, 'a', f"<{OWLRDFVocabulary.OWL_NAMED_INDIVIDUAL.as_str()}>")
+        with self.stack_variable(root_variable):
+            with self.stack_parent(ce):
+                self.process(ce)
+        return self.sparql
+
+    @property
+    def modal_depth(self):
+        return len(self.variables)
+
+    @singledispatchmethod
+    def render(self, e):
+        raise NotImplementedError(e)
+
+    @render.register
+    def _(self, lit: OWLLiteral):
+        return f'"{lit.get_literal()}"^^<{lit.get_datatype().to_string_id()}>'
+
+    @render.register
+    def _(self, e: OWLEntity):
+        if e in self.variable_entities:
+            s = self.mapping.get_variable(e)
+        else:
+            s = f"<{e.to_string_id()}>"
+        if isinstance(e, OWLObjectProperty):
+            self.properties[self.modal_depth].append(e)
+        return s
+
+    def _maybe_quote(self, e):
+        assert isinstance(e, str)
+        if e.startswith("?"):
+            return e
+        else:
+            return f"<{e}>"
+
+    def _maybe_quote_p(self, p):
+        if isinstance(p, str):
+            if p.startswith("?") or p == "a" or p.startswith("<"):
+                return p
+            else:
+                return f"<{p}>"
+        else:
+            return self.render(p)
+
+    def _maybe_render(self, o):
+        if isinstance(o, str):
+            return o
+        else:
+            return self.render(o)
+
+
+    @contextmanager
+    def stack_variable(self, var):
+        self.variables.append(var)
+        try:
+            yield
+        finally:
+            self.variables.pop()
+
+    @contextmanager
+    def stack_parent(self, parent: OWLClassExpression):
+        self.parent.append(parent)
+        self.parent_var.append(self.current_variable)
+        try:
+            yield
+        finally:
+            self.parent.pop()
+            self.parent_var.pop()
+
+    @property
+    def current_variable(self):
+        return peek(self.variables)
+
+    # this method is responsible for translating class expressions to SPARQL queries
+    # the decorator "@singledispatchmethod" denotes that the method is overload
+    # each overload of the method is responsible for processing a different type of class expressions (e.g., ⊔ or ⊓)
+    @singledispatchmethod
+    def process(self, ce: OWLClassExpression):
+        raise NotImplementedError(ce)
+
+    # an overload of process function
+    # this overload is responsible for handling single concepts (e.g., Brother)
+    # general case: C
+    # this is the final step of the recursion
+    @process.register
+    def _(self, ce: OWLClass):
+        if self.ce == ce or not ce.is_owl_thing():
+            self.append_triple(self.current_variable, "a", self.render(ce))
+            # old_var = self.current_variable
+            # new_var = self.mapping.new_individual_variable()
+            # with self.stack_variable(new_var):
+            #     self.append_triple(old_var, "a", new_var)
+            #     self.append_triple(new_var, "<http://www.w3.org/2000/01/rdf-schema#subClassOf>*", self.render(ce))
+        elif ce.is_owl_thing():
+            self.append_triple(self.current_variable, "a", "<http://www.w3.org/2002/07/owl#Thing>")
+
+    # an overload of process function
+    # this overload is responsible for handling intersections of concepts (e.g., Brother ⊓ Father)
+    # general case: C1 ⊓ ... ⊓ Cn
+    @process.register
+    def _(self, ce: OWLObjectIntersectionOf):
+        # we iterate over the concepts that appear in the intersection
+        for op in ce.operands():
+            self.process(op)
+
+    # an overload of process function
+    # this overload is responsible for handling unions of concepts (e.g., Brother ⊔ Sister)
+    # general case: C1 ⊔ ... ⊔ Cn
+    @process.register
+    def _(self, ce: OWLObjectUnionOf):
+        first = True
+        # we iterate over the concepts that appear in the union
+        for op in ce.operands():
+            # SPARQL's UNION comes after the first concept
+            if first:
+                first = False
+            else:
+                self.append(" UNION ")
+            self.append("{ ")
+            with self.stack_parent(op):
+                self.process(op)
+            self.append(" }")
+
+    # an overload of process function
+    # this overload is responsible for handling complements of concepts (e.g., ¬Brother)
+    # general case: ¬C
+    @process.register
+    def _(self, ce: OWLObjectComplementOf):
+        subject = self.current_variable
+        self.append_triple(subject, self.mapping.new_individual_variable(), self.mapping.new_individual_variable())
+
+        self.append("FILTER NOT EXISTS { ")
+        # process the concept after the ¬
+        self.process(ce.get_operand())
+        self.append(" }")
+
+    # an overload of process function
+    # this overload is responsible for handling the exists operator (e.g., ∃hasChild.Male)
+    # general case: ∃r.C
+    @process.register
+    def _(self, ce: OWLObjectSomeValuesFrom):
+        object_variable = self.mapping.new_individual_variable()
+        # property expression holds the role of the class expression (hasChild in our example)
+        property_expression = ce.get_property()
+        if property_expression.is_anonymous():
+            # property expression is inverse of a property
+            self.append_triple(object_variable, property_expression.get_named_property(), self.current_variable)
+        else:
+            self.append_triple(self.current_variable, property_expression.get_named_property(), object_variable)
+        # filler holds the concept of the expression (Male in our example) and is processed recursively
+        filler = ce.get_filler()
+        with self.stack_variable(object_variable):
+            self.process(filler)
+
+    # an overload of process function
+    # this overload is responsible for handling the forAll operator (e.g., ∀hasChild.Male)
+    # general case: ∀r.C
+    @process.register
+    def _(self, ce: OWLObjectAllValuesFrom):
+        subject = self.current_variable
+        object_variable = self.mapping.new_individual_variable()
+        # property expression holds the role of the class expression (hasChild in our example)
+        property_expression = ce.get_property()
+        predicate = property_expression.get_named_property()
+        # filler holds the concept of the expression (Male in our example) and is processed recursively
+        filler = ce.get_filler()
+
+        self.append("{")
+
+        if property_expression.is_anonymous():
+            # property expression is inverse of a property
+            self.append_triple(object_variable, predicate, self.current_variable)
+        else:
+            self.append_triple(self.current_variable, predicate, object_variable)
+
+        # restrict filler
+        var = self.mapping.new_individual_variable()
+        cnt_var1 = self.new_count_var()
+        # the count needs to use distinct
+        self.append(f"{{ SELECT {subject} ( COUNT( DISTINCT {var} ) AS {cnt_var1} ) WHERE {{ ")
+        self.append_triple(subject, predicate, var)
+        # here, we recursively process the filler (Male in our example)
+        with self.stack_variable(var):
+            self.process(filler)
+        self.append(f" }} GROUP BY {subject} }}")
+
+        var = self.mapping.new_individual_variable()
+        cnt_var2 = self.new_count_var()
+        # the count needs to use distinct
+        self.append(f"{{ SELECT {subject} ( COUNT( DISTINCT {var} ) AS {cnt_var2} ) WHERE {{ ")
+        self.append_triple(subject, predicate, var)
+        self.append(f" }} GROUP BY {subject} }}")
+
+        self.append(f" FILTER( {cnt_var1} = {cnt_var2} )")
+        self.append("} UNION { ")
+
+        # here, the second group graph pattern starts
+        # the second group graph pattern returns all those entities that do not appear in a triple with the property
+        self.append_triple(subject, self.mapping.new_individual_variable(), self.mapping.new_individual_variable())
+        self.append("FILTER NOT EXISTS { ")
+        if property_expression.is_anonymous():
+            # property expression is inverse of a property
+            self.append_triple(self.mapping.new_individual_variable(), predicate, self.current_variable)
+        else:
+            self.append_triple(self.current_variable, predicate, self.mapping.new_individual_variable())
+        self.append(" } }")
+
+    # an overload of process function
+    # this overload is responsible for handling the exists operator combined with an individual (e.g., ∃hasChild.{john})
+    # general case: ∃r.{a}
+    @process.register
+    def _(self, ce: OWLObjectHasValue):
+        property_expression = ce.get_property()
+        value = ce.get_filler()
+        # we ensure that the value is an individual
+        assert isinstance(value, OWLNamedIndividual)
+        if property_expression.is_anonymous():
+            self.append_triple(value.to_string_id(), property_expression.get_named_property(), self.current_variable)
+        else:
+            self.append_triple(self.current_variable, property_expression.get_named_property(), value)
+
+    # an overload of process function
+    # this overload is responsible for handling the exists operator combined with an individual(e.g., >=3 hasChild.Male)
+    # general case: \theta n r.C
+    @process.register
+    def _(self, ce: OWLObjectCardinalityRestriction):
+        subject_variable = self.current_variable
+        object_variable = self.mapping.new_individual_variable()
+        property_expression = ce.get_property()
+        cardinality = ce.get_cardinality()
+
+        if isinstance(ce, OWLObjectMinCardinality):
+            comparator = ">="
+        elif isinstance(ce, OWLObjectMaxCardinality):
+            comparator = "<="
+        elif isinstance(ce, OWLObjectExactCardinality):
+            comparator = "="
+        else:
+            raise ValueError(ce)
+
+        # if the comparator is ≤ or the cardinality is 0, we need an additional group graph pattern
+        # the additional group graph pattern will take care the cases where an individual is not associated with the
+        # property expression
+        if comparator == "<=" or cardinality == 0:
+            self.append("{")
+
+        self.append(f"{{ SELECT {subject_variable} WHERE {{ ")
+        if property_expression.is_anonymous():
+            # property expression is inverse of a property
+            self.append_triple(object_variable, property_expression.get_named_property(), subject_variable)
+        else:
+            self.append_triple(subject_variable, property_expression.get_named_property(), object_variable)
+
+        filler = ce.get_filler()
+        with self.stack_variable(object_variable):
+            self.process(filler)
+
+        self.append(f" }} GROUP BY {subject_variable}"
+                    f" HAVING ( COUNT ( {object_variable} ) {comparator} {cardinality} ) }}")
+
+        # here, the second group graph pattern starts
+        if comparator == "<=" or cardinality == 0:
+            self.append("} UNION {")
+            self.append_triple(subject_variable, self.mapping.new_individual_variable(),
+                               self.mapping.new_individual_variable())
+            self.append("FILTER NOT EXISTS { ")
+            object_variable = self.mapping.new_individual_variable()
+            if property_expression.is_anonymous():
+                # property expression is inverse of a property
+                self.append_triple(object_variable, property_expression.get_named_property(), self.current_variable)
+            else:
+                self.append_triple(self.current_variable, property_expression.get_named_property(), object_variable)
+            with self.stack_variable(object_variable):
+                self.process(filler)
+            self.append(" } }")
+
+    @process.register
+    def _(self, ce: OWLDataCardinalityRestriction):
+        subject_variable = self.current_variable
+        object_variable = self.mapping.new_individual_variable()
+        property_expression = ce.get_property()
+        assert isinstance(property_expression, OWLDataProperty)
+        cardinality = ce.get_cardinality()
+        if isinstance(ce, OWLDataMinCardinality):
+            comparator = ">="
+        elif isinstance(ce, OWLDataMaxCardinality):
+            comparator = "<="
+        elif isinstance(ce, OWLDataExactCardinality):
+            comparator = "="
+        else:
+            raise ValueError(ce)
+
+        self.append(f"{{ SELECT {subject_variable} WHERE {{ ")
+        self.append_triple(subject_variable, property_expression, object_variable)
+
+        filler = ce.get_filler()
+        with self.stack_variable(object_variable):
+            self.process(filler)
+
+        self.append(f" }} GROUP BY {subject_variable}"
+                    f" HAVING ( COUNT ( {object_variable} ) {comparator} {cardinality} ) }}")
+
+    # an overload of process function
+    # this overload is responsible for handling the exists operator combined with SELF
+    # general case: ∃r.SELF
+    @process.register
+    def _(self, ce: OWLObjectHasSelf):
+        subject = self.current_variable
+        property = ce.get_property()
+        self.append_triple(subject, property.get_named_property(), subject)
+
+    # an overload of process function
+    # this overload is responsible for handling the one of case (e.g., { john, jane }
+    # general case: { a1, ..., an }
+    @process.register
+    def _(self, ce: OWLObjectOneOf):
+        subject = self.current_variable
+        if self.modal_depth == 1:
+            self.append_triple(subject, "?p", "?o")
+
+        self.append(f" FILTER ( {subject} IN ( ")
+        first = True
+        for ind in ce.individuals():
+            if first:
+                first = False
+            else:
+                self.append(",")
+            assert isinstance(ind, OWLNamedIndividual)
+            self.append(f"<{ind.to_string_id()}>")
+        self.append(f" ) )")
+
+    @process.register
+    def _(self, ce: OWLDataSomeValuesFrom):
+        object_variable = self.mapping.new_individual_variable()
+        property_expression = ce.get_property()
+        assert isinstance(property_expression, OWLDataProperty)
+        self.append_triple(self.current_variable, property_expression, object_variable)
+        filler = ce.get_filler()
+        with self.stack_variable(object_variable):
+            self.process(filler)
+
+    @process.register
+    def _(self, ce: OWLDataAllValuesFrom):
+        subject = self.current_variable
+        object_variable = self.mapping.new_individual_variable()
+        property_expression = ce.get_property()
+        assert isinstance(property_expression, OWLDataProperty)
+        predicate = property_expression.to_string_id()
+        filler = ce.get_filler()
+
+        self.append_triple(self.current_variable, predicate, object_variable)
+
+        var = self.mapping.new_individual_variable()
+        cnt_var1 = self.new_count_var()
+        self.append(f"{{ SELECT {subject} ( COUNT( {var} ) AS {cnt_var1} ) WHERE {{ ")
+        self.append_triple(subject, predicate, var)
+        with self.stack_variable(var):
+            self.process(filler)
+        self.append(f" }} GROUP BY {subject} }}")
+
+        var = self.mapping.new_individual_variable()
+        cnt_var2 = self.new_count_var()
+        self.append(f"{{ SELECT {subject} ( COUNT( {var} ) AS {cnt_var2} ) WHERE {{ ")
+        self.append_triple(subject, predicate, var)
+        self.append(f" }} GROUP BY {subject} }}")
+
+        self.append(f" FILTER( {cnt_var1} = {cnt_var2} )")
+
+    @process.register
+    def _(self, ce: OWLDataHasValue):
+        property_expression = ce.get_property()
+        value = ce.get_filler()
+        assert isinstance(value, OWLDataProperty)
+        self.append_triple(self.current_variable, property_expression, value)
+
+    @process.register
+    def _(self, node: OWLDatatype):
+        if node != TopOWLDatatype:
+            self.append(f" FILTER ( DATATYPE ( {self.current_variable} = <{node.to_string_id()}> ) ) ")
+
+    @process.register
+    def _(self, node: OWLDataOneOf):
+        subject = self.current_variable
+        if self.modal_depth == 1:
+            self.append_triple(subject, "?p", "?o")
+        self.append(f" FILTER ( {subject} IN ( ")
+        first = True
+        for value in node.values():
+            if first:
+                first = False
+            else:
+                self.append(",")
+            if value:
+                self.append(self.render(value))
+        self.append(f" ) ) ")
+
+    @process.register
+    def _(self, node: OWLDatatypeRestriction):
+        frs = node.get_facet_restrictions()
+
+        for fr in frs:
+            facet = fr.get_facet()
+            value = fr.get_facet_value()
+
+            if facet in _Variable_facet_comp:
+                self.append(f' FILTER ( {self.current_variable} {_Variable_facet_comp[facet]}'
+                            f' "{value.get_literal()}"^^<{value.get_datatype().to_string_id()}> ) ')
+
+    def new_count_var(self) -> str:
+        self.cnt += 1
+        return f"?cnt_{self.cnt}"
+
+    def append_triple(self, subject, predicate, object_):
+        self.append(self.triple(subject, predicate, object_))
+
+    def append(self, frag):
+        self.sparql.append(frag)
+
+    def triple(self, subject, predicate, object_):
+        return f"{self._maybe_quote(subject)} {self._maybe_quote_p(predicate)} {self._maybe_render(object_)} . "
+
+    def as_query(self,
+                 root_variable: str,
+                 ce: OWLClassExpression,
+                 count: bool = False,
+                 values: Optional[Iterable[OWLNamedIndividual]] = None,
+                 named_individuals: bool = False)->str:
+        """
+        root variable: the variable that will be projected
+        ce: the class expression to be transformed to a SPARQL query
+        count: True, counts the results ; False, projects the individuals
+        values: positive or negative examples from a class expression problem
+        named_individuals: if set to True, the generated SPARQL query will return only entities that are instances
+        of owl:NamedIndividual
+
+        """
+
+        qs = ["SELECT"]
+        tp = self.convert(root_variable, ce, named_individuals)
+        if count:
+            qs.append(f" ( COUNT ( DISTINCT {root_variable} ) AS ?cnt ) WHERE {{ ")
+        else:
+            qs.append(f" DISTINCT {root_variable} WHERE {{ ")
+        if values is not None and root_variable.startswith("?"):
+            q = [f"VALUES {root_variable} {{ "]
+            for x in values:
+                q.append(f"<{x.to_string_id()}>")
+            q.append(f"}} . ")
+            qs.extend(q)
+        qs.extend(tp)
+        qs.append(f" }}")
+
+
+        query = "\n".join(qs)
+        parseQuery(query)
+        return query
+
+
+converter = Owl2SparqlConverter()
+
+
+def owl_expression_to_sparql(root_variable: str = "?x",
+                             expression: OWLClassExpression = None,
+                             values: Optional[Iterable[OWLNamedIndividual]] = None,
+                             named_individuals: bool = False)->str:
+    """Convert an OWL Class Expression (https://www.w3.org/TR/owl2-syntax/#Class_Expressions) into a SPARQL query
+     root variable: the variable that will be projected
+     expression: the class expression to be transformed to a SPARQL query
+
+     values: positive or negative examples from a class expression problem. Unclear
+     named_individuals: if set to True, the generated SPARQL query will return only entities
+     that are instances of owl:NamedIndividual
+    """
+    assert expression is not None, "expression cannot be None"
+    return converter.as_query(root_variable, expression, False, values, named_individuals)
```

### Comparing `owlapy-0.1.3/owlapy/owl_annotation.py` & `owlapy-1.0.0/owlapy/owl_annotation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-from abc import ABCMeta
-from .owlobject import OWLObject
-from typing import Optional
-
-
-class OWLAnnotationObject(OWLObject, metaclass=ABCMeta):
-    """A marker interface for the values (objects) of annotations."""
-    __slots__ = ()
-
-    # noinspection PyMethodMayBeStatic
-    def as_iri(self) -> Optional['IRI']:
-        """
-        Returns:
-            if the value is an IRI, return it. Return Mone otherwise.
-        """
-        return None
-
-    # noinspection PyMethodMayBeStatic
-    def as_anonymous_individual(self):
-        """
-        Returns:
-            if the value is an anonymous, return it. Return None otherwise.
-        """
-        return None
-
-class OWLAnnotationSubject(OWLAnnotationObject, metaclass=ABCMeta):
-    """A marker interface for annotation subjects, which can either be IRIs or anonymous individuals"""
-    __slots__ = ()
-    pass
-
-class OWLAnnotationValue(OWLAnnotationObject, metaclass=ABCMeta):
-    """A marker interface for annotation values, which can either be an IRI (URI), Literal or Anonymous Individual."""
-    __slots__ = ()
-
-    def is_literal(self) -> bool:
-        """
-        Returns:
-            true if the annotation value is a literal
-        """
-        return False
-
-    # noinspection PyMethodMayBeStatic
-    def as_literal(self) -> Optional['OWLLiteral']:
-        """
-        Returns:
-            if the value is a literal, returns it. Return None otherwise
-        """
+"""OWL Annotations"""
+from abc import ABCMeta
+from .owl_object import OWLObject
+from typing import Optional
+
+
+class OWLAnnotationObject(OWLObject, metaclass=ABCMeta):
+    """A marker interface for the values (objects) of annotations."""
+    __slots__ = ()
+
+    # noinspection PyMethodMayBeStatic
+    def as_iri(self) -> Optional['IRI']:
+        """
+        Returns:
+            if the value is an IRI, return it. Return Mone otherwise.
+        """
+        return None
+
+    # noinspection PyMethodMayBeStatic
+    def as_anonymous_individual(self):
+        """
+        Returns:
+            if the value is an anonymous, return it. Return None otherwise.
+        """
+        return None
+
+
+class OWLAnnotationSubject(OWLAnnotationObject, metaclass=ABCMeta):
+    """A marker interface for annotation subjects, which can either be IRIs or anonymous individuals"""
+    __slots__ = ()
+    pass
+
+
+class OWLAnnotationValue(OWLAnnotationObject, metaclass=ABCMeta):
+    """A marker interface for annotation values, which can either be an IRI (URI), Literal or Anonymous Individual."""
+    __slots__ = ()
+
+    def is_literal(self) -> bool:
+        """
+        Returns:
+            true if the annotation value is a literal
+        """
+        return False
+
+    # noinspection PyMethodMayBeStatic
+    def as_literal(self) -> Optional['OWLLiteral']:
+        """
+        Returns:
+            if the value is a literal, returns it. Return None otherwise
+        """
         return None
```

### Comparing `owlapy-0.1.3/owlapy/owl_axiom.py` & `owlapy-1.0.0/owlapy/owl_axiom.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1097 +1,1324 @@
-from abc import ABCMeta, abstractmethod
-
-from typing import TypeVar, List, Optional, Iterable, Generic, Final
-from .owl_property import OWLDataPropertyExpression, OWLObjectPropertyExpression
-from .owlobject import OWLObject, OWLEntity
-from .types import OWLDatatype, OWLDataRange
-from .meta_classes import HasOperands
-from .owl_property import OWLPropertyExpression, OWLProperty
-from .class_expression import OWLClassExpression, OWLClass
-from .owl_individual import OWLIndividual
-from .iri import IRI
-from owlapy.owl_annotation import OWLAnnotationSubject, OWLAnnotationValue
-from .owl_literal import OWLLiteral
-
-_C = TypeVar('_C', bound='OWLObject')  #:
-_P = TypeVar('_P', bound='OWLPropertyExpression')  #:
-_R = TypeVar('_R', bound='OWLPropertyRange')  #:
-
-class OWLAxiom(OWLObject, metaclass=ABCMeta):
-    """Represents Axioms in the OWL 2 Specification.
-
-    An OWL ontology contains a set of axioms. These axioms can be annotation axioms, declaration axioms, imports axioms
-    or logical axioms.
-    """
-    __slots__ = '_annotations'
-
-    _annotations: List['OWLAnnotation']
-
-    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._annotations = list(annotations) if annotations is not None else list()
-
-    def annotations(self) -> Optional[List['OWLAnnotation']]:
-        return self._annotations
-
-    def is_annotated(self) -> bool:
-        return self._annotations is not None and len(self._annotations) > 0
-
-    def is_logical_axiom(self) -> bool:
-        return False
-
-    def is_annotation_axiom(self) -> bool:
-        return False
-    # TODO: XXX
-
-
-class OWLLogicalAxiom(OWLAxiom, metaclass=ABCMeta):
-    """A base interface of all axioms that affect the logical meaning of an ontology. This excludes declaration axioms
-    (including imports declarations) and annotation axioms.
-    """
-    __slots__ = ()
-
-    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(annotations=annotations)
-
-    def is_logical_axiom(self) -> bool:
-        return True
-
-
-class OWLPropertyAxiom(OWLLogicalAxiom, metaclass=ABCMeta):
-    """The base interface for property axioms."""
-    __slots__ = ()
-
-    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(annotations=annotations)
-
-
-class OWLObjectPropertyAxiom(OWLPropertyAxiom, metaclass=ABCMeta):
-    """The base interface for object property axioms."""
-    __slots__ = ()
-
-
-class OWLDataPropertyAxiom(OWLPropertyAxiom, metaclass=ABCMeta):
-    """The base interface for data property axioms."""
-    __slots__ = ()
-
-
-class OWLIndividualAxiom(OWLLogicalAxiom, metaclass=ABCMeta):
-    """The base interface for individual axioms."""
-    __slots__ = ()
-
-    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(annotations=annotations)
-
-
-class OWLClassAxiom(OWLLogicalAxiom, metaclass=ABCMeta):
-    """The base interface for class axioms."""
-    __slots__ = ()
-
-    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(annotations=annotations)
-
-
-class OWLDeclarationAxiom(OWLAxiom):
-    """Represents a Declaration axiom in the OWL 2 Specification. A declaration axiom declares an entity in an ontology.
-       It doesn't affect the logical meaning of the ontology."""
-    __slots__ = '_entity'
-
-    _entity: OWLEntity
-
-    def __init__(self, entity: OWLEntity, annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._entity = entity
-        super().__init__(annotations=annotations)
-
-    def get_entity(self) -> OWLEntity:
-        return self._entity
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._entity == other._entity and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._entity, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLDeclarationAxiom(entity={self._entity},annotations={self._annotations})'
-
-
-class OWLDatatypeDefinitionAxiom(OWLLogicalAxiom):
-    """Represents a DatatypeDefinition axiom in the OWL 2 Specification."""
-    __slots__ = '_datatype', '_datarange'
-
-    _datatype: OWLDatatype
-    _datarange: OWLDataRange
-
-    def __init__(self, datatype: OWLDatatype, datarange: OWLDataRange,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._datatype = datatype
-        self._datarange = datarange
-        super().__init__(annotations=annotations)
-
-    def get_datatype(self) -> OWLDatatype:
-        return self._datatype
-
-    def get_datarange(self) -> OWLDataRange:
-        return self._datarange
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._datatype == other._datatype and self._datarange == other._datarange \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._datatype, self._datarange, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLDatatypeDefinitionAxiom(datatype={self._datatype},datarange={self._datarange},' \
-               f'annotations={self._annotations})'
-
-
-class OWLHasKeyAxiom(OWLLogicalAxiom, HasOperands[OWLPropertyExpression]):
-    """Represents a HasKey axiom in the OWL 2 Specification."""
-    __slots__ = '_class_expression', '_property_expressions'
-
-    _class_expression: OWLClassExpression
-    _property_expressions: List[OWLPropertyExpression]
-
-    def __init__(self, class_expression: OWLClassExpression, property_expressions: List[OWLPropertyExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._class_expression = class_expression
-        self._property_expressions = property_expressions
-        super().__init__(annotations=annotations)
-
-    def get_class_expression(self) -> OWLClassExpression:
-        return self._class_expression
-
-    def get_property_expressions(self) -> List[OWLPropertyExpression]:
-        return self._property_expressions
-
-    def operands(self) -> Iterable[OWLPropertyExpression]:
-        yield from self._property_expressions
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._class_expression == other._class_expression \
-                and self._property_expressions == other._property_expressions \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._class_expression, *self._property_expressions, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLHasKeyAxiom(class_expression={self._class_expression},' \
-               f'property_expressions={self._property_expressions},annotations={self._annotations})'
-
-
-class OWLNaryAxiom(Generic[_C], OWLAxiom, metaclass=ABCMeta):
-    """Represents an axiom that contains two or more operands that could also be represented with multiple pairwise
-    axioms.
-
-    Args:
-        _C: Class of contained objects.
-    """
-    __slots__ = ()
-
-    @abstractmethod
-    def as_pairwise_axioms(self) -> Iterable['OWLNaryAxiom[_C]']:
-        pass
-
-
-# noinspection PyUnresolvedReferences
-# noinspection PyDunderSlots
-class OWLNaryClassAxiom(OWLClassAxiom, OWLNaryAxiom[OWLClassExpression], metaclass=ABCMeta):
-    """Represents an axiom that contains two or more operands that could also be represented with
-        multiple pairwise axioms."""
-    __slots__ = '_class_expressions'
-    _class_expressions: List[OWLClassExpression]
-
-    @abstractmethod
-    def __init__(self, class_expressions: List[OWLClassExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._class_expressions = [*class_expressions]
-        super().__init__(annotations=annotations)
-
-    def class_expressions(self) -> Iterable[OWLClassExpression]:
-        """Gets all of the top level class expressions that appear in this axiom.
-
-        Returns:
-            Sorted stream of class expressions that appear in the axiom.
-        """
-        yield from self._class_expressions
-
-    def as_pairwise_axioms(self) -> Iterable['OWLNaryClassAxiom']:
-        """Gets this axiom as a set of pairwise axioms; if the axiom contains only two operands,
-        the axiom itself is returned unchanged, including its annotations.
-
-        Returns:
-            This axiom as a set of pairwise axioms.
-        """
-        if len(self._class_expressions) < 3:
-            yield self
-        else:
-            yield from map(type(self), combinations(self._class_expressions, 2))
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._class_expressions == other._class_expressions and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((*self._class_expressions, *self._annotations))
-
-    def __repr__(self):
-        return f'{type(self).__name__}({self._class_expressions},{self._annotations})'
-
-
-class OWLEquivalentClassesAxiom(OWLNaryClassAxiom):
-    """Represents an EquivalentClasses axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, class_expressions: List[OWLClassExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(class_expressions=class_expressions, annotations=annotations)
-
-    def contains_named_equivalent_class(self) -> bool:
-        return any(isinstance(ce, OWLClass) for ce in self._class_expressions)
-
-    def contains_owl_nothing(self) -> bool:
-        return any(isinstance(ce, OWLNothing) for ce in self._class_expressions)
-
-    def contains_owl_thing(self) -> bool:
-        return any(isinstance(ce, OWLThing) for ce in self._class_expressions)
-
-    def named_classes(self) -> Iterable[OWLClass]:
-        yield from (ce for ce in self._class_expressions if isinstance(ce, OWLClass))
-
-
-class OWLDisjointClassesAxiom(OWLNaryClassAxiom):
-    """Represents a DisjointClasses axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, class_expressions: List[OWLClassExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(class_expressions=class_expressions, annotations=annotations)
-
-
-class OWLNaryIndividualAxiom(OWLIndividualAxiom, OWLNaryAxiom[OWLIndividual], metaclass=ABCMeta):
-    """Represents an axiom that contains two or more operands that could also be represented with
-            multiple pairwise individual axioms."""
-    __slots__ = '_individuals'
-
-    _individuals: List[OWLIndividual]
-
-    @abstractmethod
-    def __init__(self, individuals: List[OWLIndividual],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._individuals = [*individuals]
-        super().__init__(annotations=annotations)
-
-    def individuals(self) -> Iterable[OWLIndividual]:
-        """Get the individuals.
-
-        Returns:
-            Generator containing the individuals.
-        """
-        yield from self._individuals
-
-    def as_pairwise_axioms(self) -> Iterable['OWLNaryIndividualAxiom']:
-        if len(self._individuals) < 3:
-            yield self
-        else:
-            yield from map(type(self), combinations(self._individuals, 2))
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._individuals == other._individuals and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((*self._individuals, *self._annotations))
-
-    def __repr__(self):
-        return f'{type(self).__name__}({self._individuals},{self._annotations})'
-
-
-class OWLDifferentIndividualsAxiom(OWLNaryIndividualAxiom):
-    """Represents a DifferentIndividuals axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, individuals: List[OWLIndividual],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(individuals=individuals, annotations=annotations)
-
-
-class OWLSameIndividualAxiom(OWLNaryIndividualAxiom):
-    """Represents a SameIndividual axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, individuals: List[OWLIndividual],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(individuals=individuals, annotations=annotations)
-
-
-class OWLNaryPropertyAxiom(Generic[_P], OWLPropertyAxiom, OWLNaryAxiom[_P], metaclass=ABCMeta):
-    """Represents an axiom that contains two or more operands that could also be represented with
-       multiple pairwise property axioms."""
-    __slots__ = '_properties'
-
-    _properties: List[_P]
-
-    @abstractmethod
-    def __init__(self, properties: List[_P], annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._properties = [*properties]
-        super().__init__(annotations=annotations)
-
-    def properties(self) -> Iterable[_P]:
-        """Get all the properties that appear in the axiom.
-
-        Returns:
-            Generator containing the properties.
-        """
-        yield from self._properties
-
-    def as_pairwise_axioms(self) -> Iterable['OWLNaryPropertyAxiom']:
-        if len(self._properties) < 3:
-            yield self
-        else:
-            yield from map(type(self), combinations(self._properties, 2))
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._properties == other._properties and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((*self._properties, *self._annotations))
-
-    def __repr__(self):
-        return f'{type(self).__name__}({self._properties},{self._annotations})'
-
-
-class OWLEquivalentObjectPropertiesAxiom(OWLNaryPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
-    """Represents EquivalentObjectProperties axioms in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, properties: List[OWLObjectPropertyExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(properties=properties, annotations=annotations)
-
-
-class OWLDisjointObjectPropertiesAxiom(OWLNaryPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
-    """Represents DisjointObjectProperties axioms in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, properties: List[OWLObjectPropertyExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(properties=properties, annotations=annotations)
-
-
-class OWLInverseObjectPropertiesAxiom(OWLNaryPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
-    """Represents InverseObjectProperties axioms in the OWL 2 Specification."""
-    __slots__ = '_first', '_second'
-
-    _first: OWLObjectPropertyExpression
-    _second: OWLObjectPropertyExpression
-
-    def __init__(self, first: OWLObjectPropertyExpression, second: OWLObjectPropertyExpression,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._first = first
-        self._second = second
-        super().__init__(properties=[first, second], annotations=annotations)
-
-    def get_first_property(self) -> OWLObjectPropertyExpression:
-        return self._first
-
-    def get_second_property(self) -> OWLObjectPropertyExpression:
-        return self._second
-
-    def __repr__(self):
-        return f'OWLInverseObjectPropertiesAxiom(first={self._first},second={self._second},' \
-               f'annotations={self._annotations})'
-
-
-class OWLEquivalentDataPropertiesAxiom(OWLNaryPropertyAxiom[OWLDataPropertyExpression], OWLDataPropertyAxiom):
-    """Represents EquivalentDataProperties axioms in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, properties: List[OWLDataPropertyExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(properties=properties, annotations=annotations)
-
-
-class OWLDisjointDataPropertiesAxiom(OWLNaryPropertyAxiom[OWLDataPropertyExpression], OWLDataPropertyAxiom):
-    """Represents DisjointDataProperties axioms in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, properties: List[OWLDataPropertyExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(properties=properties, annotations=annotations)
-
-
-class OWLSubClassOfAxiom(OWLClassAxiom):
-    """Represents an SubClassOf axiom in the OWL 2 Specification."""
-    __slots__ = '_sub_class', '_super_class'
-
-    _sub_class: OWLClassExpression
-    _super_class: OWLClassExpression
-
-    def __init__(self, sub_class: OWLClassExpression, super_class: OWLClassExpression,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        """Get an equivalent classes axiom with specified operands and no annotations.
-
-        Args:
-            sub_class: The sub-class.
-            super_class: The super class.
-            annotations: Annotations.
-        """
-        self._sub_class = sub_class
-        self._super_class = super_class
-        super().__init__(annotations=annotations)
-
-    def get_sub_class(self) -> OWLClassExpression:
-        return self._sub_class
-
-    def get_super_class(self) -> OWLClassExpression:
-        return self._super_class
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._super_class == other._super_class and self._sub_class == other._sub_class \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._super_class, self._sub_class, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLSubClassOfAxiom(sub_class={self._sub_class},super_class={self._super_class},' \
-               f'annotations={self._annotations})'
-
-
-class OWLDisjointUnionAxiom(OWLClassAxiom):
-    """Represents a DisjointUnion axiom in the OWL 2 Specification."""
-    __slots__ = '_cls', '_class_expressions'
-
-    _cls: OWLClass
-    _class_expressions: List[OWLClassExpression]
-
-    def __init__(self, cls_: OWLClass, class_expressions: List[OWLClassExpression],
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._cls = cls_
-        self._class_expressions = class_expressions
-        super().__init__(annotations=annotations)
-
-    def get_owl_class(self) -> OWLClass:
-        return self._cls
-
-    def get_class_expressions(self) -> Iterable[OWLClassExpression]:
-        yield from self._class_expressions
-
-    def get_owl_equivalent_classes_axiom(self) -> OWLEquivalentClassesAxiom:
-        return OWLEquivalentClassesAxiom(self._cls, OWLObjectUnionOf(self._class_expressions))
-
-    def get_owl_disjoint_classes_axiom(self) -> OWLDisjointClassesAxiom:
-        return OWLDisjointClassesAxiom(self._class_expressions)
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._cls == other._cls and self._class_expressions == other._class_expressions \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._cls, *self._class_expressions, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLDisjointUnionAxiom(class={self._cls},class_expressions={self._class_expressions},' \
-               f'annotations={self._annotations})'
-
-
-class OWLClassAssertionAxiom(OWLIndividualAxiom):
-    """Represents ClassAssertion axioms in the OWL 2 Specification."""
-    __slots__ = '_individual', '_class_expression'
-
-    _individual: OWLIndividual
-    _class_expression: OWLClassExpression
-
-    def __init__(self, individual: OWLIndividual, class_expression: OWLClassExpression,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        """Get a ClassAssertion axiom for the specified individual and class expression.
-        Args:
-            individual: The individual.
-            class_expression: The class the individual belongs to.
-            annotations: Annotations.
-        """
-        self._individual = individual
-        self._class_expression = class_expression
-        super().__init__(annotations=annotations)
-
-    def get_individual(self) -> OWLIndividual:
-        return self._individual
-
-    def get_class_expression(self) -> OWLClassExpression:
-        return self._class_expression
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._class_expression == other._class_expression and self._individual == other._individual \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._individual, self._class_expression, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLClassAssertionAxiom(individual={self._individual},class_expression={self._class_expression},' \
-               f'annotations={self._annotations})'
-class OWLAnnotationProperty(OWLProperty):
-    """Represents an AnnotationProperty in the OWL 2 specification."""
-    __slots__ = '_iri'
-
-    _iri: IRI
-
-    def __init__(self, iri: IRI):
-        """Get a new OWLAnnotationProperty object.
-
-        Args:
-            iri: New OWLAnnotationProperty IRI.
-        """
-        self._iri = iri
-
-    def get_iri(self) -> IRI:
-        # documented in parent
-        return self._iri
-
-class OWLAnnotation(OWLObject):
-    """Annotations are used in the various types of annotation axioms, which bind annotations to their subjects
-    (i.e. axioms or declarations)."""
-    __slots__ = '_property', '_value'
-
-    _property: OWLAnnotationProperty
-    _value: OWLAnnotationValue
-
-    def __init__(self, property: OWLAnnotationProperty, value: OWLAnnotationValue):
-        """Gets an annotation.
-
-        Args:
-            property: the annotation property.
-            value: The annotation value.
-        """
-        self._property = property
-        self._value = value
-
-    def get_property(self) -> OWLAnnotationProperty:
-        """Gets the property that this annotation acts along.
-
-        Returns:
-            The annotation property.
-        """
-        return self._property
-
-    def get_value(self) -> OWLAnnotationValue:
-        """Gets the annotation value. The type of value will depend upon the type of the annotation e.g. whether the
-        annotation is an OWLLiteral, an IRI or an OWLAnonymousIndividual.
-
-        Returns:
-            The annotation value.
-        """
-        return self._value
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._property == other._property and self._value == other._value
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._property, self._value))
-
-    def __repr__(self):
-        return f'OWLAnnotation({self._property}, {self._value})'
-class OWLAnnotationAxiom(OWLAxiom, metaclass=ABCMeta):
-    """A super interface for annotation axioms."""
-    __slots__ = ()
-
-    def is_annotation_axiom(self) -> bool:
-        return True
-class OWLAnnotationAssertionAxiom(OWLAnnotationAxiom):
-    """Represents AnnotationAssertion axioms in the OWL 2 specification."""
-    __slots__ = '_subject', '_annotation'
-
-    _subject: OWLAnnotationSubject
-    _annotation: OWLAnnotation
-
-    def __init__(self, subject: OWLAnnotationSubject, annotation: OWLAnnotation):
-        """Get an annotation assertion axiom - with annotations.
-
-        Args:
-            subject: Subject.
-            annotation: Annotation.
-        """
-        assert isinstance(subject, OWLAnnotationSubject)
-        assert isinstance(annotation, OWLAnnotation)
-
-        self._subject = subject
-        self._annotation = annotation
-
-    def get_subject(self) -> OWLAnnotationSubject:
-        """Gets the subject of this object.
-
-        Returns:
-            The subject.
-        """
-        return self._subject
-
-    def get_property(self) -> OWLAnnotationProperty:
-        """Gets the property.
-
-        Returns:
-            The property.
-        """
-        return self._annotation.get_property()
-
-    def get_value(self) -> OWLAnnotationValue:
-        """Gets the annotation value. This is either an IRI, an OWLAnonymousIndividual or an OWLLiteral.
-
-        Returns:
-            The annotation value.
-        """
-        return self._annotation.get_value()
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._subject == other._subject and self._annotation == other._annotation
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._subject, self._annotation))
-
-    def __repr__(self):
-        return f'OWLAnnotationAssertionAxiom({self._subject}, {self._annotation})'
-class OWLSubAnnotationPropertyOfAxiom(OWLAnnotationAxiom):
-    """Represents an SubAnnotationPropertyOf axiom in the OWL 2 specification."""
-    __slots__ = '_sub_property', '_super_property'
-
-    _sub_property: OWLAnnotationProperty
-    _super_property: OWLAnnotationProperty
-
-    def __init__(self, sub_property: OWLAnnotationProperty, super_property: OWLAnnotationProperty,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._sub_property = sub_property
-        self._super_property = super_property
-        super().__init__(annotations=annotations)
-
-    def get_sub_property(self) -> OWLAnnotationProperty:
-        return self._sub_property
-
-    def get_super_property(self) -> OWLAnnotationProperty:
-        return self._super_property
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._sub_property == other._sub_property and self._super_property == other._super_property \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._sub_property, self._super_property, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLSubAnnotationPropertyOfAxiom(sub_property={self._sub_property},' \
-               f'super_property={self._super_property},annotations={self._annotations})'
-class OWLAnnotationPropertyDomainAxiom(OWLAnnotationAxiom):
-    """Represents an AnnotationPropertyDomain axiom in the OWL 2 specification."""
-    __slots__ = '_property', '_domain'
-
-    _property: OWLAnnotationProperty
-    _domain: IRI
-
-    def __init__(self, property_: OWLAnnotationProperty, domain: IRI,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._property = property_
-        self._domain = domain
-        super().__init__(annotations=annotations)
-
-    def get_property(self) -> OWLAnnotationProperty:
-        return self._property
-
-    def get_domain(self) -> IRI:
-        return self._domain
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._property == other._property and self._domain == other._domain \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._property, self._domain, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLAnnotationPropertyDomainAxiom({repr(self._property)},{repr(self._domain)},' \
-               f'{repr(self._annotations)})'
-class OWLAnnotationPropertyRangeAxiom(OWLAnnotationAxiom):
-    """Represents an AnnotationPropertyRange axiom in the OWL 2 specification."""
-    __slots__ = '_property', '_range'
-
-    _property: OWLAnnotationProperty
-    _range: IRI
-
-    def __init__(self, property_: OWLAnnotationProperty, range_: IRI,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._property = property_
-        self._range = range_
-        super().__init__(annotations=annotations)
-
-    def get_property(self) -> OWLAnnotationProperty:
-        return self._property
-
-    def get_range(self) -> IRI:
-        return self._range
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._property == other._property and self._range == other._range \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._property, self._range, *self._annotations))
-
-    def __repr__(self):
-        return f'OWLAnnotationPropertyRangeAxiom({repr(self._property)},{repr(self._range)},' \
-               f'{repr(self._annotations)})'
-class OWLSubPropertyAxiom(Generic[_P], OWLPropertyAxiom):
-    """
-    Base interface for object and data sub-property axioms.
-    """
-    __slots__ = '_sub_property', '_super_property'
-
-    _sub_property: _P
-    _super_property: _P
-
-    @abstractmethod
-    def __init__(self, sub_property: _P, super_property: _P,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        self._sub_property = sub_property
-        self._super_property = super_property
-        super().__init__(annotations=annotations)
-
-    def get_sub_property(self) -> _P:
-        return self._sub_property
-
-    def get_super_property(self) -> _P:
-        return self._super_property
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._sub_property == other._sub_property and self._super_property == other._super_property \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._sub_property, self._super_property, *self._annotations))
-
-    def __repr__(self):
-        return f'{type(self).__name__}(sub_property={self._sub_property},super_property={self._super_property},' \
-               f'annotations={self._annotations})'
-class OWLSubObjectPropertyOfAxiom(OWLSubPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
-    """Represents a SubObjectPropertyOf axiom in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, sub_property: OWLObjectPropertyExpression, super_property: OWLObjectPropertyExpression,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(sub_property=sub_property, super_property=super_property, annotations=annotations)
-class OWLSubDataPropertyOfAxiom(OWLSubPropertyAxiom[OWLDataPropertyExpression], OWLDataPropertyAxiom):
-    """Represents a SubDataPropertyOf axiom in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, sub_property: OWLDataPropertyExpression, super_property: OWLDataPropertyExpression,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(sub_property=sub_property, super_property=super_property, annotations=annotations)
-
-class OWLPropertyAssertionAxiom(Generic[_P, _C], OWLIndividualAxiom, metaclass=ABCMeta):
-    """Represents a PropertyAssertion axiom in the OWL 2 specification."""
-    __slots__ = '_subject', '_property', '_object'
-
-    _subject: OWLIndividual
-    _property: _P
-    _object: _C
-
-    @abstractmethod
-    def __init__(self, subject: OWLIndividual, property_: _P, object_: _C,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        """Get a PropertyAssertion axiom for the specified subject, property, object.
-        Args:
-            subject: The subject of the property assertion.
-            property_: The property of the property assertion.
-            object_: The object of the property assertion.
-            annotations: Annotations.
-        """
-        assert isinstance(subject, OWLIndividual)
-
-        self._subject = subject
-        self._property = property_
-        self._object = object_
-        super().__init__(annotations=annotations)
-
-    def get_subject(self) -> OWLIndividual:
-        return self._subject
-
-    def get_property(self) -> _P:
-        return self._property
-
-    def get_object(self) -> _C:
-        return self._object
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._subject == other._subject and self._property == other._property and \
-                self._object == other._object and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._subject, self._property, self._object, *self._annotations))
-
-    def __repr__(self):
-        return f'{type(self).__name__}(subject={self._subject},property={self._property},' \
-               f'object={self._object},annotation={self._annotations})'
-class OWLObjectPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLObjectPropertyExpression, OWLIndividual]):
-    """Represents an ObjectPropertyAssertion axiom in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, subject: OWLIndividual, property_: OWLObjectPropertyExpression, object_: OWLIndividual,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(subject, property_, object_, annotations)
-class OWLNegativeObjectPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLObjectPropertyExpression, OWLIndividual]):
-    """Represents a NegativeObjectPropertyAssertion axiom in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, subject: OWLIndividual, property_: OWLObjectPropertyExpression, object_: OWLIndividual,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(subject, property_, object_, annotations)
-class OWLDataPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLDataPropertyExpression, OWLLiteral]):
-    """Represents an DataPropertyAssertion axiom in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, subject: OWLIndividual, property_: OWLDataPropertyExpression, object_: OWLLiteral,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(subject, property_, object_, annotations)
-class OWLNegativeDataPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLDataPropertyExpression, OWLLiteral]):
-    """Represents an NegativeDataPropertyAssertion axiom in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, subject: OWLIndividual, property_: OWLDataPropertyExpression, object_: OWLLiteral,
-                 annotations: Optional[Iterable['OWLAnnotation']] = None):
-        super().__init__(subject, property_, object_, annotations)
-class OWLUnaryPropertyAxiom(Generic[_P], OWLPropertyAxiom, metaclass=ABCMeta):
-    """Unary property axiom."""
-    __slots__ = '_property'
-
-    _property: _P
-
-    def __init__(self, property_: _P, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        self._property = property_
-        super().__init__(annotations=annotations)
-
-    def get_property(self) -> _P:
-        return self._property
-
-
-class OWLObjectPropertyCharacteristicAxiom(OWLUnaryPropertyAxiom[OWLObjectPropertyExpression],
-                                           OWLObjectPropertyAxiom, metaclass=ABCMeta):
-    """Base interface for functional object property axiom."""
-    __slots__ = ()
-
-    @abstractmethod
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._property == other._property and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._property, *self._annotations))
-
-    def __repr__(self):
-        return f"{type(self).__name__}({repr(self._property)},{repr(self._annotations)})"
-
-
-class OWLFunctionalObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
-    """Represents FunctionalObjectProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLAsymmetricObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
-    """Represents AsymmetricObjectProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLInverseFunctionalObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
-    """Represents InverseFunctionalObjectProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLIrreflexiveObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
-    """Represents IrreflexiveObjectProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLReflexiveObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
-    """Represents ReflexiveObjectProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLSymmetricObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
-    """Represents SymmetricObjectProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLTransitiveObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
-    """Represents TransitiveObjectProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLDataPropertyCharacteristicAxiom(OWLUnaryPropertyAxiom[OWLDataPropertyExpression],
-                                         OWLDataPropertyAxiom, metaclass=ABCMeta):
-    """Base interface for Functional data property axiom."""
-    __slots__ = ()
-
-    @abstractmethod
-    def __init__(self, property_: OWLDataPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._property == other._property and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._property, *self._annotations))
-
-    def __repr__(self):
-        return f"{type(self).__name__}({repr(self._property)},{repr(self._annotations)})"
-
-
-class OWLFunctionalDataPropertyAxiom(OWLDataPropertyCharacteristicAxiom):
-    """Represents FunctionalDataProperty axioms in the OWL 2 specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLDataPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, annotations=annotations)
-
-
-class OWLPropertyDomainAxiom(Generic[_P], OWLUnaryPropertyAxiom[_P], metaclass=ABCMeta):
-    """Represents ObjectPropertyDomain axioms in the OWL 2 specification."""
-    __slots__ = '_domain'
-
-    _domain: OWLClassExpression
-
-    @abstractmethod
-    def __init__(self, property_: _P, domain: OWLClassExpression,
-                 annotations: Optional[Iterable[OWLAnnotation]] = None):
-        self._domain = domain
-        super().__init__(property_=property_, annotations=annotations)
-
-    def get_domain(self) -> OWLClassExpression:
-        return self._domain
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._property == other._property and self._domain == other._domain \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._property, self._domain, *self._annotations))
-
-    def __repr__(self):
-        return f"{type(self).__name__}({repr(self._property)},{repr(self._domain)},{repr(self._annotations)})"
-
-
-class OWLPropertyRangeAxiom(Generic[_P, _R], OWLUnaryPropertyAxiom[_P], metaclass=ABCMeta):
-    """Represents ObjectPropertyRange axioms in the OWL 2 specification."""
-    __slots__ = '_range'
-
-    _range: _R
-
-    @abstractmethod
-    def __init__(self, property_: _P, range_: _R, annotations: Optional[Iterable[OWLAnnotation]] = None):
-        self._range = range_
-        super().__init__(property_=property_, annotations=annotations)
-
-    def get_range(self) -> _R:
-        return self._range
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self._property == other._property and self._range == other._range \
-                and self._annotations == other._annotations
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self._property, self._range, *self._annotations))
-
-    def __repr__(self):
-        return f"{type(self).__name__}({repr(self._property)},{repr(self._range)},{repr(self._annotations)})"
-
-
-class OWLObjectPropertyDomainAxiom(OWLPropertyDomainAxiom[OWLObjectPropertyExpression]):
-    """ Represents a ObjectPropertyDomain axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, domain: OWLClassExpression,
-                 annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, domain=domain, annotations=annotations)
-
-
-class OWLDataPropertyDomainAxiom(OWLPropertyDomainAxiom[OWLDataPropertyExpression]):
-    """ Represents a DataPropertyDomain axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLDataPropertyExpression, domain: OWLClassExpression,
-                 annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, domain=domain, annotations=annotations)
-
-
-class OWLObjectPropertyRangeAxiom(OWLPropertyRangeAxiom[OWLObjectPropertyExpression, OWLClassExpression]):
-    """ Represents a ObjectPropertyRange axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLObjectPropertyExpression, range_: OWLClassExpression,
-                 annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, range_=range_, annotations=annotations)
-
-
-class OWLDataPropertyRangeAxiom(OWLPropertyRangeAxiom[OWLDataPropertyExpression, OWLDataRange]):
-    """ Represents a DataPropertyRange axiom in the OWL 2 Specification."""
-    __slots__ = ()
-
-    def __init__(self, property_: OWLDataPropertyExpression, range_: OWLDataRange,
-                 annotations: Optional[Iterable[OWLAnnotation]] = None):
-        super().__init__(property_=property_, range_=range_, annotations=annotations)
+"""OWL Axioms"""
+from abc import ABCMeta, abstractmethod
+
+from typing import TypeVar, List, Optional, Iterable, Generic, Final, Union
+from .owl_property import OWLDataPropertyExpression, OWLObjectPropertyExpression
+from .owl_object import OWLObject, OWLEntity
+from .owl_datatype import OWLDatatype, OWLDataRange
+from .meta_classes import HasOperands
+from .owl_property import OWLPropertyExpression, OWLProperty
+from .class_expression import OWLClassExpression, OWLClass
+from .owl_individual import OWLIndividual
+from .iri import IRI
+from owlapy.owl_annotation import OWLAnnotationSubject, OWLAnnotationValue
+from .owl_literal import OWLLiteral
+
+_C = TypeVar('_C', bound='OWLObject')  #:
+_P = TypeVar('_P', bound='OWLPropertyExpression')  #:
+_R = TypeVar('_R', bound='OWLPropertyRange')  #:
+
+
+class OWLAxiom(OWLObject, metaclass=ABCMeta):
+    """Represents Axioms in the OWL 2 Specification.
+
+    An OWL ontology contains a set of axioms. These axioms can be annotation axioms, declaration axioms, imports axioms
+    or logical axioms.
+    """
+    __slots__ = '_annotations'
+
+    _annotations: List['OWLAnnotation']
+
+    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._annotations = list(annotations) if annotations is not None else list()
+
+    def annotations(self) -> Optional[List['OWLAnnotation']]:
+        return self._annotations
+
+    def is_annotated(self) -> bool:
+        return self._annotations is not None and len(self._annotations) > 0
+
+    def is_logical_axiom(self) -> bool:
+        return False
+
+    def is_annotation_axiom(self) -> bool:
+        return False
+    # TODO: XXX
+
+
+class OWLLogicalAxiom(OWLAxiom, metaclass=ABCMeta):
+    """A base interface of all axioms that affect the logical meaning of an ontology. This excludes declaration
+    axioms (including imports declarations) and annotation axioms.
+    """
+    __slots__ = ()
+
+    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(annotations=annotations)
+
+    def is_logical_axiom(self) -> bool:
+        return True
+
+
+class OWLPropertyAxiom(OWLLogicalAxiom, metaclass=ABCMeta):
+    """The base interface for property axioms."""
+    __slots__ = ()
+
+    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(annotations=annotations)
+
+
+class OWLObjectPropertyAxiom(OWLPropertyAxiom, metaclass=ABCMeta):
+    """The base interface for object property axioms."""
+    __slots__ = ()
+
+
+class OWLDataPropertyAxiom(OWLPropertyAxiom, metaclass=ABCMeta):
+    """The base interface for data property axioms."""
+    __slots__ = ()
+
+
+class OWLIndividualAxiom(OWLLogicalAxiom, metaclass=ABCMeta):
+    """The base interface for individual axioms."""
+    __slots__ = ()
+
+    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(annotations=annotations)
+
+
+class OWLClassAxiom(OWLLogicalAxiom, metaclass=ABCMeta):
+    """The base interface for class axioms."""
+    __slots__ = ()
+
+    def __init__(self, annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(annotations=annotations)
+
+
+class OWLDeclarationAxiom(OWLAxiom):
+    """Represents a Declaration axiom in the OWL 2 Specification. A declaration axiom declares an entity in an ontology.
+       It doesn't affect the logical meaning of the ontology."""
+    __slots__ = '_entity'
+
+    _entity: OWLEntity
+
+    def __init__(self, entity: OWLEntity, annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._entity = entity
+        super().__init__(annotations=annotations)
+
+    def get_entity(self) -> OWLEntity:
+        return self._entity
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._entity == other._entity and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._entity, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLDeclarationAxiom(entity={self._entity},annotations={self._annotations})'
+
+
+class OWLDatatypeDefinitionAxiom(OWLLogicalAxiom):
+    """A datatype definition DatatypeDefinition( DT DR ) defines a new datatype DT as being semantically
+    equivalent to the data range DR; the latter must be a unary data range. This axiom allows one to use
+    the defined datatype DT as a synonym for DR — that is, in any expression in the ontology containing
+    such an axiom, DT can be replaced with DR without affecting the meaning of the ontology.
+
+    (https://www.w3.org/TR/owl2-syntax/#Datatype_Definitions)"""
+    __slots__ = '_datatype', '_datarange'
+
+    _datatype: OWLDatatype
+    _datarange: OWLDataRange
+
+    def __init__(self, datatype: OWLDatatype, datarange: OWLDataRange,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._datatype = datatype
+        self._datarange = datarange
+        super().__init__(annotations=annotations)
+
+    def get_datatype(self) -> OWLDatatype:
+        return self._datatype
+
+    def get_datarange(self) -> OWLDataRange:
+        return self._datarange
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._datatype == other._datatype and self._datarange == other._datarange \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._datatype, self._datarange, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLDatatypeDefinitionAxiom(datatype={self._datatype},datarange={self._datarange},' \
+               f'annotations={self._annotations})'
+
+
+class OWLHasKeyAxiom(OWLLogicalAxiom, HasOperands[OWLPropertyExpression]):
+    """A key axiom HasKey( CE ( OPE1 ... OPEm ) ( DPE1 ... DPEn ) ) states that each
+    (named) instance of the class expression CE is uniquely identified by the object
+    property expressions OPEi and/or the data property expressions DPEj — that is,
+    no two distinct (named) instances of CE can coincide on the values of all
+    object property expressions OPEi and all data property expressions DPEj. In each
+    such axiom in an OWL ontology, m or n (or both) must be larger than zero. A key
+    axiom of the form HasKey( owl:Thing ( OPE ) () ) is similar to the axiom
+    InverseFunctionalObjectProperty( OPE ), the main differences being that the
+    former axiom is applicable only to individuals that are explicitly named in an
+    ontology, while the latter axiom is also applicable to anonymous individuals and
+    individuals whose existence is implied by existential quantification.
+
+    (https://www.w3.org/TR/owl2-syntax/#Keys)
+    """
+    __slots__ = '_class_expression', '_property_expressions'
+
+    _class_expression: OWLClassExpression
+    _property_expressions: List[OWLPropertyExpression]
+
+    def __init__(self, class_expression: OWLClassExpression, property_expressions: List[OWLPropertyExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._class_expression = class_expression
+        self._property_expressions = property_expressions
+        super().__init__(annotations=annotations)
+
+    def get_class_expression(self) -> OWLClassExpression:
+        return self._class_expression
+
+    def get_property_expressions(self) -> List[OWLPropertyExpression]:
+        return self._property_expressions
+
+    def operands(self) -> Iterable[OWLPropertyExpression]:
+        yield from self._property_expressions
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._class_expression == other._class_expression \
+                and self._property_expressions == other._property_expressions \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._class_expression, *self._property_expressions, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLHasKeyAxiom(class_expression={self._class_expression},' \
+               f'property_expressions={self._property_expressions},annotations={self._annotations})'
+
+
+class OWLNaryAxiom(Generic[_C], OWLAxiom, metaclass=ABCMeta):
+    """Represents an axiom that contains two or more operands that could also be represented with multiple pairwise
+    axioms.
+
+    Args:
+        _C: Class of contained objects.
+    """
+    __slots__ = ()
+
+    @abstractmethod
+    def as_pairwise_axioms(self) -> Iterable['OWLNaryAxiom[_C]']:
+        pass
+
+
+# noinspection PyUnresolvedReferences
+# noinspection PyDunderSlots
+class OWLNaryClassAxiom(OWLClassAxiom, OWLNaryAxiom[OWLClassExpression], metaclass=ABCMeta):
+    """Represents an axiom that contains two or more operands that could also be represented with
+        multiple pairwise axioms."""
+    __slots__ = '_class_expressions'
+    _class_expressions: List[OWLClassExpression]
+
+    @abstractmethod
+    def __init__(self, class_expressions: List[OWLClassExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._class_expressions = [*class_expressions]
+        super().__init__(annotations=annotations)
+
+    def class_expressions(self) -> Iterable[OWLClassExpression]:
+        """Gets all of the top level class expressions that appear in this axiom.
+
+        Returns:
+            Sorted stream of class expressions that appear in the axiom.
+        """
+        yield from self._class_expressions
+
+    def as_pairwise_axioms(self) -> Iterable['OWLNaryClassAxiom']:
+        """Gets this axiom as a set of pairwise axioms; if the axiom contains only two operands,
+        the axiom itself is returned unchanged, including its annotations.
+
+        Returns:
+            This axiom as a set of pairwise axioms.
+        """
+        if len(self._class_expressions) < 3:
+            yield self
+        else:
+            yield from map(type(self), combinations(self._class_expressions, 2))
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._class_expressions == other._class_expressions and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((*self._class_expressions, *self._annotations))
+
+    def __repr__(self):
+        return f'{type(self).__name__}({self._class_expressions},{self._annotations})'
+
+
+class OWLEquivalentClassesAxiom(OWLNaryClassAxiom):
+    """An equivalent classes axiom EquivalentClasses( CE1 ... CEn ) states that all of the class expressions CEi,
+    1 ≤ i ≤ n, are semantically equivalent to each other. This axiom allows one to use each CEi as a synonym
+    for each CEj — that is, in any expression in the ontology containing such an axiom, CEi can be replaced
+    with CEj without affecting the meaning of the ontology.
+
+    (https://www.w3.org/TR/owl2-syntax/#Equivalent_Classes)
+    """
+    __slots__ = ()
+
+    def __init__(self, class_expressions: List[OWLClassExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(class_expressions=class_expressions, annotations=annotations)
+
+    def contains_named_equivalent_class(self) -> bool:
+        return any(isinstance(ce, OWLClass) for ce in self._class_expressions)
+
+    def contains_owl_nothing(self) -> bool:
+        return any(isinstance(ce, OWLNothing) for ce in self._class_expressions)
+
+    def contains_owl_thing(self) -> bool:
+        return any(isinstance(ce, OWLThing) for ce in self._class_expressions)
+
+    def named_classes(self) -> Iterable[OWLClass]:
+        yield from (ce for ce in self._class_expressions if isinstance(ce, OWLClass))
+
+
+class OWLDisjointClassesAxiom(OWLNaryClassAxiom):
+    """A disjoint classes axiom DisjointClasses( CE1 ... CEn ) states that all of the class expressions CEi, 1 ≤ i ≤ n,
+    are pairwise disjoint; that is, no individual can be at the same time an instance of both CEi and CEj for i ≠ j.
+
+    (https://www.w3.org/TR/owl2-syntax/#Disjoint_Classes)
+    """
+    __slots__ = ()
+
+    def __init__(self, class_expressions: List[OWLClassExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(class_expressions=class_expressions, annotations=annotations)
+
+
+class OWLNaryIndividualAxiom(OWLIndividualAxiom, OWLNaryAxiom[OWLIndividual], metaclass=ABCMeta):
+    """Represents an axiom that contains two or more operands that could also be represented with
+            multiple pairwise individual axioms."""
+    __slots__ = '_individuals'
+
+    _individuals: List[OWLIndividual]
+
+    @abstractmethod
+    def __init__(self, individuals: List[OWLIndividual],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._individuals = [*individuals]
+        super().__init__(annotations=annotations)
+
+    def individuals(self) -> Iterable[OWLIndividual]:
+        """Get the individuals.
+
+        Returns:
+            Generator containing the individuals.
+        """
+        yield from self._individuals
+
+    def as_pairwise_axioms(self) -> Iterable['OWLNaryIndividualAxiom']:
+        if len(self._individuals) < 3:
+            yield self
+        else:
+            yield from map(type(self), combinations(self._individuals, 2))
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._individuals == other._individuals and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((*self._individuals, *self._annotations))
+
+    def __repr__(self):
+        return f'{type(self).__name__}({self._individuals},{self._annotations})'
+
+
+class OWLDifferentIndividualsAxiom(OWLNaryIndividualAxiom):
+    """An individual inequality axiom DifferentIndividuals( a1 ... an ) states that all of the individuals ai,
+      1 ≤ i ≤ n, are different from each other; that is, no individuals ai and aj with i ≠ j can be derived to be equal.
+      This axiom can be used to axiomatize the unique name assumption — the assumption that all different individual
+      names denote different individuals. (https://www.w3.org/TR/owl2-syntax/#Individual_Inequality)
+      """
+    __slots__ = ()
+
+    def __init__(self, individuals: List[OWLIndividual],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(individuals=individuals, annotations=annotations)
+
+
+class OWLSameIndividualAxiom(OWLNaryIndividualAxiom):
+    """An individual equality axiom SameIndividual( a1 ... an ) states that all of the individuals ai, 1 ≤ i ≤ n,
+    are equal to each other. This axiom allows one to use each ai as a synonym for each aj — that is, in any
+    expression in the ontology containing such an axiom, ai can be replaced with aj without affecting the
+    meaning of the ontology.
+
+    (https://www.w3.org/TR/owl2-syntax/#Individual_Equality)
+    """
+    __slots__ = ()
+
+    def __init__(self, individuals: List[OWLIndividual],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(individuals=individuals, annotations=annotations)
+
+
+class OWLNaryPropertyAxiom(Generic[_P], OWLPropertyAxiom, OWLNaryAxiom[_P], metaclass=ABCMeta):
+    """Represents an axiom that contains two or more operands that could also be represented with
+       multiple pairwise property axioms."""
+    __slots__ = '_properties'
+
+    _properties: List[_P]
+
+    @abstractmethod
+    def __init__(self, properties: List[_P], annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._properties = [*properties]
+        super().__init__(annotations=annotations)
+
+    def properties(self) -> Iterable[_P]:
+        """Get all the properties that appear in the axiom.
+
+        Returns:
+            Generator containing the properties.
+        """
+        yield from self._properties
+
+    def as_pairwise_axioms(self) -> Iterable['OWLNaryPropertyAxiom']:
+        if len(self._properties) < 3:
+            yield self
+        else:
+            yield from map(type(self), combinations(self._properties, 2))
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._properties == other._properties and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((*self._properties, *self._annotations))
+
+    def __repr__(self):
+        return f'{type(self).__name__}({self._properties},{self._annotations})'
+
+
+class OWLEquivalentObjectPropertiesAxiom(OWLNaryPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
+    """An equivalent object properties axiom EquivalentObjectProperties( OPE1 ... OPEn ) states that all of the object
+    property expressions OPEi, 1 ≤ i ≤ n, are semantically equivalent to each other. This axiom allows one to use each
+    OPEi as a synonym for each OPEj — that is, in any expression in the ontology containing such an axiom, OPEi can be
+    replaced with OPEj without affecting the meaning of the ontology.
+
+    (https://www.w3.org/TR/owl2-syntax/#Equivalent_Object_Properties)
+    """
+    __slots__ = ()
+
+    def __init__(self, properties: List[OWLObjectPropertyExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(properties=properties, annotations=annotations)
+
+
+class OWLDisjointObjectPropertiesAxiom(OWLNaryPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
+    """A disjoint object properties axiom DisjointObjectProperties( OPE1 ... OPEn ) states that all of the object
+     property expressions OPEi, 1 ≤ i ≤ n, are pairwise disjoint; that is, no individual x can be connected to an
+     individual y by both OPEi and OPEj for i ≠ j.
+
+     (https://www.w3.org/TR/owl2-syntax/#Disjoint_Object_Properties)"""
+    __slots__ = ()
+
+    def __init__(self, properties: List[OWLObjectPropertyExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(properties=properties, annotations=annotations)
+
+
+class OWLInverseObjectPropertiesAxiom(OWLNaryPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
+    """An inverse object properties axiom InverseObjectProperties( OPE1 OPE2 ) states that the object property
+    expression OPE1 is an inverse of the object property expression OPE2. Thus, if an individual x is connected by
+    OPE1 to an individual y, then y is also connected by OPE2 to x, and vice versa.
+
+    (https://www.w3.org/TR/owl2-syntax/#Inverse_Object_Properties_2)
+    """
+    __slots__ = '_first', '_second'
+
+    _first: OWLObjectPropertyExpression
+    _second: OWLObjectPropertyExpression
+
+    def __init__(self, first: OWLObjectPropertyExpression, second: OWLObjectPropertyExpression,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._first = first
+        self._second = second
+        super().__init__(properties=[first, second], annotations=annotations)
+
+    def get_first_property(self) -> OWLObjectPropertyExpression:
+        return self._first
+
+    def get_second_property(self) -> OWLObjectPropertyExpression:
+        return self._second
+
+    def __repr__(self):
+        return f'OWLInverseObjectPropertiesAxiom(first={self._first},second={self._second},' \
+               f'annotations={self._annotations})'
+
+
+class OWLEquivalentDataPropertiesAxiom(OWLNaryPropertyAxiom[OWLDataPropertyExpression], OWLDataPropertyAxiom):
+    """An equivalent data properties axiom EquivalentDataProperties( DPE1 ... DPEn ) states that all the data property
+    expressions DPEi, 1 ≤ i ≤ n, are semantically equivalent to each other. This axiom allows one to use each DPEi as a
+    synonym for each DPEj — that is, in any expression in the ontology containing such an axiom, DPEi can be replaced
+    with DPEj without affecting the meaning of the ontology.
+
+    (https://www.w3.org/TR/owl2-syntax/#Equivalent_Data_Properties)
+    """
+    __slots__ = ()
+
+    def __init__(self, properties: List[OWLDataPropertyExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(properties=properties, annotations=annotations)
+
+
+class OWLDisjointDataPropertiesAxiom(OWLNaryPropertyAxiom[OWLDataPropertyExpression], OWLDataPropertyAxiom):
+    """A disjoint data properties axiom DisjointDataProperties( DPE1 ... DPEn ) states that all of the data property
+    expressions DPEi, 1 ≤ i ≤ n, are pairwise disjoint; that is, no individual x can be connected to a literal y by both
+     DPEi and DPEj for i ≠ j.
+
+     (https://www.w3.org/TR/owl2-syntax/#Disjoint_Data_Properties)"""
+    __slots__ = ()
+
+    def __init__(self, properties: List[OWLDataPropertyExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(properties=properties, annotations=annotations)
+
+
+class OWLSubClassOfAxiom(OWLClassAxiom):
+    """A subclass axiom SubClassOf( CE1 CE2 ) states that the class expression CE1 is a subclass of the class
+    expression CE2. Roughly speaking, this states that CE1 is more specific than CE2. Subclass axioms are a
+    fundamental type of axioms in OWL 2 and can be used to construct a class hierarchy. Other kinds of class
+    expression axiom can be seen as syntactic shortcuts for one or more subclass axioms.
+
+     (https://www.w3.org/TR/owl2-syntax/#Subclass_Axioms)
+     """
+    __slots__ = '_sub_class', '_super_class'
+
+    _sub_class: OWLClassExpression
+    _super_class: OWLClassExpression
+
+    def __init__(self, sub_class: OWLClassExpression, super_class: OWLClassExpression,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        """Get an equivalent classes axiom with specified operands and no annotations.
+
+        Args:
+            sub_class: The sub-class.
+            super_class: The super class.
+            annotations: Annotations.
+        """
+        self._sub_class = sub_class
+        self._super_class = super_class
+        super().__init__(annotations=annotations)
+
+    def get_sub_class(self) -> OWLClassExpression:
+        return self._sub_class
+
+    def get_super_class(self) -> OWLClassExpression:
+        return self._super_class
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._super_class == other._super_class and self._sub_class == other._sub_class \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._super_class, self._sub_class, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLSubClassOfAxiom(sub_class={self._sub_class},super_class={self._super_class},' \
+               f'annotations={self._annotations})'
+
+
+class OWLDisjointUnionAxiom(OWLClassAxiom):
+    """A disjoint union axiom DisjointUnion( C CE1 ... CEn ) states that a class C is a disjoint union of the class
+    expressions CEi, 1 ≤ i ≤ n, all of which are pairwise disjoint. Such axioms are sometimes referred to as
+    covering axioms, as they state that the extensions of all CEi exactly cover the extension of C. Thus, each
+    instance of C is an instance of exactly one CEi, and each instance of CEi is an instance of C.
+
+    (https://www.w3.org/TR/owl2-syntax/#Disjoint_Union_of_Class_Expressions)
+    """
+    __slots__ = '_cls', '_class_expressions'
+
+    _cls: OWLClass
+    _class_expressions: List[OWLClassExpression]
+
+    def __init__(self, cls_: OWLClass, class_expressions: List[OWLClassExpression],
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._cls = cls_
+        self._class_expressions = class_expressions
+        super().__init__(annotations=annotations)
+
+    def get_owl_class(self) -> OWLClass:
+        return self._cls
+
+    def get_class_expressions(self) -> Iterable[OWLClassExpression]:
+        yield from self._class_expressions
+
+    def get_owl_equivalent_classes_axiom(self) -> OWLEquivalentClassesAxiom:
+        return OWLEquivalentClassesAxiom(self._cls, OWLObjectUnionOf(self._class_expressions))
+
+    def get_owl_disjoint_classes_axiom(self) -> OWLDisjointClassesAxiom:
+        return OWLDisjointClassesAxiom(self._class_expressions)
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._cls == other._cls and self._class_expressions == other._class_expressions \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._cls, *self._class_expressions, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLDisjointUnionAxiom(class={self._cls},class_expressions={self._class_expressions},' \
+               f'annotations={self._annotations})'
+
+
+class OWLClassAssertionAxiom(OWLIndividualAxiom):
+    """A class assertion ClassAssertion( CE a ) states that the individual a is an instance of the class expression CE.
+
+    (https://www.w3.org/TR/owl2-syntax/#Class_Assertions)
+    """
+    __slots__ = '_individual', '_class_expression'
+
+    _individual: OWLIndividual
+    _class_expression: OWLClassExpression
+
+    def __init__(self, individual: OWLIndividual, class_expression: OWLClassExpression,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        """Get a ClassAssertion axiom for the specified individual and class expression.
+        Args:
+            individual: The individual.
+            class_expression: The class the individual belongs to.
+            annotations: Annotations.
+        """
+        self._individual = individual
+        self._class_expression = class_expression
+        super().__init__(annotations=annotations)
+
+    def get_individual(self) -> OWLIndividual:
+        return self._individual
+
+    def get_class_expression(self) -> OWLClassExpression:
+        return self._class_expression
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._class_expression == other._class_expression and self._individual == other._individual \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._individual, self._class_expression, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLClassAssertionAxiom(individual={self._individual},class_expression={self._class_expression},' \
+               f'annotations={self._annotations})'
+
+
+class OWLAnnotationProperty(OWLProperty):
+    """Represents an AnnotationProperty in the OWL 2 specification."""
+    __slots__ = '_iri'
+
+    _iri: IRI
+
+    def __init__(self, iri: Union[IRI, str]):
+        """Get a new OWLAnnotationProperty object.
+
+        Args:
+            iri: New OWLAnnotationProperty IRI.
+        """
+        if isinstance(iri, IRI):
+            self._iri = iri
+        else:
+            self._iri = IRI.create(iri)
+
+    @property
+    def iri(self) -> IRI:
+        return self._iri
+
+    @property
+    def str(self) -> str:
+        return self._iri.as_str()
+
+
+class OWLAnnotation(OWLObject):
+    """Annotations are used in the various types of annotation axioms, which bind annotations to their subjects
+    (i.e. axioms or declarations)."""
+    __slots__ = '_property', '_value'
+
+    _property: OWLAnnotationProperty
+    _value: OWLAnnotationValue
+
+    def __init__(self, property: OWLAnnotationProperty, value: OWLAnnotationValue):
+        """Gets an annotation.
+
+        Args:
+            property: the annotation property.
+            value: The annotation value.
+        """
+        self._property = property
+        self._value = value
+
+    def get_property(self) -> OWLAnnotationProperty:
+        """Gets the property that this annotation acts along.
+
+        Returns:
+            The annotation property.
+        """
+        return self._property
+
+    def get_value(self) -> OWLAnnotationValue:
+        """Gets the annotation value. The type of value will depend upon the type of the annotation e.g. whether the
+        annotation is an OWLLiteral, an IRI or an OWLAnonymousIndividual.
+
+        Returns:
+            The annotation value.
+        """
+        return self._value
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._property == other._property and self._value == other._value
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._property, self._value))
+
+    def __repr__(self):
+        return f'OWLAnnotation({self._property}, {self._value})'
+
+
+class OWLAnnotationAxiom(OWLAxiom, metaclass=ABCMeta):
+    """A super interface for annotation axioms."""
+    __slots__ = ()
+
+    def is_annotation_axiom(self) -> bool:
+        return True
+
+
+class OWLAnnotationAssertionAxiom(OWLAnnotationAxiom):
+    """An annotation assertion AnnotationAssertion( AP as av ) states that the annotation subject as — an IRI or an
+    anonymous individual — is annotated with the annotation property AP and the annotation value av.
+
+
+    (https://www.w3.org/TR/owl2-syntax/#Annotation_Assertion)
+    """
+    __slots__ = '_subject', '_annotation'
+
+    _subject: OWLAnnotationSubject
+    _annotation: OWLAnnotation
+
+    def __init__(self, subject: OWLAnnotationSubject, annotation: OWLAnnotation):
+        """Get an annotation assertion axiom - with annotations.
+
+        Args:
+            subject: Subject.
+            annotation: Annotation.
+        """
+        assert isinstance(subject, OWLAnnotationSubject)
+        assert isinstance(annotation, OWLAnnotation)
+
+        self._subject = subject
+        self._annotation = annotation
+
+    def get_subject(self) -> OWLAnnotationSubject:
+        """Gets the subject of this object.
+
+        Returns:
+            The subject.
+        """
+        return self._subject
+
+    def get_property(self) -> OWLAnnotationProperty:
+        """Gets the property.
+
+        Returns:
+            The property.
+        """
+        return self._annotation.get_property()
+
+    def get_value(self) -> OWLAnnotationValue:
+        """Gets the annotation value. This is either an IRI, an OWLAnonymousIndividual or an OWLLiteral.
+
+        Returns:
+            The annotation value.
+        """
+        return self._annotation.get_value()
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._subject == other._subject and self._annotation == other._annotation
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._subject, self._annotation))
+
+    def __repr__(self):
+        return f'OWLAnnotationAssertionAxiom({self._subject}, {self._annotation})'
+class OWLSubAnnotationPropertyOfAxiom(OWLAnnotationAxiom):
+    """An annotation subproperty axiom SubAnnotationPropertyOf( AP1 AP2 ) states that the annotation property AP1 is
+    a subproperty of the annotation property AP2.
+
+    (https://www.w3.org/TR/owl2-syntax/#Annotation_Subproperties)
+    """
+    __slots__ = '_sub_property', '_super_property'
+
+    _sub_property: OWLAnnotationProperty
+    _super_property: OWLAnnotationProperty
+
+    def __init__(self, sub_property: OWLAnnotationProperty, super_property: OWLAnnotationProperty,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._sub_property = sub_property
+        self._super_property = super_property
+        super().__init__(annotations=annotations)
+
+    def get_sub_property(self) -> OWLAnnotationProperty:
+        return self._sub_property
+
+    def get_super_property(self) -> OWLAnnotationProperty:
+        return self._super_property
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._sub_property == other._sub_property and self._super_property == other._super_property \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._sub_property, self._super_property, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLSubAnnotationPropertyOfAxiom(sub_property={self._sub_property},' \
+               f'super_property={self._super_property},annotations={self._annotations})'
+
+
+class OWLAnnotationPropertyDomainAxiom(OWLAnnotationAxiom):
+    """An annotation property domain axiom AnnotationPropertyDomain( AP U ) states that the domain of the annotation
+    property AP is the IRI U.
+
+     (https://www.w3.org/TR/owl2-syntax/#Annotation_Property_Domain)"""
+    __slots__ = '_property', '_domain'
+
+    _property: OWLAnnotationProperty
+    _domain: IRI
+
+    def __init__(self, property_: OWLAnnotationProperty, domain: IRI,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._property = property_
+        self._domain = domain
+        super().__init__(annotations=annotations)
+
+    def get_property(self) -> OWLAnnotationProperty:
+        return self._property
+
+    def get_domain(self) -> IRI:
+        return self._domain
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._property == other._property and self._domain == other._domain \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._property, self._domain, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLAnnotationPropertyDomainAxiom({repr(self._property)},{repr(self._domain)},' \
+               f'{repr(self._annotations)})'
+
+
+class OWLAnnotationPropertyRangeAxiom(OWLAnnotationAxiom):
+    """An annotation property range axiom AnnotationPropertyRange( AP U )
+    states that the range of the annotation property AP is the IRI U.
+
+    (https://www.w3.org/TR/owl2-syntax/#Annotation_Property_Range)"""
+    __slots__ = '_property', '_range'
+
+    _property: OWLAnnotationProperty
+    _range: IRI
+
+    def __init__(self, property_: OWLAnnotationProperty, range_: IRI,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._property = property_
+        self._range = range_
+        super().__init__(annotations=annotations)
+
+    def get_property(self) -> OWLAnnotationProperty:
+        return self._property
+
+    def get_range(self) -> IRI:
+        return self._range
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._property == other._property and self._range == other._range \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._property, self._range, *self._annotations))
+
+    def __repr__(self):
+        return f'OWLAnnotationPropertyRangeAxiom({repr(self._property)},{repr(self._range)},' \
+               f'{repr(self._annotations)})'
+
+
+class OWLSubPropertyAxiom(Generic[_P], OWLPropertyAxiom):
+    """
+    Base interface for object and data sub-property axioms.
+    """
+    __slots__ = '_sub_property', '_super_property'
+
+    _sub_property: _P
+    _super_property: _P
+
+    @abstractmethod
+    def __init__(self, sub_property: _P, super_property: _P,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        self._sub_property = sub_property
+        self._super_property = super_property
+        super().__init__(annotations=annotations)
+
+    def get_sub_property(self) -> _P:
+        return self._sub_property
+
+    def get_super_property(self) -> _P:
+        return self._super_property
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._sub_property == other._sub_property and self._super_property == other._super_property \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._sub_property, self._super_property, *self._annotations))
+
+    def __repr__(self):
+        return f'{type(self).__name__}(sub_property={self._sub_property},super_property={self._super_property},' \
+               f'annotations={self._annotations})'
+
+
+class OWLSubObjectPropertyOfAxiom(OWLSubPropertyAxiom[OWLObjectPropertyExpression], OWLObjectPropertyAxiom):
+    """Object subproperty axioms are analogous to subclass axioms, and they come in two forms.
+       The basic form is SubObjectPropertyOf( OPE1 OPE2 ). This axiom states that the object property expression OPE1
+       is a subproperty of the object property expression OPE2 — that is, if an individual x is connected by OPE1 to an
+       individual y, then x is also connected by OPE2 to y.
+       The more complex form is SubObjectPropertyOf( ObjectPropertyChain( OPE1 ... OPEn ) OPE )
+       but ObjectPropertyChain is not represented in owlapy yet.
+
+       (https://www.w3.org/TR/owl2-syntax/#Object_Subproperties)"""
+    __slots__ = ()
+
+    def __init__(self, sub_property: OWLObjectPropertyExpression, super_property: OWLObjectPropertyExpression,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(sub_property=sub_property, super_property=super_property, annotations=annotations)
+
+
+class OWLSubDataPropertyOfAxiom(OWLSubPropertyAxiom[OWLDataPropertyExpression], OWLDataPropertyAxiom):
+    """A data subproperty axiom SubDataPropertyOf( DPE1 DPE2 ) states that the data property expression DPE1 is a
+    subproperty of the data property expression DPE2 — that is, if an individual x is connected by DPE1 to a literal y,
+     then x is connected by DPE2 to y as well.
+
+     (https://www.w3.org/TR/owl2-syntax/#Data_Subproperties)"""
+    __slots__ = ()
+
+    def __init__(self, sub_property: OWLDataPropertyExpression, super_property: OWLDataPropertyExpression,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(sub_property=sub_property, super_property=super_property, annotations=annotations)
+
+
+class OWLPropertyAssertionAxiom(Generic[_P, _C], OWLIndividualAxiom, metaclass=ABCMeta):
+    """Base class for Property Assertion axioms."""
+    __slots__ = '_subject', '_property', '_object'
+
+    _subject: OWLIndividual
+    _property: _P
+    _object: _C
+
+    @abstractmethod
+    def __init__(self, subject: OWLIndividual, property_: _P, object_: _C,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        """Get a PropertyAssertion axiom for the specified subject, property, object.
+        Args:
+            subject: The subject of the property assertion.
+            property_: The property of the property assertion.
+            object_: The object of the property assertion.
+            annotations: Annotations.
+        """
+        assert isinstance(subject, OWLIndividual)
+
+        self._subject = subject
+        self._property = property_
+        self._object = object_
+        super().__init__(annotations=annotations)
+
+    def get_subject(self) -> OWLIndividual:
+        return self._subject
+
+    def get_property(self) -> _P:
+        return self._property
+
+    def get_object(self) -> _C:
+        return self._object
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._subject == other._subject and self._property == other._property and \
+                self._object == other._object and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._subject, self._property, self._object, *self._annotations))
+
+    def __repr__(self):
+        return f'{type(self).__name__}(subject={self._subject},property={self._property},' \
+               f'object={self._object},annotation={self._annotations})'
+
+
+class OWLObjectPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLObjectPropertyExpression, OWLIndividual]):
+    """A positive object property assertion ObjectPropertyAssertion( OPE a1 a2 ) states that the individual a1 is
+     connected by the object property expression OPE to the individual a2.
+
+     (https://www.w3.org/TR/owl2-syntax/#Positive_Object_Property_Assertions)
+     """
+    __slots__ = ()
+
+    def __init__(self, subject: OWLIndividual, property_: OWLObjectPropertyExpression, object_: OWLIndividual,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(subject, property_, object_, annotations)
+
+
+class OWLNegativeObjectPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLObjectPropertyExpression, OWLIndividual]):
+    """A negative object property assertion NegativeObjectPropertyAssertion( OPE a1 a2 ) states that the individual a1
+    is not connected by the object property expression OPE to the individual a2.
+
+    (https://www.w3.org/TR/owl2-syntax/#Negative_Object_Property_Assertions)
+    """
+    __slots__ = ()
+
+    def __init__(self, subject: OWLIndividual, property_: OWLObjectPropertyExpression, object_: OWLIndividual,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(subject, property_, object_, annotations)
+
+
+class OWLDataPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLDataPropertyExpression, OWLLiteral]):
+    """A positive data property assertion DataPropertyAssertion( DPE a lt ) states that the individual a is connected
+    by the data property expression DPE to the literal lt.
+
+    (https://www.w3.org/TR/owl2-syntax/#Positive_Data_Property_Assertions)
+    """
+    __slots__ = ()
+
+    def __init__(self, subject: OWLIndividual, property_: OWLDataPropertyExpression, object_: OWLLiteral,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(subject, property_, object_, annotations)
+
+
+class OWLNegativeDataPropertyAssertionAxiom(OWLPropertyAssertionAxiom[OWLDataPropertyExpression, OWLLiteral]):
+    """A negative data property assertion NegativeDataPropertyAssertion( DPE a lt ) states that the individual a is not
+    connected by the data property expression DPE to the literal lt.
+
+    (https://www.w3.org/TR/owl2-syntax/#Negative_Data_Property_Assertions)
+    """
+    __slots__ = ()
+
+    def __init__(self, subject: OWLIndividual, property_: OWLDataPropertyExpression, object_: OWLLiteral,
+                 annotations: Optional[Iterable['OWLAnnotation']] = None):
+        super().__init__(subject, property_, object_, annotations)
+
+
+class OWLUnaryPropertyAxiom(Generic[_P], OWLPropertyAxiom, metaclass=ABCMeta):
+    """Base class for Unary property axiom."""
+    __slots__ = '_property'
+
+    _property: _P
+
+    def __init__(self, property_: _P, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        self._property = property_
+        super().__init__(annotations=annotations)
+
+    def get_property(self) -> _P:
+        return self._property
+
+
+class OWLObjectPropertyCharacteristicAxiom(OWLUnaryPropertyAxiom[OWLObjectPropertyExpression],
+                                           OWLObjectPropertyAxiom, metaclass=ABCMeta):
+    """Base interface for functional object property axiom."""
+    __slots__ = ()
+
+    @abstractmethod
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._property == other._property and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._property, *self._annotations))
+
+    def __repr__(self):
+        return f"{type(self).__name__}({repr(self._property)},{repr(self._annotations)})"
+
+
+class OWLFunctionalObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
+    """An object property functionality axiom FunctionalObjectProperty( OPE ) states that
+    the object property expression OPE is functional — that is, for each individual x,
+    there can be at most one distinct individual y such that x is connected by OPE to y.
+
+    (https://www.w3.org/TR/owl2-syntax/#Functional_Object_Properties)"""
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLAsymmetricObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
+    """An object property asymmetry axiom AsymmetricObjectProperty( OPE ) states that
+    the object property expression OPE is asymmetric — that is, if an individual x is
+    connected by OPE to an individual y, then y cannot be connected by OPE to x.
+
+    (https://www.w3.org/TR/owl2-syntax/#Symmetric_Object_Properties)"""
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLInverseFunctionalObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
+    """An object property inverse functionality axiom InverseFunctionalObjectProperty( OPE )
+    states that the object property expression OPE is inverse-functional — that is, for each
+    individual x, there can be at most one individual y such that y is connected by OPE with x.
+
+    (https://www.w3.org/TR/owl2-syntax/#Inverse-Functional_Object_Properties)
+    """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLIrreflexiveObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
+    """An object property irreflexivity axiom IrreflexiveObjectProperty( OPE ) states that the
+    object property expression OPE is irreflexive — that is, no individual is connected by
+    OPE to itself.
+
+    (https://www.w3.org/TR/owl2-syntax/#Irreflexive_Object_Properties)
+    """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLReflexiveObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
+    """An object property reflexivity axiom ReflexiveObjectProperty( OPE ) states that the
+    object property expression OPE is reflexive — that is, each individual is connected
+    by OPE to itself. Each such axiom can be seen as a syntactic shortcut for the
+    following axiom: SubClassOf( owl:Thing ObjectHasSelf( OPE ) )
+
+    (https://www.w3.org/TR/owl2-syntax/#Reflexive_Object_Properties)"""
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLSymmetricObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
+    """An object property symmetry axiom SymmetricObjectProperty( OPE ) states that
+    the object property expression OPE is symmetric — that is, if an individual x
+    is connected by OPE to an individual y, then y is also connected by OPE to x.
+    Each such axiom can be seen as a syntactic shortcut for the following axiom:
+     SubObjectPropertyOf( OPE ObjectInverseOf( OPE ) )
+
+     (https://www.w3.org/TR/owl2-syntax/#Symmetric_Object_Properties)
+     """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLTransitiveObjectPropertyAxiom(OWLObjectPropertyCharacteristicAxiom):
+    """An object property transitivity axiom TransitiveObjectProperty( OPE ) states that the
+    object property expressionOPE is transitive — that is, if an individual x is connected
+    by OPE to an individual y that is connected by OPE to an individual z, then x is also
+    connected by OPE to z. Each such axiom can be seen as a syntactic shortcut for the
+    following axiom: SubObjectPropertyOf( ObjectPropertyChain( OPE OPE ) OPE )
+
+     (https://www.w3.org/TR/owl2-syntax/#Transitive_Object_Properties)
+     """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLDataPropertyCharacteristicAxiom(OWLUnaryPropertyAxiom[OWLDataPropertyExpression],
+                                         OWLDataPropertyAxiom, metaclass=ABCMeta):
+    """Base interface for Functional data property axiom."""
+    __slots__ = ()
+
+    @abstractmethod
+    def __init__(self, property_: OWLDataPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._property == other._property and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._property, *self._annotations))
+
+    def __repr__(self):
+        return f"{type(self).__name__}({repr(self._property)},{repr(self._annotations)})"
+
+
+class OWLFunctionalDataPropertyAxiom(OWLDataPropertyCharacteristicAxiom):
+    """A data property functionality axiom FunctionalDataProperty( DPE ) states that
+    the data property expression DPE is functional — that is, for each individual x,
+    there can be at most one distinct literal y such that x is connected by DPE with
+    y. Each such axiom can be seen as a syntactic shortcut for the following axiom:
+    SubClassOf( owl:Thing DataMaxCardinality( 1 DPE ) )
+
+    (https://www.w3.org/TR/owl2-syntax/#Transitive_Object_Properties)
+    """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLDataPropertyExpression, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, annotations=annotations)
+
+
+class OWLPropertyDomainAxiom(Generic[_P], OWLUnaryPropertyAxiom[_P], metaclass=ABCMeta):
+    """Base class for Property Domain axioms."""
+    __slots__ = '_domain'
+
+    _domain: OWLClassExpression
+
+    @abstractmethod
+    def __init__(self, property_: _P, domain: OWLClassExpression,
+                 annotations: Optional[Iterable[OWLAnnotation]] = None):
+        self._domain = domain
+        super().__init__(property_=property_, annotations=annotations)
+
+    def get_domain(self) -> OWLClassExpression:
+        return self._domain
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._property == other._property and self._domain == other._domain \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._property, self._domain, *self._annotations))
+
+    def __repr__(self):
+        return f"{type(self).__name__}({repr(self._property)},{repr(self._domain)},{repr(self._annotations)})"
+
+
+class OWLPropertyRangeAxiom(Generic[_P, _R], OWLUnaryPropertyAxiom[_P], metaclass=ABCMeta):
+    """Base class for Property Range axioms."""
+    __slots__ = '_range'
+
+    _range: _R
+
+    @abstractmethod
+    def __init__(self, property_: _P, range_: _R, annotations: Optional[Iterable[OWLAnnotation]] = None):
+        self._range = range_
+        super().__init__(property_=property_, annotations=annotations)
+
+    def get_range(self) -> _R:
+        return self._range
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self._property == other._property and self._range == other._range \
+                and self._annotations == other._annotations
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self._property, self._range, *self._annotations))
+
+    def __repr__(self):
+        return f"{type(self).__name__}({repr(self._property)},{repr(self._range)},{repr(self._annotations)})"
+
+
+class OWLObjectPropertyDomainAxiom(OWLPropertyDomainAxiom[OWLObjectPropertyExpression]):
+    """ An object property domain axiom ObjectPropertyDomain( OPE CE ) states that the domain of the
+    object property expression OPE is the class expression CE — that is, if an individual x is
+    connected by OPE with some other individual, then x is an instance of CE. Each such axiom can
+    be seen as a syntactic shortcut for the following axiom:
+    SubClassOf( ObjectSomeValuesFrom( OPE owl:Thing ) CE )
+
+    (https://www.w3.org/TR/owl2-syntax/#Object_Property_Domain)
+    """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, domain: OWLClassExpression,
+                 annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, domain=domain, annotations=annotations)
+
+
+class OWLDataPropertyDomainAxiom(OWLPropertyDomainAxiom[OWLDataPropertyExpression]):
+    """ A data property domain axiom DataPropertyDomain( DPE CE ) states that the domain of the
+    data property expression DPE is the class expression CE — that is, if an individual x is
+    connected by DPE with some literal, then x is an instance of CE. Each such axiom can be
+    seen as a syntactic shortcut for the following axiom:
+    SubClassOf( DataSomeValuesFrom( DPE rdfs:Literal) CE )
+
+    (https://www.w3.org/TR/owl2-syntax/#Data_Property_Domain)
+    """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLDataPropertyExpression, domain: OWLClassExpression,
+                 annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, domain=domain, annotations=annotations)
+
+
+class OWLObjectPropertyRangeAxiom(OWLPropertyRangeAxiom[OWLObjectPropertyExpression, OWLClassExpression]):
+    """ An object property range axiom ObjectPropertyRange( OPE CE ) states that the range of the object property
+    expression OPE is the class expression CE — that is, if some individual is connected by OPE with an individual x,
+    then x is an instance of CE. Each such axiom can be seen as a syntactic shortcut for the following axiom:
+    SubClassOf( owl:Thing ObjectAllValuesFrom( OPE CE ) )
+
+    (https://www.w3.org/TR/owl2-syntax/#Object_Property_Range)
+    """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLObjectPropertyExpression, range_: OWLClassExpression,
+                 annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, range_=range_, annotations=annotations)
+
+
+class OWLDataPropertyRangeAxiom(OWLPropertyRangeAxiom[OWLDataPropertyExpression, OWLDataRange]):
+    """ A data property range axiom DataPropertyRange( DPE DR ) states that the range of the data property
+    expression DPE is the data range DR — that is, if some individual is connected by DPE with a literal x,
+    then x is in DR. The arity of DR must be one. Each such axiom can be seen as a syntactic shortcut for
+    the following axiom:  SubClassOf( owl:Thing DataAllValuesFrom( DPE DR ) )
+
+    (https://www.w3.org/TR/owl2-syntax/#Data_Property_Range)
+    """
+    __slots__ = ()
+
+    def __init__(self, property_: OWLDataPropertyExpression, range_: OWLDataRange,
+                 annotations: Optional[Iterable[OWLAnnotation]] = None):
+        super().__init__(property_=property_, range_=range_, annotations=annotations)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `owlapy-0.1.3/owlapy/owl_individual.py` & `owlapy-1.0.0/owlapy/owl_individual.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-from abc import ABCMeta
-from .owlobject import OWLObject, OWLEntity
-from .iri import IRI
-from typing import Final, Union
-class OWLIndividual(OWLObject, metaclass=ABCMeta):
-    """Represents a named or anonymous individual."""
-    __slots__ = ()
-    pass
-
-class OWLNamedIndividual(OWLIndividual, OWLEntity):
-    """Represents a Named Individual in the OWL 2 Specification."""
-    __slots__ = '_iri'
-    type_index: Final = 1005
-
-    _iri: IRI
-
-    def __init__(self, iri: Union[IRI, str]):
-        """Gets an instance of OWLNamedIndividual that has the specified IRI.
-
-        Args:
-            iri: an instance of IRI Class or a string representing the iri
-
-        Returns:
-            An OWLNamedIndividual that has the specified IRI.
-        """
-        if isinstance(iri, IRI):
-            self._iri = iri
-        else:
-            self._iri = IRI.create(iri)
-
-    def get_iri(self) -> IRI:
-        # TODO:CD: can be deprecated
-        # documented in parent
-        return self._iri
-
-    @property
-    def iri(self):
-        return self._iri
-
-    @property
-    def str(self):
-        return self._iri.as_str()
+"""OWL Individuals"""
+from abc import ABCMeta
+from .owl_object import OWLObject, OWLEntity
+from .iri import IRI
+from typing import Final, Union
+
+
+class OWLIndividual(OWLObject, metaclass=ABCMeta):
+    """Represents a named or anonymous individual."""
+    __slots__ = ()
+    pass
+
+
+class OWLNamedIndividual(OWLIndividual, OWLEntity):
+    """Named individuals are identified using an IRI. Since they are given an IRI, named individuals are entities.
+        IRIs from the reserved vocabulary must not be used to identify named individuals in an OWL 2 DL ontology.
+
+        (https://www.w3.org/TR/owl2-syntax/#Named_Individuals)
+        """
+    __slots__ = '_iri'
+    type_index: Final = 1005
+
+    _iri: IRI
+
+    def __init__(self, iri: Union[IRI, str]):
+        """Gets an instance of OWLNamedIndividual that has the specified IRI.
+
+        Args:
+            iri: an instance of IRI Class or a string representing the iri
+
+        Returns:
+            An OWLNamedIndividual that has the specified IRI.
+        """
+        if isinstance(iri, IRI):
+            self._iri = iri
+        else:
+            self._iri = IRI.create(iri)
+
+    @property
+    def iri(self) -> IRI:
+        return self._iri
+
+    @property
+    def str(self):
+        return self._iri.as_str()
```

### Comparing `owlapy-0.1.3/owlapy/parser.py` & `owlapy-1.0.0/owlapy/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,781 +1,785 @@
-"""String to OWL parsers."""
-from types import MappingProxyType
-from typing import Final, List, Optional, Union
-from parsimonious.grammar import Grammar
-from parsimonious.nodes import NodeVisitor
-from parsimonious.nodes import Node
-from .owlobject import OWLObjectParser
-from .namespaces import Namespaces
-from .render import _DL_SYNTAX, _MAN_SYNTAX
-from .vocab import OWLFacet, OWLRDFVocabulary
-
-
-from owlapy.model import OWLObjectHasSelf, OWLObjectIntersectionOf, OWLObjectMinCardinality, OWLObjectProperty, OWLObjectPropertyExpression, OWLObjectSomeValuesFrom, OWLObjectUnionOf, OWLClass, IRI, \
-    OWLClassExpression, OWLDataProperty, OWLNamedIndividual, OWLObjectComplementOf, OWLObjectExactCardinality, \
-    OWLQuantifiedDataRestriction, OWLQuantifiedObjectRestriction, StringOWLDatatype,  \
-    DateOWLDatatype, DateTimeOWLDatatype, DoubleOWLDatatype, DurationOWLDatatype, IntegerOWLDatatype, \
-    OWLDataSomeValuesFrom, OWLDataExactCardinality, \
-    OWLDataMaxCardinality, OWLObjectMaxCardinality, OWLDataMinCardinality, OWLDataHasValue, \
-    OWLLiteral, OWLDataRange, OWLDataOneOf, OWLDatatype, OWLObjectCardinalityRestriction, \
-    OWLDataCardinalityRestriction, OWLObjectAllValuesFrom, OWLDataAllValuesFrom, BooleanOWLDatatype
-
-from owlapy.data_ranges import OWLDataIntersectionOf, OWLDataUnionOf, OWLDataComplementOf
-from owlapy.class_expression import OWLObjectHasValue, OWLDatatypeRestriction, OWLFacetRestriction, OWLObjectOneOf
-
-
-MANCHESTER_GRAMMAR = Grammar(r"""
-    union = intersection (must_ws "or" must_ws intersection)*
-    intersection = primary (must_ws "and" must_ws primary)*
-
-    # Main entry point + object properties
-    primary = ("not" must_ws)? (data_some_only_res / some_only_res / data_cardinality_res / cardinality_res
-                           / data_value_res / value_res / has_self / class_expression)
-    some_only_res = object_property must_ws ("some"/"only") must_ws primary
-    cardinality_res = object_property must_ws ("max"/"min"/"exactly") must_ws non_negative_integer must_ws primary
-    value_res = object_property must_ws "value" must_ws individual_iri
-    has_self = object_property must_ws "Self"
-    object_property = ("inverse" must_ws)? object_property_iri
-    class_expression = class_iri / individual_list / parentheses
-    individual_list = "{" maybe_ws individual_iri (maybe_ws "," maybe_ws individual_iri)* maybe_ws "}"
-
-    # Back to start symbol (first production rule)
-    parentheses = "(" maybe_ws union maybe_ws ")"
-
-    # Data properties
-    data_some_only_res = data_property_iri must_ws ("some"/"only") must_ws data_primary
-    data_cardinality_res = data_property_iri must_ws ("max"/"min"/"exactly")
-                           must_ws non_negative_integer must_ws data_primary
-    data_value_res = data_property_iri must_ws "value" must_ws literal
-    data_primary = ("not" must_ws)? data_range
-    data_range = datatype_restriction / datatype_iri / literal_list / data_parentheses
-    literal_list = "{" maybe_ws literal (maybe_ws "," maybe_ws literal)* maybe_ws "}"
-    data_parentheses = "(" maybe_ws data_union maybe_ws ")"
-    data_union = data_intersection (must_ws "or" must_ws data_intersection)*
-    data_intersection = data_primary (must_ws "and" must_ws data_primary)*
-    datatype_restriction = datatype_iri "[" maybe_ws facet_restrictions maybe_ws "]"
-    facet_restrictions = facet_restriction (maybe_ws "," maybe_ws facet_restriction)*
-    facet_restriction = facet must_ws literal
-    facet = "length" / "minLength" / "maxLength" / "pattern" / "langRange"
-            / "totalDigits" / "fractionDigits" / "<=" / ">=" / "<" / ">"
-    datatype_iri = ("<http://www.w3.org/2001/XMLSchema#" datatype ">") / ("xsd:"? datatype)
-    datatype = "double" / "integer" / "boolean" / "string" / "dateTime" / "date" / "duration"
-
-    # Literals
-    literal = typed_literal / string_literal_language / string_literal_no_language / datetime_literal /
-              duration_literal / date_literal / float_literal / decimal_literal / integer_literal /
-              boolean_literal
-    typed_literal = quoted_string "^^" datatype_iri
-    string_literal_language = quoted_string language_tag
-    string_literal_no_language = quoted_string / no_match
-    quoted_string = ~"\"([^\"\\\\]|\\\\[\"\\\\])*\""
-    language_tag = "@" ~"[a-zA-Z]+" ("-" ~"[a-zA-Z0-9]+")*
-    float_literal = sign (float_with_integer_part / float_no_integer_part) ("f"/"F")
-    float_with_integer_part = non_negative_integer ("." ~"[0-9]+")? exponent?
-    float_no_integer_part = "." ~"[0-9]+" exponent?
-    exponent = ("e"/"E") sign ~"[0-9]+"
-    decimal_literal = sign non_negative_integer "." ~"[0-9]+"
-    integer_literal = sign non_negative_integer
-    boolean_literal = ~"[tT]rue" / ~"[fF]alse"
-    date_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))"
-    datetime_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))[T\u0020]"
-                       ~"(([0-1][0-9])|(2[0-3])):[0-5][0-9]:[0-5][0-9](\\.[0-9]{6})?"
-                       ~"(Z|([+-](([0-1][0-9])|(2[0-3])):[0-5][0-9](:[0-5][0-9](\\.[0-9]{6})?)?))?"
-    duration_literal = ~"P([0-9]+W)?([0-9]+D)?(T([0-9]+H)?([0-9]+M)?([0-9]+(\\.[0-9]{6})?S)?)?"
-    sign = ("+"/"-")?
-    non_negative_integer = ~"0|([1-9][0-9]*)"
-
-    # IRIs / Characters
-    class_iri = iri / no_match
-    individual_iri = iri / no_match
-    object_property_iri = iri / no_match
-    data_property_iri = iri / no_match
-    iri = full_iri / abbreviated_iri / simple_iri
-    full_iri = iri_ref / no_match
-    abbreviated_iri = pname_ln / no_match
-    simple_iri = pn_local / no_match
-
-    iri_ref = "<" ~"[^<>\"{}|^`\\\\\u0000-\u0020]*" ">"
-    pname_ln = pname_ns pn_local
-    pname_ns = pn_prefix? ":"
-    pn_prefix = pn_chars_base ("."* pn_chars)*
-    pn_local = (pn_chars_u / ~"[0-9]") ("."* pn_chars)*
-    pn_chars = pn_chars_u / "-" / ~"[0-9]" / ~"\u00B7" / ~"[\u0300-\u036F]" / ~"[\u203F-\u2040]"
-    pn_chars_u = pn_chars_base / "_"
-    pn_chars_base = ~"[a-zA-Z]" / ~"[\u00C0-\u00D6]" / ~"[\u00D8-\u00F6]" / ~"[\u00F8-\u02FF]" /
-                    ~"[\u0370-\u037D]" / ~"[\u037F-\u1FFF]" / ~"[\u200C-\u200D]" / ~"[\u2070-\u218F]" /
-                    ~"[\u2C00-\u2FEF]" / ~"[\u3001-\uD7FF]" / ~"[\uF900-\uFDCF]" / ~"[\uFDF0-\uFFFD]" /
-                    ~"[\U00010000-\U000EFFFF]"
-
-    must_ws = ~"[\u0020\u000D\u0009\u000A]+"
-    maybe_ws = ~"[\u0020\u000D\u0009\u000A]*"
-
-    # hacky workaround: can be added to a pass through production rule that is semantically important
-    # so nodes are not combined which makes the parsing cleaner
-    no_match = ~"(?!a)a"
-    """)
-
-
-def _transform_children(nary_visit_function):
-    def transform(self, node, visited_children):
-        if len(visited_children) > 2:
-            *_, first_operand, operands, _, _ = visited_children
-        else:
-            first_operand, operands = visited_children
-        children = first_operand if isinstance(operands, Node) else [first_operand] + [node[-1] for node in operands]
-        return nary_visit_function(self, node, children)
-    return transform
-
-
-def _node_text(node) -> str:
-    return node.text.strip()
-
-
-_STRING_TO_DATATYPE: Final = MappingProxyType({
-    "integer": IntegerOWLDatatype,
-    "double": DoubleOWLDatatype,
-    "boolean": BooleanOWLDatatype,
-    "string": StringOWLDatatype,
-    "date": DateOWLDatatype,
-    "dateTime": DateTimeOWLDatatype,
-    "duration": DurationOWLDatatype,
-})
-
-
-_DATATYPE_TO_FACETS: Final = MappingProxyType({
-    IntegerOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE, OWLFacet.MAX_EXCLUSIVE,
-                         OWLFacet.MAX_INCLUSIVE, OWLFacet.TOTAL_DIGITS},
-    DoubleOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE, OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
-    DateOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE, OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
-    DateTimeOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE,
-                          OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
-    DurationOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE,
-                          OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
-    StringOWLDatatype: {OWLFacet.LENGTH, OWLFacet.MIN_LENGTH, OWLFacet.MAX_LENGTH, OWLFacet.PATTERN},
-    BooleanOWLDatatype: {}
-})
-
-
-_FACET_TO_LITERAL_DATATYPE: Final = MappingProxyType({
-    OWLFacet.MIN_EXCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
-                             DateTimeOWLDatatype, DurationOWLDatatype},
-    OWLFacet.MAX_EXCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
-                             DateTimeOWLDatatype, DurationOWLDatatype},
-    OWLFacet.MIN_INCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
-                             DateTimeOWLDatatype, DurationOWLDatatype},
-    OWLFacet.MAX_INCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
-                             DateTimeOWLDatatype, DurationOWLDatatype},
-    OWLFacet.PATTERN: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype, DateTimeOWLDatatype,
-                       DurationOWLDatatype, StringOWLDatatype},
-    OWLFacet.LENGTH: {IntegerOWLDatatype},
-    OWLFacet.MIN_LENGTH: {IntegerOWLDatatype},
-    OWLFacet.MAX_LENGTH: {IntegerOWLDatatype},
-    OWLFacet.TOTAL_DIGITS: {IntegerOWLDatatype},
-    OWLFacet.FRACTION_DIGITS: {IntegerOWLDatatype}
-})
-
-
-# workaround to support multiple inheritance with different metaclasses
-class _ManchesterOWLSyntaxParserMeta(type(NodeVisitor), type(OWLObjectParser)):
-    pass
-
-
-class ManchesterOWLSyntaxParser(NodeVisitor, OWLObjectParser, metaclass=_ManchesterOWLSyntaxParserMeta):
-    """Manchester Syntax parser to parse strings to OWLClassExpressions.
-       Following: https://www.w3.org/TR/owl2-manchester-syntax."""
-
-    slots = 'ns', 'grammar'
-
-    ns: Optional[Union[str, Namespaces]]
-
-    def __init__(self, namespace: Optional[Union[str, Namespaces]] = None, grammar=None):
-        """Create a new Manchester Syntax parser. Names (entities) can be given as full IRIs enclosed in < and >
-           or as simple strings, in that case the namespace attribute of the parser has to be set to resolve them.
-           See https://www.w3.org/TR/owl2-manchester-syntax/#IRIs.2C_Integers.2C_Literals.2C_and_Entities
-           for more information.
-           Prefixes are currently not supported, except for datatypes.
-
-        Args:
-            namespace: Namespace to resolve names that were given without one.
-            grammar: Grammar (defaults to MANCHESTERGRAMMAR).
-        """
-        self.ns = namespace
-        self.grammar = grammar
-
-        if self.grammar is None:
-            self.grammar = MANCHESTER_GRAMMAR
-
-    def parse_expression(self, expression_str: str) -> OWLClassExpression:
-        tree = self.grammar.parse(expression_str.strip())
-        return self.visit(tree)
-
-    @_transform_children
-    def visit_union(self, node, children) -> OWLClassExpression:
-        return children if isinstance(children, OWLClassExpression) else OWLObjectUnionOf(children)
-
-    @_transform_children
-    def visit_intersection(self, node, children) -> OWLClassExpression:
-        return children if isinstance(children, OWLClassExpression) else OWLObjectIntersectionOf(children)
-
-    def visit_primary(self, node, children) -> OWLClassExpression:
-        match_not, expr = children
-        return OWLObjectComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
-
-    def visit_some_only_res(self, node, children) -> OWLQuantifiedObjectRestriction:
-        property_, _, type_, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _MAN_SYNTAX.EXISTS:
-            return OWLObjectSomeValuesFrom(property_, filler)
-        else:
-            return OWLObjectAllValuesFrom(property_, filler)
-
-    def visit_cardinality_res(self, node, children) -> OWLObjectCardinalityRestriction:
-        property_, _, type_, _, cardinality, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _MAN_SYNTAX.MIN:
-            return OWLObjectMinCardinality(cardinality, property_, filler)
-        elif type_ == _MAN_SYNTAX.MAX:
-            return OWLObjectMaxCardinality(cardinality, property_, filler)
-        else:
-            return OWLObjectExactCardinality(cardinality, property_, filler)
-
-    def visit_value_res(self, node, children) -> OWLObjectHasValue:
-        property_, *_, individual = children
-        return OWLObjectHasValue(property_, individual)
-
-    def visit_has_self(self, node, children) -> OWLObjectHasSelf:
-        property_, *_ = children
-        return OWLObjectHasSelf(property_)
-
-    def visit_object_property(self, node, children) -> OWLObjectPropertyExpression:
-        inverse, property_ = children
-        return property_.get_inverse_property() if isinstance(inverse, list) else property_
-
-    def visit_class_expression(self, node, children) -> OWLClassExpression:
-        return children[0]
-
-    @_transform_children
-    def visit_individual_list(self, node, children) -> OWLObjectOneOf:
-        return OWLObjectOneOf(children)
-
-    def visit_data_primary(self, node, children) -> OWLDataRange:
-        match_not, expr = children
-        return OWLDataComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
-
-    def visit_data_some_only_res(self, node, children) -> OWLQuantifiedDataRestriction:
-        property_, _, type_, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _MAN_SYNTAX.EXISTS:
-            return OWLDataSomeValuesFrom(property_, filler)
-        else:
-            return OWLDataAllValuesFrom(property_, filler)
-
-    def visit_data_cardinality_res(self, node, children) -> OWLDataCardinalityRestriction:
-        property_, _, type_, _, cardinality, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _MAN_SYNTAX.MIN:
-            return OWLDataMinCardinality(cardinality, property_, filler)
-        elif type_ == _MAN_SYNTAX.MAX:
-            return OWLDataMaxCardinality(cardinality, property_, filler)
-        else:
-            return OWLDataExactCardinality(cardinality, property_, filler)
-
-    def visit_data_value_res(self, node, children) -> OWLDataHasValue:
-        property_, *_, literal = children
-        return OWLDataHasValue(property_, literal)
-
-    @_transform_children
-    def visit_data_union(self, node, children) -> OWLDataRange:
-        return children if isinstance(children, OWLDataRange) else OWLDataUnionOf(children)
-
-    @_transform_children
-    def visit_data_intersection(self, node, children) -> OWLDataRange:
-        return children if isinstance(children, OWLDataRange) else OWLDataIntersectionOf(children)
-
-    @_transform_children
-    def visit_literal_list(self, node, children) -> OWLDataOneOf:
-        return OWLDataOneOf(children)
-
-    def visit_data_parentheses(self, node, children) -> OWLDataRange:
-        *_, expr, _, _ = children
-        return expr
-
-    def visit_datatype_restriction(self, node, children) -> OWLDatatypeRestriction:
-        datatype, *_, facet_restrictions, _, _ = children
-        if isinstance(facet_restrictions, OWLFacetRestriction):
-            facet_restrictions = facet_restrictions,
-        not_valid_literals = []
-        if datatype != StringOWLDatatype:
-            not_valid_literals = [res.get_facet_value() for res in facet_restrictions
-                                  if res.get_facet_value().get_datatype() != datatype]
-        not_valid_facets = [res.get_facet() for res in facet_restrictions
-                            if res.get_facet() not in _DATATYPE_TO_FACETS[datatype]]
-
-        if not_valid_literals or not_valid_facets:
-            raise ValueError(f"Literals: {not_valid_literals} and Facets: {not_valid_facets}"
-                             f" not valid for datatype: {datatype}")
-        return OWLDatatypeRestriction(datatype, facet_restrictions)
-
-    @_transform_children
-    def visit_facet_restrictions(self, node, children) -> List[OWLFacetRestriction]:
-        return children
-
-    def visit_facet_restriction(self, node, children) -> OWLFacetRestriction:
-        facet, _, literal = children
-        if literal.get_datatype() not in _FACET_TO_LITERAL_DATATYPE[facet]:
-            raise ValueError(f"Literal: {literal} not valid for facet: {facet}")
-        return OWLFacetRestriction(facet, literal)
-
-    def visit_literal(self, node, children) -> OWLLiteral:
-        return children[0]
-
-    def visit_typed_literal(self, node, children) -> OWLLiteral:
-        value, _, datatype = children
-        return OWLLiteral(value[1:-1], datatype)
-
-    def visit_string_literal_language(self, node, children):
-        raise NotImplementedError(f"Language tags and plain literals not supported in owlapy yet: {_node_text(node)}")
-
-    def visit_string_literal_no_language(self, node, children) -> OWLLiteral:
-        value = children[0]
-        return OWLLiteral(value[1:-1], StringOWLDatatype)
-
-    def visit_quoted_string(self, node, children) -> str:
-        return _node_text(node)
-
-    def visit_float_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node)[:-1], DoubleOWLDatatype)
-
-    def visit_decimal_literal(self, node, children) -> OWLLiteral:
-        # TODO: Just use float for now, decimal not supported in owlapy yet
-        return OWLLiteral(_node_text(node), DoubleOWLDatatype)
-
-    def visit_integer_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), IntegerOWLDatatype)
-
-    def visit_boolean_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), BooleanOWLDatatype)
-
-    def visit_datetime_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), DateTimeOWLDatatype)
-
-    def visit_duration_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), DurationOWLDatatype)
-
-    def visit_date_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), DateOWLDatatype)
-
-    def visit_non_negative_integer(self, node, children) -> int:
-        return int(_node_text(node))
-
-    def visit_datatype_iri(self, node, children) -> str:
-        return children[0][1]
-
-    def visit_datatype(self, node, children) -> OWLDatatype:
-        return _STRING_TO_DATATYPE[_node_text(node)]
-
-    def visit_facet(self, node, children) -> OWLFacet:
-        return OWLFacet.from_str(_node_text(node))
-
-    def visit_class_iri(self, node, children) -> OWLClass:
-        return OWLClass(children[0])
-
-    def visit_individual_iri(self, node, children) -> OWLNamedIndividual:
-        return OWLNamedIndividual(children[0])
-
-    def visit_object_property_iri(self, node, children) -> OWLObjectProperty:
-        return OWLObjectProperty(children[0])
-
-    def visit_data_property_iri(self, node, children) -> OWLDataProperty:
-        return OWLDataProperty(children[0])
-
-    def visit_iri(self, node, children) -> IRI:
-        return children[0]
-
-    def visit_full_iri(self, node, children) -> IRI:
-        try:
-            iri = _node_text(node)[1:-1]
-            return IRI.create(iri)
-        except IndexError:
-            raise ValueError(f"{iri} is not a valid IRI.")
-
-    def visit_abbreviated_iri(self, node, children):
-        # TODO: Add support for prefixes
-        raise NotImplementedError(f"Parsing of prefixes is not supported yet: {_node_text(node)}")
-
-    def visit_simple_iri(self, node, children) -> IRI:
-        simple_iri = _node_text(node)
-        if simple_iri == "Thing":
-            return OWLRDFVocabulary.OWL_THING.get_iri()
-        elif simple_iri == "Nothing":
-            return OWLRDFVocabulary.OWL_NOTHING.get_iri()
-        elif self.ns is not None:
-            return IRI(self.ns, simple_iri)
-        else:
-            raise ValueError(f"If entities are specified without a full iri ({simple_iri}), "
-                             "the namespace attribute of the parser has to be set.")
-
-    def visit_parentheses(self, node, children) -> OWLClassExpression:
-        *_, expr, _, _ = children
-        return expr
-
-    def generic_visit(self, node, children):
-        return children or node
-
-
-DL_GRAMMAR = Grammar(r"""
-    union = intersection (must_ws "⊔" must_ws intersection)*
-    intersection = primary (must_ws "⊓" must_ws primary)*
-
-    # Main entry point + object properties
-    primary = ("¬" maybe_ws)? (has_self / data_value_res / value_res / data_some_only_res / some_only_res /
-                data_cardinality_res / cardinality_res / class_expression)
-    some_only_res = ("∃"/"∀") maybe_ws object_property "." primary
-    cardinality_res = ("≥"/"≤"/"=") must_ws non_negative_integer must_ws object_property "." primary
-    value_res = "∃" maybe_ws object_property "." "{" individual_iri "}"
-    has_self = "∃" maybe_ws object_property "." "Self"
-    object_property = object_property_iri "⁻"?
-
-    class_expression = class_iri / individual_list / parentheses
-    individual_list = "{" maybe_ws individual_iri (maybe_ws "⊔" maybe_ws individual_iri)* maybe_ws "}"
-
-    # Back to start symbol (first production rule)
-    parentheses = "(" maybe_ws union maybe_ws ")"
-
-    # Data properties
-    data_some_only_res = ("∃"/"∀") maybe_ws data_property_iri "." data_primary
-    data_cardinality_res = ("≥"/"≤"/"=") must_ws non_negative_integer must_ws data_property_iri "." data_primary
-    data_value_res = "∃" maybe_ws data_property_iri "." "{" literal "}"
-    data_primary = ("¬" maybe_ws)? data_range
-    data_range = datatype_restriction / datatype_iri / literal_list / data_parentheses
-    literal_list = "{" maybe_ws literal (maybe_ws "⊔" maybe_ws literal)* maybe_ws "}"
-    data_parentheses = "(" maybe_ws data_union maybe_ws ")"
-    data_union = data_intersection (must_ws "⊔" must_ws data_intersection)*
-    data_intersection = data_primary (must_ws "⊓" must_ws data_primary)*
-    datatype_restriction = datatype_iri "[" maybe_ws facet_restrictions maybe_ws "]"
-    facet_restrictions = facet_restriction (maybe_ws "," maybe_ws facet_restriction)*
-    facet_restriction = facet must_ws literal
-    facet = "length" / "minLength" / "maxLength" / "pattern" / "langRange"
-            / "totalDigits" / "fractionDigits" / "≥" / "≤" / "<" / ">"
-    datatype_iri = ("<http://www.w3.org/2001/XMLSchema#" datatype ">") / ("xsd:"? datatype)
-    datatype = "double" / "integer" / "boolean" / "string" / "dateTime" / "date" / "duration"
-
-    # Literals
-    literal = typed_literal / string_literal_language / string_literal_no_language / datetime_literal /
-              duration_literal / date_literal / float_literal / decimal_literal / integer_literal /
-              boolean_literal
-    typed_literal = quoted_string "^^" datatype_iri
-    string_literal_language = quoted_string language_tag
-    string_literal_no_language = quoted_string / no_match
-    quoted_string = ~"\"([^\"\\\\]|\\\\[\"\\\\])*\""
-    language_tag = "@" ~"[a-zA-Z]+" ("-" ~"[a-zA-Z0-9]+")*
-    float_literal = sign (float_with_integer_part / float_no_integer_part) ("f"/"F")
-    float_with_integer_part = non_negative_integer ("." ~"[0-9]+")? exponent?
-    float_no_integer_part = "." ~"[0-9]+" exponent?
-    exponent = ("e"/"E") sign ~"[0-9]+"
-    decimal_literal = sign non_negative_integer "." ~"[0-9]+"
-    integer_literal = sign non_negative_integer
-    boolean_literal = ~"[tT]rue" / ~"[fF]alse"
-    date_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))"
-    datetime_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))[T\u0020]"
-                       ~"(([0-1][0-9])|(2[0-3])):[0-5][0-9]:[0-5][0-9](\\.[0-9]{6})?"
-                       ~"(Z|([+-](([0-1][0-9])|(2[0-3])):[0-5][0-9](:[0-5][0-9](\\.[0-9]{6})?)?))?"
-    duration_literal = ~"P([0-9]+W)?([0-9]+D)?(T([0-9]+H)?([0-9]+M)?([0-9]+(\\.[0-9]{6})?S)?)?"
-    sign = ("+"/"-")?
-    non_negative_integer = ~"0|([1-9][0-9]*)"
-
-    # IRIs / Characters
-    class_iri = "⊤" / "⊥" / iri
-    object_property_iri = iri / no_match
-    data_property_iri = iri / no_match
-    individual_iri = iri / no_match
-    iri = full_iri / abbreviated_iri / simple_iri
-    full_iri = iri_ref / no_match
-    abbreviated_iri = pname_ln / no_match
-    simple_iri = pn_local / no_match
-
-    # Changes to ManchesterGrammar -- Don't allow:
-    # . used as a separator
-    # ⁻ used for inverse properties (\u207B)
-    iri_ref = "<" ~"[^<>\"{}|^`\\\\\u0000-\u0020]*" ">"
-    pname_ln = pname_ns pn_local
-    pname_ns = pn_prefix? ":"
-    pn_prefix = pn_chars_base pn_chars*
-    pn_local = (pn_chars_u / ~"[0-9]") pn_chars*
-    pn_chars = pn_chars_u / "-" / ~"[0-9]" / ~"\u00B7" / ~"[\u0300-\u036F]" / ~"[\u203F-\u2040]"
-    pn_chars_u = pn_chars_base / "_"
-    pn_chars_base = ~"[a-zA-Z]" / ~"[\u00C0-\u00D6]" / ~"[\u00D8-\u00F6]" / ~"[\u00F8-\u02FF]" /
-                    ~"[\u0370-\u037D]" / ~"[\u037F-\u1FFF]" / ~"[\u200C-\u200D]" / ~"[\u2070-\u207A]" /
-                    ~"[\u207C-\u218F]"/ ~"[\u2C00-\u2FEF]" / ~"[\u3001-\uD7FF]" / ~"[\uF900-\uFDCF]" /
-                    ~"[\uFDF0-\uFFFD]" / ~"[\U00010000-\U000EFFFF]"
-
-    must_ws = ~"[\u0020\u000D\u0009\u000A]+"
-    maybe_ws = ~"[\u0020\u000D\u0009\u000A]*"
-
-    # hacky workaround: can be added to a pass through production rule that is semantically important
-    # so nodes are not combined which makes the parsing cleaner
-    no_match = ~"(?!a)a"
-    """)
-
-
-# workaround to support multiple inheritance with different metaclasses
-class _DLSyntaxParserMeta(type(NodeVisitor), type(OWLObjectParser)):
-    pass
-
-
-class DLSyntaxParser(NodeVisitor, OWLObjectParser, metaclass=_DLSyntaxParserMeta):
-    """Description Logic Syntax parser to parse strings to OWLClassExpressions."""
-
-    slots = 'ns', 'grammar'
-
-    ns: Optional[Union[str, Namespaces]]
-
-    def __init__(self, namespace: Optional[Union[str, Namespaces]] = None, grammar=None):
-        """Create a new Description Logic Syntax parser. Names (entities) can be given as full IRIs enclosed in < and >
-           or as simple strings, in that case the namespace attribute of the parser has to be set to resolve them.
-           Prefixes are currently not supported, except for datatypes.
-
-        Args:
-            namespace: Namespace to resolve names that were given without one.
-            grammar: Grammar (defaults to DL_GRAMMAR).
-        """
-        self.ns = namespace
-        self.grammar = grammar
-
-        if self.grammar is None:
-            self.grammar = DL_GRAMMAR
-
-    def parse_expression(self, expression_str: str) -> OWLClassExpression:
-        tree = self.grammar.parse(expression_str.strip())
-        return self.visit(tree)
-
-    @_transform_children
-    def visit_union(self, node, children) -> OWLClassExpression:
-        return children if isinstance(children, OWLClassExpression) else OWLObjectUnionOf(children)
-
-    @_transform_children
-    def visit_intersection(self, node, children) -> OWLClassExpression:
-        return children if isinstance(children, OWLClassExpression) else OWLObjectIntersectionOf(children)
-
-    def visit_primary(self, node, children) -> OWLClassExpression:
-        match_not, expr = children
-        return OWLObjectComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
-
-    def visit_some_only_res(self, node, children) -> OWLQuantifiedObjectRestriction:
-        type_, _, property_, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _DL_SYNTAX.EXISTS:
-            return OWLObjectSomeValuesFrom(property_, filler)
-        else:
-            return OWLObjectAllValuesFrom(property_, filler)
-
-    def visit_cardinality_res(self, node, children) -> OWLObjectCardinalityRestriction:
-        type_, _, cardinality, _, property_, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _DL_SYNTAX.MIN:
-            return OWLObjectMinCardinality(cardinality, property_, filler)
-        elif type_ == _DL_SYNTAX.MAX:
-            return OWLObjectMaxCardinality(cardinality, property_, filler)
-        else:
-            return OWLObjectExactCardinality(cardinality, property_, filler)
-
-    def visit_value_res(self, node, children) -> OWLObjectHasValue:
-        _, _, property_, _, _, individual, _ = children
-        return OWLObjectHasValue(property_, individual)
-
-    def visit_has_self(self, node, children) -> OWLObjectHasSelf:
-        _, _, property_, _, _ = children
-        return OWLObjectHasSelf(property_)
-
-    def visit_object_property(self, node, children) -> OWLObjectPropertyExpression:
-        property_, inverse = children
-        return property_.get_inverse_property() if isinstance(inverse, list) else property_
-
-    def visit_class_expression(self, node, children) -> OWLClassExpression:
-        return children[0]
-
-    @_transform_children
-    def visit_individual_list(self, node, children) -> OWLObjectOneOf:
-        return OWLObjectOneOf(children)
-
-    def visit_data_primary(self, node, children) -> OWLDataRange:
-        match_not, expr = children
-        return OWLDataComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
-
-    def visit_data_some_only_res(self, node, children) -> OWLQuantifiedDataRestriction:
-        type_, _, property_, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _DL_SYNTAX.EXISTS:
-            return OWLDataSomeValuesFrom(property_, filler)
-        else:
-            return OWLDataAllValuesFrom(property_, filler)
-
-    def visit_data_cardinality_res(self, node, children) -> OWLDataCardinalityRestriction:
-        type_, _, cardinality, _, property_, _, filler = children
-        type_ = _node_text(*type_)
-        if type_ == _DL_SYNTAX.MIN:
-            return OWLDataMinCardinality(cardinality, property_, filler)
-        elif type_ == _DL_SYNTAX.MAX:
-            return OWLDataMaxCardinality(cardinality, property_, filler)
-        else:
-            return OWLDataExactCardinality(cardinality, property_, filler)
-
-    def visit_data_value_res(self, node, children) -> OWLDataHasValue:
-        _, _, property_, _, _, literal, _ = children
-        return OWLDataHasValue(property_, literal)
-
-    @_transform_children
-    def visit_data_union(self, node, children) -> OWLDataRange:
-        return children if isinstance(children, OWLDataRange) else OWLDataUnionOf(children)
-
-    @_transform_children
-    def visit_data_intersection(self, node, children) -> OWLDataRange:
-        return children if isinstance(children, OWLDataRange) else OWLDataIntersectionOf(children)
-
-    @_transform_children
-    def visit_literal_list(self, node, children) -> OWLDataOneOf:
-        return OWLDataOneOf(children)
-
-    def visit_data_parentheses(self, node, children) -> OWLDataRange:
-        *_, expr, _, _ = children
-        return expr
-
-    def visit_datatype_restriction(self, node, children) -> OWLDatatypeRestriction:
-        datatype, *_, facet_restrictions, _, _ = children
-        if isinstance(facet_restrictions, OWLFacetRestriction):
-            facet_restrictions = facet_restrictions,
-        not_valid_literals = []
-        if datatype != StringOWLDatatype:
-            not_valid_literals = [res.get_facet_value() for res in facet_restrictions
-                                  if res.get_facet_value().get_datatype() != datatype]
-        not_valid_facets = [res.get_facet() for res in facet_restrictions
-                            if res.get_facet() not in _DATATYPE_TO_FACETS[datatype]]
-
-        if not_valid_literals or not_valid_facets:
-            raise ValueError(f"Literals: {not_valid_literals} and Facets: {not_valid_facets}"
-                             f" not valid for datatype: {datatype}")
-        return OWLDatatypeRestriction(datatype, facet_restrictions)
-
-    @_transform_children
-    def visit_facet_restrictions(self, node, children) -> List[OWLFacetRestriction]:
-        return children
-
-    def visit_facet_restriction(self, node, children) -> OWLFacetRestriction:
-        facet, _, literal = children
-        if literal.get_datatype() not in _FACET_TO_LITERAL_DATATYPE[facet]:
-            raise ValueError(f"Literal: {literal} not valid for facet: {facet}")
-        return OWLFacetRestriction(facet, literal)
-
-    def visit_literal(self, node, children) -> OWLLiteral:
-        return children[0]
-
-    def visit_typed_literal(self, node, children) -> OWLLiteral:
-        value, _, datatype = children
-        return OWLLiteral(value[1:-1], datatype)
-
-    def visit_string_literal_language(self, node, children):
-        raise NotImplementedError(f"Language tags and plain literals not supported in owlapy yet: {_node_text(node)}")
-
-    def visit_string_literal_no_language(self, node, children) -> OWLLiteral:
-        value = children[0]
-        return OWLLiteral(value[1:-1], StringOWLDatatype)
-
-    def visit_quoted_string(self, node, children) -> str:
-        return _node_text(node)
-
-    def visit_float_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node)[:-1], DoubleOWLDatatype)
-
-    def visit_decimal_literal(self, node, children) -> OWLLiteral:
-        # TODO: Just use float for now, decimal not supported in owlapy yet
-        return OWLLiteral(_node_text(node), DoubleOWLDatatype)
-
-    def visit_integer_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), IntegerOWLDatatype)
-
-    def visit_boolean_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), BooleanOWLDatatype)
-
-    def visit_datetime_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), DateTimeOWLDatatype)
-
-    def visit_duration_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), DurationOWLDatatype)
-
-    def visit_date_literal(self, node, children) -> OWLLiteral:
-        return OWLLiteral(_node_text(node), DateOWLDatatype)
-
-    def visit_non_negative_integer(self, node, children) -> int:
-        return int(_node_text(node))
-
-    def visit_datatype_iri(self, node, children) -> str:
-        return children[0][1]
-
-    def visit_datatype(self, node, children) -> OWLDatatype:
-        return _STRING_TO_DATATYPE[_node_text(node)]
-
-    def visit_facet(self, node, children) -> OWLFacet:
-        symbolic_form = _node_text(node)
-        if symbolic_form == _DL_SYNTAX.MIN:
-            symbolic_form = '>='
-        elif symbolic_form == _DL_SYNTAX.MAX:
-            symbolic_form = '<='
-        return OWLFacet.from_str(symbolic_form)
-
-    def visit_class_iri(self, node, children) -> OWLClass:
-        top_bottom = _node_text(node)
-        if top_bottom == _DL_SYNTAX.TOP:
-            return OWLClass(OWLRDFVocabulary.OWL_THING.get_iri())
-        elif top_bottom == _DL_SYNTAX.BOTTOM:
-            return OWLClass(OWLRDFVocabulary.OWL_NOTHING.get_iri())
-        else:
-            return OWLClass(children[0])
-
-    def visit_individual_iri(self, node, children) -> OWLNamedIndividual:
-        return OWLNamedIndividual(children[0])
-
-    def visit_object_property_iri(self, node, children) -> OWLObjectProperty:
-        return OWLObjectProperty(children[0])
-
-    def visit_data_property_iri(self, node, children) -> OWLDataProperty:
-        return OWLDataProperty(children[0])
-
-    def visit_iri(self, node, children) -> IRI:
-        return children[0]
-
-    def visit_full_iri(self, node, children) -> IRI:
-        try:
-            iri = _node_text(node)[1:-1]
-            return IRI.create(iri)
-        except IndexError:
-            raise ValueError(f"{iri} is not a valid IRI.")
-
-    def visit_abbreviated_iri(self, node, children):
-        # TODO: Add support for prefixes
-        raise NotImplementedError(f"Parsing of prefixes is not supported yet: {_node_text(node)}")
-
-    def visit_simple_iri(self, node, children) -> IRI:
-        simple_iri = _node_text(node)
-        if self.ns is not None:
-            return IRI(self.ns, simple_iri)
-        else:
-            raise ValueError(f"If entities are specified without a full iri ({simple_iri}), "
-                             "the namespace attribute of the parser has to be set.")
-
-    def visit_parentheses(self, node, children) -> OWLClassExpression:
-        *_, expr, _, _ = children
-        return expr
-
-    def generic_visit(self, node, children):
-        return children or node
-
-
-DLparser = DLSyntaxParser()
-ManchesterParser = ManchesterOWLSyntaxParser()
-
-
-def dl_to_owl_expression(dl_expression: str):
-    return DLparser.parse_expression(dl_expression)
-
-
-def manchester_to_owl_expression(manchester_expression: str):
-    return ManchesterParser.parse_expression(manchester_expression)
+"""String to OWL parsers."""
+from types import MappingProxyType
+from typing import Final, List, Optional, Union
+from parsimonious.grammar import Grammar
+from parsimonious.nodes import NodeVisitor
+from parsimonious.nodes import Node
+from .iri import IRI
+from .owl_individual import OWLNamedIndividual
+from .owl_literal import IntegerOWLDatatype, BooleanOWLDatatype, DoubleOWLDatatype, StringOWLDatatype, DateOWLDatatype, \
+    DateTimeOWLDatatype, DurationOWLDatatype, OWLLiteral
+from .owl_property import OWLObjectPropertyExpression, OWLObjectProperty, OWLDataProperty
+from .owl_object import OWLObjectParser
+from .namespaces import Namespaces
+from .render import _DL_SYNTAX, _MAN_SYNTAX
+from .owl_datatype import OWLDatatype
+from .vocab import OWLFacet, OWLRDFVocabulary
+from owlapy.class_expression import OWLObjectHasSelf, OWLObjectIntersectionOf, OWLObjectMinCardinality, \
+    OWLObjectSomeValuesFrom, OWLObjectUnionOf, OWLClass, OWLObjectOneOf, \
+    OWLClassExpression, OWLObjectComplementOf, OWLObjectExactCardinality, \
+    OWLQuantifiedDataRestriction, OWLQuantifiedObjectRestriction,  OWLFacetRestriction, \
+    OWLDataSomeValuesFrom, OWLDataExactCardinality, OWLObjectHasValue, \
+    OWLDataMaxCardinality, OWLObjectMaxCardinality, OWLDataMinCardinality, OWLDataHasValue, \
+    OWLDataOneOf, OWLObjectCardinalityRestriction, OWLDatatypeRestriction, \
+    OWLDataCardinalityRestriction, OWLObjectAllValuesFrom, OWLDataAllValuesFrom
+from owlapy.owl_data_ranges import OWLDataIntersectionOf, OWLDataUnionOf, OWLDataComplementOf, OWLDataRange
+
+
+MANCHESTER_GRAMMAR = Grammar(r"""
+    union = intersection (must_ws "or" must_ws intersection)*
+    intersection = primary (must_ws "and" must_ws primary)*
+
+    # Main entry point + object properties
+    primary = ("not" must_ws)? (data_some_only_res / some_only_res / data_cardinality_res / cardinality_res
+                           / data_value_res / value_res / has_self / class_expression)
+    some_only_res = object_property must_ws ("some"/"only") must_ws primary
+    cardinality_res = object_property must_ws ("max"/"min"/"exactly") must_ws non_negative_integer must_ws primary
+    value_res = object_property must_ws "value" must_ws individual_iri
+    has_self = object_property must_ws "Self"
+    object_property = ("inverse" must_ws)? object_property_iri
+    class_expression = class_iri / individual_list / parentheses
+    individual_list = "{" maybe_ws individual_iri (maybe_ws "," maybe_ws individual_iri)* maybe_ws "}"
+
+    # Back to start symbol (first production rule)
+    parentheses = "(" maybe_ws union maybe_ws ")"
+
+    # Data properties
+    data_some_only_res = data_property_iri must_ws ("some"/"only") must_ws data_primary
+    data_cardinality_res = data_property_iri must_ws ("max"/"min"/"exactly")
+                           must_ws non_negative_integer must_ws data_primary
+    data_value_res = data_property_iri must_ws "value" must_ws literal
+    data_primary = ("not" must_ws)? data_range
+    data_range = datatype_restriction / datatype_iri / literal_list / data_parentheses
+    literal_list = "{" maybe_ws literal (maybe_ws "," maybe_ws literal)* maybe_ws "}"
+    data_parentheses = "(" maybe_ws data_union maybe_ws ")"
+    data_union = data_intersection (must_ws "or" must_ws data_intersection)*
+    data_intersection = data_primary (must_ws "and" must_ws data_primary)*
+    datatype_restriction = datatype_iri "[" maybe_ws facet_restrictions maybe_ws "]"
+    facet_restrictions = facet_restriction (maybe_ws "," maybe_ws facet_restriction)*
+    facet_restriction = facet must_ws literal
+    facet = "length" / "minLength" / "maxLength" / "pattern" / "langRange"
+            / "totalDigits" / "fractionDigits" / "<=" / ">=" / "<" / ">"
+    datatype_iri = ("<http://www.w3.org/2001/XMLSchema#" datatype ">") / ("xsd:"? datatype)
+    datatype = "double" / "integer" / "boolean" / "string" / "dateTime" / "date" / "duration"
+
+    # Literals
+    literal = typed_literal / string_literal_language / string_literal_no_language / datetime_literal /
+              duration_literal / date_literal / float_literal / decimal_literal / integer_literal /
+              boolean_literal
+    typed_literal = quoted_string "^^" datatype_iri
+    string_literal_language = quoted_string language_tag
+    string_literal_no_language = quoted_string / no_match
+    quoted_string = ~"\"([^\"\\\\]|\\\\[\"\\\\])*\""
+    language_tag = "@" ~"[a-zA-Z]+" ("-" ~"[a-zA-Z0-9]+")*
+    float_literal = sign (float_with_integer_part / float_no_integer_part) ("f"/"F")
+    float_with_integer_part = non_negative_integer ("." ~"[0-9]+")? exponent?
+    float_no_integer_part = "." ~"[0-9]+" exponent?
+    exponent = ("e"/"E") sign ~"[0-9]+"
+    decimal_literal = sign non_negative_integer "." ~"[0-9]+"
+    integer_literal = sign non_negative_integer
+    boolean_literal = ~"[tT]rue" / ~"[fF]alse"
+    date_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))"
+    datetime_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))[T\u0020]"
+                       ~"(([0-1][0-9])|(2[0-3])):[0-5][0-9]:[0-5][0-9](\\.[0-9]{6})?"
+                       ~"(Z|([+-](([0-1][0-9])|(2[0-3])):[0-5][0-9](:[0-5][0-9](\\.[0-9]{6})?)?))?"
+    duration_literal = ~"P([0-9]+W)?([0-9]+D)?(T([0-9]+H)?([0-9]+M)?([0-9]+(\\.[0-9]{6})?S)?)?"
+    sign = ("+"/"-")?
+    non_negative_integer = ~"0|([1-9][0-9]*)"
+
+    # IRIs / Characters
+    class_iri = iri / no_match
+    individual_iri = iri / no_match
+    object_property_iri = iri / no_match
+    data_property_iri = iri / no_match
+    iri = full_iri / abbreviated_iri / simple_iri
+    full_iri = iri_ref / no_match
+    abbreviated_iri = pname_ln / no_match
+    simple_iri = pn_local / no_match
+
+    iri_ref = "<" ~"[^<>\"{}|^`\\\\\u0000-\u0020]*" ">"
+    pname_ln = pname_ns pn_local
+    pname_ns = pn_prefix? ":"
+    pn_prefix = pn_chars_base ("."* pn_chars)*
+    pn_local = (pn_chars_u / ~"[0-9]") ("."* pn_chars)*
+    pn_chars = pn_chars_u / "-" / ~"[0-9]" / ~"\u00B7" / ~"[\u0300-\u036F]" / ~"[\u203F-\u2040]"
+    pn_chars_u = pn_chars_base / "_"
+    pn_chars_base = ~"[a-zA-Z]" / ~"[\u00C0-\u00D6]" / ~"[\u00D8-\u00F6]" / ~"[\u00F8-\u02FF]" /
+                    ~"[\u0370-\u037D]" / ~"[\u037F-\u1FFF]" / ~"[\u200C-\u200D]" / ~"[\u2070-\u218F]" /
+                    ~"[\u2C00-\u2FEF]" / ~"[\u3001-\uD7FF]" / ~"[\uF900-\uFDCF]" / ~"[\uFDF0-\uFFFD]" /
+                    ~"[\U00010000-\U000EFFFF]"
+
+    must_ws = ~"[\u0020\u000D\u0009\u000A]+"
+    maybe_ws = ~"[\u0020\u000D\u0009\u000A]*"
+
+    # hacky workaround: can be added to a pass through production rule that is semantically important
+    # so nodes are not combined which makes the parsing cleaner
+    no_match = ~"(?!a)a"
+    """)
+
+
+def _transform_children(nary_visit_function):
+    def transform(self, node, visited_children):
+        if len(visited_children) > 2:
+            *_, first_operand, operands, _, _ = visited_children
+        else:
+            first_operand, operands = visited_children
+        children = first_operand if isinstance(operands, Node) else [first_operand] + [node[-1] for node in operands]
+        return nary_visit_function(self, node, children)
+    return transform
+
+
+def _node_text(node) -> str:
+    return node.text.strip()
+
+
+_STRING_TO_DATATYPE: Final = MappingProxyType({
+    "integer": IntegerOWLDatatype,
+    "double": DoubleOWLDatatype,
+    "boolean": BooleanOWLDatatype,
+    "string": StringOWLDatatype,
+    "date": DateOWLDatatype,
+    "dateTime": DateTimeOWLDatatype,
+    "duration": DurationOWLDatatype,
+})
+
+
+_DATATYPE_TO_FACETS: Final = MappingProxyType({
+    IntegerOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE, OWLFacet.MAX_EXCLUSIVE,
+                         OWLFacet.MAX_INCLUSIVE, OWLFacet.TOTAL_DIGITS},
+    DoubleOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE, OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
+    DateOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE, OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
+    DateTimeOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE,
+                          OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
+    DurationOWLDatatype: {OWLFacet.MIN_INCLUSIVE, OWLFacet.MIN_EXCLUSIVE,
+                          OWLFacet.MAX_EXCLUSIVE, OWLFacet.MAX_INCLUSIVE},
+    StringOWLDatatype: {OWLFacet.LENGTH, OWLFacet.MIN_LENGTH, OWLFacet.MAX_LENGTH, OWLFacet.PATTERN},
+    BooleanOWLDatatype: {}
+})
+
+
+_FACET_TO_LITERAL_DATATYPE: Final = MappingProxyType({
+    OWLFacet.MIN_EXCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
+                             DateTimeOWLDatatype, DurationOWLDatatype},
+    OWLFacet.MAX_EXCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
+                             DateTimeOWLDatatype, DurationOWLDatatype},
+    OWLFacet.MIN_INCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
+                             DateTimeOWLDatatype, DurationOWLDatatype},
+    OWLFacet.MAX_INCLUSIVE: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype,
+                             DateTimeOWLDatatype, DurationOWLDatatype},
+    OWLFacet.PATTERN: {IntegerOWLDatatype, DoubleOWLDatatype, DateOWLDatatype, DateTimeOWLDatatype,
+                       DurationOWLDatatype, StringOWLDatatype},
+    OWLFacet.LENGTH: {IntegerOWLDatatype},
+    OWLFacet.MIN_LENGTH: {IntegerOWLDatatype},
+    OWLFacet.MAX_LENGTH: {IntegerOWLDatatype},
+    OWLFacet.TOTAL_DIGITS: {IntegerOWLDatatype},
+    OWLFacet.FRACTION_DIGITS: {IntegerOWLDatatype}
+})
+
+
+# workaround to support multiple inheritance with different metaclasses
+class _ManchesterOWLSyntaxParserMeta(type(NodeVisitor), type(OWLObjectParser)):
+    pass
+
+
+class ManchesterOWLSyntaxParser(NodeVisitor, OWLObjectParser, metaclass=_ManchesterOWLSyntaxParserMeta):
+    """Manchester Syntax parser to parse strings to OWLClassExpressions.
+       Following: https://www.w3.org/TR/owl2-manchester-syntax."""
+
+    slots = 'ns', 'grammar'
+
+    ns: Optional[Union[str, Namespaces]]
+
+    def __init__(self, namespace: Optional[Union[str, Namespaces]] = None, grammar=None):
+        """Create a new Manchester Syntax parser. Names (entities) can be given as full IRIs enclosed in < and >
+           or as simple strings, in that case the namespace attribute of the parser has to be set to resolve them.
+           See https://www.w3.org/TR/owl2-manchester-syntax/#IRIs.2C_Integers.2C_Literals.2C_and_Entities
+           for more information.
+           Prefixes are currently not supported, except for datatypes.
+
+        Args:
+            namespace: Namespace to resolve names that were given without one.
+            grammar: Grammar (defaults to MANCHESTERGRAMMAR).
+        """
+        self.ns = namespace
+        self.grammar = grammar
+
+        if self.grammar is None:
+            self.grammar = MANCHESTER_GRAMMAR
+
+    def parse_expression(self, expression_str: str) -> OWLClassExpression:
+        tree = self.grammar.parse(expression_str.strip())
+        return self.visit(tree)
+
+    @_transform_children
+    def visit_union(self, node, children) -> OWLClassExpression:
+        return children if isinstance(children, OWLClassExpression) else OWLObjectUnionOf(children)
+
+    @_transform_children
+    def visit_intersection(self, node, children) -> OWLClassExpression:
+        return children if isinstance(children, OWLClassExpression) else OWLObjectIntersectionOf(children)
+
+    def visit_primary(self, node, children) -> OWLClassExpression:
+        match_not, expr = children
+        return OWLObjectComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
+
+    def visit_some_only_res(self, node, children) -> OWLQuantifiedObjectRestriction:
+        property_, _, type_, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _MAN_SYNTAX.EXISTS:
+            return OWLObjectSomeValuesFrom(property_, filler)
+        else:
+            return OWLObjectAllValuesFrom(property_, filler)
+
+    def visit_cardinality_res(self, node, children) -> OWLObjectCardinalityRestriction:
+        property_, _, type_, _, cardinality, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _MAN_SYNTAX.MIN:
+            return OWLObjectMinCardinality(cardinality, property_, filler)
+        elif type_ == _MAN_SYNTAX.MAX:
+            return OWLObjectMaxCardinality(cardinality, property_, filler)
+        else:
+            return OWLObjectExactCardinality(cardinality, property_, filler)
+
+    def visit_value_res(self, node, children) -> OWLObjectHasValue:
+        property_, *_, individual = children
+        return OWLObjectHasValue(property_, individual)
+
+    def visit_has_self(self, node, children) -> OWLObjectHasSelf:
+        property_, *_ = children
+        return OWLObjectHasSelf(property_)
+
+    def visit_object_property(self, node, children) -> OWLObjectPropertyExpression:
+        inverse, property_ = children
+        return property_.get_inverse_property() if isinstance(inverse, list) else property_
+
+    def visit_class_expression(self, node, children) -> OWLClassExpression:
+        return children[0]
+
+    @_transform_children
+    def visit_individual_list(self, node, children) -> OWLObjectOneOf:
+        return OWLObjectOneOf(children)
+
+    def visit_data_primary(self, node, children) -> OWLDataRange:
+        match_not, expr = children
+        return OWLDataComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
+
+    def visit_data_some_only_res(self, node, children) -> OWLQuantifiedDataRestriction:
+        property_, _, type_, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _MAN_SYNTAX.EXISTS:
+            return OWLDataSomeValuesFrom(property_, filler)
+        else:
+            return OWLDataAllValuesFrom(property_, filler)
+
+    def visit_data_cardinality_res(self, node, children) -> OWLDataCardinalityRestriction:
+        property_, _, type_, _, cardinality, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _MAN_SYNTAX.MIN:
+            return OWLDataMinCardinality(cardinality, property_, filler)
+        elif type_ == _MAN_SYNTAX.MAX:
+            return OWLDataMaxCardinality(cardinality, property_, filler)
+        else:
+            return OWLDataExactCardinality(cardinality, property_, filler)
+
+    def visit_data_value_res(self, node, children) -> OWLDataHasValue:
+        property_, *_, literal = children
+        return OWLDataHasValue(property_, literal)
+
+    @_transform_children
+    def visit_data_union(self, node, children) -> OWLDataRange:
+        return children if isinstance(children, OWLDataRange) else OWLDataUnionOf(children)
+
+    @_transform_children
+    def visit_data_intersection(self, node, children) -> OWLDataRange:
+        return children if isinstance(children, OWLDataRange) else OWLDataIntersectionOf(children)
+
+    @_transform_children
+    def visit_literal_list(self, node, children) -> OWLDataOneOf:
+        return OWLDataOneOf(children)
+
+    def visit_data_parentheses(self, node, children) -> OWLDataRange:
+        *_, expr, _, _ = children
+        return expr
+
+    def visit_datatype_restriction(self, node, children) -> OWLDatatypeRestriction:
+        datatype, *_, facet_restrictions, _, _ = children
+        if isinstance(facet_restrictions, OWLFacetRestriction):
+            facet_restrictions = facet_restrictions,
+        not_valid_literals = []
+        if datatype != StringOWLDatatype:
+            not_valid_literals = [res.get_facet_value() for res in facet_restrictions
+                                  if res.get_facet_value().get_datatype() != datatype]
+        not_valid_facets = [res.get_facet() for res in facet_restrictions
+                            if res.get_facet() not in _DATATYPE_TO_FACETS[datatype]]
+
+        if not_valid_literals or not_valid_facets:
+            raise ValueError(f"Literals: {not_valid_literals} and Facets: {not_valid_facets}"
+                             f" not valid for datatype: {datatype}")
+        return OWLDatatypeRestriction(datatype, facet_restrictions)
+
+    @_transform_children
+    def visit_facet_restrictions(self, node, children) -> List[OWLFacetRestriction]:
+        return children
+
+    def visit_facet_restriction(self, node, children) -> OWLFacetRestriction:
+        facet, _, literal = children
+        if literal.get_datatype() not in _FACET_TO_LITERAL_DATATYPE[facet]:
+            raise ValueError(f"Literal: {literal} not valid for facet: {facet}")
+        return OWLFacetRestriction(facet, literal)
+
+    def visit_literal(self, node, children) -> OWLLiteral:
+        return children[0]
+
+    def visit_typed_literal(self, node, children) -> OWLLiteral:
+        value, _, datatype = children
+        return OWLLiteral(value[1:-1], datatype)
+
+    def visit_string_literal_language(self, node, children):
+        raise NotImplementedError(f"Language tags and plain literals not supported in owlapy yet: {_node_text(node)}")
+
+    def visit_string_literal_no_language(self, node, children) -> OWLLiteral:
+        value = children[0]
+        return OWLLiteral(value[1:-1], StringOWLDatatype)
+
+    def visit_quoted_string(self, node, children) -> str:
+        return _node_text(node)
+
+    def visit_float_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node)[:-1], DoubleOWLDatatype)
+
+    def visit_decimal_literal(self, node, children) -> OWLLiteral:
+        # TODO: Just use float for now, decimal not supported in owlapy yet
+        return OWLLiteral(_node_text(node), DoubleOWLDatatype)
+
+    def visit_integer_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), IntegerOWLDatatype)
+
+    def visit_boolean_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), BooleanOWLDatatype)
+
+    def visit_datetime_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), DateTimeOWLDatatype)
+
+    def visit_duration_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), DurationOWLDatatype)
+
+    def visit_date_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), DateOWLDatatype)
+
+    def visit_non_negative_integer(self, node, children) -> int:
+        return int(_node_text(node))
+
+    def visit_datatype_iri(self, node, children) -> str:
+        return children[0][1]
+
+    def visit_datatype(self, node, children) -> OWLDatatype:
+        return _STRING_TO_DATATYPE[_node_text(node)]
+
+    def visit_facet(self, node, children) -> OWLFacet:
+        return OWLFacet.from_str(_node_text(node))
+
+    def visit_class_iri(self, node, children) -> OWLClass:
+        return OWLClass(children[0])
+
+    def visit_individual_iri(self, node, children) -> OWLNamedIndividual:
+        return OWLNamedIndividual(children[0])
+
+    def visit_object_property_iri(self, node, children) -> OWLObjectProperty:
+        return OWLObjectProperty(children[0])
+
+    def visit_data_property_iri(self, node, children) -> OWLDataProperty:
+        return OWLDataProperty(children[0])
+
+    def visit_iri(self, node, children) -> IRI:
+        return children[0]
+
+    def visit_full_iri(self, node, children) -> IRI:
+        try:
+            iri = _node_text(node)[1:-1]
+            return IRI.create(iri)
+        except IndexError:
+            raise ValueError(f"{iri} is not a valid IRI.")
+
+    def visit_abbreviated_iri(self, node, children):
+        # TODO: Add support for prefixes
+        raise NotImplementedError(f"Parsing of prefixes is not supported yet: {_node_text(node)}")
+
+    def visit_simple_iri(self, node, children) -> IRI:
+        simple_iri = _node_text(node)
+        if simple_iri == "Thing":
+            return OWLRDFVocabulary.OWL_THING.iri
+        elif simple_iri == "Nothing":
+            return OWLRDFVocabulary.OWL_NOTHING.iri
+        elif self.ns is not None:
+            return IRI(self.ns, simple_iri)
+        else:
+            raise ValueError(f"If entities are specified without a full iri ({simple_iri}), "
+                             "the namespace attribute of the parser has to be set.")
+
+    def visit_parentheses(self, node, children) -> OWLClassExpression:
+        *_, expr, _, _ = children
+        return expr
+
+    def generic_visit(self, node, children):
+        return children or node
+
+
+DL_GRAMMAR = Grammar(r"""
+    union = intersection (must_ws "⊔" must_ws intersection)*
+    intersection = primary (must_ws "⊓" must_ws primary)*
+
+    # Main entry point + object properties
+    primary = ("¬" maybe_ws)? (has_self / data_value_res / value_res / data_some_only_res / some_only_res /
+                data_cardinality_res / cardinality_res / class_expression)
+    some_only_res = ("∃"/"∀") maybe_ws object_property "." primary
+    cardinality_res = ("≥"/"≤"/"=") must_ws non_negative_integer must_ws object_property "." primary
+    value_res = "∃" maybe_ws object_property "." "{" individual_iri "}"
+    has_self = "∃" maybe_ws object_property "." "Self"
+    object_property = object_property_iri "⁻"?
+
+    class_expression = class_iri / individual_list / parentheses
+    individual_list = "{" maybe_ws individual_iri (maybe_ws "⊔" maybe_ws individual_iri)* maybe_ws "}"
+
+    # Back to start symbol (first production rule)
+    parentheses = "(" maybe_ws union maybe_ws ")"
+
+    # Data properties
+    data_some_only_res = ("∃"/"∀") maybe_ws data_property_iri "." data_primary
+    data_cardinality_res = ("≥"/"≤"/"=") must_ws non_negative_integer must_ws data_property_iri "." data_primary
+    data_value_res = "∃" maybe_ws data_property_iri "." "{" literal "}"
+    data_primary = ("¬" maybe_ws)? data_range
+    data_range = datatype_restriction / datatype_iri / literal_list / data_parentheses
+    literal_list = "{" maybe_ws literal (maybe_ws "⊔" maybe_ws literal)* maybe_ws "}"
+    data_parentheses = "(" maybe_ws data_union maybe_ws ")"
+    data_union = data_intersection (must_ws "⊔" must_ws data_intersection)*
+    data_intersection = data_primary (must_ws "⊓" must_ws data_primary)*
+    datatype_restriction = datatype_iri "[" maybe_ws facet_restrictions maybe_ws "]"
+    facet_restrictions = facet_restriction (maybe_ws "," maybe_ws facet_restriction)*
+    facet_restriction = facet must_ws literal
+    facet = "length" / "minLength" / "maxLength" / "pattern" / "langRange"
+            / "totalDigits" / "fractionDigits" / "≥" / "≤" / "<" / ">"
+    datatype_iri = ("<http://www.w3.org/2001/XMLSchema#" datatype ">") / ("xsd:"? datatype)
+    datatype = "double" / "integer" / "boolean" / "string" / "dateTime" / "date" / "duration"
+
+    # Literals
+    literal = typed_literal / string_literal_language / string_literal_no_language / datetime_literal /
+              duration_literal / date_literal / float_literal / decimal_literal / integer_literal /
+              boolean_literal
+    typed_literal = quoted_string "^^" datatype_iri
+    string_literal_language = quoted_string language_tag
+    string_literal_no_language = quoted_string / no_match
+    quoted_string = ~"\"([^\"\\\\]|\\\\[\"\\\\])*\""
+    language_tag = "@" ~"[a-zA-Z]+" ("-" ~"[a-zA-Z0-9]+")*
+    float_literal = sign (float_with_integer_part / float_no_integer_part) ("f"/"F")
+    float_with_integer_part = non_negative_integer ("." ~"[0-9]+")? exponent?
+    float_no_integer_part = "." ~"[0-9]+" exponent?
+    exponent = ("e"/"E") sign ~"[0-9]+"
+    decimal_literal = sign non_negative_integer "." ~"[0-9]+"
+    integer_literal = sign non_negative_integer
+    boolean_literal = ~"[tT]rue" / ~"[fF]alse"
+    date_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))"
+    datetime_literal = ~"[0-9]{4}-((0[1-9])|(1[0-2]))-(([0-2][0-9])|(3[01]))[T\u0020]"
+                       ~"(([0-1][0-9])|(2[0-3])):[0-5][0-9]:[0-5][0-9](\\.[0-9]{6})?"
+                       ~"(Z|([+-](([0-1][0-9])|(2[0-3])):[0-5][0-9](:[0-5][0-9](\\.[0-9]{6})?)?))?"
+    duration_literal = ~"P([0-9]+W)?([0-9]+D)?(T([0-9]+H)?([0-9]+M)?([0-9]+(\\.[0-9]{6})?S)?)?"
+    sign = ("+"/"-")?
+    non_negative_integer = ~"0|([1-9][0-9]*)"
+
+    # IRIs / Characters
+    class_iri = "⊤" / "⊥" / iri
+    object_property_iri = iri / no_match
+    data_property_iri = iri / no_match
+    individual_iri = iri / no_match
+    iri = full_iri / abbreviated_iri / simple_iri
+    full_iri = iri_ref / no_match
+    abbreviated_iri = pname_ln / no_match
+    simple_iri = pn_local / no_match
+
+    # Changes to ManchesterGrammar -- Don't allow:
+    # . used as a separator
+    # ⁻ used for inverse properties (\u207B)
+    iri_ref = "<" ~"[^<>\"{}|^`\\\\\u0000-\u0020]*" ">"
+    pname_ln = pname_ns pn_local
+    pname_ns = pn_prefix? ":"
+    pn_prefix = pn_chars_base pn_chars*
+    pn_local = (pn_chars_u / ~"[0-9]") pn_chars*
+    pn_chars = pn_chars_u / "-" / ~"[0-9]" / ~"\u00B7" / ~"[\u0300-\u036F]" / ~"[\u203F-\u2040]"
+    pn_chars_u = pn_chars_base / "_"
+    pn_chars_base = ~"[a-zA-Z]" / ~"[\u00C0-\u00D6]" / ~"[\u00D8-\u00F6]" / ~"[\u00F8-\u02FF]" /
+                    ~"[\u0370-\u037D]" / ~"[\u037F-\u1FFF]" / ~"[\u200C-\u200D]" / ~"[\u2070-\u207A]" /
+                    ~"[\u207C-\u218F]"/ ~"[\u2C00-\u2FEF]" / ~"[\u3001-\uD7FF]" / ~"[\uF900-\uFDCF]" /
+                    ~"[\uFDF0-\uFFFD]" / ~"[\U00010000-\U000EFFFF]"
+
+    must_ws = ~"[\u0020\u000D\u0009\u000A]+"
+    maybe_ws = ~"[\u0020\u000D\u0009\u000A]*"
+
+    # hacky workaround: can be added to a pass through production rule that is semantically important
+    # so nodes are not combined which makes the parsing cleaner
+    no_match = ~"(?!a)a"
+    """)
+
+
+# workaround to support multiple inheritance with different metaclasses
+class _DLSyntaxParserMeta(type(NodeVisitor), type(OWLObjectParser)):
+    pass
+
+
+class DLSyntaxParser(NodeVisitor, OWLObjectParser, metaclass=_DLSyntaxParserMeta):
+    """Description Logic Syntax parser to parse strings to OWLClassExpressions."""
+
+    slots = 'ns', 'grammar'
+
+    ns: Optional[Union[str, Namespaces]]
+
+    def __init__(self, namespace: Optional[Union[str, Namespaces]] = None, grammar=None):
+        """Create a new Description Logic Syntax parser. Names (entities) can be given as full IRIs enclosed in < and >
+           or as simple strings, in that case the namespace attribute of the parser has to be set to resolve them.
+           Prefixes are currently not supported, except for datatypes.
+
+        Args:
+            namespace: Namespace to resolve names that were given without one.
+            grammar: Grammar (defaults to DL_GRAMMAR).
+        """
+        self.ns = namespace
+        self.grammar = grammar
+
+        if self.grammar is None:
+            self.grammar = DL_GRAMMAR
+
+    def parse_expression(self, expression_str: str) -> OWLClassExpression:
+        tree = self.grammar.parse(expression_str.strip())
+        return self.visit(tree)
+
+    @_transform_children
+    def visit_union(self, node, children) -> OWLClassExpression:
+        return children if isinstance(children, OWLClassExpression) else OWLObjectUnionOf(children)
+
+    @_transform_children
+    def visit_intersection(self, node, children) -> OWLClassExpression:
+        return children if isinstance(children, OWLClassExpression) else OWLObjectIntersectionOf(children)
+
+    def visit_primary(self, node, children) -> OWLClassExpression:
+        match_not, expr = children
+        return OWLObjectComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
+
+    def visit_some_only_res(self, node, children) -> OWLQuantifiedObjectRestriction:
+        type_, _, property_, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _DL_SYNTAX.EXISTS:
+            return OWLObjectSomeValuesFrom(property_, filler)
+        else:
+            return OWLObjectAllValuesFrom(property_, filler)
+
+    def visit_cardinality_res(self, node, children) -> OWLObjectCardinalityRestriction:
+        type_, _, cardinality, _, property_, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _DL_SYNTAX.MIN:
+            return OWLObjectMinCardinality(cardinality, property_, filler)
+        elif type_ == _DL_SYNTAX.MAX:
+            return OWLObjectMaxCardinality(cardinality, property_, filler)
+        else:
+            return OWLObjectExactCardinality(cardinality, property_, filler)
+
+    def visit_value_res(self, node, children) -> OWLObjectHasValue:
+        _, _, property_, _, _, individual, _ = children
+        return OWLObjectHasValue(property_, individual)
+
+    def visit_has_self(self, node, children) -> OWLObjectHasSelf:
+        _, _, property_, _, _ = children
+        return OWLObjectHasSelf(property_)
+
+    def visit_object_property(self, node, children) -> OWLObjectPropertyExpression:
+        property_, inverse = children
+        return property_.get_inverse_property() if isinstance(inverse, list) else property_
+
+    def visit_class_expression(self, node, children) -> OWLClassExpression:
+        return children[0]
+
+    @_transform_children
+    def visit_individual_list(self, node, children) -> OWLObjectOneOf:
+        return OWLObjectOneOf(children)
+
+    def visit_data_primary(self, node, children) -> OWLDataRange:
+        match_not, expr = children
+        return OWLDataComplementOf(expr[0]) if isinstance(match_not, list) else expr[0]
+
+    def visit_data_some_only_res(self, node, children) -> OWLQuantifiedDataRestriction:
+        type_, _, property_, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _DL_SYNTAX.EXISTS:
+            return OWLDataSomeValuesFrom(property_, filler)
+        else:
+            return OWLDataAllValuesFrom(property_, filler)
+
+    def visit_data_cardinality_res(self, node, children) -> OWLDataCardinalityRestriction:
+        type_, _, cardinality, _, property_, _, filler = children
+        type_ = _node_text(*type_)
+        if type_ == _DL_SYNTAX.MIN:
+            return OWLDataMinCardinality(cardinality, property_, filler)
+        elif type_ == _DL_SYNTAX.MAX:
+            return OWLDataMaxCardinality(cardinality, property_, filler)
+        else:
+            return OWLDataExactCardinality(cardinality, property_, filler)
+
+    def visit_data_value_res(self, node, children) -> OWLDataHasValue:
+        _, _, property_, _, _, literal, _ = children
+        return OWLDataHasValue(property_, literal)
+
+    @_transform_children
+    def visit_data_union(self, node, children) -> OWLDataRange:
+        return children if isinstance(children, OWLDataRange) else OWLDataUnionOf(children)
+
+    @_transform_children
+    def visit_data_intersection(self, node, children) -> OWLDataRange:
+        return children if isinstance(children, OWLDataRange) else OWLDataIntersectionOf(children)
+
+    @_transform_children
+    def visit_literal_list(self, node, children) -> OWLDataOneOf:
+        return OWLDataOneOf(children)
+
+    def visit_data_parentheses(self, node, children) -> OWLDataRange:
+        *_, expr, _, _ = children
+        return expr
+
+    def visit_datatype_restriction(self, node, children) -> OWLDatatypeRestriction:
+        datatype, *_, facet_restrictions, _, _ = children
+        if isinstance(facet_restrictions, OWLFacetRestriction):
+            facet_restrictions = facet_restrictions,
+        not_valid_literals = []
+        if datatype != StringOWLDatatype:
+            not_valid_literals = [res.get_facet_value() for res in facet_restrictions
+                                  if res.get_facet_value().get_datatype() != datatype]
+        not_valid_facets = [res.get_facet() for res in facet_restrictions
+                            if res.get_facet() not in _DATATYPE_TO_FACETS[datatype]]
+
+        if not_valid_literals or not_valid_facets:
+            raise ValueError(f"Literals: {not_valid_literals} and Facets: {not_valid_facets}"
+                             f" not valid for datatype: {datatype}")
+        return OWLDatatypeRestriction(datatype, facet_restrictions)
+
+    @_transform_children
+    def visit_facet_restrictions(self, node, children) -> List[OWLFacetRestriction]:
+        return children
+
+    def visit_facet_restriction(self, node, children) -> OWLFacetRestriction:
+        facet, _, literal = children
+        if literal.get_datatype() not in _FACET_TO_LITERAL_DATATYPE[facet]:
+            raise ValueError(f"Literal: {literal} not valid for facet: {facet}")
+        return OWLFacetRestriction(facet, literal)
+
+    def visit_literal(self, node, children) -> OWLLiteral:
+        return children[0]
+
+    def visit_typed_literal(self, node, children) -> OWLLiteral:
+        value, _, datatype = children
+        return OWLLiteral(value[1:-1], datatype)
+
+    def visit_string_literal_language(self, node, children):
+        raise NotImplementedError(f"Language tags and plain literals not supported in owlapy yet: {_node_text(node)}")
+
+    def visit_string_literal_no_language(self, node, children) -> OWLLiteral:
+        value = children[0]
+        return OWLLiteral(value[1:-1], StringOWLDatatype)
+
+    def visit_quoted_string(self, node, children) -> str:
+        return _node_text(node)
+
+    def visit_float_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node)[:-1], DoubleOWLDatatype)
+
+    def visit_decimal_literal(self, node, children) -> OWLLiteral:
+        # TODO: Just use float for now, decimal not supported in owlapy yet
+        return OWLLiteral(_node_text(node), DoubleOWLDatatype)
+
+    def visit_integer_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), IntegerOWLDatatype)
+
+    def visit_boolean_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), BooleanOWLDatatype)
+
+    def visit_datetime_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), DateTimeOWLDatatype)
+
+    def visit_duration_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), DurationOWLDatatype)
+
+    def visit_date_literal(self, node, children) -> OWLLiteral:
+        return OWLLiteral(_node_text(node), DateOWLDatatype)
+
+    def visit_non_negative_integer(self, node, children) -> int:
+        return int(_node_text(node))
+
+    def visit_datatype_iri(self, node, children) -> str:
+        return children[0][1]
+
+    def visit_datatype(self, node, children) -> OWLDatatype:
+        return _STRING_TO_DATATYPE[_node_text(node)]
+
+    def visit_facet(self, node, children) -> OWLFacet:
+        symbolic_form = _node_text(node)
+        if symbolic_form == _DL_SYNTAX.MIN:
+            symbolic_form = '>='
+        elif symbolic_form == _DL_SYNTAX.MAX:
+            symbolic_form = '<='
+        return OWLFacet.from_str(symbolic_form)
+
+    def visit_class_iri(self, node, children) -> OWLClass:
+        top_bottom = _node_text(node)
+        if top_bottom == _DL_SYNTAX.TOP:
+            return OWLClass(OWLRDFVocabulary.OWL_THING.iri)
+        elif top_bottom == _DL_SYNTAX.BOTTOM:
+            return OWLClass(OWLRDFVocabulary.OWL_NOTHING.iri)
+        else:
+            return OWLClass(children[0])
+
+    def visit_individual_iri(self, node, children) -> OWLNamedIndividual:
+        return OWLNamedIndividual(children[0])
+
+    def visit_object_property_iri(self, node, children) -> OWLObjectProperty:
+        return OWLObjectProperty(children[0])
+
+    def visit_data_property_iri(self, node, children) -> OWLDataProperty:
+        return OWLDataProperty(children[0])
+
+    def visit_iri(self, node, children) -> IRI:
+        return children[0]
+
+    def visit_full_iri(self, node, children) -> IRI:
+        try:
+            iri = _node_text(node)[1:-1]
+            return IRI.create(iri)
+        except IndexError:
+            raise ValueError(f"{_node_text(node)[1:-1]} is not a valid IRI.")
+
+    def visit_abbreviated_iri(self, node, children):
+        # TODO: Add support for prefixes
+        raise NotImplementedError(f"Parsing of prefixes is not supported yet: {_node_text(node)}")
+
+    def visit_simple_iri(self, node, children) -> IRI:
+        simple_iri = _node_text(node)
+        if self.ns is not None:
+            return IRI(self.ns, simple_iri)
+        else:
+            raise ValueError(f"If entities are specified without a full iri ({simple_iri}), "
+                             "the namespace attribute of the parser has to be set.")
+
+    def visit_parentheses(self, node, children) -> OWLClassExpression:
+        *_, expr, _, _ = children
+        return expr
+
+    def generic_visit(self, node, children):
+        return children or node
+
+
+DLparser = DLSyntaxParser()
+ManchesterParser = ManchesterOWLSyntaxParser()
+
+
+def dl_to_owl_expression(dl_expression: str, namespace: str):
+    DLparser.ns = namespace
+    return DLparser.parse_expression(dl_expression)
+
+
+def manchester_to_owl_expression(manchester_expression: str, namespace: str):
+    ManchesterParser.ns = namespace
+    return ManchesterParser.parse_expression(manchester_expression)
```

### Comparing `owlapy-0.1.3/owlapy/render.py` & `owlapy-1.0.0/owlapy/render.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,439 +1,438 @@
-"""Renderers for different syntax."""
-# -*- coding: utf-8 -*-
-
-import types
-from functools import singledispatchmethod
-from typing import List, Callable
-
-from owlapy import namespaces
-from .owlobject import OWLObjectRenderer
-from .owl_property import OWLObjectInverseOf
-from .class_expression import OWLClassExpression, OWLBooleanClassExpression
-
-from owlapy.model import (OWLLiteral, OWLObject, OWLClass, OWLObjectSomeValuesFrom, \
-    OWLObjectAllValuesFrom, OWLObjectUnionOf, OWLNaryBooleanClassExpression, \
-    OWLObjectIntersectionOf, OWLObjectComplementOf, OWLRestriction, \
-    OWLObjectMinCardinality, OWLObjectExactCardinality, OWLObjectMaxCardinality, OWLObjectHasSelf,
-                          OWLNamedIndividual, OWLEntity, IRI, OWLPropertyExpression, OWLDataSomeValuesFrom, \
-    OWLDatatype, OWLDataAllValuesFrom, \
-    OWLDataHasValue, OWLDataOneOf, OWLDataMaxCardinality, \
-    OWLDataMinCardinality, OWLDataExactCardinality)
-from owlapy.vocab import OWLFacet
-
-from .data_ranges import OWLNaryDataRange, OWLDataComplementOf, OWLDataUnionOf, OWLDataIntersectionOf
-from .class_expression import OWLObjectHasValue, OWLFacetRestriction, OWLDatatypeRestriction, OWLObjectOneOf
-
-_DL_SYNTAX = types.SimpleNamespace(
-    SUBCLASS="⊑",
-    EQUIVALENT_TO="≡",
-    NOT="¬",
-    DISJOINT_WITH="⊑" + " " + "¬",
-    EXISTS="∃",
-    FORALL="∀",
-    IN="∈",
-    MIN="≥",
-    EQUAL="=",
-    NOT_EQUAL="≠",
-    MAX="≤",
-    INVERSE="⁻",
-    AND="⊓",
-    TOP="⊤",
-    BOTTOM="⊥",
-    OR="⊔",
-    COMP="∘",
-    WEDGE="⋀",
-    IMPLIES="←",
-    COMMA=",",
-    SELF="Self",
-)
-
-
-def _simple_short_form_provider(e: OWLEntity) -> str:
-    iri: IRI = e.get_iri()
-    sf = iri.get_short_form()
-    for ns in [namespaces.XSD, namespaces.OWL, namespaces.RDFS, namespaces.RDF]:
-        if iri.get_namespace() == ns:
-            return "%s:%s" % (ns.prefix, sf)
-    else:
-        return sf
-
-
-class DLSyntaxObjectRenderer(OWLObjectRenderer):
-    """DL Syntax renderer for OWL Objects."""
-    __slots__ = '_sfp'
-
-    _sfp: Callable[[OWLEntity], str]
-
-    def __init__(self, short_form_provider: Callable[[OWLEntity], str] = _simple_short_form_provider):
-        """Create a new DL Syntax renderer.
-
-        Args:
-            short_form_provider: Custom short form provider.
-        """
-        self._sfp = short_form_provider
-
-    def set_short_form_provider(self, short_form_provider: Callable[[OWLEntity], str]) -> None:
-        self._sfp = short_form_provider
-
-    @singledispatchmethod
-    def render(self, o: OWLObject) -> str:
-        assert isinstance(o, OWLObject), f"Tried to render non-OWLObject {o} of {type(o)}"
-        raise NotImplementedError
-
-    @render.register
-    def _(self, o: OWLClass) -> str:
-        if o.is_owl_nothing():
-            return _DL_SYNTAX.BOTTOM
-        elif o.is_owl_thing():
-            return _DL_SYNTAX.TOP
-        else:
-            return self._sfp(o)
-
-    @render.register
-    def _(self, p: OWLPropertyExpression) -> str:
-        return self._sfp(p)
-
-    @render.register
-    def _(self, i: OWLNamedIndividual) -> str:
-        return self._sfp(i)
-
-    @render.register
-    def _(self, e: OWLObjectSomeValuesFrom) -> str:
-        return "%s %s.%s" % (_DL_SYNTAX.EXISTS, self.render(e.get_property()), self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, e: OWLObjectAllValuesFrom) -> str:
-        return "%s %s.%s" % (_DL_SYNTAX.FORALL, self.render(e.get_property()), self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, c: OWLObjectUnionOf) -> str:
-        return (" %s " % _DL_SYNTAX.OR).join(self._render_operands(c))
-
-    @render.register
-    def _(self, c: OWLObjectIntersectionOf) -> str:
-        return (" %s " % _DL_SYNTAX.AND).join(self._render_operands(c))
-
-    @render.register
-    def _(self, n: OWLObjectComplementOf) -> str:
-        return "%s%s" % (_DL_SYNTAX.NOT, self._render_nested(n.get_operand()))
-
-    @render.register
-    def _(self, p: OWLObjectInverseOf) -> str:
-        return "%s%s" % (self.render(p.get_named_property()), _DL_SYNTAX.INVERSE)
-
-    @render.register
-    def _(self, r: OWLObjectMinCardinality) -> str:
-        return "%s %s %s.%s" % (
-            _DL_SYNTAX.MIN, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectExactCardinality) -> str:
-        return "%s %s %s.%s" % (
-            _DL_SYNTAX.EQUAL, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectMaxCardinality) -> str:
-        return "%s %s %s.%s" % (
-            _DL_SYNTAX.MAX, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectHasSelf) -> str:
-        return "%s %s.%s" % (_DL_SYNTAX.EXISTS, self.render(r.get_property()), _DL_SYNTAX.SELF)
-
-    @render.register
-    def _(self, r: OWLObjectHasValue):
-        return "%s %s.{%s}" % (_DL_SYNTAX.EXISTS, self.render(r.get_property()),
-                               self.render(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectOneOf):
-        return "{%s}" % (" %s " % _DL_SYNTAX.COMMA).join(
-            "%s" % (self.render(_)) for _ in r.individuals())
-
-    @render.register
-    def _(self, e: OWLDataSomeValuesFrom) -> str:
-        return "%s %s.%s" % (_DL_SYNTAX.EXISTS, self.render(e.get_property()), self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, e: OWLDataAllValuesFrom) -> str:
-        return "%s %s.%s" % (_DL_SYNTAX.FORALL, self.render(e.get_property()), self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, r: OWLFacetRestriction) -> str:
-        symbolic_form = r.get_facet().symbolic_form
-        if r.get_facet() == OWLFacet.MIN_INCLUSIVE:
-            symbolic_form = _DL_SYNTAX.MIN
-        elif r.get_facet() == OWLFacet.MAX_INCLUSIVE:
-            symbolic_form = _DL_SYNTAX.MAX
-        return "%s %s" % (symbolic_form, r.get_facet_value().get_literal())
-
-    @render.register
-    def _(self, r: OWLDatatypeRestriction) -> str:
-        s = [self.render(_) for _ in r.get_facet_restrictions()]
-        return "%s[%s]" % (self.render(r.get_datatype()), (" %s " % _DL_SYNTAX.COMMA).join(s))
-
-    @render.register
-    def _(self, r: OWLDataHasValue):
-        return "%s %s.{%s}" % (_DL_SYNTAX.EXISTS, self.render(r.get_property()),
-                               self.render(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataMinCardinality) -> str:
-        return "%s %s %s.%s" % (
-            _DL_SYNTAX.MIN, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataExactCardinality) -> str:
-        return "%s %s %s.%s" % (
-            _DL_SYNTAX.EQUAL, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataMaxCardinality) -> str:
-        return "%s %s %s.%s" % (
-            _DL_SYNTAX.MAX, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataOneOf):
-        return "{%s}" % (" %s " % _DL_SYNTAX.OR).join(
-            "%s" % (self.render(_)) for _ in r.values())
-
-    # TODO
-    # @render.register
-    # def _(self, r: OWLObjectPropertyChain):
-    #     return (" %s " % _DL_SYNTAX.COMP).join(self.render(_) for _ in r.property_chain())
-
-    @render.register
-    def _(self, n: OWLDataComplementOf) -> str:
-        return "%s%s" % (_DL_SYNTAX.NOT, self._render_nested(n.get_data_range()))
-
-    @render.register
-    def _(self, c: OWLDataUnionOf) -> str:
-        return (" %s " % _DL_SYNTAX.OR).join(self._render_operands(c))
-
-    @render.register
-    def _(self, c: OWLDataIntersectionOf) -> str:
-        return (" %s " % _DL_SYNTAX.AND).join(self._render_operands(c))
-
-    @render.register
-    def _(self, t: OWLDatatype) -> str:
-        return self._sfp(t)
-
-    @render.register
-    def _(self, t: OWLLiteral) -> str:
-        return t.get_literal()
-
-    def _render_operands(self, c: OWLNaryBooleanClassExpression) -> List[str]:
-        return [self._render_nested(_) for _ in c.operands()]
-
-    def _render_nested(self, c: OWLClassExpression) -> str:
-        if isinstance(c, OWLBooleanClassExpression) or isinstance(c, OWLRestriction) \
-                                                    or isinstance(c, OWLNaryDataRange):
-            return "(%s)" % self.render(c)
-        else:
-            return self.render(c)
-
-
-_MAN_SYNTAX = types.SimpleNamespace(
-    SUBCLASS="SubClassOf",
-    EQUIVALENT_TO="EquivalentTo",
-    NOT="not",
-    DISJOINT_WITH="DisjointWith",
-    EXISTS="some",
-    FORALL="only",
-    MIN="min",
-    EQUAL="exactly",
-    MAX="max",
-    AND="and",
-    TOP="Thing",
-    BOTTOM="Nothing",
-    OR="or",
-    INVERSE="inverse",
-    COMMA=",",
-    SELF="Self",
-    VALUE="value",
-)
-
-
-class ManchesterOWLSyntaxOWLObjectRenderer(OWLObjectRenderer):
-    """Manchester Syntax renderer for OWL Objects"""
-    __slots__ = '_sfp', '_no_render_thing'
-
-    _sfp: Callable[[OWLEntity], str]
-
-    def __init__(self, short_form_provider: Callable[[OWLEntity], str] = _simple_short_form_provider,
-                 no_render_thing=False):
-        """Create a new Manchester Syntax renderer
-
-        Args:
-            short_form_provider: custom short form provider
-            no_render_thing: disable manchester rendering for Thing and Nothing
-        """
-        self._sfp = short_form_provider
-        self._no_render_thing = no_render_thing
-
-    def set_short_form_provider(self, short_form_provider: Callable[[OWLEntity], str]) -> None:
-        self._sfp = short_form_provider
-
-    @singledispatchmethod
-    def render(self, o: OWLObject) -> str:
-        assert isinstance(o, OWLObject), f"Tried to render non-OWLObject {o} of {type(o)}"
-        raise NotImplementedError
-
-    @render.register
-    def _(self, o: OWLClass) -> str:
-        if not self._no_render_thing:
-            if o.is_owl_nothing():
-                return _MAN_SYNTAX.BOTTOM
-            if o.is_owl_thing():
-                return _MAN_SYNTAX.TOP
-        return self._sfp(o)
-
-    @render.register
-    def _(self, p: OWLPropertyExpression) -> str:
-        return self._sfp(p)
-
-    @render.register
-    def _(self, i: OWLNamedIndividual) -> str:
-        return self._sfp(i)
-
-    @render.register
-    def _(self, e: OWLObjectSomeValuesFrom) -> str:
-        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.EXISTS, self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, e: OWLObjectAllValuesFrom) -> str:
-        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.FORALL, self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, c: OWLObjectUnionOf) -> str:
-        return (" %s " % _MAN_SYNTAX.OR).join(self._render_operands(c))
-
-    @render.register
-    def _(self, c: OWLObjectIntersectionOf) -> str:
-        return (" %s " % _MAN_SYNTAX.AND).join(self._render_operands(c))
-
-    @render.register
-    def _(self, n: OWLObjectComplementOf) -> str:
-        return "%s %s" % (_MAN_SYNTAX.NOT, self._render_nested(n.get_operand()))
-
-    @render.register
-    def _(self, p: OWLObjectInverseOf) -> str:
-        return "%s %s" % (_MAN_SYNTAX.INVERSE, self.render(p.get_named_property()))
-
-    @render.register
-    def _(self, r: OWLObjectMinCardinality) -> str:
-        return "%s %s %s %s" % (
-            self.render(r.get_property()), _MAN_SYNTAX.MIN, r.get_cardinality(), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectExactCardinality) -> str:
-        return "%s %s %s %s" % (
-            self.render(r.get_property()), _MAN_SYNTAX.EQUAL, r.get_cardinality(), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectMaxCardinality) -> str:
-        return "%s %s %s %s" % (
-            self.render(r.get_property()), _MAN_SYNTAX.MAX, r.get_cardinality(), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectHasSelf) -> str:
-        return "%s %s" % (self.render(r.get_property()), _MAN_SYNTAX.SELF)
-
-    @render.register
-    def _(self, r: OWLObjectHasValue):
-        return "%s %s %s" % (self.render(r.get_property()), _MAN_SYNTAX.VALUE,
-                             self.render(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLObjectOneOf):
-        return "{%s}" % (" %s " % _MAN_SYNTAX.COMMA).join(
-            "%s" % (self.render(_)) for _ in r.individuals())
-
-    @render.register
-    def _(self, e: OWLDataSomeValuesFrom) -> str:
-        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.EXISTS, self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, e: OWLDataAllValuesFrom) -> str:
-        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.FORALL, self._render_nested(e.get_filler()))
-
-    @render.register
-    def _(self, r: OWLFacetRestriction):
-        return "%s %s" % (r.get_facet().symbolic_form, r.get_facet_value().get_literal())
-
-    @render.register
-    def _(self, r: OWLDatatypeRestriction):
-        s = [self.render(_) for _ in r.get_facet_restrictions()]
-        return "%s[%s]" % (self.render(r.get_datatype()), (" %s " % _MAN_SYNTAX.COMMA).join(s))
-
-    @render.register
-    def _(self, r: OWLDataHasValue):
-        return "%s %s %s" % (self.render(r.get_property()), _MAN_SYNTAX.VALUE,
-                             self.render(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataMinCardinality) -> str:
-        return "%s %s %s %s" % (
-            self.render(r.get_property()), _MAN_SYNTAX.MIN, r.get_cardinality(), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataExactCardinality) -> str:
-        return "%s %s %s %s" % (
-            self.render(r.get_property()), _MAN_SYNTAX.EQUAL, r.get_cardinality(), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataMaxCardinality) -> str:
-        return "%s %s %s %s" % (
-            self.render(r.get_property()), _MAN_SYNTAX.MAX, r.get_cardinality(), self._render_nested(r.get_filler()))
-
-    @render.register
-    def _(self, r: OWLDataOneOf):
-        return "{%s}" % (" %s " % _MAN_SYNTAX.COMMA).join(
-            "%s" % (self.render(_)) for _ in r.values())
-
-    # TODO
-    # @render.register
-    # def _(self, r: OWLObjectPropertyChain):
-    #     return (" %s " % _MAN_SYNTAX.COMP).join(self.render(_) for _ in r.property_chain())
-
-    @render.register
-    def _(self, n: OWLDataComplementOf) -> str:
-        return "%s %s" % (_MAN_SYNTAX.NOT, self._render_nested(n.get_data_range()))
-
-    @render.register
-    def _(self, c: OWLDataUnionOf) -> str:
-        return (" %s " % _MAN_SYNTAX.OR).join(self._render_operands(c))
-
-    @render.register
-    def _(self, c: OWLDataIntersectionOf) -> str:
-        return (" %s " % _MAN_SYNTAX.AND).join(self._render_operands(c))
-
-    @render.register
-    def _(self, t: OWLDatatype):
-        return self._sfp(t)
-
-    @render.register
-    def _(self, t: OWLLiteral) -> str:
-        return t.get_literal()
-
-    def _render_operands(self, c: OWLNaryBooleanClassExpression) -> List[str]:
-        return [self._render_nested(_) for _ in c.operands()]
-
-    def _render_nested(self, c: OWLClassExpression) -> str:
-        if isinstance(c, OWLBooleanClassExpression) or isinstance(c, OWLRestriction) \
-                                                    or isinstance(c, OWLNaryDataRange):
-            return "(%s)" % self.render(c)
-        else:
-            return self.render(c)
-
-
-DLrenderer = DLSyntaxObjectRenderer()
-ManchesterRenderer = ManchesterOWLSyntaxOWLObjectRenderer()
-
-
-def owl_expression_to_dl(o: OWLObject) -> str:
-    return DLrenderer.render(o)
-
-
-def owl_expression_to_manchester(o: OWLObject) -> str:
-    return ManchesterRenderer.render(o)
+"""Renderers for different syntax."""
+# -*- coding: utf-8 -*-
+
+import types
+from functools import singledispatchmethod
+from typing import List, Callable
+
+from owlapy import namespaces
+from .iri import IRI
+from .owl_individual import OWLNamedIndividual
+from .owl_literal import OWLLiteral
+from .owl_object import OWLObjectRenderer, OWLEntity, OWLObject
+from .owl_property import OWLObjectInverseOf, OWLPropertyExpression
+from .class_expression import OWLClassExpression, OWLBooleanClassExpression, OWLClass, OWLObjectSomeValuesFrom, \
+    OWLObjectAllValuesFrom, OWLObjectUnionOf, OWLObjectIntersectionOf, OWLObjectComplementOf, OWLObjectMinCardinality, \
+    OWLObjectExactCardinality, OWLObjectMaxCardinality, OWLObjectHasSelf, OWLDataSomeValuesFrom, OWLDataAllValuesFrom, \
+    OWLDataHasValue, OWLDataMinCardinality, OWLDataExactCardinality, OWLDataMaxCardinality, OWLDataOneOf, \
+    OWLNaryBooleanClassExpression, OWLRestriction
+from owlapy.vocab import OWLFacet
+from .owl_data_ranges import OWLNaryDataRange, OWLDataComplementOf, OWLDataUnionOf, OWLDataIntersectionOf
+from .class_expression import OWLObjectHasValue, OWLFacetRestriction, OWLDatatypeRestriction, OWLObjectOneOf
+from .owl_datatype import OWLDatatype
+
+
+_DL_SYNTAX = types.SimpleNamespace(
+    SUBCLASS="⊑",
+    EQUIVALENT_TO="≡",
+    NOT="¬",
+    DISJOINT_WITH="⊑" + " " + "¬",
+    EXISTS="∃",
+    FORALL="∀",
+    IN="∈",
+    MIN="≥",
+    EQUAL="=",
+    NOT_EQUAL="≠",
+    MAX="≤",
+    INVERSE="⁻",
+    AND="⊓",
+    TOP="⊤",
+    BOTTOM="⊥",
+    OR="⊔",
+    COMP="∘",
+    WEDGE="⋀",
+    IMPLIES="←",
+    COMMA=",",
+    SELF="Self",
+)
+
+
+def _simple_short_form_provider(e: OWLEntity) -> str:
+    iri: IRI = e.iri
+    sf = iri.get_short_form()
+    for ns in [namespaces.XSD, namespaces.OWL, namespaces.RDFS, namespaces.RDF]:
+        if iri.get_namespace() == ns:
+            return "%s:%s" % (ns.prefix, sf)
+    else:
+        return sf
+
+
+class DLSyntaxObjectRenderer(OWLObjectRenderer):
+    """DL Syntax renderer for OWL Objects."""
+    __slots__ = '_sfp'
+
+    _sfp: Callable[[OWLEntity], str]
+
+    def __init__(self, short_form_provider: Callable[[OWLEntity], str] = _simple_short_form_provider):
+        """Create a new DL Syntax renderer.
+
+        Args:
+            short_form_provider: Custom short form provider.
+        """
+        self._sfp = short_form_provider
+
+    def set_short_form_provider(self, short_form_provider: Callable[[OWLEntity], str]) -> None:
+        self._sfp = short_form_provider
+
+    @singledispatchmethod
+    def render(self, o: OWLObject) -> str:
+        assert isinstance(o, OWLObject), f"Tried to render non-OWLObject {o} of {type(o)}"
+        raise NotImplementedError
+
+    @render.register
+    def _(self, o: OWLClass) -> str:
+        if o.is_owl_nothing():
+            return _DL_SYNTAX.BOTTOM
+        elif o.is_owl_thing():
+            return _DL_SYNTAX.TOP
+        else:
+            return self._sfp(o)
+
+    @render.register
+    def _(self, p: OWLPropertyExpression) -> str:
+        return self._sfp(p)
+
+    @render.register
+    def _(self, i: OWLNamedIndividual) -> str:
+        return self._sfp(i)
+
+    @render.register
+    def _(self, e: OWLObjectSomeValuesFrom) -> str:
+        return "%s %s.%s" % (_DL_SYNTAX.EXISTS, self.render(e.get_property()), self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, e: OWLObjectAllValuesFrom) -> str:
+        return "%s %s.%s" % (_DL_SYNTAX.FORALL, self.render(e.get_property()), self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, c: OWLObjectUnionOf) -> str:
+        return (" %s " % _DL_SYNTAX.OR).join(self._render_operands(c))
+
+    @render.register
+    def _(self, c: OWLObjectIntersectionOf) -> str:
+        return (" %s " % _DL_SYNTAX.AND).join(self._render_operands(c))
+
+    @render.register
+    def _(self, n: OWLObjectComplementOf) -> str:
+        return "%s%s" % (_DL_SYNTAX.NOT, self._render_nested(n.get_operand()))
+
+    @render.register
+    def _(self, p: OWLObjectInverseOf) -> str:
+        return "%s%s" % (self.render(p.get_named_property()), _DL_SYNTAX.INVERSE)
+
+    @render.register
+    def _(self, r: OWLObjectMinCardinality) -> str:
+        return "%s %s %s.%s" % (
+            _DL_SYNTAX.MIN, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectExactCardinality) -> str:
+        return "%s %s %s.%s" % (
+            _DL_SYNTAX.EQUAL, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectMaxCardinality) -> str:
+        return "%s %s %s.%s" % (
+            _DL_SYNTAX.MAX, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectHasSelf) -> str:
+        return "%s %s.%s" % (_DL_SYNTAX.EXISTS, self.render(r.get_property()), _DL_SYNTAX.SELF)
+
+    @render.register
+    def _(self, r: OWLObjectHasValue):
+        return "%s %s.{%s}" % (_DL_SYNTAX.EXISTS, self.render(r.get_property()),
+                               self.render(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectOneOf):
+        return "{%s}" % (" %s " % _DL_SYNTAX.COMMA).join(
+            "%s" % (self.render(_)) for _ in r.individuals())
+
+    @render.register
+    def _(self, e: OWLDataSomeValuesFrom) -> str:
+        return "%s %s.%s" % (_DL_SYNTAX.EXISTS, self.render(e.get_property()), self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, e: OWLDataAllValuesFrom) -> str:
+        return "%s %s.%s" % (_DL_SYNTAX.FORALL, self.render(e.get_property()), self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, r: OWLFacetRestriction) -> str:
+        symbolic_form = r.get_facet().symbolic_form
+        if r.get_facet() == OWLFacet.MIN_INCLUSIVE:
+            symbolic_form = _DL_SYNTAX.MIN
+        elif r.get_facet() == OWLFacet.MAX_INCLUSIVE:
+            symbolic_form = _DL_SYNTAX.MAX
+        return "%s %s" % (symbolic_form, r.get_facet_value().get_literal())
+
+    @render.register
+    def _(self, r: OWLDatatypeRestriction) -> str:
+        s = [self.render(_) for _ in r.get_facet_restrictions()]
+        return "%s[%s]" % (self.render(r.get_datatype()), (" %s " % _DL_SYNTAX.COMMA).join(s))
+
+    @render.register
+    def _(self, r: OWLDataHasValue):
+        return "%s %s.{%s}" % (_DL_SYNTAX.EXISTS, self.render(r.get_property()),
+                               self.render(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataMinCardinality) -> str:
+        return "%s %s %s.%s" % (
+            _DL_SYNTAX.MIN, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataExactCardinality) -> str:
+        return "%s %s %s.%s" % (
+            _DL_SYNTAX.EQUAL, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataMaxCardinality) -> str:
+        return "%s %s %s.%s" % (
+            _DL_SYNTAX.MAX, r.get_cardinality(), self.render(r.get_property()), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataOneOf):
+        return "{%s}" % (" %s " % _DL_SYNTAX.OR).join(
+            "%s" % (self.render(_)) for _ in r.values())
+
+    # TODO
+    # @render.register
+    # def _(self, r: OWLObjectPropertyChain):
+    #     return (" %s " % _DL_SYNTAX.COMP).join(self.render(_) for _ in r.property_chain())
+
+    @render.register
+    def _(self, n: OWLDataComplementOf) -> str:
+        return "%s%s" % (_DL_SYNTAX.NOT, self._render_nested(n.get_data_range()))
+
+    @render.register
+    def _(self, c: OWLDataUnionOf) -> str:
+        return (" %s " % _DL_SYNTAX.OR).join(self._render_operands(c))
+
+    @render.register
+    def _(self, c: OWLDataIntersectionOf) -> str:
+        return (" %s " % _DL_SYNTAX.AND).join(self._render_operands(c))
+
+    @render.register
+    def _(self, t: OWLDatatype) -> str:
+        return self._sfp(t)
+
+    @render.register
+    def _(self, t: OWLLiteral) -> str:
+        return t.get_literal()
+
+    def _render_operands(self, c: OWLNaryBooleanClassExpression) -> List[str]:
+        return [self._render_nested(_) for _ in c.operands()]
+
+    def _render_nested(self, c: OWLClassExpression) -> str:
+        if isinstance(c, OWLBooleanClassExpression) or isinstance(c, OWLRestriction) \
+                                                    or isinstance(c, OWLNaryDataRange):
+            return "(%s)" % self.render(c)
+        else:
+            return self.render(c)
+
+
+_MAN_SYNTAX = types.SimpleNamespace(
+    SUBCLASS="SubClassOf",
+    EQUIVALENT_TO="EquivalentTo",
+    NOT="not",
+    DISJOINT_WITH="DisjointWith",
+    EXISTS="some",
+    FORALL="only",
+    MIN="min",
+    EQUAL="exactly",
+    MAX="max",
+    AND="and",
+    TOP="Thing",
+    BOTTOM="Nothing",
+    OR="or",
+    INVERSE="inverse",
+    COMMA=",",
+    SELF="Self",
+    VALUE="value",
+)
+
+
+class ManchesterOWLSyntaxOWLObjectRenderer(OWLObjectRenderer):
+    """Manchester Syntax renderer for OWL Objects"""
+    __slots__ = '_sfp', '_no_render_thing'
+
+    _sfp: Callable[[OWLEntity], str]
+
+    def __init__(self, short_form_provider: Callable[[OWLEntity], str] = _simple_short_form_provider,
+                 no_render_thing=False):
+        """Create a new Manchester Syntax renderer
+
+        Args:
+            short_form_provider: custom short form provider
+            no_render_thing: disable manchester rendering for Thing and Nothing
+        """
+        self._sfp = short_form_provider
+        self._no_render_thing = no_render_thing
+
+    def set_short_form_provider(self, short_form_provider: Callable[[OWLEntity], str]) -> None:
+        self._sfp = short_form_provider
+
+    @singledispatchmethod
+    def render(self, o: OWLObject) -> str:
+        assert isinstance(o, OWLObject), f"Tried to render non-OWLObject {o} of {type(o)}"
+        raise NotImplementedError
+
+    @render.register
+    def _(self, o: OWLClass) -> str:
+        if not self._no_render_thing:
+            if o.is_owl_nothing():
+                return _MAN_SYNTAX.BOTTOM
+            if o.is_owl_thing():
+                return _MAN_SYNTAX.TOP
+        return self._sfp(o)
+
+    @render.register
+    def _(self, p: OWLPropertyExpression) -> str:
+        return self._sfp(p)
+
+    @render.register
+    def _(self, i: OWLNamedIndividual) -> str:
+        return self._sfp(i)
+
+    @render.register
+    def _(self, e: OWLObjectSomeValuesFrom) -> str:
+        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.EXISTS, self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, e: OWLObjectAllValuesFrom) -> str:
+        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.FORALL, self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, c: OWLObjectUnionOf) -> str:
+        return (" %s " % _MAN_SYNTAX.OR).join(self._render_operands(c))
+
+    @render.register
+    def _(self, c: OWLObjectIntersectionOf) -> str:
+        return (" %s " % _MAN_SYNTAX.AND).join(self._render_operands(c))
+
+    @render.register
+    def _(self, n: OWLObjectComplementOf) -> str:
+        return "%s %s" % (_MAN_SYNTAX.NOT, self._render_nested(n.get_operand()))
+
+    @render.register
+    def _(self, p: OWLObjectInverseOf) -> str:
+        return "%s %s" % (_MAN_SYNTAX.INVERSE, self.render(p.get_named_property()))
+
+    @render.register
+    def _(self, r: OWLObjectMinCardinality) -> str:
+        return "%s %s %s %s" % (
+            self.render(r.get_property()), _MAN_SYNTAX.MIN, r.get_cardinality(), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectExactCardinality) -> str:
+        return "%s %s %s %s" % (
+            self.render(r.get_property()), _MAN_SYNTAX.EQUAL, r.get_cardinality(), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectMaxCardinality) -> str:
+        return "%s %s %s %s" % (
+            self.render(r.get_property()), _MAN_SYNTAX.MAX, r.get_cardinality(), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectHasSelf) -> str:
+        return "%s %s" % (self.render(r.get_property()), _MAN_SYNTAX.SELF)
+
+    @render.register
+    def _(self, r: OWLObjectHasValue):
+        return "%s %s %s" % (self.render(r.get_property()), _MAN_SYNTAX.VALUE,
+                             self.render(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLObjectOneOf):
+        return "{%s}" % (" %s " % _MAN_SYNTAX.COMMA).join(
+            "%s" % (self.render(_)) for _ in r.individuals())
+
+    @render.register
+    def _(self, e: OWLDataSomeValuesFrom) -> str:
+        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.EXISTS, self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, e: OWLDataAllValuesFrom) -> str:
+        return "%s %s %s" % (self.render(e.get_property()), _MAN_SYNTAX.FORALL, self._render_nested(e.get_filler()))
+
+    @render.register
+    def _(self, r: OWLFacetRestriction):
+        return "%s %s" % (r.get_facet().symbolic_form, r.get_facet_value().get_literal())
+
+    @render.register
+    def _(self, r: OWLDatatypeRestriction):
+        s = [self.render(_) for _ in r.get_facet_restrictions()]
+        return "%s[%s]" % (self.render(r.get_datatype()), (" %s " % _MAN_SYNTAX.COMMA).join(s))
+
+    @render.register
+    def _(self, r: OWLDataHasValue):
+        return "%s %s %s" % (self.render(r.get_property()), _MAN_SYNTAX.VALUE,
+                             self.render(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataMinCardinality) -> str:
+        return "%s %s %s %s" % (
+            self.render(r.get_property()), _MAN_SYNTAX.MIN, r.get_cardinality(), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataExactCardinality) -> str:
+        return "%s %s %s %s" % (
+            self.render(r.get_property()), _MAN_SYNTAX.EQUAL, r.get_cardinality(), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataMaxCardinality) -> str:
+        return "%s %s %s %s" % (
+            self.render(r.get_property()), _MAN_SYNTAX.MAX, r.get_cardinality(), self._render_nested(r.get_filler()))
+
+    @render.register
+    def _(self, r: OWLDataOneOf):
+        return "{%s}" % (" %s " % _MAN_SYNTAX.COMMA).join(
+            "%s" % (self.render(_)) for _ in r.values())
+
+    # TODO
+    # @render.register
+    # def _(self, r: OWLObjectPropertyChain):
+    #     return (" %s " % _MAN_SYNTAX.COMP).join(self.render(_) for _ in r.property_chain())
+
+    @render.register
+    def _(self, n: OWLDataComplementOf) -> str:
+        return "%s %s" % (_MAN_SYNTAX.NOT, self._render_nested(n.get_data_range()))
+
+    @render.register
+    def _(self, c: OWLDataUnionOf) -> str:
+        return (" %s " % _MAN_SYNTAX.OR).join(self._render_operands(c))
+
+    @render.register
+    def _(self, c: OWLDataIntersectionOf) -> str:
+        return (" %s " % _MAN_SYNTAX.AND).join(self._render_operands(c))
+
+    @render.register
+    def _(self, t: OWLDatatype):
+        return self._sfp(t)
+
+    @render.register
+    def _(self, t: OWLLiteral) -> str:
+        return t.get_literal()
+
+    def _render_operands(self, c: OWLNaryBooleanClassExpression) -> List[str]:
+        return [self._render_nested(_) for _ in c.operands()]
+
+    def _render_nested(self, c: OWLClassExpression) -> str:
+        if isinstance(c, OWLBooleanClassExpression) or isinstance(c, OWLRestriction) \
+                                                    or isinstance(c, OWLNaryDataRange):
+            return "(%s)" % self.render(c)
+        else:
+            return self.render(c)
+
+
+DLrenderer = DLSyntaxObjectRenderer()
+ManchesterRenderer = ManchesterOWLSyntaxOWLObjectRenderer()
+
+
+def owl_expression_to_dl(o: OWLObject) -> str:
+    return DLrenderer.render(o)
+
+
+def owl_expression_to_manchester(o: OWLObject) -> str:
+    return ManchesterRenderer.render(o)
```

### Comparing `owlapy-0.1.3/owlapy/util.py` & `owlapy-1.0.0/owlapy/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,528 +1,555 @@
-"""Owlapy utils."""
-from functools import singledispatchmethod, total_ordering
-from typing import Iterable, List, Type, TypeVar, Generic, Tuple, cast, Optional, Union, overload
-from .has import HasIndex
-from .owl_property import OWLObjectInverseOf
-from owlapy.model import HasIRI, OWLClassExpression, OWLClass, OWLObjectCardinalityRestriction, \
-    OWLObjectComplementOf, OWLNothing, OWLPropertyRange, OWLRestriction, OWLThing, OWLObjectSomeValuesFrom, \
-    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, OWLObjectHasSelf, \
-    OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataExactCardinality, OWLDataHasValue, \
-    OWLDataAllValuesFrom, OWLDataSomeValuesFrom, OWLObjectAllValuesFrom, HasFiller, HasCardinality, HasOperands, \
-    OWLDatatype,OWLDataOneOf, OWLLiteral, OWLObjectIntersectionOf, \
-    OWLDataCardinalityRestriction, OWLNaryBooleanClassExpression, OWLObjectUnionOf, \
-    OWLDataRange, OWLObject
-from .data_ranges import OWLDataComplementOf, OWLDataUnionOf, OWLDataIntersectionOf, OWLNaryDataRange
-from .class_expression import OWLObjectHasValue, OWLDatatypeRestriction, OWLFacetRestriction, OWLObjectOneOf
-
-_HasIRI = TypeVar('_HasIRI', bound=HasIRI)  #:
-_HasIndex = TypeVar('_HasIndex', bound=HasIndex)  #:
-_O = TypeVar('_O')  #:
-_Enc = TypeVar('_Enc')
-_Con = TypeVar('_Con')
-_K = TypeVar('_K')
-_V = TypeVar('_V')
-
-
-@total_ordering
-class OrderedOWLObject:
-    """Holder of OWL Objects that can be used for Python sorted.
-
-    The Ordering is dependent on the type_index of the impl. classes recursively followed by all components of the
-    OWL Object.
-
-    Attributes:
-        o: OWL object.
-    """
-    __slots__ = 'o', '_chain'
-
-    o: _HasIndex  # o: Intersection[OWLObject, HasIndex]
-    _chain: Optional[Tuple]
-
-    # we are limited by https://github.com/python/typing/issues/213 # o: Intersection[OWLObject, HasIndex]
-    def __init__(self, o: _HasIndex):
-        """OWL Object holder with a defined sort order.
-
-        Args:
-            o: OWL Object.
-        """
-        self.o = o
-        self._chain = None
-
-    def _comparison_chain(self):
-        if self._chain is None:
-            c = [self.o.type_index]
-
-            if isinstance(self.o, OWLRestriction):
-                c.append(OrderedOWLObject(as_index(self.o.get_property())))
-            if isinstance(self.o, OWLObjectInverseOf):
-                c.append(self.o.get_named_property().get_iri().as_str())
-            if isinstance(self.o, HasFiller):
-                c.append(OrderedOWLObject(self.o.get_filler()))
-            if isinstance(self.o, HasCardinality):
-                c.append(self.o.get_cardinality())
-            if isinstance(self.o, HasOperands):
-                c.append(tuple(map(OrderedOWLObject, self.o.operands())))
-            if isinstance(self.o, HasIRI):
-                c.append(self.o.get_iri().as_str())
-            if isinstance(self.o, OWLDataComplementOf):
-                c.append(OrderedOWLObject(self.o.get_data_range()))
-            if isinstance(self.o, OWLDatatypeRestriction):
-                c.append((OrderedOWLObject(self.o.get_datatype()),
-                          tuple(map(OrderedOWLObject, self.o.get_facet_restrictions()))))
-            if isinstance(self.o, OWLFacetRestriction):
-                c.append((self.o.get_facet().get_iri().as_str(), self.o.get_facet_value().get_literal()))
-            if isinstance(self.o, OWLLiteral):
-                c.append(self.o.get_literal())
-            if len(c) == 1:
-                raise NotImplementedError(type(self.o))
-
-            self._chain = tuple(c)
-
-        return self._chain
-
-    def __lt__(self, other):
-        if self.o.type_index < other.o.type_index:
-            return True
-        elif self.o.type_index > other.o.type_index:
-            return False
-        else:
-            return self._comparison_chain() < other._comparison_chain()
-
-    def __eq__(self, other):
-        return self.o == other.o
-
-
-def _sort_by_ordered_owl_object(i: Iterable[_O]) -> Iterable[_O]:
-    return sorted(i, key=OrderedOWLObject)
-
-
-class NNF:
-    """This class contains functions to transform a Class Expression into Negation Normal Form."""
-    @singledispatchmethod
-    def get_class_nnf(self, ce: OWLClassExpression, negated: bool = False) -> OWLClassExpression:
-        """Convert a Class Expression to Negation Normal Form. Operands will be sorted.
-
-        Args:
-            ce: Class Expression.
-            negated: Whether the result should be negated.
-
-        Returns:
-            Class Expression in Negation Normal Form.
-            """
-        raise NotImplementedError
-
-    @get_class_nnf.register
-    def _(self, ce: OWLClass, negated: bool = False):
-        if negated:
-            if ce.is_owl_thing():
-                return OWLNothing
-            if ce.is_owl_nothing():
-                return OWLThing
-            return OWLObjectComplementOf(ce)
-        return ce
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectIntersectionOf, negated: bool = False):
-        ops = map(lambda _: self.get_class_nnf(_, negated),
-                  _sort_by_ordered_owl_object(ce.operands()))
-        if negated:
-            return OWLObjectUnionOf(ops)
-        return OWLObjectIntersectionOf(ops)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectUnionOf, negated: bool = False):
-        ops = map(lambda _: self.get_class_nnf(_, negated),
-                  _sort_by_ordered_owl_object(ce.operands()))
-        if negated:
-            return OWLObjectIntersectionOf(ops)
-        return OWLObjectUnionOf(ops)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectComplementOf, negated: bool = False):
-        return self.get_class_nnf(ce.get_operand(), not negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectSomeValuesFrom, negated: bool = False):
-        filler = self.get_class_nnf(ce.get_filler(), negated)
-        if negated:
-            return OWLObjectAllValuesFrom(ce.get_property(), filler)
-        return OWLObjectSomeValuesFrom(ce.get_property(), filler)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectAllValuesFrom, negated: bool = False):
-        filler = self.get_class_nnf(ce.get_filler(), negated)
-        if negated:
-            return OWLObjectSomeValuesFrom(ce.get_property(), filler)
-        return OWLObjectAllValuesFrom(ce.get_property(), filler)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectHasValue, negated: bool = False):
-        return self.get_class_nnf(ce.as_some_values_from(), negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectMinCardinality, negated: bool = False):
-        card = ce.get_cardinality()
-        if negated:
-            card = max(0, card - 1)
-        filler = self.get_class_nnf(ce.get_filler(), negated=False)
-        if negated:
-            return OWLObjectMaxCardinality(card, ce.get_property(), filler)
-        return OWLObjectMinCardinality(card, ce.get_property(), filler)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectExactCardinality, negated: bool = False):
-        return self.get_class_nnf(ce.as_intersection_of_min_max(), negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectMaxCardinality, negated: bool = False):
-        card = ce.get_cardinality()
-        if negated:
-            card = card + 1
-        filler = self.get_class_nnf(ce.get_filler(), negated=False)
-        if negated:
-            return OWLObjectMinCardinality(card, ce.get_property(), filler)
-        return OWLObjectMaxCardinality(card, ce.get_property(), filler)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectHasSelf, negated: bool = False):
-        if negated:
-            return ce.get_object_complement_of()
-        return ce
-
-    @get_class_nnf.register
-    def _(self, ce: OWLObjectOneOf, negated: bool = False):
-        union = ce.as_object_union_of()
-        if isinstance(union, OWLObjectOneOf):
-            if negated:
-                return ce.get_object_complement_of()
-            return ce
-        return self.get_class_nnf(union, negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataSomeValuesFrom, negated: bool = False):
-        filler = self.get_class_nnf(ce.get_filler(), negated)
-        if negated:
-            return OWLDataAllValuesFrom(ce.get_property(), filler)
-        return OWLDataSomeValuesFrom(ce.get_property(), filler)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataAllValuesFrom, negated: bool = False):
-        filler = self.get_class_nnf(ce.get_filler(), negated)
-        if negated:
-            return OWLDataSomeValuesFrom(ce.get_property(), filler)
-        return OWLDataAllValuesFrom(ce.get_property(), filler)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDatatypeRestriction, negated: bool = False):
-        if negated:
-            return OWLDataComplementOf(ce)
-        return ce
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDatatype, negated: bool = False):
-        if negated:
-            return OWLDataComplementOf(ce)
-        return ce
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataComplementOf, negated: bool = False):
-        return self.get_class_nnf(ce.get_data_range(), not negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataHasValue, negated: bool = False):
-        return self.get_class_nnf(ce.as_some_values_from(), negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataOneOf, negated: bool = False):
-        if len(list(ce.values())) == 1:
-            if negated:
-                return OWLDataComplementOf(ce)
-            return ce
-        union = OWLDataUnionOf([OWLDataOneOf(v) for v in ce.values()])
-        return self.get_class_nnf(union, negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataIntersectionOf, negated: bool = False):
-        ops = map(lambda _: self.get_class_nnf(_, negated),
-                  _sort_by_ordered_owl_object(ce.operands()))
-        if negated:
-            return OWLDataUnionOf(ops)
-        return OWLDataIntersectionOf(ops)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataUnionOf, negated: bool = False):
-        ops = map(lambda _: self.get_class_nnf(_, negated),
-                  _sort_by_ordered_owl_object(ce.operands()))
-        if negated:
-            return OWLDataIntersectionOf(ops)
-        return OWLDataUnionOf(ops)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataExactCardinality, negated: bool = False):
-        return self.get_class_nnf(ce.as_intersection_of_min_max(), negated)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataMinCardinality, negated: bool = False):
-        card = ce.get_cardinality()
-        if negated:
-            card = max(0, card - 1)
-        filler = self.get_class_nnf(ce.get_filler(), negated=False)
-        if negated:
-            return OWLDataMaxCardinality(card, ce.get_property(), filler)
-        return OWLDataMinCardinality(card, ce.get_property(), filler)
-
-    @get_class_nnf.register
-    def _(self, ce: OWLDataMaxCardinality, negated: bool = False):
-        card = ce.get_cardinality()
-        if negated:
-            card = card + 1
-        filler = self.get_class_nnf(ce.get_filler(), negated=False)
-        if negated:
-            return OWLDataMinCardinality(card, ce.get_property(), filler)
-        return OWLDataMaxCardinality(card, ce.get_property(), filler)
-
-
-# OWL-APy custom util start
-
-class TopLevelCNF:
-    """This class contains functions to transform a class expression into Top-Level Conjunctive Normal Form."""
-
-    def get_top_level_cnf(self, ce: OWLClassExpression) -> OWLClassExpression:
-        """Convert a class expression into Top-Level Conjunctive Normal Form. Operands will be sorted.
-
-        Args:
-            ce: Class Expression.
-
-        Returns:
-            Class Expression in Top-Level Conjunctive Normal Form.
-            """
-        c = _get_top_level_form(ce.get_nnf(), OWLObjectUnionOf, OWLObjectIntersectionOf)
-        return combine_nary_expressions(c)
-
-
-class TopLevelDNF:
-    """This class contains functions to transform a class expression into Top-Level Disjunctive Normal Form."""
-
-    def get_top_level_dnf(self, ce: OWLClassExpression) -> OWLClassExpression:
-        """Convert a class expression into Top-Level Disjunctive Normal Form. Operands will be sorted.
-
-        Args:
-            ce: Class Expression.
-
-        Returns:
-            Class Expression in Top-Level Disjunctive Normal Form.
-            """
-        c = _get_top_level_form(ce.get_nnf(), OWLObjectIntersectionOf, OWLObjectUnionOf)
-        return combine_nary_expressions(c)
-
-
-def _get_top_level_form(ce: OWLClassExpression,
-                        type_a: Type[OWLNaryBooleanClassExpression],
-                        type_b: Type[OWLNaryBooleanClassExpression]) -> OWLClassExpression:
-    """ Transforms a class expression (that's already in NNF) into Top-Level Conjunctive/Disjunctive Normal Form.
-    Here type_a specifies the operand which should be distributed inwards over type_b.
-
-    Conjunctive Normal form:
-        type_a = OWLObjectUnionOf
-        type_b = OWLObjectIntersectionOf
-    Disjunctive Normal form:
-        type_a = OWLObjectIntersectionOf
-        type_b = OWLObjectUnionOf
-    """
-
-    def distributive_law(a: OWLClassExpression, b: OWLNaryBooleanClassExpression) -> OWLNaryBooleanClassExpression:
-        return type_b(type_a([a, op]) for op in b.operands())
-
-    if isinstance(ce, type_a):
-        ce = cast(OWLNaryBooleanClassExpression, combine_nary_expressions(ce))
-        type_b_exprs = [op for op in ce.operands() if isinstance(op, type_b)]
-        non_type_b_exprs = [op for op in ce.operands() if not isinstance(op, type_b)]
-        if not len(type_b_exprs):
-            return ce
-
-        if len(non_type_b_exprs):
-            expr = non_type_b_exprs[0] if len(non_type_b_exprs) == 1 \
-                else type_a(non_type_b_exprs)
-            expr = distributive_law(expr, type_b_exprs[0])
-        else:
-            expr = type_b_exprs[0]
-
-        if len(type_b_exprs) == 1:
-            return _get_top_level_form(expr, type_a, type_b)
-
-        for type_b_expr in type_b_exprs[1:]:
-            expr = distributive_law(type_b_expr, expr)
-        return _get_top_level_form(expr, type_a, type_b)
-    elif isinstance(ce, type_b):
-        return type_b(_get_top_level_form(op, type_a, type_b) for op in ce.operands())
-    elif isinstance(ce, OWLClassExpression):
-        return ce
-    else:
-        raise ValueError('Top-Level CNF/DNF only applicable on class expressions', ce)
-
-
-@overload
-def combine_nary_expressions(ce: OWLClassExpression) -> OWLClassExpression:
-    ...
-
-
-@overload
-def combine_nary_expressions(ce: OWLDataRange) -> OWLDataRange:
-    ...
-
-
-def combine_nary_expressions(ce: OWLPropertyRange) -> OWLPropertyRange:
-    """ Shortens an OWLClassExpression or OWLDataRange by combining all nested nary expressions of the same type.
-    Operands will be sorted.
-
-    E.g. OWLObjectUnionOf(A, OWLObjectUnionOf(C, B)) -> OWLObjectUnionOf(A, B, C).
-    """
-    if isinstance(ce, (OWLNaryBooleanClassExpression, OWLNaryDataRange)):
-        expressions: List[OWLPropertyRange] = []
-        for op in ce.operands():
-            expr = combine_nary_expressions(op)
-            if type(expr) is type(ce):
-                expr = cast(Union[OWLNaryBooleanClassExpression, OWLNaryDataRange], expr)
-                expressions.extend(expr.operands())
-            else:
-                expressions.append(expr)
-        return type(ce)(_sort_by_ordered_owl_object(expressions))  # type: ignore
-    elif isinstance(ce, OWLObjectComplementOf):
-        return OWLObjectComplementOf(combine_nary_expressions(ce.get_operand()))
-    elif isinstance(ce, OWLDataComplementOf):
-        return OWLDataComplementOf(combine_nary_expressions(ce.get_data_range()))
-    elif isinstance(ce, OWLObjectCardinalityRestriction):
-        return type(ce)(ce.get_cardinality(), ce.get_property(), combine_nary_expressions(ce.get_filler()))
-    elif isinstance(ce, OWLDataCardinalityRestriction):
-        return type(ce)(ce.get_cardinality(), ce.get_property(), combine_nary_expressions(ce.get_filler()))
-    elif isinstance(ce, (OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom)):
-        return type(ce)(ce.get_property(), combine_nary_expressions(ce.get_filler()))
-    elif isinstance(ce, (OWLDataSomeValuesFrom, OWLDataAllValuesFrom)):
-        return type(ce)(ce.get_property(), combine_nary_expressions(ce.get_filler()))
-    elif isinstance(ce, OWLObjectOneOf):
-        return OWLObjectOneOf(_sort_by_ordered_owl_object(ce.operands()))
-    elif isinstance(ce, OWLDataOneOf):
-        return OWLDataOneOf(_sort_by_ordered_owl_object(ce.operands()))
-    elif isinstance(ce, OWLPropertyRange):
-        return ce
-    else:
-        raise ValueError(f'({expr}) is not an OWLObject.')
-
-
-def iter_count(i: Iterable) -> int:
-    """Count the number of elements in an iterable."""
-    return sum(1 for _ in i)
-
-
-def as_index(o: OWLObject) -> HasIndex:
-    """Cast OWL Object to HasIndex."""
-    i = cast(HasIndex, o)
-    assert type(i).type_index
-    return i
-
-
-class LRUCache(Generic[_K, _V]):
-    """Constants shares by all lru cache instances.
-
-    Adapted from functools.lru_cache.
-
-    Attributes:
-        sentinel: Unique object used to signal cache misses.
-        PREV: Name for the link field 0.
-        NEXT: Name for the link field 1.
-        KEY: Name for the link field 2.
-        RESULT: Name for the link field 3.
-    """
-
-    sentinel = object()
-    PREV, NEXT, KEY, RESULT = 0, 1, 2, 3  # names for the link fields
-
-    def __init__(self, maxsize: Optional[int] = None):
-        from _thread import RLock
-
-        self.cache = {}
-        self.hits = self.misses = 0
-        self.full = False
-        self.cache_get = self.cache.get  # bound method to lookup a key or return None
-        self.cache_len = self.cache.__len__  # get cache size without calling len()
-        self.lock = RLock()  # because linkedlist updates aren't threadsafe
-        self.root = []  # root of the circular doubly linked list
-        self.root[:] = [self.root, self.root, None, None]  # initialize by pointing to self
-        self.maxsize = maxsize
-
-    def __contains__(self, item: _K) -> bool:
-        with self.lock:
-            link = self.cache_get(item)
-            if link is not None:
-                self.hits += 1
-                return True
-            self.misses += 1
-            return False
-
-    def __getitem__(self, item: _K) -> _V:
-        with self.lock:
-            link = self.cache_get(item)
-            if link is not None:
-                # Move the link to the front of the circular queue
-                link_prev, link_next, _key, result = link
-                link_prev[LRUCache.NEXT] = link_next
-                link_next[LRUCache.PREV] = link_prev
-                last = self.root[LRUCache.PREV]
-                last[LRUCache.NEXT] = self.root[LRUCache.PREV] = link
-                link[LRUCache.PREV] = last
-                link[LRUCache.NEXT] = self.root
-                return result
-
-    def __setitem__(self, key: _K, value: _V):
-        with self.lock:
-            if key in self.cache:
-                # Getting here means that this same key was added to the
-                # cache while the lock was released.  Since the link
-                # update is already done, we need only return the
-                # computed result and update the count of misses.
-                pass
-            elif self.full:
-                # Use the old root to store the new key and result.
-                oldroot = self.root
-                oldroot[LRUCache.KEY] = key
-                oldroot[LRUCache.RESULT] = value
-                # Empty the oldest link and make it the new root.
-                # Keep a reference to the old key and old result to
-                # prevent their ref counts from going to zero during the
-                # update. That will prevent potentially arbitrary object
-                # clean-up code (i.e. __del__) from running while we're
-                # still adjusting the links.
-                self.root = oldroot[LRUCache.NEXT]
-                oldkey = self.root[LRUCache.KEY]
-                _oldresult = self.root[LRUCache.RESULT]  # noqa: F841
-                self.root[LRUCache.KEY] = self.root[LRUCache.RESULT] = None
-                # Now update the cache dictionary.
-                del self.cache[oldkey]
-                # Save the potentially reentrant cache[key] assignment
-                # for last, after the root and links have been put in
-                # a consistent state.
-                self.cache[key] = oldroot
-            else:
-                # Put result in a new link at the front of the queue.
-                last = self.root[LRUCache.PREV]
-                link = [last, self.root, key, value]
-                last[LRUCache.NEXT] = self.root[LRUCache.PREV] = self.cache[key] = link
-                # Use the cache_len bound method instead of the len() function
-                # which could potentially be wrapped in an lru_cache itself.
-                if self.maxsize is not None:
-                    self.full = (self.cache_len() >= self.maxsize)
-
-    def cache_info(self):
-        """Report cache statistics."""
-        with self.lock:
-            from collections import namedtuple
-            return namedtuple("CacheInfo", ["hits", "misses", "maxsize", "currsize"])(
-                self.hits, self.misses, self.maxsize, self.cache_len())
-
-    def cache_clear(self):
-        """Clear the cache and cache statistics."""
-        with self.lock:
-            self.cache.clear()
-            self.root[:] = [self.root, self.root, None, None]
-            self.hits = self.misses = 0
-            self.full = False
+"""Owlapy utils."""
+from functools import singledispatchmethod, total_ordering
+from typing import Iterable, List, Type, TypeVar, Generic, Tuple, cast, Optional, Union, overload, Protocol, ClassVar
+from .meta_classes import HasIRI, HasFiller, HasCardinality, HasOperands
+from .owl_literal import OWLLiteral
+from .owl_property import OWLObjectInverseOf
+from owlapy.class_expression import OWLClassExpression, OWLClass, OWLObjectCardinalityRestriction, \
+    OWLObjectComplementOf, OWLNothing, OWLRestriction, OWLThing, OWLObjectSomeValuesFrom, \
+    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, OWLObjectHasSelf, \
+    OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataExactCardinality, OWLDataHasValue, \
+    OWLDataAllValuesFrom, OWLDataSomeValuesFrom, OWLObjectAllValuesFrom, \
+    OWLDataOneOf, OWLObjectIntersectionOf, \
+    OWLDataCardinalityRestriction, OWLNaryBooleanClassExpression, OWLObjectUnionOf, \
+    OWLObjectHasValue, OWLDatatypeRestriction, OWLFacetRestriction, OWLObjectOneOf
+from .owl_data_ranges import OWLDataComplementOf, OWLDataUnionOf, OWLDataIntersectionOf, OWLNaryDataRange, OWLDataRange, \
+    OWLPropertyRange
+from .owl_object import OWLObject
+from .owl_datatype import OWLDatatype
+
+
+class HasIndex(Protocol):
+    """Interface for types with an index; this is used to group objects by type when sorting."""
+    type_index: ClassVar[int]  #: index for this type. This is a sorting index for the types.
+
+    def __eq__(self, other): ...
+
+
+_HasIRI = TypeVar('_HasIRI', bound=HasIRI)  #:
+_HasIndex = TypeVar('_HasIndex', bound=HasIndex)  #:
+_O = TypeVar('_O')  #:
+_Enc = TypeVar('_Enc')
+_Con = TypeVar('_Con')
+_K = TypeVar('_K')
+_V = TypeVar('_V')
+
+
+@total_ordering
+class OrderedOWLObject:
+    """Holder of OWL Objects that can be used for Python sorted.
+
+    The Ordering is dependent on the type_index of the impl. classes recursively followed by all components of the
+    OWL Object.
+
+    Attributes:
+        o: OWL object.
+    """
+    __slots__ = 'o', '_chain'
+
+    o: _HasIndex  # o: Intersection[OWLObject, HasIndex]
+    _chain: Optional[Tuple]
+
+    # we are limited by https://github.com/python/typing/issues/213 # o: Intersection[OWLObject, HasIndex]
+    def __init__(self, o: _HasIndex):
+        """OWL Object holder with a defined sort order.
+
+        Args:
+            o: OWL Object.
+        """
+        self.o = o
+        self._chain = None
+
+    def _comparison_chain(self):
+        if self._chain is None:
+            c = [self.o.type_index]
+
+            if isinstance(self.o, OWLRestriction):
+                c.append(OrderedOWLObject(as_index(self.o.get_property())))
+            if isinstance(self.o, OWLObjectInverseOf):
+                c.append(self.o.get_named_property().str)
+            if isinstance(self.o, HasFiller):
+                c.append(OrderedOWLObject(self.o.get_filler()))
+            if isinstance(self.o, HasCardinality):
+                c.append(self.o.get_cardinality())
+            if isinstance(self.o, HasOperands):
+                c.append(tuple(map(OrderedOWLObject, self.o.operands())))
+            if isinstance(self.o, HasIRI):
+                c.append(self.o.str)
+            if isinstance(self.o, OWLDataComplementOf):
+                c.append(OrderedOWLObject(self.o.get_data_range()))
+            if isinstance(self.o, OWLDatatypeRestriction):
+                c.append((OrderedOWLObject(self.o.get_datatype()),
+                          tuple(map(OrderedOWLObject, self.o.get_facet_restrictions()))))
+            if isinstance(self.o, OWLFacetRestriction):
+                c.append((self.o.get_facet().str, self.o.get_facet_value().get_literal()))
+            if isinstance(self.o, OWLLiteral):
+                c.append(self.o.get_literal())
+            if len(c) == 1:
+                raise NotImplementedError(type(self.o))
+
+            self._chain = tuple(c)
+
+        return self._chain
+
+    def __lt__(self, other):
+        if self.o.type_index < other.o.type_index:
+            return True
+        elif self.o.type_index > other.o.type_index:
+            return False
+        else:
+            return self._comparison_chain() < other._comparison_chain()
+
+    def __eq__(self, other):
+        return self.o == other.o
+
+
+def _sort_by_ordered_owl_object(i: Iterable[_O]) -> Iterable[_O]:
+    return sorted(i, key=OrderedOWLObject)
+
+
+class NNF:
+    """This class contains functions to transform a Class Expression into Negation Normal Form."""
+    @singledispatchmethod
+    def get_class_nnf(self, ce: OWLClassExpression, negated: bool = False) -> OWLClassExpression:
+        """Convert a Class Expression to Negation Normal Form. Operands will be sorted.
+
+        Args:
+            ce: Class Expression.
+            negated: Whether the result should be negated.
+
+        Returns:
+            Class Expression in Negation Normal Form.
+            """
+        raise NotImplementedError
+
+    @get_class_nnf.register
+    def _(self, ce: OWLClass, negated: bool = False):
+        if negated:
+            if ce.is_owl_thing():
+                return OWLNothing
+            if ce.is_owl_nothing():
+                return OWLThing
+            return OWLObjectComplementOf(ce)
+        return ce
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectIntersectionOf, negated: bool = False):
+        ops = map(lambda _: self.get_class_nnf(_, negated),
+                  _sort_by_ordered_owl_object(ce.operands()))
+        if negated:
+            return OWLObjectUnionOf(ops)
+        return OWLObjectIntersectionOf(ops)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectUnionOf, negated: bool = False):
+        ops = map(lambda _: self.get_class_nnf(_, negated),
+                  _sort_by_ordered_owl_object(ce.operands()))
+        if negated:
+            return OWLObjectIntersectionOf(ops)
+        return OWLObjectUnionOf(ops)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectComplementOf, negated: bool = False):
+        return self.get_class_nnf(ce.get_operand(), not negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectSomeValuesFrom, negated: bool = False):
+        filler = self.get_class_nnf(ce.get_filler(), negated)
+        if negated:
+            return OWLObjectAllValuesFrom(ce.get_property(), filler)
+        return OWLObjectSomeValuesFrom(ce.get_property(), filler)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectAllValuesFrom, negated: bool = False):
+        filler = self.get_class_nnf(ce.get_filler(), negated)
+        if negated:
+            return OWLObjectSomeValuesFrom(ce.get_property(), filler)
+        return OWLObjectAllValuesFrom(ce.get_property(), filler)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectHasValue, negated: bool = False):
+        return self.get_class_nnf(ce.as_some_values_from(), negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectMinCardinality, negated: bool = False):
+        card = ce.get_cardinality()
+        if negated:
+            card = max(0, card - 1)
+        filler = self.get_class_nnf(ce.get_filler(), negated=False)
+        if negated:
+            return OWLObjectMaxCardinality(card, ce.get_property(), filler)
+        return OWLObjectMinCardinality(card, ce.get_property(), filler)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectExactCardinality, negated: bool = False):
+        return self.get_class_nnf(ce.as_intersection_of_min_max(), negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectMaxCardinality, negated: bool = False):
+        card = ce.get_cardinality()
+        if negated:
+            card = card + 1
+        filler = self.get_class_nnf(ce.get_filler(), negated=False)
+        if negated:
+            return OWLObjectMinCardinality(card, ce.get_property(), filler)
+        return OWLObjectMaxCardinality(card, ce.get_property(), filler)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectHasSelf, negated: bool = False):
+        if negated:
+            return ce.get_object_complement_of()
+        return ce
+
+    @get_class_nnf.register
+    def _(self, ce: OWLObjectOneOf, negated: bool = False):
+        union = ce.as_object_union_of()
+        if isinstance(union, OWLObjectOneOf):
+            if negated:
+                return ce.get_object_complement_of()
+            return ce
+        return self.get_class_nnf(union, negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataSomeValuesFrom, negated: bool = False):
+        filler = self.get_class_nnf(ce.get_filler(), negated)
+        if negated:
+            return OWLDataAllValuesFrom(ce.get_property(), filler)
+        return OWLDataSomeValuesFrom(ce.get_property(), filler)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataAllValuesFrom, negated: bool = False):
+        filler = self.get_class_nnf(ce.get_filler(), negated)
+        if negated:
+            return OWLDataSomeValuesFrom(ce.get_property(), filler)
+        return OWLDataAllValuesFrom(ce.get_property(), filler)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDatatypeRestriction, negated: bool = False):
+        if negated:
+            return OWLDataComplementOf(ce)
+        return ce
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDatatype, negated: bool = False):
+        if negated:
+            return OWLDataComplementOf(ce)
+        return ce
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataComplementOf, negated: bool = False):
+        return self.get_class_nnf(ce.get_data_range(), not negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataHasValue, negated: bool = False):
+        return self.get_class_nnf(ce.as_some_values_from(), negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataOneOf, negated: bool = False):
+        if len(list(ce.values())) == 1:
+            if negated:
+                return OWLDataComplementOf(ce)
+            return ce
+        union = OWLDataUnionOf([OWLDataOneOf(v) for v in ce.values()])
+        return self.get_class_nnf(union, negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataIntersectionOf, negated: bool = False):
+        ops = map(lambda _: self.get_class_nnf(_, negated),
+                  _sort_by_ordered_owl_object(ce.operands()))
+        if negated:
+            return OWLDataUnionOf(ops)
+        return OWLDataIntersectionOf(ops)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataUnionOf, negated: bool = False):
+        ops = map(lambda _: self.get_class_nnf(_, negated),
+                  _sort_by_ordered_owl_object(ce.operands()))
+        if negated:
+            return OWLDataIntersectionOf(ops)
+        return OWLDataUnionOf(ops)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataExactCardinality, negated: bool = False):
+        return self.get_class_nnf(ce.as_intersection_of_min_max(), negated)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataMinCardinality, negated: bool = False):
+        card = ce.get_cardinality()
+        if negated:
+            card = max(0, card - 1)
+        filler = self.get_class_nnf(ce.get_filler(), negated=False)
+        if negated:
+            return OWLDataMaxCardinality(card, ce.get_property(), filler)
+        return OWLDataMinCardinality(card, ce.get_property(), filler)
+
+    @get_class_nnf.register
+    def _(self, ce: OWLDataMaxCardinality, negated: bool = False):
+        card = ce.get_cardinality()
+        if negated:
+            card = card + 1
+        filler = self.get_class_nnf(ce.get_filler(), negated=False)
+        if negated:
+            return OWLDataMinCardinality(card, ce.get_property(), filler)
+        return OWLDataMaxCardinality(card, ce.get_property(), filler)
+
+
+# OWL-APy custom util start
+
+class TopLevelCNF:
+    """This class contains functions to transform a class expression into Top-Level Conjunctive Normal Form."""
+
+    def get_top_level_cnf(self, ce: OWLClassExpression) -> OWLClassExpression:
+        """Convert a class expression into Top-Level Conjunctive Normal Form. Operands will be sorted.
+
+        Args:
+            ce: Class Expression.
+
+        Returns:
+            Class Expression in Top-Level Conjunctive Normal Form.
+            """
+        c = _get_top_level_form(ce.get_nnf(), OWLObjectUnionOf, OWLObjectIntersectionOf)
+        return combine_nary_expressions(c)
+
+
+class TopLevelDNF:
+    """This class contains functions to transform a class expression into Top-Level Disjunctive Normal Form."""
+
+    def get_top_level_dnf(self, ce: OWLClassExpression) -> OWLClassExpression:
+        """Convert a class expression into Top-Level Disjunctive Normal Form. Operands will be sorted.
+
+        Args:
+            ce: Class Expression.
+
+        Returns:
+            Class Expression in Top-Level Disjunctive Normal Form.
+            """
+        c = _get_top_level_form(ce.get_nnf(), OWLObjectIntersectionOf, OWLObjectUnionOf)
+        return combine_nary_expressions(c)
+
+
+def _get_top_level_form(ce: OWLClassExpression,
+                        type_a: Type[OWLNaryBooleanClassExpression],
+                        type_b: Type[OWLNaryBooleanClassExpression]) -> OWLClassExpression:
+    """ Transforms a class expression (that's already in NNF) into Top-Level Conjunctive/Disjunctive Normal Form.
+    Here type_a specifies the operand which should be distributed inwards over type_b.
+
+    Conjunctive Normal form:
+        type_a = OWLObjectUnionOf
+        type_b = OWLObjectIntersectionOf
+    Disjunctive Normal form:
+        type_a = OWLObjectIntersectionOf
+        type_b = OWLObjectUnionOf
+    """
+
+    def distributive_law(a: OWLClassExpression, b: OWLNaryBooleanClassExpression) -> OWLNaryBooleanClassExpression:
+        return type_b(type_a([a, op]) for op in b.operands())
+
+    if isinstance(ce, type_a):
+        ce = cast(OWLNaryBooleanClassExpression, combine_nary_expressions(ce))
+        type_b_exprs = [op for op in ce.operands() if isinstance(op, type_b)]
+        non_type_b_exprs = [op for op in ce.operands() if not isinstance(op, type_b)]
+        if not len(type_b_exprs):
+            return ce
+
+        if len(non_type_b_exprs):
+            expr = non_type_b_exprs[0] if len(non_type_b_exprs) == 1 \
+                else type_a(non_type_b_exprs)
+            expr = distributive_law(expr, type_b_exprs[0])
+        else:
+            expr = type_b_exprs[0]
+
+        if len(type_b_exprs) == 1:
+            return _get_top_level_form(expr, type_a, type_b)
+
+        for type_b_expr in type_b_exprs[1:]:
+            expr = distributive_law(type_b_expr, expr)
+        return _get_top_level_form(expr, type_a, type_b)
+    elif isinstance(ce, type_b):
+        return type_b(_get_top_level_form(op, type_a, type_b) for op in ce.operands())
+    elif isinstance(ce, OWLClassExpression):
+        return ce
+    else:
+        raise ValueError('Top-Level CNF/DNF only applicable on class expressions', ce)
+
+
+@overload
+def combine_nary_expressions(ce: OWLClassExpression) -> OWLClassExpression:
+    ...
+
+
+@overload
+def combine_nary_expressions(ce: OWLDataRange) -> OWLDataRange:
+    ...
+
+
+def combine_nary_expressions(ce: OWLPropertyRange) -> OWLPropertyRange:
+    """ Shortens an OWLClassExpression or OWLDataRange by combining all nested nary expressions of the same type.
+    Operands will be sorted.
+
+    E.g. OWLObjectUnionOf(A, OWLObjectUnionOf(C, B)) -> OWLObjectUnionOf(A, B, C).
+    """
+    if isinstance(ce, (OWLNaryBooleanClassExpression, OWLNaryDataRange)):
+        expressions: List[OWLPropertyRange] = []
+        for op in ce.operands():
+            expr = combine_nary_expressions(op)
+            if type(expr) is type(ce):
+                expr = cast(Union[OWLNaryBooleanClassExpression, OWLNaryDataRange], expr)
+                expressions.extend(expr.operands())
+            else:
+                expressions.append(expr)
+        return type(ce)(_sort_by_ordered_owl_object(expressions))  # type: ignore
+    elif isinstance(ce, OWLObjectComplementOf):
+        return OWLObjectComplementOf(combine_nary_expressions(ce.get_operand()))
+    elif isinstance(ce, OWLDataComplementOf):
+        return OWLDataComplementOf(combine_nary_expressions(ce.get_data_range()))
+    elif isinstance(ce, OWLObjectCardinalityRestriction):
+        return type(ce)(ce.get_cardinality(), ce.get_property(), combine_nary_expressions(ce.get_filler()))
+    elif isinstance(ce, OWLDataCardinalityRestriction):
+        return type(ce)(ce.get_cardinality(), ce.get_property(), combine_nary_expressions(ce.get_filler()))
+    elif isinstance(ce, (OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom)):
+        return type(ce)(ce.get_property(), combine_nary_expressions(ce.get_filler()))
+    elif isinstance(ce, (OWLDataSomeValuesFrom, OWLDataAllValuesFrom)):
+        return type(ce)(ce.get_property(), combine_nary_expressions(ce.get_filler()))
+    elif isinstance(ce, OWLObjectOneOf):
+        return OWLObjectOneOf(_sort_by_ordered_owl_object(ce.operands()))
+    elif isinstance(ce, OWLDataOneOf):
+        return OWLDataOneOf(_sort_by_ordered_owl_object(ce.operands()))
+    elif isinstance(ce, OWLPropertyRange):
+        return ce
+    else:
+        raise ValueError(f'({ce}) is not an OWLObject.')
+
+
+def iter_count(i: Iterable) -> int:
+    """Count the number of elements in an iterable."""
+    return sum(1 for _ in i)
+
+
+def as_index(o: OWLObject) -> HasIndex:
+    """Cast OWL Object to HasIndex."""
+    i = cast(HasIndex, o)
+    assert type(i).type_index
+    return i
+
+
+class LRUCache(Generic[_K, _V]):
+    """Constants shares by all lru cache instances.
+
+    Adapted from functools.lru_cache.
+
+    Attributes:
+        sentinel: Unique object used to signal cache misses.
+        PREV: Name for the link field 0.
+        NEXT: Name for the link field 1.
+        KEY: Name for the link field 2.
+        RESULT: Name for the link field 3.
+    """
+
+    sentinel = object()
+    PREV, NEXT, KEY, RESULT = 0, 1, 2, 3  # names for the link fields
+
+    def __init__(self, maxsize: Optional[int] = None):
+        from _thread import RLock
+
+        self.cache = {}
+        self.hits = self.misses = 0
+        self.full = False
+        self.cache_get = self.cache.get  # bound method to lookup a key or return None
+        self.cache_len = self.cache.__len__  # get cache size without calling len()
+        self.lock = RLock()  # because linkedlist updates aren't threadsafe
+        self.root = []  # root of the circular doubly linked list
+        self.root[:] = [self.root, self.root, None, None]  # initialize by pointing to self
+        self.maxsize = maxsize
+
+    def __contains__(self, item: _K) -> bool:
+        with self.lock:
+            link = self.cache_get(item)
+            if link is not None:
+                self.hits += 1
+                return True
+            self.misses += 1
+            return False
+
+    def __getitem__(self, item: _K) -> _V:
+        with self.lock:
+            link = self.cache_get(item)
+            if link is not None:
+                # Move the link to the front of the circular queue
+                link_prev, link_next, _key, result = link
+                link_prev[LRUCache.NEXT] = link_next
+                link_next[LRUCache.PREV] = link_prev
+                last = self.root[LRUCache.PREV]
+                last[LRUCache.NEXT] = self.root[LRUCache.PREV] = link
+                link[LRUCache.PREV] = last
+                link[LRUCache.NEXT] = self.root
+                return result
+
+    def __setitem__(self, key: _K, value: _V):
+        with self.lock:
+            if key in self.cache:
+                # Getting here means that this same key was added to the
+                # cache while the lock was released.  Since the link
+                # update is already done, we need only return the
+                # computed result and update the count of misses.
+                pass
+            elif self.full:
+                # Use the old root to store the new key and result.
+                oldroot = self.root
+                oldroot[LRUCache.KEY] = key
+                oldroot[LRUCache.RESULT] = value
+                # Empty the oldest link and make it the new root.
+                # Keep a reference to the old key and old result to
+                # prevent their ref counts from going to zero during the
+                # update. That will prevent potentially arbitrary object
+                # clean-up code (i.e. __del__) from running while we're
+                # still adjusting the links.
+                self.root = oldroot[LRUCache.NEXT]
+                oldkey = self.root[LRUCache.KEY]
+                _oldresult = self.root[LRUCache.RESULT]  # noqa: F841
+                self.root[LRUCache.KEY] = self.root[LRUCache.RESULT] = None
+                # Now update the cache dictionary.
+                del self.cache[oldkey]
+                # Save the potentially reentrant cache[key] assignment
+                # for last, after the root and links have been put in
+                # a consistent state.
+                self.cache[key] = oldroot
+            else:
+                # Put result in a new link at the front of the queue.
+                last = self.root[LRUCache.PREV]
+                link = [last, self.root, key, value]
+                last[LRUCache.NEXT] = self.root[LRUCache.PREV] = self.cache[key] = link
+                # Use the cache_len bound method instead of the len() function
+                # which could potentially be wrapped in an lru_cache itself.
+                if self.maxsize is not None:
+                    self.full = (self.cache_len() >= self.maxsize)
+
+    def cache_info(self):
+        """Report cache statistics."""
+        with self.lock:
+            from collections import namedtuple
+            return namedtuple("CacheInfo", ["hits", "misses", "maxsize", "currsize"])(
+                self.hits, self.misses, self.maxsize, self.cache_len())
+
+    def cache_clear(self):
+        """Clear the cache and cache statistics."""
+        with self.lock:
+            self.cache.clear()
+            self.root[:] = [self.root, self.root, None, None]
+            self.hits = self.misses = 0
+            self.full = False
+
+
+def move(*args):
+    """"Move" an imported class to the current module by setting the classes __module__ attribute.
+
+    This is useful for documentation purposes to hide internal packages in sphinx.
+
+    Args:
+        args: List of classes to move.
+    """
+    from inspect import currentframe
+    f = currentframe()
+    f = f.f_back
+    mod = f.f_globals['__name__']
+    for cls in args:
+        cls.__module__ = mod
```

### Comparing `owlapy-0.1.3/owlapy.egg-info/SOURCES.txt` & `owlapy-1.0.0/owlapy.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 owlapy/__init__.py
-owlapy/_utils.py
-owlapy/has.py
+owlapy/converter.py
 owlapy/iri.py
 owlapy/meta_classes.py
 owlapy/namespaces.py
 owlapy/owl_annotation.py
 owlapy/owl_axiom.py
+owlapy/owl_data_ranges.py
+owlapy/owl_datatype.py
 owlapy/owl_individual.py
 owlapy/owl_literal.py
+owlapy/owl_object.py
+owlapy/owl_ontology.py
+owlapy/owl_ontology_manager.py
 owlapy/owl_property.py
-owlapy/owlobject.py
+owlapy/owl_reasoner.py
 owlapy/parser.py
+owlapy/providers.py
 owlapy/render.py
-owlapy/types.py
 owlapy/util.py
 owlapy/vocab.py
 owlapy.egg-info/PKG-INFO
 owlapy.egg-info/SOURCES.txt
 owlapy.egg-info/dependency_links.txt
 owlapy.egg-info/requires.txt
 owlapy.egg-info/top_level.txt
 owlapy/class_expression/__init__.py
 owlapy/class_expression/class_expression.py
 owlapy/class_expression/nary_boolean_expression.py
 owlapy/class_expression/owl_class.py
 owlapy/class_expression/restriction.py
-owlapy/data_ranges/__init__.py
 owlapy/entities/__init__.py
-owlapy/model/__init__.py
-owlapy/model/providers.py
-owlapy/owl2sparql/__init__.py
-owlapy/owl2sparql/converter.py
 tests/test_class_expression_semantics.py
 tests/test_examples.py
 tests/test_owlapy.py
 tests/test_owlapy_cnf_dnf.py
 tests/test_owlapy_nnf.py
 tests/test_owlapy_parser.py
 tests/test_owlapy_render.py
```

### Comparing `owlapy-0.1.3/setup.py` & `owlapy-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from setuptools import setup, find_packages
-
-with open('README.md', 'r') as fh:
-    long_description = fh.read()
-setup(
-    name="owlapy",
-    description="Owlapy is loosely based on owlapi - the java counterpart, "
-                "successfully representing the main owl objects in python.",
-    version="0.1.3",
-    packages=find_packages(),
-    install_requires=[
-        "pandas>=1.5.0",
-        "rdflib>=6.0.2",
-        "parsimonious>=0.8.1",
-        "pytest>=8.1.1"],
-    author='Caglar Demir',
-    author_email='caglardemir8@gmail.com',
-    url='https://github.com/dice-group/owlapy',
-    classifiers=[
-        "Programming Language :: Python :: 3.10",
-        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
-        "Topic :: Scientific/Engineering"],
-    python_requires='>=3.10',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-)
+from setuptools import setup, find_packages
+
+with open('README.md', 'r') as fh:
+    long_description = fh.read()
+setup(
+    name="owlapy",
+    description="OWLAPY is a Python Framework for creating and manipulating OWL Ontologies.",
+    version="1.0.0",
+    packages=find_packages(),
+    install_requires=[
+        "pandas>=1.5.0",
+        "rdflib>=6.0.2",
+        "parsimonious>=0.8.1",
+        "pytest>=8.1.1"],
+    author='Caglar Demir',
+    author_email='caglardemir8@gmail.com',
+    url='https://github.com/dice-group/owlapy',
+    classifiers=[
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+        "Topic :: Scientific/Engineering"],
+    python_requires='>=3.10',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+)
```

### Comparing `owlapy-0.1.3/tests/test_examples.py` & `owlapy-1.0.0/tests/test_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-
-from owlapy.iri import IRI
-from owlapy.class_expression import OWLClass, OWLObjectIntersectionOf
-from owlapy.owl_property import OWLObjectProperty
-from owlapy.class_expression import OWLObjectSomeValuesFrom
-from owlapy.owl2sparql.converter import owl_expression_to_sparql
-from owlapy.render import owl_expression_to_dl
-
-class TestRunningExamples:
-    def test_readme(self):
-        # Create the male class
-        male = OWLClass("http://example.com/society#male")
-
-        # Create an object property using the iri as a string for 'hasChild' property.
-        hasChild = OWLObjectProperty("http://example.com/society#hasChild")
-
-        # Create an existential restrictions
-        males_with_children = OWLObjectSomeValuesFrom(hasChild, male)
-
-        # Let's make it more complex by intersecting with another class
-        teacher = OWLClass("http://example.com/society#teacher")
-        male_teachers_with_children = OWLObjectIntersectionOf([males_with_children, teacher])
-
-        assert owl_expression_to_dl(male_teachers_with_children)=="(∃ hasChild.male) ⊓ teacher"
-        assert owl_expression_to_sparql("?x", male_teachers_with_children)=="""SELECT
- DISTINCT ?x WHERE { 
-?x <http://example.com/society#hasChild> ?s_1 . 
-?s_1 a <http://example.com/society#male> . 
-?x a <http://example.com/society#teacher> . 
+from owlapy.class_expression import OWLClass, OWLObjectIntersectionOf
+from owlapy.owl_property import OWLObjectProperty
+from owlapy.class_expression import OWLObjectSomeValuesFrom
+from owlapy.converter import owl_expression_to_sparql
+from owlapy.render import owl_expression_to_dl
+
+class TestRunningExamples:
+    def test_readme(self):
+        # Create the male class
+        male = OWLClass("http://example.com/society#male")
+
+        # Create an object property using the iri as a string for 'hasChild' property.
+        hasChild = OWLObjectProperty("http://example.com/society#hasChild")
+
+        # Create an existential restrictions
+        males_with_children = OWLObjectSomeValuesFrom(hasChild, male)
+
+        # Let's make it more complex by intersecting with another class
+        teacher = OWLClass("http://example.com/society#teacher")
+        male_teachers_with_children = OWLObjectIntersectionOf([males_with_children, teacher])
+
+        assert owl_expression_to_dl(male_teachers_with_children)=="(∃ hasChild.male) ⊓ teacher"
+        assert owl_expression_to_sparql("?x", male_teachers_with_children)=="""SELECT
+ DISTINCT ?x WHERE { 
+?x <http://example.com/society#hasChild> ?s_1 . 
+?s_1 a <http://example.com/society#male> . 
+?x a <http://example.com/society#teacher> . 
  }"""
```

### Comparing `owlapy-0.1.3/tests/test_owlapy.py` & `owlapy-1.0.0/tests/test_owlapy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-import unittest
-
-from owlapy import namespaces
-from owlapy.namespaces import Namespaces
-from owlapy.model import OWLClass, OWLObjectUnionOf, IRI
-
-base = Namespaces("ex", "http://example.org/")
-
-
-class Owlapy_Test(unittest.TestCase):
-    def test_iri(self):
-        i1 = IRI(base, "I1")
-        i2 = IRI(base, "I2")
-        i1x = IRI(base, "I1")
-        self.assertEqual(i1, i1x)
-        self.assertIs(i1, i1x)
-        self.assertNotEqual(i1, i2)
-
-    def test_class(self):
-        c1 = OWLClass(IRI(base, "C1"))
-        c2 = OWLClass(IRI(base, "C2"))
-        c1x = OWLClass(IRI(base, "C1"))
-        thing = OWLClass(IRI(namespaces.OWL, "Thing"))
-        self.assertTrue(thing.is_owl_thing())
-        self.assertEqual(c1, c1x)
-        self.assertNotEqual(c2, c1)
-
-    def test_union(self):
-        c1 = OWLClass(IRI(base, "C1"))
-        c2 = OWLClass(IRI(base, "C2"))
-        c3 = OWLObjectUnionOf((c1, c2))
-        self.assertSequenceEqual(list(c3.operands()), [c1, c2])
-
-    def test_iri_fixed_set(self):
-        fs = frozenset({IRI.create(base, "C1"), IRI.create(base, "C2")})
-        self.assertIn(IRI.create(base, "C1"), fs)
-        self.assertNotIn(IRI.create(base, "C3"), fs)
-        self.assertNotEqual(fs & {IRI.create(base, "C2")}, fs & {IRI.create(base, "C1")})
-        self.assertEqual(fs & {IRI.create(base, "C1")}, fs & {IRI.create(base, "C1")})
-        self.assertEqual(fs & {IRI.create(base, "C3")}, frozenset())
-        self.assertEqual(set(), frozenset())
-        self.assertSequenceEqual(list([IRI.create(base, "C1")]), [IRI.create(base, "C1")])
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from owlapy import namespaces
+from owlapy.class_expression import OWLClass, OWLObjectUnionOf
+from owlapy.iri import IRI
+from owlapy.namespaces import Namespaces
+
+base = Namespaces("ex", "http://example.org/")
+
+
+class Owlapy_Test(unittest.TestCase):
+    def test_iri(self):
+        i1 = IRI(base, "I1")
+        i2 = IRI(base, "I2")
+        i1x = IRI(base, "I1")
+        self.assertEqual(i1, i1x)
+        self.assertIs(i1, i1x)
+        self.assertNotEqual(i1, i2)
+
+    def test_class(self):
+        c1 = OWLClass(IRI(base, "C1"))
+        c2 = OWLClass(IRI(base, "C2"))
+        c1x = OWLClass(IRI(base, "C1"))
+        thing = OWLClass(IRI(namespaces.OWL, "Thing"))
+        self.assertTrue(thing.is_owl_thing())
+        self.assertEqual(c1, c1x)
+        self.assertNotEqual(c2, c1)
+
+    def test_union(self):
+        c1 = OWLClass(IRI(base, "C1"))
+        c2 = OWLClass(IRI(base, "C2"))
+        c3 = OWLObjectUnionOf((c1, c2))
+        self.assertSequenceEqual(list(c3.operands()), [c1, c2])
+
+    def test_iri_fixed_set(self):
+        fs = frozenset({IRI.create(base, "C1"), IRI.create(base, "C2")})
+        self.assertIn(IRI.create(base, "C1"), fs)
+        self.assertNotIn(IRI.create(base, "C3"), fs)
+        self.assertNotEqual(fs & {IRI.create(base, "C2")}, fs & {IRI.create(base, "C1")})
+        self.assertEqual(fs & {IRI.create(base, "C1")}, fs & {IRI.create(base, "C1")})
+        self.assertEqual(fs & {IRI.create(base, "C3")}, frozenset())
+        self.assertEqual(set(), frozenset())
+        self.assertSequenceEqual(list([IRI.create(base, "C1")]), [IRI.create(base, "C1")])
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `owlapy-0.1.3/tests/test_owlapy_cnf_dnf.py` & `owlapy-1.0.0/tests/test_owlapy_cnf_dnf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,195 +1,198 @@
-import unittest
-
-from owlapy.model import OWLObjectProperty, OWLObjectSomeValuesFrom, OWLObjectUnionOf, \
-    OWLClass, IRI, OWLDataProperty, OWLDataSomeValuesFrom, OWLNamedIndividual, OWLObjectComplementOf, \
-    OWLObjectIntersectionOf, OWLObjectMinCardinality
-from owlapy.model.providers import OWLDatatypeMinExclusiveRestriction
-from owlapy.util import TopLevelCNF, TopLevelDNF
-from owlapy.class_expression import OWLObjectOneOf
-
-class TopLevelNFTest(unittest.TestCase):
-
-    def setUp(self):
-        namespace = 'http://test.org/test#'
-
-        # Classes
-        self.a = OWLClass(IRI(namespace, 'A'))
-        self.b = OWLClass(IRI(namespace, 'B'))
-        self.c = OWLClass(IRI(namespace, 'C'))
-        self.d = OWLClass(IRI(namespace, 'D'))
-        self.e = OWLClass(IRI(namespace, 'E'))
-        self.f = OWLClass(IRI(namespace, 'F'))
-        self.g = OWLClass(IRI(namespace, 'G'))
-        self.h = OWLClass(IRI(namespace, 'H'))
-
-        # Object Properties
-        self.op1 = OWLObjectProperty(IRI.create(namespace, 'op1'))
-
-        # Data Properties
-        self.dp1 = OWLDataProperty(IRI.create(namespace, 'dp1'))
-
-        # Complex Expressions
-        self.c1 = OWLObjectSomeValuesFrom(self.op1,
-                                          OWLObjectUnionOf([self.a, OWLObjectIntersectionOf([self.a, self.b])]))
-        self.c2 = OWLDataSomeValuesFrom(self.dp1, OWLDatatypeMinExclusiveRestriction(5))
-        self.c3 = OWLObjectSomeValuesFrom(self.op1, OWLObjectOneOf(OWLNamedIndividual(IRI(namespace, 'AB'))))
-
-    def test_cnf(self):
-        cnf = TopLevelCNF()
-
-        # A or ( A and B)
-        c = OWLObjectUnionOf([self.a, OWLObjectIntersectionOf([self.a, self.b])])
-        c = cnf.get_top_level_cnf(c)
-        # (A or A) and (A or B)
-        true_c = OWLObjectIntersectionOf([OWLObjectUnionOf([self.a, self.a]), OWLObjectUnionOf([self.a, self.b])])
-        self.assertEqual(true_c, c)
-
-        # op1 some (A or ( A and B))
-        c = cnf.get_top_level_cnf(self.c1)
-        self.assertEqual(self.c1, c)
-
-        # (A and c2) or c1 or (D and E)
-        c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.a, self.c2)), self.c1,
-                              OWLObjectIntersectionOf((self.d, self.e))))
-        c = cnf.get_top_level_cnf(c)
-        # (A or D or c1) and (A or E or c1) and (D or c1 or c2) and (E or c1 or c2)
-        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.a, self.d, self.c1)),
-                                          OWLObjectUnionOf((self.a, self.e, self.c1)),
-                                          OWLObjectUnionOf((self.d, self.c1, self.c2)),
-                                          OWLObjectUnionOf((self.e, self.c1, self.c2))))
-        self.assertEqual(true_c, c)
-
-        # A or ((C and D) or B)
-        c = OWLObjectUnionOf((self.a, OWLObjectUnionOf((OWLObjectIntersectionOf((self.c, self.d)), self.b))))
-        c = cnf.get_top_level_cnf(c)
-        # (A or B or C) and (A or B or D)
-        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.a, self.b, self.c)),
-                                          OWLObjectUnionOf((self.a, self.b, self.d))))
-        self.assertEqual(true_c, c)
-
-        # (c1 and B) or (C and c2) or (E and c3)
-        c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.c1, self.b)),
-                              OWLObjectIntersectionOf((self.c, self.c2)),
-                              OWLObjectIntersectionOf((self.e, self.c3))))
-        # (B or C or E) and (B or C or c3) and (B or E or c2) and (B or c3 or c2) and (C or E or c1)
-        # and (C or c1 or c3) and (E or c1 or c2) and (c1 or c3 or c2)
-        c = cnf.get_top_level_cnf(c)
-        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.b, self.c, self.e)),
-                                          OWLObjectUnionOf((self.b, self.c, self.c3)),
-                                          OWLObjectUnionOf((self.b, self.e, self.c2)),
-                                          OWLObjectUnionOf((self.b, self.c3, self.c2)),
-                                          OWLObjectUnionOf((self.c, self.e, self.c1)),
-                                          OWLObjectUnionOf((self.c, self.c1, self.c3)),
-                                          OWLObjectUnionOf((self.e, self.c1, self.c2)),
-                                          OWLObjectUnionOf((self.c1, self.c3, self.c2))))
-        self.assertEqual(true_c, c)
-
-        # not (A or (B or (C and (D or (E and (F and (G or H)))))))
-        c = OWLObjectComplementOf(
-                OWLObjectUnionOf((
-                    self.a,
-                    OWLObjectUnionOf((
-                        self.b,
-                        OWLObjectIntersectionOf((
-                            self.c,
-                            OWLObjectUnionOf((
-                                self.d,
-                                OWLObjectIntersectionOf((
-                                    self.e,
-                                    OWLObjectIntersectionOf((self.f, OWLObjectUnionOf((self.g, self.h)))))))))))))))
-        c = cnf.get_top_level_cnf(c)
-        # ((not C) or (not D)) and ((not C) or (not E) or (not F) or (not G)) and ((not C) or
-        # (not E) or (not F) or (not H)) and (not A) and (not B)
-        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((OWLObjectComplementOf(self.c),
-                                                            OWLObjectComplementOf(self.d))),
-                                          OWLObjectUnionOf((OWLObjectComplementOf(self.c),
-                                                            OWLObjectComplementOf(self.e),
-                                                            OWLObjectComplementOf(self.f),
-                                                            OWLObjectComplementOf(self.g))),
-                                          OWLObjectUnionOf((OWLObjectComplementOf(self.c),
-                                                            OWLObjectComplementOf(self.e),
-                                                            OWLObjectComplementOf(self.f),
-                                                            OWLObjectComplementOf(self.h))),
-                                          OWLObjectComplementOf(self.a), OWLObjectComplementOf(self.b)))
-        self.assertEqual(true_c, c)
-
-    def test_dnf(self):
-        dnf = TopLevelDNF()
-
-        # A and ( A or B)
-        c = OWLObjectIntersectionOf([self.a, OWLObjectUnionOf([self.a, self.b])])
-        c = dnf.get_top_level_dnf(c)
-        # (A and A) or (A and B)
-        true_c = OWLObjectUnionOf([OWLObjectIntersectionOf([self.a, self.a]),
-                                   OWLObjectIntersectionOf([self.a, self.b])])
-        self.assertEqual(true_c, c)
-
-        # op1 min 5 (A and ( A or B))
-        old_c = OWLObjectMinCardinality(5, self.op1,
-                                        OWLObjectIntersectionOf([self.a, OWLObjectUnionOf([self.a, self.b])]))
-        c = dnf.get_top_level_dnf(old_c)
-        self.assertEqual(old_c, c)
-
-        # (A or c2) and c1 and (D or E)
-        c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.a, self.c2)), self.c1, OWLObjectUnionOf((self.d, self.e))))
-        c = dnf.get_top_level_dnf(c)
-        # (A and D and c1) or (A and E and c1) or (D and c1 and c2) or (E and c1 and c2)
-        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.a, self.d, self.c1)),
-                                   OWLObjectIntersectionOf((self.a, self.e, self.c1)),
-                                   OWLObjectIntersectionOf((self.d, self.c1, self.c2)),
-                                   OWLObjectIntersectionOf((self.e, self.c1, self.c2))))
-        self.assertEqual(true_c, c)
-
-        # c1 and ((C or D) and B)
-        c = OWLObjectIntersectionOf((self.c1, OWLObjectIntersectionOf((OWLObjectUnionOf((self.c, self.d)), self.b))))
-        c = dnf.get_top_level_dnf(c)
-        # (B and C and c1) or (B and D and c1)
-        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.b, self.c, self.c1)),
-                                   OWLObjectIntersectionOf((self.b, self.d, self.c1))))
-        self.assertEqual(true_c, c)
-
-        # (c1 or B) and (C or c2) and (E or c3)
-        c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.c1, self.b)),
-                                     OWLObjectUnionOf((self.c, self.c2)),
-                                     OWLObjectUnionOf((self.e, self.c3))))
-        # (B and C and E) or (B and C and c3) or (B and E and c2) or (B and c3 and c2) or (C and E and c1)
-        # or (C and c1 and c3) or (E and c1 and c2) or (c1 and c3 and c2)
-        c = dnf.get_top_level_dnf(c)
-        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.b, self.c, self.e)),
-                                   OWLObjectIntersectionOf((self.b, self.c, self.c3)),
-                                   OWLObjectIntersectionOf((self.b, self.e, self.c2)),
-                                   OWLObjectIntersectionOf((self.b, self.c3, self.c2)),
-                                   OWLObjectIntersectionOf((self.c, self.e, self.c1)),
-                                   OWLObjectIntersectionOf((self.c, self.c1, self.c3)),
-                                   OWLObjectIntersectionOf((self.e, self.c1, self.c2)),
-                                   OWLObjectIntersectionOf((self.c1, self.c3, self.c2))))
-        self.assertEqual(true_c, c)
-
-        # not (A and (B and (C or (D and (E or (F or (G and H)))))))
-        c = OWLObjectComplementOf(
-                OWLObjectIntersectionOf((
-                    self.a,
-                    OWLObjectIntersectionOf((
-                        self.b,
-                        OWLObjectUnionOf((
-                            self.c,
-                            OWLObjectIntersectionOf((
-                                self.d,
-                                OWLObjectUnionOf((
-                                    self.e,
-                                    OWLObjectUnionOf((self.f, OWLObjectIntersectionOf((self.g, self.h)))))))))))))))
-        c = dnf.get_top_level_dnf(c)
-        # ((not C) and (not D)) or ((not C) and (not E) and (not F) and (not G)) or ((not C) and
-        # (not E) and (not F) and (not H)) or (not A) or (not B)
-        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((OWLObjectComplementOf(self.c),
-                                                            OWLObjectComplementOf(self.d))),
-                                   OWLObjectIntersectionOf((OWLObjectComplementOf(self.c),
-                                                            OWLObjectComplementOf(self.e),
-                                                            OWLObjectComplementOf(self.f),
-                                                            OWLObjectComplementOf(self.g))),
-                                   OWLObjectIntersectionOf((OWLObjectComplementOf(self.c),
-                                                            OWLObjectComplementOf(self.e),
-                                                            OWLObjectComplementOf(self.f),
-                                                            OWLObjectComplementOf(self.h))),
-                                   OWLObjectComplementOf(self.a), OWLObjectComplementOf(self.b)))
-        self.assertEqual(true_c, c)
+import unittest
+
+from owlapy.class_expression import OWLObjectSomeValuesFrom, OWLObjectUnionOf, \
+    OWLClass, OWLDataSomeValuesFrom, OWLObjectComplementOf, \
+    OWLObjectIntersectionOf, OWLObjectMinCardinality, OWLObjectOneOf
+from owlapy.iri import IRI
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty
+from owlapy.providers import owl_datatype_min_exclusive_restriction
+from owlapy.util import TopLevelCNF, TopLevelDNF
+
+
+class TopLevelNFTest(unittest.TestCase):
+
+    def setUp(self):
+        namespace = 'http://test.org/test#'
+
+        # Classes
+        self.a = OWLClass(IRI(namespace, 'A'))
+        self.b = OWLClass(IRI(namespace, 'B'))
+        self.c = OWLClass(IRI(namespace, 'C'))
+        self.d = OWLClass(IRI(namespace, 'D'))
+        self.e = OWLClass(IRI(namespace, 'E'))
+        self.f = OWLClass(IRI(namespace, 'F'))
+        self.g = OWLClass(IRI(namespace, 'G'))
+        self.h = OWLClass(IRI(namespace, 'H'))
+
+        # Object Properties
+        self.op1 = OWLObjectProperty(IRI.create(namespace, 'op1'))
+
+        # Data Properties
+        self.dp1 = OWLDataProperty(IRI.create(namespace, 'dp1'))
+
+        # Complex Expressions
+        self.c1 = OWLObjectSomeValuesFrom(self.op1,
+                                          OWLObjectUnionOf([self.a, OWLObjectIntersectionOf([self.a, self.b])]))
+        self.c2 = OWLDataSomeValuesFrom(self.dp1, owl_datatype_min_exclusive_restriction(5))
+        self.c3 = OWLObjectSomeValuesFrom(self.op1, OWLObjectOneOf(OWLNamedIndividual(IRI(namespace, 'AB'))))
+
+    def test_cnf(self):
+        cnf = TopLevelCNF()
+
+        # A or ( A and B)
+        c = OWLObjectUnionOf([self.a, OWLObjectIntersectionOf([self.a, self.b])])
+        c = cnf.get_top_level_cnf(c)
+        # (A or A) and (A or B)
+        true_c = OWLObjectIntersectionOf([OWLObjectUnionOf([self.a, self.a]), OWLObjectUnionOf([self.a, self.b])])
+        self.assertEqual(true_c, c)
+
+        # op1 some (A or ( A and B))
+        c = cnf.get_top_level_cnf(self.c1)
+        self.assertEqual(self.c1, c)
+
+        # (A and c2) or c1 or (D and E)
+        c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.a, self.c2)), self.c1,
+                              OWLObjectIntersectionOf((self.d, self.e))))
+        c = cnf.get_top_level_cnf(c)
+        # (A or D or c1) and (A or E or c1) and (D or c1 or c2) and (E or c1 or c2)
+        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.a, self.d, self.c1)),
+                                          OWLObjectUnionOf((self.a, self.e, self.c1)),
+                                          OWLObjectUnionOf((self.d, self.c1, self.c2)),
+                                          OWLObjectUnionOf((self.e, self.c1, self.c2))))
+        self.assertEqual(true_c, c)
+
+        # A or ((C and D) or B)
+        c = OWLObjectUnionOf((self.a, OWLObjectUnionOf((OWLObjectIntersectionOf((self.c, self.d)), self.b))))
+        c = cnf.get_top_level_cnf(c)
+        # (A or B or C) and (A or B or D)
+        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.a, self.b, self.c)),
+                                          OWLObjectUnionOf((self.a, self.b, self.d))))
+        self.assertEqual(true_c, c)
+
+        # (c1 and B) or (C and c2) or (E and c3)
+        c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.c1, self.b)),
+                              OWLObjectIntersectionOf((self.c, self.c2)),
+                              OWLObjectIntersectionOf((self.e, self.c3))))
+        # (B or C or E) and (B or C or c3) and (B or E or c2) and (B or c3 or c2) and (C or E or c1)
+        # and (C or c1 or c3) and (E or c1 or c2) and (c1 or c3 or c2)
+        c = cnf.get_top_level_cnf(c)
+        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.b, self.c, self.e)),
+                                          OWLObjectUnionOf((self.b, self.c, self.c3)),
+                                          OWLObjectUnionOf((self.b, self.e, self.c2)),
+                                          OWLObjectUnionOf((self.b, self.c3, self.c2)),
+                                          OWLObjectUnionOf((self.c, self.e, self.c1)),
+                                          OWLObjectUnionOf((self.c, self.c1, self.c3)),
+                                          OWLObjectUnionOf((self.e, self.c1, self.c2)),
+                                          OWLObjectUnionOf((self.c1, self.c3, self.c2))))
+        self.assertEqual(true_c, c)
+
+        # not (A or (B or (C and (D or (E and (F and (G or H)))))))
+        c = OWLObjectComplementOf(
+                OWLObjectUnionOf((
+                    self.a,
+                    OWLObjectUnionOf((
+                        self.b,
+                        OWLObjectIntersectionOf((
+                            self.c,
+                            OWLObjectUnionOf((
+                                self.d,
+                                OWLObjectIntersectionOf((
+                                    self.e,
+                                    OWLObjectIntersectionOf((self.f, OWLObjectUnionOf((self.g, self.h)))))))))))))))
+        c = cnf.get_top_level_cnf(c)
+        # ((not C) or (not D)) and ((not C) or (not E) or (not F) or (not G)) and ((not C) or
+        # (not E) or (not F) or (not H)) and (not A) and (not B)
+        true_c = OWLObjectIntersectionOf((OWLObjectUnionOf((OWLObjectComplementOf(self.c),
+                                                            OWLObjectComplementOf(self.d))),
+                                          OWLObjectUnionOf((OWLObjectComplementOf(self.c),
+                                                            OWLObjectComplementOf(self.e),
+                                                            OWLObjectComplementOf(self.f),
+                                                            OWLObjectComplementOf(self.g))),
+                                          OWLObjectUnionOf((OWLObjectComplementOf(self.c),
+                                                            OWLObjectComplementOf(self.e),
+                                                            OWLObjectComplementOf(self.f),
+                                                            OWLObjectComplementOf(self.h))),
+                                          OWLObjectComplementOf(self.a), OWLObjectComplementOf(self.b)))
+        self.assertEqual(true_c, c)
+
+    def test_dnf(self):
+        dnf = TopLevelDNF()
+
+        # A and ( A or B)
+        c = OWLObjectIntersectionOf([self.a, OWLObjectUnionOf([self.a, self.b])])
+        c = dnf.get_top_level_dnf(c)
+        # (A and A) or (A and B)
+        true_c = OWLObjectUnionOf([OWLObjectIntersectionOf([self.a, self.a]),
+                                   OWLObjectIntersectionOf([self.a, self.b])])
+        self.assertEqual(true_c, c)
+
+        # op1 min 5 (A and ( A or B))
+        old_c = OWLObjectMinCardinality(5, self.op1,
+                                        OWLObjectIntersectionOf([self.a, OWLObjectUnionOf([self.a, self.b])]))
+        c = dnf.get_top_level_dnf(old_c)
+        self.assertEqual(old_c, c)
+
+        # (A or c2) and c1 and (D or E)
+        c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.a, self.c2)), self.c1, OWLObjectUnionOf((self.d, self.e))))
+        c = dnf.get_top_level_dnf(c)
+        # (A and D and c1) or (A and E and c1) or (D and c1 and c2) or (E and c1 and c2)
+        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.a, self.d, self.c1)),
+                                   OWLObjectIntersectionOf((self.a, self.e, self.c1)),
+                                   OWLObjectIntersectionOf((self.d, self.c1, self.c2)),
+                                   OWLObjectIntersectionOf((self.e, self.c1, self.c2))))
+        self.assertEqual(true_c, c)
+
+        # c1 and ((C or D) and B)
+        c = OWLObjectIntersectionOf((self.c1, OWLObjectIntersectionOf((OWLObjectUnionOf((self.c, self.d)), self.b))))
+        c = dnf.get_top_level_dnf(c)
+        # (B and C and c1) or (B and D and c1)
+        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.b, self.c, self.c1)),
+                                   OWLObjectIntersectionOf((self.b, self.d, self.c1))))
+        self.assertEqual(true_c, c)
+
+        # (c1 or B) and (C or c2) and (E or c3)
+        c = OWLObjectIntersectionOf((OWLObjectUnionOf((self.c1, self.b)),
+                                     OWLObjectUnionOf((self.c, self.c2)),
+                                     OWLObjectUnionOf((self.e, self.c3))))
+        # (B and C and E) or (B and C and c3) or (B and E and c2) or (B and c3 and c2) or (C and E and c1)
+        # or (C and c1 and c3) or (E and c1 and c2) or (c1 and c3 and c2)
+        c = dnf.get_top_level_dnf(c)
+        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((self.b, self.c, self.e)),
+                                   OWLObjectIntersectionOf((self.b, self.c, self.c3)),
+                                   OWLObjectIntersectionOf((self.b, self.e, self.c2)),
+                                   OWLObjectIntersectionOf((self.b, self.c3, self.c2)),
+                                   OWLObjectIntersectionOf((self.c, self.e, self.c1)),
+                                   OWLObjectIntersectionOf((self.c, self.c1, self.c3)),
+                                   OWLObjectIntersectionOf((self.e, self.c1, self.c2)),
+                                   OWLObjectIntersectionOf((self.c1, self.c3, self.c2))))
+        self.assertEqual(true_c, c)
+
+        # not (A and (B and (C or (D and (E or (F or (G and H)))))))
+        c = OWLObjectComplementOf(
+                OWLObjectIntersectionOf((
+                    self.a,
+                    OWLObjectIntersectionOf((
+                        self.b,
+                        OWLObjectUnionOf((
+                            self.c,
+                            OWLObjectIntersectionOf((
+                                self.d,
+                                OWLObjectUnionOf((
+                                    self.e,
+                                    OWLObjectUnionOf((self.f, OWLObjectIntersectionOf((self.g, self.h)))))))))))))))
+        c = dnf.get_top_level_dnf(c)
+        # ((not C) and (not D)) or ((not C) and (not E) and (not F) and (not G)) or ((not C) and
+        # (not E) and (not F) and (not H)) or (not A) or (not B)
+        true_c = OWLObjectUnionOf((OWLObjectIntersectionOf((OWLObjectComplementOf(self.c),
+                                                            OWLObjectComplementOf(self.d))),
+                                   OWLObjectIntersectionOf((OWLObjectComplementOf(self.c),
+                                                            OWLObjectComplementOf(self.e),
+                                                            OWLObjectComplementOf(self.f),
+                                                            OWLObjectComplementOf(self.g))),
+                                   OWLObjectIntersectionOf((OWLObjectComplementOf(self.c),
+                                                            OWLObjectComplementOf(self.e),
+                                                            OWLObjectComplementOf(self.f),
+                                                            OWLObjectComplementOf(self.h))),
+                                   OWLObjectComplementOf(self.a), OWLObjectComplementOf(self.b)))
+        self.assertEqual(true_c, c)
```

### Comparing `owlapy-0.1.3/tests/test_owlapy_nnf.py` & `owlapy-1.0.0/tests/test_owlapy_nnf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,384 +1,388 @@
-#  This file is part of the OWL API.
-#  * The contents of this file are subject to the LGPL License, Version 3.0.
-#  * Copyright 2014, The University of Manchester
-#
-# * This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public
-# License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any
-# later version. * This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
-# even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public
-# License for more details. * You should have received a copy of the GNU General Public License along with this
-# program.  If not, see http://www.gnu.org/licenses/.
-#
-# * Alternatively, the contents of this file may be used under the terms of the Apache License, Version 2.0 in which
-# case, the provisions of the Apache License Version 2.0 are applicable instead of those above. * Licensed under the
-# Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You
-# may obtain a copy of the License at * http://www.apache.org/licenses/LICENSE-2.0 * Unless required by applicable
-# law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language
-# governing permissions and limitations under the License.
-#
-# package: org.semanticweb.owlapi.api.test.axioms
-#
-#  * @author Matthew Horridge, The University of Manchester, Information Management Group
-#  * @since 3.0.0
-#
-import unittest
-
-from owlapy.model import OWLObjectProperty, OWLNamedIndividual, OWLObjectComplementOf, \
-    OWLObjectAllValuesFrom, OWLObjectSomeValuesFrom, OWLObjectIntersectionOf, OWLObjectUnionOf, \
-    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLClassExpression, IRI, \
-    BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype, OWLClass, OWLDataAllValuesFrom, \
-    OWLDataProperty, OWLDataSomeValuesFrom,OWLDataHasValue, OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataOneOf, OWLLiteral
-from owlapy.model.providers import OWLDatatypeMinMaxExclusiveRestriction
-from owlapy.util import NNF
-
-from owlapy.data_ranges import OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
-from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf
-
-def iri(suffix):
-    NS = "http://example.org/"
-    return IRI.create(NS, suffix)
-
-
-class Owlapy_NNF_Test(unittest.TestCase):
-    """ generated source for class NNFTestCase """
-    clsA = OWLClass(iri("A"))
-    clsB = OWLClass(iri("B"))
-    clsC = OWLClass(iri("C"))
-    clsD = OWLClass(iri("D"))
-    propP = OWLObjectProperty(iri("p"))
-    indA = OWLNamedIndividual(iri("a"))
-
-    def get_nnf(self, ce: OWLClassExpression):
-        return NNF().get_class_nnf(ce)
-
-    def testPosOWLClass(self):
-        """ generated source for method testPosOWLClass """
-        cls = OWLClass(iri("A"))
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegOWLClass(self):
-        """ generated source for method testNegOWLClass """
-        cls = OWLObjectComplementOf(OWLClass(iri("A")))
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testPosAllValuesFrom(self):
-        """ generated source for method testPosAllValuesFrom """
-        cls = OWLObjectAllValuesFrom(OWLObjectProperty(iri("p")), OWLClass(iri("A")))
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegAllValuesFrom(self):
-        """ generated source for method testNegAllValuesFrom """
-        property = OWLObjectProperty(iri("p"))
-        filler = OWLClass(iri("A"))
-        all_values_from = OWLObjectAllValuesFrom(property, filler)
-        cls = all_values_from.get_object_complement_of()
-        nnf = OWLObjectSomeValuesFrom(property, filler.get_object_complement_of())
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testPosSomeValuesFrom(self):
-        """ generated source for method testPosSomeValuesFrom """
-        cls = OWLObjectSomeValuesFrom(OWLObjectProperty(iri("p")), OWLClass(iri("A")))
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegSomeValuesFrom(self):
-        """ generated source for method testNegSomeValuesFrom """
-        property = OWLObjectProperty(iri("p"))
-        filler = OWLClass(iri("A"))
-        some_values_from = OWLObjectSomeValuesFrom(property, filler)
-        cls = OWLObjectComplementOf(some_values_from)
-        nnf = OWLObjectAllValuesFrom(property, OWLObjectComplementOf(filler))
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testPosObjectIntersectionOf(self):
-        """ generated source for method testPosObjectIntersectionOf """
-        cls = OWLObjectIntersectionOf((OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C"))))
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegObjectIntersectionOf(self):
-        """ generated source for method testNegObjectIntersectionOf """
-        cls = OWLObjectComplementOf(OWLObjectIntersectionOf(
-            (OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C")))))
-        nnf = OWLObjectUnionOf(
-            (OWLObjectComplementOf(OWLClass(iri("A"))),
-             OWLObjectComplementOf(OWLClass(iri("B"))),
-             OWLObjectComplementOf(OWLClass(iri("C")))))
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testPosObjectUnionOf(self):
-        """ generated source for method testPosObjectUnionOf """
-        cls = OWLObjectUnionOf((OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C"))))
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegObjectUnionOf(self):
-        """ generated source for method testNegObjectUnionOf """
-        cls = OWLObjectComplementOf(OWLObjectUnionOf((OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C")))))
-        nnf = OWLObjectIntersectionOf(
-            (OWLObjectComplementOf(OWLClass(iri("A"))),
-             OWLObjectComplementOf(OWLClass(iri("B"))),
-             OWLObjectComplementOf(OWLClass(iri("C")))))
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testPosObjectMinCardinality(self):
-        """ generated source for method testPosObjectMinCardinality """
-        prop = OWLObjectProperty(iri("p"))
-        filler = OWLClass(iri("A"))
-        cls = OWLObjectMinCardinality(cardinality=3, property=prop, filler=filler)
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegObjectMinCardinality(self):
-        """ generated source for method testNegObjectMinCardinality """
-        prop = OWLObjectProperty(iri("p"))
-        filler = OWLClass(iri("A"))
-        cls = OWLObjectMinCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
-        nnf = OWLObjectMaxCardinality(cardinality=2, property=prop, filler=filler)
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testPosObjectMaxCardinality(self):
-        """ generated source for method testPosObjectMaxCardinality """
-        prop = OWLObjectProperty(iri("p"))
-        filler = OWLClass(iri("A"))
-        cls = OWLObjectMaxCardinality(cardinality=3, property=prop, filler=filler)
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegObjectMaxCardinality(self):
-        """ generated source for method testNegObjectMaxCardinality """
-        prop = OWLObjectProperty(iri("p"))
-        filler = OWLClass(iri("A"))
-        cls = OWLObjectMaxCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
-        nnf = OWLObjectMinCardinality(cardinality=4, property=prop, filler=filler)
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testNamedClass(self):
-        """ generated source for method testNamedClass """
-        desc = self.clsA
-        nnf = self.clsA
-        comp = self.get_nnf(desc)
-        self.assertEqual(nnf, comp)
-
-    def testObjectIntersectionOf(self):
-        """ generated source for method testObjectIntersectionOf """
-        desc = OWLObjectIntersectionOf((self.clsA, self.clsB))
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectUnionOf((OWLObjectComplementOf(self.clsA), OWLObjectComplementOf(self.clsB)))
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testObjectUnionOf(self):
-        """ generated source for method testObjectUnionOf """
-        desc = OWLObjectUnionOf((self.clsA, self.clsB))
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectIntersectionOf((OWLObjectComplementOf(self.clsA), OWLObjectComplementOf(self.clsB)))
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testDoubleNegation(self):
-        """ generated source for method testDoubleNegation """
-        desc = OWLObjectComplementOf(self.clsA)
-        neg = OWLObjectComplementOf(desc)
-        nnf = self.clsA
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testTripleNegation(self):
-        """ generated source for method testTripleNegation """
-        desc = OWLObjectComplementOf(OWLObjectComplementOf(self.clsA))
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectComplementOf(self.clsA)
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testObjectSome(self):
-        """ generated source for method testObjectSome """
-        desc = OWLObjectSomeValuesFrom(self.propP, self.clsA)
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectAllValuesFrom(self.propP, OWLObjectComplementOf(self.clsA))
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testObjectAll(self):
-        """ generated source for method testObjectAll """
-        desc = OWLObjectAllValuesFrom(self.propP, self.clsA)
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectSomeValuesFrom(self.propP, OWLObjectComplementOf(self.clsA))
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testObjectHasValue(self):
-        """ generated source for method testObjectHasValue """
-        desc = OWLObjectHasValue(self.propP, self.indA)
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectAllValuesFrom(self.propP, OWLObjectComplementOf(OWLObjectOneOf(self.indA)))
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testObjectMin(self):
-        """ generated source for method testObjectMin """
-        desc = OWLObjectMinCardinality(cardinality=3, property=self.propP, filler=self.clsA)
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectMaxCardinality(cardinality=2, property=self.propP, filler=self.clsA)
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testObjectMax(self):
-        """ generated source for method testObjectMax """
-        desc = OWLObjectMaxCardinality(cardinality=3, property=self.propP, filler=self.clsA)
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectMinCardinality(cardinality=4, property=self.propP, filler=self.clsA)
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testNestedA(self):
-        """ generated source for method testNestedA """
-        filler_a = OWLObjectUnionOf((self.clsA, self.clsB))
-        op_a = OWLObjectSomeValuesFrom(self.propP, filler_a)
-        op_b = self.clsB
-        desc = OWLObjectUnionOf((op_a, op_b))
-        nnf = OWLObjectIntersectionOf(
-            (OWLObjectComplementOf(self.clsB),
-             OWLObjectAllValuesFrom(self.propP,
-                                    OWLObjectIntersectionOf((OWLObjectComplementOf(self.clsA),
-                                                             OWLObjectComplementOf(self.clsB))))))
-        neg = OWLObjectComplementOf(desc)
-        comp = self.get_nnf(neg)
-        self.assertEqual(comp, nnf)
-
-    def testNestedB(self):
-        """ generated source for method testNestedB """
-        desc = OWLObjectIntersectionOf(
-            (OWLObjectIntersectionOf((self.clsA, self.clsB)),
-             OWLObjectComplementOf(OWLObjectUnionOf((self.clsC, self.clsD)))))
-        neg = OWLObjectComplementOf(desc)
-        nnf = OWLObjectUnionOf(
-            (OWLObjectUnionOf((OWLObjectComplementOf(self.clsA),
-                               OWLObjectComplementOf(self.clsB))),
-             OWLObjectUnionOf((self.clsC, self.clsD))))
-        comp = self.get_nnf(neg)
-        self.assertEqual(comp, nnf)
-
-    def testPosDataAllValuesFrom(self):
-        cls = OWLDataAllValuesFrom(OWLDataProperty(iri("p")), IntegerOWLDatatype)
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegDataAllValuesFrom(self):
-        property = OWLDataProperty(iri("p"))
-        all_values_from = OWLDataAllValuesFrom(property, IntegerOWLDatatype)
-        cls = all_values_from.get_object_complement_of()
-        nnf = OWLDataSomeValuesFrom(property, OWLDataComplementOf(IntegerOWLDatatype))
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testPosDataSomeValuesFrom(self):
-        cls = OWLDataSomeValuesFrom(OWLDataProperty(iri("p")), IntegerOWLDatatype)
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegDataSomeValuesFrom(self):
-        property = OWLDataProperty(iri("p"))
-        some_values_from = OWLDataSomeValuesFrom(property, IntegerOWLDatatype)
-        cls = OWLDataComplementOf(some_values_from)
-        nnf = OWLDataAllValuesFrom(property, OWLDataComplementOf(IntegerOWLDatatype))
-        self.assertEqual(self.get_nnf(cls), nnf)
-
-    def testPosDataIntersectionOf(self):
-        cls = OWLDataIntersectionOf((BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype))
-        self.assertEqual(self.get_nnf(cls), cls)
-
-    def testNegDataIntersectionOf(self):
-        cls = OWLDataComplementOf(OWLDataIntersectionOf(
-            (BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype)))
-        nnf = OWLDataUnionOf(
-            (OWLDataComplementOf(BooleanOWLDatatype),
-             OWLDataComplementOf(DoubleOWLDatatype),
-             OWLDataComplementOf(IntegerOWLDatatype)))
-        self.assertEqual(self.get_nnf(cls), nnf)
-
-    def testPosDataUnionOf(self):
-        cls = OWLDataUnionOf((BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype))
-        self.assertEqual(self.get_nnf(cls), cls)
-
-    def testNegDataUnionOf(self):
-        cls = OWLDataComplementOf(OWLDataUnionOf((BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype)))
-        nnf = OWLDataIntersectionOf(
-            (OWLDataComplementOf(BooleanOWLDatatype),
-             OWLDataComplementOf(DoubleOWLDatatype),
-             OWLDataComplementOf(IntegerOWLDatatype)))
-        self.assertEqual(self.get_nnf(cls), nnf)
-
-    def testPosDataMinCardinality(self):
-        prop = OWLDataProperty(iri("p"))
-        cls = OWLDataMinCardinality(cardinality=3, property=prop, filler=IntegerOWLDatatype)
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegDataMinCardinality(self):
-        prop = OWLDataProperty(iri("p"))
-        filler = IntegerOWLDatatype
-        cls = OWLDataMinCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
-        nnf = OWLDataMaxCardinality(cardinality=2, property=prop, filler=filler)
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testPosDataMaxCardinality(self):
-        prop = OWLDataProperty(iri("p"))
-        cls = OWLDataMaxCardinality(cardinality=3, property=prop, filler=IntegerOWLDatatype)
-        self.assertEqual(cls.get_nnf(), cls)
-
-    def testNegDataMaxCardinality(self):
-        prop = OWLDataProperty(iri("p"))
-        filler = IntegerOWLDatatype
-        cls = OWLDataMaxCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
-        nnf = OWLDataMinCardinality(cardinality=4, property=prop, filler=filler)
-        self.assertEqual(cls.get_nnf(), nnf)
-
-    def testDatatype(self):
-        desc = IntegerOWLDatatype
-        nnf = IntegerOWLDatatype
-        comp = self.get_nnf(desc)
-        self.assertEqual(nnf, comp)
-
-    def testDataDoubleNegation(self):
-        desc = OWLDataComplementOf(IntegerOWLDatatype)
-        neg = OWLDataComplementOf(desc)
-        nnf = IntegerOWLDatatype
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testDataTripleNegation(self):
-        desc = OWLDataComplementOf(OWLDataComplementOf(IntegerOWLDatatype))
-        neg = OWLDataComplementOf(desc)
-        nnf = OWLDataComplementOf(IntegerOWLDatatype)
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testDataHasValue(self):
-        prop = OWLDataProperty(iri("p"))
-        literal = OWLLiteral(5)
-        desc = OWLDataHasValue(prop, literal)
-        neg = OWLDataComplementOf(desc)
-        nnf = OWLDataAllValuesFrom(prop, OWLDataComplementOf(OWLDataOneOf(literal)))
-        comp = self.get_nnf(neg)
-        self.assertEqual(nnf, comp)
-
-    def testDataNestedA(self):
-        restriction = OWLDatatypeMinMaxExclusiveRestriction(5, 6)
-        prop = OWLDataProperty(iri("p"))
-        filler_a = OWLDataUnionOf((IntegerOWLDatatype, DoubleOWLDatatype))
-        op_a = OWLDataSomeValuesFrom(prop, filler_a)
-        op_b = OWLDataIntersectionOf((restriction, IntegerOWLDatatype))
-        desc = OWLDataUnionOf((op_a, op_b))
-        nnf = OWLDataIntersectionOf(
-                (OWLDataAllValuesFrom(prop, OWLDataIntersectionOf((OWLDataComplementOf(DoubleOWLDatatype),
-                                                                   OWLDataComplementOf(IntegerOWLDatatype)))),
-                 OWLDataUnionOf((OWLDataComplementOf(IntegerOWLDatatype), OWLDataComplementOf(restriction)))))
-        neg = OWLDataComplementOf(desc)
-        comp = self.get_nnf(neg)
-        self.assertEqual(comp, nnf)
-
-    def testDataNestedB(self):
-        desc = OWLDataIntersectionOf(
-            (OWLDataIntersectionOf((IntegerOWLDatatype, DoubleOWLDatatype)),
-             OWLDataComplementOf(OWLDataUnionOf((BooleanOWLDatatype, OWLDataOneOf(OWLLiteral(True)))))))
-        neg = OWLDataComplementOf(desc)
-        nnf = OWLDataUnionOf(
-            (OWLDataUnionOf((BooleanOWLDatatype, OWLDataOneOf(OWLLiteral(True)))),
-             OWLDataUnionOf((OWLDataComplementOf(DoubleOWLDatatype),
-                             OWLDataComplementOf(IntegerOWLDatatype)))))
-        comp = self.get_nnf(neg)
-        self.assertEqual(comp, nnf)
+#  This file is part of the OWL API.
+#  * The contents of this file are subject to the LGPL License, Version 3.0.
+#  * Copyright 2014, The University of Manchester
+#
+# * This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public
+# License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any
+# later version. * This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
+# even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public
+# License for more details. * You should have received a copy of the GNU General Public License along with this
+# program.  If not, see http://www.gnu.org/licenses/.
+#
+# * Alternatively, the contents of this file may be used under the terms of the Apache License, Version 2.0 in which
+# case, the provisions of the Apache License Version 2.0 are applicable instead of those above. * Licensed under the
+# Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You
+# may obtain a copy of the License at * http://www.apache.org/licenses/LICENSE-2.0 * Unless required by applicable
+# law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language
+# governing permissions and limitations under the License.
+#
+# package: org.semanticweb.owlapi.api.test.axioms
+#
+#  * @author Matthew Horridge, The University of Manchester, Information Management Group
+#  * @since 3.0.0
+#
+import unittest
+
+from owlapy.class_expression import OWLObjectComplementOf, \
+    OWLObjectAllValuesFrom, OWLObjectSomeValuesFrom, OWLObjectIntersectionOf, OWLObjectUnionOf, \
+    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLClassExpression, \
+    OWLClass, OWLDataAllValuesFrom, \
+    OWLDataSomeValuesFrom, OWLDataHasValue, OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataOneOf
+from owlapy.iri import IRI
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import IntegerOWLDatatype, BooleanOWLDatatype, DoubleOWLDatatype, OWLLiteral
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty
+from owlapy.providers import owl_datatype_min_max_exclusive_restriction
+from owlapy.util import NNF
+
+from owlapy.owl_data_ranges import OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
+from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf
+
+def iri(suffix):
+    NS = "http://example.org/"
+    return IRI.create(NS, suffix)
+
+
+class Owlapy_NNF_Test(unittest.TestCase):
+    """ generated source for class NNFTestCase """
+    clsA = OWLClass(iri("A"))
+    clsB = OWLClass(iri("B"))
+    clsC = OWLClass(iri("C"))
+    clsD = OWLClass(iri("D"))
+    propP = OWLObjectProperty(iri("p"))
+    indA = OWLNamedIndividual(iri("a"))
+
+    def get_nnf(self, ce: OWLClassExpression):
+        return NNF().get_class_nnf(ce)
+
+    def testPosOWLClass(self):
+        """ generated source for method testPosOWLClass """
+        cls = OWLClass(iri("A"))
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegOWLClass(self):
+        """ generated source for method testNegOWLClass """
+        cls = OWLObjectComplementOf(OWLClass(iri("A")))
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testPosAllValuesFrom(self):
+        """ generated source for method testPosAllValuesFrom """
+        cls = OWLObjectAllValuesFrom(OWLObjectProperty(iri("p")), OWLClass(iri("A")))
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegAllValuesFrom(self):
+        """ generated source for method testNegAllValuesFrom """
+        property = OWLObjectProperty(iri("p"))
+        filler = OWLClass(iri("A"))
+        all_values_from = OWLObjectAllValuesFrom(property, filler)
+        cls = all_values_from.get_object_complement_of()
+        nnf = OWLObjectSomeValuesFrom(property, filler.get_object_complement_of())
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testPosSomeValuesFrom(self):
+        """ generated source for method testPosSomeValuesFrom """
+        cls = OWLObjectSomeValuesFrom(OWLObjectProperty(iri("p")), OWLClass(iri("A")))
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegSomeValuesFrom(self):
+        """ generated source for method testNegSomeValuesFrom """
+        property = OWLObjectProperty(iri("p"))
+        filler = OWLClass(iri("A"))
+        some_values_from = OWLObjectSomeValuesFrom(property, filler)
+        cls = OWLObjectComplementOf(some_values_from)
+        nnf = OWLObjectAllValuesFrom(property, OWLObjectComplementOf(filler))
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testPosObjectIntersectionOf(self):
+        """ generated source for method testPosObjectIntersectionOf """
+        cls = OWLObjectIntersectionOf((OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C"))))
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegObjectIntersectionOf(self):
+        """ generated source for method testNegObjectIntersectionOf """
+        cls = OWLObjectComplementOf(OWLObjectIntersectionOf(
+            (OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C")))))
+        nnf = OWLObjectUnionOf(
+            (OWLObjectComplementOf(OWLClass(iri("A"))),
+             OWLObjectComplementOf(OWLClass(iri("B"))),
+             OWLObjectComplementOf(OWLClass(iri("C")))))
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testPosObjectUnionOf(self):
+        """ generated source for method testPosObjectUnionOf """
+        cls = OWLObjectUnionOf((OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C"))))
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegObjectUnionOf(self):
+        """ generated source for method testNegObjectUnionOf """
+        cls = OWLObjectComplementOf(OWLObjectUnionOf((OWLClass(iri("A")), OWLClass(iri("B")), OWLClass(iri("C")))))
+        nnf = OWLObjectIntersectionOf(
+            (OWLObjectComplementOf(OWLClass(iri("A"))),
+             OWLObjectComplementOf(OWLClass(iri("B"))),
+             OWLObjectComplementOf(OWLClass(iri("C")))))
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testPosObjectMinCardinality(self):
+        """ generated source for method testPosObjectMinCardinality """
+        prop = OWLObjectProperty(iri("p"))
+        filler = OWLClass(iri("A"))
+        cls = OWLObjectMinCardinality(cardinality=3, property=prop, filler=filler)
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegObjectMinCardinality(self):
+        """ generated source for method testNegObjectMinCardinality """
+        prop = OWLObjectProperty(iri("p"))
+        filler = OWLClass(iri("A"))
+        cls = OWLObjectMinCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
+        nnf = OWLObjectMaxCardinality(cardinality=2, property=prop, filler=filler)
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testPosObjectMaxCardinality(self):
+        """ generated source for method testPosObjectMaxCardinality """
+        prop = OWLObjectProperty(iri("p"))
+        filler = OWLClass(iri("A"))
+        cls = OWLObjectMaxCardinality(cardinality=3, property=prop, filler=filler)
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegObjectMaxCardinality(self):
+        """ generated source for method testNegObjectMaxCardinality """
+        prop = OWLObjectProperty(iri("p"))
+        filler = OWLClass(iri("A"))
+        cls = OWLObjectMaxCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
+        nnf = OWLObjectMinCardinality(cardinality=4, property=prop, filler=filler)
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testNamedClass(self):
+        """ generated source for method testNamedClass """
+        desc = self.clsA
+        nnf = self.clsA
+        comp = self.get_nnf(desc)
+        self.assertEqual(nnf, comp)
+
+    def testObjectIntersectionOf(self):
+        """ generated source for method testObjectIntersectionOf """
+        desc = OWLObjectIntersectionOf((self.clsA, self.clsB))
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectUnionOf((OWLObjectComplementOf(self.clsA), OWLObjectComplementOf(self.clsB)))
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testObjectUnionOf(self):
+        """ generated source for method testObjectUnionOf """
+        desc = OWLObjectUnionOf((self.clsA, self.clsB))
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectIntersectionOf((OWLObjectComplementOf(self.clsA), OWLObjectComplementOf(self.clsB)))
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testDoubleNegation(self):
+        """ generated source for method testDoubleNegation """
+        desc = OWLObjectComplementOf(self.clsA)
+        neg = OWLObjectComplementOf(desc)
+        nnf = self.clsA
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testTripleNegation(self):
+        """ generated source for method testTripleNegation """
+        desc = OWLObjectComplementOf(OWLObjectComplementOf(self.clsA))
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectComplementOf(self.clsA)
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testObjectSome(self):
+        """ generated source for method testObjectSome """
+        desc = OWLObjectSomeValuesFrom(self.propP, self.clsA)
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectAllValuesFrom(self.propP, OWLObjectComplementOf(self.clsA))
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testObjectAll(self):
+        """ generated source for method testObjectAll """
+        desc = OWLObjectAllValuesFrom(self.propP, self.clsA)
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectSomeValuesFrom(self.propP, OWLObjectComplementOf(self.clsA))
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testObjectHasValue(self):
+        """ generated source for method testObjectHasValue """
+        desc = OWLObjectHasValue(self.propP, self.indA)
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectAllValuesFrom(self.propP, OWLObjectComplementOf(OWLObjectOneOf(self.indA)))
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testObjectMin(self):
+        """ generated source for method testObjectMin """
+        desc = OWLObjectMinCardinality(cardinality=3, property=self.propP, filler=self.clsA)
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectMaxCardinality(cardinality=2, property=self.propP, filler=self.clsA)
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testObjectMax(self):
+        """ generated source for method testObjectMax """
+        desc = OWLObjectMaxCardinality(cardinality=3, property=self.propP, filler=self.clsA)
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectMinCardinality(cardinality=4, property=self.propP, filler=self.clsA)
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testNestedA(self):
+        """ generated source for method testNestedA """
+        filler_a = OWLObjectUnionOf((self.clsA, self.clsB))
+        op_a = OWLObjectSomeValuesFrom(self.propP, filler_a)
+        op_b = self.clsB
+        desc = OWLObjectUnionOf((op_a, op_b))
+        nnf = OWLObjectIntersectionOf(
+            (OWLObjectComplementOf(self.clsB),
+             OWLObjectAllValuesFrom(self.propP,
+                                    OWLObjectIntersectionOf((OWLObjectComplementOf(self.clsA),
+                                                             OWLObjectComplementOf(self.clsB))))))
+        neg = OWLObjectComplementOf(desc)
+        comp = self.get_nnf(neg)
+        self.assertEqual(comp, nnf)
+
+    def testNestedB(self):
+        """ generated source for method testNestedB """
+        desc = OWLObjectIntersectionOf(
+            (OWLObjectIntersectionOf((self.clsA, self.clsB)),
+             OWLObjectComplementOf(OWLObjectUnionOf((self.clsC, self.clsD)))))
+        neg = OWLObjectComplementOf(desc)
+        nnf = OWLObjectUnionOf(
+            (OWLObjectUnionOf((OWLObjectComplementOf(self.clsA),
+                               OWLObjectComplementOf(self.clsB))),
+             OWLObjectUnionOf((self.clsC, self.clsD))))
+        comp = self.get_nnf(neg)
+        self.assertEqual(comp, nnf)
+
+    def testPosDataAllValuesFrom(self):
+        cls = OWLDataAllValuesFrom(OWLDataProperty(iri("p")), IntegerOWLDatatype)
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegDataAllValuesFrom(self):
+        property = OWLDataProperty(iri("p"))
+        all_values_from = OWLDataAllValuesFrom(property, IntegerOWLDatatype)
+        cls = all_values_from.get_object_complement_of()
+        nnf = OWLDataSomeValuesFrom(property, OWLDataComplementOf(IntegerOWLDatatype))
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testPosDataSomeValuesFrom(self):
+        cls = OWLDataSomeValuesFrom(OWLDataProperty(iri("p")), IntegerOWLDatatype)
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegDataSomeValuesFrom(self):
+        property = OWLDataProperty(iri("p"))
+        some_values_from = OWLDataSomeValuesFrom(property, IntegerOWLDatatype)
+        cls = OWLDataComplementOf(some_values_from)
+        nnf = OWLDataAllValuesFrom(property, OWLDataComplementOf(IntegerOWLDatatype))
+        self.assertEqual(self.get_nnf(cls), nnf)
+
+    def testPosDataIntersectionOf(self):
+        cls = OWLDataIntersectionOf((BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype))
+        self.assertEqual(self.get_nnf(cls), cls)
+
+    def testNegDataIntersectionOf(self):
+        cls = OWLDataComplementOf(OWLDataIntersectionOf(
+            (BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype)))
+        nnf = OWLDataUnionOf(
+            (OWLDataComplementOf(BooleanOWLDatatype),
+             OWLDataComplementOf(DoubleOWLDatatype),
+             OWLDataComplementOf(IntegerOWLDatatype)))
+        self.assertEqual(self.get_nnf(cls), nnf)
+
+    def testPosDataUnionOf(self):
+        cls = OWLDataUnionOf((BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype))
+        self.assertEqual(self.get_nnf(cls), cls)
+
+    def testNegDataUnionOf(self):
+        cls = OWLDataComplementOf(OWLDataUnionOf((BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype)))
+        nnf = OWLDataIntersectionOf(
+            (OWLDataComplementOf(BooleanOWLDatatype),
+             OWLDataComplementOf(DoubleOWLDatatype),
+             OWLDataComplementOf(IntegerOWLDatatype)))
+        self.assertEqual(self.get_nnf(cls), nnf)
+
+    def testPosDataMinCardinality(self):
+        prop = OWLDataProperty(iri("p"))
+        cls = OWLDataMinCardinality(cardinality=3, property=prop, filler=IntegerOWLDatatype)
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegDataMinCardinality(self):
+        prop = OWLDataProperty(iri("p"))
+        filler = IntegerOWLDatatype
+        cls = OWLDataMinCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
+        nnf = OWLDataMaxCardinality(cardinality=2, property=prop, filler=filler)
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testPosDataMaxCardinality(self):
+        prop = OWLDataProperty(iri("p"))
+        cls = OWLDataMaxCardinality(cardinality=3, property=prop, filler=IntegerOWLDatatype)
+        self.assertEqual(cls.get_nnf(), cls)
+
+    def testNegDataMaxCardinality(self):
+        prop = OWLDataProperty(iri("p"))
+        filler = IntegerOWLDatatype
+        cls = OWLDataMaxCardinality(cardinality=3, property=prop, filler=filler).get_object_complement_of()
+        nnf = OWLDataMinCardinality(cardinality=4, property=prop, filler=filler)
+        self.assertEqual(cls.get_nnf(), nnf)
+
+    def testDatatype(self):
+        desc = IntegerOWLDatatype
+        nnf = IntegerOWLDatatype
+        comp = self.get_nnf(desc)
+        self.assertEqual(nnf, comp)
+
+    def testDataDoubleNegation(self):
+        desc = OWLDataComplementOf(IntegerOWLDatatype)
+        neg = OWLDataComplementOf(desc)
+        nnf = IntegerOWLDatatype
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testDataTripleNegation(self):
+        desc = OWLDataComplementOf(OWLDataComplementOf(IntegerOWLDatatype))
+        neg = OWLDataComplementOf(desc)
+        nnf = OWLDataComplementOf(IntegerOWLDatatype)
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testDataHasValue(self):
+        prop = OWLDataProperty(iri("p"))
+        literal = OWLLiteral(5)
+        desc = OWLDataHasValue(prop, literal)
+        neg = OWLDataComplementOf(desc)
+        nnf = OWLDataAllValuesFrom(prop, OWLDataComplementOf(OWLDataOneOf(literal)))
+        comp = self.get_nnf(neg)
+        self.assertEqual(nnf, comp)
+
+    def testDataNestedA(self):
+        restriction = owl_datatype_min_max_exclusive_restriction(5, 6)
+        prop = OWLDataProperty(iri("p"))
+        filler_a = OWLDataUnionOf((IntegerOWLDatatype, DoubleOWLDatatype))
+        op_a = OWLDataSomeValuesFrom(prop, filler_a)
+        op_b = OWLDataIntersectionOf((restriction, IntegerOWLDatatype))
+        desc = OWLDataUnionOf((op_a, op_b))
+        nnf = OWLDataIntersectionOf(
+                (OWLDataAllValuesFrom(prop, OWLDataIntersectionOf((OWLDataComplementOf(DoubleOWLDatatype),
+                                                                   OWLDataComplementOf(IntegerOWLDatatype)))),
+                 OWLDataUnionOf((OWLDataComplementOf(IntegerOWLDatatype), OWLDataComplementOf(restriction)))))
+        neg = OWLDataComplementOf(desc)
+        comp = self.get_nnf(neg)
+        self.assertEqual(comp, nnf)
+
+    def testDataNestedB(self):
+        desc = OWLDataIntersectionOf(
+            (OWLDataIntersectionOf((IntegerOWLDatatype, DoubleOWLDatatype)),
+             OWLDataComplementOf(OWLDataUnionOf((BooleanOWLDatatype, OWLDataOneOf(OWLLiteral(True)))))))
+        neg = OWLDataComplementOf(desc)
+        nnf = OWLDataUnionOf(
+            (OWLDataUnionOf((BooleanOWLDatatype, OWLDataOneOf(OWLLiteral(True)))),
+             OWLDataUnionOf((OWLDataComplementOf(DoubleOWLDatatype),
+                             OWLDataComplementOf(IntegerOWLDatatype)))))
+        comp = self.get_nnf(neg)
+        self.assertEqual(comp, nnf)
```

### Comparing `owlapy-0.1.3/tests/test_owlapy_render.py` & `owlapy-1.0.0/tests/test_owlapy_render.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,188 +1,191 @@
-import unittest
-from owlapy.owl_property import OWLObjectProperty
-from owlapy.model import OWLDataMinCardinality, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom, \
-    OWLThing, OWLObjectComplementOf, OWLObjectUnionOf, OWLNamedIndividual, OWLObjectMinCardinality, IRI, OWLDataProperty, DoubleOWLDatatype, OWLClass, \
-    IntegerOWLDatatype, OWLDataExactCardinality, OWLDataHasValue, OWLDataAllValuesFrom, \
-    OWLDataOneOf, OWLDataSomeValuesFrom, OWLLiteral, BooleanOWLDatatype, \
-    OWLDataMaxCardinality
-
-from owlapy.data_ranges import OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
-from owlapy.model.providers import OWLDatatypeMinMaxInclusiveRestriction
-from owlapy.render import DLSyntaxObjectRenderer, ManchesterOWLSyntaxOWLObjectRenderer
-from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf
-
-class Owlapy_DLRenderer_Test(unittest.TestCase):
-    def test_ce_render(self):
-        renderer = DLSyntaxObjectRenderer()
-        NS = "http://example.com/father#"
-
-        male = OWLClass(IRI.create(NS, 'male'))
-        female = OWLClass(IRI.create(NS, 'female'))
-        has_child = OWLObjectProperty(IRI(NS, 'hasChild'))
-        has_age = OWLDataProperty(IRI(NS, 'hasAge'))
-
-        c = OWLObjectUnionOf((male, OWLObjectSomeValuesFrom(property=has_child, filler=female)))
-        r = renderer.render(c)
-        print(r)
-        self.assertEqual(r, "male ⊔ (∃ hasChild.female)")
-        c = OWLObjectComplementOf(OWLObjectIntersectionOf((female,
-                                                           OWLObjectSomeValuesFrom(property=has_child,
-                                                                                   filler=OWLThing))))
-        r = renderer.render(c)
-        print(r)
-        self.assertEqual(r, "¬(female ⊓ (∃ hasChild.⊤))")
-        c = OWLObjectSomeValuesFrom(property=has_child,
-                                    filler=OWLObjectSomeValuesFrom(property=has_child,
-                                                                   filler=OWLObjectSomeValuesFrom(property=has_child,
-                                                                                                  filler=OWLThing)))
-        r = renderer.render(c)
-        print(r)
-        self.assertEqual(r, "∃ hasChild.(∃ hasChild.(∃ hasChild.⊤))")
-
-        i1 = OWLNamedIndividual(IRI.create(NS, 'heinz'))
-        i2 = OWLNamedIndividual(IRI.create(NS, 'marie'))
-        oneof = OWLObjectOneOf((i1, i2))
-        r = renderer.render(oneof)
-        print(r)
-
-        self.assertEqual(r, "{heinz , marie}")
-
-        hasvalue = OWLObjectHasValue(property=has_child, individual=i1)
-        r = renderer.render(hasvalue)
-        print(r)
-        self.assertEqual(r, "∃ hasChild.{heinz}")
-
-        mincard = OWLObjectMinCardinality(cardinality=2, property=has_child, filler=OWLThing)
-        r = renderer.render(mincard)
-        print(r)
-        self.assertEqual(r, "≥ 2 hasChild.⊤")
-
-        d = OWLDataSomeValuesFrom(property=has_age,
-                                  filler=OWLDataComplementOf(DoubleOWLDatatype))
-        r = renderer.render(d)
-        print(r)
-        self.assertEqual(r, "∃ hasAge.¬xsd:double")
-
-        datatype_restriction = OWLDatatypeMinMaxInclusiveRestriction(40, 80)
-
-        dr = OWLDataAllValuesFrom(property=has_age, filler=OWLDataUnionOf([datatype_restriction, IntegerOWLDatatype]))
-        r = renderer.render(dr)
-        print(r)
-        self.assertEqual(r, "∀ hasAge.(xsd:integer[≥ 40 , ≤ 80] ⊔ xsd:integer)")
-
-        dr = OWLDataSomeValuesFrom(property=has_age,
-                                   filler=OWLDataIntersectionOf([OWLDataOneOf([OWLLiteral(32.5), OWLLiteral(4.5)]),
-                                                                 IntegerOWLDatatype]))
-        r = renderer.render(dr)
-        print(r)
-        self.assertEqual(r, "∃ hasAge.({32.5 ⊔ 4.5} ⊓ xsd:integer)")
-
-        hasvalue = OWLDataHasValue(property=has_age, value=OWLLiteral(50))
-        r = renderer.render(hasvalue)
-        print(r)
-        self.assertEqual(r, "∃ hasAge.{50}")
-
-        exactcard = OWLDataExactCardinality(cardinality=1, property=has_age, filler=IntegerOWLDatatype)
-        r = renderer.render(exactcard)
-        print(r)
-        self.assertEqual(r, "= 1 hasAge.xsd:integer")
-
-        maxcard = OWLDataMaxCardinality(cardinality=4, property=has_age, filler=DoubleOWLDatatype)
-        r = renderer.render(maxcard)
-        print(r)
-        self.assertEqual(r, "≤ 4 hasAge.xsd:double")
-
-        mincard = OWLDataMinCardinality(cardinality=7, property=has_age, filler=BooleanOWLDatatype)
-        r = renderer.render(mincard)
-        print(r)
-        self.assertEqual(r, "≥ 7 hasAge.xsd:boolean")
-
-
-class Owlapy_ManchesterRenderer_Test(unittest.TestCase):
-    def test_ce_render(self):
-        renderer = ManchesterOWLSyntaxOWLObjectRenderer()
-        NS = "http://example.com/father#"
-
-        male = OWLClass(IRI.create(NS, 'male'))
-        female = OWLClass(IRI.create(NS, 'female'))
-        has_child = OWLObjectProperty(IRI(NS, 'hasChild'))
-        has_age = OWLDataProperty(IRI(NS, 'hasAge'))
-
-        c = OWLObjectUnionOf((male, OWLObjectSomeValuesFrom(property=has_child, filler=female)))
-        r = renderer.render(c)
-        print(r)
-        self.assertEqual(r, "male or (hasChild some female)")
-        c = OWLObjectComplementOf(OWLObjectIntersectionOf((female,
-                                                           OWLObjectSomeValuesFrom(property=has_child,
-                                                                                   filler=OWLThing))))
-        r = renderer.render(c)
-        print(r)
-        self.assertEqual(r, "not (female and (hasChild some Thing))")
-        c = OWLObjectSomeValuesFrom(property=has_child,
-                                    filler=OWLObjectSomeValuesFrom(property=has_child,
-                                                                   filler=OWLObjectSomeValuesFrom(property=has_child,
-                                                                                                  filler=OWLThing)))
-        r = renderer.render(c)
-        print(r)
-        self.assertEqual(r, "hasChild some (hasChild some (hasChild some Thing))")
-
-        i1 = OWLNamedIndividual(IRI.create(NS, 'heinz'))
-        i2 = OWLNamedIndividual(IRI.create(NS, 'marie'))
-        oneof = OWLObjectOneOf((i1, i2))
-        r = renderer.render(oneof)
-        print(r)
-        self.assertEqual(r, "{heinz , marie}")
-
-        hasvalue = OWLObjectHasValue(property=has_child, individual=i1)
-        r = renderer.render(hasvalue)
-        print(r)
-        self.assertEqual(r, "hasChild value heinz")
-
-        mincard = OWLObjectMinCardinality(cardinality=2, property=has_child, filler=OWLThing)
-        r = renderer.render(mincard)
-        print(r)
-        self.assertEqual(r, "hasChild min 2 Thing")
-
-        d = OWLDataSomeValuesFrom(property=has_age,
-                                  filler=OWLDataComplementOf(DoubleOWLDatatype))
-        r = renderer.render(d)
-        print(r)
-        self.assertEqual(r, "hasAge some not xsd:double")
-
-        datatype_restriction = OWLDatatypeMinMaxInclusiveRestriction(40, 80)
-
-        dr = OWLDataAllValuesFrom(property=has_age, filler=OWLDataUnionOf([datatype_restriction, IntegerOWLDatatype]))
-        r = renderer.render(dr)
-        print(r)
-        self.assertEqual(r, "hasAge only (xsd:integer[>= 40 , <= 80] or xsd:integer)")
-
-        dr = OWLDataSomeValuesFrom(property=has_age,
-                                   filler=OWLDataIntersectionOf([OWLDataOneOf([OWLLiteral(32.5), OWLLiteral(4.5)]),
-                                                                 IntegerOWLDatatype]))
-        r = renderer.render(dr)
-        print(r)
-        self.assertEqual(r, "hasAge some ({32.5 , 4.5} and xsd:integer)")
-
-        hasvalue = OWLDataHasValue(property=has_age, value=OWLLiteral(50))
-        r = renderer.render(hasvalue)
-        print(r)
-        self.assertEqual(r, "hasAge value 50")
-
-        maxcard = OWLDataExactCardinality(cardinality=1, property=has_age, filler=IntegerOWLDatatype)
-        r = renderer.render(maxcard)
-        print(r)
-        self.assertEqual(r, "hasAge exactly 1 xsd:integer")
-
-        maxcard = OWLDataMaxCardinality(cardinality=4, property=has_age, filler=DoubleOWLDatatype)
-        r = renderer.render(maxcard)
-        print(r)
-        self.assertEqual(r, "hasAge max 4 xsd:double")
-
-        mincard = OWLDataMinCardinality(cardinality=7, property=has_age, filler=BooleanOWLDatatype)
-        r = renderer.render(mincard)
-        print(r)
-        self.assertEqual(r, "hasAge min 7 xsd:boolean")
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from owlapy.iri import IRI
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import DoubleOWLDatatype, IntegerOWLDatatype, OWLLiteral, BooleanOWLDatatype
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty
+from owlapy.class_expression import OWLDataMinCardinality, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom, \
+    OWLThing, OWLObjectComplementOf, OWLObjectUnionOf, OWLObjectMinCardinality, OWLClass, \
+    OWLDataExactCardinality, OWLDataHasValue, OWLDataAllValuesFrom, \
+    OWLDataOneOf, OWLDataSomeValuesFrom, \
+    OWLDataMaxCardinality, OWLObjectHasValue, OWLObjectOneOf
+
+from owlapy.owl_data_ranges import OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
+from owlapy.providers import owl_datatype_min_max_inclusive_restriction
+from owlapy.render import DLSyntaxObjectRenderer, ManchesterOWLSyntaxOWLObjectRenderer
+
+class Owlapy_DLRenderer_Test(unittest.TestCase):
+    def test_ce_render(self):
+        renderer = DLSyntaxObjectRenderer()
+        NS = "http://example.com/father#"
+
+        male = OWLClass(IRI.create(NS, 'male'))
+        female = OWLClass(IRI.create(NS, 'female'))
+        has_child = OWLObjectProperty(IRI(NS, 'hasChild'))
+        has_age = OWLDataProperty(IRI(NS, 'hasAge'))
+
+        c = OWLObjectUnionOf((male, OWLObjectSomeValuesFrom(property=has_child, filler=female)))
+        r = renderer.render(c)
+        print(r)
+        self.assertEqual(r, "male ⊔ (∃ hasChild.female)")
+        c = OWLObjectComplementOf(OWLObjectIntersectionOf((female,
+                                                           OWLObjectSomeValuesFrom(property=has_child,
+                                                                                   filler=OWLThing))))
+        r = renderer.render(c)
+        print(r)
+        self.assertEqual(r, "¬(female ⊓ (∃ hasChild.⊤))")
+        c = OWLObjectSomeValuesFrom(property=has_child,
+                                    filler=OWLObjectSomeValuesFrom(property=has_child,
+                                                                   filler=OWLObjectSomeValuesFrom(property=has_child,
+                                                                                                  filler=OWLThing)))
+        r = renderer.render(c)
+        print(r)
+        self.assertEqual(r, "∃ hasChild.(∃ hasChild.(∃ hasChild.⊤))")
+
+        i1 = OWLNamedIndividual(IRI.create(NS, 'heinz'))
+        i2 = OWLNamedIndividual(IRI.create(NS, 'marie'))
+        oneof = OWLObjectOneOf((i1, i2))
+        r = renderer.render(oneof)
+        print(r)
+
+        self.assertEqual(r, "{heinz , marie}")
+
+        hasvalue = OWLObjectHasValue(property=has_child, individual=i1)
+        r = renderer.render(hasvalue)
+        print(r)
+        self.assertEqual(r, "∃ hasChild.{heinz}")
+
+        mincard = OWLObjectMinCardinality(cardinality=2, property=has_child, filler=OWLThing)
+        r = renderer.render(mincard)
+        print(r)
+        self.assertEqual(r, "≥ 2 hasChild.⊤")
+
+        d = OWLDataSomeValuesFrom(property=has_age,
+                                  filler=OWLDataComplementOf(DoubleOWLDatatype))
+        r = renderer.render(d)
+        print(r)
+        self.assertEqual(r, "∃ hasAge.¬xsd:double")
+
+        datatype_restriction = owl_datatype_min_max_inclusive_restriction(40, 80)
+
+        dr = OWLDataAllValuesFrom(property=has_age, filler=OWLDataUnionOf([datatype_restriction, IntegerOWLDatatype]))
+        r = renderer.render(dr)
+        print(r)
+        self.assertEqual(r, "∀ hasAge.(xsd:integer[≥ 40 , ≤ 80] ⊔ xsd:integer)")
+
+        dr = OWLDataSomeValuesFrom(property=has_age,
+                                   filler=OWLDataIntersectionOf([OWLDataOneOf([OWLLiteral(32.5), OWLLiteral(4.5)]),
+                                                                 IntegerOWLDatatype]))
+        r = renderer.render(dr)
+        print(r)
+        self.assertEqual(r, "∃ hasAge.({32.5 ⊔ 4.5} ⊓ xsd:integer)")
+
+        hasvalue = OWLDataHasValue(property=has_age, value=OWLLiteral(50))
+        r = renderer.render(hasvalue)
+        print(r)
+        self.assertEqual(r, "∃ hasAge.{50}")
+
+        exactcard = OWLDataExactCardinality(cardinality=1, property=has_age, filler=IntegerOWLDatatype)
+        r = renderer.render(exactcard)
+        print(r)
+        self.assertEqual(r, "= 1 hasAge.xsd:integer")
+
+        maxcard = OWLDataMaxCardinality(cardinality=4, property=has_age, filler=DoubleOWLDatatype)
+        r = renderer.render(maxcard)
+        print(r)
+        self.assertEqual(r, "≤ 4 hasAge.xsd:double")
+
+        mincard = OWLDataMinCardinality(cardinality=7, property=has_age, filler=BooleanOWLDatatype)
+        r = renderer.render(mincard)
+        print(r)
+        self.assertEqual(r, "≥ 7 hasAge.xsd:boolean")
+
+
+class Owlapy_ManchesterRenderer_Test(unittest.TestCase):
+    def test_ce_render(self):
+        renderer = ManchesterOWLSyntaxOWLObjectRenderer()
+        NS = "http://example.com/father#"
+
+        male = OWLClass(IRI.create(NS, 'male'))
+        female = OWLClass(IRI.create(NS, 'female'))
+        has_child = OWLObjectProperty(IRI(NS, 'hasChild'))
+        has_age = OWLDataProperty(IRI(NS, 'hasAge'))
+
+        c = OWLObjectUnionOf((male, OWLObjectSomeValuesFrom(property=has_child, filler=female)))
+        r = renderer.render(c)
+        print(r)
+        self.assertEqual(r, "male or (hasChild some female)")
+        c = OWLObjectComplementOf(OWLObjectIntersectionOf((female,
+                                                           OWLObjectSomeValuesFrom(property=has_child,
+                                                                                   filler=OWLThing))))
+        r = renderer.render(c)
+        print(r)
+        self.assertEqual(r, "not (female and (hasChild some Thing))")
+        c = OWLObjectSomeValuesFrom(property=has_child,
+                                    filler=OWLObjectSomeValuesFrom(property=has_child,
+                                                                   filler=OWLObjectSomeValuesFrom(property=has_child,
+                                                                                                  filler=OWLThing)))
+        r = renderer.render(c)
+        print(r)
+        self.assertEqual(r, "hasChild some (hasChild some (hasChild some Thing))")
+
+        i1 = OWLNamedIndividual(IRI.create(NS, 'heinz'))
+        i2 = OWLNamedIndividual(IRI.create(NS, 'marie'))
+        oneof = OWLObjectOneOf((i1, i2))
+        r = renderer.render(oneof)
+        print(r)
+        self.assertEqual(r, "{heinz , marie}")
+
+        hasvalue = OWLObjectHasValue(property=has_child, individual=i1)
+        r = renderer.render(hasvalue)
+        print(r)
+        self.assertEqual(r, "hasChild value heinz")
+
+        mincard = OWLObjectMinCardinality(cardinality=2, property=has_child, filler=OWLThing)
+        r = renderer.render(mincard)
+        print(r)
+        self.assertEqual(r, "hasChild min 2 Thing")
+
+        d = OWLDataSomeValuesFrom(property=has_age,
+                                  filler=OWLDataComplementOf(DoubleOWLDatatype))
+        r = renderer.render(d)
+        print(r)
+        self.assertEqual(r, "hasAge some not xsd:double")
+
+        datatype_restriction = owl_datatype_min_max_inclusive_restriction(40, 80)
+
+        dr = OWLDataAllValuesFrom(property=has_age, filler=OWLDataUnionOf([datatype_restriction, IntegerOWLDatatype]))
+        r = renderer.render(dr)
+        print(r)
+        self.assertEqual(r, "hasAge only (xsd:integer[>= 40 , <= 80] or xsd:integer)")
+
+        dr = OWLDataSomeValuesFrom(property=has_age,
+                                   filler=OWLDataIntersectionOf([OWLDataOneOf([OWLLiteral(32.5), OWLLiteral(4.5)]),
+                                                                 IntegerOWLDatatype]))
+        r = renderer.render(dr)
+        print(r)
+        self.assertEqual(r, "hasAge some ({32.5 , 4.5} and xsd:integer)")
+
+        hasvalue = OWLDataHasValue(property=has_age, value=OWLLiteral(50))
+        r = renderer.render(hasvalue)
+        print(r)
+        self.assertEqual(r, "hasAge value 50")
+
+        maxcard = OWLDataExactCardinality(cardinality=1, property=has_age, filler=IntegerOWLDatatype)
+        r = renderer.render(maxcard)
+        print(r)
+        self.assertEqual(r, "hasAge exactly 1 xsd:integer")
+
+        maxcard = OWLDataMaxCardinality(cardinality=4, property=has_age, filler=DoubleOWLDatatype)
+        r = renderer.render(maxcard)
+        print(r)
+        self.assertEqual(r, "hasAge max 4 xsd:double")
+
+        mincard = OWLDataMinCardinality(cardinality=7, property=has_age, filler=BooleanOWLDatatype)
+        r = renderer.render(mincard)
+        print(r)
+        self.assertEqual(r, "hasAge min 7 xsd:boolean")
+
+
+if __name__ == '__main__':
+    unittest.main()
```

