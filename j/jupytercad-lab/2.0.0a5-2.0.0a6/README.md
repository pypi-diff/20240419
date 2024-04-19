# Comparing `tmp/jupytercad_lab-2.0.0a5.tar.gz` & `tmp/jupytercad_lab-2.0.0a6.tar.gz`

## Comparing `jupytercad_lab-2.0.0a5.tar` & `jupytercad_lab-2.0.0a6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/.prettierignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/install.json
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/setup.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/tsconfig.json
--rw-r--r--   0        0        0    94325 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/_version.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/package.json
--rw-r--r--   0        0        0    21253 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/484.fd86346ab6e7cf5a316f.js
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/remoteEntry.47f30ab005e91facf7aa.js
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/style.js
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/__init__.py
--rw-r--r--   0        0        0    29682 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/cad_document.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/utils.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/y_connector.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/any.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/box.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/chamfer.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cone.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cut.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cylinder.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/extrusion.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/fillet.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/fuse.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomCircle.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomLineSegment.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/intersection.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/jcad.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/placement.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/postOperator.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sketch.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sphere.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/torus.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/index.d.ts
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/index.js
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/notebookrenderer.d.ts
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/lib/notebookrenderer.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/scripts/bump-version.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/src/index.ts
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/src/notebookrenderer.ts
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/style/index.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/LICENSE
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/README.md
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/.prettierignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/install.json
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/setup.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/tsconfig.json
+-rw-r--r--   0        0        0    94325 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/_version.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/package.json
+-rw-r--r--   0        0        0    21253 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/484.88fe3f748ad18f11119f.js
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/remoteEntry.0e2a4693e9b355fd00d8.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/style.js
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/__init__.py
+-rw-r--r--   0        0        0    29682 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/cad_document.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/utils.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/y_connector.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/any.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/box.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/chamfer.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/cone.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/cut.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/cylinder.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/extrusion.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/fillet.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/fuse.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/geomCircle.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/geomLineSegment.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/intersection.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/jcad.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/placement.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/postOperator.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/sketch.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/sphere.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/torus.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/lib/index.d.ts
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/lib/index.js
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/lib/notebookrenderer.d.ts
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/lib/notebookrenderer.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/scripts/bump-version.py
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/src/index.ts
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/src/notebookrenderer.ts
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/style/index.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/LICENSE
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/README.md
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 jupytercad_lab-2.0.0a6/PKG-INFO
```

### Comparing `jupytercad_lab-2.0.0a5/package.json` & `jupytercad_lab-2.0.0a6/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9729166666666668%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.6', '@jupytercad/jupytercad-core': "*

 * *                   "'^2.0.0-alpha.6', '@jupytercad/schema': '^2.0.0-alpha.6'}",*

 * * "'version'": "'2.0.0-alpha.6'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad/issues"
     },
     "dependencies": {
         "@jupyter/docprovider": "^2.0.0",
-        "@jupytercad/base": "^2.0.0-alpha.5",
-        "@jupytercad/jupytercad-core": "^2.0.0-alpha.5",
-        "@jupytercad/schema": "^2.0.0-alpha.5",
+        "@jupytercad/base": "^2.0.0-alpha.6",
+        "@jupytercad/jupytercad-core": "^2.0.0-alpha.6",
+        "@jupytercad/schema": "^2.0.0-alpha.6",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -114,9 +114,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0-alpha.5"
+    "version": "2.0.0-alpha.6"
 }
```

### Comparing `jupytercad_lab-2.0.0a5/tsconfig.tsbuildinfo` & `jupytercad_lab-2.0.0a6/tsconfig.tsbuildinfo`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999503968253969%*

 * *Differences: {"'program'": "{'fileInfos': {insert: [(418, "*

 * *              "'14c1ba615330caba1a7f24bc8ed4ddbcfbe05a8750ee3691a99505b18b7605ca')], delete: "*

 * *              '[418]}}'}*

```diff
@@ -5787,15 +5787,15 @@
             "becb1ba9752bab39612cd77eaf3140cca067ff0a1e651dc2b1242caf007e08b0",
             "9c554facd42b92c91cba6e487e9b9f6d012a1ea61a6d64096748e38f0946e7a7",
             "c9258d5692cbee696190eb474b532ac5069011d13f7be2ffa9af1f72f20afb5a",
             "cf3cbaee880ea25a8440feb8c49554e4d656ec003e2a7d82799a811c91bc920d",
             "9b09f3820a22f432dd59a447574b6e29aa27b24efc817024f40404c315300c4d",
             "86fbc20c92f731d0493b083291601491a93e73a3fdff9e4d25ade2458572c21e",
             "9f021433d0dcf255a95c0ccd312a6b7ea32458365dbc30d2390257cfad374630",
