# Comparing `tmp/jaxonloader-0.3.8.tar.gz` & `tmp/jaxonloader-0.3.9.tar.gz`

## Comparing `jaxonloader-0.3.8.tar` & `jaxonloader-0.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/boto_client.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/config.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/dataset.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/datasets/download.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/tests/test_mnist.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/boto_client.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/config.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/datasets/download.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/tests/test_mnist.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/README.md
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/PKG-INFO
```

### Comparing `jaxonloader-0.3.8/.github/workflows/nox.yaml` & `jaxonloader-0.3.9/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/docs/getting-started.md` & `jaxonloader-0.3.9/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/docs/index.md` & `jaxonloader-0.3.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/docs/images/performance.png` & `jaxonloader-0.3.9/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/jaxonloader/config.py` & `jaxonloader-0.3.9/jaxonloader/config.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/jaxonloader/dataloader.py` & `jaxonloader-0.3.9/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/jaxonloader/dataset.py` & `jaxonloader-0.3.9/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/jaxonloader/utils.py` & `jaxonloader-0.3.9/jaxonloader/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.9/jaxonloader/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/jaxonloader/datasets/download.py` & `jaxonloader-0.3.9/jaxonloader/datasets/download.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.9/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/.gitignore` & `jaxonloader-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/LICENSE` & `jaxonloader-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/README.md` & `jaxonloader-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.8/pyproject.toml` & `jaxonloader-0.3.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "jaxonloader"
-version = "0.3.8"
+version = "0.3.9"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
 dependencies=[
   "jaxtyping",
-  "progressbar",
+  "progressbar2",
   "polars",
   "beartype",
   "typing_extensions",
   "loguru",
   "pyarrow",
   "boto3",
   "boto3-stubs",
```

### Comparing `jaxonloader-0.3.8/PKG-INFO` & `jaxonloader-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.8
+Version: 0.3.9
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Requires-Dist: boto3
 Requires-Dist: boto3-stubs
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxtyping
 Requires-Dist: loguru
 Requires-Dist: polars
-Requires-Dist: progressbar
+Requires-Dist: progressbar2
 Requires-Dist: pyarrow
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: mkdocs; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
```

