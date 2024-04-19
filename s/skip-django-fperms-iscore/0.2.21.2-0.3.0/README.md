# Comparing `tmp/skip-django-fperms-iscore-0.2.21.2.tar.gz` & `tmp/skip_django_fperms_iscore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-fperms-iscore-0.2.21.2.tar", last modified: Thu Jan 19 15:59:35 2023, max compression
+gzip compressed data, was "skip_django_fperms_iscore-0.3.0.tar", last modified: Fri Apr 19 10:48:04 2024, max compression
```

## Comparing `skip-django-fperms-iscore-0.2.21.2.tar` & `skip_django_fperms_iscore-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.569140 skip-django-fperms-iscore-0.2.21.2/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-01-19 15:59:35.569140 skip-django-fperms-iscore-0.2.21.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.565140 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.565140 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.565140 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.569140 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.569140 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.569140 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/management/commands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/fperms_iscore/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-01-19 15:59:35.569140 skip-django-fperms-iscore-0.2.21.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2407 2023-01-19 15:59:12.000000 skip-django-fperms-iscore-0.2.21.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:59:35.569140 skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-01-19 15:59:35.000000 skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-19 15:59:35.000000 skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 15:59:35.000000 skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 15:59:35.000000 skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-19 15:59:35.000000 skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-19 15:59:35.000000 skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/fperms_iscore/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.411938 skip_django_fperms_iscore-0.3.0/fperms_iscore/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.411938 skip_django_fperms_iscore-0.3.0/fperms_iscore/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/fperms_iscore/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/fperms_iscore/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/fperms_iscore/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/management/commands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/fperms_iscore/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2426 2024-04-19 10:48:01.000000 skip_django_fperms_iscore-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:48:04.415938 skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-19 10:48:04.000000 skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 10:48:04.000000 skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:48:04.000000 skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:48:04.000000 skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 10:48:04.000000 skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 10:48:04.000000 skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/top_level.txt
```

### Comparing `skip-django-fperms-iscore-0.2.21.2/CONTRIBUTING.rst` & `skip_django_fperms_iscore-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-iscore-0.2.21.2/LICENSE` & `skip_django_fperms_iscore-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-iscore-0.2.21.2/PKG-INFO` & `skip_django_fperms_iscore-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: skip-django-fperms-iscore
-Version: 0.2.21.2
+Version: 0.3.0
 Summary: Perms for iscore library 
 Home-page: https://github.com/skip-pay/django-fperms-iscore
-Download-URL: https://github.com/skip-pay/django-fperms-iscore/archive/0.2.21.2.tar.gz
+Download-URL: https://github.com/skip-pay/django-fperms-iscore/archive/0.3.0.tar.gz
 Author: Petr Olah
 Author-email: djangoguru@gmail.com
 License: MIT
 Keywords: django-fperms-iscore
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
@@ -16,14 +16,17 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django>=4.2
+Requires-Dist: skip-django-fperms>=0.5.0
+Requires-Dist: skip-django-is-core>=2.25.0
 
 =============================
 django-fperms-iscore
 =============================
 
 .. image:: https://badge.fury.io/py/django-fperms-iscore.svg
     :target: https://badge.fury.io/py/django-fperms-iscore
```

### Comparing `skip-django-fperms-iscore-0.2.21.2/README.rst` & `skip_django_fperms_iscore-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-iscore-0.2.21.2/fperms_iscore/conf.py` & `skip_django_fperms_iscore-0.3.0/fperms_iscore/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-iscore-0.2.21.2/fperms_iscore/forms.py` & `skip_django_fperms_iscore-0.3.0/fperms_iscore/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.core.exceptions import ValidationError
-from django.utils.translation import ugettext
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext
+from django.utils.translation import gettext_lazy as _
 
 from fperms.conf import settings as fperms_settings
 from fperms.models import Group, Perm
 
 from is_core.forms.models import SmartModelForm, ModelMultipleChoiceField
 
 
@@ -67,13 +67,13 @@
 
     fgroups = ModelMultipleChoiceField(label=_('subgroups'), queryset=Group.objects.all(), required=False)
 
     def clean_fgroups(self):
         fgroups = self.cleaned_data['fgroups']
 
         if self.instance.pk in get_all_group_pks(fgroups):
