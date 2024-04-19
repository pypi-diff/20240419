# Comparing `tmp/fvm_nerfed-0.1.3.tar.gz` & `tmp/fvm_nerfed-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fvm_nerfed-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fvm_nerfed-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fvm_nerfed-0.1.3.tar` & `fvm_nerfed-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       42 2024-04-18 23:48:45.925824 fvm_nerfed-0.1.3/.gitignore
--rw-r--r--   0        0        0      256 2024-04-18 23:19:52.471230 fvm_nerfed-0.1.3/.gitlab-ci.yml
--rw-r--r--   0        0        0     1448 2024-04-18 23:38:37.816380 fvm_nerfed-0.1.3/README.md
--rw-r--r--   0        0        0      111 2024-04-19 00:01:35.758852 fvm_nerfed-0.1.3/fvm_nerfed/__init__.py
--rwxr-xr-x   0        0        0     2315 2024-04-18 23:19:52.473718 fvm_nerfed-0.1.3/fvm_nerfed/fvm-nerfed.py
--rw-r--r--   0        0        0      437 2024-04-18 23:39:43.213442 fvm_nerfed-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 fvm_nerfed-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       42 2024-04-18 23:48:45.925824 fvm_nerfed-0.1.4/.gitignore
+-rw-r--r--   0        0        0      256 2024-04-18 23:19:52.471230 fvm_nerfed-0.1.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1448 2024-04-18 23:38:37.816380 fvm_nerfed-0.1.4/README.md
+-rw-r--r--   0        0        0       81 2024-04-19 00:02:30.377433 fvm_nerfed-0.1.4/fvm_nerfed/__init__.py
+-rwxr-xr-x   0        0        0     2315 2024-04-18 23:19:52.473718 fvm_nerfed-0.1.4/fvm_nerfed/fvm-nerfed.py
+-rw-r--r--   0        0        0      437 2024-04-18 23:39:43.213442 fvm_nerfed-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 fvm_nerfed-0.1.4/PKG-INFO
```

### Comparing `fvm_nerfed-0.1.3/README.md` & `fvm_nerfed-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fvm_nerfed-0.1.3/fvm_nerfed/fvm-nerfed.py` & `fvm_nerfed-0.1.4/fvm_nerfed/fvm-nerfed.py`

 * *Files identical despite different names*

### Comparing `fvm_nerfed-0.1.3/PKG-INFO` & `fvm_nerfed-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvm_nerfed
-Version: 0.1.3
+Version: 0.1.4
 Summary: Feather Virtual Machine (FVM)
 Author-email: $wryl <wryl@wryl.tech>
 Maintainer-email: "Justin \"Boonie Pepper\" Hill" <justin@so.dang.cool>
 Description-Content-Type: text/markdown
 
 # FVM bitcode evaluator
```

