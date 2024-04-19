# Comparing `tmp/jupytercad_salome-1.0.0a6.tar.gz` & `tmp/jupytercad_salome-1.0.1.tar.gz`

## Comparing `jupytercad_salome-1.0.0a6.tar` & `jupytercad_salome-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/.prettierignore
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/.yarnrc.yml
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/CHANGELOG.md
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/RELEASE.md
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/install.json
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/setup.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/tsconfig.json
--rw-r--r--   0        0        0   322756 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/yarn.lock
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupyter-config/server-config/jupytercad_salome.json
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/_version.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/main.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/package.json
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/657.ee82129e76948c6af0d4.js
--rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/684.345403f1740a7a3e658e.js
--rw-r--r--   0        0        0    29772 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/688.fbf9a2083872f3817a9b.js
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/747.fc9166cbc0085e68707e.js
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/remoteEntry.52aa4a9d0bb51922e8f9.js
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/style.js
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/salome_server/handler.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/salome_server/mesh_builder.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/jupytercad_salome/schema/openapi.yaml
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/src/command.ts
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/src/handler.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/src/icon.ts
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/src/index.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/src/schema.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/src/svg.d.ts
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/src/worker.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/style/index.js
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/style/icon/grid.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/ui-tests/Dockerfile
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/ui-tests/package.json
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   144639 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/ui-tests/yarn.lock
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/ui-tests/tests/ui.spec.ts
--rw-r--r--   0        0        0    81070 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/ui-tests/tests/ui.spec.ts-snapshots/UI-Test-Mesh-generation-test-Should-be-able-to-create-mesh-without-error-1-linux.png
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/README.md
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/.prettierignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/RELEASE.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/install.json
+-rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/setup.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/tsconfig.json
+-rw-r--r--   0        0        0   325747 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/yarn.lock
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupyter-config/server-config/jupytercad_salome.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/_version.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/main.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/package.json
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/657.ee82129e76948c6af0d4.js
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/684.741e3aed6786fa46cef3.js
+-rw-r--r--   0        0        0    29772 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/688.fbf9a2083872f3817a9b.js
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/747.fc9166cbc0085e68707e.js
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/remoteEntry.2a578dcd0c361f7aaae9.js
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/style.js
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/salome_server/handler.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/salome_server/mesh_builder.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/jupytercad_salome/schema/openapi.yaml
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/src/command.ts
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/src/handler.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/src/icon.ts
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/src/index.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/src/schema.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/src/svg.d.ts
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/src/worker.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/style/index.js
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/style/icon/grid.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/ui-tests/Dockerfile
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/ui-tests/package.json
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   144639 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/ui-tests/tests/ui.spec.ts
+-rw-r--r--   0        0        0    81070 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/ui-tests/tests/ui.spec.ts-snapshots/UI-Test-Mesh-generation-test-Should-be-able-to-create-mesh-without-error-1-linux.png
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/README.md
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 jupytercad_salome-1.0.1/PKG-INFO
```

### Comparing `jupytercad_salome-1.0.0a6/.pre-commit-config.yaml` & `jupytercad_salome-1.0.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,15 @@
       - id: ruff
         args: ['--fix']
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
+        args: ['--no-error-on-unmatched-pattern']
 
   - repo: https://github.com/pre-commit/mirrors-eslint
     rev: v9.0.0-alpha.0
     hooks:
       - id: eslint
         files: \.tsx?$
         types: [file]
