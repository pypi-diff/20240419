# Comparing `tmp/markdown-mdantic-2.1.0.tar.gz` & `tmp/markdown-mdantic-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-mdantic-2.1.0.tar", last modified: Thu Oct 19 07:26:02 2023, max compression
+gzip compressed data, was "markdown-mdantic-2.1.1.tar", last modified: Fri Apr 19 09:16:08 2024, max compression
```

## Comparing `markdown-mdantic-2.1.0.tar` & `markdown-mdantic-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2023-10-19 07:26:02.725365 markdown-mdantic-2.1.0/
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1519 2022-10-24 01:19:36.000000 markdown-mdantic-2.1.0/LICENSE
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     3159 2023-10-19 07:26:02.725365 markdown-mdantic-2.1.0/PKG-INFO
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     2363 2023-10-19 07:25:09.000000 markdown-mdantic-2.1.0/README.md
-drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2023-10-19 07:26:02.725365 markdown-mdantic-2.1.0/markdown_mdantic.egg-info/
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     3159 2023-10-19 07:26:02.000000 markdown-mdantic-2.1.0/markdown_mdantic.egg-info/PKG-INFO
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)      247 2023-10-19 07:26:02.000000 markdown-mdantic-2.1.0/markdown_mdantic.egg-info/SOURCES.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        1 2023-10-19 07:26:02.000000 markdown-mdantic-2.1.0/markdown_mdantic.egg-info/dependency_links.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       37 2023-10-19 07:26:02.000000 markdown-mdantic-2.1.0/markdown_mdantic.egg-info/requires.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        8 2023-10-19 07:26:02.000000 markdown-mdantic-2.1.0/markdown_mdantic.egg-info/top_level.txt
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       38 2023-10-19 07:26:02.725365 markdown-mdantic-2.1.0/setup.cfg
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1131 2023-10-19 07:22:48.000000 markdown-mdantic-2.1.0/setup.py
-drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2023-10-19 07:26:02.725365 markdown-mdantic-2.1.0/tests/
--rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     4527 2023-10-19 07:21:04.000000 markdown-mdantic-2.1.0/tests/test_analyze.py
+drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2024-04-19 09:16:08.656854 markdown-mdantic-2.1.1/
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1519 2023-08-31 12:16:03.000000 markdown-mdantic-2.1.1/LICENSE
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     3241 2024-04-19 09:16:08.656854 markdown-mdantic-2.1.1/PKG-INFO
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     2363 2024-04-19 09:04:34.000000 markdown-mdantic-2.1.1/README.md
+drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2024-04-19 09:16:08.656854 markdown-mdantic-2.1.1/markdown_mdantic.egg-info/
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     3241 2024-04-19 09:16:08.000000 markdown-mdantic-2.1.1/markdown_mdantic.egg-info/PKG-INFO
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)      305 2024-04-19 09:16:08.000000 markdown-mdantic-2.1.1/markdown_mdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        1 2024-04-19 09:16:08.000000 markdown-mdantic-2.1.1/markdown_mdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       37 2024-04-19 09:16:08.000000 markdown-mdantic-2.1.1/markdown_mdantic.egg-info/requires.txt
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)        8 2024-04-19 09:16:08.000000 markdown-mdantic-2.1.1/markdown_mdantic.egg-info/top_level.txt
+drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2024-04-19 09:16:08.656854 markdown-mdantic-2.1.1/mdantic/
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)      240 2024-04-19 09:04:34.000000 markdown-mdantic-2.1.1/mdantic/__init__.py
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     5198 2024-04-19 09:04:34.000000 markdown-mdantic-2.1.1/mdantic/mdantic.py
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     2590 2024-04-19 09:04:34.000000 markdown-mdantic-2.1.1/mdantic/samples.py
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)       38 2024-04-19 09:16:08.656854 markdown-mdantic-2.1.1/setup.cfg
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     1129 2024-04-19 09:12:11.000000 markdown-mdantic-2.1.1/setup.py
+drwxr-xr-x   0 adv_zxy   (1000) adv_zxy   (1000)        0 2024-04-19 09:16:08.656854 markdown-mdantic-2.1.1/tests/
+-rw-r--r--   0 adv_zxy   (1000) adv_zxy   (1000)     4527 2024-04-19 09:04:34.000000 markdown-mdantic-2.1.1/tests/test_analyze.py
```

### Comparing `markdown-mdantic-2.1.0/LICENSE` & `markdown-mdantic-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-mdantic-2.1.0/PKG-INFO` & `markdown-mdantic-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-mdantic
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python-Markdown extension for rendering pydantic BaseModel as table
 Home-page: https://github.com/frefreak/mdantic
 Author: Xiangyu Zhu
 Author-email: frefreak.zxy@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Filters
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: markdown>=3.0
+Requires-Dist: tabulate
+Requires-Dist: pydantic>=2.0
 
 # Mdantic
 
 This is an extension to [Python-Markdown](https://python-markdown.github.io/). It adds a new syntax so that you can reference a [pydantic](https://pydantic-docs.helpmanual.io/) `BaseModel` and translate its fields to a markdown table. (Get the name?) I originally make this to generate http api parameter tables with [mkdocs](https://www.mkdocs.org/), but you can use it for other stuffs if suitable.
 
 The code itself is a direct modification to [markdown-include](https://github.com/cmacmackin/markdown-include) since they do similar things.
```

### Comparing `markdown-mdantic-2.1.0/README.md` & `markdown-mdantic-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `markdown-mdantic-2.1.0/markdown_mdantic.egg-info/PKG-INFO` & `markdown-mdantic-2.1.1/markdown_mdantic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-mdantic
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python-Markdown extension for rendering pydantic BaseModel as table
 Home-page: https://github.com/frefreak/mdantic
 Author: Xiangyu Zhu
 Author-email: frefreak.zxy@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Filters
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: markdown>=3.0
+Requires-Dist: tabulate
+Requires-Dist: pydantic>=2.0
 
 # Mdantic
 
 This is an extension to [Python-Markdown](https://python-markdown.github.io/). It adds a new syntax so that you can reference a [pydantic](https://pydantic-docs.helpmanual.io/) `BaseModel` and translate its fields to a markdown table. (Get the name?) I originally make this to generate http api parameter tables with [mkdocs](https://www.mkdocs.org/), but you can use it for other stuffs if suitable.
 
 The code itself is a direct modification to [markdown-include](https://github.com/cmacmackin/markdown-include) since they do similar things.
```

### Comparing `markdown-mdantic-2.1.0/setup.py` & `markdown-mdantic-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name="markdown-mdantic",
-    version="2.1.0",
+    version="2.1.1",
     author="Xiangyu Zhu",
     author_email="frefreak.zxy@gmail.com",
     description="Python-Markdown extension for rendering pydantic BaseModel as table",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/frefreak/mdantic",
-    py_modules=["mdantic"],
+    packages=["mdantic"],
     install_requires=["markdown >= 3.0", "tabulate", "pydantic >= 2.0"],
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
         "Development Status :: 4 - Beta",
```

### Comparing `markdown-mdantic-2.1.0/tests/test_analyze.py` & `markdown-mdantic-2.1.1/tests/test_analyze.py`

 * *Files identical despite different names*

