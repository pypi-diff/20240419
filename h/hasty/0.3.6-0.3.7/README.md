# Comparing `tmp/hasty-0.3.6.tar.gz` & `tmp/hasty-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasty-0.3.6.tar", last modified: Mon Sep 19 18:57:13 2022, max compression
+gzip compressed data, was "hasty-0.3.7.tar", last modified: Fri Apr 19 11:56:58 2024, max compression
```

## Comparing `hasty-0.3.6.tar` & `hasty-0.3.7.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:57:13.103838 hasty-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-09-19 18:57:01.000000 hasty-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-09-19 18:57:13.103838 hasty-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-09-19 18:57:01.000000 hasty-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:57:13.099837 hasty-0.3.6/hasty/
--rwxr-xr-x   0 runner    (1001) docker     (121)      919 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5794 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/automated_labeling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/export_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/hasty_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    11464 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:57:13.103838 hasty-0.3.6/hasty/inference/
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/inference/attributer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/inference/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/inference/detector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/inference/instance_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/inference/semantic_segmentor.py
--rw-r--r--   0 runner    (1001) docker     (121)    10290 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/label_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     3862 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/label_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/label_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19125 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/requester.py
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/tag_class.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-09-19 18:57:01.000000 hasty-0.3.6/hasty/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 18:57:13.103838 hasty-0.3.6/hasty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-09-19 18:57:13.000000 hasty-0.3.6/hasty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-09-19 18:57:13.000000 hasty-0.3.6/hasty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 18:57:13.000000 hasty-0.3.6/hasty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-19 18:57:13.000000 hasty-0.3.6/hasty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-19 18:57:13.000000 hasty-0.3.6/hasty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-19 18:57:13.103838 hasty-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-09-19 18:57:01.000000 hasty-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:56:58.232264 hasty-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 11:56:48.000000 hasty-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-19 11:56:58.232264 hasty-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-19 11:56:48.000000 hasty-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:56:58.228264 hasty-0.3.7/hasty/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/automated_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/export_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/hasty_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:56:58.228264 hasty-0.3.7/hasty/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/inference/attributer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/inference/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/inference/instance_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/inference/semantic_segmentor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/label_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/label_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/label_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19125 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/tag_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-19 11:56:48.000000 hasty-0.3.7/hasty/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:56:58.232264 hasty-0.3.7/hasty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-19 11:56:58.000000 hasty-0.3.7/hasty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-19 11:56:58.000000 hasty-0.3.7/hasty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:56:58.000000 hasty-0.3.7/hasty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 11:56:58.000000 hasty-0.3.7/hasty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 11:56:58.000000 hasty-0.3.7/hasty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 11:56:58.232264 hasty-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-19 11:56:48.000000 hasty-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:56:58.228264 hasty-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-19 11:56:48.000000 hasty-0.3.7/tests/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-19 11:56:48.000000 hasty-0.3.7/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-19 11:56:48.000000 hasty-0.3.7/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-19 11:56:48.000000 hasty-0.3.7/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-19 11:56:48.000000 hasty-0.3.7/tests/test_label_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-19 11:56:48.000000 hasty-0.3.7/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-19 11:56:48.000000 hasty-0.3.7/tests/test_tag.py
```

### Comparing `hasty-0.3.6/LICENSE` & `hasty-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/PKG-INFO` & `hasty-0.3.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasty
-Version: 0.3.6
+Version: 0.3.7
 Summary: Hasty API client library
 Home-page: https://github.com/hasty-ai/hasty-python/
 Author: Hasty GmbH
 Author-email: herbert@hasty.ai
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.16
+Requires-Dist: requests>=2.23.0
+Requires-Dist: retrying==1.3.3
 
 # Python library for the Hasty API.
 [![PyPI version](https://badge.fury.io/py/hasty.svg)](https://badge.fury.io/py/hasty)
 [![Documentation Status](https://readthedocs.org/projects/hasty/badge/?version=latest)](https://hasty.readthedocs.io/en/latest/?badge=latest)
 ![CI](https://github.com/hasty-ai/hasty-python/workflows/CI/badge.svg)
```

### Comparing `hasty-0.3.6/README.md` & `hasty-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/__init__.py` & `hasty-0.3.7/hasty/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def int_or_str(value):
     try:
         return int(value)
     except ValueError:
         return value
 
 
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 VERSION = tuple(map(int_or_str, __version__.split('.')))
 
 __all__ = [
     'Attribute',
     'Attributer',
     'Client',
     'Dataset',
```

### Comparing `hasty-0.3.6/hasty/attribute.py` & `hasty-0.3.7/hasty/attribute.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/automated_labeling.py` & `hasty-0.3.7/hasty/automated_labeling.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/client.py` & `hasty-0.3.7/hasty/client.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/constants.py` & `hasty-0.3.7/hasty/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 class ImageStatus:
     New = "NEW"
     Done = "DONE"
     Skipped = "SKIPPED"
     InProgress = "IN PROGRESS"
     ToReview = "TO REVIEW"
+    Completed = "COMPLETED"
     AutoLabelled = "AUTO-LABELLED"
 
 
 class ExportFormat:
     JSON_v11 = "json_v1.1"
     SEMANTIC_PNG = "semantic_png"
     JSON_COCO = "json_coco"
@@ -25,11 +26,11 @@
     CLASS_TYPE = "class_type"
     CLASS_ORDER = "class_order"
 
 
 WAIT_INTERVAL_SEC = 10
 
 VALID_STATUSES = [ImageStatus.New, ImageStatus.Done, ImageStatus.Skipped, ImageStatus.InProgress, ImageStatus.ToReview,
-                  ImageStatus.AutoLabelled]
+                  ImageStatus.AutoLabelled, ImageStatus.Completed]
 VALID_EXPORT_FORMATS = [ExportFormat.JSON_v11, ExportFormat.SEMANTIC_PNG, ExportFormat.JSON_COCO, ExportFormat.IMAGES]
 VALID_SEMANTIC_FORMATS = [SemanticFormat.GS_DESC, SemanticFormat.GS_ASC, SemanticFormat.CLASS_COLOR]
 VALID_SEMANTIC_ORDER = [SemanticOrder.Z_INDEX, SemanticOrder.CLASS_TYPE, SemanticOrder.CLASS_ORDER]
```

### Comparing `hasty-0.3.6/hasty/dataset.py` & `hasty-0.3.7/hasty/dataset.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/exception.py` & `hasty-0.3.7/hasty/exception.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/export_job.py` & `hasty-0.3.7/hasty/export_job.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/hasty_object.py` & `hasty-0.3.7/hasty/hasty_object.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/helper.py` & `hasty-0.3.7/hasty/helper.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/image.py` & `hasty-0.3.7/hasty/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .label_class import LabelClass
 from .tag import Tag
 from .tag_class import TagClass
 
 
 class Image(HastyObject):
     endpoint = '/v1/projects/{project_id}/images'
-    endpoint_uploads = '/v1/projects/{project_id}/image_uploads'
+    endpoint_uploads = '/v1/projects/{project_id}/uploads'
     endpoint_image = '/v1/projects/{project_id}/images/{image_id}'
 
     def __repr__(self):
         return self.get__repr__(OrderedDict({"id": self._id, "dataset_name": self._dataset_name, "name": self._name,
                                              "width": self._width, "height": self._height}))
 
     @property
@@ -129,23 +129,23 @@
     @staticmethod
     def _get_by_id(requester, project_id, image_id):
         data = requester.get(Image.endpoint_image.format(project_id=project_id, image_id=image_id))
         return Image(requester, data, {"project_id": project_id})
 
     @staticmethod
     def _generate_sign_url(requester, project_id):
-        data = requester.post(Image.endpoint_uploads.format(project_id=project_id), json_data={"count": 1})
+        data = requester.get(Image.endpoint_uploads.format(project_id=project_id), query_params={"count": 1})
         return data["items"][0]
 
     @staticmethod
     def _upload_from_file(requester, project_id, dataset_id, filepath, external_id: Optional[str] = None):
         filename = os.path.basename(filepath)
         url_data = Image._generate_sign_url(requester, project_id)
         with open(filepath, 'rb') as f:
-            requester.put(url_data['url'], data=f.read(), content_type="image/*")
+            requester.put(url_data['url'], data=f.read(), content_type="")
         res = requester.post(Image.endpoint.format(project_id=project_id),
                              json_data={"dataset_id": dataset_id,
                                         "filename": filename,
                                         "upload_id": url_data["id"],
                                         "external_id": external_id})
         return Image(requester, res, {"project_id": project_id,
                                       "dataset_id": dataset_id})
@@ -167,15 +167,15 @@
         Returns image labels (list of `~hasty.Label` objects)
         """
         return PaginatedList(Label, self._requester,
                              Label.endpoint_image.format(project_id=self.project_id, image_id=self.id),
                              obj_params={"project_id": self.project_id})
 
     def create_label(self, label_class: Union[LabelClass, str], bbox: List[int] = None, polygon: List[List[int]] = None,
-                     mask: List[int] = None, z_index: int = None, external_id: Optional[str] = None):
+                     mask: List[int] = None, z_index: int = 0, external_id: Optional[str] = None):
         """
         Create label
 
         Args:
             label_class (LabelClass, str): Label class or label class ID of the label
             bbox (list of int): Coordinates of bounding box [x_min, y_min, x_max, y_max]
             polygon (list): List of x, y pairs [[x0, y0], [x1, y1], .... [x0, y0]]
```

### Comparing `hasty-0.3.6/hasty/inference/attributer.py` & `hasty-0.3.7/hasty/inference/attributer.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/inference/base.py` & `hasty-0.3.7/hasty/inference/base.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/inference/detector.py` & `hasty-0.3.7/hasty/inference/detector.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/inference/instance_segmentor.py` & `hasty-0.3.7/hasty/inference/instance_segmentor.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/inference/semantic_segmentor.py` & `hasty-0.3.7/hasty/inference/semantic_segmentor.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/label.py` & `hasty-0.3.7/hasty/label.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .exception import LimitExceededException, ValidationException
 from .label_attribute import LabelAttribute
 from .label_class import LabelClass
 from .label_utils import check_bbox_format, check_rle_mask
 
 
 C_LABELS_LIMIT = 100
+C_LABELS_TOOL_USED = "api"
 
 
 class Label(HastyObject):
     endpoint_image = '/v1/projects/{project_id}/images/{image_id}/labels'
     endpoint_project = '/v1/projects/{project_id}/labels'
 
     def __repr__(self):
@@ -179,15 +180,16 @@
             Label._validate_label(label["class_id"], label.get("bbox"), label.get("polygon"),
                                   label.get("mask"), label.get("z_index"))
             data.append({"class_id": label["class_id"],
                          "bbox": label.get("bbox"),
                          "polygon": label.get("polygon"),
                          "mask": label.get("mask"),
                          "z_index": label.get("z_index"),
-                         "external_id": label.get("external_id")})
+                         "external_id": label.get("external_id"),
+                         "tool_used": C_LABELS_TOOL_USED})
         res = requester.post(Label.endpoint_image.format(project_id=project_id, image_id=image_id), json_data=data)
         new_labels = []
         for label in res["items"]:
             new_labels.append(Label(requester, label, {"project_id": project_id, "image_id": image_id}))
         return new_labels
 
     @staticmethod
@@ -200,15 +202,16 @@
                                   label.get("mask"), label.get("z_index"))
             data.append({"label_id": label["label_id"],
                          "class_id": label["class_id"],
                          "bbox": label.get("bbox"),
                          "polygon": label.get("polygon"),
                          "mask": label.get("mask"),
                          "z_index": label.get("z_index"),
-                         "external_id": label.get("external_id")})
+                         "external_id": label.get("external_id"),
+                         "tool_used": C_LABELS_TOOL_USED})
         res = requester.put(Label.endpoint_image.format(project_id=project_id, image_id=image_id), json_data=data)
         updated_labels = []
         for label in res["items"]:
             updated_labels.append(Label(requester, label, {"project_id": project_id, "image_id": image_id}))
         return updated_labels
 
     @staticmethod
