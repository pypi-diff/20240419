# Comparing `tmp/fast_edges_extraction-0.1.1.tar.gz` & `tmp/fast_edges_extraction-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_edges_extraction-0.1.1.tar", last modified: Tue Mar 12 13:59:26 2024, max compression
+gzip compressed data, was "fast_edges_extraction-0.1.2.tar", last modified: Fri Apr 19 09:09:32 2024, max compression
```

## Comparing `fast_edges_extraction-0.1.1.tar` & `fast_edges_extraction-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:59:26.644860 fast_edges_extraction-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-12 13:59:11.000000 fast_edges_extraction-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-12 13:59:26.644860 fast_edges_extraction-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-12 13:59:11.000000 fast_edges_extraction-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:59:26.640860 fast_edges_extraction-0.1.1/fast_edges_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-12 13:59:11.000000 fast_edges_extraction-0.1.1/fast_edges_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1213707 2024-03-12 13:59:25.000000 fast_edges_extraction-0.1.1/fast_edges_extraction/_extract_edges.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:59:26.644860 fast_edges_extraction-0.1.1/fast_edges_extraction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-12 13:59:26.000000 fast_edges_extraction-0.1.1/fast_edges_extraction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-12 13:59:26.000000 fast_edges_extraction-0.1.1/fast_edges_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 13:59:26.000000 fast_edges_extraction-0.1.1/fast_edges_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 13:59:26.000000 fast_edges_extraction-0.1.1/fast_edges_extraction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-12 13:59:26.000000 fast_edges_extraction-0.1.1/fast_edges_extraction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-12 13:59:11.000000 fast_edges_extraction-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 13:59:26.644860 fast_edges_extraction-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-12 13:59:11.000000 fast_edges_extraction-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 13:59:26.644860 fast_edges_extraction-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-12 13:59:11.000000 fast_edges_extraction-0.1.1/tests/test_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:09:32.575900 fast_edges_extraction-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 09:09:20.000000 fast_edges_extraction-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-19 09:09:32.575900 fast_edges_extraction-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-19 09:09:20.000000 fast_edges_extraction-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:09:32.571900 fast_edges_extraction-0.1.2/fast_edges_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-19 09:09:20.000000 fast_edges_extraction-0.1.2/fast_edges_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1215725 2024-04-19 09:09:31.000000 fast_edges_extraction-0.1.2/fast_edges_extraction/_extract_edges.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:09:32.575900 fast_edges_extraction-0.1.2/fast_edges_extraction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-19 09:09:32.000000 fast_edges_extraction-0.1.2/fast_edges_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-19 09:09:32.000000 fast_edges_extraction-0.1.2/fast_edges_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:09:32.000000 fast_edges_extraction-0.1.2/fast_edges_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 09:09:32.000000 fast_edges_extraction-0.1.2/fast_edges_extraction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 09:09:32.000000 fast_edges_extraction-0.1.2/fast_edges_extraction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-19 09:09:20.000000 fast_edges_extraction-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:09:32.575900 fast_edges_extraction-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 09:09:20.000000 fast_edges_extraction-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:09:32.575900 fast_edges_extraction-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-19 09:09:20.000000 fast_edges_extraction-0.1.2/tests/test_consistency.py
```

### Comparing `fast_edges_extraction-0.1.1/LICENSE` & `fast_edges_extraction-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_edges_extraction-0.1.1/PKG-INFO` & `fast_edges_extraction-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_edges_extraction
-Version: 0.1.1
+Version: 0.1.2
 Summary: Edge extraction for triangle meshes
 Author: Louis Pujol
 License: MIT License
         
         Copyright (c) 2023 Louis Pujol
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,18 @@
 Requires-Dist: numpy
 
 fast-edges-extraction
 =====================
 
 Cython implementation of edges extraction from triangles as well as adjacency information (edge degrees and adjacent points/triangles for manifold and boundary edges).
 
+```bash
+pip install fast-edges-extraction
+```
+
 Example
 -------
 
 ![](example.png)
 
 
 - Extract the edges from the triangles
```

### Comparing `fast_edges_extraction-0.1.1/README.md` & `fast_edges_extraction-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 fast-edges-extraction
 =====================
 
 Cython implementation of edges extraction from triangles as well as adjacency information (edge degrees and adjacent points/triangles for manifold and boundary edges).
 
+```bash
+pip install fast-edges-extraction
+```
+
 Example
 -------
 
 ![](example.png)
 
 
 - Extract the edges from the triangles
```

### Comparing `fast_edges_extraction-0.1.1/fast_edges_extraction/__init__.py` & `fast_edges_extraction-0.1.2/fast_edges_extraction/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,13 +59,13 @@
         raise ValueError(msg)
 
     (
         edges,
         degrees,
         adjacent_triangles,
         adjacent_points
-    ) = extract_edges_cython(triangles.astype(np.int_))
+    ) = extract_edges_cython(triangles.astype(np.int64))
 
     if not return_adjacency:
         return edges
 
     return edges, degrees, adjacent_triangles, adjacent_points
```

### Comparing `fast_edges_extraction-0.1.1/fast_edges_extraction/_extract_edges.c` & `fast_edges_extraction-0.1.2/fast_edges_extraction/_extract_edges.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/core/include",
             "fast_edges_extraction"
         ],
         "language": "c",
         "name": "fast_edges_extraction._extract_edges",
         "sources": [
             "fast_edges_extraction/_extract_edges.pyx"
         ]
@@ -50,18 +50,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -145,14 +145,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -206,14 +208,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -267,60 +271,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -403,14 +430,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1647,193 +1677,193 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 
 /* "fast_edges_extraction/_extract_edges.pyx":11
  * 
- * INT_DTYPE = np.int_
- * ctypedef cnp.int_t INT_DTYPE_t             # <<<<<<<<<<<<<<
+ * INT_DTYPE = np.int64
+ * ctypedef cnp.int64_t INT_DTYPE_t             # <<<<<<<<<<<<<<
  * 
  * 
  */
-typedef __pyx_t_5numpy_int_t __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t;
+typedef __pyx_t_5numpy_int64_t __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t;
 /* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
@@ -1859,42 +1889,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2682,30 +2712,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -3063,31 +3093,31 @@
 #define __pyx_get_slice_count_pointer(memview) (&memview->acquisition_count)
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XCLEAR_MEMVIEW(slice, have_gil) __Pyx_XCLEAR_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XCLEAR_MEMVIEW(__Pyx_memviewslice *, int, int);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_long(npy_long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_int64(npy_int64 value);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE npy_long __Pyx_PyInt_As_npy_long(PyObject *);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+static CYTHON_INLINE npy_int64 __Pyx_PyInt_As_npy_int64(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
@@ -3233,15 +3263,14 @@
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k__24[] = "?";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_got[] = " (got ";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_axis[] = "axis";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
@@ -3263,14 +3292,15 @@
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_edges[] = "edges";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_index[] = "index";
+static const char __pyx_k_int64[] = "int64";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_order[] = "order";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_arange[] = "arange";
@@ -3584,15 +3614,15 @@
   PyObject *__pyx_kp_u_got_differing_extents_in_dimensi;
   PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_id;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_index;
   PyObject *__pyx_n_s_indice_ref;
   PyObject *__pyx_n_s_initializing;
-  PyObject *__pyx_n_s_int;
+  PyObject *__pyx_n_s_int64;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_itemsize;
   PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
   PyObject *__pyx_n_s_j;
   PyObject *__pyx_n_s_k;
   PyObject *__pyx_n_s_l;
@@ -3833,15 +3863,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_id);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_indice_ref);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
-  Py_CLEAR(clear_module_state->__pyx_n_s_int);
+  Py_CLEAR(clear_module_state->__pyx_n_s_int64);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_itemsize);
   Py_CLEAR(clear_module_state->__pyx_kp_s_itemsize_0_for_cython_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_j);
   Py_CLEAR(clear_module_state->__pyx_n_s_k);
   Py_CLEAR(clear_module_state->__pyx_n_s_l);
@@ -4060,15 +4090,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_id);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_indice_ref);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
-  Py_VISIT(traverse_module_state->__pyx_n_s_int);
+  Py_VISIT(traverse_module_state->__pyx_n_s_int64);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_itemsize);
   Py_VISIT(traverse_module_state->__pyx_kp_s_itemsize_0_for_cython_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_j);
   Py_VISIT(traverse_module_state->__pyx_n_s_k);
   Py_VISIT(traverse_module_state->__pyx_n_s_l);
@@ -4323,15 +4353,15 @@
 #define __pyx_kp_u_got_differing_extents_in_dimensi __pyx_mstate_global->__pyx_kp_u_got_differing_extents_in_dimensi
 #define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_id __pyx_mstate_global->__pyx_n_s_id
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
 #define __pyx_n_s_indice_ref __pyx_mstate_global->__pyx_n_s_indice_ref
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
-#define __pyx_n_s_int __pyx_mstate_global->__pyx_n_s_int
+#define __pyx_n_s_int64 __pyx_mstate_global->__pyx_n_s_int64
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_itemsize __pyx_mstate_global->__pyx_n_s_itemsize
 #define __pyx_kp_s_itemsize_0_for_cython_array __pyx_mstate_global->__pyx_kp_s_itemsize_0_for_cython_array
 #define __pyx_n_s_j __pyx_mstate_global->__pyx_n_s_j
 #define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
 #define __pyx_n_s_l __pyx_mstate_global->__pyx_n_s_l
@@ -18046,261 +18076,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18309,29 +18339,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18342,15 +18372,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18359,29 +18389,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18392,15 +18422,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18409,29 +18439,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18442,15 +18472,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18459,29 +18489,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18492,15 +18522,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18509,29 +18539,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18542,217 +18572,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18768,15 +18798,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18784,68 +18814,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18853,15 +18883,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18876,15 +18906,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18900,15 +18930,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18916,68 +18946,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18985,15 +19015,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19008,15 +19038,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19032,15 +19062,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19048,68 +19078,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19117,15 +19147,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19140,170 +19170,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19415,16 +19445,16 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_21fast_edges_extraction_14_extract_edges_extract_edges(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_triangles) {
-  int __pyx_v_i;
-  int __pyx_v_n_triangles;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_v_i;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_v_n_triangles;
   __Pyx_memviewslice __pyx_v_adjacent_triangles = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_adjacent_points = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_edge_degrees = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_edges = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_order = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_short_edges = { 0, 0, { 0 }, { 0 }, { 0 } };
   __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_v_n_keep;
@@ -19435,31 +19465,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_t_7 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  int __pyx_t_8;
-  int __pyx_t_9;
-  int __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_t_8;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_t_9;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_t_10;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   int __pyx_t_13;
-  Py_ssize_t __pyx_t_14;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   __Pyx_memviewslice __pyx_t_19 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  long __pyx_t_20;
-  long __pyx_t_21;
-  Py_ssize_t __pyx_t_22;
-  Py_ssize_t __pyx_t_23;
-  int __pyx_t_24;
+  Py_ssize_t __pyx_t_20;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_t_21;
+  __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t __pyx_t_22;
+  int __pyx_t_23;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("extract_edges", 1);
   __PYX_INC_MEMVIEW(&__pyx_v_triangles, 1);
 
   /* "fast_edges_extraction/_extract_edges.pyx":16
@@ -19516,34 +19545,34 @@
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_triangles, 1);
   __pyx_v_triangles = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
   /* "fast_edges_extraction/_extract_edges.pyx":24
  *     #Compute neighbors
- *     cdef int i, j, k, l
- *     cdef int n_triangles = triangles.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef INT_DTYPE_t i, j, k, l
+ *     cdef INT_DTYPE_t n_triangles = triangles.shape[0]             # <<<<<<<<<<<<<<
  * 
  *     cdef INT_DTYPE_t [:, :] adjacent_triangles = -1 * np.ones((3 * n_triangles, 2), dtype=INT_DTYPE)
  */
   __pyx_v_n_triangles = (__pyx_v_triangles.shape[0]);
 
   /* "fast_edges_extraction/_extract_edges.pyx":26
- *     cdef int n_triangles = triangles.shape[0]
+ *     cdef INT_DTYPE_t n_triangles = triangles.shape[0]
  * 
  *     cdef INT_DTYPE_t [:, :] adjacent_triangles = -1 * np.ones((3 * n_triangles, 2), dtype=INT_DTYPE)             # <<<<<<<<<<<<<<
  *     cdef INT_DTYPE_t [:, :] adjacent_points = -1 * np.ones((3 * n_triangles, 2), dtype=INT_DTYPE)
  *     cdef INT_DTYPE_t [:] edge_degrees = np.zeros(3 * n_triangles, dtype=INT_DTYPE)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ones); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_long((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_npy_int64((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 26, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
@@ -19582,15 +19611,15 @@
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_ones); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_long((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int64((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_4);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
@@ -19629,15 +19658,15 @@
  *     # edges store the (repeated edges)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_long((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_npy_int64((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error);
   __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
@@ -19665,15 +19694,15 @@
  *     for i in range(n_triangles):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_long((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int64((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
@@ -19755,45 +19784,45 @@
     /* "fast_edges_extraction/_extract_edges.pyx":36
  * 
  *         edges[3 * i, 0] = triangles[i, 0]
  *         edges[3 * i, 1] = triangles[i, 1]             # <<<<<<<<<<<<<<
  * 
  *         edges[3 * i + 1, 0] = triangles[i, 0]
  */
