# Comparing `tmp/django_field_logger-0.0.29.tar.gz` & `tmp/django_field_logger-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_field_logger-0.0.29.tar", last modified: Wed Apr 17 23:58:34 2024, max compression
+gzip compressed data, was "django_field_logger-0.0.30.tar", last modified: Fri Apr 19 05:01:06 2024, max compression
```

## Comparing `django_field_logger-0.0.29.tar` & `django_field_logger-0.0.30.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:58:34.099747 django_field_logger-0.0.29/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django_field_logger-0.0.29/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django_field_logger-0.0.29/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)    10187 2024-04-17 23:58:34.099747 django_field_logger-0.0.29/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7952 2024-04-17 23:57:43.000000 django_field_logger-0.0.29/README.rst
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:58:34.099747 django_field_logger-0.0.29/django_field_logger.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)    10187 2024-04-17 23:58:34.000000 django_field_logger-0.0.29/django_field_logger.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      554 2024-04-17 23:58:34.000000 django_field_logger-0.0.29/django_field_logger.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-17 23:58:34.000000 django_field_logger-0.0.29/django_field_logger.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-17 23:58:34.000000 django_field_logger-0.0.29/django_field_logger.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-17 23:58:34.000000 django_field_logger-0.0.29/django_field_logger.egg-info/top_level.txt
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:58:34.099747 django_field_logger-0.0.29/fieldlogger/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:51.000000 django_field_logger-0.0.29/fieldlogger/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-04-12 05:21:51.000000 django_field_logger-0.0.29/fieldlogger/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2213 2024-04-17 05:22:00.000000 django_field_logger-0.0.29/fieldlogger/config.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1385 2024-04-14 05:50:25.000000 django_field_logger-0.0.29/fieldlogger/encoding.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      969 2024-04-14 05:37:12.000000 django_field_logger-0.0.29/fieldlogger/fieldlogger.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-04-12 05:21:51.000000 django_field_logger-0.0.29/fieldlogger/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2816 2024-04-14 05:50:03.000000 django_field_logger-0.0.29/fieldlogger/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1665 2024-04-17 22:45:35.000000 django_field_logger-0.0.29/fieldlogger/signals.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      381 2024-04-14 05:36:16.000000 django_field_logger-0.0.29/fieldlogger/utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      497 2024-04-12 04:14:01.000000 django_field_logger-0.0.29/pyproject.toml
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1136 2024-04-17 23:58:34.099747 django_field_logger-0.0.29/setup.cfg
--rwxr-xr-x   0 nibblex   (1000) nibblex   (1000)       96 2024-04-12 04:05:44.000000 django_field_logger-0.0.29/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-17 23:58:34.099747 django_field_logger-0.0.29/tests/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:35.000000 django_field_logger-0.0.29/tests/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1630 2024-04-17 23:36:16.000000 django_field_logger-0.0.29/tests/settings.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3993 2024-04-17 22:08:59.000000 django_field_logger-0.0.29/tests/test_utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2105 2024-04-17 23:06:39.000000 django_field_logger-0.0.29/tests/tests.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-19 05:01:06.928158 django_field_logger-0.0.30/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django_field_logger-0.0.30/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django_field_logger-0.0.30/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)    10365 2024-04-19 05:01:06.928158 django_field_logger-0.0.30/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7952 2024-04-17 23:57:43.000000 django_field_logger-0.0.30/README.rst
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-19 05:01:06.928158 django_field_logger-0.0.30/django_field_logger.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)    10365 2024-04-19 05:01:06.000000 django_field_logger-0.0.30/django_field_logger.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      518 2024-04-19 05:01:06.000000 django_field_logger-0.0.30/django_field_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-19 05:01:06.000000 django_field_logger-0.0.30/django_field_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-19 05:01:06.000000 django_field_logger-0.0.30/django_field_logger.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-19 05:01:06.000000 django_field_logger-0.0.30/django_field_logger.egg-info/top_level.txt
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-19 05:01:06.928158 django_field_logger-0.0.30/fieldlogger/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:51.000000 django_field_logger-0.0.30/fieldlogger/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-04-12 05:21:51.000000 django_field_logger-0.0.30/fieldlogger/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2213 2024-04-17 05:22:00.000000 django_field_logger-0.0.30/fieldlogger/config.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1385 2024-04-14 05:50:25.000000 django_field_logger-0.0.30/fieldlogger/encoding.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      969 2024-04-14 05:37:12.000000 django_field_logger-0.0.30/fieldlogger/fieldlogger.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-04-12 05:21:51.000000 django_field_logger-0.0.30/fieldlogger/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2816 2024-04-14 05:50:03.000000 django_field_logger-0.0.30/fieldlogger/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1665 2024-04-17 22:45:35.000000 django_field_logger-0.0.30/fieldlogger/signals.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      381 2024-04-14 05:36:16.000000 django_field_logger-0.0.30/fieldlogger/utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      497 2024-04-12 04:14:01.000000 django_field_logger-0.0.30/pyproject.toml
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1270 2024-04-19 05:01:06.928158 django_field_logger-0.0.30/setup.cfg
+-rwxr-xr-x   0 nibblex   (1000) nibblex   (1000)       96 2024-04-12 04:05:44.000000 django_field_logger-0.0.30/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-19 05:01:06.928158 django_field_logger-0.0.30/tests/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3993 2024-04-18 22:37:13.000000 django_field_logger-0.0.30/tests/test_utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2105 2024-04-17 23:06:39.000000 django_field_logger-0.0.30/tests/tests.py
```

### Comparing `django_field_logger-0.0.29/LICENSE` & `django_field_logger-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/PKG-INFO` & `django_field_logger-0.0.30/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.29
+Version: 0.0.30
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: Django>=4.0
+Requires-Dist: Django>=3.1
 
 Django Field Logger
 ===================
 
 A Django app for logging changes in model fields.
 
 How to set up?
