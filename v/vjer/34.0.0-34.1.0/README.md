# Comparing `tmp/vjer-34.0.0.tar.gz` & `tmp/vjer-34.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-34.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-34.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-34.0.0.tar` & `vjer-34.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1783 2024-04-18 20:17:02.276491 vjer-34.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2134 2024-04-18 20:17:02.280491 vjer-34.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     5245 2024-04-18 20:17:02.280491 vjer-34.0.0/.gitignore
--rw-r--r--   0        0        0     4999 2024-04-18 20:17:02.280491 vjer-34.0.0/.p4ignore
--rw-r--r--   0        0        0       42 2024-04-18 20:17:02.280491 vjer-34.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    40544 2024-04-18 20:17:02.280491 vjer-34.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-04-18 20:17:02.280491 vjer-34.0.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-04-18 20:17:02.280491 vjer-34.0.0/LICENSE
--rw-r--r--   0        0        0       90 2024-04-18 20:17:02.280491 vjer-34.0.0/MANIFEST.in
--rw-r--r--   0        0        0      973 2024-04-18 20:17:02.280491 vjer-34.0.0/README.md
--rwxr-xr-x   0        0        0     1046 2024-04-18 20:17:02.280491 vjer-34.0.0/cicd-support/cicd.sh
--rw-r--r--   0        0        0      634 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/conf.py
--rw-r--r--   0        0        0      795 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/make.bat
--rw-r--r--   0        0        0       59 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2184 2024-04-18 20:17:29.368613 vjer-34.0.0/pyproject.toml
--rw-r--r--   0        0        0       90 2024-04-18 20:17:02.280491 vjer-34.0.0/tests/vjer.yml
--rw-r--r--   0        0        0      305 2024-04-18 20:17:02.280491 vjer-34.0.0/util/New-Env.ps1
--rw-r--r--   0        0        0      259 2024-04-18 20:17:02.280491 vjer-34.0.0/util/Update-Env.ps1
--rwxr-xr-x   0        0        0      261 2024-04-18 20:17:02.280491 vjer-34.0.0/util/new-env.sh
--rwxr-xr-x   0        0        0      234 2024-04-18 20:17:02.280491 vjer-34.0.0/util/update-env.sh
--rw-r--r--   0        0        0      476 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer.yml
--rw-r--r--   0        0        0      654 2024-04-18 20:17:29.368613 vjer-34.0.0/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/__main__.py
--rw-r--r--   0        0        0     5278 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/freeze.py
--rw-r--r--   0        0        0     1613 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/py.typed
--rw-r--r--   0        0        0     3170 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/release.py
--rw-r--r--   0        0        0      769 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/test.py
--rw-r--r--   0        0        0     2946 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/tool_reporter.py
--rw-r--r--   0        0        0    25423 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/utils.py
--rwxr-xr-x   0        0        0     2825 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/vjer.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-34.0.0/setup.py
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-34.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1783 2024-04-19 14:51:26.978289 vjer-34.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2134 2024-04-19 14:51:26.978289 vjer-34.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5245 2024-04-19 14:51:26.978289 vjer-34.1.0/.gitignore
+-rw-r--r--   0        0        0     4999 2024-04-19 14:51:26.978289 vjer-34.1.0/.p4ignore
+-rw-r--r--   0        0        0       42 2024-04-19 14:51:26.978289 vjer-34.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0    40661 2024-04-19 14:51:26.978289 vjer-34.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-04-19 14:51:26.978289 vjer-34.1.0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-19 14:51:26.978289 vjer-34.1.0/LICENSE
+-rw-r--r--   0        0        0       90 2024-04-19 14:51:26.978289 vjer-34.1.0/MANIFEST.in
+-rw-r--r--   0        0        0      973 2024-04-19 14:51:26.978289 vjer-34.1.0/README.md
+-rwxr-xr-x   0        0        0     1046 2024-04-19 14:51:26.978289 vjer-34.1.0/cicd-support/cicd.sh
+-rw-r--r--   0        0        0      634 2024-04-19 14:51:26.978289 vjer-34.1.0/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-04-19 14:51:26.978289 vjer-34.1.0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-04-19 14:51:26.978289 vjer-34.1.0/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-04-19 14:51:26.978289 vjer-34.1.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-04-19 14:51:26.978289 vjer-34.1.0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-19 14:51:26.978289 vjer-34.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2184 2024-04-19 14:51:56.786115 vjer-34.1.0/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-04-19 14:51:26.978289 vjer-34.1.0/tests/vjer.yml
+-rw-r--r--   0        0        0      305 2024-04-19 14:51:26.978289 vjer-34.1.0/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-04-19 14:51:26.978289 vjer-34.1.0/util/Update-Env.ps1
+-rwxr-xr-x   0        0        0      261 2024-04-19 14:51:26.982289 vjer-34.1.0/util/new-env.sh
+-rwxr-xr-x   0        0        0      234 2024-04-19 14:51:26.982289 vjer-34.1.0/util/update-env.sh
+-rw-r--r--   0        0        0      476 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer.yml
+-rw-r--r--   0        0        0      654 2024-04-19 14:51:56.786115 vjer-34.1.0/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/__main__.py
+-rw-r--r--   0        0        0     5278 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/freeze.py
+-rw-r--r--   0        0        0     1621 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/py.typed
+-rw-r--r--   0        0        0     3170 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/test.py
+-rw-r--r--   0        0        0     2946 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    25423 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/utils.py
+-rwxr-xr-x   0        0        0     2825 2024-04-19 14:51:26.982289 vjer-34.1.0/vjer/vjer.py
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-34.1.0/setup.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-34.1.0/PKG-INFO
```

### Comparing `vjer-34.0.0/.github/workflows/build.yml` & `vjer-34.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/.github/workflows/publish.yml` & `vjer-34.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/.gitignore` & `vjer-34.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/.p4ignore` & `vjer-34.1.0/.p4ignore`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/CHANGELOG.md` & `vjer-34.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
+### [34.1.0] - 2024-04-19
+
+- Changed
+  - Convert extra Helm versions on pre_release to lowercase. (GitHub #12)
+
+## Release History
+
 ### [34.0.0] - 2024-04-18
 
 - Added
   - Added integration testing. (GitHub #10)
 
 - Changed
   - Remove need to specify artifact_repo in config file. (GitHub #11)
   - Rename config values docker_repo to container_registry and help_repo to helm_repository.
 
-## Release History
-
 ### [33.0.1] - 2024-04-18
 
 - Changed
   - Switched flit to be a required module. (GitHub #9)
 
 ### [33.0.0] - 2024-04-18
```