-    __pyx_t_12 = __pyx_v_i;
-    __pyx_t_11 = 1;
+    __pyx_t_11 = __pyx_v_i;
+    __pyx_t_12 = 1;
     __pyx_t_13 = -1;
-    if (__pyx_t_12 < 0) {
-      __pyx_t_12 += __pyx_v_triangles.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
-    } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles.shape[0])) __pyx_t_13 = 0;
     if (__pyx_t_11 < 0) {
-      __pyx_t_11 += __pyx_v_triangles.shape[1];
-      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 1;
-    } else if (unlikely(__pyx_t_11 >= __pyx_v_triangles.shape[1])) __pyx_t_13 = 1;
+      __pyx_t_11 += __pyx_v_triangles.shape[0];
+      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_11 >= __pyx_v_triangles.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_12 < 0) {
+      __pyx_t_12 += __pyx_v_triangles.shape[1];
+      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles.shape[1])) __pyx_t_13 = 1;
     if (unlikely(__pyx_t_13 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 36, __pyx_L1_error)
     }
-    __pyx_t_15 = (3 * __pyx_v_i);
-    __pyx_t_14 = 1;
+    __pyx_t_14 = (3 * __pyx_v_i);
+    __pyx_t_15 = 1;
     __pyx_t_13 = -1;
-    if (__pyx_t_15 < 0) {
-      __pyx_t_15 += __pyx_v_edges.shape[0];
-      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 0;
-    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
     if (__pyx_t_14 < 0) {
-      __pyx_t_14 += __pyx_v_edges.shape[1];
-      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 1;
-    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
+      __pyx_t_14 += __pyx_v_edges.shape[0];
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_edges.shape[1];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
     if (unlikely(__pyx_t_13 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 36, __pyx_L1_error)
     }
-    *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_15 * __pyx_v_edges.strides[0]) ) + __pyx_t_14 * __pyx_v_edges.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_triangles.data + __pyx_t_12 * __pyx_v_triangles.strides[0]) ) + __pyx_t_11 * __pyx_v_triangles.strides[1]) )));
+    *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_14 * __pyx_v_edges.strides[0]) ) + __pyx_t_15 * __pyx_v_edges.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_triangles.data + __pyx_t_11 * __pyx_v_triangles.strides[0]) ) + __pyx_t_12 * __pyx_v_triangles.strides[1]) )));
 
     /* "fast_edges_extraction/_extract_edges.pyx":38
  *         edges[3 * i, 1] = triangles[i, 1]
  * 
  *         edges[3 * i + 1, 0] = triangles[i, 0]             # <<<<<<<<<<<<<<
  *         edges[3 * i + 1, 1] = triangles[i, 2]
  * 
@@ -19833,45 +19862,45 @@
     /* "fast_edges_extraction/_extract_edges.pyx":39
  * 
  *         edges[3 * i + 1, 0] = triangles[i, 0]
  *         edges[3 * i + 1, 1] = triangles[i, 2]             # <<<<<<<<<<<<<<
  * 
  *         edges[3 * i + 2, 0] = triangles[i, 1]
  */
-    __pyx_t_12 = __pyx_v_i;
-    __pyx_t_11 = 2;
+    __pyx_t_11 = __pyx_v_i;
+    __pyx_t_12 = 2;
     __pyx_t_13 = -1;
-    if (__pyx_t_12 < 0) {
-      __pyx_t_12 += __pyx_v_triangles.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
-    } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles.shape[0])) __pyx_t_13 = 0;
     if (__pyx_t_11 < 0) {
-      __pyx_t_11 += __pyx_v_triangles.shape[1];
-      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 1;
-    } else if (unlikely(__pyx_t_11 >= __pyx_v_triangles.shape[1])) __pyx_t_13 = 1;
+      __pyx_t_11 += __pyx_v_triangles.shape[0];
+      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_11 >= __pyx_v_triangles.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_12 < 0) {
+      __pyx_t_12 += __pyx_v_triangles.shape[1];
+      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles.shape[1])) __pyx_t_13 = 1;
     if (unlikely(__pyx_t_13 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 39, __pyx_L1_error)
     }
-    __pyx_t_15 = ((3 * __pyx_v_i) + 1);
-    __pyx_t_14 = 1;
+    __pyx_t_14 = ((3 * __pyx_v_i) + 1);
+    __pyx_t_15 = 1;
     __pyx_t_13 = -1;
-    if (__pyx_t_15 < 0) {
-      __pyx_t_15 += __pyx_v_edges.shape[0];
-      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 0;
-    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
     if (__pyx_t_14 < 0) {
-      __pyx_t_14 += __pyx_v_edges.shape[1];
-      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 1;
-    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
+      __pyx_t_14 += __pyx_v_edges.shape[0];
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_edges.shape[1];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
     if (unlikely(__pyx_t_13 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 39, __pyx_L1_error)
     }
-    *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_15 * __pyx_v_edges.strides[0]) ) + __pyx_t_14 * __pyx_v_edges.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_triangles.data + __pyx_t_12 * __pyx_v_triangles.strides[0]) ) + __pyx_t_11 * __pyx_v_triangles.strides[1]) )));
+    *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_14 * __pyx_v_edges.strides[0]) ) + __pyx_t_15 * __pyx_v_edges.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_triangles.data + __pyx_t_11 * __pyx_v_triangles.strides[0]) ) + __pyx_t_12 * __pyx_v_triangles.strides[1]) )));
 
     /* "fast_edges_extraction/_extract_edges.pyx":41
  *         edges[3 * i + 1, 1] = triangles[i, 2]
  * 
  *         edges[3 * i + 2, 0] = triangles[i, 1]             # <<<<<<<<<<<<<<
  *         edges[3 * i + 2, 1] = triangles[i, 2]
  * 
@@ -19911,45 +19940,45 @@
     /* "fast_edges_extraction/_extract_edges.pyx":42
  * 
  *         edges[3 * i + 2, 0] = triangles[i, 1]
  *         edges[3 * i + 2, 1] = triangles[i, 2]             # <<<<<<<<<<<<<<
  * 
  *     # Sort edges by lexicographic sort
  */
-    __pyx_t_12 = __pyx_v_i;
-    __pyx_t_11 = 2;
+    __pyx_t_11 = __pyx_v_i;
+    __pyx_t_12 = 2;
     __pyx_t_13 = -1;
-    if (__pyx_t_12 < 0) {
-      __pyx_t_12 += __pyx_v_triangles.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
-    } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles.shape[0])) __pyx_t_13 = 0;
     if (__pyx_t_11 < 0) {
-      __pyx_t_11 += __pyx_v_triangles.shape[1];
-      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 1;
-    } else if (unlikely(__pyx_t_11 >= __pyx_v_triangles.shape[1])) __pyx_t_13 = 1;
+      __pyx_t_11 += __pyx_v_triangles.shape[0];
+      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_11 >= __pyx_v_triangles.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_12 < 0) {
+      __pyx_t_12 += __pyx_v_triangles.shape[1];
+      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles.shape[1])) __pyx_t_13 = 1;
     if (unlikely(__pyx_t_13 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 42, __pyx_L1_error)
     }
