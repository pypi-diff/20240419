# Comparing `tmp/xobjects-0.3.1.tar.gz` & `tmp/xobjects-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xobjects-0.3.1.tar", last modified: Thu Mar 21 15:24:57 2024, max compression
+gzip compressed data, was "xobjects-0.4.0.tar", last modified: Fri Apr 19 13:11:01 2024, max compression
```

## Comparing `xobjects-0.3.1.tar` & `xobjects-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-03-21 15:24:57.989439 xobjects-0.3.1/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.3.1/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      760 2024-03-21 15:24:57.989344 xobjects-0.3.1/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.3.1/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)      180 2024-03-21 15:24:57.989895 xobjects-0.3.1/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1255 2024-02-09 07:53:11.000000 xobjects-0.3.1/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-03-21 15:24:57.930170 xobjects-0.3.1/tests/
--rw-r--r--   0 giadarol   (503) staff       (20)      724 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_align.py
--rw-r--r--   0 giadarol   (503) staff       (20)     7571 2023-12-01 11:05:57.000000 xobjects-0.3.1/tests/test_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3641 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_buffer.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16680 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_capi.py
--rw-r--r--   0 giadarol   (503) staff       (20)      743 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_chunk.py
--rw-r--r--   0 giadarol   (503) staff       (20)      486 2023-12-01 11:05:57.000000 xobjects-0.3.1/tests/test_context_opencl.py
--rw-r--r--   0 giadarol   (503) staff       (20)     9220 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_hybrid_class.py
--rw-r--r--   0 giadarol   (503) staff       (20)     7409 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_kernel.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2915 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_linked_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4614 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_nplike_arrays.py
--rw-r--r--   0 giadarol   (503) staff       (20)     8856 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_ref.py
--rw-r--r--   0 giadarol   (503) staff       (20)      944 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_scalars.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3865 2023-11-10 09:58:00.000000 xobjects-0.3.1/tests/test_shared_memory.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1160 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_strides.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1264 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_string.py
--rw-r--r--   0 giadarol   (503) staff       (20)     6677 2023-04-03 19:20:50.000000 xobjects-0.3.1/tests/test_struct.py
--rw-r--r--   0 giadarol   (503) staff       (20)      692 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_to_json.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3202 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_typeutils.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1540 2023-03-23 11:04:29.000000 xobjects-0.3.1/tests/test_unionref.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-03-21 15:24:57.987054 xobjects-0.3.1/xobjects/
--rw-r--r--   0 giadarol   (503) staff       (20)      915 2023-04-03 19:20:50.000000 xobjects-0.3.1/xobjects/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/_patch_pyopencl_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2024-03-21 15:24:28.000000 xobjects-0.3.1/xobjects/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)    23133 2023-12-01 11:05:57.000000 xobjects-0.3.1/xobjects/array.py
--rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/capi.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21026 2024-02-29 11:25:24.000000 xobjects-0.3.1/xobjects/context.py
--rw-r--r--   0 giadarol   (503) staff       (20)    29742 2024-03-21 15:20:23.000000 xobjects-0.3.1/xobjects/context_cpu.py
--rw-r--r--   0 giadarol   (503) staff       (20)    24625 2024-02-29 11:25:24.000000 xobjects-0.3.1/xobjects/context_cupy.py
--rw-r--r--   0 giadarol   (503) staff       (20)    17205 2024-02-29 11:25:24.000000 xobjects-0.3.1/xobjects/context_pyopencl.py
--rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.3.1/xobjects/general.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12927 2023-10-20 13:56:24.000000 xobjects-0.3.1/xobjects/hybrid_class.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/linkedarray.py
--rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/ref.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/scalar.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/specialize_source.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/string.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16357 2024-02-29 11:25:24.000000 xobjects-0.3.1/xobjects/struct.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2638 2023-04-24 06:51:14.000000 xobjects-0.3.1/xobjects/test_helpers.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/typeutils.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.3.1/xobjects/union.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-03-21 15:24:57.988770 xobjects-0.3.1/xobjects.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      760 2024-03-21 15:24:57.000000 xobjects-0.3.1/xobjects.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)     1079 2024-03-21 15:24:57.000000 xobjects-0.3.1/xobjects.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2024-03-21 15:24:57.000000 xobjects-0.3.1/xobjects.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       45 2024-03-21 15:24:57.000000 xobjects-0.3.1/xobjects.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        9 2024-03-21 15:24:57.000000 xobjects-0.3.1/xobjects.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-04-19 13:11:00.996792 xobjects-0.4.0/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.4.0/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      760 2024-04-19 13:11:00.996661 xobjects-0.4.0/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.4.0/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)      180 2024-04-19 13:11:00.997297 xobjects-0.4.0/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1255 2024-02-09 07:53:11.000000 xobjects-0.4.0/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-04-19 13:11:00.966689 xobjects-0.4.0/tests/
+-rw-r--r--   0 giadarol   (503) staff       (20)      724 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_align.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     7705 2024-04-19 13:10:14.000000 xobjects-0.4.0/tests/test_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3641 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_buffer.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16680 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_capi.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      743 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_chunk.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      486 2023-12-01 11:05:57.000000 xobjects-0.4.0/tests/test_context_opencl.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     9746 2024-04-19 13:10:14.000000 xobjects-0.4.0/tests/test_hybrid_class.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     7409 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_kernel.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2915 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_linked_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4614 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_nplike_arrays.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     8856 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_ref.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      944 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_scalars.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3865 2023-11-10 09:58:00.000000 xobjects-0.4.0/tests/test_shared_memory.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1160 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_strides.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1264 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_string.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     6677 2023-04-03 19:20:50.000000 xobjects-0.4.0/tests/test_struct.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      692 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_to_json.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3202 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_typeutils.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1540 2023-03-23 11:04:29.000000 xobjects-0.4.0/tests/test_unionref.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-04-19 13:11:00.992277 xobjects-0.4.0/xobjects/
+-rw-r--r--   0 giadarol   (503) staff       (20)      958 2024-04-19 13:10:14.000000 xobjects-0.4.0/xobjects/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/_patch_pyopencl_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2024-04-19 13:10:30.000000 xobjects-0.4.0/xobjects/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    23254 2024-04-19 13:10:14.000000 xobjects-0.4.0/xobjects/array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/capi.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21026 2024-02-29 11:25:24.000000 xobjects-0.4.0/xobjects/context.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    29774 2024-04-19 13:10:14.000000 xobjects-0.4.0/xobjects/context_cpu.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    24625 2024-02-29 11:25:24.000000 xobjects-0.4.0/xobjects/context_cupy.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    17205 2024-02-29 11:25:24.000000 xobjects-0.4.0/xobjects/context_pyopencl.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.4.0/xobjects/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    14038 2024-04-19 13:10:14.000000 xobjects-0.4.0/xobjects/hybrid_class.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/linkedarray.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/ref.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/scalar.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/specialize_source.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/string.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16357 2024-02-29 11:25:24.000000 xobjects-0.4.0/xobjects/struct.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2895 2024-04-19 13:10:14.000000 xobjects-0.4.0/xobjects/test_helpers.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/typeutils.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.4.0/xobjects/union.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2024-04-19 13:11:00.995840 xobjects-0.4.0/xobjects.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      760 2024-04-19 13:11:00.000000 xobjects-0.4.0/xobjects.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)     1079 2024-04-19 13:11:00.000000 xobjects-0.4.0/xobjects.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2024-04-19 13:11:00.000000 xobjects-0.4.0/xobjects.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       45 2024-04-19 13:11:00.000000 xobjects-0.4.0/xobjects.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        9 2024-04-19 13:11:00.000000 xobjects-0.4.0/xobjects.egg-info/top_level.txt
```

### Comparing `xobjects-0.3.1/LICENSE` & `xobjects-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/PKG-INFO` & `xobjects-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.3.1
+Version: 0.4.0
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xobjects-0.3.1/setup.py` & `xobjects-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_align.py` & `xobjects-0.4.0/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_array.py` & `xobjects-0.4.0/tests/test_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,20 @@
 
 def test_array_allocation():
     MyArray = xo.Int64[10]
     ss = MyArray()
     assert ss._itemtype == xo.Int64
 
 
