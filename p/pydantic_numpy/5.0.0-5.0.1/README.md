# Comparing `tmp/pydantic_numpy-5.0.0.tar.gz` & `tmp/pydantic_numpy-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-5.0.0.tar", max compression
+gzip compressed data, was "pydantic_numpy-5.0.1.tar", max compression
```

## Comparing `pydantic_numpy-5.0.0.tar` & `pydantic_numpy-5.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1658 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/LICENSE
--rw-r--r--   0        0        0     3247 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/README.md
--rw-r--r--   0        0        0      199 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/pydantic_numpy/helper/__init__.py
--rw-r--r--   0        0        0    13321 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/pydantic_numpy/helper/annotation.py
--rw-r--r--   0        0        0      168 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/helper/typing.py
--rw-r--r--   0        0        0     3645 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/helper/validation.py
--rw-r--r--   0        0        0     9736 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/model.py
--rw-r--r--   0        0        0      474 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/__init__.py
--rw-r--r--   0        0        0     4886 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/i_dimensional.py
--rw-r--r--   0        0        0     4981 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/ii_dimensional.py
--rw-r--r--   0        0        0     5076 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/iii_dimensional.py
--rw-r--r--   0        0        0     4810 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/n_dimensional.py
--rw-r--r--   0        0        0        0 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/__init__.py
--rw-r--r--   0        0        0     4086 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py
--rw-r--r--   0        0        0     4176 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
--rw-r--r--   0        0        0     4266 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
--rw-r--r--   0        0        0     4019 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py
--rw-r--r--   0        0        0     1621 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/util.py
--rw-r--r--   0        0        0     1542 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 pydantic_numpy-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1658 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/LICENSE
+-rw-r--r--   0        0        0     4547 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/README.md
+-rw-r--r--   0        0        0      199 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0    13321 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0      168 2024-04-19 06:32:51.120243 pydantic_numpy-5.0.1/pydantic_numpy/helper/typing.py
+-rw-r--r--   0        0        0     3645 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0     9736 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/model.py
+-rw-r--r--   0        0        0      474 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     4886 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     4981 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     5076 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     4810 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/__init__.py
+-rw-r--r--   0        0        0     4086 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py
+-rw-r--r--   0        0        0     4176 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
+-rw-r--r--   0        0        0     4266 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
+-rw-r--r--   0        0        0     4019 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py
+-rw-r--r--   0        0        0     1621 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1542 2024-04-19 06:32:51.124243 pydantic_numpy-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 pydantic_numpy-5.0.1/PKG-INFO
```

### Comparing `pydantic_numpy-5.0.0/LICENSE` & `pydantic_numpy-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/helper/annotation.py` & `pydantic_numpy-5.0.1/pydantic_numpy/helper/annotation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/helper/validation.py` & `pydantic_numpy-5.0.1/pydantic_numpy/helper/validation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/model.py` & `pydantic_numpy-5.0.1/pydantic_numpy/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/i_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/ii_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/iii_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/n_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py` & `pydantic_numpy-5.0.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pydantic_numpy/util.py` & `pydantic_numpy-5.0.1/pydantic_numpy/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-5.0.0/pyproject.toml` & `pydantic_numpy-5.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "5.0.0"
+version = "5.0.1"
 description = "Pydantic Model integration of the NumPy array"
 authors = ["Can H. Tartanoglu", "Christoph Heindl"]
 maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/caniko/pydantic-numpy"
 license = "BSD-4"
```

### Comparing `pydantic_numpy-5.0.0/PKG-INFO` & `pydantic_numpy-5.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_numpy
-Version: 5.0.0
+Version: 5.0.1
 Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
 License: BSD-4
 Keywords: pydantic,numpy,typing,validation
 Author: Can H. Tartanoglu
 Maintainer: Can H. Tartanoglu
 Maintainer-email: python@rotas.mozmail.com
@@ -37,15 +37,15 @@
 ## Usage
 
 Package that integrates NumPy Arrays into Pydantic!
 
 - `pydantic_numpy.typing` provides many typings such as `NpNDArrayFp64`, `Np3DArrayFp64` (float64 that must be 3D)! Works with both `pydantic.BaseModel` and `pydantic.dataclass`
 - `NumpyModel` (derived from `pydantic.BaseModel`) make it possible to dump and load `np.ndarray` within model fields alongside other fields that are not instances of `np.ndarray`!
 
-See the [`test.helper.groups`](https://github.com/caniko/pydantic-numpy/blob/trunk/tests/helper/groups.py) to see types that are defined explicitly. Define your own NumPy types with `pydantic_numpy.np_array_pydantic_annotated_typing`.
+See the [`test.helper.testing_groups`](https://github.com/caniko/pydantic-numpy/blob/trunk/tests/helper/testing_groups.py) to see types that are defined explicitly.
 
 ### Examples
 
 For more examples see [test_ndarray.py](./tests/test_typing.py)
 
 ```python
 import numpy as np
@@ -92,21 +92,50 @@
 ```python
 from pydantic_numpy.model import model_agnostic_load
 
 cfg.dump("path_to_dump_dir", "object_id")
 equals_cfg = model_agnostic_load("path_to_dump_dir", "object_id", models=[MyNumpyModel, MyDemoModel])
 ```
 
+### Custom type
+There are two ways to define. Function derived types with `pydantic_numpy.helper.annotation.np_array_pydantic_annotated_typing`.
+
+Function derived types don't work with static type checkers like Pyright and MyPy. In case you need the support,
+just create the types yourself:
+    
+```python
+NpStrict1DArrayInt64 = Annotated[
+    np.ndarray[tuple[int], np.dtype[np.int64]],
+    NpArrayPydanticAnnotation.factory(data_type=np.int64, dimensions=1, strict_data_typing=True),
+]
+```
+
+#### Custom serialization
+
+If the default serialization of NumpyDataDict, as outlined in [typing.py](https://github.com/caniko/pydantic-numpy/blob/trunk/pydantic_numpy/helper/typing.py), doesn't meet your requirements, you have the option to define a custom type with its own serializer. This can be achieved using the NpArrayPydanticAnnotation.factory method, which accepts a custom serialization function through its serialize_numpy_array_to_json parameter. This parameter expects a function of the form `Callable[[npt.ArrayLike], Iterable]`, allowing you to tailor the serialization process to your specific needs.
+
+Example below illustrates definition of 1d-array of `float32` type that serializes to flat Python list (without nested dict as in default `NumpyDataDict` case):
+
+```python
+def _serialize_numpy_array_to_float_list(array_like: npt.ArrayLike) -> Iterable:
+    return np.array(array_like).astype(float).tolist()
+
+
+Np1DArrayFp32 = Annotated[
+    np.ndarray[tuple[int], np.dtype[np.float32]],
+    NpArrayPydanticAnnotation.factory(
+        data_type=np.float32,
+        dimensions=1,
+        strict_data_typing=False,
+        serialize_numpy_array_to_json=_serialize_numpy_array_to_float_list,
+    ),
+]
+```
+
 ### Install
 ```shell
 pip install pydantic-numpy
 ```
 
-## Considerations
-The package is designed to work with Pydantic V2 and not V1. You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `<=3.8` and Pydantic V1 support.
-
-### Licensing notice
-As of version `3.0.0` the license has moved over to BSD-4. The versions prior are under the MIT license.
-
 ### History
 The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
```

