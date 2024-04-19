# Comparing `tmp/algophon-0.0.4.tar.gz` & `tmp/algophon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.4.tar", last modified: Thu Apr 18 23:34:11 2024, max compression
+gzip compressed data, was "algophon-0.0.5.tar", last modified: Fri Apr 19 00:19:59 2024, max compression
```

## Comparing `algophon-0.0.4.tar` & `algophon-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 23:34:11.483918 algophon-0.0.4/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.4/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)     9613 2024-04-18 23:34:11.481992 algophon-0.0.4/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)     9008 2024-04-18 23:30:58.000000 algophon-0.0.4/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 23:34:11.472504 algophon-0.0.4/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.4/algophon/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.4/algophon/ipa.txt
--rw-r--r--   0 u6052607   (503) staff       (20)     1013 2024-04-18 23:29:48.000000 algophon-0.0.4/algophon/natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.4/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     4279 2024-04-18 23:29:32.000000 algophon-0.0.4/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5696 2024-04-18 22:25:18.000000 algophon-0.0.4/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.4/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 23:34:11.481128 algophon-0.0.4/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)     9613 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      293 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-18 23:34:04.000000 algophon-0.0.4/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-18 23:34:11.484149 algophon-0.0.4/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 00:19:59.617646 algophon-0.0.5/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.5/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 00:19:59.616984 algophon-0.0.5/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.5/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 00:19:59.606679 algophon-0.0.5/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.5/algophon/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.5/algophon/ipa.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.5/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.5/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     4412 2024-04-19 00:08:46.000000 algophon-0.0.5/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5685 2024-04-19 00:15:44.000000 algophon-0.0.5/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.5/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 00:19:59.616251 algophon-0.0.5/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 00:19:59.000000 algophon-0.0.5/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      392 2024-04-19 00:19:59.000000 algophon-0.0.5/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-19 00:19:59.000000 algophon-0.0.5/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-19 00:19:59.000000 algophon-0.0.5/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-19 00:19:50.000000 algophon-0.0.5/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-19 00:19:59.617703 algophon-0.0.5/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 00:19:59.615674 algophon-0.0.5/tests/
+-rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.5/tests/test_natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.5/tests/test_seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     2132 2024-04-19 00:05:44.000000 algophon-0.0.5/tests/test_seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1303 2024-04-19 00:15:27.000000 algophon-0.0.5/tests/test_segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      740 2024-04-18 23:42:58.000000 algophon-0.0.5/tests/tester.py
```

### Comparing `algophon-0.0.4/LICENSE` & `algophon-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.4/PKG-INFO` & `algophon-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -165,15 +165,15 @@
 The class `SegStr` allows for handling several tricky aspects of IPA sequences. It is common practice to represent strings of IPA sequences in a space-separated fashion such that, for example, [eːntjə] is represented `'eː n t j ə'`.
 
 Creating a `SegStr` object requires the following arguments:
   - `segs`: a collection of segments, which can be in any of the following formats:
     - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
     - list of IPA symbols
     - list of Seg objects
-  - `seg_inv`: a `SegInv` object
+  - `seginv`: a `SegInv` object
 
 ```python
 >>> seginv = SegInv() # init SegInv
 >>> seq = SegStr('eː n t j ə', seginv)
 >>> print(seq)
 eːntjə
 ```
@@ -226,15 +226,15 @@
 ```
 
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
 ```python
->>> son = NatClass(feats={'+son'}, seg_inv=seginv)
+>>> son = NatClass(feats={'+son'}, seginv=seginv)
 >>> son
 [+son]
 >>> 'ə' in son
 True
 >>> 'n' in son
 True
 >>> 't' in son
```

### Comparing `algophon-0.0.4/README.md` & `algophon-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 The class `SegStr` allows for handling several tricky aspects of IPA sequences. It is common practice to represent strings of IPA sequences in a space-separated fashion such that, for example, [eːntjə] is represented `'eː n t j ə'`.
 
 Creating a `SegStr` object requires the following arguments:
   - `segs`: a collection of segments, which can be in any of the following formats:
     - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
     - list of IPA symbols
     - list of Seg objects