+def test_static_array_allocation_with_none():
+    MyArray = xo.Int64[10]
+    ss = MyArray(None)
+    assert ss._itemtype == xo.Int64
+
+
 def test_array_sshape_stype():
     Array1D = xo.Int64[3]
     Array2D = xo.Int64[2, 3]
     Array3D = xo.Int64[2, 3, 4]
 
     for cls in Array1D, Array2D, Array3D:
         ss = cls()
```

### Comparing `xobjects-0.3.1/tests/test_buffer.py` & `xobjects-0.4.0/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_capi.py` & `xobjects-0.4.0/tests/test_capi.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_chunk.py` & `xobjects-0.4.0/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_hybrid_class.py` & `xobjects-0.4.0/tests/test_hybrid_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,7 +306,27 @@
     inner = InnerClass(a=2, b=range(10))
     outer = OuterClass(inner=inner, inner_renamed=inner, _buffer=inner._buffer)
 
     different_buffer = xo.context_default.new_buffer()
 
     with pytest.raises(MemoryError):
         outer.inner.move(_buffer=different_buffer)
+
+
+def test_to_json_defaults():
+    class A(xo.HybridClass):
+        _xofields = {
+            "a": xo.Float64[3],
+            "b": xo.Int64,
+            "c": xo.Field(xo.Int32, default=42),
+            "d": xo.Field(xo.Int32, default_factory=lambda: 7),
+        }
+
+    a = A(c=42)
+    assert a.to_dict() == {"__class__": "A"}
+
+    b = A(a=[1, 2, 3], d=8)
+    b_dict = b.to_dict()
+    assert b_dict.pop("__class__") == "A"
+    assert np.all(b_dict.pop("a") == [1, 2, 3])
+    assert b_dict.pop("d") == 8
+    assert b_dict == {}
```

### Comparing `xobjects-0.3.1/tests/test_kernel.py` & `xobjects-0.4.0/tests/test_kernel.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_linked_array.py` & `xobjects-0.4.0/tests/test_linked_array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_nplike_arrays.py` & `xobjects-0.4.0/tests/test_nplike_arrays.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_ref.py` & `xobjects-0.4.0/tests/test_ref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_scalars.py` & `xobjects-0.4.0/tests/test_scalars.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_shared_memory.py` & `xobjects-0.4.0/tests/test_shared_memory.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_strides.py` & `xobjects-0.4.0/tests/test_strides.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_string.py` & `xobjects-0.4.0/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_struct.py` & `xobjects-0.4.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_to_json.py` & `xobjects-0.4.0/tests/test_to_json.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_typeutils.py` & `xobjects-0.4.0/tests/test_typeutils.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/tests/test_unionref.py` & `xobjects-0.4.0/tests/test_unionref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/__init__.py` & `xobjects-0.4.0/xobjects/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,8 +32,10 @@
 
 from .hybrid_class import JEncoder, HybridClass, MetaHybridClass, ThisClass
 
 from .linkedarray import BypassLinked
 
 from .general import _print
 