-            "f5183d41c569ee9a2b8ba82a97a85cc59c24f6ac33901592116ce958be4f399d",
+            "14c1ba615330caba1a7f24bc8ed4ddbcfbe05a8750ee3691a99505b18b7605ca",
             "967b1bfbb1eaa1d394465232c542bae781dcbd1aa9865a9da753c3c0ca51f032",
             "f0c4d7cd3054bf45245ab53a73336311100707472665c5b7fc90e5df7c7e795f",
             "aff801ef4268090333d6907db4fb1e1d286fbf8467283d4ee58f78d3f805c3b3",
             "43e7862403a3a325288bd4108fcb1d76d42c57fefb2a660eb46d1c1df356dbb4",
             "a81498798cca946eeaec5844059412baaca219eee731de4bb054b02faa26b8f5",
             "64a8c63ee138480e609ef6c9579c010dc0a902b61085a40f77a78b3f316cac78",
             "15afdb5ca062ea5473867906de2944f3ed87a8621e428ca60ea3a19075903cf9",
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/__init__.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/package.json` & `jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725000000000001%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.6', '@jupytercad/jupytercad-core': "*

 * *                   "'^2.0.0-alpha.6', '@jupytercad/schema': '^2.0.0-alpha.6'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.0e2a4693e9b355fd00d8.js'}}",*

 * * "'version'": "'2.0.0-alpha.6'"}*

