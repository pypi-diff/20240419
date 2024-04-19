# Comparing `tmp/tufup-0.7.1.tar.gz` & `tmp/tufup-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tufup-0.7.1.tar", last modified: Tue Mar 12 16:14:44 2024, max compression
+gzip compressed data, was "tufup-0.8.0.tar", last modified: Fri Apr 19 10:04:30 2024, max compression
```

## Comparing `tufup-0.7.1.tar` & `tufup-0.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 16:14:44.059189 tufup-0.7.1/
--rw-rw-rw-   0        0        0     1084 2022-09-21 07:49:55.000000 tufup-0.7.1/LICENSE
--rw-rw-rw-   0        0        0    15115 2024-03-12 16:14:44.054972 tufup-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    12980 2024-02-13 09:16:13.000000 tufup-0.7.1/README.md
--rw-rw-rw-   0        0        0     1412 2024-01-23 10:10:56.000000 tufup-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 16:14:44.059209 tufup-0.7.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-12 16:14:43.921714 tufup-0.7.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-12 16:14:43.958149 tufup-0.7.1/src/tufup/
--rw-rw-rw-   0        0        0      986 2024-03-12 16:10:55.000000 tufup-0.7.1/src/tufup/__init__.py
--rw-rw-rw-   0        0        0      292 2022-09-21 07:49:56.000000 tufup-0.7.1/src/tufup/__main__.py
--rw-rw-rw-   0        0        0    18112 2024-03-12 09:13:23.000000 tufup-0.7.1/src/tufup/client.py
--rw-rw-rw-   0        0        0    10301 2024-03-12 09:13:23.000000 tufup-0.7.1/src/tufup/common.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:14:43.998474 tufup-0.7.1/src/tufup/repo/
--rw-rw-rw-   0        0        0    40968 2024-03-12 11:46:48.000000 tufup-0.7.1/src/tufup/repo/__init__.py
--rw-rw-rw-   0        0        0    13246 2024-03-12 12:26:16.000000 tufup-0.7.1/src/tufup/repo/cli.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:14:44.005936 tufup-0.7.1/src/tufup/utils/
--rw-rw-rw-   0        0        0     3731 2024-01-23 10:11:12.000000 tufup-0.7.1/src/tufup/utils/__init__.py
--rw-rw-rw-   0        0        0    11287 2024-03-12 16:10:06.000000 tufup-0.7.1/src/tufup/utils/platform_specific.py
-drwxrwxrwx   0        0        0        0 2024-03-12 16:14:44.051812 tufup-0.7.1/src/tufup.egg-info/
--rw-rw-rw-   0        0        0    15115 2024-03-12 16:14:43.000000 tufup-0.7.1/src/tufup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-03-12 16:14:43.000000 tufup-0.7.1/src/tufup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 16:14:43.000000 tufup-0.7.1/src/tufup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-12 16:14:43.000000 tufup-0.7.1/src/tufup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      141 2024-03-12 16:14:43.000000 tufup-0.7.1/src/tufup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-12 16:14:43.000000 tufup-0.7.1/src/tufup.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-12 16:14:44.043454 tufup-0.7.1/tests/
--rw-rw-rw-   0        0        0    19827 2024-03-12 09:13:23.000000 tufup-0.7.1/tests/test_client.py
--rw-rw-rw-   0        0        0    10914 2024-03-12 09:13:23.000000 tufup-0.7.1/tests/test_common.py
--rw-rw-rw-   0        0        0      279 2022-10-04 13:22:25.000000 tufup-0.7.1/tests/test_package.py
--rw-rw-rw-   0        0        0    39592 2024-03-12 09:13:23.000000 tufup-0.7.1/tests/test_repo.py
--rw-rw-rw-   0        0        0    11680 2024-03-12 12:07:40.000000 tufup-0.7.1/tests/test_repo_cli.py
--rw-rw-rw-   0        0        0     1249 2022-09-21 07:49:56.000000 tufup-0.7.1/tests/test_tests.py
--rw-rw-rw-   0        0        0     3767 2024-01-23 10:11:12.000000 tufup-0.7.1/tests/test_utils.py
--rw-rw-rw-   0        0        0    10285 2024-03-12 16:10:06.000000 tufup-0.7.1/tests/test_utils_platform_specific.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:04:30.670415 tufup-0.8.0/
+-rw-rw-rw-   0        0        0     1084 2022-03-25 16:00:29.000000 tufup-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0    15115 2024-04-19 10:04:30.669321 tufup-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12980 2024-02-12 17:46:14.000000 tufup-0.8.0/README.md
+-rw-rw-rw-   0        0        0     1412 2024-04-19 09:36:52.000000 tufup-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:04:30.670415 tufup-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 10:04:30.618719 tufup-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 10:04:30.633024 tufup-0.8.0/src/tufup/
+-rw-rw-rw-   0        0        0      986 2024-04-19 09:46:40.000000 tufup-0.8.0/src/tufup/__init__.py
+-rw-rw-rw-   0        0        0      292 2022-07-01 14:31:47.000000 tufup-0.8.0/src/tufup/__main__.py
+-rw-rw-rw-   0        0        0    18105 2024-04-19 09:36:52.000000 tufup-0.8.0/src/tufup/client.py
+-rw-rw-rw-   0        0        0    10321 2024-03-22 14:12:19.000000 tufup-0.8.0/src/tufup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:04:30.645736 tufup-0.8.0/src/tufup/repo/
+-rw-rw-rw-   0        0        0    40968 2024-03-13 09:26:33.000000 tufup-0.8.0/src/tufup/repo/__init__.py
+-rw-rw-rw-   0        0        0    13246 2024-03-13 09:26:33.000000 tufup-0.8.0/src/tufup/repo/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:04:30.651569 tufup-0.8.0/src/tufup/utils/
+-rw-rw-rw-   0        0        0     3731 2023-11-20 21:15:03.000000 tufup-0.8.0/src/tufup/utils/__init__.py
+-rw-rw-rw-   0        0        0    11287 2024-03-22 12:41:45.000000 tufup-0.8.0/src/tufup/utils/platform_specific.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:04:30.668323 tufup-0.8.0/src/tufup.egg-info/
+-rw-rw-rw-   0        0        0    15115 2024-04-19 10:04:30.000000 tufup-0.8.0/src/tufup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-19 10:04:30.000000 tufup-0.8.0/src/tufup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:04:30.000000 tufup-0.8.0/src/tufup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-19 10:04:30.000000 tufup-0.8.0/src/tufup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      141 2024-04-19 10:04:30.000000 tufup-0.8.0/src/tufup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-19 10:04:30.000000 tufup-0.8.0/src/tufup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 10:04:30.666230 tufup-0.8.0/tests/
+-rw-rw-rw-   0        0        0    19827 2024-03-11 16:37:11.000000 tufup-0.8.0/tests/test_client.py
+-rw-rw-rw-   0        0        0    11457 2024-03-22 14:12:19.000000 tufup-0.8.0/tests/test_common_.py
+-rw-rw-rw-   0        0        0      279 2022-09-26 20:49:28.000000 tufup-0.8.0/tests/test_package.py
+-rw-rw-rw-   0        0        0    39592 2024-03-11 16:37:11.000000 tufup-0.8.0/tests/test_repo.py
+-rw-rw-rw-   0        0        0    11680 2024-03-13 09:26:33.000000 tufup-0.8.0/tests/test_repo_cli.py
+-rw-rw-rw-   0        0        0     1249 2022-06-22 14:44:45.000000 tufup-0.8.0/tests/test_tests.py
+-rw-rw-rw-   0        0        0     3767 2023-11-20 21:15:03.000000 tufup-0.8.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0    10285 2024-03-13 09:26:33.000000 tufup-0.8.0/tests/test_utils_platform_specific.py
```

### Comparing `tufup-0.7.1/LICENSE` & `tufup-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/PKG-INFO` & `tufup-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tufup
-Version: 0.7.1
+Version: 0.8.0
 Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
 Author-email: dennisvang <djvg@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Dennis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bsdiff4==1.2.*
 Requires-Dist: packaging>=21.3
 Requires-Dist: securesystemslib[crypto,pynacl]>=0.26.0
 Requires-Dist: setuptools>=65.5.1
