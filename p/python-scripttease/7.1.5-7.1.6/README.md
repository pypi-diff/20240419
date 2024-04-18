# Comparing `tmp/python-scripttease-7.1.5.tar.gz` & `tmp/python-scripttease-7.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-scripttease-7.1.5.tar", last modified: Thu Apr 11 16:33:10 2024, max compression
+gzip compressed data, was "python-scripttease-7.1.6.tar", last modified: Thu Apr 18 23:53:05 2024, max compression
```

## Comparing `python-scripttease-7.1.5.tar` & `python-scripttease-7.1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/
--rw-r--r--   0 shawn     (1000) shawn     (1000)       87 2019-04-26 18:33:34.000000 python-scripttease-7.1.5/DESCRIPTION.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1516 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/LICENSE.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)      204 2020-09-02 16:16:51.000000 python-scripttease-7.1.5/MANIFEST.in
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1352 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/PKG-INFO
--rw-rw-r--   0 shawn     (1000) shawn     (1000)        5 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/VERSION.txt
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/python_scripttease.egg-info/
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1352 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/PKG-INFO
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     1164 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/SOURCES.txt
--rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/dependency_links.txt
--rw-rw-r--   0 shawn     (1000) shawn     (1000)       55 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/entry_points.txt
--rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/not-zip-safe
--rw-rw-r--   0 shawn     (1000) shawn     (1000)       67 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/requires.txt
--rw-rw-r--   0 shawn     (1000) shawn     (1000)       12 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/top_level.txt
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/
--rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2020-07-16 18:21:17.000000 python-scripttease-7.1.5/scripttease/__init__.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/cli/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     3573 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/cli/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     9590 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/cli/initialize.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5349 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/cli/subcommands.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)      402 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/constants.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)       84 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/exceptions.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/lib/
--rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/__init__.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/lib/commands/
--rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/__init__.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    25121 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/base.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     7431 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/centos.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5186 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/django.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     3874 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/messages.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     7386 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/mysql.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     9099 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/pgsql.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      281 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/php.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)    19745 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/posix.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2046 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/python.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     9009 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/ubuntu.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2028 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/contexts.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     4493 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/factories.py
-drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/lib/loaders/
--rw-r--r--   0 shawn     (1000) shawn     (1000)      177 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/loaders/__init__.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)     7723 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/loaders/base.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2919 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/loaders/ini.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2176 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/loaders/yaml.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      213 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/variables.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)       82 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/version.py
--rw-rw-r--   0 shawn     (1000) shawn     (1000)       38 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/setup.cfg
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2005 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/setup.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       87 2019-04-26 18:33:34.000000 python-scripttease-7.1.6/DESCRIPTION.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1516 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/LICENSE.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      204 2020-09-02 16:16:51.000000 python-scripttease-7.1.6/MANIFEST.in
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1352 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/PKG-INFO
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        5 2024-04-18 23:51:51.000000 python-scripttease-7.1.6/VERSION.txt
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/python_scripttease.egg-info/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1352 2024-04-18 23:53:05.000000 python-scripttease-7.1.6/python_scripttease.egg-info/PKG-INFO
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1164 2024-04-18 23:53:05.000000 python-scripttease-7.1.6/python_scripttease.egg-info/SOURCES.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2024-04-18 23:53:05.000000 python-scripttease-7.1.6/python_scripttease.egg-info/dependency_links.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       55 2024-04-18 23:53:05.000000 python-scripttease-7.1.6/python_scripttease.egg-info/entry_points.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2024-04-18 23:53:05.000000 python-scripttease-7.1.6/python_scripttease.egg-info/not-zip-safe
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       67 2024-04-18 23:53:05.000000 python-scripttease-7.1.6/python_scripttease.egg-info/requires.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       12 2024-04-18 23:53:05.000000 python-scripttease-7.1.6/python_scripttease.egg-info/top_level.txt
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/scripttease/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2020-07-16 18:21:17.000000 python-scripttease-7.1.6/scripttease/__init__.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/scripttease/cli/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     3573 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/cli/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9590 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/cli/initialize.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5349 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/cli/subcommands.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      402 2024-04-11 16:31:40.000000 python-scripttease-7.1.6/scripttease/constants.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       84 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/scripttease/exceptions.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/scripttease/lib/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/scripttease/lib/__init__.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/scripttease/lib/commands/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/scripttease/lib/commands/__init__.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    25121 2024-04-11 16:31:40.000000 python-scripttease-7.1.6/scripttease/lib/commands/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7431 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/lib/commands/centos.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5186 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/lib/commands/django.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     3874 2024-04-11 16:31:40.000000 python-scripttease-7.1.6/scripttease/lib/commands/messages.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7386 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/lib/commands/mysql.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     9134 2024-04-18 23:51:51.000000 python-scripttease-7.1.6/scripttease/lib/commands/pgsql.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      281 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/lib/commands/php.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    19745 2024-04-11 16:31:40.000000 python-scripttease-7.1.6/scripttease/lib/commands/posix.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2046 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/lib/commands/python.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9009 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/lib/commands/ubuntu.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2028 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/scripttease/lib/contexts.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     4493 2024-04-11 16:31:40.000000 python-scripttease-7.1.6/scripttease/lib/factories.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/scripttease/lib/loaders/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      177 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/scripttease/lib/loaders/__init__.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     7723 2024-04-11 16:31:40.000000 python-scripttease-7.1.6/scripttease/lib/loaders/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2919 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/scripttease/lib/loaders/ini.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2176 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/scripttease/lib/loaders/yaml.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      213 2023-04-04 14:50:40.000000 python-scripttease-7.1.6/scripttease/variables.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       82 2024-04-18 23:51:51.000000 python-scripttease-7.1.6/scripttease/version.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       38 2024-04-18 23:53:05.546684 python-scripttease-7.1.6/setup.cfg
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2005 2023-04-17 17:40:07.000000 python-scripttease-7.1.6/setup.py
```

### Comparing `python-scripttease-7.1.5/LICENSE.txt` & `python-scripttease-7.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/PKG-INFO` & `python-scripttease-7.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-scripttease
-Version: 7.1.5
+Version: 7.1.6
 Summary: A collection of classes and commands for automated command line scripting using Python.
 Home-page: https://develmaycare.com/products/python/scripttease/
 Download-URL: https://gittraction.com/diff6/python-scripttease
 Author: Shawn Davis
 Author-email: shawn@develmaycare.com
 Project-URL: Documentation, https://docs.diff6.com/en/python-scripttease/latest/
 Project-URL: Source, https://gittraction.com/diff6/python-scripttease
