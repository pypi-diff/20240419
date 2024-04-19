# Comparing `tmp/requestrepo-0.0.3.tar.gz` & `tmp/requestrepo-0.0.4.tar.gz`

## Comparing `requestrepo-0.0.3.tar` & `requestrepo-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 requestrepo-0.0.3/requirements.txt
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 requestrepo-0.0.3/src/requestrepo/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 requestrepo-0.0.3/LICENSE
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 requestrepo-0.0.3/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 requestrepo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 requestrepo-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 requestrepo-0.0.4/src/requestrepo/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 requestrepo-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 requestrepo-0.0.4/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 requestrepo-0.0.4/PKG-INFO
```

### Comparing `requestrepo-0.0.3/.gitignore` & `requestrepo-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.3/LICENSE` & `requestrepo-0.0.4/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 adragos
+Copyright (c) 2024 Dragos Albastroiu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `requestrepo-0.0.3/README.md` & `requestrepo-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.3/pyproject.toml` & `requestrepo-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "requestrepo"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Dragos Albastroiu", email = "adragos@protonmail.com" }]
 description = "Python bindings to automate requestrepo.com"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `requestrepo-0.0.3/PKG-INFO` & `requestrepo-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: requestrepo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python bindings to automate requestrepo.com
 Project-URL: Homepage, https://github.com/adrgs/requestrepo-lib
 Project-URL: Issues, https://github.com/adrgs/requestrepo-lib/issues
 Author-email: Dragos Albastroiu <adragos@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

