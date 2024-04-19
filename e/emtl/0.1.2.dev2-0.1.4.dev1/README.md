# Comparing `tmp/emtl-0.1.2.dev2.tar.gz` & `tmp/emtl-0.1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtl-0.1.2.dev2.tar", last modified: Wed Apr 17 01:00:14 2024, max compression
+gzip compressed data, was "emtl-0.1.4.dev1.tar", last modified: Fri Apr 19 01:57:32 2024, max compression
```

## Comparing `emtl-0.1.2.dev2.tar` & `emtl-0.1.4.dev1.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      757 2024-04-16 09:19:18.000000 emtl-0.1.2.dev2/.bumpversion.cfg
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1901 2024-04-16 09:19:18.000000 emtl-0.1.2.dev2/.cookiecutterrc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      149 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/.coveragerc
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      353 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/.editorconfig
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.737292 emtl-0.1.2.dev2/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.737292 emtl-0.1.2.dev2/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2774 2024-04-16 07:03:41.000000 emtl-0.1.2.dev2/.github/workflows/github-actions.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      734 2024-04-16 01:37:37.000000 emtl-0.1.2.dev2/.gitignore
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      686 2024-04-16 01:27:59.000000 emtl-0.1.2.dev2/.pre-commit-config.yaml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      282 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/.readthedocs.yml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       65 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/AUTHORS.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      161 2024-04-16 09:47:50.000000 emtl-0.1.2.dev2/CHANGELOG.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2274 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/CONTRIBUTING.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1117 2024-04-16 01:42:17.000000 emtl-0.1.2.dev2/LICENSE
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1992 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2245 2024-04-16 09:19:18.000000 emtl-0.1.2.dev2/README.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.737292 emtl-0.1.2.dev2/ci/
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2867 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/ci/bootstrap.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       72 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/ci/requirements.txt
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.737292 emtl-0.1.2.dev2/ci/templates/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.737292 emtl-0.1.2.dev2/ci/templates/.github/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.737292 emtl-0.1.2.dev2/ci/templates/.github/workflows/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2179 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/docs/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       28 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/authors.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       30 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/changelog.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1109 2024-04-16 09:19:18.000000 emtl-0.1.2.dev2/docs/conf.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       33 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/contributing.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      244 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       84 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/installation.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       27 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/readme.rst
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/docs/reference/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      146 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/reference/emtl.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       56 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/reference/index.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       17 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/requirements.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      109 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/spelling_wordlist.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       98 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/docs/usage.rst
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1381 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/pyproject.toml
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1303 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/pytest.ini
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/setup.cfg
--rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2987 2024-04-16 09:19:18.000000 emtl-0.1.2.dev2/setup.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.737292 emtl-0.1.2.dev2/src/
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/src/emtl/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      108 2024-04-17 00:52:46.000000 emtl-0.1.2.dev2/src/emtl/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      354 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/src/emtl/__main__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      424 2024-04-17 01:00:14.000000 emtl-0.1.2.dev2/src/emtl/_version.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1003 2024-04-17 00:52:46.000000 emtl-0.1.2.dev2/src/emtl/cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      169 2024-04-17 00:52:46.000000 emtl-0.1.2.dev2/src/emtl/core.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/src/emtl/tests/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 01:27:17.000000 emtl-0.1.2.dev2/src/emtl/tests/__init__.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      134 2024-04-17 00:52:46.000000 emtl-0.1.2.dev2/src/emtl/tests/test_cli.py
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      235 2024-04-17 00:52:46.000000 emtl-0.1.2.dev2/src/emtl/tests/test_core.py
-drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-17 01:00:14.747292 emtl-0.1.2.dev2/src/emtl.egg-info/
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1992 2024-04-17 01:00:14.000000 emtl-0.1.2.dev2/src/emtl.egg-info/PKG-INFO
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      947 2024-04-17 01:00:14.000000 emtl-0.1.2.dev2/src/emtl.egg-info/SOURCES.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-17 01:00:14.000000 emtl-0.1.2.dev2/src/emtl.egg-info/dependency_links.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-17 01:00:14.000000 emtl-0.1.2.dev2/src/emtl.egg-info/entry_points.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-16 09:34:21.000000 emtl-0.1.2.dev2/src/emtl.egg-info/not-zip-safe
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        5 2024-04-17 01:00:14.000000 emtl-0.1.2.dev2/src/emtl.egg-info/top_level.txt
--rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1637 2024-04-16 06:27:08.000000 emtl-0.1.2.dev2/tox.ini
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      757 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/.bumpversion.cfg
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1901 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/.cookiecutterrc
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      149 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/.coveragerc
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      353 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/.editorconfig
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.737393 emtl-0.1.4.dev1/.github/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/.github/workflows/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      907 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/.github/workflows/document.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     3925 2024-04-19 01:32:21.000000 emtl-0.1.4.dev1/.github/workflows/github-actions.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      734 2024-04-16 01:37:37.000000 emtl-0.1.4.dev1/.gitignore
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      686 2024-04-16 01:27:59.000000 emtl-0.1.4.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      285 2024-04-17 09:47:16.000000 emtl-0.1.4.dev1/.readthedocs.yml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       65 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/AUTHORS.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      235 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/CHANGELOG.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2274 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1117 2024-04-16 01:42:17.000000 emtl-0.1.4.dev1/LICENSE
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2054 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/PKG-INFO
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2251 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/README.rst
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/ci/
+-rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     2867 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/ci/bootstrap.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       72 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/ci/requirements.txt
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.737393 emtl-0.1.4.dev1/ci/templates/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.737393 emtl-0.1.4.dev1/ci/templates/.github/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/ci/templates/.github/workflows/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2179 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/docs/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       28 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/authors.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       30 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/changelog.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1145 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/docs/conf.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       33 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/contributing.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      244 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/index.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       84 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/installation.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       27 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/readme.rst
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/docs/reference/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      146 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/reference/emtl.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       56 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/reference/index.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       17 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/requirements.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      109 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/spelling_wordlist.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       98 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/docs/usage.rst
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1381 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/pyproject.toml
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1303 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/pytest.ini
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/setup.cfg
+-rwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)     3066 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/setup.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/emtl/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      183 2024-04-19 01:29:59.000000 emtl-0.1.4.dev1/src/emtl/__init__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      354 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/src/emtl/__main__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      424 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl/_version.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1003 2024-04-17 00:52:46.000000 emtl-0.1.4.dev1/src/emtl/cli.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1083 2024-04-17 03:52:39.000000 emtl-0.1.4.dev1/src/emtl/const.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     4310 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/src/emtl/core.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/emtl/tests/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-16 01:27:17.000000 emtl-0.1.4.dev1/src/emtl/tests/__init__.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      133 2024-04-17 01:52:16.000000 emtl-0.1.4.dev1/src/emtl/tests/test_cli.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)      624 2024-04-19 01:18:25.000000 emtl-0.1.4.dev1/src/emtl/tests/test_core.py
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1585 2024-04-18 02:05:24.000000 emtl-0.1.4.dev1/src/emtl/utils.py
+drwxr-xr-x   0 zhoubo    (1000) zhoubo    (1000)        0 2024-04-19 01:57:32.747393 emtl-0.1.4.dev1/src/emtl.egg-info/
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     2054 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/PKG-INFO
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1045 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       38 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/entry_points.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        1 2024-04-16 09:34:21.000000 emtl-0.1.4.dev1/src/emtl.egg-info/not-zip-safe
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)       63 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/requires.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)        5 2024-04-19 01:57:32.000000 emtl-0.1.4.dev1/src/emtl.egg-info/top_level.txt
+-rw-r--r--   0 zhoubo    (1000) zhoubo    (1000)     1593 2024-04-17 08:38:27.000000 emtl-0.1.4.dev1/tox.ini
```

### Comparing `emtl-0.1.2.dev2/.cookiecutterrc` & `emtl-0.1.4.dev1/.cookiecutterrc`

 * *Files 1% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     setup_py_uses_setuptools_scm: "yes"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://emtl.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "yes"
     tests_inside_package: "yes"
-    version: "0.1.0"
+    version: "0.1.2"
     version_manager: "bump2version"
     website: "riiy.gihub.io/emtl"
     year_from: "2024"
     year_to: "2025"
```

