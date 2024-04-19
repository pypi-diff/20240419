# Comparing `tmp/django_ses-3.6.0.tar.gz` & `tmp/django_ses-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ses-3.6.0.tar", max compression
+gzip compressed data, was "django_ses-4.0.0.tar", max compression
```

## Comparing `django_ses-3.6.0.tar` & `django_ses-4.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1057 2024-04-11 15:14:56.970438 django_ses-3.6.0/LICENSE
--rw-r--r--   0        0        0    23820 2024-04-11 15:14:56.970438 django_ses-3.6.0/README.rst
--rw-r--r--   0        0        0    14050 2024-04-11 15:14:56.970438 django_ses-3.6.0/django_ses/__init__.py
--rw-r--r--   0        0        0      232 2024-04-11 15:14:56.970438 django_ses-3.6.0/django_ses/admin.py
--rw-r--r--   0        0        0      181 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/apps.py
--rw-r--r--   0        0        0       65 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/deprecation.py
--rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/commands/__init__.py
--rw-r--r--   0        0        0     2328 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/commands/get_ses_statistics.py
--rw-r--r--   0        0        0     2700 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/commands/ses_email_address.py
--rw-r--r--   0        0        0      897 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/migrations/__init__.py
--rw-r--r--   0        0        0      455 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/models.py
--rw-r--r--   0        0        0     2677 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/settings.py
--rw-r--r--   0        0        0      290 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/signals.py
--rw-r--r--   0        0        0     4894 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/templates/django_ses/send_stats.html
--rw-r--r--   0        0        0      156 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/urls.py
--rw-r--r--   0        0        0     9957 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/utils.py
--rw-r--r--   0        0        0    20556 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/views.py
--rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/__init__.py
--rw-r--r--   0        0        0      103 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/local_settings.template.py
--rw-r--r--   0        0        0      215 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/middleware.py
--rw-r--r--   0        0        0     2173 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/settings.py
--rw-r--r--   0        0        0      295 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/templates/base.html
--rw-r--r--   0        0        0      220 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/templates/index.html
--rw-r--r--   0        0        0      756 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/templates/send-email.html
--rw-r--r--   0        0        0      812 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/urls.py
--rw-r--r--   0        0        0      885 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/views.py
--rw-r--r--   0        0        0     2608 2024-04-11 15:14:56.974438 django_ses-3.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/__init__.py
--rw-r--r--   0        0        0    16378 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_backend.py
--rw-r--r--   0        0        0     2481 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_commands.py
--rw-r--r--   0        0        0     2636 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_settings.py
--rw-r--r--   0        0        0     5200 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_stats.py
--rw-r--r--   0        0        0      366 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_urls.py
--rw-r--r--   0        0        0    13660 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_verifier.py
--rw-r--r--   0        0        0    13740 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_views.py
--rw-r--r--   0        0        0      115 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/utils.py
--rw-r--r--   0        0        0    25644 1970-01-01 00:00:00.000000 django_ses-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-04-19 16:37:59.173368 django_ses-4.0.0/LICENSE
+-rw-r--r--   0        0        0    23987 2024-04-19 16:37:59.173368 django_ses-4.0.0/README.rst
+-rw-r--r--   0        0        0    14050 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/admin.py
+-rw-r--r--   0        0        0      181 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/apps.py
+-rw-r--r--   0        0        0       65 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/deprecation.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/commands/__init__.py
+-rw-r--r--   0        0        0     2328 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/commands/get_ses_statistics.py
+-rw-r--r--   0        0        0     2700 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/commands/ses_email_address.py
+-rw-r--r--   0        0        0      897 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/models.py
+-rw-r--r--   0        0        0     2677 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/settings.py
+-rw-r--r--   0        0        0      290 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/signals.py
+-rw-r--r--   0        0        0     4894 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/templates/django_ses/send_stats.html
+-rw-r--r--   0        0        0      156 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/urls.py
+-rw-r--r--   0        0        0     9957 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/utils.py
+-rw-r--r--   0        0        0    20556 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/views.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/local_settings.template.py
+-rw-r--r--   0        0        0      215 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/middleware.py
+-rw-r--r--   0        0        0     2173 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/settings.py
+-rw-r--r--   0        0        0      295 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/templates/base.html
+-rw-r--r--   0        0        0      220 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/templates/index.html
+-rw-r--r--   0        0        0      756 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/templates/send-email.html
+-rw-r--r--   0        0        0      772 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/urls.py
+-rw-r--r--   0        0        0      885 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/views.py
+-rw-r--r--   0        0        0     2540 2024-04-19 16:37:59.177368 django_ses-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    16378 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_backend.py
+-rw-r--r--   0        0        0     2481 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_commands.py
+-rw-r--r--   0        0        0     2636 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_settings.py
+-rw-r--r--   0        0        0     5200 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_stats.py
+-rw-r--r--   0        0        0      345 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_urls.py
+-rw-r--r--   0        0        0    13660 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_verifier.py
+-rw-r--r--   0        0        0    13740 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_views.py
+-rw-r--r--   0        0        0      115 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/utils.py
+-rw-r--r--   0        0        0    25733 1970-01-01 00:00:00.000000 django_ses-4.0.0/PKG-INFO
```

### Comparing `django_ses-3.6.0/LICENSE` & `django_ses-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/README.rst` & `django_ses-4.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ==========
 Django-SES
 ==========
 :Info: A Django email backend for Amazon's Simple Email Service
 :Author: Harry Marr (http://github.com/hmarr, http://twitter.com/harrymarr)
 :Collaborators: Paul Craciunoiu (http://github.com/pcraciunoiu, http://twitter.com/embrangler)
 
-|pypi| |build| |python| |django|
+|pypi| |pypi-downloads| |build| |python| |django|
 
 A bird's eye view
 =================
 Django-SES is a drop-in mail backend for Django_. Instead of sending emails
 through a traditional SMTP mail server, Django-SES routes email through
 Amazon Web Services' excellent Simple Email Service (SES_).
 
@@ -626,13 +626,16 @@
 * Run ``poetry version {patch|minor|major}`` as explained in `the docs <https://python-poetry.org/docs/cli/#version>`_. This will update the version in pyproject.toml.
 * Commit that change and use git to tag that commit with a version that matches the pattern ``v*.*.*``.
 * Push the tag and the commit (note some IDEs don't push tags by default).
 
 
 .. |pypi| image:: https://badge.fury.io/py/django-ses.svg
     :target: http://badge.fury.io/py/django-ses
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/django-ses?style=flat
+    :target: https://pypi.org/project/django-ses/
 .. |build| image:: https://github.com/django-ses/django-ses/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/django-ses/django-ses/actions/workflows/ci.yml
-.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue.svg
     :target: https://pypi.org/project/django-ses/
-.. |django| image:: https://img.shields.io/badge/django-2.2%7C%203.2+-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-4.2%7C%205.0+-blue.svg
     :target: https://www.djangoproject.com/
+
```

### Comparing `django_ses-3.6.0/django_ses/__init__.py` & `django_ses-4.0.0/django_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/django_ses/management/commands/get_ses_statistics.py` & `django_ses-4.0.0/django_ses/management/commands/get_ses_statistics.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/django_ses/management/commands/ses_email_address.py` & `django_ses-4.0.0/django_ses/management/commands/ses_email_address.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/django_ses/migrations/0001_initial.py` & `django_ses-4.0.0/django_ses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/django_ses/settings.py` & `django_ses-4.0.0/django_ses/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/django_ses/templates/django_ses/send_stats.html` & `django_ses-4.0.0/django_ses/templates/django_ses/send_stats.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/django_ses/utils.py` & `django_ses-4.0.0/django_ses/utils.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/django_ses/views.py` & `django_ses-4.0.0/django_ses/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/example/settings.py` & `django_ses-4.0.0/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/example/templates/send-email.html` & `django_ses-4.0.0/example/templates/send-email.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/example/views.py` & `django_ses-4.0.0/example/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/pyproject.toml` & `django_ses-4.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ses"
-version = "3.6.0"
+version = "4.0.0"
 description = "A Django email backend for Amazon's Simple Email Service (SES)"
 authors = [
     "Harry Marr <harry@hmarr.com>",
     "Wes Winham <winhamwr@gmail.com>",
     "Ross Lawley <ross.lawley@gmail.com>",
     "Paul Craciunoiu <paul@craciunoiu.net>",
 ]
@@ -12,19 +12,17 @@
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Framework :: Django',
-    'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.2',
-    'Framework :: Django :: 4.0',
-    'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
+    'Framework :: Django :: 5.0',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 license = "MIT"
@@ -38,25 +36,25 @@
 "Bugtracker" = "https://github.com/django-ses/django-ses/issues"
 "Changelog" = "https://github.com/django-ses/django-ses/blob/main/CHANGES.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = ">=1.0.0"
 pytz = ">=2016.10"
-django = ">=2.2"
+django = ">=3.2"
 importlib-metadata = {version = ">=1", python = "<3.8"}
 cryptography = {version = ">=36.0.2", optional = true}
 requests = {version = ">=2.27.1", optional = true}
 
 [tool.poetry.extras]
 bounce =  ["requests", "cryptography"]
 events = ["requests", "cryptography"]
 
 [tool.poetry.dev-dependencies]
-ruff = "^0.1.6"
+ruff = "^0.3.7"
 tox = "^3.24.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `django_ses-3.6.0/tests/test_backend.py` & `django_ses-4.0.0/tests/test_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,29 +116,29 @@
         settings.AWS_SES_CONFIGURATION_SET = None
 
         from_addr = 'Albertus Magnus <albertus.magnus@example.com>'
 
         send_mail('subject', 'body', from_addr, ['to@example.com'])
         message = self.outbox.pop()
         mail = email.message_from_string(smart_str(message['RawMessage']['Data']))
-        self.assertTrue('X-SES-CONFIGURAITON-SET' not in mail.keys())
+        self.assertTrue('X-SES-CONFIGURATION-SET' not in mail.keys())
         self.assertEqual(mail['subject'], 'subject')
         self.assertEqual(mail['from'], self._rfc2047_helper(from_addr))
         self.assertEqual(mail['to'], 'to@example.com')
         self.assertEqual(mail.get_payload(), 'body')
 
     def test_send_mail_unicode_body(self):
         settings.AWS_SES_CONFIGURATION_SET = None
 
         unicode_from_addr = 'Unicode Name óóóóóó <from@example.com>'
 
         send_mail('Scandinavian', 'Sören & Björn', unicode_from_addr, ['to@example.com'])
         message = self.outbox.pop()
         mail = email.message_from_string(smart_str(message['RawMessage']['Data']))
-        self.assertTrue('X-SES-CONFIGURAITON-SET' not in mail.keys())
+        self.assertTrue('X-SES-CONFIGURATION-SET' not in mail.keys())
         self.assertEqual(mail['subject'], 'Scandinavian')
         self.assertEqual(mail['from'], self._rfc2047_helper(unicode_from_addr))
         self.assertEqual(mail['to'], 'to@example.com')
         self.assertEqual(mail.get_payload(), 'Sören & Björn')
 
     def test_configuration_set_send_mail(self):
         settings.AWS_SES_CONFIGURATION_SET = 'test-set'
@@ -201,15 +201,15 @@
         settings.AWS_SES_CONFIGURATION_SET = None
 
         unicode_from_addr = 'Unicode Name óóóóóó <from@example.com>'
 
         send_mail('subject', 'body', unicode_from_addr, ['to@example.com'])
         message = self.outbox.pop()
         mail = email.message_from_string(smart_str(message['Content']['Raw']['Data']))
-        self.assertTrue('X-SES-CONFIGURAITON-SET' not in mail.keys())
+        self.assertTrue('X-SES-CONFIGURATION-SET' not in mail.keys())
         self.assertEqual(mail['subject'], 'subject')
         self.assertEqual(mail['from'], self._rfc2047_helper(unicode_from_addr))
         self.assertEqual(mail['to'], 'to@example.com')
         self.assertEqual(mail.get_payload(), 'body')
 
     def test_configuration_set_send_mail(self):
         settings.AWS_SES_CONFIGURATION_SET = 'test-set'
```

### Comparing `django_ses-3.6.0/tests/test_commands.py` & `django_ses-4.0.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/tests/test_settings.py` & `django_ses-4.0.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/tests/test_stats.py` & `django_ses-4.0.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/tests/test_verifier.py` & `django_ses-4.0.0/tests/test_verifier.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/tests/test_views.py` & `django_ses-4.0.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.6.0/PKG-INFO` & `django_ses-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: django-ses
-Version: 3.6.0
+Version: 4.0.0
 Summary: A Django email backend for Amazon's Simple Email Service (SES)
 Home-page: https://github.com/django-ses/django-ses
 License: MIT
 Author: Harry Marr
 Author-email: harry@hmarr.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: bounce
 Provides-Extra: events
 Requires-Dist: boto3 (>=1.0.0)
 Requires-Dist: cryptography (>=36.0.2) ; extra == "bounce" or extra == "events"
-Requires-Dist: django (>=2.2)
+Requires-Dist: django (>=3.2)
 Requires-Dist: importlib-metadata (>=1) ; python_version < "3.8"
 Requires-Dist: pytz (>=2016.10)
 Requires-Dist: requests (>=2.27.1) ; extra == "bounce" or extra == "events"
 Project-URL: Bugtracker, https://github.com/django-ses/django-ses/issues
 Project-URL: Changelog, https://github.com/django-ses/django-ses/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/django-ses/django-ses/blob/main/README.rst
 Project-URL: Repository, https://github.com/django-ses/django-ses
@@ -42,15 +40,15 @@
 ==========
 Django-SES
 ==========
 :Info: A Django email backend for Amazon's Simple Email Service
 :Author: Harry Marr (http://github.com/hmarr, http://twitter.com/harrymarr)
 :Collaborators: Paul Craciunoiu (http://github.com/pcraciunoiu, http://twitter.com/embrangler)
 
-|pypi| |build| |python| |django|
+|pypi| |pypi-downloads| |build| |python| |django|
 
 A bird's eye view
 =================
 Django-SES is a drop-in mail backend for Django_. Instead of sending emails
 through a traditional SMTP mail server, Django-SES routes email through
 Amazon Web Services' excellent Simple Email Service (SES_).
 
@@ -667,14 +665,17 @@
 * Run ``poetry version {patch|minor|major}`` as explained in `the docs <https://python-poetry.org/docs/cli/#version>`_. This will update the version in pyproject.toml.
 * Commit that change and use git to tag that commit with a version that matches the pattern ``v*.*.*``.
 * Push the tag and the commit (note some IDEs don't push tags by default).
 
 
 .. |pypi| image:: https://badge.fury.io/py/django-ses.svg
     :target: http://badge.fury.io/py/django-ses
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/django-ses?style=flat
+    :target: https://pypi.org/project/django-ses/
 .. |build| image:: https://github.com/django-ses/django-ses/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/django-ses/django-ses/actions/workflows/ci.yml
-.. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
+.. |python| image:: https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue.svg
     :target: https://pypi.org/project/django-ses/
-.. |django| image:: https://img.shields.io/badge/django-2.2%7C%203.2+-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-4.2%7C%205.0+-blue.svg
     :target: https://www.djangoproject.com/
 
+
```

