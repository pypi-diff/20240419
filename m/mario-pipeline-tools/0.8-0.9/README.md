# Comparing `tmp/mario-pipeline-tools-0.8.tar.gz` & `tmp/mario-pipeline-tools-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mario-pipeline-tools-0.8.tar", last modified: Thu Dec  7 15:18:22 2023, max compression
+gzip compressed data, was "mario-pipeline-tools-0.9.tar", last modified: Thu Dec  7 15:49:25 2023, max compression
```

## Comparing `mario-pipeline-tools-0.8.tar` & `mario-pipeline-tools-0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:18:22.800553 mario-pipeline-tools-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-07 15:18:22.800553 mario-pipeline-tools-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:18:22.800553 mario-pipeline-tools-0.8/mario/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/dataset_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/mario/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:18:22.800553 mario-pipeline-tools-0.8/mario_pipeline_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-07 15:18:22.000000 mario-pipeline-tools-0.8/mario_pipeline_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-07 15:18:22.000000 mario-pipeline-tools-0.8/mario_pipeline_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 15:18:22.000000 mario-pipeline-tools-0.8/mario_pipeline_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-07 15:18:22.000000 mario-pipeline-tools-0.8/mario_pipeline_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-07 15:18:22.000000 mario-pipeline-tools-0.8/mario_pipeline_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 15:18:22.800553 mario-pipeline-tools-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:18:22.800553 mario-pipeline-tools-0.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/test/test_data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/test/test_dataset_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/test/test_integrated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/test/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-12-07 15:18:12.000000 mario-pipeline-tools-0.8/test/test_query_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:49:25.192767 mario-pipeline-tools-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-07 15:49:25.192767 mario-pipeline-tools-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:49:25.188768 mario-pipeline-tools-0.9/mario/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/dataset_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/mario/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:49:25.192767 mario-pipeline-tools-0.9/mario_pipeline_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-07 15:49:25.000000 mario-pipeline-tools-0.9/mario_pipeline_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-07 15:49:25.000000 mario-pipeline-tools-0.9/mario_pipeline_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 15:49:25.000000 mario-pipeline-tools-0.9/mario_pipeline_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-07 15:49:25.000000 mario-pipeline-tools-0.9/mario_pipeline_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-07 15:49:25.000000 mario-pipeline-tools-0.9/mario_pipeline_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 15:49:25.192767 mario-pipeline-tools-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:49:25.192767 mario-pipeline-tools-0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/test/test_data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/test/test_dataset_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/test/test_integrated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/test/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-12-07 15:49:15.000000 mario-pipeline-tools-0.9/test/test_query_builder.py
```

### Comparing `mario-pipeline-tools-0.8/README.md` & `mario-pipeline-tools-0.9/README.md`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/mario/base.py` & `mario-pipeline-tools-0.9/mario/base.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/mario/data_extractor.py` & `mario-pipeline-tools-0.9/mario/data_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,17 @@
                 # TODO something here for Airflow hooks
                 pass
             else:
                 self.__load_from_sql__()
 
     def __load_from_sql__(self):
         self.__build_query__()
-        # TODO connect using ODBC connection string
-        # TODO run query using pyodbc
+        from sqlalchemy import create_engine
+        engine = create_engine(self.configuration.connection_string)
+        self._data = pd.read_sql(sql=self._query[0], con=engine.connect(), params=self._query[1])
         logger.info("Executing query")
 
     def __build_query__(self):
         logger.info("Building query")
         self._query = ''
         if self.configuration.query_builder is not None:
             from mario.query_builder import QueryBuilder
```

### Comparing `mario-pipeline-tools-0.8/mario/dataset_builder.py` & `mario-pipeline-tools-0.9/mario/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/mario/dataset_specification.py` & `mario-pipeline-tools-0.9/mario/dataset_specification.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/mario/example.py` & `mario-pipeline-tools-0.9/mario/example.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/mario/metadata.py` & `mario-pipeline-tools-0.9/mario/metadata.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/mario/query_builder.py` & `mario-pipeline-tools-0.9/mario/query_builder.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/mario_pipeline_tools.egg-info/SOURCES.txt` & `mario-pipeline-tools-0.9/mario_pipeline_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/setup.py` & `mario-pipeline-tools-0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name='mario-pipeline-tools',
-    version='0.8',
+    version='0.9',
     packages=['mario'],
     url='https://github.com/JiscDACT/mario',
     license='all rights reserved',
     author='scottbw',
     author_email='scott.wilson@jisc.ac.uk',
     description='Base classes and helpers for common data pipeline tasks',
     long_description='A set of base classes and helpers for common data pipeline tasks, '
                      'whether using in local control scripts or in Airflow tasks.',
     package_data={
         # If any package contains *.ini files, include them
         '': ['*.ini']
     },
     include_package_data=True,
-    install_requires=['pandas', 'tableauhyperapi', 'pantab', 'tableau-builder==0.18', 'pypika']
+    install_requires=['pandas', 'tableauhyperapi', 'pantab', 'tableau-builder==0.18', 'pypika', 'sqlalchemy']
 )
```

### Comparing `mario-pipeline-tools-0.8/test/test_data_extractor.py` & `mario-pipeline-tools-0.9/test/test_data_extractor.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/test/test_integrated.py` & `mario-pipeline-tools-0.9/test/test_integrated.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/test/test_manifest.py` & `mario-pipeline-tools-0.9/test/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/test/test_metadata.py` & `mario-pipeline-tools-0.9/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mario-pipeline-tools-0.8/test/test_query_builder.py` & `mario-pipeline-tools-0.9/test/test_query_builder.py`

 * *Files identical despite different names*