### Comparing `emtl-0.1.2.dev2/.github/workflows/github-actions.yml` & `emtl-0.1.4.dev1/.github/workflows/github-actions.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 name: build
-on: [push, pull_request, workflow_dispatch]
+on:
+  push:
+    branches:
+    - master
+  pull_request:
+    branches:
+      - master
+  workflow_dispatch:
 jobs:
   test:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
     strategy:
       fail-fast: false
@@ -21,31 +28,55 @@
             os: 'ubuntu-latest'
           - name: 'py310-cover (ubuntu)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310-cover'
             os: 'ubuntu-latest'
+          - name: 'py310-nocov (ubuntu)'
+            python: '3.10'
+            toxpython: 'python3.10'
+            python_arch: 'x64'
+            tox_env: 'py310-nocov'
+            os: 'ubuntu-latest'
+          - name: 'py310-cover (macos)'
+            python: '3.10'
+            toxpython: 'python3.10'
+            python_arch: 'x64'
+            tox_env: 'py310-cover'
+            os: 'macos-latest'
+          - name: 'py310-nocov (macos)'
+            python: '3.10'
+            toxpython: 'python3.10'
+            python_arch: 'x64'
+            tox_env: 'py310-nocov'
+            os: 'macos-latest'
           - name: 'py311-cover (ubuntu)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311-cover'
             os: 'ubuntu-latest'