```

### Comparing `python-scripttease-7.1.5/python_scripttease.egg-info/PKG-INFO` & `python-scripttease-7.1.6/python_scripttease.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-scripttease
-Version: 7.1.5
+Version: 7.1.6
 Summary: A collection of classes and commands for automated command line scripting using Python.
 Home-page: https://develmaycare.com/products/python/scripttease/
 Download-URL: https://gittraction.com/diff6/python-scripttease
 Author: Shawn Davis
 Author-email: shawn@develmaycare.com
 Project-URL: Documentation, https://docs.diff6.com/en/python-scripttease/latest/
 Project-URL: Source, https://gittraction.com/diff6/python-scripttease
```

### Comparing `python-scripttease-7.1.5/python_scripttease.egg-info/SOURCES.txt` & `python-scripttease-7.1.6/python_scripttease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/cli/__init__.py` & `python-scripttease-7.1.6/scripttease/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/cli/initialize.py` & `python-scripttease-7.1.6/scripttease/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/cli/subcommands.py` & `python-scripttease-7.1.6/scripttease/cli/subcommands.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/base.py` & `python-scripttease-7.1.6/scripttease/lib/commands/base.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/centos.py` & `python-scripttease-7.1.6/scripttease/lib/commands/centos.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/django.py` & `python-scripttease-7.1.6/scripttease/lib/commands/django.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/messages.py` & `python-scripttease-7.1.6/scripttease/lib/commands/messages.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/mysql.py` & `python-scripttease-7.1.6/scripttease/lib/commands/mysql.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/pgsql.py` & `python-scripttease-7.1.6/scripttease/lib/commands/pgsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
             _kwargs[key] = kwargs.pop(key)
 
     # Postgres commands always run without sudo because the -U may be provided.
     _kwargs['sudo'] = False
 
     a = list()
 
-    if password is not None:
+    # Password may be None or an empty string.
+    if password:
         a.append('export PGPASSWORD="%s" &&' % password)
 
     a.append(command)
     a.append("-U %s --host=%s --port=%s" % (user, host, port))
     for key, value in kwargs.items():
         key = key.replace("_", "-")
         if type(value) is bool and value is True:
```

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/posix.py` & `python-scripttease-7.1.6/scripttease/lib/commands/posix.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/python.py` & `python-scripttease-7.1.6/scripttease/lib/commands/python.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/commands/ubuntu.py` & `python-scripttease-7.1.6/scripttease/lib/commands/ubuntu.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/contexts.py` & `python-scripttease-7.1.6/scripttease/lib/contexts.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/factories.py` & `python-scripttease-7.1.6/scripttease/lib/factories.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/loaders/base.py` & `python-scripttease-7.1.6/scripttease/lib/loaders/base.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/loaders/ini.py` & `python-scripttease-7.1.6/scripttease/lib/loaders/ini.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/scripttease/lib/loaders/yaml.py` & `python-scripttease-7.1.6/scripttease/lib/loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.1.5/setup.py` & `python-scripttease-7.1.6/setup.py`

 * *Files identical despite different names*

