# Comparing `tmp/geneweaver_core-0.9.0a8.tar.gz` & `tmp/geneweaver_core-0.9.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_core-0.9.0a8.tar", max compression
+gzip compressed data, was "geneweaver_core-0.9.0a9.tar", max compression
```

## Comparing `geneweaver_core-0.9.0a8.tar` & `geneweaver_core-0.9.0a9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    11356 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/LICENSE
--rw-r--r--   0        0        0     2684 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/README.md
--rw-r--r--   0        0        0     1036 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/pyproject.toml
--rw-r--r--   0        0        0      109 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/__init__.py
--rw-r--r--   0        0        0      171 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/config.py
--rw-r--r--   0        0        0      739 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/config_class.py
--rw-r--r--   0        0        0    12298 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/enum.py
--rw-r--r--   0        0        0      257 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/exc.py
--rw-r--r--   0        0        0      638 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/mapping.py
--rw-r--r--   0        0        0       53 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/__init__.py
--rw-r--r--   0        0        0    18345 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/batch.py
--rw-r--r--   0        0        0     5841 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/csv.py
--rw-r--r--   0        0        0      322 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/enum.py
--rw-r--r--   0        0        0     1456 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/exceptions.py
--rw-r--r--   0        0        0     5053 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/numpy.py
--rw-r--r--   0        0        0     9436 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/score.py
--rw-r--r--   0        0        0     3435 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/threshold.py
--rw-r--r--   0        0        0     1936 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/utils.py
--rw-r--r--   0        0        0    10903 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/parse/xlsx.py
--rw-r--r--   0        0        0       81 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/publication/__init__.py
--rw-r--r--   0        0        0     6079 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/publication/pubmed.py
--rw-r--r--   0        0        0       79 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/render/__init__.py
--rw-r--r--   0        0        0     1913 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/render/batch.py
--rw-r--r--   0        0        0     1281 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/render/csv.py
--rw-r--r--   0        0        0      679 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/render/gene_list.py
--rw-r--r--   0        0        0      351 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/__init__.py
--rw-r--r--   0        0        0     4263 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/batch.py
--rw-r--r--   0        0        0     1696 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/gene.py
--rw-r--r--   0        0        0     2360 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/geneset.py
--rw-r--r--   0        0        0      462 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/group.py
--rw-r--r--   0        0        0     1204 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/legacy_api.py
--rw-r--r--   0        0        0      814 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/messages.py
--rw-r--r--   0        0        0      505 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/ontology.py
--rw-r--r--   0        0        0      330 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/project.py
--rw-r--r--   0        0        0      511 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/publication.py
--rw-r--r--   0        0        0      661 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/score.py
--rw-r--r--   0        0        0      594 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/species.py
--rw-r--r--   0        0        0      212 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/stubgenerator.py
--rw-r--r--   0        0        0      942 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/schema/user.py
--rw-r--r--   0        0        0     1453 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/threshold.py
--rw-r--r--   0        0        0      188 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/types.py
--rw-r--r--   0        0        0      528 2024-03-22 18:02:09.328851 geneweaver_core-0.9.0a8/src/geneweaver/core/utils.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 geneweaver_core-0.9.0a8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/LICENSE
+-rw-r--r--   0        0        0     3413 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/README.md
+-rw-r--r--   0        0        0     1036 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/config.py
+-rw-r--r--   0        0        0      739 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/config_class.py
+-rw-r--r--   0        0        0    12499 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/enum.py
+-rw-r--r--   0        0        0      257 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/exc.py
+-rw-r--r--   0        0        0      638 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/mapping.py
+-rw-r--r--   0        0        0       53 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/__init__.py
+-rw-r--r--   0        0        0    18345 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/batch.py
+-rw-r--r--   0        0        0     5841 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/csv.py
+-rw-r--r--   0        0        0      322 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/enum.py
+-rw-r--r--   0        0        0     1456 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/exceptions.py
+-rw-r--r--   0        0        0     5053 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/numpy.py
+-rw-r--r--   0        0        0     9436 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/score.py
+-rw-r--r--   0        0        0     3435 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/threshold.py
+-rw-r--r--   0        0        0     1936 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/utils.py
+-rw-r--r--   0        0        0    10903 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/xlsx.py
+-rw-r--r--   0        0        0       81 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/publication/__init__.py
+-rw-r--r--   0        0        0     6079 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/publication/pubmed.py
+-rw-r--r--   0        0        0       79 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/__init__.py
+-rw-r--r--   0        0        0     1913 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/batch.py
+-rw-r--r--   0        0        0     1281 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/csv.py
+-rw-r--r--   0        0        0      679 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/gene_list.py
+-rw-r--r--   0        0        0      417 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/api_response.py
+-rw-r--r--   0        0        0     4263 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/batch.py
+-rw-r--r--   0        0        0     1696 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/gene.py
+-rw-r--r--   0        0        0     2360 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/geneset.py
+-rw-r--r--   0        0        0      462 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/group.py
+-rw-r--r--   0        0        0     1204 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/legacy_api.py
+-rw-r--r--   0        0        0      814 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/messages.py
+-rw-r--r--   0        0        0      505 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/ontology.py
+-rw-r--r--   0        0        0      330 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/project.py
+-rw-r--r--   0        0        0      511 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/publication.py
+-rw-r--r--   0        0        0      944 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/score.py
+-rw-r--r--   0        0        0      594 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/species.py
+-rw-r--r--   0        0        0      212 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/stubgenerator.py
+-rw-r--r--   0        0        0      942 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/user.py
+-rw-r--r--   0        0        0     1453 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/threshold.py
+-rw-r--r--   0        0        0      321 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/types.py
+-rw-r--r--   0        0        0      528 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/utils.py
+-rw-r--r--   0        0        0     4340 1970-01-01 00:00:00.000000 geneweaver_core-0.9.0a9/PKG-INFO
```

### Comparing `geneweaver_core-0.9.0a8/LICENSE` & `geneweaver_core-0.9.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/README.md` & `geneweaver_core-0.9.0a9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Geneweaver Core
 
