# Comparing `tmp/cookieplone-0.2.0.tar.gz` & `tmp/cookieplone-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookieplone-0.2.0.tar", max compression
+gzip compressed data, was "cookieplone-0.3.0.tar", max compression
```

## Comparing `cookieplone-0.2.0.tar` & `cookieplone-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1142 2024-04-19 01:23:35.441045 cookieplone-0.2.0/README.md
--rw-r--r--   0        0        0       22 2024-04-19 01:23:35.441300 cookieplone-0.2.0/cookieplone/__init__.py
--rw-r--r--   0        0        0      191 2024-04-16 22:18:14.202809 cookieplone-0.2.0/cookieplone/__main__.py
--rw-r--r--   0        0        0     5546 2024-04-19 00:05:39.265993 cookieplone-0.2.0/cookieplone/cli.py
--rw-r--r--   0        0        0     1203 2024-04-17 19:41:55.848797 cookieplone-0.2.0/cookieplone/data.py
--rw-r--r--   0        0        0      452 2024-04-18 19:29:44.648761 cookieplone-0.2.0/cookieplone/exceptions.py
--rw-r--r--   0        0        0     2401 2024-04-18 17:59:28.841529 cookieplone-0.2.0/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0     3522 2024-04-18 23:56:24.228008 cookieplone-0.2.0/cookieplone/generator.py
--rw-r--r--   0        0        0     1347 2024-04-18 23:57:11.861636 cookieplone-0.2.0/cookieplone/repository.py
--rw-r--r--   0        0        0      394 2024-04-18 19:18:47.072810 cookieplone-0.2.0/cookieplone/settings.py
--rw-r--r--   0        0        0       60 2024-04-17 16:17:54.105869 cookieplone-0.2.0/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     2696 2024-04-18 17:54:31.026810 cookieplone-0.2.0/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0     3710 2024-04-19 00:07:35.659983 cookieplone-0.2.0/cookieplone/utils/console.py
--rw-r--r--   0        0        0      243 2024-04-18 17:23:34.273811 cookieplone-0.2.0/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      486 2024-04-18 22:26:25.935421 cookieplone-0.2.0/cookieplone/utils/files.py
--rw-r--r--   0        0        0      887 2024-04-16 23:39:28.137531 cookieplone-0.2.0/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4516 2024-04-18 22:47:44.003042 cookieplone-0.2.0/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2780 2024-04-18 17:23:34.273620 cookieplone-0.2.0/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2176 2024-04-18 04:00:14.008502 cookieplone-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 cookieplone-0.2.0/setup.py
--rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 cookieplone-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1142 2024-04-19 01:23:35.441045 cookieplone-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-19 01:27:14.538901 cookieplone-0.3.0/cookieplone/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-16 22:18:14.202809 cookieplone-0.3.0/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5546 2024-04-19 00:05:39.265993 cookieplone-0.3.0/cookieplone/cli.py
+-rw-r--r--   0        0        0     1203 2024-04-17 19:41:55.848797 cookieplone-0.3.0/cookieplone/data.py
+-rw-r--r--   0        0        0      452 2024-04-18 19:29:44.648761 cookieplone-0.3.0/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     2401 2024-04-18 17:59:28.841529 cookieplone-0.3.0/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0     3522 2024-04-18 23:56:24.228008 cookieplone-0.3.0/cookieplone/generator.py
+-rw-r--r--   0        0        0     1347 2024-04-18 23:57:11.861636 cookieplone-0.3.0/cookieplone/repository.py
+-rw-r--r--   0        0        0      394 2024-04-18 19:18:47.072810 cookieplone-0.3.0/cookieplone/settings.py
+-rw-r--r--   0        0        0       60 2024-04-17 16:17:54.105869 cookieplone-0.3.0/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     2696 2024-04-18 17:54:31.026810 cookieplone-0.3.0/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0     3710 2024-04-19 00:07:35.659983 cookieplone-0.3.0/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      243 2024-04-18 17:23:34.273811 cookieplone-0.3.0/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      486 2024-04-18 22:26:25.935421 cookieplone-0.3.0/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      887 2024-04-16 23:39:28.137531 cookieplone-0.3.0/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4516 2024-04-18 22:47:44.003042 cookieplone-0.3.0/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2780 2024-04-18 17:23:34.273620 cookieplone-0.3.0/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2196 2024-04-19 01:26:29.201409 cookieplone-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 cookieplone-0.3.0/setup.py
+-rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 cookieplone-0.3.0/PKG-INFO
```

### Comparing `cookieplone-0.2.0/README.md` & `cookieplone-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/cli.py` & `cookieplone-0.3.0/cookieplone/cli.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/data.py` & `cookieplone-0.3.0/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/filters/__init__.py` & `cookieplone-0.3.0/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/generator.py` & `cookieplone-0.3.0/cookieplone/generator.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/repository.py` & `cookieplone-0.3.0/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/utils/commands/__init__.py` & `cookieplone-0.3.0/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/utils/console.py` & `cookieplone-0.3.0/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/utils/sanity.py` & `cookieplone-0.3.0/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/utils/validators.py` & `cookieplone-0.3.0/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/cookieplone/utils/versions.py` & `cookieplone-0.3.0/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.2.0/pyproject.toml` & `cookieplone-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 cookiecutter = "^2.6.0"
 semver = "^3.0.2"
 typer = {extras = ["all"], version = "^0.12.3"}
+packaging = "^24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pre-commit = "^3.7.0"
 tox = "^4.14.2"
```

### Comparing `cookieplone-0.2.0/setup.py` & `cookieplone-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,23 +8,24 @@
  'cookieplone.utils.commands']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cookiecutter>=2.6.0,<3.0.0',
+ 'packaging>=24.0,<25.0',
  'semver>=3.0.2,<4.0.0',
  'typer[all]>=0.12.3,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['cookieplone = cookieplone.__main__:main']}
 
 setup_kwargs = {
     'name': 'cookieplone',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Create Plone projects, addons, documentation with ease!',
     'long_description': '<p align="center">\n    <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-logo.png">\n</p>\n\n<h1 align="center">\n  cookieplone\n</h1>\n\n\n<div align="center">\n\n[![PyPI](https://img.shields.io/pypi/v/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - Wheel](https://img.shields.io/pypi/wheel/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - License](https://img.shields.io/pypi/l/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - Status](https://img.shields.io/pypi/status/cookieplone)](https://pypi.org/project/cookieplone/)\n\n\n[![Tests](https://github.com/plone/cookieplone/actions/workflows/main.yml/badge.svg)](https://github.com/plone/cookieplone/actions/workflows/main.yml)\n\n[![GitHub contributors](https://img.shields.io/github/contributors/plone/cookieplone)](https://github.com/plone/cookieplone)\n[![GitHub Repo stars](https://img.shields.io/github/stars/plone/cookieplone?style=social)](https://github.com/plone/cookieplone)\n\n</div>\n',
     'author': 'Plone Community',
     'author_email': 'dev@plone.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/plone/cookieplone',
```

### Comparing `cookieplone-0.2.0/PKG-INFO` & `cookieplone-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookieplone
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create Plone projects, addons, documentation with ease!
 Home-page: https://github.com/plone/cookieplone
 Author: Plone Community
 Author-email: dev@plone.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: cookiecutter (>=2.6.0,<3.0.0)
+Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: semver (>=3.0.2,<4.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Project-URL: Documentation, https://plone.github.io/cookieplone/
 Project-URL: Repository, https://github.com/plone/cookieplone
 Description-Content-Type: text/markdown
 
 <p align="center">
```