+from .test_helpers import assert_allclose
+
 from ._version import __version__
```

### Comparing `xobjects-0.3.1/xobjects/_patch_pyopencl_array.py` & `xobjects-0.4.0/xobjects/_patch_pyopencl_array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/array.py` & `xobjects-0.4.0/xobjects/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,18 +303,22 @@
         info = Info()
         extra = {}
         if cls._size is not None:
             # static,static array
             if len(args) == 0:
                 value = None
             elif len(args) == 1:
-                shape = get_shape_from_array(args[0], len(cls._shape))
-                if shape != cls._shape:
-                    raise ValueError(f"shape not valid for {args[0]} ")
-                value = args[0]
+                (arg,) = args
+                if arg is None:
+                    value = None
+                else:
+                    shape = get_shape_from_array(arg, len(cls._shape))
+                    if shape != cls._shape:
+                        raise ValueError(f"shape not valid for {arg} ")
+                    value = arg
             elif len(args) > 1:
                 raise ValueError("too many arguments")
             size = cls._size
             shape = cls._shape
             order = cls._order
             strides = cls._strides
             offsets = np.empty(shape, dtype="int64")
```

### Comparing `xobjects-0.3.1/xobjects/capi.py` & `xobjects-0.4.0/xobjects/capi.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/context.py` & `xobjects-0.4.0/xobjects/context.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/context_cpu.py` & `xobjects-0.4.0/xobjects/context_cpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         Args:
             omp_num_threads (int | Literal['auto']): Number of threads to be
             used by OpenMP. If 0, no parallelization is used. If 'auto', the
             number of threads is selected automatically by OpenMP.
         """
         super().__init__()
         self.omp_num_threads = omp_num_threads
-        if omp_num_threads==0:
+        if omp_num_threads == 0:
             self.allow_prebuilt_kernels = True
 
     def __str__(self):
         if not self.openmp_enabled:
             return super().__str__()
         else:
             return f"{type(self).__name__}:{self.omp_num_threads}"
@@ -513,18 +513,20 @@
 
         return module
 
     @staticmethod
     def cffi_module_for_c_types(c_types, containing_dir="."):
         path = Path(containing_dir)
         for file in path.iterdir():
-            if not file.suffix in ['.so', '.dylib', '.dll']:
+            if not file.suffix in [".so", ".dylib", ".dll"]:
                 continue
-            module_name = file.name.split('.')[0]
-            spec = importlib.util.spec_from_file_location(module_name, str(file))
+            module_name = file.name.split(".")[0]
+            spec = importlib.util.spec_from_file_location(
+                module_name, str(file)
+            )
             module = importlib.util.module_from_spec(spec)
 
             typedefs = module.ffi.list_types()[0]
             if set(c_types) <= set(typedefs):
                 return module_name
 
         return None
```

### Comparing `xobjects-0.3.1/xobjects/context_cupy.py` & `xobjects-0.4.0/xobjects/context_cupy.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/context_pyopencl.py` & `xobjects-0.4.0/xobjects/context_pyopencl.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/hybrid_class.py` & `xobjects-0.4.0/xobjects/hybrid_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,22 @@
         else:
             return getattr(container._xobject, self.name)
 
     def __set__(self, container, value):
         if self.isnplikearray:
             self.__get__(container=container)[:] = value
         elif hasattr(value, "_xobject"):  # value is a dressed xobject
+
             # Copy xobject data from value inside self._xobject
             # (unless same memory area or Ref and same buffer,
             #  in the latter case reference mechanism is used)
             if not (
                 container._xobject._buffer is value._xobject._buffer
-                and getattr(container._xobject, self.name)._offset
-                == value._xobject._offset
+                and (getattr(container._xobject, self.name) is not None and
+                    getattr(container._xobject, self.name)._offset == value._xobject._offset)
             ):
                 setattr(container._xobject, self.name, value._xobject)
 
             if isinstance(getattr(container._XoStruct, self.name).ftype, Ref):
                 if value._buffer is not container._buffer:
                     raise MemoryError(
                         "Cannot make a reference to an object in "
@@ -194,23 +195,24 @@
 
         return new_class
 
 
 class HybridClass(metaclass=MetaHybridClass):
     _movable = True
     _overridable = True
+    _force_moveable = False
 
     def move(self, _context=None, _buffer=None, _offset=None):
-        if not self._movable:
+        if not self._movable and not self._force_moveable:
             raise MemoryError(
                 "This object cannot be moved, likely because it "
                 "lives within another. Please, make a copy."
             )
 
-        if self._xobject._has_refs:
+        if self._xobject._has_refs and not self._force_moveable:
             raise MemoryError(
                 "This object cannot be moved, as it contains "
                 "references to other objects."
             )
 
         self._xobject = self._xobject.__class__(
             self._xobject, _context=_context, _buffer=_buffer, _offset=_offset
@@ -281,50 +283,58 @@
         out = {"__class__": self.__class__.__name__}
         # Use a cpu copy by default:
         if copy_to_cpu:
             obj = self.copy(_context=context_default)
         else:
             obj = self
 
-        for ff in obj._fields:
-            if (
-                hasattr(self, "_skip_in_to_dict")
-                and ff in self._skip_in_to_dict
-            ):
-                continue
+        skip_fields = set(getattr(obj, "_skip_in_to_dict", []))
+        additional_fields = set(getattr(obj, "_store_in_to_dict", []))
+        fields_to_store = (set(obj._fields) - skip_fields) | additional_fields
+
+        defaults = {}
+        for field in obj._XoStruct._fields:
+            try:
+                defaults[field.name] = field.get_default()
+            except (TypeError, ValueError):
+                # The above can fail with different error types
+                # if a field type is dynamic.
+                pass
+
+        for ff in fields_to_store:
             vv = getattr(obj, ff)
             if hasattr(vv, "to_dict"):
                 out[ff] = vv.to_dict()
             elif hasattr(vv, "_to_dict"):
                 out[ff] = vv._to_dict()
-            else:
+            elif np.any(defaults.get(ff) != vv):
+                # Only include those scalar values that are not default.
                 out[ff] = vv
 
-        if hasattr(obj, "_store_in_to_dict"):
-            for nn in obj._store_in_to_dict:
-                ww = getattr(obj, nn)
-                if hasattr(ww, "to_dict"):
-                    out[nn] = ww.to_dict()
-                elif hasattr(ww, "_to_dict"):
-                    out[nn] = ww._to_dict()
-                else:
-                    out[nn] = ww
-
         return out
 
-    @classmethod
-    def from_dict(cls, dct, _context=None, _buffer=None, _offset=None):
+    @staticmethod
+    def _static_from_dict(cls, dct, _context=None, _buffer=None, _offset=None):
         return cls(
             **dct,
             _context=_context,
             _buffer=_buffer,
             _offset=_offset,
             _kwargs_name_check=False,
         )
 
+    @classmethod
+    def from_dict(cls, dct, _context=None, _buffer=None, _offset=None):
+        return HybridClass._static_from_dict(cls,
+            dct,
+            _context=_context,
+            _buffer=_buffer,
+            _offset=_offset,
+        )
+
     def copy(self, _context=None, _buffer=None, _offset=None):
         if _context is None and _buffer is None:
             _context = self._xobject._buffer.context
         # This makes a copy of the xobject
         xobject = self._XoStruct(
             self._xobject, _context=_context, _buffer=_buffer, _offset=_offset
         )
@@ -363,13 +373,31 @@
             "`extra_sources` has been removed. Use `_extra_c_sources` instead."
         )
 
     def compile_kernels(self, *args, **kwargs):
         return self._xobject.compile_kernels(*args, **kwargs)
 
     def __repr__(self):
-        args = [f"{fname}={getattr(self, fname)}" for fname in self._fields]
+
+        if hasattr(self, "_repr_fields"):
+            fnames = self._repr_fields
+        else:
+            fnames = []
+            if hasattr(self, "_add_to_repr"):
+                fnames += self._add_to_repr
+            fnames += [fname for fname in self._fields]
+            if hasattr(self, "_skip_in_repr"):
+                fnames = [ff for ff in fnames if ff not in self._skip_in_repr]
+
+        args = []
+        for fname in fnames:
+            vv = getattr(self, fname)
+            if isinstance(vv, float):
+                vvrepr = f"{vv:.3g}"
+            else:
+                vvrepr = repr(vv)
+            args.append(f"{fname}={vvrepr}")
         return f'{type(self).__name__}({", ".join(args)})'
 
 
 class ThisClass:  # Place holder
     pass
```

### Comparing `xobjects-0.3.1/xobjects/linkedarray.py` & `xobjects-0.4.0/xobjects/linkedarray.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/ref.py` & `xobjects-0.4.0/xobjects/ref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/scalar.py` & `xobjects-0.4.0/xobjects/scalar.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/specialize_source.py` & `xobjects-0.4.0/xobjects/specialize_source.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/string.py` & `xobjects-0.4.0/xobjects/string.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/struct.py` & `xobjects-0.4.0/xobjects/struct.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/test_helpers.py` & `xobjects-0.4.0/xobjects/test_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # copyright ################################# #
 # This file is part of the Xobjects Package.  #
 # Copyright (c) CERN, 2022.                   #
 # ########################################### #
 
 from functools import wraps
 from typing import Callable, Iterable, Union
+from numpy.testing import assert_allclose as np_assert_allclose
 
 import pytest
 
 from .context import get_context_from_string, get_test_contexts
 
 
 def _for_all_test_contexts_excluding(
@@ -79,7 +80,14 @@
 def requires_context(context_name: str):
     ctx_names = (type(ctx).__name__ for ctx in get_test_contexts())
 
     if {context_name} & set(ctx_names):  # proceed as normal
         return lambda test_function: test_function
 
     return pytest.mark.skip(f"{context_name} is unavailable on this platform.")
+
+def assert_allclose(a, b, rtol=1e-7, atol=1e-7):
+    if hasattr(a, 'get'):
+        a = a.get()
+    if hasattr(b, 'get'):
+        b = b.get()
+    np_assert_allclose(a, b, rtol=rtol, atol=atol)
```

### Comparing `xobjects-0.3.1/xobjects/typeutils.py` & `xobjects-0.4.0/xobjects/typeutils.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects/union.py` & `xobjects-0.4.0/xobjects/union.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.3.1/xobjects.egg-info/PKG-INFO` & `xobjects-0.4.0/xobjects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.3.1
+Version: 0.4.0
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xobjects-0.3.1/xobjects.egg-info/SOURCES.txt` & `xobjects-0.4.0/xobjects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

