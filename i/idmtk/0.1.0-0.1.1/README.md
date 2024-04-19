# Comparing `tmp/idmtk-0.1.0.tar.gz` & `tmp/idmtk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idmtk-0.1.0.tar", max compression
+gzip compressed data, was "idmtk-0.1.1.tar", max compression
```

## Comparing `idmtk-0.1.0.tar` & `idmtk-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650796 idmtk-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650757 idmtk-0.1.0/idmtk/__init__.py
--rw-r--r--   0        0        0      272 2024-04-18 11:58:11.899918 idmtk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 idmtk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650796 idmtk-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 11:57:54.650757 idmtk-0.1.1/idmtk/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-19 02:59:10.847663 idmtk-0.1.1/idmtk/auth.py
+-rw-r--r--   0        0        0      320 2024-04-19 02:50:55.137937 idmtk-0.1.1/idmtk/models.py
+-rw-r--r--   0        0        0      313 2024-04-19 03:01:32.716029 idmtk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 idmtk-0.1.1/PKG-INFO
```

