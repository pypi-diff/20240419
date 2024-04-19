# Comparing `tmp/whyis_activitystreams-0.0.7.tar.gz` & `tmp/whyis_activitystreams-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyis_activitystreams-0.0.7.tar", last modified: Fri Apr 19 07:48:32 2024, max compression
+gzip compressed data, was "whyis_activitystreams-0.0.8.tar", last modified: Fri Apr 19 07:57:08 2024, max compression
```

## Comparing `whyis_activitystreams-0.0.7.tar` & `whyis_activitystreams-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:48:32.678182 whyis_activitystreams-0.0.7/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis_activitystreams-0.0.7/LICENSE
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 07:48:32.678182 whyis_activitystreams-0.0.7/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     3708 2024-02-06 16:09:12.000000 whyis_activitystreams-0.0.7/README.md
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:48:32.674182 whyis_activitystreams-0.0.7/perception_pipeline/
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:48:32.674182 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-04-19 07:40:33.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1185 2024-04-19 07:38:08.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/backbone_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1227 2024-04-19 07:38:13.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/geometric_attribute_detection_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1196 2024-04-19 07:38:19.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/object_classification_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1176 2024-04-19 07:38:25.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/object_detection_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1165 2024-04-19 07:38:28.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/part_detection_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1235 2024-04-19 07:38:32.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/photometric_attribute_detection_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1178 2024-04-19 07:38:37.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/saliency_map_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1217 2024-04-19 07:38:42.000000 whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/uncertainty_attribution_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1295 2024-04-19 07:48:15.000000 whyis_activitystreams-0.0.7/pyproject.toml
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-04-19 07:48:32.678182 whyis_activitystreams-0.0.7/setup.cfg
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:48:32.674182 whyis_activitystreams-0.0.7/whyis_activitystreams/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       52 2024-02-06 15:00:14.000000 whyis_activitystreams-0.0.7/whyis_activitystreams/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis_activitystreams-0.0.7/whyis_activitystreams/_version.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:48:32.674182 whyis_activitystreams-0.0.7/whyis_activitystreams/activity_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis_activitystreams-0.0.7/whyis_activitystreams/activity_agent/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1642 2024-04-19 07:27:51.000000 whyis_activitystreams-0.0.7/whyis_activitystreams/activity_agent/activity_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis_activitystreams-0.0.7/whyis_activitystreams/plugin.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:48:32.678182 whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 07:48:32.000000 whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1069 2024-04-19 07:48:32.000000 whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/SOURCES.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-04-19 07:48:32.000000 whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/dependency_links.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      873 2024-04-19 07:48:32.000000 whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/entry_points.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-04-19 07:48:32.000000 whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/requires.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       42 2024-04-19 07:48:32.000000 whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/top_level.txt
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:57:08.821734 whyis_activitystreams-0.0.8/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis_activitystreams-0.0.8/LICENSE
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 07:57:08.821734 whyis_activitystreams-0.0.8/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     3708 2024-02-06 16:09:12.000000 whyis_activitystreams-0.0.8/README.md
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:57:08.817734 whyis_activitystreams-0.0.8/perception_pipeline/
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:57:08.817734 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1185 2024-04-19 07:38:08.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/backbone_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1227 2024-04-19 07:38:13.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/geometric_attribute_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1196 2024-04-19 07:38:19.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/object_classification_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1176 2024-04-19 07:38:25.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/object_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1165 2024-04-19 07:38:28.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/part_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1235 2024-04-19 07:38:32.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/photometric_attribute_detection_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1178 2024-04-19 07:38:37.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/saliency_map_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1217 2024-04-19 07:38:42.000000 whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/uncertainty_attribution_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1305 2024-04-19 07:56:48.000000 whyis_activitystreams-0.0.8/pyproject.toml
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-04-19 07:57:08.821734 whyis_activitystreams-0.0.8/setup.cfg
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:57:08.817734 whyis_activitystreams-0.0.8/whyis_activitystreams/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       52 2024-02-06 15:00:14.000000 whyis_activitystreams-0.0.8/whyis_activitystreams/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis_activitystreams-0.0.8/whyis_activitystreams/_version.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:57:08.821734 whyis_activitystreams-0.0.8/whyis_activitystreams/activity_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis_activitystreams-0.0.8/whyis_activitystreams/activity_agent/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1642 2024-04-19 07:27:51.000000 whyis_activitystreams-0.0.8/whyis_activitystreams/activity_agent/activity_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis_activitystreams-0.0.8/whyis_activitystreams/plugin.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 07:57:08.821734 whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 07:57:08.000000 whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1022 2024-04-19 07:57:08.000000 whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-04-19 07:57:08.000000 whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      150 2024-04-19 07:57:08.000000 whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/entry_points.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-04-19 07:57:08.000000 whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/requires.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       22 2024-04-19 07:57:08.000000 whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/top_level.txt
```

### Comparing `whyis_activitystreams-0.0.7/LICENSE` & `whyis_activitystreams-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/README.md` & `whyis_activitystreams-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/backbone_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/backbone_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/geometric_attribute_detection_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/geometric_attribute_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/object_classification_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/object_classification_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/object_detection_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/object_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/part_detection_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/part_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/photometric_attribute_detection_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/photometric_attribute_detection_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/saliency_map_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/saliency_map_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/perception_pipeline/pipeline_agent/uncertainty_attribution_agent.py` & `whyis_activitystreams-0.0.8/perception_pipeline/pipeline_agent/uncertainty_attribution_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/pyproject.toml` & `whyis_activitystreams-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='whyis-activitystreams'
-version='0.0.7'
+version='0.0.8'
 description = "A whyis plugin to support the interpretation of activity streams."
 dependencies=[
   'whyis',
 ]
 
 [tool.setuptools]
