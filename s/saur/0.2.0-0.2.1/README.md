# Comparing `tmp/saur-0.2.0.tar.gz` & `tmp/saur-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saur-0.2.0.tar", last modified: Tue Apr 16 15:40:52 2024, max compression
+gzip compressed data, was "saur-0.2.1.tar", last modified: Fri Apr 19 14:08:42 2024, max compression
```

## Comparing `saur-0.2.0.tar` & `saur-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.718361 saur-0.2.0/
--rw-rw-r--   0 aition    (1000) aition    (1000)     3125 2023-08-17 19:01:43.000000 saur-0.2.0/.gitignore
--rw-rw-r--   0 aition    (1000) aition    (1000)    15215 2024-01-01 21:07:23.000000 saur-0.2.0/LICENSE.txt
--rw-r--r--   0 aition    (1000) aition    (1000)      853 2024-04-16 15:40:52.718361 saur-0.2.0/PKG-INFO
--rw-rw-r--   0 aition    (1000) aition    (1000)       82 2023-08-17 18:51:44.000000 saur-0.2.0/README.md
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.714361 saur-0.2.0/examples/
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.714361 saur-0.2.0/examples/fastapi/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:31:45.000000 saur-0.2.0/examples/fastapi/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      581 2023-08-17 19:05:39.000000 saur-0.2.0/examples/fastapi/app.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     4901 2024-04-05 18:38:16.000000 saur-0.2.0/examples/fastapi/auth.py
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 19:05:53.000000 saur-0.2.0/examples/fastapi/cli.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      885 2023-08-17 19:05:54.000000 saur-0.2.0/examples/fastapi/models.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1780 2023-08-17 19:05:56.000000 saur-0.2.0/examples/fastapi/routes.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      519 2023-08-17 19:05:57.000000 saur-0.2.0/examples/fastapi/schemas.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1227 2024-04-16 15:15:46.000000 saur-0.2.0/pyproject.toml
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.718361 saur-0.2.0/saur/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 16:44:45.000000 saur-0.2.0/saur/__init__.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.718361 saur-0.2.0/saur/app/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:27:09.000000 saur-0.2.0/saur/app/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2042 2024-03-13 22:25:15.000000 saur-0.2.0/saur/app/fastapi.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.718361 saur-0.2.0/saur/mixins/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-09-17 21:12:38.000000 saur-0.2.0/saur/mixins/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)      786 2024-04-04 22:15:42.000000 saur-0.2.0/saur/mixins/active.py
--rw-rw-r--   0 aition    (1000) aition    (1000)    13279 2024-04-05 01:27:20.000000 saur-0.2.0/saur/mixins/async_access.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     5469 2024-04-04 22:20:37.000000 saur-0.2.0/saur/mixins/watch.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     3886 2024-04-04 22:23:10.000000 saur-0.2.0/saur/settings.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.718361 saur-0.2.0/saur/types/
--rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 16:44:39.000000 saur-0.2.0/saur/types/__init__.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1414 2024-04-04 22:15:28.000000 saur-0.2.0/saur/types/delimited.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1976 2024-01-01 21:55:05.000000 saur-0.2.0/saur/types/hashid.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2541 2023-08-17 17:30:51.000000 saur-0.2.0/saur/types/numeric_datetime.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     1240 2024-03-20 01:44:04.000000 saur-0.2.0/saur/types/pydantic.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2430 2024-01-03 23:21:18.000000 saur-0.2.0/saur/types/relativedelta.py
--rw-rw-r--   0 aition    (1000) aition    (1000)     2194 2023-09-14 17:06:30.000000 saur-0.2.0/saur/types/uuid.py
--rw-rw-r--   0 aition    (1000) aition    (1000)       91 2024-04-04 22:40:37.000000 saur-0.2.0/saur/utils.py
-drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-16 15:40:52.718361 saur-0.2.0/saur.egg-info/
--rw-r--r--   0 aition    (1000) aition    (1000)      853 2024-04-16 15:40:52.000000 saur-0.2.0/saur.egg-info/PKG-INFO
--rw-rw-r--   0 aition    (1000) aition    (1000)      723 2024-04-16 15:40:52.000000 saur-0.2.0/saur.egg-info/SOURCES.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)        1 2024-04-16 15:40:52.000000 saur-0.2.0/saur.egg-info/dependency_links.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)       54 2024-04-16 15:40:52.000000 saur-0.2.0/saur.egg-info/requires.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)        5 2024-04-16 15:40:52.000000 saur-0.2.0/saur.egg-info/top_level.txt
--rw-rw-r--   0 aition    (1000) aition    (1000)       38 2024-04-16 15:40:52.718361 saur-0.2.0/setup.cfg
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.292301 saur-0.2.1/
+-rw-rw-r--   0 aition    (1000) aition    (1000)     3125 2023-08-17 19:01:43.000000 saur-0.2.1/.gitignore
+-rw-rw-r--   0 aition    (1000) aition    (1000)    15215 2024-01-01 21:07:23.000000 saur-0.2.1/LICENSE.txt
+-rw-r--r--   0 aition    (1000) aition    (1000)     1037 2024-04-19 14:08:42.292301 saur-0.2.1/PKG-INFO
+-rw-rw-r--   0 aition    (1000) aition    (1000)       82 2023-08-17 18:51:44.000000 saur-0.2.1/README.md
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/examples/
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/examples/fastapi/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:31:45.000000 saur-0.2.1/examples/fastapi/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      581 2023-08-17 19:05:39.000000 saur-0.2.1/examples/fastapi/app.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     4901 2024-04-05 18:38:16.000000 saur-0.2.1/examples/fastapi/auth.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 19:05:53.000000 saur-0.2.1/examples/fastapi/cli.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      885 2023-08-17 19:05:54.000000 saur-0.2.1/examples/fastapi/models.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1780 2023-08-17 19:05:56.000000 saur-0.2.1/examples/fastapi/routes.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      519 2023-08-17 19:05:57.000000 saur-0.2.1/examples/fastapi/schemas.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1397 2024-04-19 14:06:44.000000 saur-0.2.1/pyproject.toml
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 16:44:45.000000 saur-0.2.1/saur/__init__.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/app/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 17:27:09.000000 saur-0.2.1/saur/app/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2042 2024-03-13 22:25:15.000000 saur-0.2.1/saur/app/fastapi.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/mixins/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-09-17 21:12:38.000000 saur-0.2.1/saur/mixins/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)      786 2024-04-04 22:15:42.000000 saur-0.2.1/saur/mixins/active.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)    13279 2024-04-05 01:27:20.000000 saur-0.2.1/saur/mixins/async_access.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     5469 2024-04-04 22:20:37.000000 saur-0.2.1/saur/mixins/watch.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     3886 2024-04-04 22:23:10.000000 saur-0.2.1/saur/settings.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur/types/
+-rw-rw-r--   0 aition    (1000) aition    (1000)        0 2023-08-17 16:44:39.000000 saur-0.2.1/saur/types/__init__.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1414 2024-04-04 22:15:28.000000 saur-0.2.1/saur/types/delimited.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1976 2024-01-01 21:55:05.000000 saur-0.2.1/saur/types/hashid.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2541 2023-08-17 17:30:51.000000 saur-0.2.1/saur/types/numeric_datetime.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     1240 2024-03-20 01:44:04.000000 saur-0.2.1/saur/types/pydantic.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2430 2024-01-03 23:21:18.000000 saur-0.2.1/saur/types/relativedelta.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)     2194 2023-09-14 17:06:30.000000 saur-0.2.1/saur/types/uuid.py
+-rw-rw-r--   0 aition    (1000) aition    (1000)       91 2024-04-04 22:40:37.000000 saur-0.2.1/saur/utils.py
+drwxrwxr-x   0 aition    (1000) aition    (1000)        0 2024-04-19 14:08:42.288301 saur-0.2.1/saur.egg-info/
+-rw-r--r--   0 aition    (1000) aition    (1000)     1037 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/PKG-INFO
+-rw-rw-r--   0 aition    (1000) aition    (1000)      723 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/SOURCES.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)        1 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/dependency_links.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)       54 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/requires.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)        5 2024-04-19 14:08:42.000000 saur-0.2.1/saur.egg-info/top_level.txt
+-rw-rw-r--   0 aition    (1000) aition    (1000)       38 2024-04-19 14:08:42.292301 saur-0.2.1/setup.cfg
```

### Comparing `saur-0.2.0/.gitignore` & `saur-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/LICENSE.txt` & `saur-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/PKG-INFO` & `saur-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: saur
-Version: 0.2.0
+Version: 0.2.1
 Summary: SQL Alchemy Utilities Repository
 Author-email: Michael Tartre <quantology.org@gmail.com>
