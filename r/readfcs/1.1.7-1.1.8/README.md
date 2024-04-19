# Comparing `tmp/readfcs-1.1.7.tar.gz` & `tmp/readfcs-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readfcs-1.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "readfcs-1.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `readfcs-1.1.7.tar` & `readfcs-1.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1855 2023-08-25 09:57:47.512474 readfcs-1.1.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-25 08:22:00.201619 readfcs-1.1.7/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-25 08:22:00.201910 readfcs-1.1.7/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1207 2022-08-30 14:21:07.236348 readfcs-1.1.7/.gitignore
--rw-r--r--   0        0        0     1943 2022-07-10 14:01:24.300288 readfcs-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      624 2022-08-30 14:11:54.721602 readfcs-1.1.7/CITATION.cff
--rw-r--r--   0        0        0    11324 2022-05-28 11:31:06.237861 readfcs-1.1.7/LICENSE
--rw-r--r--   0        0        0     1033 2023-08-24 16:17:25.469661 readfcs-1.1.7/README.md
--rw-r--r--   0        0        0       49 2022-05-28 10:53:31.440992 readfcs-1.1.7/docs/api.md
--rw-r--r--   0        0        0     4445 2023-10-03 17:41:17.031275 readfcs-1.1.7/docs/changelog.md
--rw-r--r--   0        0        0      125 2023-08-24 17:04:51.637787 readfcs-1.1.7/docs/index.md
--rw-r--r--   0        0        0     5548 2023-10-03 17:39:56.458372 readfcs-1.1.7/docs/quickstart.ipynb
--rw-r--r--   0        0        0      119 2022-08-30 14:11:54.723988 readfcs-1.1.7/lamin-project.yaml
--rw-r--r--   0        0        0      437 2023-08-24 16:17:25.470004 readfcs-1.1.7/noxfile.py
--rw-r--r--   0        0        0      964 2023-08-25 09:04:50.347501 readfcs-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      389 2023-10-03 17:41:05.484364 readfcs-1.1.7/readfcs/__init__.py
--rw-r--r--   0        0        0     8725 2023-08-24 16:17:25.470999 readfcs-1.1.7/readfcs/_core.py
--rw-r--r--   0        0        0      178 2023-10-03 17:39:56.460154 readfcs-1.1.7/readfcs/datasets/__init__.py
--rw-r--r--   0        0        0     1698 2023-10-03 17:39:56.460537 readfcs-1.1.7/readfcs/datasets/_datasets.py
--rw-r--r--   0        0        0       88 2022-07-11 14:13:41.976849 readfcs-1.1.7/tests/test_base.py
--rw-r--r--   0        0        0      509 2023-08-24 16:17:25.471209 readfcs-1.1.7/tests/test_notebooks.py
--rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 readfcs-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-08-25 09:57:47.512474 readfcs-1.1.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-25 08:22:00.201619 readfcs-1.1.8/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-25 08:22:00.201910 readfcs-1.1.8/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1207 2022-08-30 14:21:07.236348 readfcs-1.1.8/.gitignore
+-rw-r--r--   0        0        0     1943 2022-07-10 14:01:24.300288 readfcs-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      624 2022-08-30 14:11:54.721602 readfcs-1.1.8/CITATION.cff
+-rw-r--r--   0        0        0    11324 2022-05-28 11:31:06.237861 readfcs-1.1.8/LICENSE
+-rw-r--r--   0        0        0     1033 2023-08-24 16:17:25.469661 readfcs-1.1.8/README.md
+-rw-r--r--   0        0        0       49 2022-05-28 10:53:31.440992 readfcs-1.1.8/docs/api.md
+-rw-r--r--   0        0        0     4589 2024-04-19 11:36:59.995773 readfcs-1.1.8/docs/changelog.md
+-rw-r--r--   0        0        0      125 2023-08-24 17:04:51.637787 readfcs-1.1.8/docs/index.md
+-rw-r--r--   0        0        0     5548 2023-10-03 17:39:56.458372 readfcs-1.1.8/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      119 2022-08-30 14:11:54.723988 readfcs-1.1.8/lamin-project.yaml
+-rw-r--r--   0        0        0      437 2023-08-24 16:17:25.470004 readfcs-1.1.8/noxfile.py
+-rw-r--r--   0        0        0      964 2023-08-25 09:04:50.347501 readfcs-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      275 2024-04-19 11:37:17.462990 readfcs-1.1.8/readfcs/__init__.py
+-rw-r--r--   0        0        0     8865 2024-04-19 11:36:58.338070 readfcs-1.1.8/readfcs/_core.py
+-rw-r--r--   0        0        0      178 2023-10-03 17:39:56.460154 readfcs-1.1.8/readfcs/datasets/__init__.py
+-rw-r--r--   0        0        0     1698 2023-10-03 17:39:56.460537 readfcs-1.1.8/readfcs/datasets/_datasets.py
+-rw-r--r--   0        0        0       88 2022-07-11 14:13:41.976849 readfcs-1.1.8/tests/test_base.py
+-rw-r--r--   0        0        0      509 2023-08-24 16:17:25.471209 readfcs-1.1.8/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 readfcs-1.1.8/PKG-INFO
```

### Comparing `readfcs-1.1.7/.github/workflows/build.yml` & `readfcs-1.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/.github/workflows/latest-changes.yml` & `readfcs-1.1.8/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/.gitignore` & `readfcs-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/.pre-commit-config.yaml` & `readfcs-1.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/CITATION.cff` & `readfcs-1.1.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/LICENSE` & `readfcs-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/README.md` & `readfcs-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/docs/changelog.md` & `readfcs-1.1.8/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🏷️ Save object as category | [36](https://github.com/laminlabs/readfcs/pull/36) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-19 |
 🍱 Added oetjen18 files | [35](https://github.com/laminlabs/readfcs/pull/35) | [sunnyosun](https://github.com/sunnyosun) | 2023-10-03 | 1.1.7
 👷 Remove nox cache | [34](https://github.com/laminlabs/readfcs/pull/34) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-25 |
 👷 Test py3.11 | [33](https://github.com/laminlabs/readfcs/pull/33) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-25 | 1.1.6
 🚑️ Raise error if the spill index doesn't match channels | [32](https://github.com/laminlabs/readfcs/pull/32) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-24 |
 ✏️ Fix blank stripping | [30](https://github.com/laminlabs/readfcs/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-08 | 1.1.5
 🚑️ Make sure channels are sorted by n | [29](https://github.com/laminlabs/readfcs/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-07 | 1.1.4
 🩹 Remove whitespace only markers | [26](https://github.com/laminlabs/readfcs/pull/26) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-27 | 1.1.3
```

### Comparing `readfcs-1.1.7/docs/quickstart.ipynb` & `readfcs-1.1.8/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/pyproject.toml` & `readfcs-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/readfcs/_core.py` & `readfcs-1.1.8/readfcs/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,18 @@
                         f"spill matrix index contains {n_mismatch} mismatches to the channels, please check your metadata."  # noqa
                     )
                 self._meta["spill"].rename(index=mapper, inplace=True)
                 self._meta["spill"].rename(columns=mapper, inplace=True)
 
         # write metadata into adata.uns
         adata.uns["meta"] = self.meta
+
+        for k, v in adata.var.dtypes.items():
+            if v == "object":
+                adata.var[k] = adata.var[k].astype("category")
         return adata
 
 
 def read(filepath, reindex=True) -> ad.AnnData:
     """Read in fcs file as AnnData.
 
     Args:
```

### Comparing `readfcs-1.1.7/readfcs/datasets/_datasets.py` & `readfcs-1.1.8/readfcs/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `readfcs-1.1.7/PKG-INFO` & `readfcs-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readfcs
-Version: 1.1.7
+Version: 1.1.8
 Summary: Parse fcs files into AnnData.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