-    __pyx_t_15 = ((3 * __pyx_v_i) + 2);
-    __pyx_t_14 = 1;
+    __pyx_t_14 = ((3 * __pyx_v_i) + 2);
+    __pyx_t_15 = 1;
     __pyx_t_13 = -1;
-    if (__pyx_t_15 < 0) {
-      __pyx_t_15 += __pyx_v_edges.shape[0];
-      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 0;
-    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
     if (__pyx_t_14 < 0) {
-      __pyx_t_14 += __pyx_v_edges.shape[1];
-      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 1;
-    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
+      __pyx_t_14 += __pyx_v_edges.shape[0];
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_edges.shape[1];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
     if (unlikely(__pyx_t_13 != -1)) {
       __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 42, __pyx_L1_error)
     }
-    *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_15 * __pyx_v_edges.strides[0]) ) + __pyx_t_14 * __pyx_v_edges.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_triangles.data + __pyx_t_12 * __pyx_v_triangles.strides[0]) ) + __pyx_t_11 * __pyx_v_triangles.strides[1]) )));
+    *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_14 * __pyx_v_edges.strides[0]) ) + __pyx_t_15 * __pyx_v_edges.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_triangles.data + __pyx_t_11 * __pyx_v_triangles.strides[0]) ) + __pyx_t_12 * __pyx_v_triangles.strides[1]) )));
   }
 
   /* "fast_edges_extraction/_extract_edges.pyx":45
  * 
  *     # Sort edges by lexicographic sort
  *     edges = np.sort(np.asarray(edges), axis=1)             # <<<<<<<<<<<<<<
  *     cdef INT_DTYPE_t[:] order = np.lexsort((np.asarray(edges[:, 1]), np.asarray(edges[:, 0])))
@@ -19964,30 +19993,30 @@
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_edges, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_16 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_16)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_16);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
-      __pyx_t_8 = 1;
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_16, __pyx_t_3};
-    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
     __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 45, __pyx_L1_error)
@@ -20049,30 +20078,30 @@
 }
 
 __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_t_7, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __PYX_XCLEAR_MEMVIEW(&__pyx_t_7, 1);
   __pyx_t_7.memview = NULL; __pyx_t_7.data = NULL;
   __pyx_t_17 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_16))) {
     __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_16);
     if (likely(__pyx_t_17)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_16);
       __Pyx_INCREF(__pyx_t_17);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_16, function);
-      __pyx_t_8 = 1;
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_17, __pyx_t_4};
-    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_16, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_16, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
     __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   }
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
@@ -20102,30 +20131,30 @@
 }
 
 __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_t_7, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __PYX_XCLEAR_MEMVIEW(&__pyx_t_7, 1);
   __pyx_t_7.memview = NULL; __pyx_t_7.data = NULL;
   __pyx_t_18 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_17))) {
     __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_17);
     if (likely(__pyx_t_18)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_17);
       __Pyx_INCREF(__pyx_t_18);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_17, function);
-      __pyx_t_8 = 1;
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_18, __pyx_t_4};
-    __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_17, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+    __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_17, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
     __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
   }
   __pyx_t_17 = PyTuple_New(2); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 46, __pyx_L1_error)
@@ -20133,30 +20162,30 @@
   __Pyx_GIVEREF(__pyx_t_2);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_16);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_16)) __PYX_ERR(0, 46, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_16 = 0;
   __pyx_t_16 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_16)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_16);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
-      __pyx_t_8 = 1;
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_16, __pyx_t_17};
-    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
     __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 46, __pyx_L1_error)
@@ -20173,15 +20202,15 @@
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_long((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_npy_int64((3 * __pyx_v_n_triangles)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_17 = PyTuple_New(2); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_GIVEREF(__pyx_t_3);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
@@ -20210,167 +20239,160 @@
   __pyx_t_6.data = NULL;
 
   /* "fast_edges_extraction/_extract_edges.pyx":50
  *     #Remove duplicates
  *     cdef INT_DTYPE_t[:, :] short_edges = np.zeros((3 * n_triangles, 2), dtype=INT_DTYPE)
  *     cdef INT_DTYPE_t n_keep = 1             # <<<<<<<<<<<<<<
  * 
- *     cdef INT_DTYPE_t[:] triangles_ref = np.repeat(np.arange(n_triangles), repeats=3)
+ *     cdef INT_DTYPE_t[:] triangles_ref = np.repeat(np.arange(n_triangles, dtype=INT_DTYPE), repeats=3)
  */
   __pyx_v_n_keep = 1;
 
   /* "fast_edges_extraction/_extract_edges.pyx":52
  *     cdef INT_DTYPE_t n_keep = 1
  * 
- *     cdef INT_DTYPE_t[:] triangles_ref = np.repeat(np.arange(n_triangles), repeats=3)             # <<<<<<<<<<<<<<
+ *     cdef INT_DTYPE_t[:] triangles_ref = np.repeat(np.arange(n_triangles, dtype=INT_DTYPE), repeats=3)             # <<<<<<<<<<<<<<
  *     cdef INT_DTYPE_t[:] indice_ref = np.tile(np.array([2, 1, 0], dtype=INT_DTYPE), reps=n_triangles)
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_repeat); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_arange); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_triangles); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = NULL;
-  __pyx_t_8 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-      __pyx_t_8 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_3};
-    __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_16);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
+  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+  __pyx_t_16 = __Pyx_PyInt_From_npy_int64(__pyx_v_n_triangles); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
   __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_16);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_16)) __PYX_ERR(0, 52, __pyx_L1_error);
   __pyx_t_16 = 0;
   __pyx_t_16 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  if (PyDict_SetItem(__pyx_t_16, __pyx_n_s_repeats, __pyx_int_3) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_17, __pyx_t_5, __pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_INT_DTYPE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_16, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_16 = PyTuple_New(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_repeats, __pyx_int_3) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_17, __pyx_t_16, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_triangles_ref = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
   /* "fast_edges_extraction/_extract_edges.pyx":53
  * 
- *     cdef INT_DTYPE_t[:] triangles_ref = np.repeat(np.arange(n_triangles), repeats=3)
+ *     cdef INT_DTYPE_t[:] triangles_ref = np.repeat(np.arange(n_triangles, dtype=INT_DTYPE), repeats=3)
  *     cdef INT_DTYPE_t[:] indice_ref = np.tile(np.array([2, 1, 0], dtype=INT_DTYPE), reps=n_triangles)             # <<<<<<<<<<<<<<
  * 
  *     short_edges[0, :] = edges[order[0]]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_tile); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_tile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_int_2)) __PYX_ERR(0, 53, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_int_2)) __PYX_ERR(0, 53, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_int_1)) __PYX_ERR(0, 53, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_int_1)) __PYX_ERR(0, 53, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_int_0)) __PYX_ERR(0, 53, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 2, __pyx_int_0)) __PYX_ERR(0, 53, __pyx_L1_error);
   __pyx_t_17 = PyTuple_New(1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_INT_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_t_17, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_INT_DTYPE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_17, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_17 = __Pyx_PyInt_From_int(__pyx_v_n_triangles); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyInt_From_npy_int64(__pyx_v_n_triangles); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_reps, __pyx_t_17) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_reps, __pyx_t_17) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-  __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
-  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t(__pyx_t_17, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
   __pyx_v_indice_ref = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
   /* "fast_edges_extraction/_extract_edges.pyx":55
  *     cdef INT_DTYPE_t[:] indice_ref = np.tile(np.array([2, 1, 0], dtype=INT_DTYPE), reps=n_triangles)
  * 
  *     short_edges[0, :] = edges[order[0]]             # <<<<<<<<<<<<<<
  *     adjacent_triangles[0, 0] = triangles_ref[order[0]]
  *     adjacent_points[0, 0] = indice_ref[order[0]]
  */
-  __pyx_t_11 = 0;
-  __pyx_t_8 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_v_order.shape[0];
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_8 = 0;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+  __pyx_t_12 = 0;
+  __pyx_t_13 = -1;
+  if (__pyx_t_12 < 0) {
+    __pyx_t_12 += __pyx_v_order.shape[0];
+    if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_12 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 55, __pyx_L1_error)
   }
   __pyx_t_7.data = __pyx_v_edges.data;
   __pyx_t_7.memview = __pyx_v_edges.memview;
   __PYX_INC_MEMVIEW(&__pyx_t_7, 1);
   {
-    Py_ssize_t __pyx_tmp_idx = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
+    Py_ssize_t __pyx_tmp_idx = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_12 * __pyx_v_order.strides[0]) )));
         Py_ssize_t __pyx_tmp_shape = __pyx_v_edges.shape[0];
     Py_ssize_t __pyx_tmp_stride = __pyx_v_edges.strides[0];
         if (__pyx_tmp_idx < 0)
             __pyx_tmp_idx += __pyx_tmp_shape;
         if (unlikely(!__Pyx_is_valid_index(__pyx_tmp_idx, __pyx_tmp_shape))) {
             PyErr_SetString(PyExc_IndexError,
                             "Index out of bounds (axis 0)");
@@ -20413,259 +20435,259 @@
   /* "fast_edges_extraction/_extract_edges.pyx":56
  * 
  *     short_edges[0, :] = edges[order[0]]
  *     adjacent_triangles[0, 0] = triangles_ref[order[0]]             # <<<<<<<<<<<<<<
  *     adjacent_points[0, 0] = indice_ref[order[0]]
  *     edge_degrees[0] = 1
  */
-  __pyx_t_11 = 0;
-  __pyx_t_8 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_v_order.shape[0];
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_8 = 0;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+  __pyx_t_12 = 0;
+  __pyx_t_13 = -1;
+  if (__pyx_t_12 < 0) {
+    __pyx_t_12 += __pyx_v_order.shape[0];
+    if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_12 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 56, __pyx_L1_error)
   }
-  __pyx_t_12 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
-  __pyx_t_8 = -1;
-  if (__pyx_t_12 < 0) {
-    __pyx_t_12 += __pyx_v_triangles_ref.shape[0];
-    if (unlikely(__pyx_t_12 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles_ref.shape[0])) __pyx_t_8 = 0;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+  __pyx_t_8 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_12 * __pyx_v_order.strides[0]) )));
+  __pyx_t_13 = -1;
+  if (__pyx_t_8 < 0) {
+    __pyx_t_8 += __pyx_v_triangles_ref.shape[0];
+    if (unlikely(__pyx_t_8 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_8 >= __pyx_v_triangles_ref.shape[0])) __pyx_t_13 = 0;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 56, __pyx_L1_error)
   }