```diff
@@ -1,17 +1,17 @@
 {
     "author": "JupyterCad contributors",
     "bugs": {
         "url": "https://github.com/jupytercad/jupytercad/issues"
     },
     "dependencies": {
         "@jupyter/docprovider": "^2.0.0",
-        "@jupytercad/base": "^2.0.0-alpha.5",
-        "@jupytercad/jupytercad-core": "^2.0.0-alpha.5",
-        "@jupytercad/schema": "^2.0.0-alpha.5",
+        "@jupytercad/base": "^2.0.0-alpha.6",
+        "@jupytercad/jupytercad-core": "^2.0.0-alpha.6",
+        "@jupytercad/schema": "^2.0.0-alpha.6",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -37,15 +37,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupytercad/jupytercad",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.47f30ab005e91facf7aa.js",
+            "load": "static/remoteEntry.0e2a4693e9b355fd00d8.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupytercad_lab"
                 },
@@ -119,9 +119,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0-alpha.5"
+    "version": "2.0.0-alpha.6"
 }
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js` & `jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/432.99819ec4f414dbcd800e.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/484.fd86346ab6e7cf5a316f.js` & `jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/484.88fe3f748ad18f11119f.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_jupytercad_jupytercad_lab = self.webpackChunk_jupytercad_jupytercad_lab || []).push([
     [484], {
         484: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => m
             });
-            var o = a(244),
-                r = a(266),
+            var o = a(965),
+                r = a(615),
                 d = a(465),
                 n = a(381),
                 s = a(714),
                 i = a(796),
                 l = a(597),
                 c = a(486),
                 u = a(230),
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js` & `jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/829.a15a497a850dc99c9a70.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/remoteEntry.47f30ab005e91facf7aa.js` & `jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/remoteEntry.0e2a4693e9b355fd00d8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -45,21 +45,21 @@
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         256: "08612c5ea708c7e41bc6",
         432: "99819ec4f414dbcd800e",
-        484: "fd86346ab6e7cf5a316f",
+        484: "88fe3f748ad18f11119f",
         767: "88bd72c65e1bf31130e2",
         829: "a15a497a850dc99c9a70"
     } [e] + ".js?v=" + {
         256: "08612c5ea708c7e41bc6",
         432: "99819ec4f414dbcd800e",
-        484: "fd86346ab6e7cf5a316f",
+        484: "88fe3f748ad18f11119f",
         767: "88bd72c65e1bf31130e2",
         829: "a15a497a850dc99c9a70"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@jupytercad/jupytercad-lab", "2.0.0-alpha.5", (() => Promise.all([S.e(256), S.e(484)]).then((() => () => S(484))))), u("yjs-widgets", "0.3.4", (() => Promise.all([S.e(829), S.e(767), S.e(256)]).then((() => () => S(829)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@jupytercad/jupytercad-lab", "2.0.0-alpha.6", (() => Promise.all([S.e(256), S.e(484)]).then((() => () => S(484))))), u("yjs-widgets", "0.3.4", (() => Promise.all([S.e(829), S.e(767), S.e(256)]).then((() => () => S(829)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -224,30 +224,30 @@
     })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
         var o = r && S.o(r, t) && f(r, t, a);
         return o ? c(o) : n()
     })), v = {}, y = {
         256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         78: () => b("default", "yjs-widgets", [2, 0, 3, 3], (() => Promise.all([S.e(829), S.e(767)]).then((() => () => S(829))))),
         230: () => h("default", "@lumino/messaging", [1, 2, 0, 0]),
-        244: () => h("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 5]),
-        266: () => h("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 5]),
         381: () => h("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
         465: () => h("default", "@jupyterlab/application", [1, 4, 1, 6]),
         486: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
         597: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        615: () => h("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 6]),
         714: () => h("default", "@jupyterlab/translation", [1, 4, 1, 6]),
         796: () => h("default", "@jupyter/docprovider", [1, 2, 0, 0]),
+        965: () => h("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 6]),
         206: () => h("default", "yjs", [1, 13, 5, 40]),
         262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         372: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 6]),
         602: () => h("default", "@lumino/signaling", [1, 2, 0, 0]),
         723: () => h("default", "@jupyterlab/rendermime", [1, 4, 1, 6])
     }, m = {
         256: [256],
-        484: [78, 230, 244, 266, 381, 465, 486, 597, 714, 796],
+        484: [78, 230, 381, 465, 486, 597, 615, 714, 796, 965],
         767: [206, 262, 372, 602, 723]
     }, g = {}, S.f.consumes = (e, r) => {
         S.o(m, e) && m[e].forEach((e => {
             if (S.o(v, e)) return r.push(v[e]);
             if (!g[e]) {
                 var t = r => {
                     v[e] = 0, S.m[e] = t => {
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/labextension/static/third-party-licenses.json` & `jupytercad_lab-2.0.0a6/jupytercad_lab/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/cad_document.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/cad_document.py`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/y_connector.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/y_connector.py`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/__init__.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/any.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/any.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  any.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel, ConfigDict, Field
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/box.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/box.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  box.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/chamfer.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/chamfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  chamfer.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cone.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/cone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  cone.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/cylinder.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/cylinder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  cylinder.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/extrusion.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/extrusion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  extrusion.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import BaseModel, ConfigDict, Field
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/fillet.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/fillet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  fillet.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomCircle.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/geomCircle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  geomCircle.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Literal
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/geomLineSegment.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/geomLineSegment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  geomLineSegment.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Literal
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/jcad.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/jcad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  jcad.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, ConfigDict, Field, RootModel, constr
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/placement.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/cut.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # generated by datamodel-codegen:
-#   filename:  placement.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   filename:  cut.json
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import BaseModel, ConfigDict, Field
 
+from . import placement
+
 
-class Model(BaseModel):
+class ICut(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
     )
-    Position: List[float] = Field(..., description='Position of the Placement')
-    Axis: List[float] = Field(..., description='Axis of the Placement')
-    Angle: float = Field(..., description='Angle of the Placement')
+    Base: str = Field(..., description='The base of the cut operator')
+    Tool: str = Field(..., description='The tool of the cut operator')
+    Refine: bool = Field(..., description='Refine shape')
+    Placement: placement.Model
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sketch.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/sketch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  sketch.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/sphere.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/sphere.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  sphere.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a5/jupytercad_lab/notebook/objects/_schema/torus.py` & `jupytercad_lab-2.0.0a6/jupytercad_lab/notebook/objects/_schema/torus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  torus.json
-#   timestamp: 2024-04-18T14:32:47+00:00
+#   timestamp: 2024-04-19T16:26:18+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from . import placement
```

### Comparing `jupytercad_lab-2.0.0a5/lib/index.js` & `jupytercad_lab-2.0.0a6/lib/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/lib/notebookrenderer.d.ts` & `jupytercad_lab-2.0.0a6/lib/notebookrenderer.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/lib/notebookrenderer.js` & `jupytercad_lab-2.0.0a6/lib/notebookrenderer.js`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/src/index.ts` & `jupytercad_lab-2.0.0a6/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/src/notebookrenderer.ts` & `jupytercad_lab-2.0.0a6/src/notebookrenderer.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/style/base.css` & `jupytercad_lab-2.0.0a6/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/LICENSE` & `jupytercad_lab-2.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/pyproject.toml` & `jupytercad_lab-2.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupytercad_lab-2.0.0a5/PKG-INFO` & `jupytercad_lab-2.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupytercad_lab
-Version: 2.0.0a5
+Version: 2.0.0a6
 Dynamic: Keywords
 Summary: JupyterCad Lab extension.
 Project-URL: Homepage, https://github.com/jupytercad/jupytercad
 Project-URL: Bug Tracker, https://github.com/jupytercad/jupytercad/issues
 Project-URL: Repository, https://github.com/jupytercad/jupytercad.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
```