### Comparing `vjer-34.0.0/LICENSE` & `vjer-34.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/README.md` & `vjer-34.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/cicd-support/cicd.sh` & `vjer-34.1.0/cicd-support/cicd.sh`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/docs/Makefile` & `vjer-34.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/docs/coding_standards.py` & `vjer-34.1.0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/docs/conf.py` & `vjer-34.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/docs/make.bat` & `vjer-34.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/pyproject.toml` & `vjer-34.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v34.0.0"
+current_version = "v34.1.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-34.0.0/vjer/__init__.py` & `vjer-34.1.0/vjer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'Vjer'
 __summary__ = 'CI/CD Toolkit'
 __uri__ = 'https://github.com/tardis4500/vjer/'
 
-__version__ = '34.0.0'
+__version__ = '34.1.0'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `vjer-34.0.0/vjer/build.py` & `vjer-34.1.0/vjer/build.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/deploy.py` & `vjer-34.1.0/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/freeze.py` & `vjer-34.1.0/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/pre_release.py` & `vjer-34.1.0/vjer/pre_release.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             self.step_info.args = {'tag-num': True}
         super().release_bumpver()
 
     def release_helm(self) -> None:
         """Pre_release a Helm chart."""
         self._release_helm()
         for version in self.step_info.extra_versions:
-            self.project.version = version
+            self.project.version = version.lower()
             self._release_helm()
 
     def _release_helm(self) -> None:
         if self.helm_repo.type == 'oci':
             self.update_version_files()
             try:
                 self.helm_build()
```

### Comparing `vjer-34.0.0/vjer/release.py` & `vjer-34.1.0/vjer/release.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/rollback.py` & `vjer-34.1.0/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/test.py` & `vjer-34.1.0/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/tool_reporter.py` & `vjer-34.1.0/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/utils.py` & `vjer-34.1.0/vjer/utils.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/vjer/vjer.py` & `vjer-34.1.0/vjer/vjer.py`

 * *Files identical despite different names*

### Comparing `vjer-34.0.0/setup.py` & `vjer-34.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 extras_require = \
 {'dev': ['twine'], 'test': ['types-PyYAML', 'types-requests']}
 
 entry_points = \
 {'console_scripts': ['vjer = vjer.vjer:main']}
 
 setup(name='vjer',
-      version='34.0.0',
+      version='34.1.0',
       description='Vjer CI/CD module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `vjer-34.0.0/PKG-INFO` & `vjer-34.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 34.0.0
+Version: 34.1.0
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