-  __pyx_t_14 = 0;
   __pyx_t_15 = 0;
-  __pyx_t_8 = -1;
-  if (__pyx_t_14 < 0) {
-    __pyx_t_14 += __pyx_v_adjacent_triangles.shape[0];
-    if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_14 >= __pyx_v_adjacent_triangles.shape[0])) __pyx_t_8 = 0;
+  __pyx_t_20 = 0;
+  __pyx_t_13 = -1;
   if (__pyx_t_15 < 0) {
-    __pyx_t_15 += __pyx_v_adjacent_triangles.shape[1];
-    if (unlikely(__pyx_t_15 < 0)) __pyx_t_8 = 1;
-  } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_triangles.shape[1])) __pyx_t_8 = 1;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+    __pyx_t_15 += __pyx_v_adjacent_triangles.shape[0];
+    if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_triangles.shape[0])) __pyx_t_13 = 0;
+  if (__pyx_t_20 < 0) {
+    __pyx_t_20 += __pyx_v_adjacent_triangles.shape[1];
+    if (unlikely(__pyx_t_20 < 0)) __pyx_t_13 = 1;
+  } else if (unlikely(__pyx_t_20 >= __pyx_v_adjacent_triangles.shape[1])) __pyx_t_13 = 1;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 56, __pyx_L1_error)
   }
-  *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_triangles.data + __pyx_t_14 * __pyx_v_adjacent_triangles.strides[0]) ) + __pyx_t_15 * __pyx_v_adjacent_triangles.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_triangles_ref.data + __pyx_t_12 * __pyx_v_triangles_ref.strides[0]) )));
+  *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_triangles.data + __pyx_t_15 * __pyx_v_adjacent_triangles.strides[0]) ) + __pyx_t_20 * __pyx_v_adjacent_triangles.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_triangles_ref.data + __pyx_t_8 * __pyx_v_triangles_ref.strides[0]) )));
 
   /* "fast_edges_extraction/_extract_edges.pyx":57
  *     short_edges[0, :] = edges[order[0]]
  *     adjacent_triangles[0, 0] = triangles_ref[order[0]]
  *     adjacent_points[0, 0] = indice_ref[order[0]]             # <<<<<<<<<<<<<<
  *     edge_degrees[0] = 1
  * 
  */
-  __pyx_t_11 = 0;
-  __pyx_t_8 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_v_order.shape[0];
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_8 = 0;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+  __pyx_t_12 = 0;
+  __pyx_t_13 = -1;
+  if (__pyx_t_12 < 0) {
+    __pyx_t_12 += __pyx_v_order.shape[0];
+    if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_12 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 57, __pyx_L1_error)
   }
-  __pyx_t_12 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
-  __pyx_t_8 = -1;
-  if (__pyx_t_12 < 0) {
-    __pyx_t_12 += __pyx_v_indice_ref.shape[0];
-    if (unlikely(__pyx_t_12 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_12 >= __pyx_v_indice_ref.shape[0])) __pyx_t_8 = 0;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+  __pyx_t_8 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_12 * __pyx_v_order.strides[0]) )));
+  __pyx_t_13 = -1;
+  if (__pyx_t_8 < 0) {
+    __pyx_t_8 += __pyx_v_indice_ref.shape[0];
+    if (unlikely(__pyx_t_8 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_8 >= __pyx_v_indice_ref.shape[0])) __pyx_t_13 = 0;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 57, __pyx_L1_error)
   }
+  __pyx_t_20 = 0;
   __pyx_t_15 = 0;
-  __pyx_t_14 = 0;
-  __pyx_t_8 = -1;
+  __pyx_t_13 = -1;
+  if (__pyx_t_20 < 0) {
+    __pyx_t_20 += __pyx_v_adjacent_points.shape[0];
+    if (unlikely(__pyx_t_20 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_20 >= __pyx_v_adjacent_points.shape[0])) __pyx_t_13 = 0;
   if (__pyx_t_15 < 0) {
-    __pyx_t_15 += __pyx_v_adjacent_points.shape[0];
-    if (unlikely(__pyx_t_15 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_points.shape[0])) __pyx_t_8 = 0;
-  if (__pyx_t_14 < 0) {
-    __pyx_t_14 += __pyx_v_adjacent_points.shape[1];
-    if (unlikely(__pyx_t_14 < 0)) __pyx_t_8 = 1;
-  } else if (unlikely(__pyx_t_14 >= __pyx_v_adjacent_points.shape[1])) __pyx_t_8 = 1;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+    __pyx_t_15 += __pyx_v_adjacent_points.shape[1];
+    if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 1;
+  } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_points.shape[1])) __pyx_t_13 = 1;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 57, __pyx_L1_error)
   }
-  *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_points.data + __pyx_t_15 * __pyx_v_adjacent_points.strides[0]) ) + __pyx_t_14 * __pyx_v_adjacent_points.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_indice_ref.data + __pyx_t_12 * __pyx_v_indice_ref.strides[0]) )));
+  *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_points.data + __pyx_t_20 * __pyx_v_adjacent_points.strides[0]) ) + __pyx_t_15 * __pyx_v_adjacent_points.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_indice_ref.data + __pyx_t_8 * __pyx_v_indice_ref.strides[0]) )));
 
   /* "fast_edges_extraction/_extract_edges.pyx":58
  *     adjacent_triangles[0, 0] = triangles_ref[order[0]]
  *     adjacent_points[0, 0] = indice_ref[order[0]]
  *     edge_degrees[0] = 1             # <<<<<<<<<<<<<<
  * 
  *     for i in range(1, 3 * n_triangles):
  */
-  __pyx_t_11 = 0;
-  __pyx_t_8 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_v_edge_degrees.shape[0];
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_8 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_v_edge_degrees.shape[0])) __pyx_t_8 = 0;
-  if (unlikely(__pyx_t_8 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_8);
+  __pyx_t_12 = 0;
+  __pyx_t_13 = -1;
+  if (__pyx_t_12 < 0) {
+    __pyx_t_12 += __pyx_v_edge_degrees.shape[0];
+    if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 0;
+  } else if (unlikely(__pyx_t_12 >= __pyx_v_edge_degrees.shape[0])) __pyx_t_13 = 0;
+  if (unlikely(__pyx_t_13 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_13);
     __PYX_ERR(0, 58, __pyx_L1_error)
   }
-  *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_edge_degrees.data + __pyx_t_11 * __pyx_v_edge_degrees.strides[0]) )) = 1;
+  *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_edge_degrees.data + __pyx_t_12 * __pyx_v_edge_degrees.strides[0]) )) = 1;
 
   /* "fast_edges_extraction/_extract_edges.pyx":60
  *     edge_degrees[0] = 1
  * 
  *     for i in range(1, 3 * n_triangles):             # <<<<<<<<<<<<<<
  *         if (edges[order[i], 0] != edges[order[i - 1], 0]) or (edges[order[i], 1] != edges[order[i - 1], 1]):
  *             short_edges[n_keep, :] = edges[order[i], :]
  */