-Requires-Dist: tuf==3.1.*
+Requires-Dist: tuf==4.0.*
 Requires-Dist: certifi>=2022.12.7
 Requires-Dist: cryptography>=38.0.3
 
 # tufup
 
 ![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
```

### Comparing `tufup-0.7.1/README.md` & `tufup-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/pyproject.toml` & `tufup-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 requires-python = ">=3.8"
 dependencies = [
     # direct dependencies
     "bsdiff4==1.2.*",
     "packaging>=21.3",
     "securesystemslib[crypto,pynacl]>=0.26.0",
     "setuptools>=65.5.1",
-    "tuf==3.1.*",
+    "tuf==4.0.*",
     # constraints on sub-dependencies
     "certifi>=2022.12.7",
     "cryptography>=38.0.3",
 ]
 
 [project.urls]
 source = "https://github.com/dennisvang/tufup"
```

### Comparing `tufup-0.7.1/src/tufup/__init__.py` & `tufup-0.8.0/src/tufup/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 
 from tufup.repo import cli
 
 # https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
 # https://semver.org/
-__version__ = '0.7.1'
+__version__ = '0.8.0'
 
 logger = logging.getLogger(__name__)
 
 
 def main(args=None):
     # show version before anything else
     print(f'tufup {__version__}')
```

### Comparing `tufup-0.7.1/src/tufup/client.py` & `tufup-0.8.0/src/tufup/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         """
         # todo: _trusted_set is private, but ideally we would use a public
         #  interface (if only tuf.ngclient exposed one...)
         _trusted_target_metas = []
         if self._trusted_set.targets:
             _trusted_target_metas = [
                 TargetMeta(target_path=key, custom=target.custom)
-                for key, target in self._trusted_set.targets.signed.targets.items()
+                for key, target in self._trusted_set.targets.targets.items()
             ]
             logger.debug(f'{len(_trusted_target_metas)} TargetMeta objects created')
         else:
             logger.warning('targets metadata not found')
         return _trusted_target_metas
 
     def get_targetinfo(
```

### Comparing `tufup-0.7.1/src/tufup/common.py` & `tufup-0.8.0/src/tufup/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 class CustomMetadataDict(TypedDict):
     """
     explicitly separate custom metadata into user-specified metadata and metadata
     used by tufup internally
     """
 
-    user: Optional[dict]
-    tufup: Optional[dict]
+    user: dict
+    tufup: dict
 
 
 def _immutable(value):
     """
     Make value immutable, recursively, so the result is hashable.
 
     Applies to (nested) dict, list, set, and bytearray [1] mutable sequence types.
@@ -75,36 +75,37 @@
             )
         self.target_path_str = str(target_path)  # keep the original for reference
         self.path = pathlib.Path(target_path)
         if ' ' in self.filename:
             logger.critical(
                 f'invalid filename "{self.filename}": whitespace not allowed'
             )