-          - name: 'py312-cover (ubuntu)'
-            python: '3.12'
-            toxpython: 'python3.12'
+          - name: 'py311-nocov (ubuntu)'
+            python: '3.11'
+            toxpython: 'python3.11'
             python_arch: 'x64'
-            tox_env: 'py312-cover'
+            tox_env: 'py311-nocov'
             os: 'ubuntu-latest'
-          - name: 'py312-cover (macos)'
-            python: '3.12'
-            toxpython: 'python3.12'
+          - name: 'py311-cover (macos)'
+            python: '3.11'
+            toxpython: 'python3.11'
+            python_arch: 'x64'
+            tox_env: 'py311-cover'
+            os: 'macos-latest'
+          - name: 'py311-nocov (macos)'
+            python: '3.11'
+            toxpython: 'python3.11'
             python_arch: 'x64'
-            tox_env: 'py312-cover'
+            tox_env: 'py311-nocov'
             os: 'macos-latest'
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v5
       with:
@@ -57,14 +88,16 @@
         virtualenv --version
         pip --version
         tox --version
         pip list --format=freeze
     - name: test
       env:
         TOXPYTHON: '${{ matrix.toxpython }}'
+        EM_USERNAME: ${{ secrets.EM_USERNAME }}
+        EM_PASSWORD: ${{ secrets.EM_PASSWORD }}
       run: >
         tox -e ${{ matrix.tox_env }} -v
   finish:
     needs: test
     if: ${{ always() }}
     runs-on: ubuntu-latest
     steps:
@@ -82,16 +115,20 @@
         pip --version
         tox --version
         pip list --format=freeze
     - name: test
       env:
         TOXPYTHON: 'python311'
         PYTEST_ADDOPTS: '--cov-append'
+        EM_USERNAME: ${{ secrets.EM_USERNAME }}
+        EM_PASSWORD: ${{ secrets.EM_PASSWORD }}
       run: >
         PYTEST_ADDOPTS=--cov-append tox -e py310-cover -v
     - uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
         verbose: true
       env:
         CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        EM_USERNAME: ${{ secrets.EM_USERNAME }}