-  __pyx_t_20 = (3 * __pyx_v_n_triangles);
-  __pyx_t_21 = __pyx_t_20;
-  for (__pyx_t_8 = 1; __pyx_t_8 < __pyx_t_21; __pyx_t_8+=1) {
-    __pyx_v_i = __pyx_t_8;
+  __pyx_t_8 = (3 * __pyx_v_n_triangles);
+  __pyx_t_9 = __pyx_t_8;
+  for (__pyx_t_10 = 1; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
+    __pyx_v_i = __pyx_t_10;
 
     /* "fast_edges_extraction/_extract_edges.pyx":61
  * 
  *     for i in range(1, 3 * n_triangles):
  *         if (edges[order[i], 0] != edges[order[i - 1], 0]) or (edges[order[i], 1] != edges[order[i - 1], 1]):             # <<<<<<<<<<<<<<
  *             short_edges[n_keep, :] = edges[order[i], :]
  *             adjacent_triangles[n_keep, 0] = triangles_ref[order[i]]
  */
     __pyx_t_11 = __pyx_v_i;
-    __pyx_t_9 = -1;
+    __pyx_t_13 = -1;
     if (__pyx_t_11 < 0) {
       __pyx_t_11 += __pyx_v_order.shape[0];
-      if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
-    __pyx_t_12 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
-    __pyx_t_14 = 0;
-    __pyx_t_9 = -1;
-    if (__pyx_t_12 < 0) {
-      __pyx_t_12 += __pyx_v_edges.shape[0];
-      if (unlikely(__pyx_t_12 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_12 >= __pyx_v_edges.shape[0])) __pyx_t_9 = 0;
+    __pyx_t_14 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
+    __pyx_t_12 = 0;
+    __pyx_t_13 = -1;
     if (__pyx_t_14 < 0) {
-      __pyx_t_14 += __pyx_v_edges.shape[1];
-      if (unlikely(__pyx_t_14 < 0)) __pyx_t_9 = 1;
-    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[1])) __pyx_t_9 = 1;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_14 += __pyx_v_edges.shape[0];
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_12 < 0) {
+      __pyx_t_12 += __pyx_v_edges.shape[1];
+      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_12 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
-    __pyx_t_15 = (__pyx_v_i - 1);
-    __pyx_t_9 = -1;
-    if (__pyx_t_15 < 0) {
-      __pyx_t_15 += __pyx_v_order.shape[0];
-      if (unlikely(__pyx_t_15 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_15 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+    __pyx_t_21 = (__pyx_v_i - 1);
+    __pyx_t_13 = -1;
+    if (__pyx_t_21 < 0) {
+      __pyx_t_21 += __pyx_v_order.shape[0];
+      if (unlikely(__pyx_t_21 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_21 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
-    __pyx_t_22 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_15 * __pyx_v_order.strides[0]) )));
-    __pyx_t_23 = 0;
-    __pyx_t_9 = -1;
+    __pyx_t_22 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_21 * __pyx_v_order.strides[0]) )));
+    __pyx_t_15 = 0;
+    __pyx_t_13 = -1;
     if (__pyx_t_22 < 0) {
       __pyx_t_22 += __pyx_v_edges.shape[0];
-      if (unlikely(__pyx_t_22 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_22 >= __pyx_v_edges.shape[0])) __pyx_t_9 = 0;
-    if (__pyx_t_23 < 0) {
-      __pyx_t_23 += __pyx_v_edges.shape[1];
-      if (unlikely(__pyx_t_23 < 0)) __pyx_t_9 = 1;
-    } else if (unlikely(__pyx_t_23 >= __pyx_v_edges.shape[1])) __pyx_t_9 = 1;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      if (unlikely(__pyx_t_22 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_22 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_edges.shape[1];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
-    __pyx_t_24 = ((*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_12 * __pyx_v_edges.strides[0]) ) + __pyx_t_14 * __pyx_v_edges.strides[1]) ))) != (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_22 * __pyx_v_edges.strides[0]) ) + __pyx_t_23 * __pyx_v_edges.strides[1]) ))));
-    if (!__pyx_t_24) {
+    __pyx_t_23 = ((*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_14 * __pyx_v_edges.strides[0]) ) + __pyx_t_12 * __pyx_v_edges.strides[1]) ))) != (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_22 * __pyx_v_edges.strides[0]) ) + __pyx_t_15 * __pyx_v_edges.strides[1]) ))));
+    if (!__pyx_t_23) {
     } else {
-      __pyx_t_1 = __pyx_t_24;
+      __pyx_t_1 = __pyx_t_23;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_15 = __pyx_v_i;
-    __pyx_t_9 = -1;
-    if (__pyx_t_15 < 0) {
-      __pyx_t_15 += __pyx_v_order.shape[0];
-      if (unlikely(__pyx_t_15 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_15 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+    __pyx_t_21 = __pyx_v_i;
+    __pyx_t_13 = -1;
+    if (__pyx_t_21 < 0) {
+      __pyx_t_21 += __pyx_v_order.shape[0];
+      if (unlikely(__pyx_t_21 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_21 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
-    __pyx_t_23 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_15 * __pyx_v_order.strides[0]) )));
-    __pyx_t_22 = 1;
-    __pyx_t_9 = -1;
-    if (__pyx_t_23 < 0) {
-      __pyx_t_23 += __pyx_v_edges.shape[0];
-      if (unlikely(__pyx_t_23 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_23 >= __pyx_v_edges.shape[0])) __pyx_t_9 = 0;
+    __pyx_t_22 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_21 * __pyx_v_order.strides[0]) )));
+    __pyx_t_15 = 1;
+    __pyx_t_13 = -1;
     if (__pyx_t_22 < 0) {
-      __pyx_t_22 += __pyx_v_edges.shape[1];
-      if (unlikely(__pyx_t_22 < 0)) __pyx_t_9 = 1;
-    } else if (unlikely(__pyx_t_22 >= __pyx_v_edges.shape[1])) __pyx_t_9 = 1;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_22 += __pyx_v_edges.shape[0];
+      if (unlikely(__pyx_t_22 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_22 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_edges.shape[1];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
     __pyx_t_11 = (__pyx_v_i - 1);
-    __pyx_t_9 = -1;
+    __pyx_t_13 = -1;
     if (__pyx_t_11 < 0) {
       __pyx_t_11 += __pyx_v_order.shape[0];
-      if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
     __pyx_t_14 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
     __pyx_t_12 = 1;
-    __pyx_t_9 = -1;
+    __pyx_t_13 = -1;
     if (__pyx_t_14 < 0) {
       __pyx_t_14 += __pyx_v_edges.shape[0];
-      if (unlikely(__pyx_t_14 < 0)) __pyx_t_9 = 0;
-    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[0])) __pyx_t_9 = 0;
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_v_edges.shape[0])) __pyx_t_13 = 0;
     if (__pyx_t_12 < 0) {
       __pyx_t_12 += __pyx_v_edges.shape[1];
-      if (unlikely(__pyx_t_12 < 0)) __pyx_t_9 = 1;
-    } else if (unlikely(__pyx_t_12 >= __pyx_v_edges.shape[1])) __pyx_t_9 = 1;
-    if (unlikely(__pyx_t_9 != -1)) {
-      __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+    } else if (unlikely(__pyx_t_12 >= __pyx_v_edges.shape[1])) __pyx_t_13 = 1;
+    if (unlikely(__pyx_t_13 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_13);
       __PYX_ERR(0, 61, __pyx_L1_error)
     }
-    __pyx_t_24 = ((*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_23 * __pyx_v_edges.strides[0]) ) + __pyx_t_22 * __pyx_v_edges.strides[1]) ))) != (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_14 * __pyx_v_edges.strides[0]) ) + __pyx_t_12 * __pyx_v_edges.strides[1]) ))));
-    __pyx_t_1 = __pyx_t_24;
+    __pyx_t_23 = ((*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_22 * __pyx_v_edges.strides[0]) ) + __pyx_t_15 * __pyx_v_edges.strides[1]) ))) != (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_edges.data + __pyx_t_14 * __pyx_v_edges.strides[0]) ) + __pyx_t_12 * __pyx_v_edges.strides[1]) ))));
+    __pyx_t_1 = __pyx_t_23;
     __pyx_L8_bool_binop_done:;
     if (__pyx_t_1) {
 
       /* "fast_edges_extraction/_extract_edges.pyx":62
  *     for i in range(1, 3 * n_triangles):
  *         if (edges[order[i], 0] != edges[order[i - 1], 0]) or (edges[order[i], 1] != edges[order[i - 1], 1]):
  *             short_edges[n_keep, :] = edges[order[i], :]             # <<<<<<<<<<<<<<
  *             adjacent_triangles[n_keep, 0] = triangles_ref[order[i]]
  *             adjacent_points[n_keep, 0] = indice_ref[order[i]]
  */
       __pyx_t_11 = __pyx_v_i;
-      __pyx_t_9 = -1;
+      __pyx_t_13 = -1;
       if (__pyx_t_11 < 0) {
         __pyx_t_11 += __pyx_v_order.shape[0];
-        if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+        if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 62, __pyx_L1_error)
       }
       __pyx_t_7.data = __pyx_v_edges.data;
       __pyx_t_7.memview = __pyx_v_edges.memview;
       __PYX_INC_MEMVIEW(&__pyx_t_7, 1);
       {
     Py_ssize_t __pyx_tmp_idx = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
@@ -20716,109 +20738,109 @@
  *         if (edges[order[i], 0] != edges[order[i - 1], 0]) or (edges[order[i], 1] != edges[order[i - 1], 1]):
  *             short_edges[n_keep, :] = edges[order[i], :]
  *             adjacent_triangles[n_keep, 0] = triangles_ref[order[i]]             # <<<<<<<<<<<<<<
  *             adjacent_points[n_keep, 0] = indice_ref[order[i]]
  *             edge_degrees[n_keep] = 1
  */
       __pyx_t_11 = __pyx_v_i;
-      __pyx_t_9 = -1;
+      __pyx_t_13 = -1;
       if (__pyx_t_11 < 0) {
         __pyx_t_11 += __pyx_v_order.shape[0];
-        if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+        if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 63, __pyx_L1_error)
       }
-      __pyx_t_12 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
-      __pyx_t_9 = -1;
-      if (__pyx_t_12 < 0) {
-        __pyx_t_12 += __pyx_v_triangles_ref.shape[0];
-        if (unlikely(__pyx_t_12 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles_ref.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_14 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
+      __pyx_t_13 = -1;
+      if (__pyx_t_14 < 0) {
+        __pyx_t_14 += __pyx_v_triangles_ref.shape[0];
+        if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_14 >= __pyx_v_triangles_ref.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 63, __pyx_L1_error)
       }
-      __pyx_t_14 = __pyx_v_n_keep;
-      __pyx_t_15 = 0;
-      __pyx_t_9 = -1;
-      if (__pyx_t_14 < 0) {
-        __pyx_t_14 += __pyx_v_adjacent_triangles.shape[0];
-        if (unlikely(__pyx_t_14 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_14 >= __pyx_v_adjacent_triangles.shape[0])) __pyx_t_9 = 0;
-      if (__pyx_t_15 < 0) {
-        __pyx_t_15 += __pyx_v_adjacent_triangles.shape[1];
-        if (unlikely(__pyx_t_15 < 0)) __pyx_t_9 = 1;
-      } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_triangles.shape[1])) __pyx_t_9 = 1;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_21 = __pyx_v_n_keep;
+      __pyx_t_12 = 0;
+      __pyx_t_13 = -1;
+      if (__pyx_t_21 < 0) {
+        __pyx_t_21 += __pyx_v_adjacent_triangles.shape[0];
+        if (unlikely(__pyx_t_21 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_21 >= __pyx_v_adjacent_triangles.shape[0])) __pyx_t_13 = 0;
+      if (__pyx_t_12 < 0) {
+        __pyx_t_12 += __pyx_v_adjacent_triangles.shape[1];
+        if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+      } else if (unlikely(__pyx_t_12 >= __pyx_v_adjacent_triangles.shape[1])) __pyx_t_13 = 1;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 63, __pyx_L1_error)
       }
-      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_triangles.data + __pyx_t_14 * __pyx_v_adjacent_triangles.strides[0]) ) + __pyx_t_15 * __pyx_v_adjacent_triangles.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_triangles_ref.data + __pyx_t_12 * __pyx_v_triangles_ref.strides[0]) )));
+      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_triangles.data + __pyx_t_21 * __pyx_v_adjacent_triangles.strides[0]) ) + __pyx_t_12 * __pyx_v_adjacent_triangles.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_triangles_ref.data + __pyx_t_14 * __pyx_v_triangles_ref.strides[0]) )));
 
       /* "fast_edges_extraction/_extract_edges.pyx":64
  *             short_edges[n_keep, :] = edges[order[i], :]
  *             adjacent_triangles[n_keep, 0] = triangles_ref[order[i]]
  *             adjacent_points[n_keep, 0] = indice_ref[order[i]]             # <<<<<<<<<<<<<<
  *             edge_degrees[n_keep] = 1
  *             n_keep += 1
  */
       __pyx_t_11 = __pyx_v_i;
-      __pyx_t_9 = -1;
+      __pyx_t_13 = -1;
       if (__pyx_t_11 < 0) {
         __pyx_t_11 += __pyx_v_order.shape[0];
-        if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+        if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 64, __pyx_L1_error)
       }
