# Comparing `tmp/precommend-0.2.1.tar.gz` & `tmp/precommend-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precommend-0.2.1.tar", last modified: Thu Mar 21 12:42:29 2024, max compression
+gzip compressed data, was "precommend-0.2.2.tar", last modified: Fri Apr 19 08:50:28 2024, max compression
```

## Comparing `precommend-0.2.1.tar` & `precommend-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.123643 precommend-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.115643 precommend-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 12:42:25.000000 precommend-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-21 12:42:25.000000 precommend-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-21 12:42:25.000000 precommend-0.2.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-21 12:42:25.000000 precommend-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-21 12:42:25.000000 precommend-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-21 12:42:25.000000 precommend-0.2.1/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-21 12:42:25.000000 precommend-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-21 12:42:25.000000 precommend-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-21 12:42:29.119643 precommend-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-21 12:42:25.000000 precommend-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/precommend/
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-21 12:42:25.000000 precommend-0.2.1/precommend/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 12:42:25.000000 precommend-0.2.1/precommend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-21 12:42:25.000000 precommend-0.2.1/precommend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-21 12:42:29.000000 precommend-0.2.1/precommend/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-21 12:42:25.000000 precommend-0.2.1/precommend/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-21 12:42:25.000000 precommend-0.2.1/precommend/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/precommend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-21 12:42:29.000000 precommend-0.2.1/precommend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-21 12:42:29.000000 precommend-0.2.1/precommend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 12:42:29.000000 precommend-0.2.1/precommend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-21 12:42:29.000000 precommend-0.2.1/precommend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-21 12:42:29.000000 precommend-0.2.1/precommend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 12:42:29.000000 precommend-0.2.1/precommend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-21 12:42:25.000000 precommend-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 12:42:29.123643 precommend-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-21 12:42:25.000000 precommend-0.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-21 12:42:25.000000 precommend-0.2.1/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.115643 precommend-0.2.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/tests/data/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/data/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/data/cpp/test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/tests/data/generic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/tests/data/generic/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/data/generic/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/tests/data/generic/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/data/generic/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/data/generic/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:29.119643 precommend-0.2.1/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/data/python/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/data/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-21 12:42:25.000000 precommend-0.2.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 08:50:23.000000 precommend-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-19 08:50:23.000000 precommend-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-19 08:50:23.000000 precommend-0.2.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-19 08:50:23.000000 precommend-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 08:50:23.000000 precommend-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-19 08:50:23.000000 precommend-0.2.2/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 08:50:23.000000 precommend-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 08:50:23.000000 precommend-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-19 08:50:28.472251 precommend-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 08:50:23.000000 precommend-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/precommend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-19 08:50:23.000000 precommend-0.2.2/precommend/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/precommend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 08:50:28.000000 precommend-0.2.2/precommend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 08:50:23.000000 precommend-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:50:28.472251 precommend-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 08:50:23.000000 precommend-0.2.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 08:50:23.000000 precommend-0.2.2/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.468251 precommend-0.2.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/cpp/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/generic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/generic/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/generic/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/generic/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/generic/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/generic/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:28.472251 precommend-0.2.2/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/python/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/data/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-19 08:50:23.000000 precommend-0.2.2/tests/test_core.py
```

### Comparing `precommend-0.2.1/.github/workflows/ci.yml` & `precommend-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/.github/workflows/pypi.yml` & `precommend-0.2.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/.gitignore` & `precommend-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/.pre-commit-config.yaml` & `precommend-0.2.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
         name: Synchronize files within the repository
         entry: python sync.py
         language: system
         always_run: true
         pass_filenames: false
 
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.0
     hooks:
       - id: black  # Run Black - the uncompromising Python code formatter
       - id: black-jupyter  # Run Black - the uncompromising Python code formatter (Jupyter version)
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: end-of-file-fixer  # Ensure existence of newline characters at file ends
       - id: check-yaml  # Make sure that contained YAML files are well-formed
       - id: trailing-whitespace  # Trim trailing whitespace of all sorts
       - id: check-added-large-files  # Apply a file size limit of 500kB
       - id: check-toml  # Simple parser validation of e.g. pyproject.toml
       - id: requirements-txt-fixer  # Sort lines in requirements files
@@ -53,15 +53,15 @@
     hooks:
       - id: cmake-format  # Apply formatting to CMake files
         additional_dependencies:
           - pyyaml
       - id: cmake-lint  # Apply linting to CMake files
 
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.1
+    rev: v18.1.3
     hooks:
       - id: clang-format  # Format C++ code with Clang-Format - automatically applying the changes
         types_or: [c++, c, c#, cuda, objective-c]
         args:
         - --style=Mozilla
 
   - repo: https://github.com/asottile/setup-cfg-fmt
@@ -81,11 +81,11 @@
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.16
     hooks:
       - id: validate-pyproject  # Validate the contents of pyproject.toml
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.2
     hooks:
       - id: check-readthedocs  # Validate the given .readthedocs.yml file
       - id: check-dependabot  # Validate the given dependabot.yml file
```

### Comparing `precommend-0.2.1/LICENSE.md` & `precommend-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/PKG-INFO` & `precommend-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.2.1
+Version: 0.2.2
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `precommend-0.2.1/README.md` & `precommend-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/precommend/.pre-commit-config.yaml` & `precommend-0.2.2/precommend/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
         name: Synchronize files within the repository
         entry: python sync.py
         language: system
         always_run: true
         pass_filenames: false
 
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.0
     hooks:
       - id: black  # Run Black - the uncompromising Python code formatter
       - id: black-jupyter  # Run Black - the uncompromising Python code formatter (Jupyter version)
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: end-of-file-fixer  # Ensure existence of newline characters at file ends
       - id: check-yaml  # Make sure that contained YAML files are well-formed
       - id: trailing-whitespace  # Trim trailing whitespace of all sorts
       - id: check-added-large-files  # Apply a file size limit of 500kB
       - id: check-toml  # Simple parser validation of e.g. pyproject.toml
       - id: requirements-txt-fixer  # Sort lines in requirements files
@@ -53,15 +53,15 @@
     hooks:
       - id: cmake-format  # Apply formatting to CMake files
         additional_dependencies:
           - pyyaml
       - id: cmake-lint  # Apply linting to CMake files
 
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.1
+    rev: v18.1.3
     hooks:
       - id: clang-format  # Format C++ code with Clang-Format - automatically applying the changes
         types_or: [c++, c, c#, cuda, objective-c]
         args:
         - --style=Mozilla
 
   - repo: https://github.com/asottile/setup-cfg-fmt
@@ -81,11 +81,11 @@
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.16
     hooks:
       - id: validate-pyproject  # Validate the contents of pyproject.toml
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.2
     hooks:
       - id: check-readthedocs  # Validate the given .readthedocs.yml file
       - id: check-dependabot  # Validate the given dependabot.yml file
```

### Comparing `precommend-0.2.1/precommend/__main__.py` & `precommend-0.2.2/precommend/__main__.py`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/precommend/core.py` & `precommend-0.2.2/precommend/core.py`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/precommend/rules.py` & `precommend-0.2.2/precommend/rules.py`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/precommend.egg-info/PKG-INFO` & `precommend-0.2.2/precommend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.2.1
+Version: 0.2.2
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `precommend-0.2.1/precommend.egg-info/SOURCES.txt` & `precommend-0.2.2/precommend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/pyproject.toml` & `precommend-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `precommend-0.2.1/tests/test_core.py` & `precommend-0.2.2/tests/test_core.py`

 * *Files identical despite different names*

