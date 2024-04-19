# Comparing `tmp/django-flex-report-0.7.5.tar.gz` & `tmp/django-flex-report-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.7.5.tar", last modified: Thu Apr 18 15:55:53 2024, max compression
+gzip compressed data, was "django-flex-report-0.7.6.tar", last modified: Fri Apr 19 16:10:04 2024, max compression
```

## Comparing `django-flex-report-0.7.5.tar` & `django-flex-report-0.7.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 15:55:53.489635 django-flex-report-0.7.5/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.5/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.5/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 15:55:53.489635 django-flex-report-0.7.5/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 15:55:53.489635 django-flex-report-0.7.5/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 15:55:53.000000 django-flex-report-0.7.5/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-18 15:55:53.000000 django-flex-report-0.7.5/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 15:55:53.000000 django-flex-report-0.7.5/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 15:55:53.000000 django-flex-report-0.7.5/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-18 15:55:53.000000 django-flex-report-0.7.5/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-18 15:55:53.000000 django-flex-report-0.7.5/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 15:55:53.485635 django-flex-report-0.7.5/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1703 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-18 15:55:53.000000 django-flex-report-0.7.5/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3729 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 15:55:53.489635 django-flex-report-0.7.5/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0013_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0014_alter_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0015_remove_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/0016_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    13918 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 15:55:53.489635 django-flex-report-0.7.5/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    23695 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11192 2024-04-18 15:55:45.000000 django-flex-report-0.7.5/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.5/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.5/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-18 15:55:53.489635 django-flex-report-0.7.5/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.5/setup.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/LICENSE
+-rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/MANIFEST.in
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/PKG-INFO
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/django_flex_report.egg-info/
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/PKG-INFO
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/not-zip-safe
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/requires.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-19 16:10:04.000000 django-flex-report-0.7.6/django_flex_report.egg-info/top_level.txt
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/flex_report/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1703 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-19 16:10:03.000000 django-flex-report-0.7.6/flex_report/_version.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/admin.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/app_settings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/apps.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/choices.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3745 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/constants.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/fields.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/filterset.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/forms.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/managers.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/flex_report/migrations/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0001_initial.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0002_alter_column_title.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0004_column_creator.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0005_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0006_tablebutton_query_strings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0008_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0009_alter_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0011_alter_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0013_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0014_alter_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0015_remove_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/0016_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/migrations/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    14027 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/mixins.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/models.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/flex_report/templatetags/
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/templatetags/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/templatetags/flex_report_filters.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/urls.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    24121 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/utils.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    11771 2024-04-19 16:09:52.000000 django-flex-report-0.7.6/flex_report/views.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/pyproject.toml
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/requirements.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-19 16:10:04.185084 django-flex-report-0.7.6/setup.cfg
+-rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.6/setup.py
```

### Comparing `django-flex-report-0.7.5/LICENSE` & `django-flex-report-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/MANIFEST.in` & `django-flex-report-0.7.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/PKG-INFO` & `django-flex-report-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.5/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.7.6/django_flex_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.5/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.7.6/django_flex_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/__init__.py` & `django-flex-report-0.7.6/flex_report/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/admin.py` & `django-flex-report-0.7.6/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/app_settings.py` & `django-flex-report-0.7.6/flex_report/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/constants.py` & `django-flex-report-0.7.6/flex_report/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,16 @@
     @abstractmethod
     def format_name(cls):
         raise NotImplementedError
 
     @classmethod
     def register(cls, format_):
         assert issubclass(format_, BaseExportFormat)
-        return cls.formats.update({format_.format_slug: format_})
+        cls.formats.update({format_.format_slug: format_})
+        return format_
 
     @classmethod
     def register_formats(cls, formats: dict):
         cls.formats.update(formats)
 
     @abstractmethod
     def handle(cls):
```

### Comparing `django-flex-report-0.7.5/flex_report/fields.py` & `django-flex-report-0.7.6/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/filterset.py` & `django-flex-report-0.7.6/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/forms.py` & `django-flex-report-0.7.6/flex_report/forms.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0001_initial.py` & `django-flex-report-0.7.6/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.7.6/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.7.6/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.7.6/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.7.6/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.7.6/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.7.6/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.7.6/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.7.6/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0013_column_column_type.py` & `django-flex-report-0.7.6/flex_report/migrations/0013_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0014_alter_column_column_type.py` & `django-flex-report-0.7.6/flex_report/migrations/0014_alter_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/migrations/0016_column_column_type.py` & `django-flex-report-0.7.6/flex_report/migrations/0016_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/mixins.py` & `django-flex-report-0.7.6/flex_report/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 
 
 class QuerySetExportMixin(View):
     export_qs = []
     export_headers = {}
     export_columns = []
     export_kwargs = {}
+    export_filename = None
+    
+    def get_export_filename(self):
+        return self.export_filename
     
     def get_export_columns(self):
         return self.export_columns
     
     def get_export_headers(self):
         return self.export_headers
     
