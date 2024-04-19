# Comparing `tmp/risclog.sqlalchemy-7.1.tar.gz` & `tmp/risclog.sqlalchemy-7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risclog.sqlalchemy-7.1.tar", last modified: Fri Mar 22 09:40:35 2024, max compression
+gzip compressed data, was "risclog.sqlalchemy-7.2.tar", last modified: Fri Apr 19 07:00:43 2024, max compression
```

## Comparing `risclog.sqlalchemy-7.1.tar` & `risclog.sqlalchemy-7.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.870005 risclog.sqlalchemy-7.1/
--rw-r--r--   0 sweh       (501) staff       (20)     7828 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/CHANGES.rst
--rw-r--r--   0 sweh       (501) staff       (20)      443 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/COPYRIGHT.rst
--rw-r--r--   0 sweh       (501) staff       (20)      967 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/HACKING.rst
--rw-r--r--   0 sweh       (501) staff       (20)     2070 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/LICENSE.txt
--rw-r--r--   0 sweh       (501) staff       (20)    11023 2024-03-22 09:40:35.869902 risclog.sqlalchemy-7.1/PKG-INFO
--rw-r--r--   0 sweh       (501) staff       (20)      384 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/README.rst
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.866191 risclog.sqlalchemy-7.1/doc/
--rw-r--r--   0 sweh       (501) staff       (20)      100 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/doc/about.txt
--rw-r--r--   0 sweh       (501) staff       (20)     7114 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/doc/api.txt
--rw-r--r--   0 sweh       (501) staff       (20)       28 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/doc/changes.txt
--rw-r--r--   0 sweh       (501) staff       (20)      717 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/doc/conf.py
--rw-r--r--   0 sweh       (501) staff       (20)      109 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/doc/index.txt
--rw-r--r--   0 sweh       (501) staff       (20)     1085 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/pyproject.toml
--rw-r--r--   0 sweh       (501) staff       (20)      174 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/requirements.txt
--rw-r--r--   0 sweh       (501) staff       (20)      316 2024-03-22 09:40:35.870208 risclog.sqlalchemy-7.1/setup.cfg
--rw-r--r--   0 sweh       (501) staff       (20)     2391 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/setup.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.864088 risclog.sqlalchemy-7.1/src/
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.866318 risclog.sqlalchemy-7.1/src/risclog/
--rw-r--r--   0 sweh       (501) staff       (20)       76 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/__init__.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.868134 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/
--rw-r--r--   0 sweh       (501) staff       (20)      133 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/__init__.py
--rw-r--r--   0 sweh       (501) staff       (20)    18422 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/cache.py
--rw-r--r--   0 sweh       (501) staff       (20)    13856 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/db.py
--rw-r--r--   0 sweh       (501) staff       (20)      585 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/fixtures.py
--rw-r--r--   0 sweh       (501) staff       (20)      232 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/functions.py
--rw-r--r--   0 sweh       (501) staff       (20)     1097 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/interfaces.py
--rw-r--r--   0 sweh       (501) staff       (20)     3461 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/model.py
--rw-r--r--   0 sweh       (501) staff       (20)     1849 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/serializer.py
--rw-r--r--   0 sweh       (501) staff       (20)     3988 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/testing.py
--rw-r--r--   0 sweh       (501) staff       (20)     1051 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/testlayer.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.868864 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/
--rw-r--r--   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/__init__.py
--rw-r--r--   0 sweh       (501) staff       (20)     2008 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/conftest.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.864379 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/fixtures/
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.869060 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/fixtures/alembic/
--rw-r--r--   0 sweh       (501) staff       (20)     1892 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/fixtures/alembic/env.py
--rw-r--r--   0 sweh       (501) staff       (20)      412 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/fixtures/alembic/script.py.mako
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.869185 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/fixtures/alembic/versions/
--rw-r--r--   0 sweh       (501) staff       (20)      374 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/fixtures/alembic/versions/3f735078d5a8_foo.py
--rw-r--r--   0 sweh       (501) staff       (20)     7959 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_cache.py
--rw-r--r--   0 sweh       (501) staff       (20)     6759 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_db.py
--rw-r--r--   0 sweh       (501) staff       (20)      948 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_fixtures.py
--rw-r--r--   0 sweh       (501) staff       (20)      666 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_model.py
--rw-r--r--   0 sweh       (501) staff       (20)     1584 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_serializer.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-03-22 09:40:35.869347 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/
--rw-r--r--   0 sweh       (501) staff       (20)    11023 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 sweh       (501) staff       (20)     1366 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 sweh       (501) staff       (20)        1 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 sweh       (501) staff       (20)        8 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 sweh       (501) staff       (20)        1 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 sweh       (501) staff       (20)      192 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 sweh       (501) staff       (20)        8 2024-03-22 09:40:35.000000 risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/top_level.txt
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.599974 risclog.sqlalchemy-7.2/
+-rw-r--r--   0 sweh       (501) staff       (20)     7913 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/CHANGES.rst
+-rw-r--r--   0 sweh       (501) staff       (20)      443 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/COPYRIGHT.rst
+-rw-r--r--   0 sweh       (501) staff       (20)      967 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/HACKING.rst
+-rw-r--r--   0 sweh       (501) staff       (20)     2070 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/LICENSE.txt
+-rw-r--r--   0 sweh       (501) staff       (20)    11108 2024-04-19 07:00:43.599874 risclog.sqlalchemy-7.2/PKG-INFO
+-rw-r--r--   0 sweh       (501) staff       (20)      384 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/README.rst
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.595752 risclog.sqlalchemy-7.2/doc/
+-rw-r--r--   0 sweh       (501) staff       (20)      100 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/doc/about.txt
+-rw-r--r--   0 sweh       (501) staff       (20)     7114 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/doc/api.txt
+-rw-r--r--   0 sweh       (501) staff       (20)       28 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/doc/changes.txt
+-rw-r--r--   0 sweh       (501) staff       (20)      717 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/doc/conf.py
+-rw-r--r--   0 sweh       (501) staff       (20)      109 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/doc/index.txt
+-rw-r--r--   0 sweh       (501) staff       (20)     1085 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/pyproject.toml
+-rw-r--r--   0 sweh       (501) staff       (20)      174 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/requirements.txt
+-rw-r--r--   0 sweh       (501) staff       (20)      316 2024-04-19 07:00:43.600212 risclog.sqlalchemy-7.2/setup.cfg
+-rw-r--r--   0 sweh       (501) staff       (20)     2391 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/setup.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.593848 risclog.sqlalchemy-7.2/src/
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.595848 risclog.sqlalchemy-7.2/src/risclog/
+-rw-r--r--   0 sweh       (501) staff       (20)       76 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/__init__.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.597987 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/
+-rw-r--r--   0 sweh       (501) staff       (20)      133 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/__init__.py
+-rw-r--r--   0 sweh       (501) staff       (20)    18422 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/cache.py
+-rw-r--r--   0 sweh       (501) staff       (20)    13856 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/db.py
+-rw-r--r--   0 sweh       (501) staff       (20)      585 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/fixtures.py
+-rw-r--r--   0 sweh       (501) staff       (20)      232 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/functions.py
+-rw-r--r--   0 sweh       (501) staff       (20)     1097 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/interfaces.py
+-rw-r--r--   0 sweh       (501) staff       (20)     3461 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/model.py
+-rw-r--r--   0 sweh       (501) staff       (20)     1885 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/serializer.py
+-rw-r--r--   0 sweh       (501) staff       (20)     3988 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/testing.py
+-rw-r--r--   0 sweh       (501) staff       (20)     1051 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/testlayer.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.598820 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/
+-rw-r--r--   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/__init__.py
+-rw-r--r--   0 sweh       (501) staff       (20)     2008 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/conftest.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.594117 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/fixtures/
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.599073 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/fixtures/alembic/
+-rw-r--r--   0 sweh       (501) staff       (20)     1892 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/fixtures/alembic/env.py
+-rw-r--r--   0 sweh       (501) staff       (20)      412 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/fixtures/alembic/script.py.mako
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.599206 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/fixtures/alembic/versions/
+-rw-r--r--   0 sweh       (501) staff       (20)      374 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/fixtures/alembic/versions/3f735078d5a8_foo.py
+-rw-r--r--   0 sweh       (501) staff       (20)     7959 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_cache.py
+-rw-r--r--   0 sweh       (501) staff       (20)     6759 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_db.py
+-rw-r--r--   0 sweh       (501) staff       (20)      948 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_fixtures.py
+-rw-r--r--   0 sweh       (501) staff       (20)      666 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_model.py
+-rw-r--r--   0 sweh       (501) staff       (20)     1584 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_serializer.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2024-04-19 07:00:43.599375 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/
+-rw-r--r--   0 sweh       (501) staff       (20)    11108 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 sweh       (501) staff       (20)     1366 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 sweh       (501) staff       (20)        1 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 sweh       (501) staff       (20)        8 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 sweh       (501) staff       (20)        1 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 sweh       (501) staff       (20)      192 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 sweh       (501) staff       (20)        8 2024-04-19 07:00:43.000000 risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/top_level.txt
```

### Comparing `risclog.sqlalchemy-7.1/CHANGES.rst` & `risclog.sqlalchemy-7.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =================================
 Change log for risclog.sqlalchemy
 =================================
 
