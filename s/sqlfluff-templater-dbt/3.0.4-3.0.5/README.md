# Comparing `tmp/sqlfluff-templater-dbt-3.0.4.tar.gz` & `tmp/sqlfluff_templater_dbt-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff-templater-dbt-3.0.4.tar", last modified: Tue Apr  9 17:45:04 2024, max compression
+gzip compressed data, was "sqlfluff_templater_dbt-3.0.5.tar", last modified: Fri Apr 19 13:48:32 2024, max compression
```

## Comparing `sqlfluff-templater-dbt-3.0.4.tar` & `sqlfluff_templater_dbt-3.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.783415 sqlfluff-templater-dbt-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 17:44:55.000000 sqlfluff-templater-dbt-3.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-09 17:45:04.783415 sqlfluff-templater-dbt-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 17:44:55.000000 sqlfluff-templater-dbt-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-09 17:45:04.783415 sqlfluff-templater-dbt-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 17:44:55.000000 sqlfluff-templater-dbt-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.779415 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 17:44:55.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33153 2024-04-09 17:44:55.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.783415 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-09 17:45:04.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-09 17:45:04.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:45:04.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 17:45:04.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 17:45:04.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 17:45:04.000000 sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33153 2024-04-19 13:48:23.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:32.172606 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:48:32.000000 sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff-templater-dbt-3.0.4/LICENSE.md` & `sqlfluff_templater_dbt-3.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-3.0.4/PKG-INFO` & `sqlfluff_templater_dbt-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 3.0.4
+Version: 3.0.5
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: sqlfluff==3.0.4
+Requires-Dist: sqlfluff==3.0.5
 Requires-Dist: dbt-core>=1.0.0
 Requires-Dist: jinja2-simple-tags>=0.3.1
 Requires-Dist: markupsafe
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
```

### Comparing `sqlfluff-templater-dbt-3.0.4/setup.cfg` & `sqlfluff_templater_dbt-3.0.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 3.0.4
+version = 3.0.5
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -60,15 +60,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	sqlfluff==3.0.4
+	sqlfluff==3.0.5
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt/templater.py` & `sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt/templater.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-3.0.4/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff_templater_dbt-3.0.5/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 3.0.4
+Version: 3.0.5
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: sqlfluff==3.0.4
+Requires-Dist: sqlfluff==3.0.5
 Requires-Dist: dbt-core>=1.0.0
 Requires-Dist: jinja2-simple-tags>=0.3.1
 Requires-Dist: markupsafe
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: ruamel.yaml
```

