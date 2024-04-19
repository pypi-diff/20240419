# Comparing `tmp/tcia_utils-2.1.4.tar.gz` & `tmp/tcia_utils-2.1.5.tar.gz`

## Comparing `tcia_utils-2.1.4.tar` & `tcia_utils-2.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    87292 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/src/tcia_utils/utils.py
--rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/src/tcia_utils/wordpress.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/LICENSE
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/README.md
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 tcia_utils-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    87296 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/src/tcia_utils/wordpress.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/LICENSE
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 tcia_utils-2.1.5/PKG-INFO
```

### Comparing `tcia_utils-2.1.4/src/tcia_utils/datacite.py` & `tcia_utils-2.1.5/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.4/src/tcia_utils/nbia.py` & `tcia_utils-2.1.5/src/tcia_utils/nbia.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 _log = logging.getLogger(__name__)
 logging.basicConfig(
     format='%(asctime)s:%(levelname)s:%(message)s'
     , level=logging.INFO
 )
 
 # set token creation URL for getToken and refreshToken
-token_url = "https://keycloak.dbmi.cloud/auth/realms/TCIA/protocol/openid-connect/token"
+token_url = "https://keycloak-stg.dbmi.cloud/auth/realms/TCIA/protocol/openid-connect/token"
 
 # Used by functions that accept parameters used in GUI Simple Search
 # e.g. getSimpleSearchWithModalityAndBodyPartPaged()
 class Criteria(Enum):
     Collection = "CollectionCriteria"
     Species = "SpeciesCriteria"
     ImageModality = "ImageModalityCriteria"
```

### Comparing `tcia_utils-2.1.4/src/tcia_utils/pathdb.py` & `tcia_utils-2.1.5/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.4/src/tcia_utils/utils.py` & `tcia_utils-2.1.5/src/tcia_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.4/src/tcia_utils/wordpress.py` & `tcia_utils-2.1.5/src/tcia_utils/wordpress.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.4/.gitignore` & `tcia_utils-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.4/LICENSE` & `tcia_utils-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.4/README.md` & `tcia_utils-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.4/pyproject.toml` & `tcia_utils-2.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "2.1.4"
+version = "2.1.5"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -24,14 +24,13 @@
   "requests",
   "pandas",
   "matplotlib",
   "plotly",
   "numpy",
   "ipywidgets", 
   "pydicom-seg", 
-  "rt-utils",
-  "jsonschema==4.21.1" # Prevent pydicom-seg from installing v3.2.0
+  "rt-utils"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/kirbyju/tcia_utils"
 "Bug Tracker" = "https://github.com/kirbyju/tcia_utils/issues"
```

### Comparing `tcia_utils-2.1.4/PKG-INFO` & `tcia_utils-2.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.3
 Name: tcia_utils
-Version: 2.1.4
+Version: 2.1.5
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bs4
 Requires-Dist: ipywidgets
-Requires-Dist: jsonschema==4.21.1
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pydicom
 Requires-Dist: pydicom-seg
 Requires-Dist: requests
```