+        EM_PASSWORD: ${{ secrets.EM_PASSWORD }}
```

### Comparing `emtl-0.1.2.dev2/.gitignore` & `emtl-0.1.4.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/.pre-commit-config.yaml` & `emtl-0.1.4.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/CONTRIBUTING.rst` & `emtl-0.1.4.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/LICENSE` & `emtl-0.1.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/PKG-INFO` & `emtl-0.1.4.dev1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.1.2.dev2
-Summary: 东方财富交易系统
+Version: 0.1.4.dev1
+Summary: 东方财富自动交易系统
 Home-page: https://github.com/riiy/emtl
 Author: Eastmoney Trade Library
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/riiy/emtl/issues
-Keywords: trade,东方财富,股票,交易
+Keywords: autotrade,trade,东方财富,股票,交易,交易机器人
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
 
 
-东方财富交易系统
+东方财富自动交易系统
 
 * Free software: MIT license
 
 Installation
 ============
 
 ::
@@ -81,14 +80,19 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+0.1.2 (2024-04-18)
+------------------
+
+* add login && add asset position
+
 0.1.1 (2024-04-16)
 ------------------
 
 * Delete python3.8 python3.9 pypy.
 
 0.1.0 (2024-04-14)
 ------------------
```

### Comparing `emtl-0.1.2.dev2/README.rst` & `emtl-0.1.4.dev1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,23 +37,23 @@
     :alt: Supported versions
     :target: https://pypi.org/project/emtl
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/emtl.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/emtl
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.1.1.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/riiy/emtl/v0.1.3.svg
     :alt: Commits since latest release
-    :target: https://github.com/riiy/emtl/compare/v0.1.1...master
+    :target: https://github.com/riiy/emtl/compare/v0.1.3...master
 
 
 
 .. end-badges
 
-东方财富交易系统
+东方财富自动交易系统
 
 * Free software: MIT license
 
 Installation
 ============
 
 ::
```

### Comparing `emtl-0.1.2.dev2/ci/bootstrap.py` & `emtl-0.1.4.dev1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/ci/templates/.github/workflows/github-actions.yml` & `emtl-0.1.4.dev1/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/docs/conf.py` & `emtl-0.1.4.dev1/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+needs_sphinx = "7.2"
+sphinx = "7.2"
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.extlinks",
     "sphinx.ext.ifconfig",
@@ -19,15 +21,15 @@
     from pkg_resources import get_distribution
 
     version = release = get_distribution("emtl").version
 except Exception:
     import traceback
 
     traceback.print_exc()
-    version = release = "0.1.1"
+    version = release = "0.1.3"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/riiy/emtl/issues/%s", "#%s"),
     "pr": ("https://github.com/riiy/emtl/pull/%s", "PR #%s"),
 }
```

### Comparing `emtl-0.1.2.dev2/pyproject.toml` & `emtl-0.1.4.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/pytest.ini` & `emtl-0.1.4.dev1/pytest.ini`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/setup.py` & `emtl-0.1.4.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 
 setup(
     name="emtl",
     use_scm_version={
         "local_scheme": "dirty-tag",
         "write_to": "src/emtl/_version.py",
-        "fallback_version": "0.1.1",
+        "fallback_version": "0.1.3",
     },
     license="MIT",
-    description="东方财富交易系统",
+    description="东方财富自动交易系统",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Eastmoney Trade Library",
     author_email="riiyzhou@gmail.com",
     url="https://github.com/riiy/emtl",
@@ -43,38 +43,38 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         # "Programming Language :: Python :: 3.8",
         # "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
+        # "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         # "Programming Language :: Python :: Implementation :: PyPy",
         # uncomment if you test on these interpreters:
         # "Programming Language :: Python :: Implementation :: IronPython",
         # "Programming Language :: Python :: Implementation :: Jython",
         # "Programming Language :: Python :: Implementation :: Stackless",
         "Topic :: Utilities",
     ],
     project_urls={
         "Documentation": "https://emtl.readthedocs.io/",
         "Changelog": "https://emtl.readthedocs.io/en/latest/changelog.html",
         "Issue Tracker": "https://github.com/riiy/emtl/issues",
     },
     keywords=[
+        "autotrade",
         "trade",
         "东方财富",
         "股票",
         "交易",
+        "交易机器人",
     ],
-    python_requires=">=3.8",
-    install_requires=[
-        # eg: "aspectlib==1.1.1", "six>=1.7",
-    ],
+    python_requires=">=3.10",
+    install_requires=["rsa==4.9", "requests==2.31.0", "ddddocr==1.4.11", "cryptography==42.0.5"],
     extras_require={
         # eg:
         #   "rst": ["docutils>=0.11"],
         #   ":python_version=='3.8'": ["backports.zoneinfo"],
     },
     setup_requires=[
         "setuptools_scm>=3.3.1",
```

