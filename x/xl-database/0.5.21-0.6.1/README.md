# Comparing `tmp/xl_database-0.5.21.tar.gz` & `tmp/xl_database-0.6.1.tar.gz`

## Comparing `xl_database-0.5.21.tar` & `xl_database-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 xl_database-0.5.21/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 xl_database-0.5.21/src/zdatabase/mixins.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 xl_database-0.5.21/src/zdatabase/model.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 xl_database-0.5.21/src/zdatabase/utils/time.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 xl_database-0.5.21/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_database-0.5.21/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 xl_database-0.5.21/README.md
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 xl_database-0.5.21/pyproject.toml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 xl_database-0.5.21/PKG-INFO
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 xl_database-0.6.1/src/xl-database/__init__.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 xl_database-0.6.1/src/xl-database/mixins.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 xl_database-0.6.1/src/xl-database/model.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 xl_database-0.6.1/src/xl-database/utils/time.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 xl_database-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 xl_database-0.6.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_database-0.6.1/README.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 xl_database-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 xl_database-0.6.1/PKG-INFO
```

### Comparing `xl_database-0.5.21/src/zdatabase/mixins.py` & `xl_database-0.6.1/src/xl-database/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from zdatabase import db
+from xl_database import db
 from jsonschema import validate
 
 
 class DatabaseMixin:
     @staticmethod
     def flush():
         db.session.flush()
```

### Comparing `xl_database-0.5.21/src/zdatabase/model.py` & `xl_database-0.6.1/src/xl-database/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from zdatabase import db
-from zdatabase.mixins import DatabaseMixin, QueryMixin, MapperMixin
-from zdatabase.utils import time
+from xl_database import db
+from xl_database.mixins import DatabaseMixin, QueryMixin, MapperMixin
+from xl_database.utils import time
 
 
 class Model(DatabaseMixin, QueryMixin, MapperMixin, db.Model):
     __abstract__ = True
     __schema__ = {}
 
     @classmethod
```

### Comparing `xl_database-0.5.21/LICENSE` & `xl_database-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xl_database-0.5.21/pyproject.toml` & `xl_database-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xl-database"
-version = "0.5.21"
+version = "0.6.1"
 authors = [
   { name="xilong", email="xilonglab@163.com" },
 ]
 description = "xilong database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `xl_database-0.5.21/PKG-INFO` & `xl_database-0.6.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 Metadata-Version: 2.1
 Name: xl-database
-Version: 0.5.21
+Version: 0.6.1
 Summary: xilong database library
 Project-URL: Homepage, https://git.xilonglab.com/xilong/zdatabase
 Project-URL: Bug Tracker, https://git.xilonglab.com/xilong/zdatabase/issues
 Author-email: xilong <xilonglab@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: arrow==0.17.0
 Requires-Dist: flask-sqlalchemy==2.5.1
 Requires-Dist: jsonschema==4.17.3
 Requires-Dist: sqlalchemy==1.4.39
-Description-Content-Type: text/markdown
-
-# zdb
-
-Zen database library.
```

