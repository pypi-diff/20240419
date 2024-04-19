# Comparing `tmp/datalookup-1.0.0rc3.tar.gz` & `tmp/datalookup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalookup-1.0.0rc3.tar", last modified: Mon Jun 12 13:08:39 2023, max compression
+gzip compressed data, was "datalookup-1.0.1.tar", last modified: Fri Apr 19 09:17:55 2024, max compression
```

## Comparing `datalookup-1.0.0rc3.tar` & `datalookup-1.0.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.201708 datalookup-1.0.0rc3/
--rw-rw-rw-   0        0        0      106 2023-06-09 08:05:43.000000 datalookup-1.0.0rc3/.coveragerc
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:38.887206 datalookup-1.0.0rc3/.github/
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:38.997206 datalookup-1.0.0rc3/.github/workflows/
--rw-rw-rw-   0        0        0     1079 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/coverage.yml
--rw-rw-rw-   0        0        0      747 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1110 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/linters.yml
--rw-rw-rw-   0        0        0      959 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.github/workflows/tests.yml
--rw-rw-rw-   0        0        0      987 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/.gitignore
--rw-rw-rw-   0        0        0      709 2023-03-14 20:24:24.000000 datalookup-1.0.0rc3/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      383 2023-06-09 20:02:09.000000 datalookup-1.0.0rc3/.readthedocs.yml
--rw-rw-rw-   0        0        0      127 2023-06-05 15:31:40.000000 datalookup-1.0.0rc3/AUTHORS
--rw-rw-rw-   0        0        0     5352 2023-03-05 10:52:09.000000 datalookup-1.0.0rc3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     9257 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1091 2023-06-04 19:25:49.000000 datalookup-1.0.0rc3/LICENCE
--rw-rw-rw-   0        0        0    12690 2023-06-12 13:08:39.196705 datalookup-1.0.0rc3/PKG-INFO
--rw-rw-rw-   0        0        0    11454 2023-06-12 07:25:37.000000 datalookup-1.0.0rc3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.026207 datalookup-1.0.0rc3/datalookup/
--rw-rw-rw-   0        0        0    16179 2023-06-09 10:34:07.000000 datalookup-1.0.0rc3/datalookup/__init__.py
--rw-rw-rw-   0        0        0      167 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup/_version.py
--rw-rw-rw-   0        0        0      500 2023-06-09 07:34:13.000000 datalookup-1.0.0rc3/datalookup/exceptions.py
--rw-rw-rw-   0        0        0     5638 2023-06-08 19:20:21.000000 datalookup-1.0.0rc3/datalookup/fields.py
--rw-rw-rw-   0        0        0     8265 2023-06-08 19:39:46.000000 datalookup-1.0.0rc3/datalookup/lookup.py
--rw-rw-rw-   0        0        0     2106 2023-06-09 08:05:56.000000 datalookup-1.0.0rc3/datalookup/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.048205 datalookup-1.0.0rc3/datalookup.egg-info/
--rw-rw-rw-   0        0        0    12690 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 13:08:38.000000 datalookup-1.0.0rc3/datalookup.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.109205 datalookup-1.0.0rc3/docs/
--rw-rw-rw-   0        0        0      654 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.113707 datalookup-1.0.0rc3/docs/_ext/
--rw-rw-rw-   0        0        0      205 2023-06-08 17:25:06.000000 datalookup-1.0.0rc3/docs/_ext/datalookup_docs.py
--rw-rw-rw-   0        0        0     3861 2023-06-09 07:24:11.000000 datalookup-1.0.0rc3/docs/conf.py
--rw-rw-rw-   0        0        0      307 2023-06-06 16:38:28.000000 datalookup-1.0.0rc3/docs/contents.rst
--rw-rw-rw-   0        0        0    15980 2023-06-09 20:02:09.000000 datalookup-1.0.0rc3/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.141707 datalookup-1.0.0rc3/docs/internals/
--rw-rw-rw-   0        0        0      443 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/docs/internals/changelog.rst
--rw-rw-rw-   0        0        0     2905 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/docs/internals/coding-style.rst
--rw-rw-rw-   0        0        0       58 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/internals/contributing.rst
--rw-rw-rw-   0        0        0      449 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/internals/deprecations.rst
--rw-rw-rw-   0        0        0      307 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/internals/index.rst
--rw-rw-rw-   0        0        0     2395 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/docs/internals/release-process.rst
--rwxrwxrwx   0        0        0      800 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/make.bat
--rw-rw-rw-   0        0        0       63 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/docs/requirements.txt
--rw-rw-rw-   0        0        0      202 2023-06-08 17:25:06.000000 datalookup-1.0.0rc3/docs/spelling_wordlist
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.147708 datalookup-1.0.0rc3/licenses/
--rw-rw-rw-   0        0        0     1579 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/licenses/django.license
--rw-rw-rw-   0        0        0     1497 2023-06-12 13:01:49.000000 datalookup-1.0.0rc3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 13:08:39.202206 datalookup-1.0.0rc3/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-06-05 15:31:49.000000 datalookup-1.0.0rc3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.175205 datalookup-1.0.0rc3/tests/
--rw-rw-rw-   0        0        0      439 2023-06-09 10:37:27.000000 datalookup-1.0.0rc3/tests/README.rst
--rw-rw-rw-   0        0        0        0 2022-04-23 14:09:47.000000 datalookup-1.0.0rc3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:08:39.188207 datalookup-1.0.0rc3/tests/data/
--rw-rw-rw-   0        0        0      956 2023-05-29 16:14:03.000000 datalookup-1.0.0rc3/tests/data/books.json
--rw-rw-rw-   0        0        0     1652 2023-05-30 19:23:32.000000 datalookup-1.0.0rc3/tests/data/recipe.json
--rw-rw-rw-   0        0        0      231 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/tests/lookup.py
--rw-rw-rw-   0        0        0       77 2023-05-11 15:53:03.000000 datalookup-1.0.0rc3/tests/pytest.ini
--rw-rw-rw-   0        0        0       62 2023-06-06 15:59:32.000000 datalookup-1.0.0rc3/tests/requirements.txt
--rw-rw-rw-   0        0        0    23841 2023-06-09 10:34:07.000000 datalookup-1.0.0rc3/tests/tests.py
--rw-rw-rw-   0        0        0     1406 2023-06-05 15:25:48.000000 datalookup-1.0.0rc3/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:55.259658 datalookup-1.0.1/
+-rw-rw-rw-   0        0        0      106 2024-04-18 13:42:09.000000 datalookup-1.0.1/.coveragerc
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:54.478166 datalookup-1.0.1/.github/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:54.696941 datalookup-1.0.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1079 2023-06-05 10:16:26.000000 datalookup-1.0.1/.github/workflows/coverage.yml
+-rw-rw-rw-   0        0        0      747 2023-06-05 10:16:26.000000 datalookup-1.0.1/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1110 2023-06-05 10:16:26.000000 datalookup-1.0.1/.github/workflows/linters.yml
+-rw-rw-rw-   0        0        0      959 2023-06-05 10:16:26.000000 datalookup-1.0.1/.github/workflows/tests.yml
+-rw-rw-rw-   0        0        0      987 2023-06-05 13:57:28.000000 datalookup-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0      709 2023-05-12 11:42:42.000000 datalookup-1.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      383 2024-04-18 13:42:09.000000 datalookup-1.0.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0      127 2023-06-06 10:06:10.000000 datalookup-1.0.1/AUTHORS
+-rw-rw-rw-   0        0        0     5352 2023-05-12 11:42:42.000000 datalookup-1.0.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     9257 2023-06-06 12:21:31.000000 datalookup-1.0.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1091 2023-06-05 07:07:04.000000 datalookup-1.0.1/LICENCE
+-rw-rw-rw-   0        0        0    12689 2024-04-19 09:17:55.259658 datalookup-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11456 2024-04-18 13:42:09.000000 datalookup-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:54.790690 datalookup-1.0.1/datalookup/
+-rw-rw-rw-   0        0        0    16323 2024-04-19 07:51:38.000000 datalookup-1.0.1/datalookup/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-04-19 09:17:53.000000 datalookup-1.0.1/datalookup/_version.py
+-rw-rw-rw-   0        0        0      500 2024-04-18 13:42:09.000000 datalookup-1.0.1/datalookup/exceptions.py
+-rw-rw-rw-   0        0        0     5638 2024-04-18 13:42:09.000000 datalookup-1.0.1/datalookup/fields.py
+-rw-rw-rw-   0        0        0     8265 2024-04-18 13:42:09.000000 datalookup-1.0.1/datalookup/lookup.py
+-rw-rw-rw-   0        0        0     2106 2024-04-18 13:42:09.000000 datalookup-1.0.1/datalookup/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:55.259658 datalookup-1.0.1/datalookup.egg-info/
+-rw-rw-rw-   0        0        0    12689 2024-04-19 09:17:54.000000 datalookup-1.0.1/datalookup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2024-04-19 09:17:54.000000 datalookup-1.0.1/datalookup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:17:54.000000 datalookup-1.0.1/datalookup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 09:17:54.000000 datalookup-1.0.1/datalookup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:54.978269 datalookup-1.0.1/docs/
+-rw-rw-rw-   0        0        0      634 2023-06-05 13:15:14.000000 datalookup-1.0.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:54.993779 datalookup-1.0.1/docs/_ext/
+-rw-rw-rw-   0        0        0      205 2023-06-08 14:09:41.000000 datalookup-1.0.1/docs/_ext/datalookup_docs.py
+-rw-rw-rw-   0        0        0     3861 2024-04-19 07:57:53.000000 datalookup-1.0.1/docs/conf.py
+-rw-rw-rw-   0        0        0      307 2023-06-05 13:33:46.000000 datalookup-1.0.1/docs/contents.rst
+-rw-rw-rw-   0        0        0    15980 2024-04-18 13:42:09.000000 datalookup-1.0.1/docs/index.rst
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:55.103166 datalookup-1.0.1/docs/internals/
+-rw-rw-rw-   0        0        0      763 2024-04-19 07:57:01.000000 datalookup-1.0.1/docs/internals/changelog.rst
+-rw-rw-rw-   0        0        0     2905 2023-06-06 12:11:49.000000 datalookup-1.0.1/docs/internals/coding-style.rst
+-rw-rw-rw-   0        0        0       58 2023-06-05 13:31:46.000000 datalookup-1.0.1/docs/internals/contributing.rst
+-rw-rw-rw-   0        0        0      449 2023-06-05 14:29:00.000000 datalookup-1.0.1/docs/internals/deprecations.rst
+-rw-rw-rw-   0        0        0      307 2023-06-05 13:41:14.000000 datalookup-1.0.1/docs/internals/index.rst
+-rw-rw-rw-   0        0        0     2395 2023-06-06 12:12:24.000000 datalookup-1.0.1/docs/internals/release-process.rst
+-rwxrwxrwx   0        0        0      800 2023-06-05 13:15:14.000000 datalookup-1.0.1/docs/make.bat
+-rw-rw-rw-   0        0        0       63 2023-06-05 10:16:26.000000 datalookup-1.0.1/docs/requirements.txt
+-rw-rw-rw-   0        0        0      201 2023-06-08 14:23:43.000000 datalookup-1.0.1/docs/spelling_wordlist
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:55.118791 datalookup-1.0.1/licenses/
+-rw-rw-rw-   0        0        0     1578 2023-06-05 13:49:28.000000 datalookup-1.0.1/licenses/django.license
+-rw-rw-rw-   0        0        0     1497 2024-04-18 13:42:09.000000 datalookup-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:17:55.259658 datalookup-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-05-12 11:42:42.000000 datalookup-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:55.241013 datalookup-1.0.1/tests/
+-rw-rw-rw-   0        0        0      439 2024-04-18 13:42:09.000000 datalookup-1.0.1/tests/README.rst
+-rw-rw-rw-   0        0        0        0 2023-05-09 09:51:25.000000 datalookup-1.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:55.259658 datalookup-1.0.1/tests/data/
+-rw-rw-rw-   0        0        0      957 2023-05-30 08:32:44.000000 datalookup-1.0.1/tests/data/books.json
+-rw-rw-rw-   0        0        0     1652 2023-05-30 13:10:44.000000 datalookup-1.0.1/tests/data/recipe.json
+-rw-rw-rw-   0        0        0      231 2023-06-05 07:11:51.000000 datalookup-1.0.1/tests/lookup.py
+-rw-rw-rw-   0        0        0       77 2023-05-12 11:42:42.000000 datalookup-1.0.1/tests/pytest.ini
+-rw-rw-rw-   0        0        0       62 2023-06-06 12:18:59.000000 datalookup-1.0.1/tests/requirements.txt
+-rw-rw-rw-   0        0        0    24042 2024-04-19 07:51:38.000000 datalookup-1.0.1/tests/tests.py
+-rw-rw-rw-   0        0        0     1406 2023-06-05 13:28:13.000000 datalookup-1.0.1/tox.ini
```

### Comparing `datalookup-1.0.0rc3/.github/workflows/coverage.yml` & `datalookup-1.0.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/.github/workflows/docs.yml` & `datalookup-1.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/.github/workflows/linters.yml` & `datalookup-1.0.1/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/.github/workflows/tests.yml` & `datalookup-1.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/.gitignore` & `datalookup-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/.pre-commit-config.yaml` & `datalookup-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/CODE_OF_CONDUCT.md` & `datalookup-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/CONTRIBUTING.rst` & `datalookup-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/LICENCE` & `datalookup-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/PKG-INFO` & `datalookup-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalookup
-Version: 1.0.0rc3
+Version: 1.0.1
 Summary: Deep nested data filtering library
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: MIT
 Project-URL: homepage, https://datalookup.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/pyshare/datalookup
 Project-URL: changelog, https://datalookup.readthedocs.io/en/latest/internals/changelog.html
 Keywords: filter,dictionary,nested,datalookup,data-filtering,deep-filtering,lookup
