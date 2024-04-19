# Comparing `tmp/whyis_activitystreams-0.0.5.tar.gz` & `tmp/whyis_activitystreams-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyis_activitystreams-0.0.5.tar", last modified: Fri Apr 19 06:52:31 2024, max compression
+gzip compressed data, was "whyis_activitystreams-0.0.6.tar", last modified: Fri Apr 19 07:44:39 2024, max compression
```

## Comparing `whyis_activitystreams-0.0.5.tar` & `whyis_activitystreams-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,31 @@
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.156129 whyis_activitystreams-0.0.5/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis_activitystreams-0.0.5/LICENSE
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     3708 2024-02-06 16:09:12.000000 whyis_activitystreams-0.0.5/README.md
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      517 2024-04-19 03:26:36.000000 whyis_activitystreams-0.0.5/pyproject.toml
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-04-19 06:52:31.156129 whyis_activitystreams-0.0.5/setup.cfg
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/whyis_activitystreams/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       52 2024-02-06 15:00:14.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/_version.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/whyis_activitystreams/activity_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/activity_agent/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1650 2024-04-19 04:22:39.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/activity_agent/activity_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/plugin.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      508 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/SOURCES.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/dependency_links.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      150 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/entry_points.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/requires.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       22 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/top_level.txt
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:44:39.790505 whyis_activitystreams-0.0.6/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis_activitystreams-0.0.6/LICENSE
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 07:44:39.790505 whyis_activitystreams-0.0.6/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     3708 2024-02-06 16:09:12.000000 whyis_activitystreams-0.0.6/README.md
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:44:39.786505 whyis_activitystreams-0.0.6/perception_pipeline/
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:44:39.786505 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-04-19 07:40:33.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1185 2024-04-19 07:38:08.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/backbone_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1227 2024-04-19 07:38:13.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/geometric_attribute_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1196 2024-04-19 07:38:19.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/object_classification_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1176 2024-04-19 07:38:25.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/object_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1165 2024-04-19 07:38:28.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/part_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1235 2024-04-19 07:38:32.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/photometric_attribute_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1178 2024-04-19 07:38:37.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/saliency_map_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1217 2024-04-19 07:38:42.000000 whyis_activitystreams-0.0.6/perception_pipeline/pipeline_agent/uncertainty_attribution_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1385 2024-04-19 07:44:28.000000 whyis_activitystreams-0.0.6/pyproject.toml
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-04-19 07:44:39.790505 whyis_activitystreams-0.0.6/setup.cfg
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:44:39.786505 whyis_activitystreams-0.0.6/whyis_activitystreams/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       52 2024-02-06 15:00:14.000000 whyis_activitystreams-0.0.6/whyis_activitystreams/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis_activitystreams-0.0.6/whyis_activitystreams/_version.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:44:39.790505 whyis_activitystreams-0.0.6/whyis_activitystreams/activity_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis_activitystreams-0.0.6/whyis_activitystreams/activity_agent/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1642 2024-04-19 07:27:51.000000 whyis_activitystreams-0.0.6/whyis_activitystreams/activity_agent/activity_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis_activitystreams-0.0.6/whyis_activitystreams/plugin.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:44:39.790505 whyis_activitystreams-0.0.6/whyis_activitystreams.egg-info/
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 07:44:39.000000 whyis_activitystreams-0.0.6/whyis_activitystreams.egg-info/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1069 2024-04-19 07:44:39.000000 whyis_activitystreams-0.0.6/whyis_activitystreams.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-04-19 07:44:39.000000 whyis_activitystreams-0.0.6/whyis_activitystreams.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      963 2024-04-19 07:44:39.000000 whyis_activitystreams-0.0.6/whyis_activitystreams.egg-info/entry_points.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-04-19 07:44:39.000000 whyis_activitystreams-0.0.6/whyis_activitystreams.egg-info/requires.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       42 2024-04-19 07:44:39.000000 whyis_activitystreams-0.0.6/whyis_activitystreams.egg-info/top_level.txt
```

### Comparing `whyis_activitystreams-0.0.5/LICENSE` & `whyis_activitystreams-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.5/README.md` & `whyis_activitystreams-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.5/whyis_activitystreams/activity_agent/activity_agent.py` & `whyis_activitystreams-0.0.6/whyis_activitystreams/activity_agent/activity_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from whyis.namespace import NS
 
 from whyis.plugin import Plugin
 import rdflib
 from flask import current_app
 
 
-from whyis.namespace import sioc_types, sioc, schema, sio, dc, prov, whyis
+from whyis.namespace import sioc_types, sioc, sio, dc, prov, whyis
 
 prefixes = dict(
     skos = rdflib.URIRef("http://www.w3.org/2004/02/skos/core#"),
     foaf = rdflib.URIRef("http://xmlns.com/foaf/0.1/"),
     text = rdflib.URIRef("http://jena.apache.org/fulltext#"),
     schema = rdflib.URIRef("http://schema.org/"),
     owl = rdflib.OWL,
```