-  - `seg_inv`: a `SegInv` object
+  - `seginv`: a `SegInv` object
 
 ```python
 >>> seginv = SegInv() # init SegInv
 >>> seq = SegStr('eː n t j ə', seginv)
 >>> print(seq)
 eːntjə
 ```
@@ -211,15 +211,15 @@
 ```
 
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
 ```python
->>> son = NatClass(feats={'+son'}, seg_inv=seginv)
+>>> son = NatClass(feats={'+son'}, seginv=seginv)
 >>> son
 [+son]
 >>> 'ə' in son
 True
 >>> 'n' in son
 True
 >>> 't' in son
```

### Comparing `algophon-0.0.4/algophon/ipa.txt` & `algophon-0.0.5/algophon/ipa.txt`

 * *Files identical despite different names*

### Comparing `algophon-0.0.4/algophon/natclass.py` & `algophon-0.0.5/algophon/natclass.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 class NatClass:
-    def __init__(self, feats, seg_inv):
+    def __init__(self, feats, seginv):
         self.feats = set(feats)
-        self._seg_inv = seg_inv
+        self._seginv = seginv
         self._name = '[' + ','.join(sorted(self.feats)) + ']'
 
     def __str__(self) -> str:
         return self._name
 
     def __repr__(self) -> str:
         return self.__str__()
     
     def __contains__(self, seg) -> bool:
         '''
         :seg: a str IPA segment or Seg object
 
         :return: True if the :seg: is in the NatClass, False otherwise
         '''
-        seg = self._seg_inv[seg]
+        seg = self._seginv[seg]
         return all(seg.features[feat[1:]] == feat[0] for feat in self.feats)
     
     def extension(self) -> set:
         '''
         :return: the extensional representation of the natural class
         '''
-        return self._seg_inv.extension(self)
+        return self._seginv.extension(self)
     
     def extension_complement(self) -> set:
         '''
-        :return: the extensional complement of the natural class relative to self._seg_inv: SegInv \ NatClass
+        :return: the extensional complement of the natural class relative to self._seginv: SegInv \ NatClass
         '''
-        return self._seg_inv.extension_complement(self)
+        return self._seginv.extension_complement(self)
```

### Comparing `algophon-0.0.4/algophon/seg.py` & `algophon-0.0.5/algophon/seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.4/algophon/seginv.py` & `algophon-0.0.5/algophon/seginv.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,20 +51,19 @@
         :seg: Can be any of the following:
             - str IPA symbol
             - Seg object
 
         :return: the Seg object corresponding to :seg: if present, otherwise KeyError is raised
         '''
         if seg not in self:
-            raise KeyError(f'{seg} of type {type(seg)} is not in the SegInv (try <seg_inv_obj>.add({seg}))')
+            raise KeyError(f'{seg} of type {type(seg)} is not in the SegInv (try <seginv_obj>.add({seg}))')
         return self._ipa_to_seg[seg]
 
     def _load_seg_to_feat_dict(self) -> None:
         self._seg_to_feat_vec = dict()
-        # with open(self.ipa_file_path, 'r') as f: # load IPA file
         data = pkgutil.get_data(__name__, "ipa.txt")
 
         if self.ipa_file_path is None:
             lines = data.decode('utf-8').strip().split('\n')
         else:
             with open(self.ipa_file_path, 'r') as f:
                 lines = f.readlines()
@@ -72,14 +71,18 @@
             line = line.strip().split(self.sep)
             seg, feats = line[0], line[1:] # extract the IPA segment and its features
             if i == 0: # extract the header
                 self.feature_space = feats
             else: # add the segment to the dict
                 self._seg_to_feat_vec[seg] = feats
 
+        if self.ipa_file_path is None:
+            # make ord('g') == 103 and ord('ɡ') == 609 the same, since panphon only as 609
+            self._seg_to_feat_vec['g'] = self._seg_to_feat_vec['ɡ']
+
     def add(self, ipa_seg: str) -> None:
         '''
         :ipa_seg: a IPA segment in str form
 
         :return: None
         '''
         if ipa_seg in self:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `algophon-0.0.4/algophon/segstr.py` & `algophon-0.0.5/algophon/segstr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 class SegStr:
     '''
     A class representing a sequence of phonological segments (Seg objects).
     '''
-    def __init__(self, segs, seg_inv):
+    def __init__(self, segs, seginv):
         '''
         :segs: Can be any of the following:
             - a str of IPA symbols, where each symbol is separated by a space ' '
             - a list of IPA symbols
             - a list of Seg objects
