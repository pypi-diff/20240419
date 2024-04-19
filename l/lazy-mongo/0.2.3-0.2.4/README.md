# Comparing `tmp/lazy_mongo-0.2.3.tar.gz` & `tmp/lazy_mongo-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_mongo-0.2.3.tar", max compression
+gzip compressed data, was "lazy_mongo-0.2.4.tar", max compression
```

## Comparing `lazy_mongo-0.2.3.tar` & `lazy_mongo-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.2.3/README.md
--rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.2.3/lazy_mongo/__init__.py
--rw-r--r--   0        0        0      265 2024-04-16 01:49:02.827730 lazy_mongo-0.2.3/lazy_mongo/insert_response.py
--rw-r--r--   0        0        0     2180 2024-04-16 01:50:16.611945 lazy_mongo-0.2.3/lazy_mongo/lazy_collection.py
--rw-r--r--   0        0        0     1818 2024-03-27 05:13:57.761621 lazy_mongo-0.2.3/lazy_mongo/lazy_database.py
--rw-r--r--   0        0        0     2406 2024-03-27 05:14:35.152714 lazy_mongo-0.2.3/lazy_mongo/lazy_mongo.py
--rw-r--r--   0        0        0      211 2024-04-16 01:49:06.275740 lazy_mongo-0.2.3/lazy_mongo/update_response.py
--rw-r--r--   0        0        0      296 2024-04-16 01:52:03.912265 lazy_mongo-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.2.4/README.md
+-rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.2.4/lazy_mongo/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-16 01:49:02.827730 lazy_mongo-0.2.4/lazy_mongo/insert_response.py
+-rw-r--r--   0        0        0     2180 2024-04-16 01:50:16.611945 lazy_mongo-0.2.4/lazy_mongo/lazy_collection.py
+-rw-r--r--   0        0        0     1818 2024-03-27 05:13:57.761621 lazy_mongo-0.2.4/lazy_mongo/lazy_database.py
+-rw-r--r--   0        0        0     2456 2024-04-19 04:05:17.074776 lazy_mongo-0.2.4/lazy_mongo/lazy_mongo.py
+-rw-r--r--   0        0        0      211 2024-04-16 01:49:06.275740 lazy_mongo-0.2.4/lazy_mongo/update_response.py
+-rw-r--r--   0        0        0      296 2024-04-19 04:05:26.666226 lazy_mongo-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.2.4/PKG-INFO
```

### Comparing `lazy_mongo-0.2.3/lazy_mongo/lazy_collection.py` & `lazy_mongo-0.2.4/lazy_mongo/lazy_collection.py`

 * *Files identical despite different names*

### Comparing `lazy_mongo-0.2.3/lazy_mongo/lazy_database.py` & `lazy_mongo-0.2.4/lazy_mongo/lazy_database.py`

 * *Files identical despite different names*

### Comparing `lazy_mongo-0.2.3/lazy_mongo/lazy_mongo.py` & `lazy_mongo-0.2.4/lazy_mongo/lazy_mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 class LazyMongo:
     def __init__(self):
         self.mongo: MongoClient = None  # type: ignore
         self.default_database: str = None  # type: ignore
         self.default_collection: str = None  # type: ignore
 
     def connect(self, uri: str):
-        self.mongo = MongoClient(uri)
+        try:
+            self.mongo = MongoClient(uri)
+        except:
+            pass
 
         return self
 
     def __getitem__(self, key: str):
         return LazyDatabase(
             database=self.mongo[key or self.default_database],
             default_collection_name=self.default_collection,
```

### Comparing `lazy_mongo-0.2.3/PKG-INFO` & `lazy_mongo-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-mongo
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

