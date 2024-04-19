# Comparing `tmp/fvm-0.1.0.tar.gz` & `tmp/fvm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fvm-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fvm-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fvm-0.1.0.tar` & `fvm-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       57 2024-04-19 14:54:01.865012 fvm-0.1.0/.gitignore
--rw-r--r--   0        0        0      256 2024-04-19 14:43:58.541005 fvm-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1632 2024-04-19 14:43:58.542004 fvm-0.1.0/README.md
--rw-r--r--   0        0        0       82 2024-04-19 14:58:12.219014 fvm-0.1.0/fvm/__init__.py
--rwxr-xr-x   0        0        0     2315 2024-04-15 23:52:25.508931 fvm-0.1.0/fvm/run.py
--rw-r--r--   0        0        0      466 2024-04-19 14:58:05.214014 fvm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 fvm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-04-19 14:54:01.865012 fvm-0.1.1/.gitignore
+-rw-r--r--   0        0        0      435 2024-04-19 15:06:47.692020 fvm-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1625 2024-04-19 15:06:28.835020 fvm-0.1.1/README.md
+-rw-r--r--   0        0        0       82 2024-04-19 15:07:43.367021 fvm-0.1.1/fvm/__init__.py
+-rwxr-xr-x   0        0        0     2315 2024-04-15 23:52:25.508931 fvm-0.1.1/fvm/run.py
+-rw-r--r--   0        0        0      466 2024-04-19 14:58:05.214014 fvm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 fvm-0.1.1/PKG-INFO
```

### Comparing `fvm-0.1.0/README.md` & `fvm-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 https://hub.docker.com/r/booniepepper/fvm
 
 Packaging is performed by GitLab CI.
 
 ## PyPI
 
-https://pypi.org/project/fvm-nerfed/
+https://pypi.org/project/fvm/
 
 Packaging is performed by GitLab CI.
 
 ## As a discord bot
 
 This docker image is the FVM runtime used for a discord
 bot running on the concatenative programming discord server.
```

### Comparing `fvm-0.1.0/fvm/run.py` & `fvm-0.1.1/fvm/run.py`

 * *Files identical despite different names*

### Comparing `fvm-0.1.0/PKG-INFO` & `fvm-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fvm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Feather Virtual Machine (FVM)
 Author-email: $wryl <wryl@wryl.tech>
 Maintainer-email: "Justin \"Boonie Pepper\" Hill" <justin@so.dang.cool>
 Description-Content-Type: text/markdown
 Project-URL: source, https://gitlab.com/feather-lang/fvm
 
 # FVM bitcode evaluator
@@ -42,15 +42,15 @@
 
 https://hub.docker.com/r/booniepepper/fvm
 
 Packaging is performed by GitLab CI.
 
 ## PyPI
 
-https://pypi.org/project/fvm-nerfed/
+https://pypi.org/project/fvm/
 
 Packaging is performed by GitLab CI.
 
 ## As a discord bot
 
 This docker image is the FVM runtime used for a discord
 bot running on the concatenative programming discord server.
```

