# Comparing `tmp/more_decorators-0.1.0.tar.gz` & `tmp/more_decorators-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "more_decorators-0.1.0.tar", max compression
+gzip compressed data, was "more_decorators-0.1.1.tar", max compression
```

## Comparing `more_decorators-0.1.0.tar` & `more_decorators-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1055 2024-03-13 05:05:07.485933 more_decorators-0.1.0/LICENSE
--rw-r--r--   0        0        0       25 2024-03-13 05:05:07.485933 more_decorators-0.1.0/README.md
--rw-r--r--   0        0        0     1271 2024-03-13 05:05:07.485933 more_decorators-0.1.0/more_decorators/runtime_defaults.py
--rw-r--r--   0        0        0     1047 2024-03-13 05:05:43.481909 more_decorators-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 more_decorators-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2024-04-19 16:56:23.293957 more_decorators-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1210 2024-04-19 16:56:23.293957 more_decorators-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 16:56:23.293957 more_decorators-0.1.1/more_decorators/__init__.py
+-rw-r--r--   0        0        0     2349 2024-04-19 16:56:23.293957 more_decorators-0.1.1/more_decorators/runtime_defaults.py
+-rw-r--r--   0        0        0     2214 2024-04-19 16:56:43.714089 more_decorators-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 more_decorators-0.1.1/PKG-INFO
```

### Comparing `more_decorators-0.1.0/LICENSE` & `more_decorators-0.1.1/LICENSE`

 * *Files identical despite different names*

