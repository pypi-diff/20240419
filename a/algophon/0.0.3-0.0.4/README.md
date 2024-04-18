# Comparing `tmp/algophon-0.0.3.tar.gz` & `tmp/algophon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.3.tar", last modified: Thu Apr 18 19:13:23 2024, max compression
+gzip compressed data, was "algophon-0.0.4.tar", last modified: Thu Apr 18 23:34:11 2024, max compression
```

## Comparing `algophon-0.0.3.tar` & `algophon-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 19:13:23.949517 algophon-0.0.3/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.3/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)     7284 2024-04-18 19:13:23.948313 algophon-0.0.3/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)     6679 2024-04-18 19:12:29.000000 algophon-0.0.3/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 19:13:23.937728 algophon-0.0.3/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.3/algophon/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.3/algophon/ipa.txt
--rw-r--r--   0 u6052607   (503) staff       (20)       87 2024-04-18 17:52:47.000000 algophon-0.0.3/algophon/natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.3/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     3465 2024-04-18 19:01:16.000000 algophon-0.0.3/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5615 2024-04-18 17:35:20.000000 algophon-0.0.3/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.3/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 19:13:23.946220 algophon-0.0.3/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)     7284 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      293 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-18 19:13:23.000000 algophon-0.0.3/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      788 2024-04-18 19:13:08.000000 algophon-0.0.3/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-18 19:13:23.949591 algophon-0.0.3/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 23:34:11.483918 algophon-0.0.4/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.4/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)     9613 2024-04-18 23:34:11.481992 algophon-0.0.4/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     9008 2024-04-18 23:30:58.000000 algophon-0.0.4/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 23:34:11.472504 algophon-0.0.4/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.4/algophon/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.4/algophon/ipa.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)     1013 2024-04-18 23:29:48.000000 algophon-0.0.4/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.4/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     4279 2024-04-18 23:29:32.000000 algophon-0.0.4/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5696 2024-04-18 22:25:18.000000 algophon-0.0.4/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.4/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 23:34:11.481128 algophon-0.0.4/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)     9613 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      293 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-18 23:34:11.000000 algophon-0.0.4/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-18 23:34:04.000000 algophon-0.0.4/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-18 23:34:11.484149 algophon-0.0.4/setup.cfg
```

### Comparing `algophon-0.0.3/LICENSE` & `algophon-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.3/PKG-INFO` & `algophon-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: algophon
-Version: 0.0.3
-Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
-Author: Caleb Belth
-License: Apache 2.0
-Project-URL: Homepage, https://github.com/cbelth/algophon
-Keywords: computational linguistics,phonology,morphology,natural language processing
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # algophon
 
 **Code for working on computational phonology and morphology in Python.** 
 
 The project is based on code developed by [Caleb Belth](https://cbelth.github.io/) during the course of his PhD; the title of his [dissertation](https://cbelth.github.io/public/assets/documents/belth_dissertation.pdf), *Towards an Algorithmic Account of Phonological Rules and Representations*, serves as the origin for the repository's name *algophon*.
 
 This is a <span style="color:orange">work in progress</span>. The pypi distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
@@ -158,18 +143,111 @@
 True
 ```
 
 ### Strings of Segments: `SegStr`
 
 **A class to represent a sequence of phonological segments (Seg objects).**
 
+The class `SegStr` allows for handling several tricky aspects of IPA sequences. It is common practice to represent strings of IPA sequences in a space-separated fashion such that, for example, [eːntjə] is represented `'eː n t j ə'`.
+
+Creating a `SegStr` object requires the following arguments:
+  - `segs`: a collection of segments, which can be in any of the following formats:
+    - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
+    - list of IPA symbols
+    - list of Seg objects
+  - `seg_inv`: a `SegInv` object
+
+```python
+>>> seginv = SegInv() # init SegInv
+>>> seq = SegStr('eː n t j ə', seginv)
+>>> print(seq)
+eːntjə
+```
+
+Creating the `SegStr` object automatically adds the segments in the object to the `SegInv` object.
+
+```python
+>>> print(seginv.segs)
+{ə, t, n, j, eː}
+```
+
+For clean visuzliation, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
+
+```python
+>>> print(len(seq))
+5
+>>> seq[0]
+eː
+>>> type(seq[0]) # indexing returns a Seg object
+<class 'algophon.seg.Seg'>
+>>> seq[-2:]
+jə
+>>> type(seq[-2:]) # slicing returns a new SegStr object
+<class 'algophon.segstr.SegStr'>
+>>> seq[-2:] == 'j ə' # comparison to str objects works as expected
+True
+>>> seq[-2:] == 'ə n'
+False
+```
+
+`SegStr` also implements equivalents of useful str methods.
+
+```python
+>>> seq.endswith('j ə')
+True
+>>> dim_sufx = seq[-2:]
+>>> seq.endswith(dim_sufx)
+True
+>>> seq.startswith(seq[:-2])
+True
+```
+
+A `SegStr` object hashes to the value of its (space-separated) string:
+
+```python
+>>> len({seq, 'eː n t j ə'})
+1
+>>> seq in {'eː n t j ə'}
+True
+```
+
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
+```python
+>>> son = NatClass(feats={'+son'}, seg_inv=seginv)
+>>> son
+[+son]
+>>> 'ə' in son
+True
+>>> 'n' in son
+True
+>>> 't' in son
+False
+```
+
+The class also allows you to get the natural class's extension and the extension's complement, relative to the `SegInv` (in our example, only `{ə, t, n, j, eː}` are in `seginv`):
+
+```python
+>>> son.extension()
+{eː, j, ə, n}
+>>> son.extension_complement()
+{t}
+```
+
+You can also retrieve an extension (complement) directly from a `SegInv` object without creating a `NatClass` obj:
+
+```python
+>>> seginv.extension({'+syl'})
+{ə, eː}
+>>> seginv.extension_complement({'+syl'})
+{j, t, n}
+```
+
 ### Symbols: The `symbols` module
 
 The `symbols` module (techincally just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
@@ -208,8 +286,8 @@
   year={2023},
   school={{University of Michigan}}
 }
 ```
 
 ## References
 
-- Mortensen, D. R., Littell, P., Bharadwaj, A., Goyal, K., Dyer, C., & Levin, L. (2016, December). Panphon: A resource for mapping IPA segments to articulatory feature vectors. In Proceedings of COLING 2016, the 26th International Conference on Computational Linguistics: Technical Papers (pp. 3475-3484).
+- Mortensen, D. R., Littell, P., Bharadwaj, A., Goyal, K., Dyer, C., & Levin, L. (2016, December). Panphon: A resource for mapping IPA segments to articulatory feature vectors. In Proceedings of COLING 2016, the 26th International Conference on Computational Linguistics: Technical Papers (pp. 3475-3484).
```

### Comparing `algophon-0.0.3/README.md` & `algophon-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: algophon
+Version: 0.0.4
+Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
+Author: Caleb Belth
+License: Apache 2.0
+Project-URL: Homepage, https://github.com/cbelth/algophon
+Keywords: computational linguistics,phonology,morphology,natural language processing
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # algophon
 
 **Code for working on computational phonology and morphology in Python.** 
 
 The project is based on code developed by [Caleb Belth](https://cbelth.github.io/) during the course of his PhD; the title of his [dissertation](https://cbelth.github.io/public/assets/documents/belth_dissertation.pdf), *Towards an Algorithmic Account of Phonological Rules and Representations*, serves as the origin for the repository's name *algophon*.
 
 This is a <span style="color:orange">work in progress</span>. The pypi distribution and documentation will be updated as the project progresses! The initial plan for the project is to include:
@@ -143,18 +158,111 @@
 True
 ```
 
 ### Strings of Segments: `SegStr`
 
 **A class to represent a sequence of phonological segments (Seg objects).**
 
+The class `SegStr` allows for handling several tricky aspects of IPA sequences. It is common practice to represent strings of IPA sequences in a space-separated fashion such that, for example, [eːntjə] is represented `'eː n t j ə'`.
+
+Creating a `SegStr` object requires the following arguments:
+  - `segs`: a collection of segments, which can be in any of the following formats:
+    - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
+    - list of IPA symbols
+    - list of Seg objects
+  - `seg_inv`: a `SegInv` object
+
+```python
+>>> seginv = SegInv() # init SegInv
+>>> seq = SegStr('eː n t j ə', seginv)
+>>> print(seq)
+eːntjə
+```
+
+Creating the `SegStr` object automatically adds the segments in the object to the `SegInv` object.
+
+```python
+>>> print(seginv.segs)
+{ə, t, n, j, eː}
+```
+
+For clean visuzliation, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
+
+```python
+>>> print(len(seq))
+5
+>>> seq[0]
+eː
+>>> type(seq[0]) # indexing returns a Seg object
+<class 'algophon.seg.Seg'>
+>>> seq[-2:]
+jə
+>>> type(seq[-2:]) # slicing returns a new SegStr object
+<class 'algophon.segstr.SegStr'>
+>>> seq[-2:] == 'j ə' # comparison to str objects works as expected
+True
+>>> seq[-2:] == 'ə n'
+False
+```
+
+`SegStr` also implements equivalents of useful str methods.
+
+```python
+>>> seq.endswith('j ə')
+True
+>>> dim_sufx = seq[-2:]
+>>> seq.endswith(dim_sufx)
+True
+>>> seq.startswith(seq[:-2])
+True
+```
+
+A `SegStr` object hashes to the value of its (space-separated) string:
+
+```python
+>>> len({seq, 'eː n t j ə'})
+1
+>>> seq in {'eː n t j ə'}
+True
+```
+
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
+```python
+>>> son = NatClass(feats={'+son'}, seg_inv=seginv)
+>>> son
+[+son]
+>>> 'ə' in son
+True
+>>> 'n' in son
+True
+>>> 't' in son
+False
+```
+
+The class also allows you to get the natural class's extension and the extension's complement, relative to the `SegInv` (in our example, only `{ə, t, n, j, eː}` are in `seginv`):
+
+```python
+>>> son.extension()
+{eː, j, ə, n}
+>>> son.extension_complement()
+{t}
+```
+
+You can also retrieve an extension (complement) directly from a `SegInv` object without creating a `NatClass` obj:
+
+```python
+>>> seginv.extension({'+syl'})
+{ə, eː}
+>>> seginv.extension_complement({'+syl'})
+{j, t, n}
+```
+
 ### Symbols: The `symbols` module
 
 The `symbols` module (techincally just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
@@ -193,8 +301,8 @@
   year={2023},
   school={{University of Michigan}}
 }
 ```
 
 ## References
 
-- Mortensen, D. R., Littell, P., Bharadwaj, A., Goyal, K., Dyer, C., & Levin, L. (2016, December). Panphon: A resource for mapping IPA segments to articulatory feature vectors. In Proceedings of COLING 2016, the 26th International Conference on Computational Linguistics: Technical Papers (pp. 3475-3484).
+- Mortensen, D. R., Littell, P., Bharadwaj, A., Goyal, K., Dyer, C., & Levin, L. (2016, December). Panphon: A resource for mapping IPA segments to articulatory feature vectors. In Proceedings of COLING 2016, the 26th International Conference on Computational Linguistics: Technical Papers (pp. 3475-3484).
```

### Comparing `algophon-0.0.3/algophon/ipa.txt` & `algophon-0.0.4/algophon/ipa.txt`

 * *Files identical despite different names*

### Comparing `algophon-0.0.3/algophon/seg.py` & `algophon-0.0.4/algophon/seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.3/algophon/seginv.py` & `algophon-0.0.4/algophon/seginv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from algophon.seg import Seg
+from algophon.natclass import NatClass
 
 import pkgutil
 
 class SegInv:
     '''
     A class representing an inventory of phonological segments (Seg objects).
     '''
@@ -50,15 +51,15 @@
         :seg: Can be any of the following:
             - str IPA symbol
             - Seg object
 
         :return: the Seg object corresponding to :seg: if present, otherwise KeyError is raised
         '''
         if seg not in self:
-            raise KeyError(f'{seg} of type {type(seg)} is not in the SegInv')
+            raise KeyError(f'{seg} of type {type(seg)} is not in the SegInv (try <seg_inv_obj>.add({seg}))')
         return self._ipa_to_seg[seg]
 
     def _load_seg_to_feat_dict(self) -> None:
         self._seg_to_feat_vec = dict()
         # with open(self.ipa_file_path, 'r') as f: # load IPA file
         data = pkgutil.get_data(__name__, "ipa.txt")
 
@@ -97,8 +98,30 @@
 
         :return: None
         '''
         for ipa in ipa_segs:
             self.add(ipa)
 
     def add_segs_by_str(self, seg_str: str) -> None:
-        self.add_segs(seg_str.split())
+        self.add_segs(seg_str.split())
+
+    def add_and_get(self, seg: object) -> Seg:
+        self.add(f'{seg}')
+        return self[seg]
+    
+    def extension(self, nat_class) -> set:
+        '''
+        :nat_class: a set of features or a NatClass object
+
+        :return: the extension of the :nat_class:
+        '''
+        if type(nat_class) is set:
+            nat_class = NatClass(nat_class, self)
+        return set(seg for seg in self.segs if seg in nat_class)
+    
+    def extension_complement(self, nat_class) -> set:
+        '''
+        :nat_class: a set of features or a NatClass object
+
+        :return: the extensional complement of :nat_class: relative to :self: SegInv \ NatClass
+        '''
+        return self.segs.difference(self.extension(nat_class=nat_class))
```

### Comparing `algophon-0.0.3/algophon/segstr.py` & `algophon-0.0.4/algophon/segstr.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,30 @@
             - a list of IPA symbols
             - a list of Seg objects
         :seg_inv: a SegInv object
         '''
         self._seg_inv = seg_inv
 
         if isinstance(segs, list):
-            self._segs = list(self._seg_inv[seg] for seg in segs)
+            self._segs = list(self._seg_inv.add_and_get(seg) for seg in segs)
         elif isinstance(segs, str):
-            self._segs = list(self._seg_inv[seg] for seg in segs.split())
+            self._segs = list(self._seg_inv.add_and_get(seg) for seg in segs.split())
         else:
             raise ValueError(f':segs: should be a list of IPA symbols, a list of Seg objects, or a str of space-separated IPA symbols, instead found type {type(segs)}')
         
+        # compute str form
+        self._str = ''
+        for seg in self._segs:
+            self._str += f'{seg}'
+        
     def __len__(self) -> int:
         return len(self._segs)
     
     def __str__(self) -> str:
-        s = ''
-        for seg in self._segs:
-            s += f'{seg}'
-        return s
+        return self._str
     
     def __repr__(self) -> str:
         return self.__str__()
     
     def __hash__(self) -> int:
         '''
         Uses hash of space-separated IPA symbols
@@ -134,15 +136,15 @@
         '''
         if isinstance(other, str):
             other = other.split()
         elif not isinstance(other, list) and not isinstance(other, SegStr):
             raise ValueError(f'Cannot compare a SegStr object with an object of type {type(other)}')
         idx = -1
         for offset in range(len(other)):
-            if self.segments[idx - offset] != other[idx - offset]:
+            if self._segs[idx - offset] != other[idx - offset]:
                 return False
         return True
 
     def count(self, item: object) -> int:
         '''
         :item: Can be either of the following:
             - str IPA symbol
```

### Comparing `algophon-0.0.3/algophon.egg-info/PKG-INFO` & `algophon-0.0.4/algophon.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -158,18 +158,111 @@
 True
 ```
 
 ### Strings of Segments: `SegStr`
 
 **A class to represent a sequence of phonological segments (Seg objects).**
 
+The class `SegStr` allows for handling several tricky aspects of IPA sequences. It is common practice to represent strings of IPA sequences in a space-separated fashion such that, for example, [eːntjə] is represented `'eː n t j ə'`.
+
+Creating a `SegStr` object requires the following arguments:
+  - `segs`: a collection of segments, which can be in any of the following formats:
+    - str of IPA symbols, where each symbol is separated by a space ' ' (**most common**)
+    - list of IPA symbols
+    - list of Seg objects
+  - `seg_inv`: a `SegInv` object
+
+```python
+>>> seginv = SegInv() # init SegInv
+>>> seq = SegStr('eː n t j ə', seginv)
+>>> print(seq)
+eːntjə
+```
+
+Creating the `SegStr` object automatically adds the segments in the object to the `SegInv` object.
+
+```python
+>>> print(seginv.segs)
+{ə, t, n, j, eː}
+```
+
+For clean visuzliation, `SegStr` displays the sequence of segments without spaces, as `print(seq)` shows above. But internally a `SegStr` object knows what the segments are:
+
+```python
+>>> print(len(seq))
+5
+>>> seq[0]
+eː
+>>> type(seq[0]) # indexing returns a Seg object
+<class 'algophon.seg.Seg'>
+>>> seq[-2:]
+jə
+>>> type(seq[-2:]) # slicing returns a new SegStr object
+<class 'algophon.segstr.SegStr'>
+>>> seq[-2:] == 'j ə' # comparison to str objects works as expected
+True
+>>> seq[-2:] == 'ə n'
+False
+```
+
+`SegStr` also implements equivalents of useful str methods.
+
+```python
+>>> seq.endswith('j ə')
+True
+>>> dim_sufx = seq[-2:]
+>>> seq.endswith(dim_sufx)
+True
+>>> seq.startswith(seq[:-2])
+True
+```
+
+A `SegStr` object hashes to the value of its (space-separated) string:
+
+```python
+>>> len({seq, 'eː n t j ə'})
+1
+>>> seq in {'eː n t j ə'}
+True
+```
+
 ### Natural Class: `NatClass`
 
 **A class to represent a Natural class, in the sense of sets of segments represented intensionally as conjunctions of features.**
 
+```python
+>>> son = NatClass(feats={'+son'}, seg_inv=seginv)
+>>> son
+[+son]
+>>> 'ə' in son
+True
+>>> 'n' in son
+True
+>>> 't' in son
+False
+```
+
+The class also allows you to get the natural class's extension and the extension's complement, relative to the `SegInv` (in our example, only `{ə, t, n, j, eː}` are in `seginv`):
+
+```python
+>>> son.extension()
+{eː, j, ə, n}
+>>> son.extension_complement()
+{t}
+```
+
+You can also retrieve an extension (complement) directly from a `SegInv` object without creating a `NatClass` obj:
+
+```python
+>>> seginv.extension({'+syl'})
+{ə, eː}
+>>> seginv.extension_complement({'+syl'})
+{j, t, n}
+```
+
 ### Symbols: The `symbols` module
 
 The `symbols` module (techincally just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
```

### Comparing `algophon-0.0.3/pyproject.toml` & `algophon-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
@@ -24,8 +24,8 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools.package-data]
 algophon = ["ipa.txt"]
 
 [project.urls]
-Homepage = "https://github.com/cbelth/algophon"
+Homepage = "https://github.com/cbelth/algophon"
```