-packages=['whyis_activitystreams', 'whyis_activitystreams.activity_agent', 'perception_pipeline.pipeline_agent']
+packages=['whyis_activitystreams', 'whyis_activitystreams.activity_agent']#, 'perception_pipeline.pipeline_agent']
 
 [project.entry-points.whyis]
 whyis_activitystreams = "whyis_activitystreams:ActivityStreamsPlugin"
 whyis_activity_agent = "whyis_activitystreams.activity_agent:ActivityAgent"
-backbone_agent = "perception_pipeline.pipeline_agent:BackboneAgent"
-geometric_attribute_detection_agent = "perception_pipeline.pipeline_agent:GeometricAttributeDetectionAgent"
-object_classification_agent = "perception_pipeline.pipeline_agent:ObjectClassificationAgent"
-object_detection_agent = "perception_pipeline.pipeline_agent:ObjectDetectionAgent"
-part_detection_agent = "perception_pipeline.pipeline_agent:PartDetectionAgent"
-photometric_attribute_detection_agent = "perception_pipeline.pipeline_agent:PhotometricAttributeDetectionAgent"
-self_compare_saliency_map_agent = "perception_pipeline.pipeline_agent:SelfCompareSaliencyMapAgent"
-uncertainty_attribution_agent = "perception_pipeline.pipeline_agent:UncertaintyAttributionAgent"
+#backbone_agent = "perception_pipeline.pipeline_agent:BackboneAgent"
+#geometric_attribute_detection_agent = "perception_pipeline.pipeline_agent:GeometricAttributeDetectionAgent"
+#object_classification_agent = "perception_pipeline.pipeline_agent:ObjectClassificationAgent"
+#object_detection_agent = "perception_pipeline.pipeline_agent:ObjectDetectionAgent"
+#part_detection_agent = "perception_pipeline.pipeline_agent:PartDetectionAgent"
+#photometric_attribute_detection_agent = "perception_pipeline.pipeline_agent:PhotometricAttributeDetectionAgent"
+#self_compare_saliency_map_agent = "perception_pipeline.pipeline_agent:SelfCompareSaliencyMapAgent"
+#uncertainty_attribution_agent = "perception_pipeline.pipeline_agent:UncertaintyAttributionAgent"
```

### Comparing `whyis_activitystreams-0.0.7/whyis_activitystreams/activity_agent/activity_agent.py` & `whyis_activitystreams-0.0.8/whyis_activitystreams/activity_agent/activity_agent.py`

 * *Files identical despite different names*

### Comparing `whyis_activitystreams-0.0.7/whyis_activitystreams.egg-info/SOURCES.txt` & `whyis_activitystreams-0.0.8/whyis_activitystreams.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-perception_pipeline/pipeline_agent/__init__.py
 perception_pipeline/pipeline_agent/backbone_agent.py
 perception_pipeline/pipeline_agent/geometric_attribute_detection_agent.py
 perception_pipeline/pipeline_agent/object_classification_agent.py
 perception_pipeline/pipeline_agent/object_detection_agent.py
 perception_pipeline/pipeline_agent/part_detection_agent.py
 perception_pipeline/pipeline_agent/photometric_attribute_detection_agent.py
 perception_pipeline/pipeline_agent/saliency_map_agent.py
```

