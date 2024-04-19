# Comparing `tmp/skip-django-generic-m2m-field-0.0.9.3.tar.gz` & `tmp/skip_django_generic_m2m_field-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-generic-m2m-field-0.0.9.3.tar", last modified: Thu Jan 12 15:53:22 2023, max compression
+gzip compressed data, was "skip_django_generic_m2m_field-0.1.0.tar", last modified: Fri Apr 19 10:15:39 2024, max compression
```

## Comparing `skip-django-generic-m2m-field-0.0.9.3.tar` & `skip_django_generic_m2m_field-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.590285 skip-django-generic-m2m-field-0.0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-01-12 15:53:22.590285 skip-django-generic-m2m-field-0.0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.586285 skip-django-generic-m2m-field-0.0.9.3/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.586285 skip-django-generic-m2m-field-0.0.9.3/example/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.586285 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.586285 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/0002_auto_20201007_1210.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/0003_auto_20210604_1406.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.586285 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/apps/app/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.590285 skip-django-generic-m2m-field-0.0.9.3/example/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/example/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.590285 skip-django-generic-m2m-field-0.0.9.3/generic_m2m_field/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/generic_m2m_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/generic_m2m_field/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 15:53:22.590285 skip-django-generic-m2m-field-0.0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-01-12 15:53:04.000000 skip-django-generic-m2m-field-0.0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:53:22.590285 skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-01-12 15:53:22.000000 skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-12 15:53:22.000000 skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:53:22.000000 skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:53:22.000000 skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-12 15:53:22.000000 skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-12 15:53:22.000000 skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.165616 skip_django_generic_m2m_field-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 10:15:39.165616 skip_django_generic_m2m_field-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/example/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/example/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/0002_auto_20201007_1210.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/0003_auto_20210604_1406.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/example/apps/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/apps/app/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      330 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/example/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/example/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/generic_m2m_field/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/generic_m2m_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/generic_m2m_field/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:15:39.165616 skip_django_generic_m2m_field-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-19 10:15:35.000000 skip_django_generic_m2m_field-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:15:39.161616 skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 10:15:39.000000 skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-19 10:15:39.000000 skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:15:39.000000 skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:15:39.000000 skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 10:15:39.000000 skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 10:15:39.000000 skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/top_level.txt
```

### Comparing `skip-django-generic-m2m-field-0.0.9.3/LICENSE` & `skip_django_generic_m2m_field-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/PKG-INFO` & `skip_django_generic_m2m_field-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-generic-m2m-field
-Version: 0.0.9.3
+Version: 0.1.0
 Summary: Django generic many to many field library.
 Home-page: https://github.com/skip-pay/django-generic-m2m-field
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,fields,generic
 Classifier: Development Status :: 3 - Alpha
@@ -15,7 +15,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 License-File: LICENSE
+Requires-Dist: django>=4.2.0
+Requires-Dist: skip-django-chamber>=0.7.2
```

### Comparing `skip-django-generic-m2m-field-0.0.9.3/README.md` & `skip_django_generic_m2m_field-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/0001_initial.py` & `skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/0002_auto_20201007_1210.py` & `skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/0002_auto_20201007_1210.py`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/example/apps/app/migrations/0003_auto_20210604_1406.py` & `skip_django_generic_m2m_field-0.1.0/example/apps/app/migrations/0003_auto_20210604_1406.py`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/example/apps/app/models.py` & `skip_django_generic_m2m_field-0.1.0/example/apps/app/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/example/apps/app/tests/__init__.py` & `skip_django_generic_m2m_field-0.1.0/example/apps/app/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/example/settings/base.py` & `skip_django_generic_m2m_field-0.1.0/example/settings/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/example/wsgi.py` & `skip_django_generic_m2m_field-0.1.0/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-generic-m2m-field-0.0.9.3/generic_m2m_field/models.py` & `skip_django_generic_m2m_field-0.1.0/generic_m2m_field/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from types import MethodType
 
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.db.models.functions import Cast
 from django.utils.functional import cached_property
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from chamber.models import SmartModel, SmartQuerySet
 from chamber.shortcuts import get_object_or_none
 
 
 def camel_to_snake(name):
   name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
```

### Comparing `skip-django-generic-m2m-field-0.0.9.3/setup.py` & `skip_django_generic_m2m_field-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='skip-django-generic-m2m-field',
-    version='0.0.9.3',
+    version='0.1.0',
     description="Django generic many to many field library.",
     keywords='django, fields, generic',
     author='Lubos Matl',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/django-generic-m2m-field',
     license='MIT',
     package_dir={'generic_m2m_field': 'generic_m2m_field'},
@@ -23,12 +23,12 @@
         'Natural Language :: Czech',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Internet :: WWW/HTTP :: Site Management',
     ],
     install_requires=[
-        'django>=2.2.9, <4.0',
-        'skip-django-chamber>=0.6.16.3'
+        'django>=4.2.0',
+        'skip-django-chamber>=0.7.2'
     ],
     zip_safe=False
 )
```

### Comparing `skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/PKG-INFO` & `skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-generic-m2m-field
-Version: 0.0.9.3
+Version: 0.1.0
 Summary: Django generic many to many field library.
 Home-page: https://github.com/skip-pay/django-generic-m2m-field
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,fields,generic
 Classifier: Development Status :: 3 - Alpha
@@ -15,7 +15,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 License-File: LICENSE
+Requires-Dist: django>=4.2.0
+Requires-Dist: skip-django-chamber>=0.7.2
```

### Comparing `skip-django-generic-m2m-field-0.0.9.3/skip_django_generic_m2m_field.egg-info/SOURCES.txt` & `skip_django_generic_m2m_field-0.1.0/skip_django_generic_m2m_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