@@ -236,15 +239,16 @@
         updated_labels = Label._batch_update(self._requester, self.project_id, self.image_id,
                                              [{"label_id": self.id,
                                                "class_id": class_id,
                                                "bbox": bbox,
                                                "polygon": polygon,
                                                "mask": mask,
                                                "z_index": z_index,
-                                               "external_id": external_id}])
+                                               "external_id": external_id,
+                                               "tool_used": C_LABELS_TOOL_USED}])
         updated_label = updated_labels[0]
         self._class_id = updated_label.class_id
         self._bbox = updated_label.bbox
         self._polygon = updated_label.polygon
         self._mask = updated_label.mask
         self._z_index = updated_label.z_index
         self._external_id = updated_label.external_id
```

### Comparing `hasty-0.3.6/hasty/label_attribute.py` & `hasty-0.3.7/hasty/label_attribute.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/label_class.py` & `hasty-0.3.7/hasty/label_class.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/label_utils.py` & `hasty-0.3.7/hasty/label_utils.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/project.py` & `hasty-0.3.7/hasty/project.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/requester.py` & `hasty-0.3.7/hasty/requester.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/tag.py` & `hasty-0.3.7/hasty/tag.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/tag_class.py` & `hasty-0.3.7/hasty/tag_class.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty/workspace.py` & `hasty-0.3.7/hasty/workspace.py`

 * *Files identical despite different names*

### Comparing `hasty-0.3.6/hasty.egg-info/PKG-INFO` & `hasty-0.3.7/hasty.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hasty
-Version: 0.3.6
+Version: 0.3.7
 Summary: Hasty API client library
 Home-page: https://github.com/hasty-ai/hasty-python/
 Author: Hasty GmbH
 Author-email: herbert@hasty.ai
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.16
+Requires-Dist: requests>=2.23.0
+Requires-Dist: retrying==1.3.3
 
 # Python library for the Hasty API.
 [![PyPI version](https://badge.fury.io/py/hasty.svg)](https://badge.fury.io/py/hasty)
 [![Documentation Status](https://readthedocs.org/projects/hasty/badge/?version=latest)](https://hasty.readthedocs.io/en/latest/?badge=latest)
 ![CI](https://github.com/hasty-ai/hasty-python/workflows/CI/badge.svg)
```

### Comparing `hasty-0.3.6/hasty.egg-info/SOURCES.txt` & `hasty-0.3.7/hasty.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -28,8 +28,15 @@
 hasty.egg-info/requires.txt
 hasty.egg-info/top_level.txt
 hasty/inference/__init__.py
 hasty/inference/attributer.py
 hasty/inference/base.py
 hasty/inference/detector.py
 hasty/inference/instance_segmentor.py
-hasty/inference/semantic_segmentor.py
+hasty/inference/semantic_segmentor.py
+tests/test_attribute.py
+tests/test_dataset.py
+tests/test_image.py
+tests/test_label.py
+tests/test_label_class.py
+tests/test_project.py
+tests/test_tag.py
```

### Comparing `hasty-0.3.6/setup.py` & `hasty-0.3.7/setup.py`

 * *Files identical despite different names*