-      __pyx_t_12 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
-      __pyx_t_9 = -1;
-      if (__pyx_t_12 < 0) {
-        __pyx_t_12 += __pyx_v_indice_ref.shape[0];
-        if (unlikely(__pyx_t_12 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_12 >= __pyx_v_indice_ref.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_14 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
+      __pyx_t_13 = -1;
+      if (__pyx_t_14 < 0) {
+        __pyx_t_14 += __pyx_v_indice_ref.shape[0];
+        if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_14 >= __pyx_v_indice_ref.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 64, __pyx_L1_error)
       }
-      __pyx_t_15 = __pyx_v_n_keep;
-      __pyx_t_14 = 0;
-      __pyx_t_9 = -1;
-      if (__pyx_t_15 < 0) {
-        __pyx_t_15 += __pyx_v_adjacent_points.shape[0];
-        if (unlikely(__pyx_t_15 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_points.shape[0])) __pyx_t_9 = 0;
-      if (__pyx_t_14 < 0) {
-        __pyx_t_14 += __pyx_v_adjacent_points.shape[1];
-        if (unlikely(__pyx_t_14 < 0)) __pyx_t_9 = 1;
-      } else if (unlikely(__pyx_t_14 >= __pyx_v_adjacent_points.shape[1])) __pyx_t_9 = 1;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_21 = __pyx_v_n_keep;
+      __pyx_t_12 = 0;
+      __pyx_t_13 = -1;
+      if (__pyx_t_21 < 0) {
+        __pyx_t_21 += __pyx_v_adjacent_points.shape[0];
+        if (unlikely(__pyx_t_21 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_21 >= __pyx_v_adjacent_points.shape[0])) __pyx_t_13 = 0;
+      if (__pyx_t_12 < 0) {
+        __pyx_t_12 += __pyx_v_adjacent_points.shape[1];
+        if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+      } else if (unlikely(__pyx_t_12 >= __pyx_v_adjacent_points.shape[1])) __pyx_t_13 = 1;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 64, __pyx_L1_error)
       }
-      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_points.data + __pyx_t_15 * __pyx_v_adjacent_points.strides[0]) ) + __pyx_t_14 * __pyx_v_adjacent_points.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_indice_ref.data + __pyx_t_12 * __pyx_v_indice_ref.strides[0]) )));
+      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_points.data + __pyx_t_21 * __pyx_v_adjacent_points.strides[0]) ) + __pyx_t_12 * __pyx_v_adjacent_points.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_indice_ref.data + __pyx_t_14 * __pyx_v_indice_ref.strides[0]) )));
 
       /* "fast_edges_extraction/_extract_edges.pyx":65
  *             adjacent_triangles[n_keep, 0] = triangles_ref[order[i]]
  *             adjacent_points[n_keep, 0] = indice_ref[order[i]]
  *             edge_degrees[n_keep] = 1             # <<<<<<<<<<<<<<
  *             n_keep += 1
  *         else:
  */
       __pyx_t_11 = __pyx_v_n_keep;
-      __pyx_t_9 = -1;
+      __pyx_t_13 = -1;
       if (__pyx_t_11 < 0) {
         __pyx_t_11 += __pyx_v_edge_degrees.shape[0];
-        if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_11 >= __pyx_v_edge_degrees.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+        if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_11 >= __pyx_v_edge_degrees.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 65, __pyx_L1_error)
       }
       *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_edge_degrees.data + __pyx_t_11 * __pyx_v_edge_degrees.strides[0]) )) = 1;
 
       /* "fast_edges_extraction/_extract_edges.pyx":66
  *             adjacent_points[n_keep, 0] = indice_ref[order[i]]
  *             edge_degrees[n_keep] = 1
@@ -20843,109 +20865,109 @@
  *         else:
  *             adjacent_triangles[n_keep - 1, 1] = triangles_ref[order[i]]             # <<<<<<<<<<<<<<
  *             adjacent_points[n_keep - 1, 1] = indice_ref[order[i]]
  *             edge_degrees[n_keep - 1] += 1
  */
     /*else*/ {
       __pyx_t_11 = __pyx_v_i;
-      __pyx_t_9 = -1;
+      __pyx_t_13 = -1;
       if (__pyx_t_11 < 0) {
         __pyx_t_11 += __pyx_v_order.shape[0];
-        if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+        if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 68, __pyx_L1_error)
       }
-      __pyx_t_12 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
-      __pyx_t_9 = -1;
-      if (__pyx_t_12 < 0) {
-        __pyx_t_12 += __pyx_v_triangles_ref.shape[0];
-        if (unlikely(__pyx_t_12 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_12 >= __pyx_v_triangles_ref.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_14 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
+      __pyx_t_13 = -1;
+      if (__pyx_t_14 < 0) {
+        __pyx_t_14 += __pyx_v_triangles_ref.shape[0];
+        if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_14 >= __pyx_v_triangles_ref.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 68, __pyx_L1_error)
       }
-      __pyx_t_14 = (__pyx_v_n_keep - 1);
-      __pyx_t_15 = 1;
-      __pyx_t_9 = -1;
-      if (__pyx_t_14 < 0) {
-        __pyx_t_14 += __pyx_v_adjacent_triangles.shape[0];
-        if (unlikely(__pyx_t_14 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_14 >= __pyx_v_adjacent_triangles.shape[0])) __pyx_t_9 = 0;
-      if (__pyx_t_15 < 0) {
-        __pyx_t_15 += __pyx_v_adjacent_triangles.shape[1];
-        if (unlikely(__pyx_t_15 < 0)) __pyx_t_9 = 1;
-      } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_triangles.shape[1])) __pyx_t_9 = 1;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_21 = (__pyx_v_n_keep - 1);
+      __pyx_t_12 = 1;
+      __pyx_t_13 = -1;
+      if (__pyx_t_21 < 0) {
+        __pyx_t_21 += __pyx_v_adjacent_triangles.shape[0];
+        if (unlikely(__pyx_t_21 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_21 >= __pyx_v_adjacent_triangles.shape[0])) __pyx_t_13 = 0;
+      if (__pyx_t_12 < 0) {
+        __pyx_t_12 += __pyx_v_adjacent_triangles.shape[1];
+        if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+      } else if (unlikely(__pyx_t_12 >= __pyx_v_adjacent_triangles.shape[1])) __pyx_t_13 = 1;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 68, __pyx_L1_error)
       }
-      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_triangles.data + __pyx_t_14 * __pyx_v_adjacent_triangles.strides[0]) ) + __pyx_t_15 * __pyx_v_adjacent_triangles.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_triangles_ref.data + __pyx_t_12 * __pyx_v_triangles_ref.strides[0]) )));
+      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_triangles.data + __pyx_t_21 * __pyx_v_adjacent_triangles.strides[0]) ) + __pyx_t_12 * __pyx_v_adjacent_triangles.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_triangles_ref.data + __pyx_t_14 * __pyx_v_triangles_ref.strides[0]) )));
 
       /* "fast_edges_extraction/_extract_edges.pyx":69
  *         else:
  *             adjacent_triangles[n_keep - 1, 1] = triangles_ref[order[i]]
  *             adjacent_points[n_keep - 1, 1] = indice_ref[order[i]]             # <<<<<<<<<<<<<<
  *             edge_degrees[n_keep - 1] += 1
  * 
  */
       __pyx_t_11 = __pyx_v_i;
-      __pyx_t_9 = -1;
+      __pyx_t_13 = -1;
       if (__pyx_t_11 < 0) {
         __pyx_t_11 += __pyx_v_order.shape[0];
-        if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+        if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_11 >= __pyx_v_order.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 69, __pyx_L1_error)
       }
-      __pyx_t_12 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
-      __pyx_t_9 = -1;
-      if (__pyx_t_12 < 0) {
-        __pyx_t_12 += __pyx_v_indice_ref.shape[0];
-        if (unlikely(__pyx_t_12 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_12 >= __pyx_v_indice_ref.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_14 = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_order.data + __pyx_t_11 * __pyx_v_order.strides[0]) )));
+      __pyx_t_13 = -1;
+      if (__pyx_t_14 < 0) {
+        __pyx_t_14 += __pyx_v_indice_ref.shape[0];
+        if (unlikely(__pyx_t_14 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_14 >= __pyx_v_indice_ref.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 69, __pyx_L1_error)
       }
-      __pyx_t_15 = (__pyx_v_n_keep - 1);
-      __pyx_t_14 = 1;
-      __pyx_t_9 = -1;
-      if (__pyx_t_15 < 0) {
-        __pyx_t_15 += __pyx_v_adjacent_points.shape[0];
-        if (unlikely(__pyx_t_15 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_15 >= __pyx_v_adjacent_points.shape[0])) __pyx_t_9 = 0;
-      if (__pyx_t_14 < 0) {
-        __pyx_t_14 += __pyx_v_adjacent_points.shape[1];
-        if (unlikely(__pyx_t_14 < 0)) __pyx_t_9 = 1;
-      } else if (unlikely(__pyx_t_14 >= __pyx_v_adjacent_points.shape[1])) __pyx_t_9 = 1;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+      __pyx_t_21 = (__pyx_v_n_keep - 1);
+      __pyx_t_12 = 1;
+      __pyx_t_13 = -1;
+      if (__pyx_t_21 < 0) {
+        __pyx_t_21 += __pyx_v_adjacent_points.shape[0];
+        if (unlikely(__pyx_t_21 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_21 >= __pyx_v_adjacent_points.shape[0])) __pyx_t_13 = 0;
+      if (__pyx_t_12 < 0) {
+        __pyx_t_12 += __pyx_v_adjacent_points.shape[1];
+        if (unlikely(__pyx_t_12 < 0)) __pyx_t_13 = 1;
+      } else if (unlikely(__pyx_t_12 >= __pyx_v_adjacent_points.shape[1])) __pyx_t_13 = 1;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 69, __pyx_L1_error)
       }
-      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_points.data + __pyx_t_15 * __pyx_v_adjacent_points.strides[0]) ) + __pyx_t_14 * __pyx_v_adjacent_points.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_indice_ref.data + __pyx_t_12 * __pyx_v_indice_ref.strides[0]) )));
+      *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_adjacent_points.data + __pyx_t_21 * __pyx_v_adjacent_points.strides[0]) ) + __pyx_t_12 * __pyx_v_adjacent_points.strides[1]) )) = (*((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_indice_ref.data + __pyx_t_14 * __pyx_v_indice_ref.strides[0]) )));
 
       /* "fast_edges_extraction/_extract_edges.pyx":70
  *             adjacent_triangles[n_keep - 1, 1] = triangles_ref[order[i]]
  *             adjacent_points[n_keep - 1, 1] = indice_ref[order[i]]
  *             edge_degrees[n_keep - 1] += 1             # <<<<<<<<<<<<<<
  * 
  *     return (
  */
       __pyx_t_11 = (__pyx_v_n_keep - 1);
