# Comparing `tmp/linalgebralib-0.0.0.tar.gz` & `tmp/linalgebralib-0.0.1.tar.gz`

## Comparing `linalgebralib-0.0.0.tar` & `linalgebralib-0.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 linalgebralib-0.0.0/src/test.py
--rw-r--r--   0        0        0    27596 2020-02-02 00:00:00.000000 linalgebralib-0.0.0/src/linalgebralib/LinAlgebraLib.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 linalgebralib-0.0.0/src/linalgebralib/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 linalgebralib-0.0.0/LICENSE
--rw-r--r--   0        0        0    13244 2020-02-02 00:00:00.000000 linalgebralib-0.0.0/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 linalgebralib-0.0.0/pyproject.toml
--rw-r--r--   0        0        0    13341 2020-02-02 00:00:00.000000 linalgebralib-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 linalgebralib-0.0.1/src/test.py
+-rw-r--r--   0        0        0    28548 2020-02-02 00:00:00.000000 linalgebralib-0.0.1/src/linalgebralib/LinAlgebraLib.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 linalgebralib-0.0.1/src/linalgebralib/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 linalgebralib-0.0.1/LICENSE
+-rw-r--r--   0        0        0    13513 2020-02-02 00:00:00.000000 linalgebralib-0.0.1/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 linalgebralib-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 linalgebralib-0.0.1/PKG-INFO
```

### Comparing `linalgebralib-0.0.0/src/linalgebralib/LinAlgebraLib.py` & `linalgebralib-0.0.1/src/linalgebralib/LinAlgebraLib.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                     tmp.append([self.contents[i][0]-u.contents[i][0]])
                 return columnVector(contents=tmp)
         elif isinstance(u, columnVector):
             if len(self.contents) != len(u.contents):
                 raise TypeError("Vector subtraction must use vectors of the same dimension!")
             else:
                 tmp = []
-                for i in range(self.contents):
+                for i in range(len(self.contents)):
                     tmp.append(self.contents[i][0]-u.contents[i][0])
                 return columnVector(contents=tmp)
         else:
             raise TypeError("Cannot subtract column vectors with non-vectors or row vectors (Aside from n*1 matricies of the same dimension).")
         
     def __mul__(self, u):
         #Method for scalar multiplication of column vectors, and multiplication by row vectors or matrices of appropriate sizes.
@@ -170,15 +170,15 @@
             if type(u) == Matrix:
                 if (len(u.contents) == 1) and (len(u.contents[0]) == self.size):
                     result = 0
                     for i in range(len(u.contents[0])):
                         result += self.contents[i][0]*u.contents[0][i]
                     return result
                 else:
-                    raise TypeError("Invalid dimensions for multiplication of row vector by matrix.")
+                    raise TypeError("Invalid dimensions for multiplication of column vector by matrix.")
             else:
                 if u.size != self.size:
                     raise TypeError("Invalid dimensions for multiplication of row vector by column vector.")
                 else:
                     result = 0
                     for i in range(self.size):
                         result += self.contents[i][0]*u.contents[i]
@@ -319,16 +319,36 @@
                         for k in range(B.rows):
                             value += self.contents[i][k]*B.contents[k][j]
                         tmp1.append(value)
                     tmp.append(tmp1)
                 return Matrix(content=tmp)
             else:
                 raise ValueError("To multiply matrix A by matrix B, number of columns of A must equal number of rows of B.")
-        elif isinstance(B, rowVector) or isinstance(B,columnVector):
-            return B*self
+        elif isinstance(B,columnVector):
+            if B.size != self.columns:
+                raise ValueError("Invalid dimensions for matrix multiplication with a column vector.")
+            else:
+                tmp = []
+                for i in range(self.rows):
+                    tmp1 = 0
+                    for j in range(self.columns):
+                        tmp1 += self.contents[i][j]*B.contents[j][0]
+                    tmp.append([tmp1])
+                return Matrix(content=tmp)._clean_matrix()
+        elif isinstance(B, rowVector):
+            if self.columns != 1:
+                raise ValueError("Invalid dimensions for multiplication of a Matrix and a row vector.")
+            else:
+                tmp = []
+                for i in range(self.rows):
+                    tmp1 = []
+                    for j in range(B.size):
+                        tmp1.append(self.contents[i][0]*B.contents[j])
+                    tmp.append(tmp1)
+                return Matrix(content=tmp)._clean_matrix()
         else:
             raise TypeError("Can only multiply matrices by scalars and vectors of appropriate dimensions.")
         
 
     def row_swap(self,r1,r2):
         """Swap two rows of a matrix. If A is a matrix, A.row_swap(i,j) will swap rows i and j."""
         tmp = []
```

### Comparing `linalgebralib-0.0.0/LICENSE` & `linalgebralib-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linalgebralib-0.0.0/README.md` & `linalgebralib-0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 ### Technologies
 
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 
 This project was built for Python, with the ultimate aim of contributing to other machine learning libraries.
 
+### PyPi and Installation
+
+You can find linalgebralib on pypi here: https://pypi.org/project/linalgebralib/
+
+To install and utilize this library, simply run `pip install linalgebralib`, and import the library via `from linalgebralib import LinAlgebraLib as la`.
+
 # Documentation
 The following documents everything presently supported by linalgebralib.
 
 # Row Vectors
 rowVector objects allow users to create Row Vectors for the purposes of matrix initialization, or for uncommon applications requiring row vectors.
 
 ## Instantiation
```

### Comparing `linalgebralib-0.0.0/pyproject.toml` & `linalgebralib-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "linalgebralib"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Adam Authur", email="aauthur@tamu.edu" },
 ]
 description = "This package contains a library of methods and classes relating to Linear Algebra."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `linalgebralib-0.0.0/PKG-INFO` & `linalgebralib-0.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: linalgebralib
-Version: 0.0.0
+Version: 0.0.1
 Summary: This package contains a library of methods and classes relating to Linear Algebra.
 Project-URL: Homepage, https://github.com/aauthur/LinAlgLib
 Author-email: Adam Authur <aauthur@tamu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,20 @@
 
 ### Technologies
 
 [![python](https://img.shields.io/badge/Python-3.9-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 
 This project was built for Python, with the ultimate aim of contributing to other machine learning libraries.
 
+### PyPi and Installation
+
+You can find linalgebralib on pypi here: https://pypi.org/project/linalgebralib/
+
+To install and utilize this library, simply run `pip install linalgebralib`, and import the library via `from linalgebralib import LinAlgebraLib as la`.
+
 # Documentation
 The following documents everything presently supported by linalgebralib.
 
 # Row Vectors
 rowVector objects allow users to create Row Vectors for the purposes of matrix initialization, or for uncommon applications requiring row vectors.
 
 ## Instantiation
```