+Project-URL: Homepage, https://gitlab.com/sofet-dev/saur
+Project-URL: Repository, https://gitlab.com/sofet-dev/saur.git
+Project-URL: Issues, https://gitlab.com/sofet-dev/saur/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `saur-0.2.0/examples/fastapi/app.py` & `saur-0.2.1/examples/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/examples/fastapi/auth.py` & `saur-0.2.1/examples/fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/examples/fastapi/models.py` & `saur-0.2.1/examples/fastapi/models.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/examples/fastapi/routes.py` & `saur-0.2.1/examples/fastapi/routes.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/examples/fastapi/schemas.py` & `saur-0.2.1/examples/fastapi/schemas.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/pyproject.toml` & `saur-0.2.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saur"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name = "Michael Tartre", email = "quantology.org@gmail.com"},
 ]
 description = "SQL Alchemy Utilities Repository"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,14 +22,19 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "sqlalchemy>=2",
     "pydantic-settings>=2"
 ]
 
+[project.urls]
+Homepage = "https://gitlab.com/sofet-dev/saur"
+Repository = "https://gitlab.com/sofet-dev/saur.git"
+Issues = "https://gitlab.com/sofet-dev/saur/-/issues"
+
 [project.optional-dependencies]
 fastapi = ["fastapi"]
 
 [tool.ruff]
 line-length = 100
 
 [tool.ruff.lint]
