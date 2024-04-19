# Comparing `tmp/atomrdf-0.4.4.tar.gz` & `tmp/atomrdf-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomrdf-0.4.4.tar", last modified: Mon Apr 15 10:37:58 2024, max compression
+gzip compressed data, was "atomrdf-0.6.0.tar", last modified: Fri Apr 19 14:49:53 2024, max compression
```

## Comparing `atomrdf-0.4.4.tar` & `atomrdf-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:58.361899 atomrdf-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 10:37:55.000000 atomrdf-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 10:37:55.000000 atomrdf-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 10:37:58.361899 atomrdf-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 10:37:55.000000 atomrdf-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:58.353899 atomrdf-0.4.4/atomrdf/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:58.357899 atomrdf-0.4.4/atomrdf/data/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/data/asmo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/data/cmso.owl
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/data/element.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/data/pldo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/data/podo.owl
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/json_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:58.357899 atomrdf-0.4.4/atomrdf/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/network/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/network/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/network/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    37476 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:58.357899 atomrdf-0.4.4/atomrdf/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/workflow/pyiron.py
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-04-15 10:37:55.000000 atomrdf-0.4.4/atomrdf/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:58.357899 atomrdf-0.4.4/atomrdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-15 10:37:58.000000 atomrdf-0.4.4/atomrdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 10:37:58.000000 atomrdf-0.4.4/atomrdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:37:58.000000 atomrdf-0.4.4/atomrdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:37:58.000000 atomrdf-0.4.4/atomrdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 10:37:58.000000 atomrdf-0.4.4/atomrdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 10:37:58.000000 atomrdf-0.4.4/atomrdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:37:58.361899 atomrdf-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 10:37:58.000000 atomrdf-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:37:58.357899 atomrdf-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 10:37:55.000000 atomrdf-0.4.4/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-15 10:37:55.000000 atomrdf-0.4.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 10:37:55.000000 atomrdf-0.4.4/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.227151 atomrdf-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 14:49:50.000000 atomrdf-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 14:49:50.000000 atomrdf-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-19 14:49:53.227151 atomrdf-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-19 14:49:50.000000 atomrdf-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.219151 atomrdf-0.6.0/atomrdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.223151 atomrdf-0.6.0/atomrdf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    52930 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/asmo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/cmso.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/dft_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/md_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/pldo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/data/podo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38627 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.223151 atomrdf-0.6.0/atomrdf/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/network/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59158 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.223151 atomrdf-0.6.0/atomrdf/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/workflow/pyiron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-04-19 14:49:50.000000 atomrdf-0.6.0/atomrdf/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.227151 atomrdf-0.6.0/atomrdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 14:49:53.000000 atomrdf-0.6.0/atomrdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:49:53.227151 atomrdf-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 14:49:52.000000 atomrdf-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:53.227151 atomrdf-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_structuregraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 14:49:50.000000 atomrdf-0.6.0/tests/test_workflow.py
```

### Comparing `atomrdf-0.4.4/LICENSE` & `atomrdf-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.4/PKG-INFO` & `atomrdf-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.4.4
+Version: 0.6.0
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -21,14 +21,18 @@
 Requires-Dist: owlready2
 
 # atomRDF
 
 > [!NOTE]
 > `atomRDF` was previously called `pyscal-rdf`. 
 
