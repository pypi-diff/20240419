# Comparing `tmp/pip_blame-0.1.0.tar.gz` & `tmp/pip_blame-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_blame-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pip_blame-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_blame-0.1.0.tar` & `pip_blame-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        5 2024-04-12 22:44:10.475997 pip_blame-0.1.0/.gitignore
--rw-r--r--   0        0        0     1143 2024-04-12 22:50:30.959347 pip_blame-0.1.0/pip_blame.py
--rw-r--r--   0        0        0      516 2024-04-12 22:59:07.275834 pip_blame-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      471 2024-04-12 22:58:31.051761 pip_blame-0.1.0/readme.md
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 pip_blame-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-12 22:44:10.475997 pip_blame-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3007 2024-04-19 09:50:02.312330 pip_blame-0.2.0/pip_blame.py
+-rw-r--r--   0        0        0      516 2024-04-19 09:49:04.445982 pip_blame-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1618 2024-04-19 08:48:02.594338 pip_blame-0.2.0/readme.md
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 pip_blame-0.2.0/PKG-INFO
```

### Comparing `pip_blame-0.1.0/pyproject.toml` & `pip_blame-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "requests >=2.31",
   "rich >=13.7.1",
 ]
 description = "finds packages that prevent upgrading a transitive dependency"
 name = "pip-blame"
 readme = 'readme.md'
 requires-python = ">=3.8"
-version = "0.1.0"
+version = "0.2.0"
 
 [tool.flit.module]
 name = "pip_blame"
 
 [project.urls]
 Home = "https://github.com/banteg/pip-blame"
```

