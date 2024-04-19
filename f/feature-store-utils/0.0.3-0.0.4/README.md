# Comparing `tmp/feature_store_utils-0.0.3.tar.gz` & `tmp/feature_store_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_store_utils-0.0.3.tar", last modified: Mon May 29 18:31:44 2023, max compression
+gzip compressed data, was "feature_store_utils-0.0.4.tar", last modified: Fri Apr 19 13:26:41 2024, max compression
```

## Comparing `feature_store_utils-0.0.3.tar` & `feature_store_utils-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.267015 feature_store_utils-0.0.3/
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)    11357 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/LICENSE
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3593 2023-05-29 18:31:44.266809 feature_store_utils-0.0.3/PKG-INFO
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3195 2023-05-29 18:30:36.000000 feature_store_utils-0.0.3/README.md
-drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.262908 feature_store_utils-0.0.3/feature_store_utils.egg-info/
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3593 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/PKG-INFO
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)      561 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)        1 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)       59 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/requires.txt
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)        9 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/top_level.txt
-drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.264886 feature_store_utils-0.0.3/features/
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)        0 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/__init__.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     5807 2023-05-22 13:30:53.000000 feature_store_utils-0.0.3/features/feature_generation.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1730 2023-05-22 13:30:53.000000 feature_store_utils-0.0.3/features/feature_spec.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1341 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/hyper_feature.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1779 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/sql_gen.py
-drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.266486 feature_store_utils-0.0.3/features/templates/
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1339 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/fact_aggregations.j2
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     2656 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/timeseries_growth.j2
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1721 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/timeseries_growth_m.j2
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)      526 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/type1_lookup.j2
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)      708 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/type2_lookup.j2
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)      653 2023-05-29 18:31:38.000000 feature_store_utils-0.0.3/pyproject.toml
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)       38 2023-05-29 18:31:44.267068 feature_store_utils-0.0.3/setup.cfg
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2024-04-19 13:26:41.791518 feature_store_utils-0.0.4/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)    11357 2023-02-13 15:10:53.000000 feature_store_utils-0.0.4/LICENSE
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3727 2024-04-19 13:26:41.791183 feature_store_utils-0.0.4/PKG-INFO
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3195 2023-05-29 18:30:36.000000 feature_store_utils-0.0.4/README.md
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2024-04-19 13:26:41.790779 feature_store_utils-0.0.4/feature_store_utils.egg-info/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3727 2024-04-19 13:26:41.000000 feature_store_utils-0.0.4/feature_store_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      561 2024-04-19 13:26:41.000000 feature_store_utils-0.0.4/feature_store_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)        1 2024-04-19 13:26:41.000000 feature_store_utils-0.0.4/feature_store_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)       59 2024-04-19 13:26:41.000000 feature_store_utils-0.0.4/feature_store_utils.egg-info/requires.txt
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)        9 2024-04-19 13:26:41.000000 feature_store_utils-0.0.4/feature_store_utils.egg-info/top_level.txt
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2024-04-19 13:26:41.787184 feature_store_utils-0.0.4/features/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)        0 2023-02-13 15:10:53.000000 feature_store_utils-0.0.4/features/__init__.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     5807 2023-05-22 13:30:53.000000 feature_store_utils-0.0.4/features/feature_generation.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1730 2023-05-22 13:30:53.000000 feature_store_utils-0.0.4/features/feature_spec.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1341 2023-02-13 15:10:53.000000 feature_store_utils-0.0.4/features/hyper_feature.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1774 2024-04-19 11:45:05.000000 feature_store_utils-0.0.4/features/sql_gen.py
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2024-04-19 13:26:41.790175 feature_store_utils-0.0.4/features/templates/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1340 2024-04-19 13:02:59.000000 feature_store_utils-0.0.4/features/templates/fact_aggregations.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     2656 2023-02-13 15:10:53.000000 feature_store_utils-0.0.4/features/templates/timeseries_growth.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1721 2023-02-13 15:10:53.000000 feature_store_utils-0.0.4/features/templates/timeseries_growth_m.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      526 2023-02-13 15:10:53.000000 feature_store_utils-0.0.4/features/templates/type1_lookup.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      708 2023-02-13 15:10:53.000000 feature_store_utils-0.0.4/features/templates/type2_lookup.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      653 2024-04-19 13:26:32.000000 feature_store_utils-0.0.4/pyproject.toml
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)       38 2024-04-19 13:26:41.791582 feature_store_utils-0.0.4/setup.cfg
```

### Comparing `feature_store_utils-0.0.3/LICENSE` & `feature_store_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/PKG-INFO` & `feature_store_utils-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: feature_store_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A utility to generate ML features from yaml
 Author-email: Example Author <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
