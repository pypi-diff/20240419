# Comparing `tmp/vjer-33.0.1.tar.gz` & `tmp/vjer-34.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-33.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-34.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-33.0.1.tar` & `vjer-34.0.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1788 2024-04-18 18:47:56.171917 vjer-33.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     2134 2024-04-18 18:47:56.171917 vjer-33.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     5245 2024-04-18 18:47:56.171917 vjer-33.0.1/.gitignore
--rw-r--r--   0        0        0     4999 2024-04-18 18:47:56.171917 vjer-33.0.1/.p4ignore
--rw-r--r--   0        0        0       42 2024-04-18 18:47:56.171917 vjer-33.0.1/.readthedocs.yml
--rw-r--r--   0        0        0    40281 2024-04-18 18:47:56.171917 vjer-33.0.1/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-04-18 18:47:56.171917 vjer-33.0.1/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-04-18 18:47:56.171917 vjer-33.0.1/LICENSE
--rw-r--r--   0        0        0       90 2024-04-18 18:47:56.171917 vjer-33.0.1/MANIFEST.in
--rw-r--r--   0        0        0      973 2024-04-18 18:47:56.171917 vjer-33.0.1/README.md
--rwxr-xr-x   0        0        0      878 2024-04-18 18:47:56.171917 vjer-33.0.1/cicd-support/cicd.sh
--rw-r--r--   0        0        0      634 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/conf.py
--rw-r--r--   0        0        0      795 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/make.bat
--rw-r--r--   0        0        0       59 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     2184 2024-04-18 18:48:25.336224 vjer-33.0.1/pyproject.toml
--rw-r--r--   0        0        0      305 2024-04-18 18:47:56.171917 vjer-33.0.1/util/New-Env.ps1
--rw-r--r--   0        0        0      259 2024-04-18 18:47:56.171917 vjer-33.0.1/util/Update-Env.ps1
--rwxr-xr-x   0        0        0      261 2024-04-18 18:47:56.171917 vjer-33.0.1/util/new-env.sh
--rwxr-xr-x   0        0        0      234 2024-04-18 18:47:56.171917 vjer-33.0.1/util/update-env.sh
--rw-r--r--   0        0        0      476 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer.yml
--rw-r--r--   0        0        0      654 2024-04-18 18:48:25.336224 vjer-33.0.1/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/__main__.py
--rw-r--r--   0        0        0     5278 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/freeze.py
--rw-r--r--   0        0        0     1613 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/py.typed
--rw-r--r--   0        0        0     3170 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/release.py
--rw-r--r--   0        0        0      769 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/test.py
--rw-r--r--   0        0        0     2946 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/tool_reporter.py
--rw-r--r--   0        0        0    25691 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/utils.py
--rwxr-xr-x   0        0        0     2825 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/vjer.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-33.0.1/setup.py
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-33.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1783 2024-04-18 20:17:02.276491 vjer-34.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2134 2024-04-18 20:17:02.280491 vjer-34.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5245 2024-04-18 20:17:02.280491 vjer-34.0.0/.gitignore
+-rw-r--r--   0        0        0     4999 2024-04-18 20:17:02.280491 vjer-34.0.0/.p4ignore
+-rw-r--r--   0        0        0       42 2024-04-18 20:17:02.280491 vjer-34.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    40544 2024-04-18 20:17:02.280491 vjer-34.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-04-18 20:17:02.280491 vjer-34.0.0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-18 20:17:02.280491 vjer-34.0.0/LICENSE
+-rw-r--r--   0        0        0       90 2024-04-18 20:17:02.280491 vjer-34.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      973 2024-04-18 20:17:02.280491 vjer-34.0.0/README.md
+-rwxr-xr-x   0        0        0     1046 2024-04-18 20:17:02.280491 vjer-34.0.0/cicd-support/cicd.sh
+-rw-r--r--   0        0        0      634 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-18 20:17:02.280491 vjer-34.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2184 2024-04-18 20:17:29.368613 vjer-34.0.0/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-04-18 20:17:02.280491 vjer-34.0.0/tests/vjer.yml
+-rw-r--r--   0        0        0      305 2024-04-18 20:17:02.280491 vjer-34.0.0/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-04-18 20:17:02.280491 vjer-34.0.0/util/Update-Env.ps1
+-rwxr-xr-x   0        0        0      261 2024-04-18 20:17:02.280491 vjer-34.0.0/util/new-env.sh
+-rwxr-xr-x   0        0        0      234 2024-04-18 20:17:02.280491 vjer-34.0.0/util/update-env.sh
+-rw-r--r--   0        0        0      476 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer.yml
+-rw-r--r--   0        0        0      654 2024-04-18 20:17:29.368613 vjer-34.0.0/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/__main__.py
+-rw-r--r--   0        0        0     5278 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/freeze.py
+-rw-r--r--   0        0        0     1613 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/py.typed
+-rw-r--r--   0        0        0     3170 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/test.py
+-rw-r--r--   0        0        0     2946 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    25423 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/utils.py
+-rwxr-xr-x   0        0        0     2825 2024-04-18 20:17:02.280491 vjer-34.0.0/vjer/vjer.py
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-34.0.0/setup.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-34.0.0/PKG-INFO
```

### Comparing `vjer-33.0.1/.github/workflows/build.yml` & `vjer-34.0.0/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ env.PYTHON_BUILD_VER }}
       - uses: actions/download-artifact@v4
