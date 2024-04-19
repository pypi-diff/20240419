# Comparing `tmp/skytek-generic-map-api-0.8.2.tar.gz` & `tmp/skytek_generic_map_api-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek-generic-map-api-0.8.2.tar", last modified: Wed Mar 20 13:11:57 2024, max compression
+gzip compressed data, was "skytek_generic_map_api-0.8.4.tar", last modified: Fri Apr 19 08:45:32 2024, max compression
```

## Comparing `skytek-generic-map-api-0.8.2.tar` & `skytek_generic_map_api-0.8.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.837804 skytek-generic-map-api-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-20 13:11:57.837804 skytek-generic-map-api-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.833804 skytek-generic-map-api-0.8.2/generic_map_api/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-20 13:11:55.000000 skytek-generic-map-api-0.8.2/generic_map_api/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/date_line_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/geometry_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.833804 skytek-generic-map-api-0.8.2/generic_map_api/multi_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/multi_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/multi_meta/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/multi_meta/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.833804 skytek-generic-map-api-0.8.2/generic_map_api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/resources/empty_tile.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.837804 skytek-generic-map-api-0.8.2/generic_map_api/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/resources/icons/default-features.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/resources/icons/default-tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/resources/icons/default.png
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/generic_map_api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.837804 skytek-generic-map-api-0.8.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 13:11:57.837804 skytek-generic-map-api-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.837804 skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-20 13:11:57.000000 skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-20 13:11:57.000000 skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:11:57.000000 skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:11:57.000000 skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-20 13:11:57.000000 skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 13:11:57.000000 skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:11:57.837804 skytek-generic-map-api-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-20 13:11:51.000000 skytek-generic-map-api-0.8.2/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.316545 skytek_generic_map_api-0.8.4/generic_map_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 08:45:30.000000 skytek_generic_map_api-0.8.4/generic_map_api/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/date_line_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/geometry_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.316545 skytek_generic_map_api-0.8.4/generic_map_api/multi_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/multi_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/multi_meta/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/multi_meta/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/generic_map_api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/resources/empty_tile.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/generic_map_api/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/resources/icons/default-features.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/resources/icons/default-tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/resources/icons/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/generic_map_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-19 08:45:32.000000 skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 08:45:32.000000 skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:45:32.000000 skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:45:32.000000 skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 08:45:32.000000 skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 08:45:32.000000 skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:45:32.320545 skytek_generic_map_api-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-19 08:45:28.000000 skytek_generic_map_api-0.8.4/tests/test_values.py
```

### Comparing `skytek-generic-map-api-0.8.2/LICENSE` & `skytek_generic_map_api-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/PKG-INFO` & `skytek_generic_map_api-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-generic-map-api
-Version: 0.8.2
+Version: 0.8.4
 Summary: skytek-generic-map-api - expose geographical data for Skytek's frontends
 Home-page: http://github.com/Skytek/generic-map-api
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/clustering.py` & `skytek_generic_map_api-0.8.4/generic_map_api/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Tuple
 
 import numpy as np
-from django.db import connections
+from django.db import DEFAULT_DB_ALIAS, connections
 from django.db.models import QuerySet
 from shapely import wkb
 from shapely.geometry import LineString, MultiPoint, MultiPolygon, Point
 from sklearn.cluster import DBSCAN
 
 if TYPE_CHECKING:
     from .values import BaseViewPort
@@ -44,14 +44,15 @@
     def get_clustering_config(self, view, viewport):  # pylint: disable=unused-argument
         return {
             "include_orphans": True,
             "geometry_field": self.DEFAULT_GEOMETRY_FIELD,
             "min_cluster_size": self.DEFAULT_MIN_CLUSTER_SIZE,
             "num_clusters": self.DEFAULT_NUM_CLUSTERS,
             "radius": self.DEFAULT_RADIUS,
+            "db_alias": None,
         }
 
     def get_clustering_function_sql_with_params(
         self, config
     ) -> Tuple[str, Tuple[Any, ...]]:
         geometry_field = config["geometry_field"]
         num_clusters = config["num_clusters"]
@@ -73,14 +74,15 @@
             raise ValueError("Database clustering requires QuerySet on input")
 
         config = self.get_clustering_config(view, viewport)
 
         include_orphans = config["include_orphans"]
         geometry_field = config["geometry_field"]
         min_cluster_size = config["min_cluster_size"]
+        db_alias = config["db_alias"] or items.db or DEFAULT_DB_ALIAS
 
         viewport_wkb = None
         if viewport:
             viewport_polygon = viewport.to_polygon()
             viewport_wkb = wkb.dumps(viewport_polygon, include_srid=True)
 
         sql, sql_params = items.query.sql_with_params()
@@ -111,15 +113,15 @@
                 + sql_params
                 + (
                     min_cluster_size,
                     viewport_wkb,
                     viewport_wkb,
                 )
             )
-            items_outside_clusters = items.model.objects.raw(
+            items_outside_clusters = items.model.objects.using(db_alias).raw(
                 items_outside_clusters_raw_sql,
                 items_outside_clusters_raw_sql_params,
             )
 
             for item in items_outside_clusters.iterator():
                 yield ClusteringOutput(
                     is_cluster=False,
@@ -146,15 +148,15 @@
             + (
                 min_cluster_size,
                 viewport_wkb,
                 viewport_wkb,
             )
         )
 
-        connection = connections[items.db]
+        connection = connections[db_alias]
         with connection.cursor() as cursor:
             cursor.execute(clusters_raw_sql, clusters_raw_sql_params)
             while row := cursor.fetchone():
                 cluster_shape = wkb.loads(row[1]).convex_hull
                 if isinstance(cluster_shape, (LineString, Point)):
                     cluster_shape = cluster_shape.buffer(0.1).convex_hull
                 shape = MultiPolygon([cluster_shape])
```

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/date_line_normalization.py` & `skytek_generic_map_api-0.8.4/generic_map_api/date_line_normalization.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/geometry_serializers.py` & `skytek_generic_map_api-0.8.4/generic_map_api/geometry_serializers.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/multi_meta/views.py` & `skytek_generic_map_api-0.8.4/generic_map_api/multi_meta/views.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/params.py` & `skytek_generic_map_api-0.8.4/generic_map_api/params.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/resources/empty_tile.png` & `skytek_generic_map_api-0.8.4/generic_map_api/resources/empty_tile.png`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/resources/icons/default-features.png` & `skytek_generic_map_api-0.8.4/generic_map_api/resources/icons/default-features.png`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/resources/icons/default-tiles.png` & `skytek_generic_map_api-0.8.4/generic_map_api/resources/icons/default-tiles.png`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/resources/icons/default.png` & `skytek_generic_map_api-0.8.4/generic_map_api/resources/icons/default.png`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/routers.py` & `skytek_generic_map_api-0.8.4/generic_map_api/routers.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/serializers.py` & `skytek_generic_map_api-0.8.4/generic_map_api/serializers.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/values.py` & `skytek_generic_map_api-0.8.4/generic_map_api/values.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/generic_map_api/views.py` & `skytek_generic_map_api-0.8.4/generic_map_api/views.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/setup.py` & `skytek_generic_map_api-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/PKG-INFO` & `skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-generic-map-api
-Version: 0.8.2
+Version: 0.8.4
 Summary: skytek-generic-map-api - expose geographical data for Skytek's frontends
 Home-page: http://github.com/Skytek/generic-map-api
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-generic-map-api-0.8.2/skytek_generic_map_api.egg-info/SOURCES.txt` & `skytek_generic_map_api-0.8.4/skytek_generic_map_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