-            raise ValidationError(ugettext('Cycles are not allowed'))
+            raise ValidationError(gettext('Cycles are not allowed'))
 
         if get_group_level(self.instance, fgroups) > fperms_settings.PERM_GROUP_MAX_LEVEL:
-            raise ValidationError(ugettext('Max group level was reached'))
+            raise ValidationError(gettext('Max group level was reached'))
 
         return fgroups
```

### Comparing `skip-django-fperms-iscore-0.2.21.2/fperms_iscore/locale/cs/LC_MESSAGES/django.mo` & `skip_django_fperms_iscore-0.3.0/fperms_iscore/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-iscore-0.2.21.2/fperms_iscore/locale/cs/LC_MESSAGES/django.po` & `skip_django_fperms_iscore-0.3.0/fperms_iscore/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-iscore-0.2.21.2/fperms_iscore/management/commands/sync_permissions.py` & `skip_django_fperms_iscore-0.3.0/fperms_iscore/management/commands/sync_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.core.management.base import BaseCommand
 from django.db.models import F, Value
 from django.db.models.functions import Concat
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from chamber.shortcuts import get_object_or_none
 from chamber.utils.decorators import translation_activate_block
 
 from fperms import get_perm_model
 
 from fperms_iscore import enums
@@ -69,13 +69,13 @@
             nonexistent_used_permissions_qs.delete()
             self.stdout.write(' Removed: {}'.format(count))
         elif nonexistent_used_permissions_qs.exists():
             self.stderr.write(
                 f'Found used obsolete permissions ({nonexistent_used_permissions_qs.count()}), '
                 f'run command with "--clean-obsolete" parameter for cleaning'
             )
-            obsolete_string = ugettext(' (obsolete)')
+            obsolete_string = gettext(' (obsolete)')
             nonexistent_used_permissions_qs.exclude(
                 name__endswith=obsolete_string
             ).update(
                 name=Concat(F('name'), Value(obsolete_string))
             )
```

### Comparing `skip-django-fperms-iscore-0.2.21.2/fperms_iscore/mixins.py` & `skip_django_fperms_iscore-0.3.0/fperms_iscore/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from .permissions import FPermPermission
 
 
 class PermCoreMixin:
 
     default_permission_classes = ()
```

### Comparing `skip-django-fperms-iscore-0.2.21.2/fperms_iscore/permissions.py` & `skip_django_fperms_iscore-0.3.0/fperms_iscore/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-iscore-0.2.21.2/setup.py` & `skip_django_fperms_iscore-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,17 @@
     url='https://github.com/skip-pay/django-fperms-iscore',
     download_url='https://github.com/skip-pay/django-fperms-iscore/archive/{}.tar.gz'.format(version),
     packages=[
         'fperms_iscore',
     ],
     include_package_data=True,
     install_requires=[
-        "skip-django-fperms>=0.4.8.3",
-        "skip-django-is-core>=2.24.6.2",
+        "django>=4.2",
+        "skip-django-fperms>=0.5.0",
+        "skip-django-is-core>=2.25.0",
     ],
     license="MIT",
     zip_safe=False,
     keywords='django-fperms-iscore',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
```

### Comparing `skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/PKG-INFO` & `skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: skip-django-fperms-iscore
-Version: 0.2.21.2
+Version: 0.3.0
 Summary: Perms for iscore library 
 Home-page: https://github.com/skip-pay/django-fperms-iscore
-Download-URL: https://github.com/skip-pay/django-fperms-iscore/archive/0.2.21.2.tar.gz
+Download-URL: https://github.com/skip-pay/django-fperms-iscore/archive/0.3.0.tar.gz
 Author: Petr Olah
 Author-email: djangoguru@gmail.com
 License: MIT
 Keywords: django-fperms-iscore
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
@@ -16,14 +16,17 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django>=4.2
+Requires-Dist: skip-django-fperms>=0.5.0
+Requires-Dist: skip-django-is-core>=2.25.0
 
 =============================
 django-fperms-iscore
 =============================
 
 .. image:: https://badge.fury.io/py/django-fperms-iscore.svg
     :target: https://badge.fury.io/py/django-fperms-iscore
```

### Comparing `skip-django-fperms-iscore-0.2.21.2/skip_django_fperms_iscore.egg-info/SOURCES.txt` & `skip_django_fperms_iscore-0.3.0/skip_django_fperms_iscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