+7.2 (2024-04-19)
+================
+
+- Add json encoder for `datetime.time` objects.
+
+
 7.1 (2024-03-22)
 ================
 
 - Fix `sqlalchemy` 1.3 compatibility in `Database.empty()`.
 
 
 7.0 (2024-03-21)
```

### Comparing `risclog.sqlalchemy-7.1/HACKING.rst` & `risclog.sqlalchemy-7.2/HACKING.rst`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/LICENSE.txt` & `risclog.sqlalchemy-7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/PKG-INFO` & `risclog.sqlalchemy-7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risclog.sqlalchemy
-Version: 7.1
+Version: 7.2
 Summary: Encapsulate sqlalchemy modelling infrastructure.
 Home-page: https://github.com/gocept/risclog.sqlalchemy
 Author: gocept <mail@gocept.com>
 Author-email: mail@gocept.com
 License: ZPL 2.1
 Keywords: sqlalchemy alembic model infrastructure utility
 Classifier: Development Status :: 5 - Production/Stable
@@ -102,14 +102,20 @@
     $ python setup.py upload_sphinx
 
 
 =================================
 Change log for risclog.sqlalchemy
 =================================
 
+7.2 (2024-04-19)
+================
+
+- Add json encoder for `datetime.time` objects.
+
+
 7.1 (2024-03-22)
 ================
 
 - Fix `sqlalchemy` 1.3 compatibility in `Database.empty()`.
 
 
 7.0 (2024-03-21)
```