-        self._custom = custom
+        self._custom = custom or dict(user=dict(), tufup=dict())
 
     @property
-    def custom(self) -> Optional[dict]:
-        """returns user-specified custom metadata"""
+    def custom(self) -> dict:
+        """returns user-specified custom metadata dict"""
         return self._get_custom_metadata('user')
 
     @property
-    def custom_internal(self) -> Optional[dict]:
-        """returns tufup-internal custom metadata"""
+    def custom_internal(self) -> dict:
+        """returns tufup-internal custom metadata dict"""
         return self._get_custom_metadata('tufup')
 
-    def _get_custom_metadata(self, key: str) -> Optional[dict]:
+    def _get_custom_metadata(self, _key: str) -> dict:
         """
         get custom metadata in a backward-compatible manner (older versions did not
         distinguish between user-specified and internal metadata)
         """
         if isinstance(self._custom, dict):
             # check dict keys for backward compatibility
             if get_type_hints(CustomMetadataDict).keys() != self._custom.keys():
                 return self._custom
-            return self._custom.get(key)
+            return self._custom.get(_key)
+        return dict()
 
     def __str__(self):
         return str(self.target_path_str)
 
     def __repr__(self):
         return f'{self.__class__.__name__}(target_path="{self.target_path_str}")'
```

### Comparing `tufup-0.7.1/src/tufup/repo/__init__.py` & `tufup-0.8.0/src/tufup/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/src/tufup/repo/cli.py` & `tufup-0.8.0/src/tufup/repo/cli.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/src/tufup/utils/__init__.py` & `tufup-0.8.0/src/tufup/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/src/tufup/utils/platform_specific.py` & `tufup-0.8.0/src/tufup/utils/platform_specific.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/src/tufup.egg-info/PKG-INFO` & `tufup-0.8.0/src/tufup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tufup
-Version: 0.7.1
+Version: 0.8.0
 Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
 Author-email: dennisvang <djvg@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Dennis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bsdiff4==1.2.*
 Requires-Dist: packaging>=21.3
 Requires-Dist: securesystemslib[crypto,pynacl]>=0.26.0
 Requires-Dist: setuptools>=65.5.1
