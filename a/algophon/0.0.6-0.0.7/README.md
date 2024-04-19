# Comparing `tmp/algophon-0.0.6.tar.gz` & `tmp/algophon-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.6.tar", last modified: Fri Apr 19 16:31:09 2024, max compression
+gzip compressed data, was "algophon-0.0.7.tar", last modified: Fri Apr 19 17:55:21 2024, max compression
```

## Comparing `algophon-0.0.6.tar` & `algophon-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 16:31:09.992761 algophon-0.0.6/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.6/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 16:31:09.992155 algophon-0.0.6/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.6/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 16:31:09.956607 algophon-0.0.6/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.6/algophon/__init__.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 16:31:09.970140 algophon-0.0.6/algophon/dist/
--rw-r--r--   0 u6052607   (503) staff       (20)     4045 2024-04-19 14:52:46.000000 algophon-0.0.6/algophon/dist/edit_distance.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 16:31:09.977339 algophon-0.0.6/algophon/ipa/
--rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.0.6/algophon/ipa/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1347 2024-04-19 14:16:56.000000 algophon-0.0.6/algophon/ipa/convert.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.6/algophon/ipa.txt
--rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.6/algophon/natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.6/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     4745 2024-04-19 14:22:59.000000 algophon-0.0.6/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5664 2024-04-19 16:30:11.000000 algophon-0.0.6/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.6/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 16:31:09.991460 algophon-0.0.6/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 16:31:09.000000 algophon-0.0.6/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      472 2024-04-19 16:31:09.000000 algophon-0.0.6/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-19 16:31:09.000000 algophon-0.0.6/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-19 16:31:09.000000 algophon-0.0.6/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-19 16:30:38.000000 algophon-0.0.6/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-19 16:31:09.992816 algophon-0.0.6/setup.cfg
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 16:31:09.990573 algophon-0.0.6/tests/
--rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.6/tests/test_natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.6/tests/test_seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     2132 2024-04-19 00:05:44.000000 algophon-0.0.6/tests/test_seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1462 2024-04-19 16:29:02.000000 algophon-0.0.6/tests/test_segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      740 2024-04-18 23:42:58.000000 algophon-0.0.6/tests/tester.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.845556 algophon-0.0.7/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.7/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 17:55:21.845037 algophon-0.0.7/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     9006 2024-04-19 00:09:14.000000 algophon-0.0.7/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.823849 algophon-0.0.7/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      168 2024-04-18 16:51:58.000000 algophon-0.0.7/algophon/__init__.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.833758 algophon-0.0.7/algophon/dist/
+-rw-r--r--   0 u6052607   (503) staff       (20)     4045 2024-04-19 14:52:46.000000 algophon-0.0.7/algophon/dist/edit_distance.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.839194 algophon-0.0.7/algophon/ipa/
+-rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.0.7/algophon/ipa/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1347 2024-04-19 14:16:56.000000 algophon-0.0.7/algophon/ipa/convert.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.7/algophon/ipa.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.0.7/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1173 2024-04-18 18:31:25.000000 algophon-0.0.7/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     4745 2024-04-19 14:22:59.000000 algophon-0.0.7/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5660 2024-04-19 17:53:50.000000 algophon-0.0.7/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      166 2024-04-18 18:39:21.000000 algophon-0.0.7/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.844452 algophon-0.0.7/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)     9611 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      472 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-19 17:55:21.000000 algophon-0.0.7/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      789 2024-04-19 17:55:15.000000 algophon-0.0.7/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-19 17:55:21.845614 algophon-0.0.7/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-19 17:55:21.843870 algophon-0.0.7/tests/
+-rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.0.7/tests/test_natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1273 2024-04-18 23:49:35.000000 algophon-0.0.7/tests/test_seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     2132 2024-04-19 00:05:44.000000 algophon-0.0.7/tests/test_seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1696 2024-04-19 17:54:23.000000 algophon-0.0.7/tests/test_segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      740 2024-04-18 23:42:58.000000 algophon-0.0.7/tests/tester.py
```

### Comparing `algophon-0.0.6/LICENSE` & `algophon-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/PKG-INFO` & `algophon-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `algophon-0.0.6/README.md` & `algophon-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/algophon/dist/edit_distance.py` & `algophon-0.0.7/algophon/dist/edit_distance.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/algophon/ipa/convert.py` & `algophon-0.0.7/algophon/ipa/convert.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/algophon/ipa.txt` & `algophon-0.0.7/algophon/ipa.txt`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/algophon/natclass.py` & `algophon-0.0.7/algophon/natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/algophon/seg.py` & `algophon-0.0.7/algophon/seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/algophon/seginv.py` & `algophon-0.0.7/algophon/seginv.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/algophon/segstr.py` & `algophon-0.0.7/algophon/segstr.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     
     def __lt__(self, other) -> bool:
         '''
         :other: a SegStr object
         '''
         if not isinstance(other, SegStr):
             raise ValueError(f'Cannot compare a SegStr object with an object of type {type(other)}')
-        return self._segs() < other._segs()
+        return self._segs < other._segs
     
     def __getitem__(self, idx):
         '''
         Handles slicing and indexing like a str or list
 
         :return: 
             - Slicing: SegStr object containing the slice
```

### Comparing `algophon-0.0.6/algophon.egg-info/PKG-INFO` & `algophon-0.0.7/algophon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `algophon-0.0.6/pyproject.toml` & `algophon-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
```

### Comparing `algophon-0.0.6/tests/test_natclass.py` & `algophon-0.0.7/tests/test_natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/tests/test_seg.py` & `algophon-0.0.7/tests/test_seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/tests/test_seginv.py` & `algophon-0.0.7/tests/test_seginv.py`

 * *Files identical despite different names*

### Comparing `algophon-0.0.6/tests/test_segstr.py` & `algophon-0.0.7/tests/test_segstr.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,10 +39,18 @@
         assert(len({x, 'eː n t j ə', SegStr('eː n t j ə', seginv=SegInv())}) == 1)
 
     def test_concat(self):
         x = SegStr('eː n t', seginv=SegInv())
         y = SegStr('j ə', seginv=SegInv())
         assert(x + y == 'eː n t j ə')
 
+    def test_lt(self):
+        x = SegStr('a', seginv=SegInv())
+        y = SegStr('b', seginv=SegInv())
+        assert(x < y)
+
+        x = SegStr('a b', seginv=SegInv())
+        y = SegStr('b', seginv=SegInv())
+        assert(x < y)
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `algophon-0.0.6/tests/tester.py` & `algophon-0.0.7/tests/tester.py`

 * *Files identical despite different names*

