# Comparing `tmp/mypy-boto3-personalize-1.34.20.tar.gz` & `tmp/mypy_boto3_personalize-1.34.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-1.34.20.tar", last modified: Tue Jan 16 20:32:46 2024, max compression
+gzip compressed data, was "mypy_boto3_personalize-1.34.88.tar", last modified: Fri Apr 19 19:32:14 2024, max compression
```

## Comparing `mypy-boto3-personalize-1.34.20.tar` & `mypy_boto3_personalize-1.34.88.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.124973 mypy-boto3-personalize-1.34.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-01-16 20:32:46.124973 mypy-boto3-personalize-1.34.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.120973 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52070 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    52067 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    64697 2024-01-16 20:32:12.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64697 2024-01-16 20:32:12.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-16 20:32:11.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:46.124973 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-01-16 20:32:46.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-16 20:32:46.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:46.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:46.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-16 20:32:46.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-16 20:32:46.000000 mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 20:32:46.124973 mypy-boto3-personalize-1.34.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-16 20:32:10.000000 mypy-boto3-personalize-1.34.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.733938 mypy_boto3_personalize-1.34.88/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-04-19 19:32:14.729938 mypy_boto3_personalize-1.34.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.729938 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51875 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51872 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    65297 2024-04-19 19:32:03.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65297 2024-04-19 19:32:02.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:32:14.729938 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 19:32:14.000000 mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:32:14.733938 mypy_boto3_personalize-1.34.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-19 19:32:01.000000 mypy_boto3_personalize-1.34.88/setup.py
```

### Comparing `mypy-boto3-personalize-1.34.20/LICENSE` & `mypy_boto3_personalize-1.34.88/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.34.20/PKG-INFO` & `mypy_boto3_personalize-1.34.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.34.20
-Summary: Type annotations for boto3.Personalize 1.34.20 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.88
+Summary: Type annotations for boto3.Personalize 1.34.88 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize)](https://pepy.tech/project/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-personalize-1.34.20/README.md` & `mypy_boto3_personalize-1.34.88/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize)](https://pepy.tech/project/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/__init__.py` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/__init__.pyi` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/__main__.py` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Personalize 1.34.20\nVersion:         1.34.20\nBuilder version:"
-        " 7.23.1\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Personalize 1.34.88\n"
+        "Version:         1.34.88\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.20")
+    print("1.34.88")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/client.py` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
-        Creates a campaign that deploys a solution version.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
 
     def create_dataset(
         self,
@@ -379,21 +379,22 @@
     def create_solution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
+        performAutoTraining: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionResponseTypeDef:
         """
-        Creates the configuration for training a model.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
         """
 
     def create_solution_version(
         self,
@@ -831,15 +832,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solution_versions)
         """
 
     def list_solutions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListSolutionsResponseTypeDef:
         """
-        Returns a list of solutions that use the given dataset group.
+        Returns a list of solutions in a given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -886,18 +887,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Remove
-        [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-resources.html)
-        that are attached to a
-        resource.
+        Removes the specified tags that are attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#untag_resource)
         """
 
     def update_campaign(
         self,
@@ -906,15 +904,14 @@
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign to deploy a retrained solution version with an existing
         campaign, change your campaign's `minProvisionedTPS`, or modify your campaign's
-        configuration, such as the exploration
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
 
     def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/client.pyi` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
-        Creates a campaign that deploys a solution version.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_campaign)
         """
 
     def create_dataset(
         self,
@@ -376,21 +376,22 @@
     def create_solution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
+        performAutoTraining: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionResponseTypeDef:
         """