-Requires-Dist: tuf==3.1.*
+Requires-Dist: tuf==4.0.*
 Requires-Dist: certifi>=2022.12.7
 Requires-Dist: cryptography>=38.0.3
 
 # tufup
 
 ![Build](https://github.com/dennisvang/tufup/actions/workflows/python-package.yml/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/tufup)](https://pypi.org/project/tufup/)
```

### Comparing `tufup-0.7.1/src/tufup.egg-info/SOURCES.txt` & `tufup-0.8.0/src/tufup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 src/tufup.egg-info/requires.txt
 src/tufup.egg-info/top_level.txt
 src/tufup/repo/__init__.py
 src/tufup/repo/cli.py
 src/tufup/utils/__init__.py
 src/tufup/utils/platform_specific.py
 tests/test_client.py
-tests/test_common.py
+tests/test_common_.py
 tests/test_package.py
 tests/test_repo.py
 tests/test_repo_cli.py
 tests/test_tests.py
 tests/test_utils.py
 tests/test_utils_platform_specific.py
```

### Comparing `tufup-0.7.1/tests/test_client.py` & `tufup-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/tests/test_common.py` & `tufup-0.8.0/tests/test_common_.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             1,
             ('a', 1),
             ['a', 1],
             {'a', 1},
             bytearray(b'b'),
             dict(a=1),
             [dict(a=[dict(c={1})], b=bytearray(b'd'))],
+            dict(a=dict(b=dict(c=dict()))),
         ]
         for case in cases:
             with self.subTest(msg=case):
                 self.assertIsInstance(_immutable(case), Hashable)
 
 
 class TargetMetaTests(TempDirTestCase):
@@ -62,15 +63,24 @@
             with self.subTest(msg=target_path):
                 self.assertIsInstance(
                     TargetMeta(target_path=target_path).__str__(), str
                 )
 
     def test_hashable(self):
         obj = TargetMeta()
-        self.assertEqual(obj.__hash__(), hash(tuple(vars(obj).items())))
+        try:
+            obj.__hash__()
+        except Exception as e:
+            self.fail(f'__hash__ failed unexpectedly: {e}')
+        expected_obj_hashable = (
+            ('target_path_str', 'None-None.tar.gz'),
+            ('path', pathlib.Path('None-None.tar.gz')),
+            ('_custom', (('user', ()), ('tufup', ()))),
+        )
+        self.assertEqual(hash(expected_obj_hashable), obj.__hash__())
         # we can use the obj as a set member or as dict key
         self.assertEqual({obj, obj}, {obj})
 
     def test_sortable(self):
         version_1 = TargetMeta(target_path='my-app-win-1.0.tar.gz')
         version_2 = TargetMeta(target_path='my-app-win-2.0.tar.gz')
         info_list = [version_2, version_1]
@@ -167,16 +177,19 @@
         custom_metadata = dict(foo='bar')
         target_meta = TargetMeta(custom=custom_metadata)  # noqa
         self.assertEqual(custom_metadata, target_meta.custom)
         self.assertEqual(custom_metadata, target_meta.custom_internal)
 
     def test_custom_metadata_not_specified(self):
         target_meta = TargetMeta()
-        self.assertIsNone(target_meta.custom)
-        self.assertIsNone(target_meta.custom_internal)
+        self.assertIsInstance(target_meta.custom, dict)
+        self.assertIsInstance(target_meta.custom_internal, dict)
+        # user overrides _custom attr
+        target_meta._custom = None
+        self.assertIsInstance(target_meta.custom, dict)
 
 
 class PatcherTests(TempDirTestCase):
     def setUp(self) -> None:
         super().setUp()
         # define dummy .tar content
         self.tar_content = {
```

### Comparing `tufup-0.7.1/tests/test_repo.py` & `tufup-0.8.0/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/tests/test_repo_cli.py` & `tufup-0.8.0/tests/test_repo_cli.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/tests/test_tests.py` & `tufup-0.8.0/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/tests/test_utils.py` & `tufup-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tufup-0.7.1/tests/test_utils_platform_specific.py` & `tufup-0.8.0/tests/test_utils_platform_specific.py`

 * *Files identical despite different names*