-      - run: pip install ${{ env.ARTIFACTS_DIR }}/*.tar.gz
+      - run: cicd-support/cicd.sh "${{ github.job }}"
 
   show-run-id:
     runs-on: ubuntu-latest
     steps:
       - run: echo ${{ github.run_id }}
 
 # cSpell:ignore vjer venv
```

### Comparing `vjer-33.0.1/.github/workflows/publish.yml` & `vjer-34.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/.gitignore` & `vjer-34.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/.p4ignore` & `vjer-34.0.0/.p4ignore`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/CHANGELOG.md` & `vjer-34.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,30 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
-### [33.0.1] - 2024-04-18
+### [34.0.0] - 2024-04-18
+
+- Added
+  - Added integration testing. (GitHub #10)
 
 - Changed
-  - Switched flit to be a required module. (GitHub #9)
+  - Remove need to specify artifact_repo in config file. (GitHub #11)
+  - Rename config values docker_repo to container_registry and help_repo to helm_repository.
 
 ## Release History
 
+### [33.0.1] - 2024-04-18
+
+- Changed
+  - Switched flit to be a required module. (GitHub #9)
+
 ### [33.0.0] - 2024-04-18
 
 - Added
   - Added support for multiple Docker tags and Helm versions at build. (GitHub #8)
 
 - Changed
   - Required specification of full Docker and Helm repo info in config file.
```

### Comparing `vjer-33.0.1/LICENSE` & `vjer-34.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/README.md` & `vjer-34.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/cicd-support/cicd.sh` & `vjer-34.0.0/cicd-support/cicd.sh`

 * *Files 26% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 
 function install-pip-tools {
     pip-install pip
     pip-install setuptools wheel
 }
 
 install-pip-tools
+
+if [[ $1 == install-test ]]; then
+    pip install $ARTIFACTS_DIR/*.tar.gz
+    cd tests
+    for test in test build release; do
+        vjer $test
+    done
+    exit
+fi
+
 pip-install virtualenv
 if [[ ! -e $VIRTUAL_ENV ]]; then virtualenv $VIRTUAL_ENV; fi
 source $VIRTUAL_ENV/bin/activate
 install-pip-tools
 pip-install flit
 flit install -s --deps all
 if [[ $1 == 'pre_release' || $1 == 'release' ]]; then
```

### Comparing `vjer-33.0.1/docs/Makefile` & `vjer-34.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/docs/coding_standards.py` & `vjer-34.0.0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/docs/conf.py` & `vjer-34.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/docs/make.bat` & `vjer-34.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/pyproject.toml` & `vjer-34.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v33.0.1"
+current_version = "v34.0.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-33.0.1/vjer/build.py` & `vjer-34.0.0/vjer/build.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/deploy.py` & `vjer-34.0.0/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/freeze.py` & `vjer-34.0.0/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/pre_release.py` & `vjer-34.0.0/vjer/pre_release.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/release.py` & `vjer-34.0.0/vjer/release.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/rollback.py` & `vjer-34.0.0/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/test.py` & `vjer-34.0.0/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/tool_reporter.py` & `vjer-34.0.0/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/vjer/utils.py` & `vjer-34.0.0/vjer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,19 +262,14 @@
         for section in _CONFIG_SECTIONS:
             if section in yaml_as_dict:
                 self._sections[section].update(yaml_as_dict[section])
 
     def _set_defaults(self) -> None:
         self.project.update_defaults(DotMap(artifacts_dir=self.project.project_root / self.project.build_artifacts,
                                             test_results_dir=self.project.project_root / self.project.test_results))
-        if hasattr(self.project, 'artifact_repo'):
-            if hasattr(self.project, 'docker_repo'):
-                self.project.update_defaults(DotMap(container_registry=DotMap(self.project.docker_repo)))
-            if hasattr(self.project, 'helm_repo'):
-                self.project.update_defaults(DotMap(chart_repo=DotMap(self.project.helm_repo)))
 
     def _set_version(self) -> None:
         match self.project.version_service.type:
             case 'bumpver':
                 self.project.version = bumpver_config()[1].pep440_version
             case 'environment':
                 self.project.version = getenv(self.project.version_service.variable, '').rstrip('.')
@@ -351,17 +346,17 @@
         Args:
             login (optional, default=True): If True, login to the Docker image registry.
             mode (optional, default='pull'): The mode for which this initialization will be used.
 
         Returns:
             Nothing.
         """
-        self.registry_client = Cloud(CloudType.gcloud if (self.container_registry.type == 'gcp') else CloudType.local, login=login)
+        self.registry_client = Cloud(CloudType.gcloud if (self.project.container_registry.type == 'gcp') else CloudType.local, login=login)
         self.docker_client = Cloud(CloudType.local)
-        registry_name_path = f'{self.container_registry.name}/' if login else ''
+        registry_name_path = f'{self.project.container_registry.name}/' if login else ''
         self.image_name = f'{registry_name_path}{self.step_info.image if self.step_info.image else self.project.name}'
         self.version_tag = f'{self.image_name}:{self.project.version}'
         self.image_tag = f'{self.version_tag}-{self.build.build_num}'.lower()
 
     def _execute(self) -> None:
         """This method is called by the Action super class when this class's execute method is called."""
         class_name = type(self).__name__.lower().removeprefix('pre').removesuffix('step')
@@ -385,20 +380,20 @@
         if self.step_info.helm_variables:
             helm_args['set'] = ','.join([f'{k}={v}' for (k, v) in self.step_info.helm_variables.items()])
         return helm_args
 
     @property
     def helm_repo(self) -> DotMap:
         """A read-only property which returns the Helm repo name with a randomized suffix."""
-        if (self.chart_repo.type != 'oci') and self.chart_repo.url and not self.chart_repo.name:
+        if (self.project.helm_repository.type != 'oci') and self.project.helm_repository.url and not self.project.helm_repository.name:
             repo_name = f'vjer-{randint(0, 100)}'
             helm('repo', 'add', repo_name, self.chart_repo.url)
             helm('repo', 'update')
-            self.chart_repo.name = repo_name
-        return self.chart_repo
+            self.project.helm_repository.name = repo_name
+        return self.project.helm_repository
 
     def commit_files(self, message: str, branch: str, *files, file_updater: Optional[Callable] = None) -> None:
         """Checkin files during to the source repository."""
         self.git_client.client.add_remote_ref(remote_ref := REMOTE_REF, self.git_client.CI_REMOTE_REF, exists_ok=True)
         git('fetch', all=True, syscmd_args={'ignore_stderr': True})
         git('remote', 'update', remote_ref, prune=True, syscmd_args={'ignore_stderr': True})
         git('checkout', '-B', branch, '--track', f'{remote_ref}/{branch}', syscmd_args={'ignore_stderr': True})
@@ -456,15 +451,15 @@
         Args:
             source_Tag: The tag of the existing image to which to add the new tags.
             tags: The list of tags to add.
 
         Returns:
             Nothing.
         """
-        if (registry := self.container_registry).type not in ('gcp', 'gcp-art'):
+        if (registry := self.project.container_registry).type not in ('gcp', 'gcp-art'):
             (image := self.registry_client.get_image(source_tag)).pull()
         for tag in tags:
             self.log_message(f'Tagging image: {tag}')
             match registry.type:
                 case 'gcp':
                     gcloud('container', 'images', 'add-tag', source_tag, tag, syscmd_args={'ignore_stderr': True})
                 case 'gcp-art':
```

### Comparing `vjer-33.0.1/vjer/vjer.py` & `vjer-34.0.0/vjer/vjer.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.1/setup.py` & `vjer-34.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 extras_require = \
 {'dev': ['twine'], 'test': ['types-PyYAML', 'types-requests']}
 
 entry_points = \
 {'console_scripts': ['vjer = vjer.vjer:main']}
 
 setup(name='vjer',
-      version='33.0.1',
+      version='34.0.0',
       description='Vjer CI/CD module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `vjer-33.0.1/PKG-INFO` & `vjer-34.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 33.0.1
+Version: 34.0.0
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