```

### Comparing `jupytercad_salome-1.0.0a6/CHANGELOG.md` & `jupytercad_salome-1.0.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,45 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.0.1
+
+([Full Changelog](https://github.com/jupytercad/jupytercad-salome/compare/v1.0.0...6b399abfd25689ab2fc3899f1dc0b98d529bb15e))
+
+### Enhancements made
+
+- Bump JupyterCAD [#16](https://github.com/jupytercad/jupytercad-salome/pull/16) ([@trungleduc](https://github.com/trungleduc))
+
+### Maintenance and upkeep improvements
+
+- Bump jupytercad [#15](https://github.com/jupytercad/jupytercad-salome/pull/15) ([@trungleduc](https://github.com/trungleduc))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupytercad/jupytercad-salome/graphs/contributors?from=2024-01-12&to=2024-04-19&type=c))
+
+[@trungleduc](https://github.com/search?q=repo%3Ajupytercad%2Fjupytercad-salome+involves%3Atrungleduc+updated%3A2024-01-12..2024-04-19&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
+## 1.0.0
+
+([Full Changelog](https://github.com/jupytercad/jupytercad-salome/compare/v1.0.0a6...04dd76583128290de03cfa4019327e6886db9220))
+
+### Maintenance and upkeep improvements
+
+- Bump jupytercad [#13](https://github.com/jupytercad/jupytercad-salome/pull/13) ([@trungleduc](https://github.com/trungleduc))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupytercad/jupytercad-salome/graphs/contributors?from=2024-01-04&to=2024-01-12&type=c))
+
+[@trungleduc](https://github.com/search?q=repo%3Ajupytercad%2Fjupytercad-salome+involves%3Atrungleduc+updated%3A2024-01-04..2024-01-12&type=Issues)
+
 ## 1.0.0a6
 
 ([Full Changelog](https://github.com/jupytercad/jupytercad-salome/compare/v1.0.0a5...c2ce83df6882a28abb969d8dae64133c2a284600))
 
 ### Enhancements made
 
 - Export STL in binary format [#11](https://github.com/jupytercad/jupytercad-salome/pull/11) ([@trungleduc](https://github.com/trungleduc))
@@ -16,16 +50,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupytercad/jupytercad-salome/graphs/contributors?from=2023-12-22&to=2024-01-04&type=c))
 
 [@pre-commit-ci](https://github.com/search?q=repo%3Ajupytercad%2Fjupytercad-salome+involves%3Apre-commit-ci+updated%3A2023-12-22..2024-01-04&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3Ajupytercad%2Fjupytercad-salome+involves%3Atrungleduc+updated%3A2023-12-22..2024-01-04&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.0a5
 
 ([Full Changelog](https://github.com/jupytercad/jupytercad-salome/compare/v1.0.0a4...f43f1f98e2aa334d290e6c3aaa4a9adadb2f0f8b))
 
 ### Enhancements made
 
 - Add error dialog [#9](https://github.com/jupytercad/jupytercad-salome/pull/9) ([@trungleduc](https://github.com/trungleduc))
```

### Comparing `jupytercad_salome-1.0.0a6/RELEASE.md` & `jupytercad_salome-1.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/package.json` & `jupytercad_salome-1.0.1/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904763%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.5', '@jupytercad/schema': '^2.0.0-alpha.5'}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad-salome/issues"
     },
     "dependencies": {
-        "@jupytercad/base": "^1.0.0-alpha.4",
-        "@jupytercad/schema": "^1.0.0-alpha.4",
+        "@jupytercad/base": "^2.0.0-alpha.5",
+        "@jupytercad/schema": "^2.0.0-alpha.5",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/services": "^7.0.0",
         "axios": "^1.3.5",
         "uuid": "^8.3.2"
     },
     "description": "A JupyterLab extension.",
@@ -209,9 +209,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-a6"
+    "version": "1.0.1"
 }
```

### Comparing `jupytercad_salome-1.0.0a6/tsconfig.json` & `jupytercad_salome-1.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/yarn.lock` & `jupytercad_salome-1.0.1/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -788,32 +788,32 @@
     backbone: 1.4.0
     jquery: ^3.1.1
     lodash: ^4.17.4
   checksum: 6414a56d7aaf287462b97f192f5022f9f3f52809df2e6e49b64073cb6ab851dea005033d508730140159e4dc6ef54a2af2d637c6ce3b6813a52d29fc153be296
   languageName: node
   linkType: hard
 
-"@jupyter/docprovider@npm:^1.0.0":
-  version: 1.2.0
-  resolution: "@jupyter/docprovider@npm:1.2.0"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.0
-    "@jupyterlab/services": ^7.0.0
+"@jupyter/docprovider@npm:^2.0.0":
+  version: 2.0.11
+  resolution: "@jupyter/docprovider@npm:2.0.11"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.0-a0
+    "@jupyterlab/coreutils": ^6.0.5
+    "@jupyterlab/services": ^7.0.5
     "@lumino/coreutils": ^2.1.0
     "@lumino/disposable": ^2.1.0
     "@lumino/signaling": ^2.1.0
     y-protocols: ^1.0.5
     y-websocket: ^1.3.15
     yjs: ^13.5.40
-  checksum: 8522dbb61a2e95162ad98a5377cb4d8defd7c88a7d51c4e74f67691f9cb00a0281e7b450c38af33f8aa17ca4b9c8bd76a46e0a8eae7afebe5fba2ae0f0df8b7b
+  checksum: 3af340e40781be66a7aea6b48291dcaa477fa510822aee592a10deb31c010c81b531b65189710ffc35a5279c889822ab1814e8818084abb2f90387b432b29ee6
   languageName: node
   linkType: hard
 
-"@jupyter/ydoc@npm:^0.3.4 || ^1.0.2, @jupyter/ydoc@npm:^1.0.2, @jupyter/ydoc@npm:^1.1.1":
+"@jupyter/ydoc@npm:^1.0.0, @jupyter/ydoc@npm:^1.0.2, @jupyter/ydoc@npm:^1.1.0-a0, @jupyter/ydoc@npm:^1.1.1":
   version: 1.1.1
   resolution: "@jupyter/ydoc@npm:1.1.1"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
     "@lumino/coreutils": ^1.11.0 || ^2.0.0
     "@lumino/disposable": ^1.10.0 || ^2.0.0
     "@lumino/signaling": ^1.10.0 || ^2.0.0
@@ -833,23 +833,23 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0-alpha.6
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: d6babc5ee75f646b6981636216dc26e7307fac2be5c736563efa7ee7d8cb00d2ce655efa7c17dd12bb1bc670420f83f87f2381cb9c44b16805e33065167eb349
   languageName: node
   linkType: hard
 
-"@jupytercad/base@npm:^1.0.0-alpha.4":
-  version: 1.0.0-alpha.4
-  resolution: "@jupytercad/base@npm:1.0.0-alpha.4"
+"@jupytercad/base@npm:^2.0.0-alpha.5":
+  version: 2.0.0-alpha.5
+  resolution: "@jupytercad/base@npm:2.0.0-alpha.5"
   dependencies:
     "@deathbeds/jupyterlab-rjsf": ^1.1.0
-    "@jupyter/docprovider": ^1.0.0
-    "@jupyter/ydoc": ^0.3.4 || ^1.0.2
-    "@jupytercad/occ-worker": ^1.0.0-alpha.4
-    "@jupytercad/schema": ^1.0.0-alpha.4
+    "@jupyter/docprovider": ^2.0.0
+    "@jupyter/ydoc": ^1.0.0
+    "@jupytercad/occ-worker": ^2.0.0-alpha.5
+    "@jupytercad/schema": ^2.0.0-alpha.5
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/filebrowser": ^4.0.0
     "@jupyterlab/launcher": ^4.0.0
     "@jupyterlab/observables": ^5.0.0
@@ -868,24 +868,24 @@
     d3-color: ^3.1.0
     react: ^18.0.1
     styled-components: ^5.3.6
     three: ^0.135.0
     three-mesh-bvh: ^0.5.17
     uuid: ^8.3.2
     yjs-widgets: ^0.3.3
-  checksum: 785e92dfb986c261f7af26176372d23deec5437d4ba456b0279b42c83a4dedc9e613086b5c54034e9e6e89b8a139351ac6dc2b615e0da1b592c0e68d63bbfcc0
+  checksum: 7c2a799bd302536a551bb9a6732c696b0569870915a11f589d2bf790dcf3b86048dba2c4c22a0100a68595c2198213ba32a199e920703466ae93bd921f47fa1b
   languageName: node
   linkType: hard
 
 "@jupytercad/jupytercad-salome@workspace:.":
   version: 0.0.0-use.local
   resolution: "@jupytercad/jupytercad-salome@workspace:."
   dependencies:
-    "@jupytercad/base": ^1.0.0-alpha.4
-    "@jupytercad/schema": ^1.0.0-alpha.4
+    "@jupytercad/base": ^2.0.0-alpha.5
+    "@jupytercad/schema": ^2.0.0-alpha.5
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/services": ^7.0.0
     "@types/json-schema": ^7.0.11
     "@types/react": ^18.0.26
     "@types/react-addons-linked-state-mixin": ^0.14.22
@@ -911,50 +911,50 @@
     stylelint-prettier: ^4.0.0
     typescript: ~5.0.2
     uuid: ^8.3.2
     yjs: ^13.5.0
   languageName: unknown
   linkType: soft
 
-"@jupytercad/occ-worker@npm:^1.0.0-alpha.4":
-  version: 1.0.0-alpha.4
-  resolution: "@jupytercad/occ-worker@npm:1.0.0-alpha.4"
+"@jupytercad/occ-worker@npm:^2.0.0-alpha.5":
+  version: 2.0.0-alpha.5
+  resolution: "@jupytercad/occ-worker@npm:2.0.0-alpha.5"
   dependencies:
-    "@jupytercad/opencascade": ^1.0.0-alpha.4
-    "@jupytercad/schema": ^1.0.0-alpha.4
+    "@jupytercad/opencascade": ^2.0.0-alpha.5
+    "@jupytercad/schema": ^2.0.0-alpha.5
     "@lumino/coreutils": ^2.0.0
     uuid: ^8.3.2
-  checksum: cd92f8d006066c42d7bc46c30fea11492d0a65936b933014d033fe35b7d4daac6d531a16de126d7f5a36dd6f10b4fed84036a33a9cb10cf272230b225bd4d894
+  checksum: 8e53a1386ed1175955d0172affb9d91b169a1be4e056c079dfa3d75cc885fe6dfce63a8dd62a2def792729fdbd81d29128d087c90bd681aabcf7c81f0c477a89
   languageName: node
   linkType: hard
 
-"@jupytercad/opencascade@npm:^1.0.0-alpha.4":
-  version: 1.0.0-alpha.4
-  resolution: "@jupytercad/opencascade@npm:1.0.0-alpha.4"
-  checksum: 79ea92d104b09cfc8c6e54b91341906a143745aae1b9aef5dc8ba477b80b0f3dbfb5e13a3b78129697ec35b92a2cc84fc47403d1adf8b3c6e1033453e1939e24
+"@jupytercad/opencascade@npm:^2.0.0-alpha.5":
+  version: 2.0.0-alpha.5
+  resolution: "@jupytercad/opencascade@npm:2.0.0-alpha.5"
+  checksum: e57cfd7b47eedad1fb46eb8c310627bf8dcd26969b6805f65de5dadf10a6d476d5835218b909de800d3fe6f8ebc349859619833bacd7cbe50988048c0711788b
   languageName: node
   linkType: hard
 
-"@jupytercad/schema@npm:^1.0.0-alpha.4":
-  version: 1.0.0-alpha.4
-  resolution: "@jupytercad/schema@npm:1.0.0-alpha.4"
+"@jupytercad/schema@npm:^2.0.0-alpha.5":
+  version: 2.0.0-alpha.5
+  resolution: "@jupytercad/schema@npm:2.0.0-alpha.5"
   dependencies:
     "@apidevtools/json-schema-ref-parser": ^9.0.9
-    "@jupyter/ydoc": ^0.3.4 || ^1.0.2
+    "@jupyter/ydoc": ^1.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/services": ^7.0.0
     "@jupyterlab/ui-components": ^4.0.0
     "@lumino/coreutils": ^2.0.0
     "@lumino/signaling": ^2.0.0
     ajv: ^8.12.0
     json-schema-to-typescript: ^10.1.5
     yjs: ^13.5.40
-  checksum: 06932e97c2641c10495c000c59c256037a34dd59cdfda859ead9da933677382d1e1be37b18fa482bf9ee9c93668df1430d47d85837cc9e5e1773a742af545ae7
+  checksum: 87b9f9d775f07957668b767dd80183859ef5346439f021b7d54da1d4b42e74981e5d8072996eaa089d8916b1ef657c72e6cf56e31b20e867c910c436348a399e
   languageName: node
   linkType: hard
 
 "@jupyterlab/application@npm:^4.0.0":
   version: 4.0.9
   resolution: "@jupyterlab/application@npm:4.0.9"
   dependencies:
@@ -1287,14 +1287,28 @@
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
   checksum: d2e9bb5d55f7bf3d439151ca4dbbd404adf742be31ea98a5713869f65cc86ebc8e89459ad7d0792cab51ebd7136d77ec86bf06ff990dd88f6d66780296d8983d
   languageName: node
   linkType: hard
 
+"@jupyterlab/coreutils@npm:^6.0.5, @jupyterlab/coreutils@npm:^6.1.6":
+  version: 6.1.6
+  resolution: "@jupyterlab/coreutils@npm:6.1.6"
+  dependencies:
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    minimist: ~1.2.0
+    path-browserify: ^1.0.0
+    url-parse: ~1.5.4
+  checksum: f351f327f9c7ab14ac291e4ca85a8f4289dd315e9f2e68fc6acb52efab6c47fde158f65a83ba780c382665459995bad68c7b1f9c4ffef6b9038ac81252a3f07a
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/docmanager@npm:^4.0.9":
   version: 4.0.9
   resolution: "@jupyterlab/docmanager@npm:4.0.9"
   dependencies:
     "@jupyterlab/apputils": ^4.1.9
     "@jupyterlab/coreutils": ^6.0.9
     "@jupyterlab/docregistry": ^4.0.9
@@ -1438,14 +1452,23 @@
   resolution: "@jupyterlab/nbformat@npm:3.6.6"
   dependencies:
     "@lumino/coreutils": ^1.11.0
   checksum: 43a0437c91e2eedd88d0943df13b0004928c4ed676210ad04727fbdff0154442dae6d611d5d3e6168c3a1990ac10ead172ef48e64e54f4082e9c72fc43e87adc
   languageName: node
   linkType: hard
 
+"@jupyterlab/nbformat@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/nbformat@npm:4.1.6"
+  dependencies:
+    "@lumino/coreutils": ^2.1.2
+  checksum: 4ef43fdaaecec06732528753c5316adaa883c77ae86d129fb5d1f0542124acc0e7bb5692aae799463722b8c47ce8934356572c040d682e0ce41548eca3ca421b
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/notebook@npm:^4.0.0":
   version: 4.0.9
   resolution: "@jupyterlab/notebook@npm:4.0.9"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
     "@jupyterlab/apputils": ^4.1.9
     "@jupyterlab/cells": ^4.0.9
@@ -1614,14 +1637,33 @@
     "@lumino/signaling": ^1.10.0
     node-fetch: ^2.6.0
     ws: ^7.4.6
   checksum: 5b7e4041c66c0a5519c385e0402b4b97c33e68a9d68dbb4700444a94ba02d3f4ac2940bebf31732cdf83d647ae8b041e0809464877ada6c4d38e7cb5d34e2ee6
   languageName: node
   linkType: hard
 
+"@jupyterlab/services@npm:^7.0.5":
+  version: 7.1.6
+  resolution: "@jupyterlab/services@npm:7.1.6"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/settingregistry": ^4.1.6
+    "@jupyterlab/statedb": ^4.1.6
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/polling": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    ws: ^8.11.0
+  checksum: ad47d3c9b211be4be3aad2714f3028e66ad381a6367a57f347644c693f055ee9c7655d15630a637d9181b42e89c2b8183675abc561c3959820a6bc03d3f2af12
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/settingregistry@npm:^3.6.6":
   version: 3.6.6
   resolution: "@jupyterlab/settingregistry@npm:3.6.6"
   dependencies:
     "@jupyterlab/statedb": ^3.6.6
     "@lumino/commands": ^1.19.0
     "@lumino/coreutils": ^1.11.0
@@ -1648,14 +1690,33 @@
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
   checksum: 7d4c6f3e69ac1e66b7e7c5e53ccfb98a7e073a5a69837b814f368de247ba22f830ac567a6bb231577f6e256b2b2d9c180d50542f43891640e9a5294cb3e7a189
   languageName: node
   linkType: hard
 
+"@jupyterlab/settingregistry@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/settingregistry@npm:4.1.6"
+  dependencies:
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/statedb": ^4.1.6
+    "@lumino/commands": ^2.2.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/signaling": ^2.1.2
+    "@rjsf/utils": ^5.13.4
+    ajv: ^8.12.0
+    json5: ^2.2.3
+  peerDependencies:
+    react: ">=16"
+  checksum: 93c1a4921a30243f2bd2c9591319e749e2f5cb5884f6962241857640afb6b67600cdba44fb308a23bffacc7defa3c6fc3d2ad15be52ff5946f0a8fd873b5fddd
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/shared-models@npm:^3.6.6":
   version: 3.6.6
   resolution: "@jupyterlab/shared-models@npm:3.6.6"
   dependencies:
     "@jupyter/ydoc": ~0.2.4
     "@jupyterlab/nbformat": ^3.6.6
   checksum: e53a49ac307803956f8c139da41810dd1f78d4b7e4afafc9b0c59e59389b0e70776057f7b11499b7b971042d3b3e70784748a127a5bd517a7ce9a1cd7f84fe57
@@ -1684,14 +1745,27 @@
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
   checksum: 0a813068476a1e2dad5aebbbe2a339e8931ba4e29c873d59a2baeed05ab71307e5a629802fddeaec666cec14e4bee45e0d733abe0b1ea0dbf930c8a427188e7b
   languageName: node
   linkType: hard
 
+"@jupyterlab/statedb@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/statedb@npm:4.1.6"
+  dependencies:
+    "@lumino/commands": ^2.2.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+  checksum: 4aba49eeead6ac6306ec2d8146543230db9296e7bf088380290eb4b89698b66573c00ba630890b821047b584fc59716b64ba06a013d4698551adeaf20b034301
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/statusbar@npm:^3.6.6":
   version: 3.6.6
   resolution: "@jupyterlab/statusbar@npm:3.6.6"
   dependencies:
     "@jupyterlab/apputils": ^3.6.6
     "@jupyterlab/codeeditor": ^3.6.6
     "@jupyterlab/services": ^6.6.6
@@ -2413,14 +2487,29 @@
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
   checksum: ec0d56bf2627d55759a59090db0d59402244a6fae64528f66dde1f5de2eaaf2a6841dea7bbb185eb36fd344b3abd4825b2b422f3b1b0bb05365847073aa1e790
   languageName: node
   linkType: hard
 
+"@rjsf/utils@npm:^5.13.4":
+  version: 5.18.2
+  resolution: "@rjsf/utils@npm:5.18.2"
+  dependencies:
+    json-schema-merge-allof: ^0.8.1
+    jsonpointer: ^5.0.1
+    lodash: ^4.17.21
+    lodash-es: ^4.17.21
+    react-is: ^18.2.0
+  peerDependencies:
+    react: ^16.14.0 || >=17
+  checksum: 19342ce160f5f2ff1b1448bc61b0767c9b19a3c365fe3dca221c9178dff6b54123bdfe9dd4b0314aa7965011edb0e76029f7e76226936066bfacbaaa619546b4
+  languageName: node
+  linkType: hard
+
 "@types/backbone@npm:1.4.14":
   version: 1.4.14
   resolution: "@types/backbone@npm:1.4.14"
   dependencies:
     "@types/jquery": "*"
     "@types/underscore": "*"
   checksum: 4f44bfb71d75332b5de610be7687f4ae523ad4ef02da844a828403b534b6a94a6288b32cab64371d0ad526e35cfed511652ac53af22d0b9caaac3f4cfb4375dd
```

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/__init__.py` & `jupytercad_salome-1.0.1/jupytercad_salome/__init__.py`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/main.py` & `jupytercad_salome-1.0.1/jupytercad_salome/main.py`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/package.json` & `jupytercad_salome-1.0.1/jupytercad_salome/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758432539682541%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.5', '@jupytercad/schema': '^2.0.0-alpha.5'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2a578dcd0c361f7aaae9.js'}}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad-salome/issues"
     },
     "dependencies": {
-        "@jupytercad/base": "^1.0.0-alpha.4",
-        "@jupytercad/schema": "^1.0.0-alpha.4",
+        "@jupytercad/base": "^2.0.0-alpha.5",
+        "@jupytercad/schema": "^2.0.0-alpha.5",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/services": "^7.0.0",
         "axios": "^1.3.5",
         "uuid": "^8.3.2"
     },
     "description": "A JupyterLab extension.",
@@ -108,15 +108,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupytercad/jupytercad-salome",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.52aa4a9d0bb51922e8f9.js",
+            "load": "static/remoteEntry.2a578dcd0c361f7aaae9.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupytercad_salome"
                 },
@@ -214,9 +214,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0-a6"
+    "version": "1.0.1"
 }
```

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/657.ee82129e76948c6af0d4.js` & `jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/657.ee82129e76948c6af0d4.js`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/684.345403f1740a7a3e658e.js` & `jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/684.741e3aed6786fa46cef3.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 (self.webpackChunk_jupytercad_jupytercad_salome = self.webpackChunk_jupytercad_jupytercad_salome || []).push([
     [684], {
         684: (e, t, r) => {
             "use strict";
             r.r(t), r.d(t, {
-                default: () => D
+                default: () => I
             });
-            var s = r(454),
-                n = r(483),
-                o = r(429),
-                a = r(33);
+            var s = r(242),
+                n = r(671),
+                o = r(818),
+                a = r(937);
             class i {
                 constructor(e) {
                     this.config = e
                 }
             }
             var c = r(450),
                 l = r.n(c),
@@ -76,15 +76,15 @@
                 }
             }
             Symbol.toStringTag;
             const y = e => null != e,
                 v = e => "string" == typeof e,
                 f = e => v(e) && "" !== e,
                 g = e => "object" == typeof e && "string" == typeof e.type && "function" == typeof e.stream && "function" == typeof e.arrayBuffer && "function" == typeof e.constructor && "string" == typeof e.constructor.name && /^(Blob|File)$/.test(e.constructor.name) && /^(Blob|File)$/.test(e[Symbol.toStringTag]),
-                b = async (e, t) => "function" == typeof t ? t(e) : t, E = async (e, t, r) => {
+                b = async (e, t) => "function" == typeof t ? t(e) : t, S = async (e, t, r) => {
                     const s = await b(t, e.TOKEN),
                         n = await b(t, e.USERNAME),
                         o = await b(t, e.PASSWORD),
                         a = await b(t, e.HEADERS),
                         i = "function" == typeof(null == r ? void 0 : r.getHeaders) && (null == r ? void 0 : r.getHeaders()) || {},
                         c = Object.entries({
                             Accept: "application/json",
@@ -102,15 +102,15 @@
                             } catch (t) {
                                 return Buffer.from(e).toString("base64")
                             }
                         })(`${n}:${o}`);
                         c.Authorization = `Basic ${e}`
                     }
                     return t.body && (t.mediaType ? c["Content-Type"] = t.mediaType : g(t.body) ? c["Content-Type"] = t.body.type || "application/octet-stream" : v(t.body) ? c["Content-Type"] = "text/plain" : t.body instanceof u() || (c["Content-Type"] = "application/json")), c
-                }, S = (e, t) => new m((async (r, s, n) => {
+                }, E = (e, t) => new m((async (r, s, n) => {
                     try {
                         const s = ((e, t) => {
                                 const r = e.ENCODE_PATH || encodeURI,
                                     s = t.url.replace("{api-version}", e.VERSION).replace(/{(.*?)}/g, ((e, s) => {
                                         var n;
                                         return (null === (n = t.path) || void 0 === n ? void 0 : n.hasOwnProperty(s)) ? r(String(t.path[s])) : e
                                     })),
@@ -141,15 +141,15 @@
                                         Array.isArray(t) ? t.forEach((t => r(e, t))) : r(e, t)
                                     })), t
                                 }
                             })(t),
                             i = (e => {
                                 if (e.body) return e.body
                             })(t),
-                            c = await E(e, t, a);
+                            c = await S(e, t, a);
                         if (!n.isCancelled) {
                             const d = await (async (e, t, r, s, n, o, a) => {
                                     const i = l().CancelToken.source(),
                                         c = {
                                             url: r,
                                             headers: o,
                                             data: null != s ? s : n,
@@ -203,15 +203,15 @@
                     var o
                 }));
             class _ extends i {
                 constructor(e) {
                     super(e)
                 }
                 request(e) {
-                    return S(this.config, e)
+                    return E(this.config, e)
                 }
             }
             class j {
                 constructor(e) {
                     this.httpRequest = e
                 }
                 generateMesh({
@@ -240,142 +240,150 @@
                         USERNAME: null == e ? void 0 : e.USERNAME,
                         PASSWORD: null == e ? void 0 : e.PASSWORD,
                         HEADERS: null == e ? void 0 : e.HEADERS,
                         ENCODE_PATH: null == e ? void 0 : e.ENCODE_PATH
                     }), this.execute = new j(this.request)
                 }
             }
-            var C = r(987),
-                R = r(178);
-            const O = new(r(83).LabIcon)({
+            var C = r(147),
+                R = r(464);
+            const O = new(r(805).LabIcon)({
                     name: "jupytercad:grid-icon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 -960 960 960" width="24">\n  <g class="jp-icon3" fill="#616161">\n    <path\n      d="M120-520v-320h320v320H120Zm0 400v-320h320v320H120Zm400-400v-320h320v320H520Zm0 400v-320h320v320H520ZM200-600h160v-160H200v160Zm400 0h160v-160H600v160Zm0 400h160v-160H600v160Zm-400 0h160v-160H200v160Zm400-400Zm0 240Zm-240 0Zm0-240Z" />\n  </g>\n</svg>\n'
                 }),
                 T = JSON.parse('{"type":"object","required":["Object"],"additionalProperties":false,"properties":{"Object":{"type":"string","description":"The name of input object"},"NumberOfSegments":{"type":"number","description":"The number of segments"}}}');
-            var N, A;
-            ! function(e) {
-                e.mesh = "jupytercad:salome:mesh"
-            }(N || (N = {})),
-            function(e) {
-                const t = e => {
-                    var t, r, s;
-                    const n = e.getAllObject(),
-                        o = (null === (r = null === (t = e.localState) || void 0 === t ? void 0 : t.selected) || void 0 === r ? void 0 : r.value) || [];
-                    return {
-                        Name: (0, C.newName)("Mesh", e),
-                        Object: o.length > 0 ? o[0] : null !== (s = n[0].name) && void 0 !== s ? s : "",
-                        NumberOfSegments: 10
-                    }
-                };
-                e.executeMeshOperatorFactory = function(e) {
-                    return async r => {
-                        const s = e.currentWidget;
-                        if (!s) return;
-                        const n = JSON.parse(JSON.stringify(T));
-                        n.required = ["Name", ...n.required], n.properties = {
-                            Name: {
-                                type: "string",
-                                description: "The Name of the Object"
-                            },
-                            ...n.properties
-                        };
-                        const {
-                            ...o
-                        } = n, a = new C.FormDialog({
-                            context: s.context,
-                            title: "Mesh parameters",
-                            sourceData: t(s.context.model),
-                            schema: o,
-                            syncData: (i = s.context.model, e => {
-                                const {
-                                    Name: t,
-                                    ...r
-                                } = e, s = {
-                                    shape: "Post::SalomeMesh",
-                                    parameters: r,
-                                    visible: !0,
-                                    name: t
-                                }, n = i.sharedModel;
-                                n && n.transact((() => {
-                                    r.Object.length > 0 && (0, C.setVisible)(n, r.Object, !1), n.objectExists(s.name) ? (0, R.showErrorMessage)("The object already exists", "There is an existing object with the same name.") : n.addObject(s)
-                                }))
-                            }),
-                            cancelButton: !0
-                        });
-                        var i;
-                        await a.launch()
-                    }
-                }
-            }(A || (A = {}));
-            var k, x = r(930),
-                H = r(231);
+            var N, k = r(930),
+                A = r(231);
             ! function(e) {
                 let t;
                 ! function(e) {
                     e.BREP = "brep", e.STEP = "step"
                 }(t = e.format || (e.format = {}))
-            }(k || (k = {}));
-            class P {
+            }(N || (N = {}));
+            const x = "jupytercad-salome-worker";
+            class H {
                 constructor(e) {
-                    this._ready = new x.PromiseDelegate, this._messageHandlers = new Map, this._appClient = e.appClient, this._tracker = e.tracker
+                    this.shapeFormat = s.JCadWorkerSupportedFormat.BREP, this._ready = new k.PromiseDelegate, this._messageHandlers = new Map, this._appClient = e.appClient, this._tracker = e.tracker
                 }
                 get ready() {
                     return this._ready.promise
                 }
                 register(e) {
                     const {
                         messageHandler: t,
                         thisArg: r
-                    } = e, s = (0, H.v4)();
+                    } = e, s = (0, A.v4)();
                     return r && t.bind(r), this._messageHandlers.set(s, t), s
                 }
                 unregister(e) {
                     this._messageHandlers.delete(e)
                 }
                 postMessage(e) {
-                    var t, r, n, o;
-                    if (e.action === s.WorkerAction.POSTPROCESS && e.payload && Object.keys(e.payload).length > 0) {
-                        const a = [],
-                            i = [];
-                        for (const s in e.payload) {
-                            const c = e.payload[s],
-                                l = null !== (n = null === (r = null === (t = c.jcObject) || void 0 === t ? void 0 : t.parameters) || void 0 === r ? void 0 : r.NumberOfSegments) && void 0 !== n ? n : 15,
-                                d = this._appClient.execute.generateMesh({
-                                    requestBody: {
-                                        sourcePath: null === (o = this._tracker.currentWidget) || void 0 === o ? void 0 : o.context.path,
-                                        geometry: c.occBrep,
-                                        format: k.format.BREP,
-                                        numberOfSegments: l
-                                    }
-                                });
-                            a.push(d), i.push(c.jcObject)
-                        }
-                        Promise.all(a).then((t => {
+                    var t, r, n;
+                    if (e.action === s.WorkerAction.POSTPROCESS && e.payload) {
+                        const {
+                            jcObject: o,
+                            postShape: a
+                        } = e.payload;
+                        if (!a) return;
+                        const i = null !== (r = null === (t = null == o ? void 0 : o.parameters) || void 0 === t ? void 0 : t.NumberOfSegments) && void 0 !== r ? r : 15;
+                        this._appClient.execute.generateMesh({
+                            requestBody: {
+                                sourcePath: null === (n = this._tracker.currentWidget) || void 0 === n ? void 0 : n.context.path,
+                                geometry: a,
+                                format: N.format.BREP,
+                                numberOfSegments: i
+                            }
+                        }).then((t => {
                             const r = e.id,
                                 n = [];
-                            t.forEach(((e, t) => {
-                                e.error ? (0, R.showErrorMessage)("Execution Error", e.error) : n.push({
+                            if (t.error ? (0, R.showErrorMessage)("Execution Error", t.error) : n.push({
                                     postResult: {
                                         format: "STL",
                                         binary: !0,
-                                        value: e.mesh
+                                        value: t.mesh
                                     },
-                                    jcObject: i[t]
+                                    jcObject: o
+                                }), n.length > 0) {
+                                const e = this._messageHandlers.get(r);
+                                e && e({
+                                    action: s.MainAction.DISPLAY_POST,
+                                    payload: n
                                 })
-                            }));
-                            const o = this._messageHandlers.get(r);
-                            o && o({
-                                action: s.MainAction.DISPLAY_POST,
-                                payload: n
-                            })
+                            }
                         }))
                     }
                 }
             }
-            const D = [{
+            var P, D;
+            ! function(e) {
+                e.mesh = "jupytercad:salome:mesh"
+            }(P || (P = {})),
+            function(e) {
+                const t = e => {
+                    var t, r, s;
+                    const n = e.getAllObject(),
+                        o = null === (r = null === (t = e.localState) || void 0 === t ? void 0 : t.selected) || void 0 === r ? void 0 : r.value;
+                    let a = null !== (s = n[0].name) && void 0 !== s ? s : "";
+                    if (o)
+                        for (const e in o)
+                            if ("shape" === o[e].type) {
+                                a = e;
+                                break
+                            } return {
+                        Name: (0, C.newName)("Mesh", e),
+                        Object: a,
+                        NumberOfSegments: 10
+                    }
+                };
+                e.executeMeshOperatorFactory = function(e) {
+                    return async r => {
+                        const n = e.currentWidget;
+                        if (!n) return;
+                        const o = JSON.parse(JSON.stringify(T));
+                        o.required = ["Name", ...o.required], o.properties = {
+                            Name: {
+                                type: "string",
+                                description: "The Name of the Object"
+                            },
+                            ...o.properties
+                        };
+                        const {
+                            ...a
+                        } = o, i = new C.FormDialog({
+                            context: n.context,
+                            title: "Mesh parameters",
+                            sourceData: t(n.context.model),
+                            schema: a,
+                            syncData: (c = n.context.model, e => {
+                                const {
+                                    Name: t,
+                                    ...r
+                                } = e, n = {
+                                    shape: "Post::SalomeMesh",
+                                    parameters: r,
+                                    visible: !0,
+                                    name: t,
+                                    shapeMetadata: {
+                                        shapeFormat: s.JCadWorkerSupportedFormat.BREP,
+                                        workerId: x
+                                    }
+                                }, o = c.sharedModel;
+                                o && o.transact((() => {
+                                    r.Object.length > 0 && (0, C.setVisible)(o, r.Object, !1), o.objectExists(n.name) ? (0, R.showErrorMessage)("The object already exists", "There is an existing object with the same name.") : o.addObject(n)
+                                }))
+                            }),
+                            cancelButton: !0
+                        });
+                        var c;
+                        await i.launch()
+                    }
+                }
+            }(D || (D = {}));
+            const I = [{
                 id: "jupytercad-salome:plugin",
                 description: "JupyterCad Salome plugin.",
                 autoStart: !0,
                 requires: [s.IJCadWorkerRegistryToken, s.IJCadFormSchemaRegistryToken, s.IJupyterCadDocTracker, s.IJCadExternalCommandRegistryToken],
                 optional: [a.ITranslator],
                 activate: async (e, t, r, s, i, c) => {
                     console.log("jupytercad:salome is activated!"), c = null != c ? c : a.nullTranslator;
@@ -401,33 +409,33 @@
                         }(d);
                     let h = "";
                     h = u.backend_url ? u.backend_url : l.baseUrl.replace(/\/$/, "");
                     const p = new w({
                             BASE: h,
                             TOKEN: l.token
                         }),
-                        m = new P({
+                        m = new H({
                             appClient: p,
                             tracker: s
                         });
-                    t.registerWorker("jupytercad-salome:worker", m), r.registerSchema("Post::SalomeMesh", T),
+                    t.registerWorker(x, m), r.registerSchema("Post::SalomeMesh", T),
                         function(e, t, r) {
                             const s = r.load("jupyterlab"),
                                 {
                                     commands: n
                                 } = e;
-                            n.addCommand(N.mesh, {
+                            n.addCommand(P.mesh, {
                                 label: s.__("Mesh creation"),
                                 isEnabled: () => Boolean(t.currentWidget),
                                 icon: O,
-                                execute: A.executeMeshOperatorFactory(t)
+                                execute: D.executeMeshOperatorFactory(t)
                             })
                         }(e, s, c), i.registerCommand({
                             name: "Mesh Creation",
-                            id: N.mesh
+                            id: P.mesh
                         })
                 }
             }]
         },
         230: e => {
             e.exports = "object" == typeof self ? self.FormData : window.FormData
         }
```

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/688.fbf9a2083872f3817a9b.js` & `jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/688.fbf9a2083872f3817a9b.js`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/747.fc9166cbc0085e68707e.js` & `jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/747.fc9166cbc0085e68707e.js`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/remoteEntry.52aa4a9d0bb51922e8f9.js` & `jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/remoteEntry.2a578dcd0c361f7aaae9.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -44,20 +44,20 @@
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         657: "ee82129e76948c6af0d4",
-        684: "345403f1740a7a3e658e",
+        684: "741e3aed6786fa46cef3",
         688: "fbf9a2083872f3817a9b",
         747: "fc9166cbc0085e68707e"
     } [e] + ".js?v=" + {
         657: "ee82129e76948c6af0d4",
-        684: "345403f1740a7a3e658e",
+        684: "741e3aed6786fa46cef3",
         688: "fbf9a2083872f3817a9b",
         747: "fc9166cbc0085e68707e"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -111,15 +111,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : u > i.from)) && (n[r] = {
                             get: t,
                             from: u,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (i("@jupytercad/jupytercad-salome", "1.0.0-a6", (() => w.e(684).then((() => () => w(684))))), i("axios", "1.6.2", (() => w.e(688).then((() => () => w(688))))), i("uuid", "8.3.2", (() => w.e(657).then((() => () => w(657)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@jupytercad/jupytercad-salome", "1.0.1", (() => w.e(684).then((() => () => w(684))))), i("axios", "1.6.2", (() => w.e(688).then((() => () => w(688))))), i("uuid", "8.3.2", (() => w.e(657).then((() => () => w(657)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -219,26 +219,26 @@
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, a, n)) : e(r, w.S[r], t, a, n)
     })(((e, r, t, a) => (u(e, t), d(r, 0, t, a)))), v = p(((e, r, t, a, n) => {
         var o = r && w.o(r, t) && f(r, t, a);
         return o ? c(o) : n()
     })), y = {}, b = {
-        33: () => h("default", "@jupyterlab/translation", [1, 4, 0, 10]),
-        83: () => h("default", "@jupyterlab/ui-components", [1, 4, 0, 10]),
-        178: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 10]),
+        147: () => h("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 5]),
         231: () => v("default", "uuid", [1, 8, 3, 2], (() => w.e(657).then((() => () => w(657))))),
-        429: () => h("default", "@jupyterlab/services", [1, 7, 0, 10]),
+        242: () => h("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 5]),
         450: () => v("default", "axios", [1, 1, 3, 5], (() => w.e(688).then((() => () => w(688))))),
-        454: () => h("default", "@jupytercad/schema", [1, 1, 0, 0, , "alpha", 4]),
-        483: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 10]),
+        464: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        671: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        805: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        818: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
         930: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        987: () => h("default", "@jupytercad/base", [1, 1, 0, 0, , "alpha", 4])
+        937: () => h("default", "@jupyterlab/translation", [1, 4, 1, 6])
     }, m = {
-        684: [33, 83, 178, 231, 429, 450, 454, 483, 930, 987]
+        684: [147, 231, 242, 450, 464, 671, 805, 818, 930, 937]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
             if (w.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/labextension/static/third-party-licenses.json` & `jupytercad_salome-1.0.1/jupytercad_salome/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/salome_server/handler.py` & `jupytercad_salome-1.0.1/jupytercad_salome/salome_server/handler.py`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/salome_server/mesh_builder.py` & `jupytercad_salome-1.0.1/jupytercad_salome/salome_server/mesh_builder.py`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/jupytercad_salome/schema/openapi.yaml` & `jupytercad_salome-1.0.1/jupytercad_salome/schema/openapi.yaml`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/src/command.ts` & `jupytercad_salome-1.0.1/src/command.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import { FormDialog, newName, setVisible } from '@jupytercad/base';
 import {
   IDict,
   IJCadObject,
   IJupyterCadModel,
-  IJupyterCadTracker
+  IJupyterCadTracker,
+  JCadWorkerSupportedFormat
 } from '@jupytercad/schema';
 import { JupyterFrontEnd } from '@jupyterlab/application';
 import { showErrorMessage } from '@jupyterlab/apputils';
 import { ITranslator } from '@jupyterlab/translation';
 
 import { gridIcon } from './icon';
 import formSchema from './schema.json';
+import { WORKER_ID } from './worker';
 
 export namespace CommandIDs {
   export const mesh = 'jupytercad:salome:mesh';
 }
 export function addCommands(
   app: JupyterFrontEnd,
   tracker: IJupyterCadTracker,
@@ -29,42 +31,54 @@
     execute: Private.executeMeshOperatorFactory(tracker)
   });
 }
 
 namespace Private {
   const meshOperator = {
     title: 'Mesh parameters',
-    shape: 'Post::SalomeMesh',
     default: (model: IJupyterCadModel) => {
       const objects = model.getAllObject();
-      const selected = model.localState?.selected?.value || [];
+      const selected = model.localState?.selected?.value;
+      let objectName = objects[0].name ?? '';
+      if (selected) {
+        for (const key in selected) {
+          if (selected[key].type === 'shape') {
+            objectName = key;
+            break;
+          }
+        }
+      }
       return {
         Name: newName('Mesh', model),
-        Object: selected.length > 0 ? selected[0] : objects[0].name ?? '',
+        Object: objectName,
         NumberOfSegments: 10
       };
     },
     syncData: (model: IJupyterCadModel) => {
       return (props: IDict) => {
         const { Name, ...parameters } = props;
-        const objectModel = {
-          shape: 'Post::SalomeMesh',
+        const objectModel: IJCadObject = {
+          shape: 'Post::SalomeMesh' as any,
           parameters,
           visible: true,
-          name: Name
+          name: Name,
+          shapeMetadata: {
+            shapeFormat: JCadWorkerSupportedFormat.BREP,
+            workerId: WORKER_ID
+          }
         };
         const sharedModel = model.sharedModel;
         if (sharedModel) {
           sharedModel.transact(() => {
             if (parameters['Object'].length > 0) {
               setVisible(sharedModel, parameters['Object'], false);
             }
 
             if (!sharedModel.objectExists(objectModel.name)) {
-              sharedModel.addObject(objectModel as IJCadObject);
+              sharedModel.addObject(objectModel);
             } else {
               showErrorMessage(
                 'The object already exists',
                 'There is an existing object with the same name.'
               );
             }
           });
```

### Comparing `jupytercad_salome-1.0.0a6/src/handler.ts` & `jupytercad_salome-1.0.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/src/index.ts` & `jupytercad_salome-1.0.1/src/index.ts`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import { URLExt } from '@jupyterlab/coreutils';
 import { ServerConnection } from '@jupyterlab/services';
 import { ITranslator, nullTranslator } from '@jupyterlab/translation';
 
 import { AppClient } from './_client/AppClient';
-import { CommandIDs, addCommands } from './command';
+import { addCommands, CommandIDs } from './command';
 import { API_NAMESPACE, requestAPI } from './handler';
 import formSchema from './schema.json';
-import { SalomeWorker } from './worker';
+import { SalomeWorker, WORKER_ID } from './worker';
 
 /**
  * Initialization data for the jupytercad-salome extension.
  */
 const plugin: JupyterFrontEndPlugin<void> = {
   id: 'jupytercad-salome:plugin',
   description: 'JupyterCad Salome plugin.',
@@ -60,15 +60,15 @@
     }
 
     const appClient = new AppClient({
       BASE: serverURL,
       TOKEN: settings.token
     });
     const worker = new SalomeWorker({ appClient, tracker });
-    workerRegistry.registerWorker('jupytercad-salome:worker', worker);
+    workerRegistry.registerWorker(WORKER_ID, worker);
     schemaRegistry.registerSchema('Post::SalomeMesh', formSchema);
 
     addCommands(app, tracker, translator);
     externalCommandRegistry.registerCommand({
       name: 'Mesh Creation',
       id: CommandIDs.mesh
     });
```

### Comparing `jupytercad_salome-1.0.0a6/ui-tests/yarn.lock` & `jupytercad_salome-1.0.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/ui-tests/tests/ui.spec.ts` & `jupytercad_salome-1.0.1/ui-tests/tests/ui.spec.ts`

 * *Files 16% similar despite different names*

```diff
@@ -42,18 +42,18 @@
       await page.goto();
       await page.locator('div.jpcad-Spinner').waitFor({ state: 'hidden' });
 
       await page
         .getByLabel('notebook content')
         .getByText('New JCAD File')
         .click();
-      await page.getByRole('button', { name: 'New Box' }).click();
-      await page.getByRole('button', { name: 'Submit' }).click();
-      await page.getByRole('button', { name: 'Mesh creation' }).click();
-      await page.getByRole('button', { name: 'Submit' }).click();
+      await page.getByTitle('New Box').click();
+      await page.getByText('Submit', { exact: true }).click();
+      await page.getByTitle('Mesh creation').click();
+      await page.getByText('Submit', { exact: true }).click();
       await page.waitForTimeout(1000);
       await page
         .getByRole('tablist', { name: 'main sidebar' })
         .getByRole('tab', { name: 'JupyterCad Control Panel' })
         .click();
       await page
         .getByRole('tablist', { name: 'alternate sidebar' })
```

### Comparing `jupytercad_salome-1.0.0a6/ui-tests/tests/ui.spec.ts-snapshots/UI-Test-Mesh-generation-test-Should-be-able-to-create-mesh-without-error-1-linux.png` & `jupytercad_salome-1.0.1/ui-tests/tests/ui.spec.ts-snapshots/UI-Test-Mesh-generation-test-Should-be-able-to-create-mesh-without-error-1-linux.png`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/.gitignore` & `jupytercad_salome-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/LICENSE` & `jupytercad_salome-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/README.md` & `jupytercad_salome-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupytercad_salome-1.0.0a6/pyproject.toml` & `jupytercad_salome-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "jupyter_server>=2.0.1,<3",
-    "jupytercad_core>=1.0.0a3,<2",
-    "jupytercad_lab>=1.0.0a3,<2"
+    "jupytercad_core>=2.0.0a1,<3",
+    "jupytercad_lab>=2.0.0a1,<3"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
```

### Comparing `jupytercad_salome-1.0.0a6/PKG-INFO` & `jupytercad_salome-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupytercad_salome
-Version: 1.0.0a6
+Version: 1.0.1
+Dynamic: Keywords
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/jupytercad/jupytercad-salome
 Project-URL: Bug Tracker, https://github.com/jupytercad/jupytercad-salome/issues
 Project-URL: Repository, https://github.com/jupytercad/jupytercad-salome.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
         
@@ -47,16 +48,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: jupyter-server<3,>=2.0.1
-Requires-Dist: jupytercad-core<2,>=1.0.0a3
-Requires-Dist: jupytercad-lab<2,>=1.0.0a3
+Requires-Dist: jupytercad-core<3,>=2.0.0a1
+Requires-Dist: jupytercad-lab<3,>=2.0.0a1
 Description-Content-Type: text/markdown
 
 # jupytercad_salome
 
 [![Github Actions Status](https://github.com/jupytercad/jupytercad-salome/workflows/Build/badge.svg)](https://github.com/jupytercad/jupytercad-salome/actions/workflows/build.yml)
 
 `JupyterCAD-Salome` is an extension for JupyterCAD which enables users to generate meshes from their creations in JupyterCAD, leveraging the powerful meshing capabilities of Salome, a leading open-source platform for numerical simulation.
```