@@ -154,22 +158,22 @@
         
         return super().dispatch(*args, **kwargs)
     
     def get_exporter(self) -> BaseExportFormat:
         try:
             format_ = export_format.formats[self.export_format]
             if any(self.get_handle_qs().values()):
-                return type("DynamicExporter", (format_), self.get_handle_qs())(request=self.request, user=self.request.user)
+                return type("DynamicExporter", (format_,), self.get_handle_qs())(request=self.request, user=self.request.user)
             return format_(request=self.request, user=self.request.user)
         except KeyError as e:
             raise NotImplementedError(f"The wanted format '{self.export_format}' isn't handled.") from e
 
     def get(self, *args, **kwargs):
         format_ = self.get_exporter()
-        filename = format_.get_export_filename()
+        filename = str(format_.get_export_filename())
         
         response = HttpResponse(
             content_type=mimetypes.types_map.get(
                 f".{format_.format_ext}",
                 "application/octet-stream",
             ),
             headers={"Content-Disposition": f'attachment; filename="{filename}"'},
```

### Comparing `django-flex-report-0.7.5/flex_report/models.py` & `django-flex-report-0.7.6/flex_report/models.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.7.6/flex_report/templatetags/flex_report_filters.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.5/flex_report/urls.py` & `django-flex-report-0.7.6/flex_report/urls.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 VIEWS = app_settings.VIEWS
 
 
 app_name = "flex_report"
 template_urls = [
     path("", VIEWS["TEMPLATE_LIST"], name="index"),
-    path("export/", VIEWS["GENERAL_QS_EXPORT"], name="export"),
+    path("<int:pk>/export", VIEWS["REPORT_EXPORT"], name="export"),
     path(
         "new/",
         VIEWS["TEMPLATE_CREATE_INIT"],
         name="create",
     ),
     path(
         "new/<int:pk>/",
@@ -63,14 +63,14 @@
         view=VIEWS["COLUMN_DELETE"],
         name="delete",
     ),
 ]
 
 urlpatterns = [
     path("<int:pk>/", VIEWS["REPORT"], name="view"),
-    path("<int:pk>/export", VIEWS["REPORT_EXPORT"], name="export"),
+    path("export/", VIEWS["GENERAL_QS_EXPORT"], name="export"),
     path("columns/", include((column_urls, "column"), namespace="column")),
     path(
         "template/",
         include((template_urls, "template"), namespace="template"),
     ),
 ]
```

### Comparing `django-flex-report-0.7.5/flex_report/utils.py` & `django-flex-report-0.7.6/flex_report/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import contextlib
 import csv
 import datetime
 import io
 import json
 import re
+from django.utils.translation import override
 from collections import OrderedDict
 from decimal import Decimal
+from django.db.models import QuerySet
 from functools import lru_cache, reduce
 from importlib import import_module
 from itertools import chain
 from operator import attrgetter, methodcaller, and_, or_
 from typing import List
 from phonenumber_field.modelfields import PhoneNumberField
 import jdatetime
@@ -37,14 +39,15 @@
 from .app_settings import app_settings
 from .constants import (
     REPORT_CELL_STYLE_MAP,
     REPORT_CUSTOM_FIELDS_KEY,
     REPORT_EXCULDE_KEY,
     REPORT_FIELDS_KEY,
     FieldTypes,
+    DynamicSubField
 )
 
 
 logger = getLogger(__name__)
 
 
 def nested_getattr(obj, attr, *args, sep="."):
@@ -275,27 +278,26 @@
 
 
 def get_column_type(model, column):
     """
     takes in a model and a column name, and returns the column type.
     currently the possible types are: field, property, and custom.
     """
-    field = get_model_field(model, column)
+    if column in dynamic_field.fields:
+        return FieldTypes.dynamic
 
+    field = get_model_field(model, column)
     if field:
         return FieldTypes.field
 
     field = get_model_property(model, column)
 
     if isinstance(field, property):
         return FieldTypes.property
 
-    if field in dynamic_field.fields:
-        return FieldTypes.dynamic
-
     return None
 
 
 def get_fields_lookups(model, fields):
     """
     Takes in a model and a list of fields, and returns a dict where the keys are the field names,
     and the values are a list of lookup-expression used for them.
@@ -423,14 +425,18 @@
 
 def get_column_cell(obj, name, *, absolute_url=True):
     """
     Takes in an object and a column name, and returns the value of the column for the object.
     If the column is a custom field, it returns the value of the custom field.
     """
     model = obj._meta.model
+    
+    if isinstance(name, DynamicSubField):
+        return name.get_value(obj)
+    
     if (
         (custom_field_part := name.split("."))
         and len(custom_field_part) > 1
         and get_column_type(model, (custom_field_function_name := custom_field_part[0]))
         == FieldTypes.custom
     ):
         custom_field_value = get_model_custom_field_value(
@@ -474,52 +480,53 @@
 
 
 class ExportXls(BaseExportFormat):
     format_slug = "xls"
     format_name = "Excel"
     format_ext = ".xlsx"
     
+    def get_export_filename(self):
+        qs = self.get_export_qs()
+        if not self.export_filename and isinstance(qs, QuerySet):
+            with override("en"):
+                return f"{qs.model._meta.verbose_name_plural}{self.format_ext}"
+        
+        return f"{self.export_filename}{self.format_ext}"
+    
+    def _apply_cell_style_map(self, style, value):
+        style_map = {k: v for k, v in REPORT_CELL_STYLE_MAP if isinstance(value, k)}
+        for _, cell_style in style_map:
+            return cell_style, (callable(cell_style) and cell_style or (lambda i: i))(value)
+        return style, value
+    
+    def _default_cell_fn(self, style, value, *args, **kwargs):
+        return style, value
+    
     def export(self):
         headers_name = self.get_export_headers()
         columns = self.get_export_columns()
         queryset = self.get_export_qs()
         sheet_name = self.get_export_kwargs().get("sheet_name", "default")
-        cell_fn = self.get_export_kwargs().get("cell_fn")
+        cell_fn = self.get_export_kwargs().get("cell_fn", self._default_cell_fn)
         
         workbook = xlwt.Workbook(encoding="utf-8")
         default_style = xlwt.XFStyle()
         sheet = workbook.add_sheet(sheet_name or str(nested_getattr(queryset, "model._meta.verbose_name_plural", "sheet")))
 
         for num, column in enumerate(columns):
-            value = headers_name.get(column, column)
-            style = default_style
-            if cell_fn:
-                style, value = cell_fn(obj=None, row_number=0, column=column, style=default_style, value=value)
+            style, value = default_style, headers_name.get(column, column)
+            style, value = cell_fn(obj=None, row_number=0, column=column, style=style, value=value)
             sheet.write(0, num, value, style)
-
+        
         for x, obj in enumerate(queryset, start=1):
             for y, column in enumerate(columns):
-                value = get_column_cell(obj, column)
-                style = default_style
-                for value_type, cell_style in REPORT_CELL_STYLE_MAP:
-                    if isinstance(value, value_type):
-                        if callable(cell_style):
-                            style = default_style
-                            value = cell_style(value)
-                        else:
-                            style = cell_style
-                        break
-                if cell_fn:
-                    style, value = cell_fn(obj=obj, row_number=x, column=column, style=style, value=value)
-                args = [x, y]
-                if style:
-                    args.extend([value, style])
-                else:
-                    args.append(value)
-                sheet.write(*args)
+                style, value = default_style, get_column_cell(obj, column)
+                style, value = self._apply_cell_style_map(default_style, value)                    
+                style, value = cell_fn(obj=obj, row_number=x, column=column, style=style, value=value)
+                sheet.write(x, y, value, style or default_style)
 
         return workbook
 
     def handle(self):
         return self.export()
 
     def handle_response(self, response, *args, **kwargs):
```

### Comparing `django-flex-report-0.7.5/flex_report/views.py` & `django-flex-report-0.7.6/flex_report/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import contextlib
 from operator import call
+from collections import OrderedDict
 
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.core.exceptions import FieldError, PermissionDenied
 from django.db.models import Q
 from django.http import Http404
 from django.shortcuts import redirect
 from django.urls import reverse, reverse_lazy
@@ -25,20 +26,23 @@
 from .forms import (
     generate_column_create_form,
     generate_report_create_form,
     generate_template_create_form,
     model_user_path_formset,
 )
 from .mixins import QuerySetExportMixin, TablePageMixin, TemplateObjectMixin
+from .templatetags.flex_report_filters import get_column_verbose_name
 from .models import Column, Template
 from .utils import (
     clean_request_data,
     get_report_filename,
     increment_string_suffix,
     set_template_as_page_default,
+    get_column_type,
+    FieldTypes
 )
 
 
 class BaseView(LoginRequiredMixin, View):
     def get_queryset(self):
         qs = super().get_queryset()
         if self.request.user.is_superuser:
@@ -368,17 +372,27 @@
 general_qs_export_view = GeneralQuerySetExportView.as_view()
 
 
 class ReportExportView(QuerySetExportMixin, ReportViewBase):
     def get(self, *args, **kwargs):
         self.export_file_name = get_report_filename(self.template_object)
 
-        columns = self.template_columns
+        columns = OrderedDict()
+        for col in self.template_columns:
+            if get_column_type(self.report_model, col.title) != FieldTypes.dynamic:
+                columns[col.title] = str(get_column_verbose_name(self.report_model, col.title))
+                continue
+                
+            columns.update({
+                subfield: str(subfield.verbose_name)
+                for subfield in col.get_dynamic_obj().unpack_field()
+            })
+                
         self.export_qs = self.report_qs
-        self.export_columns = columns.values()
+        self.export_columns = columns.keys()
         self.export_headers = columns
 
         return super().get(*args, **kwargs)
 
     def template_not_ready(self):
         raise Http404
```

### Comparing `django-flex-report-0.7.5/pyproject.toml` & `django-flex-report-0.7.6/pyproject.toml`

 * *Files identical despite different names*

