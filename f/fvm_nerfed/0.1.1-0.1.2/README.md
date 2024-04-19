# Comparing `tmp/fvm_nerfed-0.1.1.tar.gz` & `tmp/fvm_nerfed-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fvm_nerfed-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fvm_nerfed-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fvm_nerfed-0.1.1.tar` & `fvm_nerfed-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       42 2024-04-18 23:48:45.925824 fvm_nerfed-0.1.1/.gitignore
--rw-r--r--   0        0        0      256 2024-04-18 23:19:52.471230 fvm_nerfed-0.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     1448 2024-04-18 23:38:37.816380 fvm_nerfed-0.1.1/README.md
--rw-r--r--   0        0        0      130 2024-04-18 23:50:47.277712 fvm_nerfed-0.1.1/fvm_nerfed/__init__.py
--rwxr-xr-x   0        0        0     2315 2024-04-18 23:19:52.473718 fvm_nerfed-0.1.1/fvm_nerfed/fvm-nerfed.py
--rw-r--r--   0        0        0      437 2024-04-18 23:39:43.213442 fvm_nerfed-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 fvm_nerfed-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2024-04-18 23:48:45.925824 fvm_nerfed-0.1.2/.gitignore
+-rw-r--r--   0        0        0      256 2024-04-18 23:19:52.471230 fvm_nerfed-0.1.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1448 2024-04-18 23:38:37.816380 fvm_nerfed-0.1.2/README.md
+-rw-r--r--   0        0        0       90 2024-04-18 23:52:10.749546 fvm_nerfed-0.1.2/fvm_nerfed/__init__.py
+-rwxr-xr-x   0        0        0     2315 2024-04-18 23:19:52.473718 fvm_nerfed-0.1.2/fvm_nerfed/fvm-nerfed.py
+-rw-r--r--   0        0        0      437 2024-04-18 23:39:43.213442 fvm_nerfed-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1692 1970-01-01 00:00:00.000000 fvm_nerfed-0.1.2/PKG-INFO
```

### Comparing `fvm_nerfed-0.1.1/README.md` & `fvm_nerfed-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fvm_nerfed-0.1.1/fvm_nerfed/fvm-nerfed.py` & `fvm_nerfed-0.1.2/fvm_nerfed/fvm-nerfed.py`

 * *Files identical despite different names*

### Comparing `fvm_nerfed-0.1.1/PKG-INFO` & `fvm_nerfed-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvm_nerfed
-Version: 0.1.1
+Version: 0.1.2
 Summary: Feather Virtual Machine (FVM)
 Author-email: $wryl <wryl@wryl.tech>
 Maintainer-email: "Justin \"Boonie Pepper\" Hill" <justin@so.dang.cool>
 Description-Content-Type: text/markdown
 
 # FVM bitcode evaluator
```