+Requires-Dist: databricks-feature-store
+Requires-Dist: Jinja2
+Requires-Dist: pandas
+Requires-Dist: pyaml
 
 # feature store utils
 
 A light-weight package that allows you express ML features in simple yaml, build a training data set and then write them to a feature store. 
 
 
 ### some general thoughts on building a training dataset
```

### Comparing `feature_store_utils-0.0.3/README.md` & `feature_store_utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/feature_store_utils.egg-info/PKG-INFO` & `feature_store_utils-0.0.4/feature_store_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
-Name: feature-store-utils
-Version: 0.0.3
+Name: feature_store_utils
+Version: 0.0.4
 Summary: A utility to generate ML features from yaml
 Author-email: Example Author <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
+Requires-Dist: databricks-feature-store
+Requires-Dist: Jinja2
+Requires-Dist: pandas
+Requires-Dist: pyaml
 
 # feature store utils
 
 A light-weight package that allows you express ML features in simple yaml, build a training data set and then write them to a feature store. 
 
 
 ### some general thoughts on building a training dataset
```

### Comparing `feature_store_utils-0.0.3/feature_store_utils.egg-info/SOURCES.txt` & `feature_store_utils-0.0.4/feature_store_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/features/feature_generation.py` & `feature_store_utils-0.0.4/features/feature_generation.py`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/features/feature_spec.py` & `feature_store_utils-0.0.4/features/feature_spec.py`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/features/hyper_feature.py` & `feature_store_utils-0.0.4/features/hyper_feature.py`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/features/sql_gen.py` & `feature_store_utils-0.0.4/features/sql_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 def get_query_template(feature, table):
     if feature['type'] == 'time_series_aggregate':
         template = environment.get_template("timeseries_growth.j2")
     elif feature['type'] == 'lookup' and table['type'] == 'dimension_type2':
         template = environment.get_template("type2_lookup.j2")
     elif feature['type'] == 'lookup' and table['type'] == 'dimension_type1':
         template = environment.get_template("type1_lookup.j2")
-    
     elif feature['type'] == 'fact_aggregate':
         template = environment.get_template("fact_aggregations.j2")
  
     return template
 
 
 def get_sql_for_feature(feature_name, eo_table=None):
```

### Comparing `feature_store_utils-0.0.3/features/templates/fact_aggregations.j2` & `feature_store_utils-0.0.4/features/templates/fact_aggregations.j2`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% macro fact_agg_time_window(eol_table, table, feature) -%}
 {% if feature.offset is defined %}
 {{table.source_table_name}}.{{table.date}} <= dateadd({{feature.offset.grain}}, -{{feature.offset.length}},{{eol_table.name}}.{{eol_table.observation_date.name}}) and
-{{table.source_table_name}}.{{table.date}} > dateadd({{feature.offset.grain}},-{{feature.offset.length}}, dateadd({{feature.grain}}, -{feature.window_length}}))
+{{table.source_table_name}}.{{table.date}} > dateadd({{feature.offset.grain}},-{{feature.offset.length}}, dateadd({{feature.grain}}, -{{feature.window_length}}))
 {% else %}
 {{table.source_table_name}}.{{table.date}} <= {{eol_table.name}}.{{eol_table.observation_date.name}} and
 {{table.source_table_name}}.{{table.date}} > dateadd({{feature.grain}}, -{{feature.window_length}}, {{eol_table.name}}.{{eol_table.observation_date.name}})
 {% endif %}
 {%- endmacro -%}
 
 select {{eol_table.name}}.{{eol_table.entity.name}}, {{eol_table.name}}.{{eol_table.observation_date.name}}, {{feature.function}}({{feature.source_col}}) as {{feature.name}}
```

### Comparing `feature_store_utils-0.0.3/features/templates/timeseries_growth.j2` & `feature_store_utils-0.0.4/features/templates/timeseries_growth.j2`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/features/templates/timeseries_growth_m.j2` & `feature_store_utils-0.0.4/features/templates/timeseries_growth_m.j2`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/features/templates/type1_lookup.j2` & `feature_store_utils-0.0.4/features/templates/type1_lookup.j2`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/features/templates/type2_lookup.j2` & `feature_store_utils-0.0.4/features/templates/type2_lookup.j2`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.3/pyproject.toml` & `feature_store_utils-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feature_store_utils"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A utility to generate ML features from yaml"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

