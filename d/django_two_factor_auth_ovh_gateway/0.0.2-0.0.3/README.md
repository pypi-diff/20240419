# Comparing `tmp/django_two_factor_auth_ovh_gateway-0.0.2.tar.gz` & `tmp/django_two_factor_auth_ovh_gateway-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_two_factor_auth_ovh_gateway-0.0.2.tar", max compression
+gzip compressed data, was "django_two_factor_auth_ovh_gateway-0.0.3.tar", max compression
```

## Comparing `django_two_factor_auth_ovh_gateway-0.0.2.tar` & `django_two_factor_auth_ovh_gateway-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35150 2023-05-22 07:49:13.081601 django_two_factor_auth_ovh_gateway-0.0.2/LICENSE
--rw-r--r--   0        0        0     2519 2023-05-23 08:15:35.616837 django_two_factor_auth_ovh_gateway-0.0.2/README.md
--rw-r--r--   0        0        0       22 2023-05-23 08:15:53.900984 django_two_factor_auth_ovh_gateway-0.0.2/django_two_factor_auth_ovh_gateway/__init__.py
--rw-r--r--   0        0        0      141 2023-05-22 14:13:19.244365 django_two_factor_auth_ovh_gateway-0.0.2/django_two_factor_auth_ovh_gateway/apps.py
--rw-r--r--   0        0        0        0 2023-05-22 07:49:13.089600 django_two_factor_auth_ovh_gateway-0.0.2/django_two_factor_auth_ovh_gateway/conf/__init__.py
--rw-r--r--   0        0        0     2142 2023-05-22 14:19:17.798990 django_two_factor_auth_ovh_gateway-0.0.2/django_two_factor_auth_ovh_gateway/conf/settings.py
--rw-r--r--   0        0        0     1610 2023-05-23 07:44:25.632145 django_two_factor_auth_ovh_gateway-0.0.2/django_two_factor_auth_ovh_gateway/gateway.py
--rw-r--r--   0        0        0     1336 2023-05-23 08:15:53.904984 django_two_factor_auth_ovh_gateway-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 django_two_factor_auth_ovh_gateway-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-05-22 07:49:13.081601 django_two_factor_auth_ovh_gateway-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2519 2023-05-23 08:15:35.616837 django_two_factor_auth_ovh_gateway-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-19 13:35:22.510401 django_two_factor_auth_ovh_gateway-0.0.3/django_two_factor_auth_ovh_gateway/__init__.py
+-rw-r--r--   0        0        0      141 2023-05-22 14:13:19.244365 django_two_factor_auth_ovh_gateway-0.0.3/django_two_factor_auth_ovh_gateway/apps.py
+-rw-r--r--   0        0        0        0 2023-05-22 07:49:13.089600 django_two_factor_auth_ovh_gateway-0.0.3/django_two_factor_auth_ovh_gateway/conf/__init__.py
+-rw-r--r--   0        0        0     2142 2023-05-22 14:19:17.798990 django_two_factor_auth_ovh_gateway-0.0.3/django_two_factor_auth_ovh_gateway/conf/settings.py
+-rw-r--r--   0        0        0     1610 2023-05-23 07:44:25.632145 django_two_factor_auth_ovh_gateway-0.0.3/django_two_factor_auth_ovh_gateway/gateway.py
+-rw-r--r--   0        0        0     1375 2024-04-19 13:35:22.510401 django_two_factor_auth_ovh_gateway-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 django_two_factor_auth_ovh_gateway-0.0.3/PKG-INFO
```

### Comparing `django_two_factor_auth_ovh_gateway-0.0.2/LICENSE` & `django_two_factor_auth_ovh_gateway-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_two_factor_auth_ovh_gateway-0.0.2/README.md` & `django_two_factor_auth_ovh_gateway-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_two_factor_auth_ovh_gateway-0.0.2/django_two_factor_auth_ovh_gateway/conf/settings.py` & `django_two_factor_auth_ovh_gateway-0.0.3/django_two_factor_auth_ovh_gateway/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_two_factor_auth_ovh_gateway-0.0.2/django_two_factor_auth_ovh_gateway/gateway.py` & `django_two_factor_auth_ovh_gateway-0.0.3/django_two_factor_auth_ovh_gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `django_two_factor_auth_ovh_gateway-0.0.2/pyproject.toml` & `django_two_factor_auth_ovh_gateway-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "django_two_factor_auth_ovh_gateway"
-version = "0.0.2"
+version = "0.0.3"
 description = "Extension for django-two-factor-auth to use OVH SMS gateway"
 authors = ["Kapt dev team <dev@kapt.mobi>"]
 license = "GNU GPLv3"
 readme = "README.md"
 repository = "https://gitlab.com/kapt/open-source/django-two-factor-auth-ovh-gateway"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Django = "^3.0"
-django-two-factor-auth = "^1.15.2"
+django-two-factor-auth = {extras = ["phonenumbers"], version = "^1.15.2"}
 ovh = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 gitchangelog = "^3.0.4"
 bumpversion = "^0.6.0"
 black = "~23.3.0"
 flake8 = "~6.0.0"
```

### Comparing `django_two_factor_auth_ovh_gateway-0.0.2/PKG-INFO` & `django_two_factor_auth_ovh_gateway-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: django-two-factor-auth-ovh-gateway
-Version: 0.0.2
+Name: django_two_factor_auth_ovh_gateway
+Version: 0.0.3
 Summary: Extension for django-two-factor-auth to use OVH SMS gateway
 Home-page: https://gitlab.com/kapt/open-source/django-two-factor-auth-ovh-gateway
 License: GNU GPLv3
 Author: Kapt dev team
 Author-email: dev@kapt.mobi
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.0,<4.0)
-Requires-Dist: django-two-factor-auth (>=1.15.2,<2.0.0)
+Requires-Dist: django-two-factor-auth[phonenumbers] (>=1.15.2,<2.0.0)
 Requires-Dist: ovh (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/kapt/open-source/django-two-factor-auth-ovh-gateway
 Description-Content-Type: text/markdown
 
 # django_two_factor_auth_ovh_gateway
```

