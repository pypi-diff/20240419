# Comparing `tmp/whyis_activitystreams-0.1.0.tar.gz` & `tmp/whyis_activitystreams-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyis_activitystreams-0.1.0.tar", last modified: Fri Apr 19 09:45:57 2024, max compression
+gzip compressed data, was "whyis_activitystreams-0.1.1.tar", last modified: Fri Apr 19 09:49:43 2024, max compression
```

## Comparing `whyis_activitystreams-0.1.0.tar` & `whyis_activitystreams-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.729310 whyis_activitystreams-0.1.0/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis_activitystreams-0.1.0/LICENSE
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 09:45:57.729310 whyis_activitystreams-0.1.0/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     3708 2024-02-06 16:09:12.000000 whyis_activitystreams-0.1.0/README.md
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-04-19 03:30:37.000000 whyis_activitystreams-0.1.0/perception_pipeline/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-04-19 03:30:08.000000 whyis_activitystreams-0.1.0/perception_pipeline/_version.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/backbone_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1185 2024-04-19 07:38:08.000000 whyis_activitystreams-0.1.0/perception_pipeline/backbone_agent/backbone_agent.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/geometric_attribute_detection_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1227 2024-04-19 07:38:13.000000 whyis_activitystreams-0.1.0/perception_pipeline/geometric_attribute_detection_agent/geometric_attribute_detection_agent.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/object_classification_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1196 2024-04-19 07:38:19.000000 whyis_activitystreams-0.1.0/perception_pipeline/object_classification_agent/object_classification_agent.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/object_detection_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1176 2024-04-19 07:38:25.000000 whyis_activitystreams-0.1.0/perception_pipeline/object_detection_agent/object_detection_agent.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/part_detection_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1165 2024-04-19 07:38:28.000000 whyis_activitystreams-0.1.0/perception_pipeline/part_detection_agent/part_detection_agent.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/photometric_attribute_detection_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1235 2024-04-19 07:38:32.000000 whyis_activitystreams-0.1.0/perception_pipeline/photometric_attribute_detection_agent/photometric_attribute_detection_agent.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/saliency_map_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1178 2024-04-19 07:38:37.000000 whyis_activitystreams-0.1.0/perception_pipeline/saliency_map_agent/saliency_map_agent.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.725310 whyis_activitystreams-0.1.0/perception_pipeline/uncertainty_attribution_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1217 2024-04-19 07:38:42.000000 whyis_activitystreams-0.1.0/perception_pipeline/uncertainty_attribution_agent/uncertainty_attribution_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1789 2024-04-19 09:45:37.000000 whyis_activitystreams-0.1.0/pyproject.toml
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-04-19 09:45:57.729310 whyis_activitystreams-0.1.0/setup.cfg
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.729310 whyis_activitystreams-0.1.0/whyis_activitystreams/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       52 2024-02-06 15:00:14.000000 whyis_activitystreams-0.1.0/whyis_activitystreams/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis_activitystreams-0.1.0/whyis_activitystreams/_version.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.729310 whyis_activitystreams-0.1.0/whyis_activitystreams/activity_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis_activitystreams-0.1.0/whyis_activitystreams/activity_agent/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1642 2024-04-19 07:27:51.000000 whyis_activitystreams-0.1.0/whyis_activitystreams/activity_agent/activity_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis_activitystreams-0.1.0/whyis_activitystreams/plugin.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:45:57.729310 whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 09:45:57.000000 whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1176 2024-04-19 09:45:57.000000 whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/SOURCES.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-04-19 09:45:57.000000 whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/dependency_links.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      963 2024-04-19 09:45:57.000000 whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/entry_points.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-04-19 09:45:57.000000 whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/requires.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       42 2024-04-19 09:45:57.000000 whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/top_level.txt
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.746492 whyis_activitystreams-0.1.1/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis_activitystreams-0.1.1/LICENSE
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 09:49:43.746492 whyis_activitystreams-0.1.1/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     3708 2024-02-06 16:09:12.000000 whyis_activitystreams-0.1.1/README.md
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-04-19 09:48:55.000000 whyis_activitystreams-0.1.1/perception_pipeline/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-04-19 03:30:08.000000 whyis_activitystreams-0.1.1/perception_pipeline/_version.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/backbone_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1185 2024-04-19 07:38:08.000000 whyis_activitystreams-0.1.1/perception_pipeline/backbone_agent/backbone_agent.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/geometric_attribute_detection_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1227 2024-04-19 07:38:13.000000 whyis_activitystreams-0.1.1/perception_pipeline/geometric_attribute_detection_agent/geometric_attribute_detection_agent.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/object_classification_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1196 2024-04-19 07:38:19.000000 whyis_activitystreams-0.1.1/perception_pipeline/object_classification_agent/object_classification_agent.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/object_detection_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1176 2024-04-19 07:38:25.000000 whyis_activitystreams-0.1.1/perception_pipeline/object_detection_agent/object_detection_agent.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/part_detection_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1165 2024-04-19 07:38:28.000000 whyis_activitystreams-0.1.1/perception_pipeline/part_detection_agent/part_detection_agent.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/photometric_attribute_detection_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1235 2024-04-19 07:38:32.000000 whyis_activitystreams-0.1.1/perception_pipeline/photometric_attribute_detection_agent/photometric_attribute_detection_agent.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/saliency_map_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1178 2024-04-19 07:38:37.000000 whyis_activitystreams-0.1.1/perception_pipeline/saliency_map_agent/saliency_map_agent.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/perception_pipeline/uncertainty_attribution_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1217 2024-04-19 07:38:42.000000 whyis_activitystreams-0.1.1/perception_pipeline/uncertainty_attribution_agent/uncertainty_attribution_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1789 2024-04-19 09:49:18.000000 whyis_activitystreams-0.1.1/pyproject.toml
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-04-19 09:49:43.746492 whyis_activitystreams-0.1.1/setup.cfg
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.742492 whyis_activitystreams-0.1.1/whyis_activitystreams/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       52 2024-02-06 15:00:14.000000 whyis_activitystreams-0.1.1/whyis_activitystreams/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis_activitystreams-0.1.1/whyis_activitystreams/_version.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.746492 whyis_activitystreams-0.1.1/whyis_activitystreams/activity_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis_activitystreams-0.1.1/whyis_activitystreams/activity_agent/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1642 2024-04-19 07:27:51.000000 whyis_activitystreams-0.1.1/whyis_activitystreams/activity_agent/activity_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis_activitystreams-0.1.1/whyis_activitystreams/plugin.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 09:49:43.746492 whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 09:49:43.000000 whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1176 2024-04-19 09:49:43.000000 whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-04-19 09:49:43.000000 whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      963 2024-04-19 09:49:43.000000 whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/entry_points.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-04-19 09:49:43.000000 whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/requires.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       42 2024-04-19 09:49:43.000000 whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/top_level.txt
```

### Comparing `whyis_activitystreams-0.1.0/LICENSE` & `whyis_activitystreams-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/README.md` & `whyis_activitystreams-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/backbone_agent/backbone_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/backbone_agent/backbone_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/geometric_attribute_detection_agent/geometric_attribute_detection_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/geometric_attribute_detection_agent/geometric_attribute_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/object_classification_agent/object_classification_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/object_classification_agent/object_classification_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/object_detection_agent/object_detection_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/object_detection_agent/object_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/part_detection_agent/part_detection_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/part_detection_agent/part_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/photometric_attribute_detection_agent/photometric_attribute_detection_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/photometric_attribute_detection_agent/photometric_attribute_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/saliency_map_agent/saliency_map_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/saliency_map_agent/saliency_map_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/perception_pipeline/uncertainty_attribution_agent/uncertainty_attribution_agent.py` & `whyis_activitystreams-0.1.1/perception_pipeline/uncertainty_attribution_agent/uncertainty_attribution_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/pyproject.toml` & `whyis_activitystreams-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='whyis-activitystreams'
-version='0.1.0'
+version='0.1.1'
 description = "A whyis plugin to support the interpretation of activity streams."
 dependencies=[
   'whyis',
 ]
 
 [tool.setuptools]
 packages=[
```

### Comparing `whyis_activitystreams-0.1.0/whyis_activitystreams/activity_agent/activity_agent.py` & `whyis_activitystreams-0.1.1/whyis_activitystreams/activity_agent/activity_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/SOURCES.txt` & `whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.1.0/whyis_activitystreams.egg-info/entry_points.txt` & `whyis_activitystreams-0.1.1/whyis_activitystreams.egg-info/entry_points.txt`

 * *Files identical despite different names*