@@ -262,15 +262,15 @@
 | len          |                         | Check length of the array. ArrayField only                      |
 +--------------+-------------------------+-----------------------------------------------------------------+
 
 Documentation
 =============
 
 Datalookup does not stop here. The full documentation is in the ``docs``
-directory or online at https://datalookup.readthedocs.io/en/latest/
+directory or online at `https://datalookup.readthedocs.io/en/latest/`
 
 Contribution
 ============
 
 Anyone can contribute to Datalookup's development. Checkout our documentation on how to
 get involved: `https://datalookup.readthedocs.io/en/latest/internals/contributing.html`
```

### Comparing `datalookup-1.0.0rc3/README.rst` & `datalookup-1.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 | len          |                         | Check length of the array. ArrayField only                      |
 +--------------+-------------------------+-----------------------------------------------------------------+
 
 Documentation
 =============
 
 Datalookup does not stop here. The full documentation is in the ``docs``
-directory or online at https://datalookup.readthedocs.io/en/latest/
+directory or online at `https://datalookup.readthedocs.io/en/latest/`
 
 Contribution
 ============
 
 Anyone can contribute to Datalookup's development. Checkout our documentation on how to
 get involved: `https://datalookup.readthedocs.io/en/latest/internals/contributing.html`
```

### Comparing `datalookup-1.0.0rc3/datalookup/__init__.py` & `datalookup-1.0.1/datalookup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,20 @@
                     "books": {
                         "genre": "Fantasy"
                     }
                 }
             ]
 
             books = Dataset(data)
