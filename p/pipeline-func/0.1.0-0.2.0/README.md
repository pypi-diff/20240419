# Comparing `tmp/pipeline_func-0.1.0.tar.gz` & `tmp/pipeline_func-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_func-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pipeline_func-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pipeline_func-0.1.0.tar` & `pipeline_func-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2106 2024-04-04 17:38:36.110997 pipeline_func-0.1.0/README.md
--rw-r--r--   0        0        0      334 2024-04-04 17:38:37.070995 pipeline_func-0.1.0/pipeline_func.py
--rw-r--r--   0        0        0     1341 2024-04-04 17:38:36.110997 pipeline_func-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 pipeline_func-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3490 2024-04-19 16:11:29.741601 pipeline_func-0.2.0/README.md
+-rw-r--r--   0        0        0     2748 2024-04-19 16:11:30.649602 pipeline_func-0.2.0/pipeline_func.py
+-rw-r--r--   0        0        0     1340 2024-04-19 16:11:29.741601 pipeline_func-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4193 1970-01-01 00:00:00.000000 pipeline_func-0.2.0/PKG-INFO
```

### Comparing `pipeline_func-0.1.0/pyproject.toml` & `pipeline_func-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -48,8 +48,8 @@
     "^\\s*raise AssertionError\\b",
     "^\\s*raise NotImplementedError\\b",
 ]
 
 [tool.semantic_release]
 version_variables = ['pipeline_func.py:__version__']
 build_command = 'python -m pip install build && python -m build'
-major_on_zero = false
+major_on_zero = true
```