### Comparing `risclog.sqlalchemy-7.1/doc/api.txt` & `risclog.sqlalchemy-7.2/doc/api.txt`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/doc/conf.py` & `risclog.sqlalchemy-7.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/pyproject.toml` & `risclog.sqlalchemy-7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/setup.py` & `risclog.sqlalchemy-7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import glob
 
 from setuptools import find_packages, setup
 
 setup(
     name='risclog.sqlalchemy',
-    version='7.1',
+    version='7.2',
     python_requires='>=3.7',
     install_requires=[
         'SQLAlchemy >= 1.0, < 2',
         'alembic >= 0.7',
         'pytz',
         'setuptools',
         'transaction',
```

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/cache.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/cache.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/db.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/db.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/fixtures.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/fixtures.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/interfaces.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/interfaces.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/model.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/serializer.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     return str(o)
 
 
 ENCODERS = {
     ObjectBase: sqlalchemy_encode,
     datetime.date: datetime_encode,
     datetime.datetime: datetime_encode,
+    datetime.time: datetime_encode,
     decimal.Decimal: decimal_encode,
     uuid.UUID: uuid_encode,
 }
 
 
 def encode(o):
     for klass, encoder in ENCODERS.items():
```

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/testing.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/testing.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/testlayer.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/testlayer.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/conftest.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/fixtures/alembic/env.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/fixtures/alembic/env.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_cache.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_db.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_fixtures.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_model.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog/sqlalchemy/tests/test_serializer.py` & `risclog.sqlalchemy-7.2/src/risclog/sqlalchemy/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/PKG-INFO` & `risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risclog.sqlalchemy
-Version: 7.1
+Version: 7.2
 Summary: Encapsulate sqlalchemy modelling infrastructure.
 Home-page: https://github.com/gocept/risclog.sqlalchemy
 Author: gocept <mail@gocept.com>
 Author-email: mail@gocept.com
 License: ZPL 2.1
 Keywords: sqlalchemy alembic model infrastructure utility
 Classifier: Development Status :: 5 - Production/Stable
@@ -102,14 +102,20 @@
     $ python setup.py upload_sphinx
 
 
 =================================
 Change log for risclog.sqlalchemy
 =================================
 
+7.2 (2024-04-19)
+================
+
+- Add json encoder for `datetime.time` objects.
+
+
 7.1 (2024-03-22)
 ================
 
 - Fix `sqlalchemy` 1.3 compatibility in `Database.empty()`.
 
 
 7.0 (2024-03-21)
```

### Comparing `risclog.sqlalchemy-7.1/src/risclog.sqlalchemy.egg-info/SOURCES.txt` & `risclog.sqlalchemy-7.2/src/risclog.sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

