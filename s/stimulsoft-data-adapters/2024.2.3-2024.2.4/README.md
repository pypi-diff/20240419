# Comparing `tmp/stimulsoft_data_adapters-2024.2.3.tar.gz` & `tmp/stimulsoft_data_adapters-2024.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimulsoft_data_adapters-2024.2.3.tar", last modified: Tue Apr  2 07:47:42 2024, max compression
+gzip compressed data, was "stimulsoft_data_adapters-2024.2.4.tar", last modified: Thu Apr 18 09:32:47 2024, max compression
```

## Comparing `stimulsoft_data_adapters-2024.2.3.tar` & `stimulsoft_data_adapters-2024.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:42.098706 stimulsoft_data_adapters-2024.2.3/
--rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_data_adapters-2024.2.3/LICENSE.md
--rw-rw-rw-   0        0        0     9937 2024-04-02 07:47:42.097967 stimulsoft_data_adapters-2024.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     9130 2024-03-07 13:34:04.000000 stimulsoft_data_adapters-2024.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 07:47:42.098706 stimulsoft_data_adapters-2024.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1209 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:42.082207 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/
--rw-rw-rw-   0        0        0     8777 2023-10-30 12:58:46.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiDataAdapter.py
--rw-rw-rw-   0        0        0     2153 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiFirebirdAdapter.py
--rw-rw-rw-   0        0        0     4725 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiMongoDbAdapter.py
--rw-rw-rw-   0        0        0     3805 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiMsSqlAdapter.py
--rw-rw-rw-   0        0        0     3087 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiMySqlAdapter.py
--rw-rw-rw-   0        0        0     1124 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiOdbcAdapter.py
--rw-rw-rw-   0        0        0     4247 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiOracleAdapter.py
--rw-rw-rw-   0        0        0     2735 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiPostgreSqlAdapter.py
--rw-rw-rw-   0        0        0      204 2023-11-14 15:52:08.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:42.082207 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/
--rw-rw-rw-   0        0        0     8906 2024-03-27 13:55:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseHandler.py
--rw-rw-rw-   0        0        0     2090 2023-11-06 18:22:33.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseRequest.py
--rw-rw-rw-   0        0        0     3454 2024-02-26 13:30:18.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseResponse.py
--rw-rw-rw-   0        0        0      883 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseResult.py
--rw-rw-rw-   0        0        0      336 2023-09-22 14:50:49.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiConnectionInfo.py
--rw-rw-rw-   0        0        0     1368 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiDataResult.py
--rw-rw-rw-   0        0        0      786 2023-10-30 12:49:14.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiParameter.py
--rw-rw-rw-   0        0        0        0 2023-09-29 07:52:43.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:42.082207 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/enums/
--rw-rw-rw-   0        0        0      282 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/enums/StiDataCommand.py
--rw-rw-rw-   0        0        0      456 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/enums/StiDatabaseType.py
--rw-rw-rw-   0        0        0      175 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/enums/StiFrameworkType.py
--rw-rw-rw-   0        0        0       88 2023-11-16 09:48:40.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:42.097225 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/
--rw-rw-rw-   0        0        0     1074 2023-10-30 12:47:41.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/StiDataEventArgs.py
--rw-rw-rw-   0        0        0     1651 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/StiEvent.py
--rw-rw-rw-   0        0        0      585 2023-10-20 09:23:17.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/StiEventArgs.py
--rw-rw-rw-   0        0        0       46 2023-11-14 15:52:07.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 07:47:42.082207 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/
--rw-rw-rw-   0        0        0     9937 2024-04-02 07:47:41.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1449 2024-04-02 07:47:41.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 07:47:41.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-02 07:47:41.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-02 07:47:41.000000 stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:47.752364 stimulsoft_data_adapters-2024.2.4/
+-rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_data_adapters-2024.2.4/LICENSE.md
+-rw-rw-rw-   0        0        0     9937 2024-04-18 09:32:47.752364 stimulsoft_data_adapters-2024.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9130 2024-03-07 13:34:04.000000 stimulsoft_data_adapters-2024.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 09:32:47.752364 stimulsoft_data_adapters-2024.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:47.710402 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/
+-rw-rw-rw-   0        0        0     8777 2023-10-30 12:58:46.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiDataAdapter.py
+-rw-rw-rw-   0        0        0     2153 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiFirebirdAdapter.py
+-rw-rw-rw-   0        0        0     4725 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiMongoDbAdapter.py
+-rw-rw-rw-   0        0        0     3805 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiMsSqlAdapter.py
+-rw-rw-rw-   0        0        0     3087 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiMySqlAdapter.py
+-rw-rw-rw-   0        0        0     1124 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiOdbcAdapter.py
+-rw-rw-rw-   0        0        0     4247 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiOracleAdapter.py
+-rw-rw-rw-   0        0        0     2735 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiPostgreSqlAdapter.py
+-rw-rw-rw-   0        0        0      204 2023-11-14 15:52:08.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:47.714768 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/
+-rw-rw-rw-   0        0        0     9170 2024-04-16 11:07:52.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseHandler.py
+-rw-rw-rw-   0        0        0     2102 2024-04-10 08:33:54.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseRequest.py
+-rw-rw-rw-   0        0        0     3454 2024-02-26 13:30:18.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseResponse.py
+-rw-rw-rw-   0        0        0      883 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseResult.py
+-rw-rw-rw-   0        0        0      336 2023-09-22 14:50:49.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiConnectionInfo.py
+-rw-rw-rw-   0        0        0     1368 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiDataResult.py
+-rw-rw-rw-   0        0        0      786 2023-10-30 12:49:14.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiParameter.py
+-rw-rw-rw-   0        0        0        0 2023-09-29 07:52:43.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:47.715966 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/enums/
+-rw-rw-rw-   0        0        0      282 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/enums/StiDataCommand.py
+-rw-rw-rw-   0        0        0      456 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/enums/StiDatabaseType.py
+-rw-rw-rw-   0        0        0      175 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/enums/StiFrameworkType.py
+-rw-rw-rw-   0        0        0       88 2023-11-16 09:48:40.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:47.751364 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/
+-rw-rw-rw-   0        0        0     1074 2023-10-30 12:47:41.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/StiDataEventArgs.py
+-rw-rw-rw-   0        0        0     1651 2023-10-30 08:59:56.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/StiEvent.py
+-rw-rw-rw-   0        0        0      585 2023-10-20 09:23:17.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/StiEventArgs.py
+-rw-rw-rw-   0        0        0       46 2023-11-14 15:52:07.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:47.711401 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/
+-rw-rw-rw-   0        0        0     9937 2024-04-18 09:32:47.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1449 2024-04-18 09:32:47.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 09:32:47.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-18 09:32:47.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-18 09:32:47.000000 stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/top_level.txt
```

### Comparing `stimulsoft_data_adapters-2024.2.3/LICENSE.md` & `stimulsoft_data_adapters-2024.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/PKG-INFO` & `stimulsoft_data_adapters-2024.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft_data_adapters
-Version: 2024.2.3
+Version: 2024.2.4
 Summary: Stimulsoft data adapters for Python.
 Home-page: https://www.stimulsoft.com/en/products/reports-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_data_adapters-2024.2.3/README.md` & `stimulsoft_data_adapters-2024.2.4/README.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/setup.py` & `stimulsoft_data_adapters-2024.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readmeFile = file.read()
 
 with open('REQUIREMENTS.txt') as file:
     requiresFile = [text.strip() for text in file if text.strip()]
 
 setup(
     name = 'stimulsoft_data_adapters',
-    version = '2024.2.3',
+    version = '2024.2.4',
     author = 'Stimulsoft',
     author_email = 'info@stimulsoft.com',
     description = 'Stimulsoft data adapters for Python.',
     long_description = readmeFile,
     long_description_content_type = 'text/markdown',
     url = 'https://www.stimulsoft.com/en/products/reports-python',
     license = 'https://www.stimulsoft.com/en/licensing/developers',
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiDataAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiDataAdapter.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiFirebirdAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiFirebirdAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiFirebirdAdapter(StiDataAdapter):
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkVersion: bool = True
 
     def getOdbcConnectionString(self):
         connectionString: str = \
             f'Driver={self.connectionInfo.driver};' \
             f'Dbname={self.connectionInfo.host}/{self.connectionInfo.port}:{self.connectionInfo.database};' \
             f'Uid={self.connectionInfo.userId};' \
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiMongoDbAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiMongoDbAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from urllib.parse import urlparse
 
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiMongoDbAdapter(StiDataAdapter):
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkVersion: bool = True
 
     def connect(self):
         try:
             from pymongo import MongoClient
             self.connectionLink = MongoClient(self.connectionString)
         except Exception as e:
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiMsSqlAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiMsSqlAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from uuid import UUID
 
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiMsSqlAdapter(StiDataAdapter):
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkVersion: bool = True
     trustServerCertificate: str = None
     integratedSecurity: str = None
 
     def getOdbcConnectionString(self):
         connectionString: str = \
             f'Driver={self.connectionInfo.driver};' \
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiMySqlAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiMySqlAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .classes.StiDataResult import StiDataResult
 from .classes.StiBaseResult import StiBaseResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiMySqlAdapter(StiDataAdapter):
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkVersion: bool = True
     
     def connect(self):
         if self.connectionInfo.driver:
             return self.connectOdbc()
         
         if not self.connectionInfo.charset:
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiOdbcAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiOdbcAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pyodbc import Connection
 
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiOdbcAdapter(StiDataAdapter):
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkVersion: bool = True
     connectionLink: Connection
 
     def connect(self):
         try:
             self.connectionLink = pyodbc.connect(self.connectionString)
             if self.connectionInfo.charset:
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiOracleAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiOracleAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiOracleAdapter(StiDataAdapter):
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkVersion: bool = True
 
     def getOdbcConnectionString(self):
         connectionString: str = \
             f'Driver={self.connectionInfo.driver};' \
             f'Dbq={self.connectionInfo.database};' \
             f'Uid={self.connectionInfo.userId};' \
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/StiPostgreSqlAdapter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/StiPostgreSqlAdapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .classes.StiDataResult import StiDataResult
 from .StiDataAdapter import StiDataAdapter
 
 
 class StiPostgreSqlAdapter(StiDataAdapter):
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkVersion: bool = True
 
     def connect(self):
         if self.connectionInfo.driver:
             return self.connectOdbc()
         
         if not self.connectionInfo.charset:
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseHandler.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class StiBaseHandler:
     """
     Event handler for all requests from the report generator. 
     The incoming request is processed, a data adapter is created and all necessary actions are performed.
     """
 
-    version: str = '2024.2.3'
+    version: str = '2024.2.4'
     checkDataAdaptersVersion: bool = True
     framework: str = StiFrameworkType.DEFAULT
     origin: str = None
     query: dict = None
     body: str = None
     error: str = None
     request: StiBaseRequest = None
@@ -66,42 +66,46 @@
             if isinstance(request, DjangoRequest):
                 self.__setQuery(request.GET)
                 self.__setBody(request.body)
                 self.origin = '{0}://{1}'.format(request.scheme, request.get_host())
                 self.framework = StiFrameworkType.DJANGO
                 return True
         except Exception as e:
-            self.error = 'Request: ' + str(e)
-            return False
+            if not isinstance(e, ModuleNotFoundError):
+                self.error = 'Request: ' + str(e)
+                return False
 
         try:
             from flask import Request as FlaskRequest
             if isinstance(request, FlaskRequest):
                 self.__setQuery(request.args.to_dict())
                 self.__setBody(request.get_data(False))
                 self.origin = request.origin
                 self.framework = StiFrameworkType.FLASK
                 return True
         except Exception as e:
-            self.error = 'Request: ' + str(e)
-            return False
+            if not isinstance(e, ModuleNotFoundError):
+                self.error = 'Request: ' + str(e)
+                return False
 
         try:
             from tornado.httputil import HTTPServerRequest as TornadoRequest
             if isinstance(request, TornadoRequest):
                 self.__setQuery(request.query)
                 self.__setBody(request.body)
                 self.origin = '{0}://{1}'.format(request.protocol, request.host)
                 self.framework = StiFrameworkType.TORNADO
                 return True
         except Exception as e:
-            self.error = 'Request: ' + str(e)
-            return False
+            if not isinstance(e, ModuleNotFoundError):
+                self.error = 'Request: ' + str(e)
+                return False
         
-        return True
+        self.error = 'Unsupported request: ' + str(request.__class__)
+        return False
 
     def __getSupportedDataAdaptersResult(self) -> StiBaseResult:
         result = StiBaseResult.getSuccess()
         result.types = StiDatabaseType.getTypes()
         result.handlerVersion = self.version
         return result
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseRequest.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,18 +36,18 @@
     def _setField(self, name, value):
         setattr(self, name, value)
 
 
 ### Public
 
     def process(self, query: dict, body: str) -> bool:
-        if len(query) > 0:
+        if len(query or '') > 0:
             self.__populateVars(query, True)
 
-        if len(body) > 0:
+        if len(body or '') > 0:
             if body[0] != '{':
                 try:
                     body = codecs.decode(body, 'rot_13')
                     body = codecs.decode(body.encode(), 'base64').decode()
                 except Exception as e:
                     self.error = 'Base64: ' + str(e)
                     return False
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseResponse.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseResponse.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiBaseResult.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiBaseResult.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiDataResult.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiDataResult.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/classes/StiParameter.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/classes/StiParameter.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/StiDataEventArgs.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/StiDataEventArgs.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/StiEvent.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/StiEvent.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters/events/StiEventArgs.py` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters/events/StiEventArgs.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/PKG-INFO` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft-data-adapters
-Version: 2024.2.3
+Version: 2024.2.4
 Summary: Stimulsoft data adapters for Python.
 Home-page: https://www.stimulsoft.com/en/products/reports-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_data_adapters-2024.2.3/stimulsoft_data_adapters.egg-info/SOURCES.txt` & `stimulsoft_data_adapters-2024.2.4/stimulsoft_data_adapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

