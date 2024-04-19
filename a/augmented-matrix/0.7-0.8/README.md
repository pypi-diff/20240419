# Comparing `tmp/augmented_matrix-0.7.tar.gz` & `tmp/augmented_matrix-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmented_matrix-0.7.tar", last modified: Fri Apr 19 00:16:01 2024, max compression
+gzip compressed data, was "augmented_matrix-0.8.tar", last modified: Fri Apr 19 00:17:12 2024, max compression
```

## Comparing `augmented_matrix-0.7.tar` & `augmented_matrix-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:16:01.301044 augmented_matrix-0.7/
--rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.7/LICENSE
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-19 00:16:01.300865 augmented_matrix-0.7/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.7/README.md
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:16:01.299274 augmented_matrix-0.7/augmented_matrix/
--rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.7/augmented_matrix/__init__.py
--rw-r--r--   0 yumengliu   (501) staff       (20)     5001 2024-04-19 00:10:28.000000 augmented_matrix-0.7/augmented_matrix/augmented_matrix.py
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:16:01.300679 augmented_matrix-0.7/augmented_matrix.egg-info/
--rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-19 00:16:01.000000 augmented_matrix-0.7/augmented_matrix.egg-info/PKG-INFO
--rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-04-19 00:16:01.000000 augmented_matrix-0.7/augmented_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-19 00:16:01.000000 augmented_matrix-0.7/augmented_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-19 00:16:01.000000 augmented_matrix-0.7/augmented_matrix.egg-info/requires.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-19 00:16:01.000000 augmented_matrix-0.7/augmented_matrix.egg-info/top_level.txt
--rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-04-19 00:12:21.000000 augmented_matrix-0.7/pyproject.toml
--rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-19 00:16:01.301077 augmented_matrix-0.7/setup.cfg
-drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:16:01.300186 augmented_matrix-0.7/test/
--rw-r--r--   0 yumengliu   (501) staff       (20)     2255 2024-04-16 20:10:05.000000 augmented_matrix-0.7/test/test_augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.484227 augmented_matrix-0.8/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     1068 2024-04-15 19:47:36.000000 augmented_matrix-0.8/LICENSE
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-19 00:17:12.483937 augmented_matrix-0.8/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      168 2024-04-16 17:23:36.000000 augmented_matrix-0.8/README.md
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.482853 augmented_matrix-0.8/augmented_matrix/
+-rw-r--r--   0 yumengliu   (501) staff       (20)       32 2024-04-15 23:00:31.000000 augmented_matrix-0.8/augmented_matrix/__init__.py
+-rw-r--r--   0 yumengliu   (501) staff       (20)     4949 2024-04-19 00:17:04.000000 augmented_matrix-0.8/augmented_matrix/augmented_matrix.py
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.483761 augmented_matrix-0.8/augmented_matrix.egg-info/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2009 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 yumengliu   (501) staff       (20)      327 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        1 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)        6 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/requires.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)       17 2024-04-19 00:17:12.000000 augmented_matrix-0.8/augmented_matrix.egg-info/top_level.txt
+-rw-r--r--   0 yumengliu   (501) staff       (20)      613 2024-04-19 00:17:04.000000 augmented_matrix-0.8/pyproject.toml
+-rw-r--r--   0 yumengliu   (501) staff       (20)       38 2024-04-19 00:17:12.484272 augmented_matrix-0.8/setup.cfg
+drwxr-xr-x   0 yumengliu   (501) staff       (20)        0 2024-04-19 00:17:12.483477 augmented_matrix-0.8/test/
+-rw-r--r--   0 yumengliu   (501) staff       (20)     2255 2024-04-16 20:10:05.000000 augmented_matrix-0.8/test/test_augmented_matrix.py
```

### Comparing `augmented_matrix-0.7/LICENSE` & `augmented_matrix-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `augmented_matrix-0.7/PKG-INFO` & `augmented_matrix-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.7
+Version: 0.8
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.7/augmented_matrix/augmented_matrix.py` & `augmented_matrix-0.8/augmented_matrix/augmented_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
                     if leading_value == 0:
                         continue
                     factor = -1 * pivot / leading_value
                     matrix[i] = factor * matrix[i] + matrix[row]
 
             column += 1
             row = column
-            print(matrix)
 
         self._matrix = matrix
         return matrix
 
     def simplify_echelon(self) -> np.ndarray:
         """
         Simplifies the upper triangular form so that the pivots are 1
@@ -132,15 +131,14 @@
                     leading = matrix[i][pivot_coord[1]]
                     if leading == 0:
                         continue
 
                     pivot = matrix[pivot_coord[0]][pivot_coord[1]]
                     factor = -1 * leading / pivot
                     matrix[i] = factor * matrix[pivot_coord[0]] + matrix[i]
-            print(matrix)
 
         self._matrix = matrix
         return matrix
 
     def solve(self) -> np.ndarray:
         """
         Solves the augmented matrix
```

### Comparing `augmented_matrix-0.7/augmented_matrix.egg-info/PKG-INFO` & `augmented_matrix-0.8/augmented_matrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmented-matrix
-Version: 0.7
+Version: 0.8
 Summary: A package that solves augmented matrices into reduced echelon forms
 Author-email: Yumeng Liu <lym20041026@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `augmented_matrix-0.7/pyproject.toml` & `augmented_matrix-0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "augmented-matrix"
-version = "0.7"
+version = "0.8"
 authors = [
   { name="Yumeng Liu", email="lym20041026@gmail.com" }
 ]
 description = "A package that solves augmented matrices into reduced echelon forms"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies= ['numpy']
```

### Comparing `augmented_matrix-0.7/test/test_augmented_matrix.py` & `augmented_matrix-0.8/test/test_augmented_matrix.py`

 * *Files identical despite different names*

