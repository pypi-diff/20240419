# Comparing `tmp/scbl_utils-1.13.tar.gz` & `tmp/scbl_utils-1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scbl_utils-1.13.tar", max compression
+gzip compressed data, was "scbl_utils-1.14.tar", max compression
```

## Comparing `scbl_utils-1.13.tar` & `scbl_utils-1.14.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1079 2023-12-14 16:32:13.627049 scbl_utils-1.13/LICENSE
--rw-r--r--   0        0        0     8239 2024-01-23 19:13:12.443282 scbl_utils-1.13/README.md
--rw-r--r--   0        0        0      995 2024-04-16 14:34:19.641614 scbl_utils-1.13/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 16:32:13.628638 scbl_utils-1.13/scbl_utils/__init__.py
--rw-r--r--   0        0        0     8720 2024-04-16 14:41:10.856027 scbl_utils-1.13/scbl_utils/main.py
--rw-r--r--   0        0        0     7527 2024-03-27 18:02:48.976351 scbl_utils-1.13/scbl_utils/utils/defaults.py
--rw-r--r--   0        0        0     9033 2024-04-16 14:41:03.477720 scbl_utils-1.13/scbl_utils/utils/gdrive.py
--rw-r--r--   0        0        0    14379 2024-03-27 17:51:34.920949 scbl_utils-1.13/scbl_utils/utils/samplesheet.py
--rw-r--r--   0        0        0     4049 2023-12-14 16:32:13.629985 scbl_utils-1.13/scbl_utils/utils/validate.py
--rw-r--r--   0        0        0     9353 1970-01-01 00:00:00.000000 scbl_utils-1.13/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-12-14 16:32:13.627049 scbl_utils-1.14/LICENSE
+-rw-r--r--   0        0        0     8239 2024-01-23 19:13:12.443282 scbl_utils-1.14/README.md
+-rw-r--r--   0        0        0      995 2024-04-19 20:37:24.798412 scbl_utils-1.14/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 16:32:13.628638 scbl_utils-1.14/scbl_utils/__init__.py
+-rw-r--r--   0        0        0     8720 2024-04-16 14:41:10.856027 scbl_utils-1.14/scbl_utils/main.py
+-rw-r--r--   0        0        0     7527 2024-03-27 18:02:48.976351 scbl_utils-1.14/scbl_utils/utils/defaults.py
+-rw-r--r--   0        0        0     9033 2024-04-16 14:41:03.477720 scbl_utils-1.14/scbl_utils/utils/gdrive.py
+-rw-r--r--   0        0        0    14379 2024-04-19 20:36:46.028249 scbl_utils-1.14/scbl_utils/utils/samplesheet.py
+-rw-r--r--   0        0        0     4049 2023-12-14 16:32:13.629985 scbl_utils-1.14/scbl_utils/utils/validate.py
+-rw-r--r--   0        0        0     9353 1970-01-01 00:00:00.000000 scbl_utils-1.14/PKG-INFO
```

### Comparing `scbl_utils-1.13/LICENSE` & `scbl_utils-1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.13/README.md` & `scbl_utils-1.14/README.md`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.13/pyproject.toml` & `scbl_utils-1.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scbl-utils"
-version = "1.13"
+version = "1.14"
 description = "A set of command-line utilities that facilitate data processing at the Single Cell Biology Lab at the Jackson Laboratory."
 authors = ["Ahmed Said <ahmed.said@jax.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TheJacksonLaboratory/scbl-utils/"
 documentation = "https://github.com/TheJacksonLaboratory/scbl-utils/"
```

### Comparing `scbl_utils-1.13/scbl_utils/main.py` & `scbl_utils-1.14/scbl_utils/main.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.13/scbl_utils/utils/defaults.py` & `scbl_utils-1.14/scbl_utils/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.13/scbl_utils/utils/gdrive.py` & `scbl_utils-1.14/scbl_utils/utils/gdrive.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.13/scbl_utils/utils/samplesheet.py` & `scbl_utils-1.14/scbl_utils/utils/samplesheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ) -> (
     str
 ):
     match tool:
         case 'cellranger':
             return '7.1.0'
         case 'spaceranger':
-            return '7.1.0'
+            return '2.1.0'
         case 'cellranger-atac':
             return '2.1.0'
         case 'cellranger-arc':
             return '2.0.1'
         case _:
             raise NotImplementedError(f'{tool} not available')
```

### Comparing `scbl_utils-1.13/scbl_utils/utils/validate.py` & `scbl_utils-1.14/scbl_utils/utils/validate.py`

 * *Files identical despite different names*

### Comparing `scbl_utils-1.13/PKG-INFO` & `scbl_utils-1.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scbl-utils
-Version: 1.13
+Version: 1.14
 Summary: A set of command-line utilities that facilitate data processing at the Single Cell Biology Lab at the Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/scbl-utils/
 License: MIT
 Author: Ahmed Said
 Author-email: ahmed.said@jax.org
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