```

### Comparing `django_field_logger-0.0.29/README.rst` & `django_field_logger-0.0.30/README.rst`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/django_field_logger.egg-info/PKG-INFO` & `django_field_logger-0.0.30/django_field_logger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.29
+Version: 0.0.30
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: Django>=4.0
+Requires-Dist: Django>=3.1
 
 Django Field Logger
 ===================
 
 A Django app for logging changes in model fields.
 
 How to set up?
```

### Comparing `django_field_logger-0.0.29/django_field_logger.egg-info/SOURCES.txt` & `django_field_logger-0.0.30/django_field_logger.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,11 +14,9 @@
 fieldlogger/config.py
 fieldlogger/encoding.py
 fieldlogger/fieldlogger.py
 fieldlogger/mixins.py
 fieldlogger/models.py
 fieldlogger/signals.py
 fieldlogger/utils.py
-tests/__init__.py
-tests/settings.py
 tests/test_utils.py
 tests/tests.py
```

### Comparing `django_field_logger-0.0.29/fieldlogger/config.py` & `django_field_logger-0.0.30/fieldlogger/config.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/fieldlogger/encoding.py` & `django_field_logger-0.0.30/fieldlogger/encoding.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/fieldlogger/fieldlogger.py` & `django_field_logger-0.0.30/fieldlogger/fieldlogger.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/fieldlogger/models.py` & `django_field_logger-0.0.30/fieldlogger/models.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/fieldlogger/signals.py` & `django_field_logger-0.0.30/fieldlogger/signals.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/setup.cfg` & `django_field_logger-0.0.30/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 [metadata]
 name = django-field-logger
-version = 0.0.29
+version = 0.0.30
 description = A Django app for logging changes in model fields.
 long_description = file: README.rst, LICENSE
 author = Sergio Rodríguez
 author_email = srodriguez3441@gmail.com
 maintainer = Sergio Rodríguez
 maintainer_email = srodriguez3441@gmail.com
 url = https://github.com/nibblex/django-field-logger
 classifiers = 
 	Framework :: Django
+	Framework :: Django :: 3.1
+	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
 	Framework :: Django :: 5.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3.13
 	Topic :: Software Development :: Libraries :: Python Modules
 license = MIT
 
 [options]
 include_package_data = True
-python_requires = >=3.8
+python_requires = >=3.6
 setup_requires = 
 	setuptools>=42
 install_requires = 
-	Django>=4.0
+	Django>=3.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django_field_logger-0.0.29/tests/test_utils.py` & `django_field_logger-0.0.30/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_field_logger-0.0.29/tests/tests.py` & `django_field_logger-0.0.30/tests/tests.py`

 * *Files identical despite different names*