+[![codecov](https://codecov.io/gh/pyscal/atomRDF/graph/badge.svg?token=X7S3TP2MP6)](https://codecov.io/gh/pyscal/atomRDF)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/atomrdf.svg)](https://anaconda.org/conda-forge/atomrdf)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atomrdf?label=pypi&link=https%3A%2F%2Fpypi.org%2Fproject%2Fatomrdf%2F)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10973374.svg)](https://doi.org/10.5281/zenodo.10973374)
 
 `atomRDF` is a python tool for ontology-based creation, manipulation, and quering of structures. `atomRDF` uses the [Computational Material Sample Ontology (CMSO)](https://github.com/Materials-Data-Science-and-Informatics/cmso-ontology). 
 
 The package is currently under activate development and could be  unstable .
 
 More details coming soon...
```

### Comparing `atomrdf-0.4.4/atomrdf/data/asmo.owl` & `atomrdf-0.6.0/atomrdf/data/asmo.owl`

 * *Files 0% similar despite different names*

#### Comparing `atomrdf-0.4.4/atomrdf/data/asmo.owl` & `atomrdf-0.6.0/atomrdf/data/asmo.owl`

```diff
@@ -1,14 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/asmo/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:prov="http://www.w3.org/ns/prov#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/asmo/">
   <owl:Ontology rdf:about="http://purls.helmholtz-metadaten.de/asmo/">
     <terms:contributor>https://orcid.org/0000-0002-6776-1213</terms:contributor>
     <terms:creator>https://orcid.org/0000-0001-7564-7990</terms:creator>
     <terms:description>ASMO is an ontology that aims to define the concepts needed to describe commonly used atomic scale simulation methods, i.e. density functional theory, molecular dynamics, Monte Carlo methods, etc. ASMO uses the Provenance Ontology (PROV-O) to describe the simulation process.</terms:description>
     <terms:title>Atomistic Simulation Methods Ontology (ASMO)</terms:title>
+    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">0.0.1</owl:versionInfo>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotation properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
```

### Comparing `atomrdf-0.4.4/atomrdf/data/cmso.owl` & `atomrdf-0.6.0/atomrdf/data/cmso.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.4/atomrdf/data/element.yml` & `atomrdf-0.6.0/atomrdf/data/element.yml`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.4/atomrdf/data/pldo.owl` & `atomrdf-0.6.0/atomrdf/data/pldo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.4/atomrdf/data/podo.owl` & `atomrdf-0.6.0/atomrdf/data/podo.owl`

 * *Files identical despite different names*

### Comparing `atomrdf-0.4.4/atomrdf/json_io.py` & `atomrdf-0.6.0/atomrdf/json_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import json
 import yaml
 from atomrdf.encoder import NumpyArrayEncoder
 
+
 def write_file(outfile, data):
     """
     Write a given dict as json file
-    
+
     Parameters
     ----------
     outfile: string
         name of output file. `.json` will be added to the given file name
-    
+
     data: dict
         input data dict
-    
+
     Returns
     -------
     None
     """
     with open(".".join([outfile, "json"]), "w") as fout:
         json.dump(data, fout, cls=NumpyArrayEncoder)
-    #with open(".".join([outfile, "yaml"]), "w") as fout:
-    #    yaml.unsafe_dump(convert_to_dict(sys), fout)
+    # with open(".".join([outfile, "yaml"]), "w") as fout:
+    #    yaml.unsafe_dump(convert_to_dict(sys), fout)
```

### Comparing `atomrdf-0.4.4/atomrdf/network/network.py` & `atomrdf-0.6.0/atomrdf/network/network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,72 @@
+
+
 import networkx as nx
 import graphviz
 import matplotlib.pyplot as plt
 import numpy as np
 import os
 import warnings
 from pyscal3.atoms import AttrSetter
 
 from atomrdf.network.parser import OntoParser
 from atomrdf.network.term import OntoTerm, strip_name
 
 owlfile = os.path.join(os.path.dirname(__file__), "../data/cmso.owl")
 
+
 def _replace_name(name):
-    return ".".join(name.split(':'))
+    return ".".join(name.split(":"))
+
 
 class OntologyNetwork:
     """
     Network representation of Onto
     """
-    def __init__(self, infile=None, delimiter='/'):
+
+    def __init__(self, infile=None, delimiter="/"):
         if infile is None:
             infile = owlfile
-            
+
         self.g = nx.DiGraph()
         self.onto = OntoParser(infile, delimiter=delimiter)
-        self.onto.attributes['data_node'] = []
-        self.data_prefix = 'value'
+        self.onto.attributes["data_node"] = []
+        self.data_prefix = "value"
         self.terms = AttrSetter()
-        self._parse_all()        
-    
+        self._parse_all()
+
     def _assign_attributes(self):
         mapdict = {}
-        #add first level - namespaces
+        # add first level - namespaces
         for key in self.namespaces.keys():
             mapdict[key] = {}
-        
-        #now iterate over all attributes
-        for k1 in ['class', 'object_property', 'data_property']:
+
+        # now iterate over all attributes
+        for k1 in ["class", "object_property", "data_property"]:
             for k2, val in self.onto.attributes[k1].items():
                 mapdict[val.namespace][val.name_without_prefix] = val
-        
 
-        self.terms._add_attribute(mapdict) 
+        self.terms._add_attribute(mapdict)
 
     def _parse_all(self):
-        #call methods
+        # call methods
         self._add_class_nodes()
         self._add_object_properties()
         self._add_data_properties()
         self._assign_attributes()
 
     def __add__(self, ontonetwork):
-        #add onto network
+        # add onto network
         self.onto = self.onto + ontonetwork.onto
-        #now parse again
+        # now parse again
         self._parse_all()
         return self
 
     def strip_name(self, name):
-        raw = name.split(':')
+        raw = name.split(":")
         if len(raw) > 1:
             return raw[-1]
         return name
 
     @property
     def attributes(self):
         return self.onto.attributes
@@ -75,197 +79,345 @@
     def extra_namespaces(self):
         return self.onto.extra_namespaces
 
     def __radd__(self, ontonetwork):
         return self.__add__(ontonetwork)
 
     def get_shortest_path(self, source, target, triples=False):
+        """
+        Compute the shortest path between two nodes in the graph.
+
+        Parameters:
+        -----------
+        source : node
+            The starting node for the path.
+        target : node
+            The target node for the path.
+        triples : bool, optional
+            If True, returns the path as a list of triples. Each triple consists of three consecutive nodes in the path.
+            If False, returns the path as a list of nodes.
+
+        Returns:
+        --------
+        path : list
+            The shortest path between the source and target nodes. If `triples` is True, the path is returned as a list of triples.
+            If `triples` is False, the path is returned as a list of nodes.
+
+        """
         path = nx.shortest_path(self.g, source=source, target=target)
         if triples:
             triple_list = []
-            for x in range(len(path)//2):
-                triple_list.append(path[2*x:2*x+3])
+            for x in range(len(path) // 2):
+                triple_list.append(path[2 * x : 2 * x + 3])
             return triple_list
         return path
-    
+
     def _add_class_nodes(self):
-        for key, val in self.onto.attributes['class'].items():
-            self.g.add_node(val.name, node_type='class')
-    
+        for key, val in self.onto.attributes["class"].items():
+            self.g.add_node(val.name, node_type="class")
+
     def _add_object_properties(self):
-        for key, val in self.onto.attributes['object_property'].items():
-            self.g.add_node(val.name, node_type='object_property')
-            #find domain
+        for key, val in self.onto.attributes["object_property"].items():
+            self.g.add_node(val.name, node_type="object_property")
+            # find domain
             for d in val.domain:
                 self.g.add_edge(d, val.name)
             for r in val.range:
                 self.g.add_edge(val.name, r)
 
-    
     def _add_data_properties(self):
-        for key, val in self.onto.attributes['data_property'].items():
-            self.g.add_node(val.name, node_type='data_property')
+        for key, val in self.onto.attributes["data_property"].items():
+            self.g.add_node(val.name, node_type="data_property")
             for d in val.domain:
                 self.g.add_edge(d, val.name)
             for r in val.range:
-                data_node = f'{val.name}{self.data_prefix}'
-                self.onto.attributes['data_node'].append(data_node)
-                self.g.add_node(data_node, node_type='literal', data_type=r)
+                data_node = f"{val.name}{self.data_prefix}"
+                self.onto.attributes["data_node"].append(data_node)
+                self.g.add_node(data_node, node_type="literal", data_type=r)
                 self.g.add_edge(val.name, data_node)
 
-                
     def add_namespace(self, namespace_name, namespace_iri):
         """
-        Add a new namespace
+        Add a new namespace.
+
+        Parameters
+        ----------
+        namespace_name : str
+            The name of the namespace to add.
+        namespace_iri : str
+            The IRI of the namespace.
+
+        Raises
+        ------
+        KeyError
+            If the namespace already exists.
+
         """
         if namespace_name not in self.onto.namespaces.keys():
             self.onto.namespaces[namespace_name] = namespace_iri
         else:
             raise KeyError("namespace is already there!")
 
-    def add_term(self, uri, node_type, namespace=None,
-                dm=[], rn=[], data_type=None, 
-                node_id=None, delimiter='/'):
-        """
-        Add a node
-        """
-        #namespace = strip_name(uri, delimiter, get_what="namespace")
-        #name = strip_name(uri, delimiter, get_what="name")
-        term = OntoTerm(uri, namespace=namespace,
-            node_type=node_type, dm =dm, 
-            rn=rn, data_type=data_type, node_id=node_id,
-            delimiter=delimiter)
+    def add_term(
+        self,
+        uri,
+        node_type,
+        namespace=None,
+        dm=(),
+        rn=(),
+        data_type=None,
+        node_id=None,
+        delimiter="/",
+    ):
+        """
+        Add a node.
+
+        Parameters
+        ----------
+        uri : str
+            The URI of the node.
+        node_type : str
+            The type of the node.
+        namespace : str, optional
+            The namespace of the node.
+        dm : list, optional
+            The domain metadata of the node.
+        rn : list, optional
+            The range metadata of the node.
+        data_type : str, optional
+            The data type of the node.
+        node_id : str, optional
+            The ID of the node.
+        delimiter : str, optional
+            The delimiter used for parsing the URI.
+
+        Raises
+        ------
+        ValueError
+            If the namespace is not found.
+
+        """
+        term = OntoTerm(
+            uri,
+            namespace=namespace,
+            node_type=node_type,
+            dm=dm,
+            rn=rn,
+            data_type=data_type,
+            node_id=node_id,
+            delimiter=delimiter,
+        )
         if not term.namespace in self.onto.namespaces.keys():
             raise ValueError("Namespace not found, first add namespace")
         self.onto.attributes[node_type][term.name] = term
         self._assign_attributes()
 
     def add_path(self, triple):
         """
-        Add a triple as path. Note that all attributes of the triple should already
-        exist in the graph. The ontology itself is not modified. Only the graph
-        representation of it is.
-        The expected use is to bridge between two(or more) different ontologies.
+        Add a triple as path.
+
+        Note that all attributes of the triple should already exist in the graph.
+        The ontology itself is not modified. Only the graph representation of it is.
+        The expected use is to bridge between two (or more) different ontologies.
         Therefore, mapping can only be between classes.
+
+        Parameters
+        ----------
+        triple : tuple
+        A tuple representing the triple to be added. The tuple should contain three elements:
+        subject, predicate, and object.
+
+        Raises
+        ------
+        ValueError
+        If the subject or object of the triple is not found in the attributes of the ontology.
+
         """
         sub = triple[0]
         pred = triple[1]
         obj = triple[2]
 
-        if sub not in self.onto.attributes['class'].keys():
-            raise ValueError(f'{sub} not found in self.attributes')
+        if sub not in self.onto.attributes["class"].keys():
+            raise ValueError(f"{sub} not found in self.attributes")
 
-        #now add
+        # now add
         subclasses = self.onto._get_subclasses(sub)
         for subclass in subclasses:
-            self.g.add_edge(subclass, pred)            
-        
-        #now add pred
-        if pred in self.onto.attributes['object_property'].keys():
-            if obj not in self.onto.attributes['class'].keys():
-                raise ValueError(f'{obj} not found in self.attributes')
+            self.g.add_edge(subclass, pred)
+
+        # now add pred
+        if pred in self.onto.attributes["object_property"].keys():
+            if obj not in self.onto.attributes["class"].keys():
+                raise ValueError(f"{obj} not found in self.attributes")
             subclasses = self.onto._get_subclasses(obj)
             for subclass in subclasses:
-                self.g.add_edge(pred, subclass) 
+                self.g.add_edge(pred, subclass)
 
-        #another possibility it is data property
-        elif pred in self.onto.attributes['data_property'].keys():
-            data_node = f'{pred}{self.data_prefix}'
-            self.g.add_node(data_node, node_type='literal', data_type=obj)
+        # another possibility it is data property
+        elif pred in self.onto.attributes["data_property"].keys():
+            data_node = f"{pred}{self.data_prefix}"
+            self.g.add_node(data_node, node_type="literal", data_type=obj)
             self.g.add_edge(pred, data_node)
-        
+
         else:
-            raise ValueError(f'{pred} not found in self.attributes')
+            raise ValueError(f"{pred} not found in self.attributes")
+
+    def draw(self, 
+        styledict={
+            "class": {"shape": "box"},
+            "object_property": {"shape": "ellipse"},
+            "data_property": {"shape": "ellipse"},
+            "literal": {"shape": "parallelogram"},
+        },):
+        """
+        Draw the network graph using graphviz.
 
-    def draw(self, styledict = {"class": {"shape":"box"},
-                                "object_property": {"shape":"ellipse"},
-                                "data_property": {"shape":"ellipse"},
-                                "literal": {"shape":"parallelogram"},}):
+        Parameters
+        ----------
+        styledict : dict, optional
+            A dictionary specifying the styles for different node types.
+            The keys of the dictionary are the node types, and the values are dictionaries
+            specifying the shape for each node type. Defaults to None.
+
+        Returns
+        -------
+        graphviz.Digraph
+            The graph object representing the network graph.
+
+        Example
+        -------
+        styledict = {
+            "class": {"shape": "box"},
+            "object_property": {"shape": "ellipse"},
+            "data_property": {"shape": "ellipse"},
+            "literal": {"shape": "parallelogram"},
+        }
+        network.draw(styledict)
+        """
         dot = graphviz.Digraph()
-        node_list = list(self.g.nodes(data='node_type'))
+        node_list = list(self.g.nodes(data="node_type"))
         edge_list = list(self.g.edges)
         for node in node_list:
             name = _replace_name(node[0])
             if node[1] is not None:
                 t = node[1]
-                dot.node(name, shape=styledict[t]['shape'], fontsize="6")
+                dot.node(name, shape=styledict[t]["shape"], fontsize="6")
         for edge in edge_list:
             dot.edge(_replace_name(edge[0]), _replace_name(edge[1]))
         return dot
 
     def get_path_from_sample(self, target):
-        path = self.get_shortest_path(source="cmso:ComputationalSample", target=target, triples=True)
+        """
+        Get the shortest path from the 'cmso:ComputationalSample' node to the target node.
+
+        Parameters
+        ----------
+        target : OntoTerm
+            The target node to find the shortest path to.
+
+        Returns
+        -------
+        list
+            A list of triples representing the shortest path from 'cmso:ComputationalSample' to the target node.
+        """
+        path = self.get_shortest_path(
+            source="cmso:ComputationalSample", target=target, triples=True
+        )
         return path
-        
-        
+
     def create_query(self, source, destinations, condition=None, enforce_types=True):
         """
-        values is a dict with keys value, operation
+        Create a SPARQL query string based on the given source, destinations, condition, and enforce_types.
+
+        Parameters
+        ----------
+        source : Node
+            The source node from which the query starts.
+        destinations : list or Node
+            The destination node(s) to which the query should reach. If a single node is provided, it will be converted to a list.
+        condition : Condition, optional
+            The condition to be applied in the query. Defaults to None.
+        enforce_types : bool, optional
+            Whether to enforce the types of the source and destination nodes in the query. Defaults to True.
+
+        Returns
+        -------
+        str
+            The generated SPARQL query string.
+
         """
         if not isinstance(destinations, list):
             destinations = [destinations]
-        
+
         source_name = source.query_name
         destination_names = [destination.query_name for destination in destinations]
-        
-        #if condition is specified, and is not there, add it
+
+        # if condition is specified, and is not there, add it
         if condition is not None:
             if condition.query_name not in destination_names:
                 destination_names.append(condition.query_name)
-        
-        #add source if not available
+
+        # add source if not available
         if source_name not in destination_names:
             destination_names.append(source_name)
 
-        #start prefix of query
+        # start prefix of query
         query = []
         for key, val in self.namespaces.items():
-            query.append(f'PREFIX {key}: <{val}>')
+            query.append(f"PREFIX {key}: <{val}>")
         for key, val in self.extra_namespaces.items():
-            query.append(f'PREFIX {key}: <{val}>')
-        
-        #now for each destination, start adding the paths in the query
+            query.append(f"PREFIX {key}: <{val}>")
+
+        # now for each destination, start adding the paths in the query
         all_triplets = {}
         for destination in destination_names:
             triplets = self.get_shortest_path(source_name, destination, triples=True)
             all_triplets[destination] = triplets
-        
-        select_destinations = [f'?{self.strip_name(destination)}' for destination in destination_names]
+
+        select_destinations = [
+            f"?{self.strip_name(destination)}" for destination in destination_names
+        ]
         query.append(f'SELECT DISTINCT {" ".join(select_destinations)}')
         query.append("WHERE {")
-        
-        #now add corresponding triples
+
+        # now add corresponding triples
         for destination in destination_names:
             for triple in all_triplets[destination]:
-                #print(triple)
-                query.append("    ?%s %s ?%s ."%(self.strip_name(triple[0]), 
-                                                 triple[1], 
-                                                 self.strip_name(triple[2])))
-        
-        #we enforce types of the source and destination
+                # print(triple)
+                query.append(
+                    "    ?%s %s ?%s ."
+                    % (
+                        self.strip_name(triple[0]),
+                        triple[1],
+                        self.strip_name(triple[2]),
+                    )
+                )
+
+        # we enforce types of the source and destination
         if enforce_types:
-            if source.node_type == 'class':
-                query.append("    ?%s rdf:type %s ."%(self.strip_name(source.query_name), source.query_name))
+            if source.node_type == "class":
+                query.append(
+                    "    ?%s rdf:type %s ."
+                    % (self.strip_name(source.query_name), source.query_name)
+                )
             for destination in destinations:
-                if destination.node_type == 'class':
-                    query.append("    ?%s rdf:type %s ."%(self.strip_name(destination.query_name), destination.query_name))
-        #now we have to add filters
-        #filters are only needed if it is a dataproperty
-        filter_text = ''
-        
-        #make filters; get all the unique filters from all the classes in destinations
+                if destination.node_type == "class":
+                    query.append(
+                        "    ?%s rdf:type %s ."
+                        % (
+                            self.strip_name(destination.query_name),
+                            destination.query_name,
+                        )
+                    )
+        # now we have to add filters
+        # filters are only needed if it is a dataproperty
+        filter_text = ""
+
+        # make filters; get all the unique filters from all the classes in destinations
         if condition is not None:
             if condition._condition is not None:
                 filter_text = condition._condition
 
-        if filter_text != '':
-            query.append(f'FILTER {filter_text}')
-        query.append('}')
-        return '\n'.join(query)
-
-        
-            
-            
-            
-
-        
-        
+        if filter_text != "":
+            query.append(f"FILTER {filter_text}")
+        query.append("}")
+        return "\n".join(query)
```

### Comparing `atomrdf-0.4.4/atomrdf/network/parser.py` & `atomrdf-0.6.0/atomrdf/network/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,137 @@
-
 from owlready2 import get_ontology
 import owlready2
 
 import os
 import copy
 import numpy as np
 import itertools
 
-from atomrdf.network.term import OntoTerm, strip_name 
+from atomrdf.network.term import OntoTerm, strip_name
 from atomrdf.network.patch import patch_terms
 
 
 class OntoParser:
-    def __init__(self, infile, delimiter='/'):
+    def __init__(self, infile, delimiter="/"):
         if os.path.exists(infile):
-            self.tree = get_ontology(f'file://{infile}').load()
-        elif infile[:4] == 'http':
+            self.tree = get_ontology(f"file://{infile}").load()
+        elif infile[:4] == "http":
             self.tree = get_ontology(infile)
         else:
-            raise FileNotFoundError(f'file {infile} not found!')
+            raise FileNotFoundError(f"file {infile} not found!")
         self.attributes = {}
-        self.attributes['class'] = {}
-        self.attributes['object_property'] = {}
-        self.attributes['data_property'] = {}        
+        self.attributes["class"] = {}
+        self.attributes["object_property"] = {}
+        self.attributes["data_property"] = {}
         self.delimiter = delimiter
         self.classes = None
         self.namespaces = {self.tree.name: self.tree.base_iri}
         self.extra_namespaces = {}
         self._parse_class()
-        #print(self.attributes)
+        # print(self.attributes)
         self._parse_object_property()
         self._parse_data_property()
         self._recheck_namespaces()
 
     def __add__(self, ontoparser):
         """
         Add method; in principle it should add-
         - classes
         - attributes dict
         """
-        for mainkey in ['class', 'object_property', 'data_property']:
+        for mainkey in ["class", "object_property", "data_property"]:
             if mainkey in ontoparser.attributes.keys():
                 for key, val in ontoparser.attributes[mainkey].items():
-                    self.attributes[mainkey][key] = val        
-                    
+                    self.attributes[mainkey][key] = val
 
-        #now change classes
+        # now change classes
         if ontoparser.classes is not None:
             for clx in ontoparser.classes:
                 self.classes.append(clx)
 
         for key, val in ontoparser.namespaces.items():
             self.namespaces[key] = val
 
         for key, val in ontoparser.extra_namespaces.items():
             self.extra_namespaces[key] = val
 
         return self
 
     def __radd__(self, ontoparser):
         return self.__add__(ontoparser)
-    
-    def _strip_datatype(self, uri, delimiter='#'):
+
+    def _strip_datatype(self, uri, delimiter="#"):
         uri_split = uri.split(delimiter)
-        return uri_split[-1]        
-        
+        return uri_split[-1]
+
     def _dict_to_lst(self, d):
         return [val for key, val in d.items()]
-    
+
     def _get_subclasses(self, name):
         arg = self._in_which_bin_is_class(name)
         if arg is not None:
             return self.classes[arg]
         else:
             return [name]
-    
+
     def _recheck_namespaces(self):
         for mainkey in self.attributes.keys():
             for key, val in self.attributes[mainkey].items():
                 namespace = self.attributes[mainkey][key].namespace
                 if namespace not in self.namespaces.keys():
-                    self.namespaces[namespace] = self.attributes[mainkey][key].namespace_with_prefix
-
+                    self.namespaces[namespace] = self.attributes[mainkey][
+                        key
+                    ].namespace_with_prefix
 
     def _parse_data_property(self):
         for c in self.tree.data_properties():
             iri = c.iri
             dm = c.domain
             try:
                 dm = [strip_name(d.iri, self.delimiter) for d in dm[0].Classes]
             except:
                 dm = [strip_name(d.iri, self.delimiter) for d in dm]
-            
-            #now get subclasses
+
+            # now get subclasses
             dm = [self._get_subclasses(d) for d in dm]
             dm = list(itertools.chain(*dm))
-            
+
             rn = c.range
             try:
                 rn = [r.__name__ for r in rn[0].Classes if r is not None]
             except:
                 rn = [r.__name__ for r in rn if r is not None]
 
-            
-            #Subproperties
-            #Commented out for now
-            #subprops = self.tree.search(subproperty_of=getattr(self.tree, c.name))
-            #for subprop in subprops:
+            # Subproperties
+            # Commented out for now
+            # subprops = self.tree.search(subproperty_of=getattr(self.tree, c.name))
+            # for subprop in subprops:
             #    if subprop.iri != iri:
             #        #print(subprop.iri)
             #        pass
 
-            #PATCH
-            #Here: we patch specific items specifically for pyscal rdf
-            rn  = patch_terms(iri, rn)
+            # PATCH
+            # Here: we patch specific items specifically for pyscal rdf
+            rn = patch_terms(iri, rn)
 
-            #print(iri, rn)
-            #print(iri, dm)
+            # print(iri, rn)
+            # print(iri, dm)
             term = OntoTerm(iri, delimiter=self.delimiter)
+            dm = [x.replace("07:owl#Thing", "owl:Thing") for x in dm]
             term.domain = dm
             term.range = rn
-            term.node_type = 'data_property'
-            self.attributes['data_property'][term.name] = term
-            #assign this data
+            term.node_type = "data_property"
+            self.attributes["data_property"][term.name] = term
+            # assign this data
             for d in dm:
-                if d!='07:owl#Thing':
-                    self.attributes['class'][d].is_range_of.append(term.name)
-
+                if d != "owl:Thing":
+                    self.attributes["class"][d].is_range_of.append(term.name)
 
-            #subproperties should be treated the same
+            # subproperties should be treated the same
 
-            
     def _parse_object_property(self):
         for c in self.tree.object_properties():
             iri = c.iri
             dm = c.domain
             try:
                 dm = [strip_name(d.iri, self.delimiter) for d in dm[0].Classes]
             except:
@@ -142,106 +139,115 @@
                 for d in dm:
                     if isinstance(d, owlready2.class_construct.Or):
                         for x in d.Classes:
                             dmnew.append(strip_name(x.iri, self.delimiter))
                     else:
                         dmnew.append(strip_name(d.iri, self.delimiter))
                 dm = dmnew
-            
-            #now get subclasses
+
+            # now get subclasses
             dm = [self._get_subclasses(d) for d in dm]
             dm = list(itertools.chain(*dm))
 
             rn = c.range
             try:
                 rn = [strip_name(r.iri, self.delimiter) for r in rn[0].Classes]
             except:
                 rn = [strip_name(r.iri, self.delimiter) for r in rn]
-            
-            #now get subclasses
+
+            # now get subclasses
             rn = [self._get_subclasses(d) for d in rn]
             rn = list(itertools.chain(*rn))
 
             term = OntoTerm(iri, delimiter=self.delimiter)
             term.domain = dm
             term.range = rn
-            term.node_type = 'object_property'
-            self.attributes['object_property'][term.name] = term
+            term.node_type = "object_property"
+            self.attributes["object_property"][term.name] = term
             for d in dm:
-                if d!='07:owl#Thing':
-                    if d in self.attributes['class']:
-                        self.attributes['class'][d].is_range_of.append(term.name)
+                if d != "07:owl#Thing":
+                    if d in self.attributes["class"]:
+                        self.attributes["class"][d].is_range_of.append(term.name)
             for r in rn:
-                if r!='07:owl#Thing':
-                    if d in self.attributes['class']:
-                        self.attributes['class'][d].is_domain_of.append(term.name)
-                
+                if r != "07:owl#Thing":
+                    if d in self.attributes["class"]:
+                        self.attributes["class"][d].is_domain_of.append(term.name)
+
     def _parse_class_basic(self):
         classes = []
         for c in self.tree.classes():
             iri = c.iri
-            #print(iri)
-            #print(iri)
-            try:
-                subclasses = self.tree.search(subclass_of=getattr(self.tree, c.name))
-                for sb in subclasses:
-                    term = OntoTerm(sb.iri, delimiter=self.delimiter)
-                    term.node_type ='class'
-                    self.attributes['class'][term.name] = term
-                subclasses = [strip_name(sb.iri, self.delimiter) for sb in subclasses]
-                classes.append(subclasses)
-            except:
-                term = OntoTerm(c.iri, delimiter=self.delimiter)
-                term.node_type ='class'
-                self.attributes['class'][term.name] = term                
-                classes.append([strip_name(c.iri, self.delimiter)])
+            # print(iri)
+            # print(iri)
+            # CHILDREN
+            children = self.tree.get_children_of(c)
+            named_instances = self.tree.get_instances_of(c)
+            equiv_classes = c.equivalent_to
+            subclasses = [*children, *named_instances, *equiv_classes]
+            subclasses.append(c)
+            for sb in subclasses:
+                term = OntoTerm(sb.iri, delimiter=self.delimiter)
+                term.node_type = "class"
+                self.attributes["class"][term.name] = term
+            subclasses = [strip_name(sb.iri, self.delimiter) for sb in subclasses]
+            classes.append(subclasses)
+
+            # try:
+            #    subclasses = self.tree.search(subclass_of=getattr(self.tree, c.name))
+            #    for sb in subclasses:
+            #        term = OntoTerm(sb.iri, delimiter=self.delimiter)
+            #        term.node_type ='class'
+            #        self.attributes['class'][term.name] = term
+            #    subclasses = [strip_name(sb.iri, self.delimiter) for sb in subclasses]
+            #    classes.append(subclasses)
+            # except:
+            #    term = OntoTerm(c.iri, delimiter=self.delimiter)
+            #    term.node_type ='class'
+            #    self.attributes['class'][term.name] = term
+            #    classes.append([strip_name(c.iri, self.delimiter)])
         return classes
-    
+
     def _aggregate_keys(self, dd):
         lst = copy.deepcopy(dd)
-        #choose the first list
+        # choose the first list
         large_list = []
         start = lst[0]
-        #delete it from the main list
+        # delete it from the main list
         nruns = len(lst)
         del lst[0]
-        #now loop, if there is intersection add to this list
+        # now loop, if there is intersection add to this list
         while True:
             found = False
             index_to_delete = []
             for count, ls in enumerate(lst):
                 common = len(list(set(start) & set(ls)))
-                #print(common)
-                if  common>0:
-                    #common elements found! merge them
+                # print(common)
+                if common > 0:
+                    # common elements found! merge them
                     for l in ls:
                         start.append(l)
                     found = True
                     index_to_delete.append(count)
             if found:
                 for ii in index_to_delete[::-1]:
                     del lst[ii]
             else:
                 large_list.append(np.unique(start))
-                if len(lst)==0:
+                if len(lst) == 0:
                     break
                 else:
                     start = lst[0]
                     del lst[0]
         return large_list
-            
+
     def _parse_class(self):
         sub_classes = self._parse_class_basic()
-        #now we have to go through and clean up sub classes
+        # now we have to go through and clean up sub classes
         sub_classes = self._aggregate_keys(sub_classes)
         self.classes = sub_classes
-        
+
     def _in_which_bin_is_class(self, name):
         for count, lst in enumerate(self.classes):
             if name in lst:
                 return count
         else:
             return None
-    
-            
-            
-
```

### Comparing `atomrdf-0.4.4/atomrdf/network/term.py` & `atomrdf-0.6.0/atomrdf/network/term.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,259 @@
 """
 https://docs.python.org/3/library/operator.html
 """
+
 from rdflib import Namespace
 import numbers
 
+
 def _get_name(uri, delimiter):
     """
     Just get name with namespace prefix
     """
     uri_split = uri.split(delimiter)
     name = uri_split[-1]
     return name
 
+
 def _get_namespace(uri, delimiter):
     if delimiter == "/":
         uri_split = uri.split(delimiter)
-        if len(uri_split)>1:
+        if len(uri_split) > 1:
             namespace = uri_split[-2]
         else:
-            namespace = uri 
+            namespace = uri
     else:
         uri_split = uri.split(delimiter)
         uri_split = uri_split[0].split("/")
-        if len(uri_split)>0:
+        if len(uri_split) > 0:
             namespace = uri_split[-1]
         else:
             namespace = uri
-    return namespace    
+    return namespace
+
 
-def strip_name(uri, delimiter, get_what='name', namespace=None):
+def strip_name(uri, delimiter, get_what="name", namespace=None):
     if get_what == "namespace":
         return _get_namespace(uri, delimiter)
-    
-    elif get_what == "name":    
+
+    elif get_what == "name":
         if namespace is None:
             namespace = _get_namespace(uri, delimiter)
         name = _get_name(uri, delimiter)
         return ":".join([namespace, name])
 
 
 class OntoTerm:
-    def __init__(self, uri,
-        namespace=None, 
-        node_type=None, 
-        dm=[], rn=[], 
-        data_type=None, 
-        node_id=None, 
-        delimiter='/'):
-        """
-        This is class that represents an ontology element.
-
-        Parameters
-        -----------
-        uri: string
-            uri of the ontology term
-
-        namespace: string, optional
-            if provided this will be used as namespace
-        
-        """
+    def __init__(
+        self,
+        uri,
+        namespace=None,
+        node_type=None,
+        dm=[],
+        rn=[],
+        data_type=None,
+        node_id=None,
+        delimiter="/",
+    ):
+
         self.uri = uri
-        #type: can be object property, data property, or class
+        # type: can be object property, data property, or class
         self.node_type = node_type
-        #now we need domain and range
+        # now we need domain and range
         self.domain = dm
         self.range = rn
-        #datatype, that is only need for data properties
+        # datatype, that is only need for data properties
         self.data_type = data_type
-        #identifier
+        # identifier
         self.node_id = node_id
         self.subclasses = []
         self.subproperties = []
         self.delimiter = delimiter
         self.is_domain_of = []
         self.is_range_of = []
         self._condition = None
         self._namespace = namespace
-        #name of the class
+        # name of the class
         self._name = None
 
-
-
     @property
     def uri(self):
+        """
+        Get the URI of the ontology term.
+
+        Returns
+        -------
+        str
+            The URI of the ontology term.
+        """
         return self._uri
-    
+
     @uri.setter
     def uri(self, val):
         self._uri = val
-    
+
     @property
     def name_without_prefix(self):
-        return _get_name(self.uri, self.delimiter)
+        """
+        Get the name without the namespace prefix.
+
+        Returns
+        -------
+        str
+            The name of the term without the namespace prefix.
+        """
+        name = _get_name(self.uri, self.delimiter)
+        name = name.replace("–", "")
+        name = name.replace("-", "")
+        return name
 
     @property
     def name(self):
-        return strip_name(self.uri, self.delimiter, 
-            namespace=self._namespace, get_what="name")        
+        """
+        Get the name of the term.
+
+        Returns
+        -------
+        str
+            The name of the term.
+        """
+        return strip_name(
+            self.uri, self.delimiter, namespace=self._namespace, get_what="name"
+        )
 
     @property
     def namespace(self):
+        """
+        Get the namespace of the term.
+
+        Returns
+        -------
+        str
+            The namespace of the term.
+        """
         if self._namespace is not None:
             return self._namespace
         else:
-            return strip_name(self.uri, self.delimiter, get_what="namespace")        
+            return strip_name(self.uri, self.delimiter, get_what="namespace")
 
     @property
     def namespace_with_prefix(self):
+        """
+        Get the namespace of the term with the prefix.
+
+        Returns
+        -------
+        str
+            The namespace of the term with the prefix.
+        """
         uri_split = self.uri.split(self.delimiter)
-        if len(uri_split)>1:
+        if len(uri_split) > 1:
             namespace = self.delimiter.join(uri_split[:-1]) + self.delimiter
             return namespace
         else:
             return self.uri
 
     @property
     def namespace_object(self):
+        """
+        Get the namespace object for the term.
+
+        Returns
+        -------
+        object
+            The namespace object for the term.
+
+        """
         uri_split = self.uri.split(self.delimiter)
-        if len(uri_split)>1:
+        if len(uri_split) > 1:
             namespace = self.delimiter.join(uri_split[:-1]) + self.delimiter
             prop = uri_split[-1]
             return getattr(Namespace(namespace), prop)
         else:
             return self.uri
 
     @property
     def query_name(self):
         """
-        What it is called in a sparql query
+        Get the name of the term as it appears in a SPARQL query.
+
+        Returns
+        -------
+        str
+            The name of the term in a SPARQL query.
+
+        Notes
+        -----
+        If the term is a data property, the name will be appended with "value".
+
         """
         if self.node_type == "data_property":
             return self.name + "value"
         return self.name
 
     @property
     def query_name_without_prefix(self):
         """
-        What it is called in a sparql query
+        Get the name of the term as it appears in a SPARQL query without prefix.
+
+        Returns
+        -------
+        str
+            The name of the term in a SPARQL query.
+
+        Notes
+        -----
+        If the term is a data property, the name will be suffixed with "value".
         """
         if self.node_type == "data_property":
             return self.name_without_prefix + "value"
         return self.name_without_prefix
 
+    def toPython(self):
+        return self.uri
+
     def __repr__(self):
         return str(self.name)
 
     def _clean_datatype(self, r):
-        if r=='str':
-            return 'string'
+        if r == "str":
+            return "string"
         return r
 
-    #convenience methods for overload checking
+    # convenience methods for overload checking
     def _ensure_condition_exists(self):
         if self._condition is None:
-            raise ValueError("Individual terms should have condition for this operation!")
+            raise ValueError(
+                "Individual terms should have condition for this operation!"
+            )
 
     def _is_term(self, val):
         if not isinstance(val, OntoTerm):
             raise TypeError("can only be performed with an OntoTerm!")
 
     def _is_number(self, val):
         if not isinstance(val, numbers.Number):
             raise TypeError("can only be performed with a number!")
-    
+
     def _is_data_node(self):
         if not self.node_type == "data_property":
-            raise TypeError("This operation can only be performed with a data property!")
+            raise TypeError(
+                "This operation can only be performed with a data property!"
+            )
 
     def _create_condition_string(self, condition, val):
-        return f'(?{self.query_name_without_prefix}{condition}\"{val}\"^^xsd:{self._clean_datatype(self.range[0])})'
-    
-    #overloading operators
+        return f'(?{self.query_name_without_prefix}{condition}"{val}"^^xsd:{self._clean_datatype(self.range[0])})'
+
+    # overloading operators
     def __eq__(self, val):
         """
-        = 
+        =
         """
-        #self._is_number(val)
+        # self._is_number(val)
         self._is_data_node()
         self._condition = self._create_condition_string("=", val)
         return self
 
     def __lt__(self, val):
         self._is_number(val)
         self._is_data_node()
@@ -188,51 +262,50 @@
 
     def __le__(self, val):
         self._is_number(val)
         self._is_data_node()
         self._condition = self._create_condition_string("<=", val)
         return self
 
-
     def __ne__(self, val):
-        #self._is_number(val)
+        # self._is_number(val)
         self._is_data_node()
         self._condition = self._create_condition_string("!=", val)
         return self
-    
+
     def __ge__(self, val):
         self._is_number(val)
         self._is_data_node()
         self._condition = self._create_condition_string(">=", val)
         return self
-    
+
     def __gt__(self, val):
         self._is_number(val)
         self._is_data_node()
         self._condition = self._create_condition_string(">", val)
         return self
 
     def __and__(self, term):
         self._is_term(term)
         self._is_data_node()
         term._is_data_node()
         self._ensure_condition_exists()
-        term._ensure_condition_exists()        
+        term._ensure_condition_exists()
         self._condition = "&&".join([self._condition, term._condition])
-        self._condition = f'({self._condition})'
+        self._condition = f"({self._condition})"
         return self
 
     def and_(self, term):
         self.__and__(term)
 
     def __or__(self, term):
         self._is_term(term)
         self._is_data_node()
         term._is_data_node()
         self._ensure_condition_exists()
-        term._ensure_condition_exists()        
+        term._ensure_condition_exists()
         self._condition = "||".join([self._condition, term._condition])
-        self._condition = f'({self._condition})'
+        self._condition = f"({self._condition})"
         return self
 
     def or_(self, term):
-        self.__or__(term)
+        self.__or__(term)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `atomrdf-0.4.4/atomrdf/visualize.py` & `atomrdf-0.6.0/atomrdf/visualize.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,149 +4,217 @@
 import uuid
 import json
 
 
 def get_title_from_BNode(x):
     return x.toPython()
 
+
 def get_string_from_URI(x):
     """
-    Extract a presentable string from URI
+    Extract a presentable string from URI.
 
-    Also differentiate between fixed notes and URIs, and assign color
+    Parameters
+    ----------
+    x : rdflib.term.URIRef
+        The URI object to extract the string from.
+
+    Returns
+    -------
+    tuple
+        A tuple containing the presentable string representation of the URI and its type.
+        The string representation is the last part of the URI after splitting by '#' or '/'.
+        The type can be either "URIRef" or "BNode".
     """
     raw = x.toPython()
-    #first try splitting by #
+    # first try splitting by #
     rawsplit = raw.split("#")
     if len(rawsplit) > 1:
         return rawsplit[-1], "URIRef"
-    
-    #try splitting by = for chebi values
-    if 'CHEBI' in raw:
+
+    # try splitting by = for chebi values
+    if "CHEBI" in raw:
         rawsplit = raw.split("=")
         rawsplit = rawsplit[-1].split(":")
         if len(rawsplit) > 1:
             return ".".join(rawsplit[-2:]), "URIRef"
-    
-    if 'sample:' in raw:
+
+    if "sample:" in raw:
         rawsplit = raw.split(":")
         if len(rawsplit) > 1:
             return "_".join(rawsplit), "BNode"
 
-    #just a normal url split now
+    # just a normal url split now
     rawsplit = raw.split("/")
     if len(rawsplit) > 1:
         return ".".join(rawsplit[-2:]), "URIRef"
 
-    rawsplit = raw.split(':')
-    if len(rawsplit) == 2:
-        return "_".join(rawsplit), "BNode"        
-
-    #none of the conditions, worked, which means its a hex string
+    # none of the conditions worked, which means it's a hex string
     return raw, "BNode"
 
+
 def parse_object(x):
+    """
+    Parse the given object and return its title and type.
+
+    Parameters
+    ----------
+    x : RDF term
+        The RDF term to parse.
+
+    Returns
+    -------
+    tuple
+        A tuple containing the title of the object and its type.
+
+    """
     if isinstance(x, BNode):
         return get_title_from_BNode(x), "BNode"
     elif isinstance(x, URIRef):
         return get_string_from_URI(x)
     elif isinstance(x, Literal):
         return str(x.title()), "Literal"
 
+
 styledict = {
     "BNode": {"color": "#ffe6ff", "shape": "box", "style": "filled"},
     "URIRef": {"color": "#ffffcc", "shape": "box", "style": "filled"},
     "Literal": {"color": "#e6ffcc", "shape": "ellipse", "style": "filled"},
 }
 
+
 def _switch_box(box):
     if box == "box":
-        return 'rectangle'
-    #remember that only boxes will be used, circles no!
-    
+        return "rectangle"
+    # remember that only boxes will be used, circles no!
+
+
 def _fix_id(string1, istype1):
-    if istype1 == 'Literal':
+    if istype1 == "Literal":
         id1 = str(uuid.uuid4())
     else:
         id1 = string1
     return id1
 
-def visualize_graph(g,
-            styledict=styledict,
-            rankdir='TB',
-            hide_types=False,
-            workflow_view=False,
-            size=None,
-            layout='dot'):
-    
+
+def visualize_graph(
+    g,
+    styledict=styledict,
+    rankdir="TB",
+    hide_types=False,
+    workflow_view=False,
+    size=None,
+    layout="dot",
+):
+    """
+    Visualizes a graph using Graphviz.
+
+    Parameters
+    ----------
+    g : dict
+        The graph to visualize.
+    styledict : dict, optional
+        A dictionary containing styles for different types of nodes and edges. Default is `styledict`.
+    rankdir : str, optional
+        The direction of the graph layout. Default is "TB" (top to bottom).
+    hide_types : bool, optional
+        Whether to hide nodes with the "type" attribute. Default is False.
+    workflow_view : bool, optional
+        Whether to enable the workflow view. Default is False.
+    size : str, optional
+        The size of the graph. Default is None.
+    layout : str, optional
+        The layout algorithm to use. Default is "dot".
+
+    Returns
+    -------
+    dot : graphviz.Digraph
+        The graph visualization.
+    """
     dot = graphviz.Digraph()
 
     dot.attr(
         rankdir=rankdir,
         style="filled",
         size=size,
         layout=layout,
         overlap="false",
     )
-    
+
     for k in g:
         string1, istype1 = parse_object(k[0])
         string2, istype2 = parse_object(k[2])
         string3, istype = parse_object(k[1])
 
         plot = True
-        
+
         if workflow_view:
-            #we collapse sample information
-            #if cmso.connector is found, only use it is it is cmso.hasCalculated
-            #all sub sample props, indicated by sample_x_jsjsj will be ignored.
+            # we collapse sample information
+            # if cmso.connector is found, only use it is it is cmso.hasCalculated
+            # all sub sample props, indicated by sample_x_jsjsj will be ignored.
             green_list = ["hasCalculatedProperty", "wasCalculatedBy", "hasValue"]
-            ssplit = string3.split('.')
-            if (len(ssplit) == 2):
-                if (ssplit[0] == 'cmso') and (ssplit[1] not in green_list):
+            ssplit = string3.split(".")
+            if len(ssplit) == 2:
+                if (ssplit[0] == "cmso") and (ssplit[1] not in green_list):
                     plot = False
-            if string3 == 'subClassOf':
+            if string3 == "subClassOf":
                 plot = False
-            ssplit = string2.split('.')
-            if string3 == 'type':
-                if (ssplit[0] == 'cmso') and (ssplit[1] not in  ["CalculatedProperty"]):
+            ssplit = string2.split(".")
+            if string3 == "type":
+                if (ssplit[0] == "cmso") and (ssplit[1] not in ["CalculatedProperty"]):
+                    plot = False
+                if (ssplit[0] == "cmso") and (ssplit[1] in ["AtomicScaleSample"]):
+                    dot.node(
+                        string1,
+                        label=string1,
+                        shape=styledict[istype1]["shape"],
+                        style=styledict[istype1]["style"],
+                        color=styledict[istype1]["color"],
+                        fontsize=styledict[istype1]["fontsize"],
+                        fontname=styledict[istype1]["fontname"],
+                    )
                     plot = False
-                if (ssplit[0] == 'cmso') and (ssplit[1] in  ["AtomicScaleSample"]):
-                    dot.node(string1, label=string1, shape=styledict[istype1]["shape"], 
-                             style=styledict[istype1]["style"], 
-                             color=styledict[istype1]["color"],
-                             fontsize=styledict[istype1]["fontsize"],
-                             fontname=styledict[istype1]["fontname"])
-                    plot=False
 
-        if hide_types and (string3 == 'type'):
+        if hide_types and (string3 == "type"):
             plot = False
 
         if not plot:
             continue
 
-        if istype1 == 'Literal':
+        if istype1 == "Literal":
             id1 = str(uuid.uuid4())
         else:
-            id1 = string1 
-        dot.node(id1, label=string1, shape=styledict[istype1]["shape"], 
-                 style=styledict[istype1]["style"], 
-                 color=styledict[istype1]["color"],
-                 fontsize=styledict[istype1]["fontsize"],
-                 fontname=styledict[istype1]["fontname"])
-        
-        if istype2 == 'Literal':
+            id1 = string1
+        dot.node(
+            id1,
+            label=string1,
+            shape=styledict[istype1]["shape"],
+            style=styledict[istype1]["style"],
+            color=styledict[istype1]["color"],
+            fontsize=styledict[istype1]["fontsize"],
+            fontname=styledict[istype1]["fontname"],
+        )
+
+        if istype2 == "Literal":
             id2 = str(uuid.uuid4())
         else:
-            id2 = string2 
-        dot.node(id2, label=string2, shape=styledict[istype2]["shape"], 
-                 style=styledict[istype2]["style"], 
-                 color=styledict[istype2]["color"],
-                 fontsize=styledict[istype2]["fontsize"],
-                 fontname=styledict[istype2]["fontname"])
-        
-        dot.edge(id1, id2, color=styledict["edgecolor"], 
-            label=string3, 
+            id2 = string2
+        dot.node(
+            id2,
+            label=string2,
+            shape=styledict[istype2]["shape"],
+            style=styledict[istype2]["style"],
+            color=styledict[istype2]["color"],
             fontsize=styledict[istype2]["fontsize"],
-            fontname=styledict[istype2]["fontname"])
-    
-    return dot
+            fontname=styledict[istype2]["fontname"],
+        )
+
+        dot.edge(
+            id1,
+            id2,
+            color=styledict["edgecolor"],
+            label=string3,
+            fontsize=styledict[istype2]["fontsize"],
+            fontname=styledict[istype2]["fontname"],
+        )
+
+    return dot
```

### Comparing `atomrdf-0.4.4/atomrdf/workflow/workflow.py` & `atomrdf-0.6.0/atomrdf/workflow/workflow.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,288 +10,404 @@
 _identify_method
 extract_calculated_properties
 inform_graph
 
 See atomrdf.workflow.pyiron for more details
 """
 
-from rdflib import Graph, Literal, Namespace, XSD, RDF, RDFS, BNode, URIRef, FOAF, SKOS, DCTERMS
+from rdflib import Literal, Namespace, XSD, RDF, RDFS, BNode, URIRef
 
 import warnings
 import numpy as np
 import os
 import copy
 import ast
 import uuid
 
 from atomrdf.structure import System
 
-#Move imports to another file
-PROV = Namespace("http://www.w3.org/ns/prov#")
-CMSO = Namespace("http://purls.helmholtz-metadaten.de/cmso/")
-PODO = Namespace("http://purls.helmholtz-metadaten.de/podo/")
-ASO = Namespace("http://purls.helmholtz-metadaten.de/aso/")
+# Move imports to another file
+from atomrdf.namespace import PROV, CMSO, PODO, ASMO
 
-#custom imports as needed
+# custom imports as needed
 import atomrdf.workflow.pyiron as pi
 
 
 class Workflow:
-    def __init__(self, kg, 
-        environment='pyiron'):
+    def __init__(self, kg, environment="pyiron"):
         """
         Initialize the workflow environment
 
         Parameters
         ----------
         kg: pyscal-rdf KnowledgeGraph
         environment: string
             the workflow environment. This is used to import the necessary functions.
 
         """
         self.kg = kg
-        if environment == 'pyiron':
+        if environment == "pyiron":
             self.wenv = pi
         else:
-            raise ValueError('unknow workflow environment')
+            raise ValueError("unknown workflow environment")
 
     def _prepare_job(self, workflow_object):
+
         self.wenv._check_if_job_is_valid(workflow_object)
-        parent_structure, parent_sample, structure, sample = self.wenv._add_structures(workflow_object)
+        parent_structure, parent_sample, structure, sample = self.wenv._add_structures(
+            workflow_object
+        )
         method_dict = self.wenv._identify_method(workflow_object)
 
         if (structure is None) and (sample is None):
-            raise ValueError('Either structure or sample should be specified')
+            raise ValueError("Either structure or sample should be specified")
 
         if sample is None:
-            #its not added to graph yet
+            # its not added to graph yet
             structure.graph = self.kg
             structure.to_graph()
             sample = structure.sample
-        
+
         if parent_sample is None:
-            #its not added to graph yet
-            parent_structure.graph = self.kg
-            parent_structure.to_graph()
-            parent_sample = parent_structure.sample
+            # its not added to graph yet
+            if parent_structure is not None:
+                parent_structure.graph = self.kg
+                parent_structure.to_graph()
+                parent_sample = parent_structure.sample
 
+        self.structure = structure
         self.sample = sample
         self.mdict = method_dict
+        self.main_id = method_dict["id"]
         self.parent_sample = parent_sample
 
-    def _add_inherited_properties(self, ):
-        #Here we need to add inherited info: CalculatedProperties will be lost
-        #Defects will be inherited
+    def _get_lattice_properties(
+        self,
+    ):
+        if self.parent_sample is None:
+            return
+
+        material = list(
+            [
+                k[2]
+                for k in self.kg.triples((self.parent_sample, CMSO.hasMaterial, None))
+            ]
+        )[0]
+        crystal_structure = self.kg.value(material, CMSO.hasStructure)
+
+        altname = self.kg.value(crystal_structure, CMSO.hasAltName)
+
+        space_group = self.kg.value(crystal_structure, CMSO.hasSpaceGroup)
+        space_group_symbol = self.kg.value(space_group, CMSO.hasSpaceGroupSymbol)
+        space_group_number = self.kg.value(space_group, CMSO.hasSpaceGroupNumber)
+
+        unit_cell = self.kg.value(crystal_structure, CMSO.hasUnitCell)
+        blattice = self.kg.value(
+            unit_cell,
+            Namespace("http://purls.helmholtz-metadaten.de/cmso/").hasBravaisLattice,
+        )
+
+        lattice_parameter = self.kg.value(unit_cell, CMSO.hasLatticeParameter)
+        lattice_parameter_x = self.kg.value(lattice_parameter, CMSO.hasLength_x)
+        lattice_parameter_y = self.kg.value(lattice_parameter, CMSO.hasLength_y)
+        lattice_parameter_z = self.kg.value(lattice_parameter, CMSO.hasLength_z)
+
+        lattice_angle = self.kg.value(unit_cell, CMSO.hasAngle)
+        lattice_angle_x = self.kg.value(lattice_angle, CMSO.hasAngle_alpha)
+        lattice_angle_y = self.kg.value(lattice_angle, CMSO.hasAngle_beta)
+        lattice_angle_z = self.kg.value(lattice_angle, CMSO.hasAngle_gamma)
+
+        targets = [
+            altname,
+            space_group_symbol,
+            space_group_number,
+            blattice,
+            [lattice_parameter_x, lattice_parameter_y, lattice_parameter_z],
+            [lattice_angle_x, lattice_angle_y, lattice_angle_z],
+        ]
+
+        self.structure._add_crystal_structure(targets=targets)
+
+    def _add_inherited_properties(
+        self,
+    ):
+        # Here we need to add inherited info: CalculatedProperties will be lost
+        # Defects will be inherited
         if self.parent_sample is None:
             return
 
-        parent_material = list([k[2] for k in self.kg.graph.triples((self.parent_sample, CMSO.hasMaterial, None))])[0]
-        parent_defects = list([x[2] for x in self.kg.graph.triples((parent_material, CMSO.hasDefect, None))])
-        #now for each defect we copy add this to the final sample
-        material = list([k[2] for k in self.kg.graph.triples((self.sample, CMSO.hasMaterial, None))])[0]
+        parent_material = list(
+            [
+                k[2]
+                for k in self.kg.triples((self.parent_sample, CMSO.hasMaterial, None))
+            ]
+        )[0]
+        parent_defects = list(
+            [x[2] for x in self.kg.triples((parent_material, CMSO.hasDefect, None))]
+        )
+        # now for each defect we copy add this to the final sample
+        material = list(
+            [k[2] for k in self.kg.triples((self.sample, CMSO.hasMaterial, None))]
+        )[0]
 
         for defect in parent_defects:
             new_defect = URIRef(defect.toPython())
-            self.kg.graph.add((material, CMSO.hasDefect, new_defect))
-            #now fetch all defect based info
-            for triple in self.kg.graph.triples((defect, None, None)):
-                self.kg.graph.add((new_defect, triple[1], triple[2]))
-
-        #now add the special props for vacancy
-        parent_simcell = self.kg.graph.value(self.sample, CMSO.hasSimulationCell)
-        simcell = self.kg.graph.value(self.parent_sample, CMSO.hasSimulationCell) 
-        
-        for triple in self.kg.graph.triples((parent_simcell, PODO.hasVacancyConcentration, None)):
-            self.kg.graph.add((simcell, triple[1], triple[2]))
-        for triple in self.kg.graph.triples((parent_simcell, PODO.hasNumberOfVacancies, None)):
-            self.kg.graph.add((simcell, triple[1], triple[2]))
-
-    def _get_lattice_properties(self, ):
-        if self.parent_sample is None:
-            return
+            self.kg.add((material, CMSO.hasDefect, new_defect))
+            # now fetch all defect based info
+            for triple in self.kg.triples((defect, None, None)):
+                self.kg.add((new_defect, triple[1], triple[2]))
+
+        # now add the special props for vacancy
+        parent_simcell = self.kg.value(self.sample, CMSO.hasSimulationCell)
+        simcell = self.kg.value(self.parent_sample, CMSO.hasSimulationCell)
+
+        for triple in self.kg.triples(
+            (parent_simcell, PODO.hasVacancyConcentration, None)
+        ):
+            self.kg.add((simcell, triple[1], triple[2]))
+        for triple in self.kg.triples(
+            (parent_simcell, PODO.hasNumberOfVacancies, None)
+        ):
+            self.kg.add((simcell, triple[1], triple[2]))
+
+    def add_structural_relation(
+        self,
+    ):
+        """
+        Add structural relation between samples.
 
-        parent_material = list([k[2] for k in self.kg.graph.triples((self.parent_sample, CMSO.hasMaterial, None))])[0]
-        parent_crystal_structure = self.kg.graph.value(parent_material, CMSO.hasStructure)
-        parent_altname = self.kg.graph.value(parent_crystal_structure, CMSO.hasAltName)
-
-        #add this to new structure
-        material = list([k[2] for k in self.kg.graph.triples((self.sample, CMSO.hasMaterial, None))])[0]
-        crystal_structure = self.kg.graph.value(material, CMSO.hasStructure)
-        self.kg.add((crystal_structure, CMSO.hasAltName, parent_altname))
-
-        #space group
-        parent_space_group = self.kg.graph.value(parent_crystal_structure, CMSO.hasSpaceGroup)
-        space_group = self.kg.graph.value(crystal_structure, CMSO.hasSpaceGroup)
-        for triple in self.kg.graph.triples((parent_space_group, None, None)):
-            self.kg.graph.add((space_group, triple[1], triple[2]))
-
-        #unit cell
-        parent_unit_cell = self.kg.graph.value(parent_crystal_structure, CMSO.hasUnitCell)
-        parent_bv = self.kg.graph.value(parent_unit_cell, CMSO.hasBravaisLattice)
-
-        unit_cell = self.kg.graph.value(crystal_structure, CMSO.hasUnitCell)
-        self.kg.graph.add((unit_cell, CMSO.hasBravaisLattice, parent_bv))
-
-        #lattice parameter
-        parent_lattice_parameter = self.kg.graph.value(parent_unit_cell, CMSO.hasLatticeParameter)
-        lattice_parameter = self.kg.graph.value(unit_cell, CMSO.hasLatticeParameter)
-        for triple in self.kg.graph.triples((parent_lattice_parameter, None, None)):
-            self.kg.graph.add((lattice_parameter, triple[1], triple[2]))
-
-        #lattice angle
-        parent_lattice_angle = self.kg.graph.value(parent_unit_cell, CMSO.hasAngle)
-        lattice_angle = self.kg.graph.value(unit_cell, CMSO.hasAngle)
-        for triple in self.kg.graph.triples((parent_lattice_angle, None, None)):
-            self.kg.graph.add((lattice_angle, triple[1], triple[2]))
+        This method adds the structural relation between the current sample and its parent sample.
+        It also retrieves lattice properties and adds inherited properties, such as defect information.
 
+        Parameters
+        ----------
+        None
 
-    def add_structural_relation(self, ):
+        Returns
+        -------
+        None
+        """
         self.kg.add((self.sample, RDF.type, PROV.Entity))
         if self.parent_sample is not None:
             self.kg.add((self.parent_sample, RDF.type, PROV.Entity))
             self.kg.add((self.sample, PROV.wasDerivedFrom, self.parent_sample))
-            self._add_inherited_properties()
             self._get_lattice_properties()
+            self._add_inherited_properties()
 
-
-    def add_method(self, ):
+    def add_method(
+            self,
+        ):
         """
-        mdict
+        Add the computational method and related information to the knowledge graph.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+
+        Notes
         -----
-        md:
-           method: MolecularStatics
-           temperature: 100
-           pressure: 0
-           dof:
-             - AtomicPositions
-             - CellVolume
-           ensemble: NPT
-           id: 2314
-           potential:
-             uri: https://doi.org/xxx
-             type: eam
-             label: string
-           workflow_manager:
-             uri: xxxx
-             label: pyiron
-           software:
-           - uri: xxxx
-             label: lammps
-           - uri: xxxx
-             label: pyscal
+        This method adds the computational method and related information to the knowledge graph.
+        It creates an activity node representing the method and adds it to the graph.
+        The method is associated with the main activity using the `ASMO.hasComputationalMethod` property.
+        The type of the method is determined based on the value of the `method` key in the `mdict` dictionary.
+        The method-specific items are added to the graph based on the method type.
+        The structure generation information is also added to the graph.
 
         """
         if self.mdict is None:
             return
 
-        if 'md' in self.mdict.keys():
-            method_type = 'md'
-            mdict = self.mdict['md']
-        elif 'dft' in self.mdict.keys():
-            method_type = 'dft'
-            mdict = self.mdict['dft']
-        else:
-            raise KeyError('method dict keys should be either md or dft')
-
-        
-        #add activity
-        main_id = mdict['id']
-        activity = URIRef(f'activity:{main_id}')
+        # add activity
+        # ----------------------------------------------------------
+        activity = URIRef(f"activity_{self.main_id}")
         self.kg.add((activity, RDF.type, PROV.Activity))
 
-        #method, this is specific to dft/md
-        if method_type == 'md':
-            method = URIRef(f'method:{main_id}')
-            if mdict['method'] == 'MolecularStatics':
-                self.kg.add((method, RDF.type, ASO.MolecularStatics))
-            elif mdict['method'] == 'MolecularDynamics':
-                self.kg.add((method, RDF.type, ASO.MolecularDynamics))
-        elif method_type == 'dft':
-            method = URIRef(f'method:{main_id}')
-            if mdict['method'] == 'DensityFunctionalTheory':
-                self.kg.add((method, RDF.type, ASO.DensityFunctionalTheory))
-        self.kg.add((activity, ASO.hasMethod, method))
-
-        if len(mdict['dof']) == 0:
-            self.kg.add((activity, RDF.type, ASO.RigidEnergyCalculation))
+        # add method
+        # ----------------------------------------------------------
+        method = URIRef(f"method_{self.main_id}")
+        if self.mdict["method"] == "MolecularStatics":
+            self.kg.add((method, RDF.type, ASMO.MolecularStatics))
+        elif self.mdict["method"] == "MolecularDynamics":
+            self.kg.add((method, RDF.type, ASMO.MolecularDynamics))
+        elif self.mdict["method"] == "DensityFunctionalTheory":
+            self.kg.add((method, RDF.type, ASMO.DensityFunctionalTheory))
+        self.kg.add((activity, ASMO.hasComputationalMethod, method))
+
+        # choose if its rigid energy or structure optimisation
+        # ----------------------------------------------------------
+        if len(self.mdict["dof"]) == 0:
+            self.kg.add(
+                (
+                    activity,
+                    RDF.type,
+                    Namespace(
+                        "http://purls.helmholtz-metadaten.de/asmo/"
+                    ).RigidEnergyCalculation,
+                )
+            )
         else:
-            self.kg.add((activity, RDF.type, ASO.StructureOptimization))
+            self.kg.add((activity, RDF.type, ASMO.StructureOptimization))
+        # add DOFs
+        for dof in self.mdict["dof"]:
+            self.kg.add((activity, ASMO.hasRelaxationDOF, getattr(ASMO, dof)))
+
+        # add method specific items
+        if self.mdict["method"] in ["MolecularStatics", "MolecularDynamics"]:
+            self._add_md(method, activity)
+        elif self.mdict["method"] in ["DensityFunctionalTheory"]:
+            self._add_dft(method, activity)
 
-        for dof in mdict['dof']:
-            self.kg.add((activity, ASO.hasRelaxationDOF, getattr(ASO, dof)))
-
-        if method_type == 'md':
-            self.kg.add((method, ASO.hasStatisticalEnsemble, getattr(ASO, mdict['ensemble'])))
+        # add that structure was generated
+        self.kg.add((self.sample, PROV.wasGeneratedBy, activity))
+        self._add_inputs(activity)
+        self._add_outputs(activity)
+        self._add_software(method)
 
-            #add temperature if needed
-            if mdict['temperature'] is not None:
-                temperature = URIRef(f'temperature:{main_id}')
-                self.kg.add((temperature, RDF.type, ASO.InputParameter))
-                self.kg.add((temperature, RDFS.label, Literal('temperature', datatype=XSD.string)))
-                self.kg.add((activity, ASO.hasInputParameter, temperature))
-                self.kg.add((temperature, ASO.hasValue, Literal(mdict['temperature'], datatype=XSD.float)))
-                self.kg.add((temperature, ASO.hasUnit, URIRef('http://qudt.org/vocab/unit/K')))
-
-            if mdict['pressure'] is not None:
-                pressure = URIRef(f'pressure:{main_id}')
-                self.kg.add((pressure, RDF.type, ASO.InputParameter))
-                self.kg.add((pressure, RDFS.label, Literal('pressure', datatype=XSD.string)))
-                self.kg.add((activity, ASO.hasInputParameter, pressure))
-                self.kg.add((pressure, ASO.hasValue, Literal(mdict['pressure'], datatype=XSD.float)))
-                self.kg.add((pressure, ASO.hasUnit, URIRef('http://qudt.org/vocab/unit/GigaPA')))
-
-            #potentials need to be mapped
-            potential = URIRef(f'potential:{main_id}')
-            if 'meam' in mdict['potential']['type']:
-                self.kg.add((potential, RDF.type, ASO.MEAM))
-            elif 'eam' in mdict['potential']['type']:
-                self.kg.add((potential, RDF.type, ASO.EAM))
-            elif 'lj' in mdict['potential']['type']:
-                self.kg.add((potential, RDF.type, ASO.LennardJones))
-            elif 'ace' in mdict['potential']['type']:
-                self.kg.add((potential, RDF.type, ASO.MLPotential))
-            else:
-                self.kg.add((potential, RDF.type, ASO.InteratomicPotential))
+    def to_graph(self, workflow_object):
+        """
+        Converts a workflow object to a graph representation.
 
-            if 'uri' in mdict['potential'].keys():
-                self.kg.add((potential, ASO.hasReference, Literal(mdict['potential']['uri'])))
-            if 'label' in mdict['potential'].keys():
-                self.kg.add((potential, RDFS.label, Literal(mdict['potential']['label'])))
+        Parameters:
+        - workflow_object: The workflow object to convert.
 
-            self.kg.add((method, ASO.hasInteratomicPotential, potential))
+        Returns:
+        - None
+        """
+        self._prepare_job(workflow_object)
+        self.add_structural_relation()
+        self.add_method()
 
-        self.kg.add((self.sample, PROV.wasGeneratedBy, activity))
+    def _add_outputs(self, activity):
+        if "outputs" in self.mdict.keys():
+            for out in self.mdict["outputs"]:
+                prop = self.kg.create_node(
+                    f'{self.main_id}_{out["label"]}', CMSO.CalculatedProperty
+                )
+                self.kg.add((prop, RDFS.label, Literal(out["label"])))
+                self.kg.add((prop, ASMO.hasValue, Literal(out["value"])))
+                if "unit" in out.keys():
+                    unit = out["unit"]
+                    self.kg.add(
+                        (
+                            prop,
+                            ASMO.hasUnit,
+                            URIRef(f"http://qudt.org/vocab/unit/{unit}"),
+                        )
+                    )
+                self.kg.add((prop, ASMO.wasCalculatedBy, activity))
+                if out["associate_to_sample"]:
+                    self.kg.add((self.sample, CMSO.hasCalculatedProperty, prop))
+
+    def _add_inputs(self, activity):
+        if "inputs" in self.mdict.keys():
+            for inp in self.mdict["inputs"]:
+                prop = self.kg.create_node(
+                    f'{self.main_id}_{inp["label"]}', ASMO.InputParameter
+                )
+                self.kg.add((prop, RDFS.label, Literal(inp["label"])))
+                self.kg.add((prop, ASMO.hasValue, Literal(inp["value"])))
+                if "unit" in inp.keys():
+                    unit = inp["unit"]
+                    self.kg.add(
+                        (
+                            prop,
+                            ASMO.hasUnit,
+                            URIRef(f"http://qudt.org/vocab/unit/{unit}"),
+                        )
+                    )
+                self.kg.add((activity, ASMO.hasInputParameter, prop))
 
-        #finally add software
+    def _add_software(self, method):
+        # finally add software
         wfagent = None
-        if 'workflow_manager' in mdict.keys():
-            wfagent = URIRef(mdict["workflow_manager"]['uri'])
-            self.kg.add((wfagent, RDF.type, PROV.SoftwareAgent))
-            self.kg.add((wfagent, RDFS.label, Literal(mdict["workflow_manager"]['label'])))
+        if "workflow_manager" in self.mdict.keys():
+            wfagent = self.kg.create_node(
+                self.mdict["workflow_manager"]["uri"], PROV.SoftwareAgent
+            )
+            self.kg.add(
+                (wfagent, RDFS.label, Literal(self.mdict["workflow_manager"]["label"]))
+            )
             self.kg.add((method, PROV.wasAssociatedWith, wfagent))
-        
-        for software in mdict['software']:
-            agent = URIRef(software['uri'])
-            self.kg.add((agent, RDF.type, PROV.SoftwareAgent))
-            self.kg.add((agent, RDFS.label, Literal(software['label'])))
 
+        for software in self.mdict["software"]:
+            agent = self.kg.create_node(software["uri"], PROV.SoftwareAgent)
+            self.kg.add((agent, RDFS.label, Literal(software["label"])))
             if wfagent is not None:
                 self.kg.add((wfagent, PROV.actedOnBehalfOf, agent))
             else:
                 self.kg.add((method, PROV.wasAssociatedWith, agent))
 
-        for key, val in mdict['outputs'].items():
-            prop = URIRef(f'{main_id}_{key}')
-            self.kg.add((prop, RDF.type, CMSO.CalculatedProperty))
-            self.kg.add((prop, RDFS.label, Literal(key)))
-            self.kg.add((prop, ASO.hasValue, Literal(val["value"])))
-            if "unit" in val.keys():
-                unit = val['unit']
-                self.kg.add((prop, ASO.hasUnit, URIRef(f'http://qudt.org/vocab/unit/{unit}')))
-            self.kg.add((prop, CMSO.wasCalculatedBy, activity))
-            if val['associate_to_sample']:
-                self.kg.add((self.sample, CMSO.hasCalculatedProperty, prop))
+    def _add_md(self, method, activity):
+        self.kg.add(
+            (method, ASMO.hasStatisticalEnsemble, getattr(ASMO, self.mdict["ensemble"]))
+        )
+
+        # add temperature if needed
+        if self.mdict["temperature"] is not None:
+            temperature = self.kg.create_node(
+                f"temperature_{self.main_id}", ASMO.InputParameter
+            )
+            self.kg.add(
+                (temperature, RDFS.label, Literal("temperature", datatype=XSD.string))
+            )
+            self.kg.add((activity, ASMO.hasInputParameter, temperature))
+            self.kg.add(
+                (
+                    temperature,
+                    ASMO.hasValue,
+                    Literal(self.mdict["temperature"], datatype=XSD.float),
+                )
+            )
+            self.kg.add(
+                (temperature, ASMO.hasUnit, URIRef("http://qudt.org/vocab/unit/K"))
+            )
+
+        if self.mdict["pressure"] is not None:
+            pressure = self.kg.create_node(
+                f"pressure_{self.main_id}", ASMO.InputParameter
+            )
+            self.kg.add(
+                (pressure, RDFS.label, Literal("pressure", datatype=XSD.string))
+            )
+            self.kg.add((activity, ASMO.hasInputParameter, pressure))
+            self.kg.add(
+                (
+                    pressure,
+                    ASMO.hasValue,
+                    Literal(self.mdict["pressure"], datatype=XSD.float),
+                )
+            )
+            self.kg.add(
+                (pressure, ASMO.hasUnit, URIRef("http://qudt.org/vocab/unit/GigaPA"))
+            )
+
+        # potentials need to be mapped
+        potential = URIRef(f"potential_{self.main_id}")
+        if "meam" in self.mdict["potential"]["type"]:
+            self.kg.add((potential, RDF.type, ASMO.ModifiedEmbeddedAtomModel))
+        elif "eam" in self.mdict["potential"]["type"]:
+            self.kg.add((potential, RDF.type, ASMO.EmbeddedAtomModel))
+        elif "lj" in self.mdict["potential"]["type"]:
+            self.kg.add((potential, RDF.type, ASMO.LennardJonesPotential))
+        elif "ace" in self.mdict["potential"]["type"]:
+            self.kg.add((potential, RDF.type, ASMO.MachineLearningPotential))
+        else:
+            self.kg.add((potential, RDF.type, ASMO.InteratomicPotential))
 
-    def to_graph(self, workflow_object):
-        self._prepare_job(workflow_object)
-        self.add_structural_relation()
-        self.add_method()
+        if "uri" in self.mdict["potential"].keys():
+            self.kg.add(
+                (
+                    potential,
+                    CMSO.hasReference,
+                    Literal(self.mdict["potential"]["uri"], datatype=XSD.string),
+                )
+            )
+        if "label" in self.mdict["potential"].keys():
+            self.kg.add(
+                (potential, RDFS.label, Literal(self.mdict["potential"]["label"]))
+            )
+
+        self.kg.add((method, ASMO.hasInteratomicPotential, potential))
```

### Comparing `atomrdf-0.4.4/atomrdf.egg-info/PKG-INFO` & `atomrdf-0.6.0/atomrdf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.4.4
+Version: 0.6.0
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -21,14 +21,18 @@
 Requires-Dist: owlready2
 
 # atomRDF
 
 > [!NOTE]
 > `atomRDF` was previously called `pyscal-rdf`. 
 
+[![codecov](https://codecov.io/gh/pyscal/atomRDF/graph/badge.svg?token=X7S3TP2MP6)](https://codecov.io/gh/pyscal/atomRDF)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/atomrdf.svg)](https://anaconda.org/conda-forge/atomrdf)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atomrdf?label=pypi&link=https%3A%2F%2Fpypi.org%2Fproject%2Fatomrdf%2F)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10973374.svg)](https://doi.org/10.5281/zenodo.10973374)
 
 `atomRDF` is a python tool for ontology-based creation, manipulation, and quering of structures. `atomRDF` uses the [Computational Material Sample Ontology (CMSO)](https://github.com/Materials-Data-Science-and-Informatics/cmso-ontology). 
 
 The package is currently under activate development and could be  unstable .
 
 More details coming soon...
```

### Comparing `atomrdf-0.4.4/atomrdf.egg-info/SOURCES.txt` & `atomrdf-0.6.0/atomrdf.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 MANIFEST.in
 README.md
 setup.py
 atomrdf/__init__.py
 atomrdf/encoder.py
 atomrdf/graph.py
 atomrdf/json_io.py
+atomrdf/namespace.py
 atomrdf/properties.py
 atomrdf/stores.py
 atomrdf/structure.py
 atomrdf/visualize.py
 atomrdf.egg-info/PKG-INFO
 atomrdf.egg-info/SOURCES.txt
 atomrdf.egg-info/dependency_links.txt
 atomrdf.egg-info/not-zip-safe
 atomrdf.egg-info/requires.txt
 atomrdf.egg-info/top_level.txt
 atomrdf/data/asmo.owl
 atomrdf/data/cmso.owl
+atomrdf/data/dft_template.yml
 atomrdf/data/element.yml
+atomrdf/data/md_template.yml
 atomrdf/data/pldo.owl
 atomrdf/data/podo.owl
 atomrdf/network/__init__.py
 atomrdf/network/network.py
 atomrdf/network/ontology.py
 atomrdf/network/parser.py
 atomrdf/network/patch.py
 atomrdf/network/term.py
 atomrdf/workflow/__init__.py
 atomrdf/workflow/pyiron.py
 atomrdf/workflow/workflow.py
 tests/test_encoder_and_write.py
 tests/test_graph.py
-tests/test_structuregraph.py
+tests/test_network.py
+tests/test_store.py
+tests/test_structure.py
+tests/test_structuregraph.py
+tests/test_term.py
+tests/test_visualise.py
+tests/test_workflow.py
```

### Comparing `atomrdf-0.4.4/setup.py` & `atomrdf-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='atomrdf',
-    version='0.4.4',
+    version='0.6.0',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['atomrdf', 'atomrdf.*']),
     zip_safe=False,
```

### Comparing `atomrdf-0.4.4/tests/test_encoder_and_write.py` & `atomrdf-0.6.0/tests/test_encoder_and_write.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,12 +7,18 @@
 
 def test_encoder():
     arr = np.linspace(0, 10, 100)
     data = {"array": arr}
     dumpdata = json.dumps(data, cls=NumpyArrayEncoder)
     assert(np.abs(float(dumpdata.split(',')[-2]) - arr[-2]) < 1E-5)
 
+    enc = NumpyArrayEncoder()
+    assert type(enc.default(np.float64(23))) == float
+    assert type(enc.default(np.int64(23))) == int
+    assert type(enc.default(np.array([23]))) == list
+
 def test_writer(tmp_path):
     arr = np.linspace(0, 10, 100)
     data = {"array": arr}
     write_file("test_json", data)
-    assert(os.path.exists("test_json.json"))
+    assert(os.path.exists("test_json.json"))
+
```

### Comparing `atomrdf-0.4.4/tests/test_structuregraph.py` & `atomrdf-0.6.0/tests/test_structuregraph.py`

 * *Files identical despite different names*