-      __pyx_t_9 = -1;
+      __pyx_t_13 = -1;
       if (__pyx_t_11 < 0) {
         __pyx_t_11 += __pyx_v_edge_degrees.shape[0];
-        if (unlikely(__pyx_t_11 < 0)) __pyx_t_9 = 0;
-      } else if (unlikely(__pyx_t_11 >= __pyx_v_edge_degrees.shape[0])) __pyx_t_9 = 0;
-      if (unlikely(__pyx_t_9 != -1)) {
-        __Pyx_RaiseBufferIndexError(__pyx_t_9);
+        if (unlikely(__pyx_t_11 < 0)) __pyx_t_13 = 0;
+      } else if (unlikely(__pyx_t_11 >= __pyx_v_edge_degrees.shape[0])) __pyx_t_13 = 0;
+      if (unlikely(__pyx_t_13 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_13);
         __PYX_ERR(0, 70, __pyx_L1_error)
       }
       *((__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) ( /* dim=0 */ (__pyx_v_edge_degrees.data + __pyx_t_11 * __pyx_v_edge_degrees.strides[0]) )) += 1;
     }
     __pyx_L7:;
   }
 
@@ -20961,234 +20983,234 @@
   /* "fast_edges_extraction/_extract_edges.pyx":73
  * 
  *     return (
  *         np.asarray(short_edges)[:n_keep, :],             # <<<<<<<<<<<<<<
  *         np.asarray(edge_degrees)[:n_keep],
  *         np.asarray(adjacent_triangles)[:n_keep, :],
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_short_edges, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_16 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_short_edges, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = NULL;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_16)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_16);
+  if (unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_8 = 1;
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_16, __pyx_t_2};
-    __pyx_t_17 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_3};
+    __pyx_t_17 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_17);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_3 = __Pyx_PyInt_From_npy_long(__pyx_v_n_keep); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PySlice_New(Py_None, __pyx_t_3, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_npy_int64(__pyx_v_n_keep); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = PySlice_New(Py_None, __pyx_t_5, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error);
   __Pyx_INCREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_slice__5)) __PYX_ERR(0, 73, __pyx_L1_error);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_17, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_slice__5)) __PYX_ERR(0, 73, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_17, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "fast_edges_extraction/_extract_edges.pyx":74
  *     return (
  *         np.asarray(short_edges)[:n_keep, :],
  *         np.asarray(edge_degrees)[:n_keep],             # <<<<<<<<<<<<<<
  *         np.asarray(adjacent_triangles)[:n_keep, :],
  *         np.asarray(adjacent_points)[:n_keep, :],
  */
   __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_np); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_asarray); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_16);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
   __pyx_t_17 = __pyx_memoryview_fromslice(__pyx_v_edge_degrees, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
-  __pyx_t_5 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_16 = NULL;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_16))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_16);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_16);
-      __Pyx_INCREF(__pyx_t_5);
+  if (unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_16)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_16);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_16, function);
-      __pyx_t_8 = 1;
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_17};
-    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_16, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    PyObject *__pyx_callargs[2] = {__pyx_t_16, __pyx_t_17};
+    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
+    __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_16 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, __pyx_v_n_keep, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_16);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_5, 0, __pyx_v_n_keep, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "fast_edges_extraction/_extract_edges.pyx":75
  *         np.asarray(short_edges)[:n_keep, :],
  *         np.asarray(edge_degrees)[:n_keep],
  *         np.asarray(adjacent_triangles)[:n_keep, :],             # <<<<<<<<<<<<<<
  *         np.asarray(adjacent_points)[:n_keep, :],
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_17, __pyx_n_s_np); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_17, __pyx_n_s_asarray); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
   __pyx_t_17 = __pyx_memoryview_fromslice(__pyx_v_adjacent_triangles, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __pyx_t_4 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+  if (unlikely(PyMethod_Check(__pyx_t_16))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_16);
     if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_16);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-      __pyx_t_8 = 1;
+      __Pyx_DECREF_SET(__pyx_t_16, function);
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_17};
-    __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_16, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   }
-  __pyx_t_5 = __Pyx_PyInt_From_npy_long(__pyx_v_n_keep); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_17 = PySlice_New(Py_None, __pyx_t_5, Py_None); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyInt_From_npy_int64(__pyx_v_n_keep); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
+  __pyx_t_17 = PySlice_New(Py_None, __pyx_t_16, Py_None); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+  __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_17);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error);
   __Pyx_INCREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_slice__5)) __PYX_ERR(0, 75, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_slice__5)) __PYX_ERR(0, 75, __pyx_L1_error);
   __pyx_t_17 = 0;
-  __pyx_t_17 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_16); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
   /* "fast_edges_extraction/_extract_edges.pyx":76
  *         np.asarray(edge_degrees)[:n_keep],
  *         np.asarray(adjacent_triangles)[:n_keep, :],
  *         np.asarray(adjacent_points)[:n_keep, :],             # <<<<<<<<<<<<<<
  * 
  *     )
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_adjacent_points, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __pyx_memoryview_fromslice(__pyx_v_adjacent_points, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_18 = NULL;
-  __pyx_t_8 = 0;
+  __pyx_t_13 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_18)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_18);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
-      __pyx_t_8 = 1;
+      __pyx_t_13 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_18, __pyx_t_3};
-    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+    PyObject *__pyx_callargs[2] = {__pyx_t_18, __pyx_t_5};
+    __pyx_t_16 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
     __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = __Pyx_PyInt_From_npy_long(__pyx_v_n_keep); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_npy_int64(__pyx_v_n_keep); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = PySlice_New(Py_None, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error);
   __Pyx_INCREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_slice__5)) __PYX_ERR(0, 76, __pyx_L1_error);
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_16, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "fast_edges_extraction/_extract_edges.pyx":73
  * 
  *     return (
  *         np.asarray(short_edges)[:n_keep, :],             # <<<<<<<<<<<<<<
  *         np.asarray(edge_degrees)[:n_keep],
  *         np.asarray(adjacent_triangles)[:n_keep, :],
  */
   __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_16);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_16)) __PYX_ERR(0, 73, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_17);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_17)) __PYX_ERR(0, 73, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error);
+  __pyx_t_3 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_16 = 0;
   __pyx_t_17 = 0;
-  __pyx_t_3 = 0;
+  __pyx_t_5 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
   /* "fast_edges_extraction/_extract_edges.pyx":14
  * 
  * 
@@ -22272,15 +22294,15 @@
     {&__pyx_kp_u_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 1, 0, 0},
     {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
     {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
     {&__pyx_n_s_indice_ref, __pyx_k_indice_ref, sizeof(__pyx_k_indice_ref), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
-    {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+    {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
     {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
     {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
     {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
     {&__pyx_n_s_l, __pyx_k_l, sizeof(__pyx_k_l), 0, 0, 1, 1},
@@ -22404,26 +22426,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-omqlxiv3/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-4pns5o49/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -22778,41 +22800,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -23642,31 +23664,31 @@
   __pyx_t_9 = __pyx_f_5numpy_import_array(); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 7, __pyx_L1_error)
 
   /* "fast_edges_extraction/_extract_edges.pyx":8
  * cimport numpy as cnp
  * cnp.import_array()
  * import numpy as np             # <<<<<<<<<<<<<<
  * 
- * INT_DTYPE = np.int_
+ * INT_DTYPE = np.int64
  */
   __pyx_t_7 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_7) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "fast_edges_extraction/_extract_edges.pyx":10
  * import numpy as np
  * 
- * INT_DTYPE = np.int_             # <<<<<<<<<<<<<<
- * ctypedef cnp.int_t INT_DTYPE_t
+ * INT_DTYPE = np.int64             # <<<<<<<<<<<<<<
+ * ctypedef cnp.int64_t INT_DTYPE_t
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_INT_DTYPE, __pyx_t_4) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "fast_edges_extraction/_extract_edges.pyx":14
  * 
