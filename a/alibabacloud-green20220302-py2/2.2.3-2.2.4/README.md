# Comparing `tmp/alibabacloud_green20220302_py2-2.2.3.tar.gz` & `tmp/alibabacloud_green20220302_py2-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302_py2-2.2.3.tar", last modified: Thu Apr 11 11:25:08 2024, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302_py2-2.2.4.tar", last modified: Fri Apr 19 17:10:44 2024, max compression
```

## Comparing `alibabacloud_green20220302_py2-2.2.3.tar` & `alibabacloud_green20220302_py2-2.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20988 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)   121028 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 11:25:08.000000 alibabacloud_green20220302_py2-2.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2024-04-11 11:25:07.000000 alibabacloud_green20220302_py2-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20988 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)   123403 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2024-04-19 17:10:44.000000 alibabacloud_green20220302_py2-2.2.4/setup.py
```

### Comparing `alibabacloud_green20220302_py2-2.2.3/ChangeLog.md` & `alibabacloud_green20220302_py2-2.2.4/ChangeLog.md`

 * *Files 4% similar despite different names*

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

### Comparing `alibabacloud_green20220302_py2-2.2.3/LICENSE` & `alibabacloud_green20220302_py2-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-2.2.3/PKG-INFO` & `alibabacloud_green20220302_py2-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302_py2
-Version: 2.2.3
+Version: 2.2.4
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-2.2.3/README-CN.md` & `alibabacloud_green20220302_py2-2.2.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-2.2.3/README.md` & `alibabacloud_green20220302_py2-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1508,14 +1508,75 @@
         if m.get('Service') is not None:
             self.service = m.get('Service')
         if m.get('ServiceParameters') is not None:
             self.service_parameters = m.get('ServiceParameters')
         return self
 
 
+class ImageModerationResponseBodyDataExtRecognition(TeaModel):
+    def __init__(self, classification=None, confidence=None):
+        self.classification = classification  # type: str
+        self.confidence = confidence  # type: float
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImageModerationResponseBodyDataExtRecognition, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Classification') is not None:
+            self.classification = m.get('Classification')
+        if m.get('Confidence') is not None:
+            self.confidence = m.get('Confidence')
+        return self
+
+
+class ImageModerationResponseBodyDataExt(TeaModel):
+    def __init__(self, recognition=None):
+        self.recognition = recognition  # type: list[ImageModerationResponseBodyDataExtRecognition]
+
+    def validate(self):
+        if self.recognition:
+            for k in self.recognition:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ImageModerationResponseBodyDataExt, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, confidence=None, label=None):
         self.confidence = confidence  # type: float
         self.label = label  # type: str
 
     def validate(self):
         pass
@@ -1538,42 +1599,50 @@
             self.confidence = m.get('Confidence')
         if m.get('Label') is not None:
             self.label = m.get('Label')
         return self
 
 
 class ImageModerationResponseBodyData(TeaModel):
-    def __init__(self, data_id=None, result=None):
+    def __init__(self, data_id=None, ext=None, result=None):
         self.data_id = data_id  # type: str
+        self.ext = ext  # type: ImageModerationResponseBodyDataExt
         self.result = result  # type: list[ImageModerationResponseBodyDataResult]
 
     def validate(self):
+        if self.ext:
+            self.ext.validate()
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super(ImageModerationResponseBodyData, self).to_map()
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
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_green20220302_py2-2.2.3/alibabacloud_green20220302_py2.egg-info/PKG-INFO` & `alibabacloud_green20220302_py2-2.2.4/alibabacloud_green20220302_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302-py2
-Version: 2.2.3
+Version: 2.2.4
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302_py2-2.2.3/setup.py` & `alibabacloud_green20220302_py2-2.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302_py2.
 
-Created on 11/04/2024
+Created on 19/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python2"
```

