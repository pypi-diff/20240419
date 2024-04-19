# Comparing `tmp/seqprocessor-0.1.0.tar.gz` & `tmp/seqprocessor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqprocessor-0.1.0.tar", max compression
+gzip compressed data, was "seqprocessor-0.1.1.tar", max compression
```

## Comparing `seqprocessor-0.1.0.tar` & `seqprocessor-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      482 2024-04-14 10:41:33.731398 seqprocessor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       16 2024-04-14 10:55:59.389946 seqprocessor-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-13 11:53:41.434474 seqprocessor-0.1.0/seqprocessor/__init__.py
--rw-r--r--   0        0        0      194 2024-04-14 10:55:11.236545 seqprocessor-0.1.0/seqprocessor/main.py
--rw-r--r--   0        0        0      118 2024-04-13 13:15:00.933190 seqprocessor-0.1.0/seqprocessor/options.py
--rw-r--r--   0        0        0        0 2024-04-14 10:50:53.969059 seqprocessor-0.1.0/seqprocessor/seq/__init__.py
--rw-r--r--   0        0        0     4327 2024-04-14 10:55:20.345850 seqprocessor-0.1.0/seqprocessor/seq/info.py
--rw-r--r--   0        0        0      637 2024-04-14 10:55:28.914659 seqprocessor-0.1.0/seqprocessor/utils.py
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 seqprocessor-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2024-04-15 06:48:57.446696 seqprocessor-0.1.1/README.md
+-rwxr-xr-x   0        0        0      504 2024-04-19 05:20:39.751102 seqprocessor-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-04-15 06:48:18.998387 seqprocessor-0.1.1/seqprocessor/__init__.py
+-rwxr-xr-x   0        0        0      326 2024-04-15 08:59:31.839970 seqprocessor-0.1.1/seqprocessor/main.py
+-rwxr-xr-x   0        0        0      118 2024-04-15 06:48:18.999386 seqprocessor-0.1.1/seqprocessor/options.py
+-rwxr-xr-x   0        0        0        0 2024-04-15 06:48:19.000405 seqprocessor-0.1.1/seqprocessor/seq/__init__.py
+-rwxr-xr-x   0        0        0     3100 2024-04-15 08:44:35.871290 seqprocessor-0.1.1/seqprocessor/seq/info.py
+-rwxr-xr-x   0        0        0     7755 2024-04-19 05:18:20.464621 seqprocessor-0.1.1/seqprocessor/seq/pretreat.py
+-rwxr-xr-x   0        0        0     1316 2024-04-15 11:30:12.162660 seqprocessor-0.1.1/seqprocessor/utils.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 seqprocessor-0.1.1/PKG-INFO
```

