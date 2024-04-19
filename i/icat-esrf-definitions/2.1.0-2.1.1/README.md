# Comparing `tmp/icat-esrf-definitions-2.1.0.tar.gz` & `tmp/icat_esrf_definitions-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icat-esrf-definitions-2.1.0.tar", last modified: Wed Apr 10 19:25:02 2024, max compression
+gzip compressed data, was "icat_esrf_definitions-2.1.1.tar", last modified: Fri Apr 19 12:23:12 2024, max compression
```

## Comparing `icat-esrf-definitions-2.1.0.tar` & `icat_esrf_definitions-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     6362 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5691 2024-04-10 11:48:26.000000 icat-esrf-definitions-2.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-10 11:48:26.000000 icat-esrf-definitions-2.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-10 11:48:26.000000 icat-esrf-definitions-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.360925 icat-esrf-definitions-2.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.360925 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-10 19:25:00.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)   137625 2024-04-10 19:20:41.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/hdf5_cfg.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:25:02.364925 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6362 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      364 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-10 19:25:02.000000 icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 12:23:12.126261 icat_esrf_definitions-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     6561 2024-04-19 12:23:12.126261 icat_esrf_definitions-2.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5691 2024-03-27 18:23:44.000000 icat_esrf_definitions-2.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-11 08:34:07.000000 icat_esrf_definitions-2.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-04-19 12:23:12.126261 icat_esrf_definitions-2.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-11 08:34:07.000000 icat_esrf_definitions-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 12:23:12.122261 icat_esrf_definitions-2.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 12:23:12.122261 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-19 12:15:33.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   137625 2024-04-19 12:23:03.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions/hdf5_cfg.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 12:23:12.126261 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 12:23:08.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-19 05:51:23.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions/tests/test_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 12:23:12.126261 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6561 2024-04-19 12:23:12.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2024-04-19 12:23:12.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 12:23:12.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2024-04-19 12:23:12.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-19 12:23:12.000000 icat_esrf_definitions-2.1.1/src/icat_esrf_definitions.egg-info/top_level.txt
```

### Comparing `icat-esrf-definitions-2.1.0/PKG-INFO` & `icat_esrf_definitions-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: icat-esrf-definitions
-Version: 2.1.0
+Version: 2.1.1
 Summary: ESRF ICAT definitions
 Home-page: https://gitlab.esrf.fr/icat/hdf5-master-config/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/hdf5-master-config/
 Project-URL: Documentation, https://gitlab.esrf.fr/icat/hdf5-master-config/
 Project-URL: Tracker, https://gitlab.esrf.fr/icat/hdf5-master-config/issues/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: importlib_resources; python_version < "3.9"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
 # HDF5 Master config
 
 This repository contains the XML file that describes the mapping between ICAT database and the master file in HDF5 format. It also contains a set of [tools](#tools) that will help with the maintenance of it.
 
 :warning: The file `hdf5_cfg.xml` is not longer updated and only exists for backward compatibility with `pyicat-plus<=0.1.7`.
 The new definitions file is `src/icat_esrf_definitions/hdf5_cfg.xml`. Changes should be applied to the new file only.
```

### Comparing `icat-esrf-definitions-2.1.0/README.md` & `icat_esrf_definitions-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `icat-esrf-definitions-2.1.0/setup.cfg` & `icat_esrf_definitions-2.1.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -18,23 +18,28 @@
 	Programming Language :: Python :: 3
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.6
+install_requires = 
+	importlib_resources; python_version<'3.9'
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.xml
 
 [options.extras_require]
+test = 
+	pytest
 dev = 
+	%(test)s
 	pre-commit
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
 
 [egg_info]
```

### Comparing `icat-esrf-definitions-2.1.0/src/icat_esrf_definitions/hdf5_cfg.xml` & `icat_esrf_definitions-2.1.1/src/icat_esrf_definitions/hdf5_cfg.xml`

 * *Files identical despite different names*

### Comparing `icat-esrf-definitions-2.1.0/src/icat_esrf_definitions.egg-info/PKG-INFO` & `icat_esrf_definitions-2.1.1/src/icat_esrf_definitions.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: icat-esrf-definitions
-Version: 2.1.0
+Version: 2.1.1
 Summary: ESRF ICAT definitions
 Home-page: https://gitlab.esrf.fr/icat/hdf5-master-config/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/hdf5-master-config/
 Project-URL: Documentation, https://gitlab.esrf.fr/icat/hdf5-master-config/
 Project-URL: Tracker, https://gitlab.esrf.fr/icat/hdf5-master-config/issues/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: importlib_resources; python_version < "3.9"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
 # HDF5 Master config
 
 This repository contains the XML file that describes the mapping between ICAT database and the master file in HDF5 format. It also contains a set of [tools](#tools) that will help with the maintenance of it.
 
 :warning: The file `hdf5_cfg.xml` is not longer updated and only exists for backward compatibility with `pyicat-plus<=0.1.7`.
 The new definitions file is `src/icat_esrf_definitions/hdf5_cfg.xml`. Changes should be applied to the new file only.
```