```

### Comparing `saur-0.2.0/saur/app/fastapi.py` & `saur-0.2.1/saur/app/fastapi.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/mixins/active.py` & `saur-0.2.1/saur/mixins/active.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/mixins/async_access.py` & `saur-0.2.1/saur/mixins/async_access.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/mixins/watch.py` & `saur-0.2.1/saur/mixins/watch.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/settings.py` & `saur-0.2.1/saur/settings.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/types/delimited.py` & `saur-0.2.1/saur/types/delimited.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/types/hashid.py` & `saur-0.2.1/saur/types/hashid.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/types/numeric_datetime.py` & `saur-0.2.1/saur/types/numeric_datetime.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/types/pydantic.py` & `saur-0.2.1/saur/types/pydantic.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/types/relativedelta.py` & `saur-0.2.1/saur/types/relativedelta.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur/types/uuid.py` & `saur-0.2.1/saur/types/uuid.py`

 * *Files identical despite different names*

### Comparing `saur-0.2.0/saur.egg-info/PKG-INFO` & `saur-0.2.1/saur.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: saur
-Version: 0.2.0
+Version: 0.2.1
 Summary: SQL Alchemy Utilities Repository
 Author-email: Michael Tartre <quantology.org@gmail.com>
+Project-URL: Homepage, https://gitlab.com/sofet-dev/saur
+Project-URL: Repository, https://gitlab.com/sofet-dev/saur.git
+Project-URL: Issues, https://gitlab.com/sofet-dev/saur/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `saur-0.2.0/saur.egg-info/SOURCES.txt` & `saur-0.2.1/saur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

