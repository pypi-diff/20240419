# Comparing `tmp/texta-elastic-tools-1.5.0.tar.gz` & `tmp/texta-elastic-tools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/texta-elastic-tools-1.5.0.tar", last modified: Wed Apr 26 14:25:20 2023, max compression
+gzip compressed data, was "dist/texta-elastic-tools-1.6.0.tar", last modified: Fri Apr 19 13:38:33 2024, max compression
```

## Comparing `texta-elastic-tools-1.5.0.tar` & `texta-elastic-tools-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    35062 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      570 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 14:25:09.000000 texta-elastic-tools-1.5.0/texta_elastic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11251 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/aggregator.py
--rw-rw-rw-   0 root         (0) root         (0)    21412 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)    14298 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/document.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/enums.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5637 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/mapping_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/mapping_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/query.py
--rw-rw-rw-   0 root         (0) root         (0)    17928 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/searcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-04-26 14:24:11.000000 texta-elastic-tools-1.5.0/texta_elastic/spam_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      570 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 14:25:20.000000 texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35062 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      570 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/texta_elastic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 13:37:58.000000 texta-elastic-tools-1.6.0/texta_elastic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11251 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/aggregator.py
+-rw-rw-rw-   0 root         (0) root         (0)    21412 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)    14298 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5637 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/mapping_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/mapping_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/query.py
+-rw-rw-rw-   0 root         (0) root         (0)    17965 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/searcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2024-04-19 13:13:45.000000 texta-elastic-tools-1.6.0/texta_elastic/spam_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      570 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      618 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-19 13:38:33.000000 texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/top_level.txt
```

### Comparing `texta-elastic-tools-1.5.0/LICENSE` & `texta-elastic-tools-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/PKG-INFO` & `texta-elastic-tools-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-elastic-tools
-Version: 1.5.0
+Version: 1.6.0
 Summary: TEXTA Elasticsearch tools
 Home-page: https://git.texta.ee/texta/texta-elastic-tools-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `texta-elastic-tools-1.5.0/setup.py` & `texta-elastic-tools-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/aggregator.py` & `texta-elastic-tools-1.6.0/texta_elastic/aggregator.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/core.py` & `texta-elastic-tools-1.6.0/texta_elastic/core.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/decorators.py` & `texta-elastic-tools-1.6.0/texta_elastic/decorators.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/document.py` & `texta-elastic-tools-1.6.0/texta_elastic/document.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/exceptions.py` & `texta-elastic-tools-1.6.0/texta_elastic/exceptions.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/mapping_generator.py` & `texta-elastic-tools-1.6.0/texta_elastic/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/mapping_tools.py` & `texta-elastic-tools-1.6.0/texta_elastic/mapping_tools.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/query.py` & `texta-elastic-tools-1.6.0/texta_elastic/query.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/searcher.py` & `texta-elastic-tools-1.6.0/texta_elastic/searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,18 +211,17 @@
     def count(self) -> int:
         try:
             count = self.core.es.count(index=self.indices, body=self.query)
             return count["count"]
         except elasticsearch.NotFoundError:
             return 0
 
-    def search(self, size=10):
+    def search(self, size=10, source_fields=True, disable_with_meta=True):
         # by default return all fields
-        source_fields = True
-        if self.output == self.OUT_META:
+        if self.output == self.OUT_META and disable_with_meta:
             source_fields = False
         # In case size/from is included in query in pagination, don't overwrite it by passing the size parameter
         if 'size' in self.query:
             response = self.core.es.search(index=self.indices, body=self.query, timeout=self.timeout, _source=source_fields)
         else:
             response = self.core.es.search(index=self.indices, body=self.query, size=size, timeout=self.timeout, _source=source_fields)
         if self.output == self.OUT_DOC:
```

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/settings.py` & `texta-elastic-tools-1.6.0/texta_elastic/settings.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic/spam_detector.py` & `texta-elastic-tools-1.6.0/texta_elastic/spam_detector.py`

 * *Files identical despite different names*

### Comparing `texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/PKG-INFO` & `texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-elastic-tools
-Version: 1.5.0
+Version: 1.6.0
 Summary: TEXTA Elasticsearch tools
 Home-page: https://git.texta.ee/texta/texta-elastic-tools-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `texta-elastic-tools-1.5.0/texta_elastic_tools.egg-info/SOURCES.txt` & `texta-elastic-tools-1.6.0/texta_elastic_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

