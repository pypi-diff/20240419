# Comparing `tmp/alibabacloud_green20220302-2.2.3.tar.gz` & `tmp/alibabacloud_green20220302-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-2.2.3.tar", last modified: Thu Apr 11 11:25:55 2024, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-2.2.4.tar", last modified: Fri Apr 19 17:11:49 2024, max compression
```

## Comparing `alibabacloud_green20220302-2.2.3.tar` & `alibabacloud_green20220302-2.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/
--rw-r--r--   0 root         (0) root         (0)     1203 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1188 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50071 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)   119635 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2621 2024-04-11 11:25:55.000000 alibabacloud_green20220302-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50071 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)   121973 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/setup.py
```

### Comparing `alibabacloud_green20220302-2.2.3/ChangeLog.md` & `alibabacloud_green20220302-2.2.4/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-11 Version: 2.2.3
+- Update API DescribeImageResultExt: update response param.
+
+
 2024-03-26 Version: 2.2.2
 - Update API VideoModeration: update response param.
 - Update API VideoModerationResult: update response param.
 - Update API VoiceModeration: update response param.
 - Update API VoiceModerationResult: update response param.
```

### Comparing `alibabacloud_green20220302-2.2.3/LICENSE` & `alibabacloud_green20220302-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.3/PKG-INFO` & `alibabacloud_green20220302-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 2.2.3
+Version: 2.2.4
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.3/README-CN.md` & `alibabacloud_green20220302-2.2.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.3/README.md` & `alibabacloud_green20220302-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.3/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1713,14 +1713,82 @@
         if m.get('Service') is not None:
             self.service = m.get('Service')
         if m.get('ServiceParameters') is not None:
             self.service_parameters = m.get('ServiceParameters')
         return self
 
 
+class ImageModerationResponseBodyDataExtRecognition(TeaModel):
+    def __init__(
+        self,
+        classification: str = None,
+        confidence: float = None,
+    ):
+        self.classification = classification
+        self.confidence = confidence
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.classification is not None:
+            result['Classification'] = self.classification
+        if self.confidence is not None:
+            result['Confidence'] = self.confidence
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Classification') is not None:
+            self.classification = m.get('Classification')
+        if m.get('Confidence') is not None:
+            self.confidence = m.get('Confidence')
+        return self
+
+
+class ImageModerationResponseBodyDataExt(TeaModel):
+    def __init__(
+        self,
+        recognition: List[ImageModerationResponseBodyDataExtRecognition] = None,
+    ):
+        self.recognition = recognition
+
+    def validate(self):
+        if self.recognition:
+            for k in self.recognition:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Recognition'] = []
+        if self.recognition is not None:
+            for k in self.recognition:
+                result['Recognition'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.recognition = []
+        if m.get('Recognition') is not None:
+            for k in m.get('Recognition'):
+                temp_model = ImageModerationResponseBodyDataExtRecognition()
+                self.recognition.append(temp_model.from_map(k))
+        return self
+
+
 class ImageModerationResponseBodyDataResult(TeaModel):
     def __init__(
         self,
         confidence: float = None,
         label: str = None,
     ):
         self.confidence = confidence
@@ -1750,43 +1818,52 @@
         return self
 
 
 class ImageModerationResponseBodyData(TeaModel):
     def __init__(
         self,
         data_id: str = None,
+        ext: ImageModerationResponseBodyDataExt = None,
         result: List[ImageModerationResponseBodyDataResult] = None,
     ):
         self.data_id = data_id
+        self.ext = ext
         self.result = result
 
     def validate(self):
+        if self.ext:
+            self.ext.validate()
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.data_id is not None:
             result['DataId'] = self.data_id
+        if self.ext is not None:
+            result['Ext'] = self.ext.to_map()
         result['Result'] = []
         if self.result is not None:
             for k in self.result:
                 result['Result'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DataId') is not None:
             self.data_id = m.get('DataId')
+        if m.get('Ext') is not None:
+            temp_model = ImageModerationResponseBodyDataExt()
+            self.ext = temp_model.from_map(m['Ext'])
         self.result = []
         if m.get('Result') is not None:
             for k in m.get('Result'):
                 temp_model = ImageModerationResponseBodyDataResult()
                 self.result.append(temp_model.from_map(k))
         return self
```

### Comparing `alibabacloud_green20220302-2.2.3/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 2.2.3
+Version: 2.2.4
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.3/setup.py` & `alibabacloud_green20220302-2.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 11/04/2024
+Created on 19/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
```