@@ -27047,18 +27069,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -27104,23 +27126,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -29496,19 +29518,19 @@
             }\
         }\
         return (target_type) value;\
     }
 
 /* MemviewDtypeToObject */
   static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t(const char *itemp) {
-    return (PyObject *) __Pyx_PyInt_From_npy_long(*(__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) itemp);
+    return (PyObject *) __Pyx_PyInt_From_npy_int64(*(__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t(const char *itemp, PyObject *obj) {
-    __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t value = __Pyx_PyInt_As_npy_long(obj);
-    if (unlikely((value == ((npy_long)-1)) && PyErr_Occurred()))
+    __pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t value = __Pyx_PyInt_As_npy_int64(obj);
+    if (unlikely((value == ((npy_int64)-1)) && PyErr_Occurred()))
         return 0;
     *(__pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t *) itemp = value;
     return 1;
 }
 
 /* ObjectToMemviewSlice */
   static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_21fast_edges_extraction_14_extract_edges_INT_DTYPE_t(PyObject *obj, int writable_flag) {
@@ -30040,55 +30062,55 @@
     } else {
         __pyx_fatalerror("Acquisition count is %d (line %d)",
                          old_acquisition_count-1, lineno);
     }
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_long(npy_long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_int64(npy_int64 value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const npy_long neg_one = (npy_long) -1, const_zero = (npy_long) 0;
+    const npy_int64 neg_one = (npy_int64) -1, const_zero = (npy_int64) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(npy_long) < sizeof(long)) {
+        if (sizeof(npy_int64) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(npy_long) <= sizeof(unsigned long)) {
+        } else if (sizeof(npy_int64) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(npy_long) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(npy_int64) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(npy_long) <= sizeof(long)) {
+        if (sizeof(npy_int64) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(npy_long) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(npy_int64) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
 #if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(npy_long),
+        return _PyLong_FromByteArray(bytes, sizeof(npy_int64),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
         from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(npy_long));
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(npy_int64));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
         if (!is_unsigned) {
             kwds = PyDict_New();
@@ -30104,173 +30126,173 @@
         Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE npy_long __Pyx_PyInt_As_npy_long(PyObject *x) {
+  static CYTHON_INLINE npy_int64 __Pyx_PyInt_As_npy_int64(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const npy_long neg_one = (npy_long) -1, const_zero = (npy_long) 0;
+    const npy_int64 neg_one = (npy_int64) -1, const_zero = (npy_int64) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(npy_long) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(npy_long, long, PyInt_AS_LONG(x))
+        if ((sizeof(npy_int64) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(npy_int64, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (npy_long) val;
+            return (npy_int64) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (unlikely(__Pyx_PyLong_IsNeg(x))) {
                 goto raise_neg_overflow;
             } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(npy_long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+                __PYX_VERIFY_RETURN_INT(npy_int64, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_DigitCount(x)) {
                     case 2:
-                        if ((8 * sizeof(npy_long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) >= 2 * PyLong_SHIFT)) {
-                                return (npy_long) (((((npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) >= 2 * PyLong_SHIFT)) {
+                                return (npy_int64) (((((npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0]));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(npy_long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) >= 3 * PyLong_SHIFT)) {
-                                return (npy_long) (((((((npy_long)digits[2]) << PyLong_SHIFT) | (npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) >= 3 * PyLong_SHIFT)) {
+                                return (npy_int64) (((((((npy_int64)digits[2]) << PyLong_SHIFT) | (npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0]));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(npy_long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) >= 4 * PyLong_SHIFT)) {
-                                return (npy_long) (((((((((npy_long)digits[3]) << PyLong_SHIFT) | (npy_long)digits[2]) << PyLong_SHIFT) | (npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) >= 4 * PyLong_SHIFT)) {
+                                return (npy_int64) (((((((((npy_int64)digits[3]) << PyLong_SHIFT) | (npy_int64)digits[2]) << PyLong_SHIFT) | (npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0]));
                             }
                         }
                         break;
                 }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (npy_long) -1;
+                    return (npy_int64) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(npy_long) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_long, unsigned long, PyLong_AsUnsignedLong(x))
+            if ((sizeof(npy_int64) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(npy_int64, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(npy_long) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if ((sizeof(npy_int64) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(npy_int64, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(npy_long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+                __PYX_VERIFY_RETURN_INT(npy_int64, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_SignedDigitCount(x)) {
                     case -2:
-                        if ((8 * sizeof(npy_long) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) - 1 > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (npy_long) (((npy_long)-1)*(((((npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) - 1 > 2 * PyLong_SHIFT)) {
+                                return (npy_int64) (((npy_int64)-1)*(((((npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0])));
                             }
                         }
                         break;
                     case 2:
-                        if ((8 * sizeof(npy_long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (npy_long) ((((((npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) - 1 > 2 * PyLong_SHIFT)) {
+                                return (npy_int64) ((((((npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0])));
                             }
                         }
                         break;
                     case -3:
-                        if ((8 * sizeof(npy_long) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) - 1 > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (npy_long) (((npy_long)-1)*(((((((npy_long)digits[2]) << PyLong_SHIFT) | (npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) - 1 > 3 * PyLong_SHIFT)) {
+                                return (npy_int64) (((npy_int64)-1)*(((((((npy_int64)digits[2]) << PyLong_SHIFT) | (npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0])));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(npy_long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (npy_long) ((((((((npy_long)digits[2]) << PyLong_SHIFT) | (npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) - 1 > 3 * PyLong_SHIFT)) {
+                                return (npy_int64) ((((((((npy_int64)digits[2]) << PyLong_SHIFT) | (npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0])));
                             }
                         }
                         break;
                     case -4:
-                        if ((8 * sizeof(npy_long) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) - 1 > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (npy_long) (((npy_long)-1)*(((((((((npy_long)digits[3]) << PyLong_SHIFT) | (npy_long)digits[2]) << PyLong_SHIFT) | (npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) - 1 > 4 * PyLong_SHIFT)) {
+                                return (npy_int64) (((npy_int64)-1)*(((((((((npy_int64)digits[3]) << PyLong_SHIFT) | (npy_int64)digits[2]) << PyLong_SHIFT) | (npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0])));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(npy_long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(npy_int64) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(npy_long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(npy_long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (npy_long) ((((((((((npy_long)digits[3]) << PyLong_SHIFT) | (npy_long)digits[2]) << PyLong_SHIFT) | (npy_long)digits[1]) << PyLong_SHIFT) | (npy_long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(npy_int64, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int64) - 1 > 4 * PyLong_SHIFT)) {
+                                return (npy_int64) ((((((((((npy_int64)digits[3]) << PyLong_SHIFT) | (npy_int64)digits[2]) << PyLong_SHIFT) | (npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0])));
                             }
                         }
                         break;
                 }
             }
 #endif
-            if ((sizeof(npy_long) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_long, long, PyLong_AsLong(x))
+            if ((sizeof(npy_int64) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(npy_int64, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(npy_long) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(npy_long, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if ((sizeof(npy_int64) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(npy_int64, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-            npy_long val;
+            npy_int64 val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
 #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -30289,227 +30311,99 @@
                 long idigit;
                 int chunk_size = (sizeof(long) < 8) ? 30 : 62;
                 if (unlikely(!PyLong_CheckExact(v))) {
                     PyObject *tmp = v;
                     v = PyNumber_Long(v);
                     assert(PyLong_CheckExact(v));
                     Py_DECREF(tmp);
-                    if (unlikely(!v)) return (npy_long) -1;
+                    if (unlikely(!v)) return (npy_int64) -1;
                 }
 #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                 if (Py_SIZE(x) == 0)
-                    return (npy_long) 0;
+                    return (npy_int64) 0;
                 is_negative = Py_SIZE(x) < 0;
 #else
                 {
                     int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                     if (unlikely(result < 0))
-                        return (npy_long) -1;
+                        return (npy_int64) -1;
                     is_negative = result == 1;
                 }
 #endif
                 if (is_unsigned && unlikely(is_negative)) {
                     goto raise_neg_overflow;
                 } else if (is_negative) {
                     stepval = PyNumber_Invert(v);
                     if (unlikely(!stepval))
-                        return (npy_long) -1;
+                        return (npy_int64) -1;
                 } else {
                     stepval = __Pyx_NewRef(v);
                 }
-                val = (npy_long) 0;
+                val = (npy_int64) 0;
                 mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
                 shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(npy_long) * 8 - chunk_size; bits += chunk_size) {
+                for (bits = 0; bits < (int) sizeof(npy_int64) * 8 - chunk_size; bits += chunk_size) {
                     PyObject *tmp, *digit;
                     digit = PyNumber_And(stepval, mask);
                     if (unlikely(!digit)) goto done;
                     idigit = PyLong_AsLong(digit);
                     Py_DECREF(digit);
                     if (unlikely(idigit < 0)) goto done;
                     tmp = PyNumber_Rshift(stepval, shift);
                     if (unlikely(!tmp)) goto done;
                     Py_DECREF(stepval); stepval = tmp;
-                    val |= ((npy_long) idigit) << bits;
+                    val |= ((npy_int64) idigit) << bits;
                     #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                     if (Py_SIZE(stepval) == 0)
                         goto unpacking_done;
                     #endif
                 }
                 idigit = PyLong_AsLong(stepval);
                 if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(npy_long) * 8) - bits - (is_unsigned ? 0 : 1);
+                remaining_bits = ((int) sizeof(npy_int64) * 8) - bits - (is_unsigned ? 0 : 1);
                 if (unlikely(idigit >= (1L << remaining_bits)))
                     goto raise_overflow;
-                val |= ((npy_long) idigit) << bits;
+                val |= ((npy_int64) idigit) << bits;
             #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
             unpacking_done:
             #endif
                 if (!is_unsigned) {
-                    if (unlikely(val & (((npy_long) 1) << (sizeof(npy_long) * 8 - 1))))
+                    if (unlikely(val & (((npy_int64) 1) << (sizeof(npy_int64) * 8 - 1))))
                         goto raise_overflow;
                     if (is_negative)
                         val = ~val;
                 }
                 ret = 0;
             done:
                 Py_XDECREF(shift);
                 Py_XDECREF(mask);
                 Py_XDECREF(stepval);
 #endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-            return (npy_long) -1;
+            return (npy_int64) -1;
         }
     } else {
-        npy_long val;
+        npy_int64 val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (npy_long) -1;
-        val = __Pyx_PyInt_As_npy_long(tmp);
+        if (!tmp) return (npy_int64) -1;
+        val = __Pyx_PyInt_As_npy_int64(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to npy_long");
-    return (npy_long) -1;
+        "value too large to convert to npy_int64");
+    return (npy_int64) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to npy_long");
-    return (npy_long) -1;
-}
-
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
+        "can't convert negative value to npy_int64");
+    return (npy_int64) -1;
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
@@ -31050,14 +30944,142 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
```

### Comparing `fast_edges_extraction-0.1.1/fast_edges_extraction.egg-info/PKG-INFO` & `fast_edges_extraction-0.1.2/fast_edges_extraction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_edges_extraction
-Version: 0.1.1
+Version: 0.1.2
 Summary: Edge extraction for triangle meshes
 Author: Louis Pujol
 License: MIT License
         
         Copyright (c) 2023 Louis Pujol
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,18 @@
 Requires-Dist: numpy
 
 fast-edges-extraction
 =====================
 
 Cython implementation of edges extraction from triangles as well as adjacency information (edge degrees and adjacent points/triangles for manifold and boundary edges).
 
+```bash
+pip install fast-edges-extraction
+```
+
 Example
 -------
 
 ![](example.png)
 
 
 - Extract the edges from the triangles
```

### Comparing `fast_edges_extraction-0.1.1/pyproject.toml` & `fast_edges_extraction-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "fast_edges_extraction"
 description = "Edge extraction for triangle meshes"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">= 3.8"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Louis Pujol" }
 ]
 dependencies = [
     "numpy",
 ]
```

### Comparing `fast_edges_extraction-0.1.1/tests/test_consistency.py` & `fast_edges_extraction-0.1.2/tests/test_consistency.py`

 * *Files identical despite different names*