-            books.filter(author__exact="J. K. Rowling")
-            books.filter(books__genre__in=["Fantasy"])
+            books.exclude(author__exact="J. K. Rowling")
+            books.exclude(books__genre__in=["Fantasy"])
         """
+        if not kwargs:
+            return self
+
         data: list[Node] = []
         for node in self:
             try:
                 node.filter(**kwargs)
             except ObjectNotFound:
                 data.append(node)
         return Dataset.from_nodes(data)
@@ -284,17 +287,19 @@
         except FieldNotFound:
             raise AttributeError(f"{name} attribute does not exist")
 
     def __repr__(self):
         return "<{}: {}>".format(self.__class__.__name__, self)
 
     def __str__(self):
-        return "{} object ({})".format(
-            self.__class__.__name__, list(self.fields.values())[0].get_value()
-        )
+        try:
+            field_value = list(self.fields.values())[0].get_value()
+        except IndexError:
+            field_value = "None"
+        return "{} object ({})".format(self.__class__.__name__, field_value)
 
     def activate_on_cascade(self):
         """Activate filtering on cascade"""
         self.on_cascade = True
         for field in self.fields.values():
             for node in getattr(field, "related_node", []):
                 node.activate_on_cascade()
```

### Comparing `datalookup-1.0.0rc3/datalookup/fields.py` & `datalookup-1.0.1/datalookup/fields.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/datalookup/lookup.py` & `datalookup-1.0.1/datalookup/lookup.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/datalookup/utils.py` & `datalookup-1.0.1/datalookup/utils.py`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/datalookup.egg-info/PKG-INFO` & `datalookup-1.0.1/datalookup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalookup
-Version: 1.0.0rc3
+Version: 1.0.1
 Summary: Deep nested data filtering library
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: MIT
 Project-URL: homepage, https://datalookup.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/pyshare/datalookup
 Project-URL: changelog, https://datalookup.readthedocs.io/en/latest/internals/changelog.html
 Keywords: filter,dictionary,nested,datalookup,data-filtering,deep-filtering,lookup
@@ -262,15 +262,15 @@
 | len          |                         | Check length of the array. ArrayField only                      |
 +--------------+-------------------------+-----------------------------------------------------------------+
 
 Documentation
 =============
 
 Datalookup does not stop here. The full documentation is in the ``docs``
-directory or online at https://datalookup.readthedocs.io/en/latest/
+directory or online at `https://datalookup.readthedocs.io/en/latest/`
 
 Contribution
 ============
 
 Anyone can contribute to Datalookup's development. Checkout our documentation on how to
 get involved: `https://datalookup.readthedocs.io/en/latest/internals/contributing.html`
```

### Comparing `datalookup-1.0.0rc3/datalookup.egg-info/SOURCES.txt` & `datalookup-1.0.1/datalookup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/docs/Makefile` & `datalookup-1.0.1/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `datalookup-1.0.0rc3/docs/conf.py` & `datalookup-1.0.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "Datalookup"
 copyright = "2023, Stephane Capponi and others"
 author = "Stephane Capponi"
 
 # The full version, including alpha/beta/rc tags
-version = "1.0.0"
+version = "1.0.1"
 
 # Documentation release version
 try:
     from datalookup import __version__ as version
 except ImportError:
     release = version
 else:
```

### Comparing `datalookup-1.0.0rc3/docs/index.rst` & `datalookup-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/docs/internals/coding-style.rst` & `datalookup-1.0.1/docs/internals/coding-style.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/docs/internals/release-process.rst` & `datalookup-1.0.1/docs/internals/release-process.rst`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/docs/make.bat` & `datalookup-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/licenses/django.license` & `datalookup-1.0.1/licenses/django.license`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
 ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `datalookup-1.0.0rc3/pyproject.toml` & `datalookup-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/tests/data/books.json` & `datalookup-1.0.1/tests/data/books.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 00000340: 6520 5765 7265 204e 6f6e 6522 2c0d 0a20  e Were None",.. 
 00000350: 2020 2020 2020 2020 2020 2020 2020 2022                 "
 00000360: 6765 6e72 6522 3a20 224d 7973 7465 7279  genre": "Mystery
 00000370: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
 00000380: 2020 2020 2270 7562 6c69 7368 6564 223a      "published":
 00000390: 2022 3139 3339 220d 0a20 2020 2020 2020   "1939"..       
 000003a0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-000003b0: 5d0d 0a20 2020 207d 0d0a 5d0a            ]..    }..].
+000003b0: 5d0d 0a20 2020 207d 0d0a 5d0d 0a         ]..    }..]..
```

### Comparing `datalookup-1.0.0rc3/tests/data/recipe.json` & `datalookup-1.0.1/tests/data/recipe.json`

 * *Files identical despite different names*

### Comparing `datalookup-1.0.0rc3/tests/tests.py` & `datalookup-1.0.1/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,19 @@
 
     def test_exclude(self, books: Dataset):
         """Check that we return all elements that are not exclude"""
         authors = books.exclude(books__genre="Fantasy")
         assert len(authors) == 1
         assert authors[0].author == "Agatha Christie"
 
+    def test_exclude_empty_kwargs(self, books: Dataset):
+        """If an empty directory is passed, return the full dataset"""
+        authors = books.exclude()
+        assert len(authors) == 3
+
     def test_distinct(self):
         """Check that we correctly remove duplicates"""
         data = [{"test": "test"}, {"test": "test"}, {"hello": "test"}]
         dataset = Dataset(data)
         assert len(dataset) == 3
         distinct_set = dataset.distinct()
         assert len(distinct_set) == 2
```

### Comparing `datalookup-1.0.0rc3/tox.ini` & `datalookup-1.0.1/tox.ini`

 * *Files identical despite different names*

