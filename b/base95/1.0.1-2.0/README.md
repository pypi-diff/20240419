# Comparing `tmp/base95-1.0.1.tar.gz` & `tmp/base95-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base95-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "base95-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `base95-1.0.1.tar` & `base95-2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11275 2024-04-13 03:33:01.837811 base95-1.0.1/LICENSE
--rw-r--r--   0        0        0     2690 2024-04-13 13:22:26.084398 base95-1.0.1/README.md
--rw-r--r--   0        0        0       33 2024-04-13 03:21:49.855973 base95-1.0.1/__init__.py
--rw-r--r--   0        0        0     1822 2024-04-13 04:05:56.297240 base95-1.0.1/_core.py
--rw-r--r--   0        0        0       98 2024-04-13 08:02:33.643534 base95-1.0.1/art.json
--rw-r--r--   0        0        0       44 2024-04-13 03:22:45.204180 base95-1.0.1/base95.py
--rw-r--r--   0        0        0      674 2024-04-14 08:05:13.889778 base95-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 base95-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11275 2024-04-13 03:33:01.837811 base95-2.0/LICENSE
+-rw-r--r--   0        0        0     2678 2024-04-19 09:42:08.567290 base95-2.0/README.md
+-rw-r--r--   0        0        0       63 2024-04-19 09:19:32.694427 base95-2.0/__init__.py
+-rw-r--r--   0        0        0     3553 2024-04-19 09:19:14.294026 base95-2.0/_core.py
+-rw-r--r--   0        0        0       98 2024-04-13 08:02:33.643534 base95-2.0/art.json
+-rw-r--r--   0        0        0       74 2024-04-19 09:19:40.646468 base95-2.0/base95.py
+-rw-r--r--   0        0        0      672 2024-04-19 09:47:07.876329 base95-2.0/pyproject.toml
+-rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 base95-2.0/PKG-INFO
```

### Comparing `base95-1.0.1/LICENSE` & `base95-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `base95-1.0.1/pyproject.toml` & `base95-2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "base95"
-version = "1.0.1"
+version = "2.0"
 description = "Base95 是一种用 95 个可见的 ASCII 字符（含空格）表示任意二进制数据的编码方法，编码后的信息密度高于 Base64 编码。"
-dependencies = ["arts>=2024.4.13"]
+dependencies = ["arts>=2024.4.19"]
 keywords = ["base64", "base85", "base95"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