-        :seg_inv: a SegInv object
+        :seginv: a SegInv object
         '''
-        self._seg_inv = seg_inv
+        self._seginv = seginv
 
         if isinstance(segs, list):
-            self._segs = list(self._seg_inv.add_and_get(seg) for seg in segs)
+            self._segs = list(self._seginv.add_and_get(seg) for seg in segs)
         elif isinstance(segs, str):
-            self._segs = list(self._seg_inv.add_and_get(seg) for seg in segs.split())
+            self._segs = list(self._seginv.add_and_get(seg) for seg in segs.split())
         else:
             raise ValueError(f':segs: should be a list of IPA symbols, a list of Seg objects, or a str of space-separated IPA symbols, instead found type {type(segs)}')
         
         # compute str form
         self._str = ''
         for seg in self._segs:
             self._str += f'{seg}'
@@ -73,15 +73,15 @@
 
         :return: 
             - Slicing: SegStr object containing the slice
             - Indexing: Seg object at the index
         '''
         res = self._segs.__getitem__(idx)
         if isinstance(res, list): # handle a slice
-            return SegStr(segs=res, seg_inv=self._seg_inv)
+            return SegStr(segs=res, seginv=self._seginv)
         return res # handle an index
     
     def __add__(self, other: object):
         '''
         Handles concatenation.
 
         :other: Can be any of the following:
@@ -118,15 +118,15 @@
             - a SegStr object
         '''
         if isinstance(other, str):
             other = other.split()
         elif not isinstance(other, list) and not isinstance(other, SegStr):
             raise ValueError(f'Cannot compare a SegStr object with an object of type {type(other)}')
         for idx in range(len(other)):
-            if self.segments[idx] != other[idx]:
+            if self._segs[idx] != other[idx]:
                 return False
         return True
     
     def endswith(self, other: object) -> bool:
         '''
         :other: Can be any of the following:
             - a str of IPA symbols, where each symbol is separated by a space ' '
```

### Comparing `algophon-0.0.4/algophon.egg-info/PKG-INFO` & `algophon-0.0.5/algophon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -165,15 +165,15 @@
 The class `SegStr` allows for handling several tricky aspects of IPA sequences. It is common practice to represent strings of IPA sequences in a space-separated fashion such that, for example, [eːntjə] is represented `'eː n t j ə'`.
 
 Creating a `SegStr` object requires the following arguments:
   - `segs`: a collection of segments, which can be in any of the following formats:
     - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
     - list of IPA symbols
     - list of Seg objects
-  - `seg_inv`: a `SegInv` object
+  - `seginv`: a `SegInv` object
 
 ```python
 >>> seginv = SegInv() # init SegInv
 >>> seq = SegStr('eː n t j ə', seginv)
 >>> print(seq)
 eːntjə
 ```
@@ -226,15 +226,15 @@
 ```
 
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
 ```python
->>> son = NatClass(feats={'+son'}, seg_inv=seginv)
+>>> son = NatClass(feats={'+son'}, seginv=seginv)
 >>> son
 [+son]
 >>> 'ə' in son
 True
 >>> 'n' in son
 True
 >>> 't' in son
```

### Comparing `algophon-0.0.4/pyproject.toml` & `algophon-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
```