-[![Tests](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/tests.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/tests.yml)
-[![Style](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/style.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/style.yml)
-[![Coverage](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/coverage.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/coverage.yml)
+
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/geneweaver-core/tests.yml?branch=main&style=for-the-badge&logo=github&label=Tests)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/tests.yml?query=branch%3Amain++)
+[![Style](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/geneweaver-core/style.yml?branch=main&style=for-the-badge&logo=github&label=Style)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/style.yml?query=branch%3Amain++)
+[![Coverage](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/geneweaver-core/coverage.yml?branch=main&style=for-the-badge&logo=github&label=Coverage)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/coverage.yml?query=branch%3Amain++)
+
+![PyPI - License](https://img.shields.io/pypi/l/geneweaver-core?style=for-the-badge)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/geneweaver-core?style=for-the-badge)
+[![PyPI - Version](https://img.shields.io/pypi/v/geneweaver-core?style=for-the-badge&logo=pypi&logoColor=%23fff)](https://pypi.org/project/geneweaver-core/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/geneweaver-core?style=for-the-badge)](https://pypi.org/project/geneweaver-core/)
+
 
 The Geneweaver Core Python library provides shared foundational functionality for the Geneweaver project. 
 It is a dependency of all other Geneweaver Python libraries, and is not intended to be used directly.
 
 ## Installation
 The Geneweaver Core library is available on PyPI and can be installed with pip:
 ```bash
```

### Comparing `geneweaver_core-0.9.0a8/pyproject.toml` & `geneweaver_core-0.9.0a9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-core"
-version = "0.9.0a8"
+version = "0.9.0a9"
 description = "The core of the Jax-Geneweaver Python library"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-client"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 packages = [
```

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/config_class.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/config_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/enum.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,26 @@
     APPROVED = 5
 
     @staticmethod
     def _str_class() -> Enum:
         return CurationAssignment
 
 
+class Sex(Enum):
+    """The Sex of an Animal."""
+
+    FEMALE = "Female"
+    MALE = "Male"
+    BOTH = "Both"
+
+    def __str__(self) -> str:
+        """Render as a string."""
+        return self.value
+
+
 class ScoreType(_StrToIntMixin, Enum):
     """Enum for the different types of geneset scores."""
 
     P_VALUE = "p-value"
     Q_VALUE = "q-value"
     BINARY = "binary"
     CORRELATION = "correlation"
```

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/mapping.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/mapping.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/batch.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/csv.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/csv.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/exceptions.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/exceptions.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/numpy.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/numpy.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/score.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/score.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/threshold.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/utils.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/parse/xlsx.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/xlsx.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/publication/pubmed.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/publication/pubmed.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/render/batch.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/render/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/render/csv.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/render/csv.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/render/gene_list.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/render/gene_list.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/batch.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/gene.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/geneset.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/legacy_api.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/legacy_api.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/messages.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/messages.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/score.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/score.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,7 +15,14 @@
 
     def __str__(self: "GenesetScoreType") -> str:
         """Return a string representation of the score type."""
         name = self.score_type.name.title().replace("_", "-")
         if self.threshold_low:
             return f"{self.threshold_low} < {name} < {self.threshold}"
         return f"{name} < {self.threshold}"
+
+    def threshold_as_db_string(self) -> str:
+        """Return a string representation of the score type for the database."""
+        if self.threshold_low is not None:
+            return f"{self.threshold_low},{self.threshold}"
+        else:
+            return str(self.threshold)
```

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/species.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/schema/user.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/threshold.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/src/geneweaver/core/utils.py` & `geneweaver_core-0.9.0a9/src/geneweaver/core/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a8/PKG-INFO` & `geneweaver_core-0.9.0a9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-core
-Version: 0.9.0a8
+Version: 0.9.0a9
 Summary: The core of the Jax-Geneweaver Python library
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,17 +19,24 @@
 Requires-Dist: pydantic[dotenv] (>=1.10,<2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/TheJacksonLaboratory/geneweaver-client
 Description-Content-Type: text/markdown
 
 # Geneweaver Core
 
-[![Tests](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/tests.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/tests.yml)
-[![Style](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/style.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/style.yml)
-[![Coverage](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/coverage.yml/badge.svg?event=push)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/coverage.yml)
+
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/geneweaver-core/tests.yml?branch=main&style=for-the-badge&logo=github&label=Tests)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/tests.yml?query=branch%3Amain++)
+[![Style](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/geneweaver-core/style.yml?branch=main&style=for-the-badge&logo=github&label=Style)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/style.yml?query=branch%3Amain++)
+[![Coverage](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/geneweaver-core/coverage.yml?branch=main&style=for-the-badge&logo=github&label=Coverage)](https://github.com/TheJacksonLaboratory/geneweaver-core/actions/workflows/coverage.yml?query=branch%3Amain++)
+
+![PyPI - License](https://img.shields.io/pypi/l/geneweaver-core?style=for-the-badge)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/geneweaver-core?style=for-the-badge)
+[![PyPI - Version](https://img.shields.io/pypi/v/geneweaver-core?style=for-the-badge&logo=pypi&logoColor=%23fff)](https://pypi.org/project/geneweaver-core/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/geneweaver-core?style=for-the-badge)](https://pypi.org/project/geneweaver-core/)
+
 
 The Geneweaver Core Python library provides shared foundational functionality for the Geneweaver project. 
 It is a dependency of all other Geneweaver Python libraries, and is not intended to be used directly.
 
 ## Installation
 The Geneweaver Core library is available on PyPI and can be installed with pip:
 ```bash
```