-        Creates the configuration for training a model.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#create_solution)
         """
 
     def create_solution_version(
         self,
@@ -828,15 +829,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solution_versions)
         """
 
     def list_solutions(
         self, *, datasetGroupArn: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListSolutionsResponseTypeDef:
         """
-        Returns a list of solutions that use the given dataset group.
+        Returns a list of solutions in a given dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#list_solutions)
         """
 
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
@@ -883,18 +884,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Remove
-        [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-resources.html)
-        that are attached to a
-        resource.
+        Removes the specified tags that are attached to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#untag_resource)
         """
 
     def update_campaign(
         self,
@@ -903,15 +901,14 @@
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign to deploy a retrained solution version with an existing
         campaign, change your campaign's `minProvisionedTPS`, or modify your campaign's
-        configuration, such as the exploration
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/client/#update_campaign)
         """
 
     def update_dataset(self, *, datasetArn: str, schemaArn: str) -> UpdateDatasetResponseTypeDef:
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/literals.py` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "ListRecommendersPaginatorName",
     "ListSchemasPaginatorName",
     "ListSolutionVersionsPaginatorName",
     "ListSolutionsPaginatorName",
     "ObjectiveSensitivityType",
     "RecipeProviderType",
     "TrainingModeType",
+    "TrainingTypeType",
     "PersonalizeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -68,15 +69,16 @@
 ListRecipesPaginatorName = Literal["list_recipes"]
 ListRecommendersPaginatorName = Literal["list_recommenders"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 ListSolutionVersionsPaginatorName = Literal["list_solution_versions"]
 ListSolutionsPaginatorName = Literal["list_solutions"]
 ObjectiveSensitivityType = Literal["HIGH", "LOW", "MEDIUM", "OFF"]
 RecipeProviderType = Literal["SERVICE"]
-TrainingModeType = Literal["FULL", "UPDATE"]
+TrainingModeType = Literal["AUTOTRAIN", "FULL", "UPDATE"]
+TrainingTypeType = Literal["AUTOMATIC", "MANUAL"]
 PersonalizeServiceName = Literal["personalize"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -96,14 +98,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -114,14 +117,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -139,14 +143,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -159,24 +164,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -237,15 +244,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -425,14 +431,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/literals.pyi` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "ListRecommendersPaginatorName",
     "ListSchemasPaginatorName",
     "ListSolutionVersionsPaginatorName",
     "ListSolutionsPaginatorName",
     "ObjectiveSensitivityType",
     "RecipeProviderType",
     "TrainingModeType",
+    "TrainingTypeType",
     "PersonalizeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
@@ -68,15 +69,16 @@
 ListRecipesPaginatorName = Literal["list_recipes"]
 ListRecommendersPaginatorName = Literal["list_recommenders"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 ListSolutionVersionsPaginatorName = Literal["list_solution_versions"]
 ListSolutionsPaginatorName = Literal["list_solutions"]
 ObjectiveSensitivityType = Literal["HIGH", "LOW", "MEDIUM", "OFF"]
 RecipeProviderType = Literal["SERVICE"]
-TrainingModeType = Literal["FULL", "UPDATE"]
+TrainingModeType = Literal["AUTOTRAIN", "FULL", "UPDATE"]
+TrainingTypeType = Literal["AUTOMATIC", "MANUAL"]
 PersonalizeServiceName = Literal["personalize"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -96,14 +98,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -114,14 +117,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -139,14 +143,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -159,24 +164,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -237,15 +244,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -425,14 +431,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/paginator.py` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/paginator.pyi` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/type_defs.py` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .literals import (
     BatchInferenceJobModeType,
     DomainType,
     ImportModeType,
     IngestionModeType,
     ObjectiveSensitivityType,
     TrainingModeType,
+    TrainingTypeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -38,14 +39,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlgorithmImageTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
+    "AutoTrainingConfigTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
@@ -270,14 +272,20 @@
 )
 AutoMLResultTypeDef = TypedDict(
     "AutoMLResultTypeDef",
     {
         "bestRecipeArn": NotRequired[str],
     },
 )
+AutoTrainingConfigTypeDef = TypedDict(
+    "AutoTrainingConfigTypeDef",
+    {
+        "schedulingExpression": NotRequired[str],
+    },
+)
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
     },
 )
 S3DataConfigTypeDef = TypedDict(
@@ -313,14 +321,15 @@
     },
 )
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
         "enableMetadataWithRecommendations": NotRequired[bool],
+        "syncWithLatestSolutionVersion": NotRequired[bool],
     },
 )
 CampaignSummaryTypeDef = TypedDict(
     "CampaignSummaryTypeDef",
     {
         "name": NotRequired[str],
         "campaignArn": NotRequired[str],
@@ -352,18 +361,18 @@
         "tagValue": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "dataLocation": NotRequired[str],
     },
@@ -915,14 +924,16 @@
     },
 )
 SolutionVersionSummaryTypeDef = TypedDict(
     "SolutionVersionSummaryTypeDef",
     {
         "solutionVersionArn": NotRequired[str],
         "status": NotRequired[str],
+        "trainingMode": NotRequired[TrainingModeType],
+        "trainingType": NotRequired[TrainingTypeType],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "failureReason": NotRequired[str],
     },
 )
 ListSolutionsRequestRequestTypeDef = TypedDict(
     "ListSolutionsRequestRequestTypeDef",
@@ -1930,14 +1941,15 @@
         "eventValueThreshold": NotRequired[str],
         "hpoConfig": NotRequired[HPOConfigTypeDef],
         "algorithmHyperParameters": NotRequired[Mapping[str, str]],
         "featureTransformationParameters": NotRequired[Mapping[str, str]],
         "autoMLConfig": NotRequired[AutoMLConfigTypeDef],
         "optimizationObjective": NotRequired[OptimizationObjectiveTypeDef],
         "trainingDataConfig": NotRequired[TrainingDataConfigTypeDef],
+        "autoTrainingConfig": NotRequired[AutoTrainingConfigTypeDef],
     },
 )
 ListRecommendersResponsePaginatorTypeDef = TypedDict(
     "ListRecommendersResponsePaginatorTypeDef",
     {
         "recommenders": List[RecommenderSummaryPaginatorTypeDef],
         "nextToken": str,
@@ -1971,27 +1983,29 @@
 CreateSolutionRequestRequestTypeDef = TypedDict(
     "CreateSolutionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
+        "performAutoTraining": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "eventType": NotRequired[str],
         "solutionConfig": NotRequired[SolutionConfigTypeDef],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": NotRequired[str],
         "solutionArn": NotRequired[str],
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
+        "performAutoTraining": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "eventType": NotRequired[str],
         "solutionConfig": NotRequired[SolutionConfigTypeDef],
         "autoMLResult": NotRequired[AutoMLResultTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
@@ -2014,14 +2028,15 @@
         "trainingHours": NotRequired[float],
         "trainingMode": NotRequired[TrainingModeType],
         "tunedHPOParams": NotRequired[TunedHPOParamsTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
+        "trainingType": NotRequired[TrainingTypeType],
     },
 )
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize/type_defs.pyi` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .literals import (
     BatchInferenceJobModeType,
     DomainType,
     ImportModeType,
     IngestionModeType,
     ObjectiveSensitivityType,
     TrainingModeType,
+    TrainingTypeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 12):
@@ -38,14 +39,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlgorithmImageTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
+    "AutoTrainingConfigTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
     "BatchSegmentJobSummaryTypeDef",
     "CampaignConfigTypeDef",
     "CampaignSummaryTypeDef",
     "CategoricalHyperParameterRangeTypeDef",
@@ -270,14 +272,20 @@
 )
 AutoMLResultTypeDef = TypedDict(
     "AutoMLResultTypeDef",
     {
         "bestRecipeArn": NotRequired[str],
     },
 )
+AutoTrainingConfigTypeDef = TypedDict(
+    "AutoTrainingConfigTypeDef",
+    {
+        "schedulingExpression": NotRequired[str],
+    },
+)
 BatchInferenceJobConfigTypeDef = TypedDict(
     "BatchInferenceJobConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
     },
 )
 S3DataConfigTypeDef = TypedDict(
@@ -313,14 +321,15 @@
     },
 )
 CampaignConfigTypeDef = TypedDict(
     "CampaignConfigTypeDef",
     {
         "itemExplorationConfig": NotRequired[Mapping[str, str]],
         "enableMetadataWithRecommendations": NotRequired[bool],
+        "syncWithLatestSolutionVersion": NotRequired[bool],
     },
 )
 CampaignSummaryTypeDef = TypedDict(
     "CampaignSummaryTypeDef",
     {
         "name": NotRequired[str],
         "campaignArn": NotRequired[str],
@@ -352,18 +361,18 @@
         "tagValue": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "dataLocation": NotRequired[str],
     },
@@ -915,14 +924,16 @@
     },
 )
 SolutionVersionSummaryTypeDef = TypedDict(
     "SolutionVersionSummaryTypeDef",
     {
         "solutionVersionArn": NotRequired[str],
         "status": NotRequired[str],
+        "trainingMode": NotRequired[TrainingModeType],
+        "trainingType": NotRequired[TrainingTypeType],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
         "failureReason": NotRequired[str],
     },
 )
 ListSolutionsRequestRequestTypeDef = TypedDict(
     "ListSolutionsRequestRequestTypeDef",
@@ -1930,14 +1941,15 @@
         "eventValueThreshold": NotRequired[str],
         "hpoConfig": NotRequired[HPOConfigTypeDef],
         "algorithmHyperParameters": NotRequired[Mapping[str, str]],
         "featureTransformationParameters": NotRequired[Mapping[str, str]],
         "autoMLConfig": NotRequired[AutoMLConfigTypeDef],
         "optimizationObjective": NotRequired[OptimizationObjectiveTypeDef],
         "trainingDataConfig": NotRequired[TrainingDataConfigTypeDef],
+        "autoTrainingConfig": NotRequired[AutoTrainingConfigTypeDef],
     },
 )
 ListRecommendersResponsePaginatorTypeDef = TypedDict(
     "ListRecommendersResponsePaginatorTypeDef",
     {
         "recommenders": List[RecommenderSummaryPaginatorTypeDef],
         "nextToken": str,
@@ -1971,27 +1983,29 @@
 CreateSolutionRequestRequestTypeDef = TypedDict(
     "CreateSolutionRequestRequestTypeDef",
     {
         "name": str,
         "datasetGroupArn": str,
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
+        "performAutoTraining": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "eventType": NotRequired[str],
         "solutionConfig": NotRequired[SolutionConfigTypeDef],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 SolutionTypeDef = TypedDict(
     "SolutionTypeDef",
     {
         "name": NotRequired[str],
         "solutionArn": NotRequired[str],
         "performHPO": NotRequired[bool],
         "performAutoML": NotRequired[bool],
+        "performAutoTraining": NotRequired[bool],
         "recipeArn": NotRequired[str],
         "datasetGroupArn": NotRequired[str],
         "eventType": NotRequired[str],
         "solutionConfig": NotRequired[SolutionConfigTypeDef],
         "autoMLResult": NotRequired[AutoMLResultTypeDef],
         "status": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
@@ -2014,14 +2028,15 @@
         "trainingHours": NotRequired[float],
         "trainingMode": NotRequired[TrainingModeType],
         "tunedHPOParams": NotRequired[TunedHPOParamsTypeDef],
         "status": NotRequired[str],
         "failureReason": NotRequired[str],
         "creationDateTime": NotRequired[datetime],
         "lastUpdatedDateTime": NotRequired[datetime],
+        "trainingType": NotRequired[TrainingTypeType],
     },
 )
 DescribeRecommenderResponseTypeDef = TypedDict(
     "DescribeRecommenderResponseTypeDef",
     {
         "recommender": RecommenderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/PKG-INFO` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize
-Version: 1.34.20
-Summary: Type annotations for boto3.Personalize 1.34.20 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.88
+Summary: Type annotations for boto3.Personalize 1.34.88 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize)](https://pepy.tech/project/mypy-boto3-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Personalize 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[boto3.Personalize 1.34.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-personalize docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-personalize-1.34.20/mypy_boto3_personalize.egg-info/SOURCES.txt` & `mypy_boto3_personalize-1.34.88/mypy_boto3_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-1.34.20/setup.py` & `mypy_boto3_personalize-1.34.88/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize",
-    version="1.34.20",
+    version="1.34.88",
     packages=["mypy_boto3_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Personalize 1.34.20 service generated with mypy-boto3-builder"
-        " 7.23.1"
-    ),
+    description="Type annotations for boto3.Personalize 1.34.88 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