### Comparing `emtl-0.1.2.dev2/src/emtl/cli.py` & `emtl-0.1.4.dev1/src/emtl/cli.py`

 * *Files identical despite different names*

### Comparing `emtl-0.1.2.dev2/src/emtl.egg-info/PKG-INFO` & `emtl-0.1.4.dev1/src/emtl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: emtl
-Version: 0.1.2.dev2
-Summary: 东方财富交易系统
+Version: 0.1.4.dev1
+Summary: 东方财富自动交易系统
 Home-page: https://github.com/riiy/emtl
 Author: Eastmoney Trade Library
 Author-email: riiyzhou@gmail.com
 License: MIT
 Project-URL: Documentation, https://emtl.readthedocs.io/
 Project-URL: Changelog, https://emtl.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/riiy/emtl/issues
-Keywords: trade,东方财富,股票,交易
+Keywords: autotrade,trade,东方财富,股票,交易,交易机器人
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
 
 
-东方财富交易系统
+东方财富自动交易系统
 
 * Free software: MIT license
 
 Installation
 ============
 
 ::
@@ -81,14 +80,19 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+0.1.2 (2024-04-18)
+------------------
+
+* add login && add asset position
+
 0.1.1 (2024-04-16)
 ------------------
 
 * Delete python3.8 python3.9 pypy.
 
 0.1.0 (2024-04-14)
 ------------------
```

### Comparing `emtl-0.1.2.dev2/src/emtl.egg-info/SOURCES.txt` & `emtl-0.1.4.dev1/src/emtl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 CONTRIBUTING.rst
 LICENSE
 README.rst
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
+.github/workflows/document.yml
 .github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
@@ -30,17 +31,20 @@
 docs/usage.rst
 docs/reference/emtl.rst
 docs/reference/index.rst
 src/emtl/__init__.py
 src/emtl/__main__.py
 src/emtl/_version.py
 src/emtl/cli.py
+src/emtl/const.py
 src/emtl/core.py
+src/emtl/utils.py
 src/emtl.egg-info/PKG-INFO
 src/emtl.egg-info/SOURCES.txt
 src/emtl.egg-info/dependency_links.txt
 src/emtl.egg-info/entry_points.txt
 src/emtl.egg-info/not-zip-safe
+src/emtl.egg-info/requires.txt
 src/emtl.egg-info/top_level.txt
 src/emtl/tests/__init__.py
 src/emtl/tests/test_cli.py
 src/emtl/tests/test_core.py
```

### Comparing `emtl-0.1.2.dev2/tox.ini` & `emtl-0.1.4.dev1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 
 ; a generative tox configuration, see: https://tox.wiki/en/latest/user_guide.html#generative-environments
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py310,py311,py312}-{cover,nocov},
+    {py310,py311}-{cover,nocov},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
     py310: {env:TOXPYTHON:python3.10}
     py311: {env:TOXPYTHON:python3.11}
-    py312: {env:TOXPYTHON:python3.12}
     {bootstrap,clean,check,report,docs,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop =
```

