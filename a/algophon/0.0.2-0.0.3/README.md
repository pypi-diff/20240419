# Comparing `tmp/algophon-0.0.2.tar.gz` & `tmp/algophon-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.2.tar", last modified: Thu Apr 18 16:47:35 2024, max compression
+gzip compressed data, was "algophon-0.0.3.tar", last modified: Thu Apr 18 19:13:23 2024, max compression
```

## Comparing `algophon-0.0.2.tar` & `algophon-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 16:47:35.692990 algophon-0.0.2/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.2/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)     1147 2024-04-18 16:47:35.692376 algophon-0.0.2/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      542 2024-04-18 15:22:58.000000 algophon-0.0.2/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 16:47:35.687142 algophon-0.0.2/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      129 2024-04-18 16:17:39.000000 algophon-0.0.2/algophon/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.2/algophon/ipa.txt
--rw-r--r--   0 u6052607   (503) staff       (20)     1167 2024-04-18 15:56:55.000000 algophon-0.0.2/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     3485 2024-04-18 16:31:03.000000 algophon-0.0.2/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)      202 2024-04-18 15:16:06.000000 algophon-0.0.2/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      203 2024-04-18 15:37:08.000000 algophon-0.0.2/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 16:47:35.691532 algophon-0.0.2/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)     1147 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      272 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      788 2024-04-18 16:46:20.000000 algophon-0.0.2/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-18 16:47:35.693068 algophon-0.0.2/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 19:13:23.949517 algophon-0.0.3/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.3/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)     7284 2024-04-18 19:13:23.948313 algophon-0.0.3/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     6679 2024-04-18 19:12:29.000000 algophon-0.0.3/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 19:13:23.937728 algophon-0.0.3/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.3/algophon/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.3/algophon/ipa.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)       87 2024-04-18 17:52:47.000000 algophon-0.0.3/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.3/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     3465 2024-04-18 19:01:16.000000 algophon-0.0.3/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5615 2024-04-18 17:35:20.000000 algophon-0.0.3/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.3/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 19:13:23.946220 algophon-0.0.3/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)     7284 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      293 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      788 2024-04-18 19:13:08.000000 algophon-0.0.3/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-18 19:13:23.949591 algophon-0.0.3/setup.cfg
```

### Comparing `algophon-0.0.2/LICENSE` & `algophon-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.2/algophon/ipa.txt` & `algophon-0.0.3/algophon/ipa.txt`

 * *Files identical despite different names*

### Comparing `algophon-0.0.2/algophon/seg.py` & `algophon-0.0.3/algophon/seg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 class Seg:
     '''
     A class representing a phonological segment.
 
     Allows for an ipa symbol to represent the segment as shorthand, but treats the segment as a feature bundle internally.
     '''
-    def __init__(self, ipa: str, features: dict):
+    def __init__(self, ipa: str, features: dict=dict()):
         self._ipa = ipa
-        self._features = features
+        self.features = features
 
     def __str__(self) -> str:
         return self._ipa
     
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `algophon-0.0.2/algophon/seginv.py` & `algophon-0.0.3/algophon/seginv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from algophon.symbols import UNKNOWN, UNDERSPECIFIED
 from algophon.seg import Seg
 
 import pkgutil
 
 class SegInv:
     '''
     A class representing an inventory of phonological segments (Seg objects).
@@ -72,32 +71,34 @@
             line = line.strip().split(self.sep)
             seg, feats = line[0], line[1:] # extract the IPA segment and its features
             if i == 0: # extract the header
                 self.feature_space = feats
             else: # add the segment to the dict
                 self._seg_to_feat_vec[seg] = feats
 
-    def add(self, ipa_seg: str) -> bool:
+    def add(self, ipa_seg: str) -> None:
         '''
         :ipa_seg: a IPA segment in str form
 
-        :return: True if the addition was successful
+        :return: None
         '''
         if ipa_seg in self:
-            return True
+            return
         if ipa_seg not in self._seg_to_feat_vec:
             raise KeyError(f'Segment {ipa_seg} is not in the IPA data from {self._ipa_source}.')
         feat_vec = self._seg_to_feat_vec[ipa_seg] # get the feature vector
         features = dict((feat, feat_vec[idx]) for idx, feat in enumerate(self.feature_space)) # convert the vector to dict form
         seg = Seg(ipa=ipa_seg, features=features)
         self.segs.add(seg)
         self._ipa_to_seg[ipa_seg] = seg
-        return True
 
-    def add_segments(self, ipa_segs: object) -> None:
+    def add_segs(self, ipa_segs: object) -> None:
         '''
         :ipa_segs: an iterable of IPA segments, each in str form
 
         :return: None
         '''
         for ipa in ipa_segs:
-            self.add(ipa)
+            self.add(ipa)
+
+    def add_segs_by_str(self, seg_str: str) -> None:
+        self.add_segs(seg_str.split())
```

### Comparing `algophon-0.0.2/pyproject.toml` & `algophon-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
```

