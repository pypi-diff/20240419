# Comparing `tmp/zro2-0.1.0.tar.gz` & `tmp/zro2-0.2.0b1.tar.gz`

## Comparing `zro2-0.1.0.tar` & `zro2-0.2.0b1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zro2-0.1.0/.gitattributes
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zro2-0.1.0/.python-version
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 zro2-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zro2-0.1.0/requirements.lock
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 zro2-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/hashlib.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/json.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/keyring.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/logging.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/pygetwindow.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/readchar.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/requests.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/screeninfo.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/subprocess.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 zro2-0.1.0/src/zro2/typing.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 zro2-0.1.0/tests/test_readchar.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zro2-0.1.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zro2-0.1.0/README.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 zro2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 zro2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.gitattributes
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.python-version
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 zro2-0.2.0b1/CHANGELOG
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 zro2-0.2.0b1/cli.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 zro2-0.2.0b1/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zro2-0.2.0b1/requirements.lock
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.vscode/settings.json
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/hashlib.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/io.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/json.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/keyring.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/logging.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/pygetwindow.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/readchar.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/requests.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/screeninfo.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/subprocess.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/typing.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 zro2-0.2.0b1/tests/test_readchar.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.gitignore
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 zro2-0.2.0b1/README.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 zro2-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 zro2-0.2.0b1/PKG-INFO
```

### Comparing `zro2-0.1.0/requirements-dev.lock` & `zro2-0.2.0b1/requirements-dev.lock`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
+click==8.1.7
 colorama==0.4.6
+    # via click
     # via pytest
 iniconfig==2.0.0
     # via pytest
 jaraco-classes==3.4.0
     # via keyring
 jaraco-context==5.3.0
     # via keyring
@@ -32,7 +34,8 @@
 pytest==8.1.1
 pywin32-ctypes==0.2.2
     # via keyring
 readchar==4.0.6
 screeninfo==0.8.1
 setuptools==69.5.1
     # via readchar
+toml==0.10.2
```

### Comparing `zro2-0.1.0/src/zro2/hashlib.py` & `zro2-0.2.0b1/src/zro2/hashlib.py`

 * *Files identical despite different names*

### Comparing `zro2-0.1.0/src/zro2/pygetwindow.py` & `zro2-0.2.0b1/src/zro2/pygetwindow.py`

 * *Files identical despite different names*

### Comparing `zro2-0.1.0/src/zro2/readchar.py` & `zro2-0.2.0b1/src/zro2/readchar.py`

 * *Files identical despite different names*

### Comparing `zro2-0.1.0/src/zro2/screeninfo.py` & `zro2-0.2.0b1/src/zro2/screeninfo.py`

 * *Files identical despite different names*

### Comparing `zro2-0.1.0/src/zro2/subprocess.py` & `zro2-0.2.0b1/src/zro2/subprocess.py`

 * *Files identical despite different names*

### Comparing `zro2-0.1.0/src/zro2/typing.py` & `zro2-0.2.0b1/src/zro2/typing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
     target_commitish: str
     name: str
     draft: bool
     prerelease: bool
     assets: typing.List[GithubAsset]
     tarball_url: str
     zipball_url: str
-    body: str
+    body: str
```

### Comparing `zro2-0.1.0/tests/test_readchar.py` & `zro2-0.2.0b1/tests/test_readchar.py`

 * *Files identical despite different names*

### Comparing `zro2-0.1.0/.gitignore` & `zro2-0.2.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `zro2-0.1.0/README.md` & `zro2-0.2.0b1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 # ZrO2
 util functions for projects
 
 ## Features
 This module contains a series of files, each providing extended utility functions specific to the module that it named. The goal is to primarily utilize standard libraries to ensure maximum compatibility. This project does not introduce additional dependencies. However, some files may require extra dependencies and co-dependencies. Please refer to the table below for detailed information.
 
+## Install
+### by pypi
+
+```bash
+pip install zro2
+```
+
+### by github
+
+```bash
+pip install git+https://github.com/ZackaryW/ZrO2.git
+```
+
+## Index
 
 | File        | Non Std Dependencies    | Co-dependencies |
 | ----------- | ----------------------- | --------------- |
 | hashlib     | [None]                  | [None]          |
 | json        | [None]                  | [None]          |
 | logging     | [None]                  | [None]          |
 | pygetwindow | pygetwindow             | sceeninfo       |
 | requests    | [None]                  | [None]          |
 | screeninfo  | screeninfo, pygetwindow | [None]          |
 | typing      | [None]                  | [None]          |
 | subprocess  | [None]                  | [None]          |
-| keyring     | keyring                 | [None]          |
+| keyring     | keyring                 | [None]          |
+| io          | pyyaml, toml            | [None]          |
+
+## Update cycles
+1. by default, this project will update util functions every 30 days (month)
+2. a beta release will be made available each week
+
```

