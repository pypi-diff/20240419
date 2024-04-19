# Comparing `tmp/jupytercad_core-2.0.0a5.tar.gz` & `tmp/jupytercad_core-2.0.0a6.tar.gz`

## Comparing `jupytercad_core-2.0.0a5.tar` & `jupytercad_core-2.0.0a6.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/extension.webpack.config.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/install.json
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/setup.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/tsconfig.json
--rw-r--r--   0        0        0   101190 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupyter-config/server-config/jupytercad_core.json
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/_version.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/handlers.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/jcad_ydoc.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/step_ydoc.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/stl_ydoc.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/package.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js
--rw-r--r--   0        0        0   237762 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/201.7c726c3797b41065333d.js
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js
--rw-r--r--   0        0        0    18674 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js.LICENSE.txt
--rw-r--r--   0        0        0   113655 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/32.a95d615bf766af4875ef.js
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js
--rw-r--r--   0        0        0   183516 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js
--rw-r--r--   0        0        0    13710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/413.ef292566c68bab717b65.js
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js
--rw-r--r--   0        0        0   103210 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js
--rw-r--r--   0        0        0  1120083 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js.LICENSE.txt
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/794.ef97522617bcf473b833.js
--rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/813.f59d706f506dbfe48994.js
--rw-r--r--   0        0        0  8606972 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/remoteEntry.8944d87432fbcb496854.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/style.js
--rw-r--r--   0        0        0    64526 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/externalcommand.d.ts
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/externalcommand.js
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/factory.d.ts
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/factory.js
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/index.d.ts
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/index.js
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/plugin.d.ts
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/plugin.js
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/schemaregistry.d.ts
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/schemaregistry.js
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/workerregistry.d.ts
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/workerregistry.js
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/jcadplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/jcadplugin/modelfactory.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/jcadplugin/plugins.d.ts
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/jcadplugin/plugins.js
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stepplugin/model.d.ts
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stepplugin/model.js
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stepplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stepplugin/modelfactory.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stepplugin/plugins.d.ts
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stepplugin/plugins.js
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stlplugin/model.d.ts
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stlplugin/model.js
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stlplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stlplugin/modelfactory.js
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stlplugin/plugins.d.ts
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/lib/stlplugin/plugins.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/node_modules/.bin/webpack -> ../../../../node_modules/webpack/bin/webpack.js
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/scripts/bump-version.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/externalcommand.ts
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/factory.ts
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/index.ts
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/plugin.ts
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/schemaregistry.ts
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/workerregistry.ts
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/jcadplugin/modelfactory.ts
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/jcadplugin/plugins.ts
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/stepplugin/model.ts
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/stepplugin/modelfactory.ts
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/stepplugin/plugins.ts
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/stlplugin/model.ts
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/stlplugin/modelfactory.ts
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/src/stlplugin/plugins.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/style/index.js
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/README.md
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/extension.webpack.config.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/install.json
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/setup.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/tsconfig.json
+-rw-r--r--   0        0        0   101190 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupyter-config/server-config/jupytercad_core.json
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/_version.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/handlers.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/jcad_ydoc.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/step_ydoc.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/stl_ydoc.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/package.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js
+-rw-r--r--   0        0        0   237762 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/201.7c726c3797b41065333d.js
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js
+-rw-r--r--   0        0        0    18674 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js.LICENSE.txt
+-rw-r--r--   0        0        0   113742 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/32.249c6bd27daaea51e991.js
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js
+-rw-r--r--   0        0        0   183516 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js
+-rw-r--r--   0        0        0    13710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/413.e3edef5e15636d5f7630.js
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js
+-rw-r--r--   0        0        0   103210 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js
+-rw-r--r--   0        0        0  1120083 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js.LICENSE.txt
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/794.55a891e10ed7a9b7a805.js
+-rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/813.013761880a7e5d30e958.js
+-rw-r--r--   0        0        0  8606972 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0    10430 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/remoteEntry.42b7768c40743ee87403.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/style.js
+-rw-r--r--   0        0        0    64526 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/externalcommand.d.ts
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/externalcommand.js
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/factory.d.ts
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/factory.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/index.d.ts
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/index.js
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/plugin.d.ts
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/plugin.js
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/schemaregistry.d.ts
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/schemaregistry.js
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/workerregistry.d.ts
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/workerregistry.js
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/jcadplugin/plugins.js
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/model.d.ts
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/model.js
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/plugins.d.ts
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stepplugin/plugins.js
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/model.d.ts
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/model.js
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.js
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/plugins.d.ts
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/lib/stlplugin/plugins.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/build-labextension -> ../../../../node_modules/@jupyterlab/builder/lib/build-labextension.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/mkdirp -> ../../../../node_modules/mkdirp/bin/cmd.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/npm-run-all -> ../../../../node_modules/npm-run-all/bin/npm-run-all/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/rimraf -> ../../../../node_modules/rimraf/bin.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/run-p -> ../../../../node_modules/npm-run-all/bin/run-p/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/run-s -> ../../../../node_modules/npm-run-all/bin/run-s/index.js
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/tsc -> ../../../../node_modules/typescript/bin/tsc
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/tsserver -> ../../../../node_modules/typescript/bin/tsserver
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/node_modules/.bin/webpack -> ../../../../node_modules/webpack/bin/webpack.js
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/scripts/bump-version.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/externalcommand.ts
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/factory.ts
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/index.ts
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/plugin.ts
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/schemaregistry.ts
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/workerregistry.ts
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/jcadplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/jcadplugin/plugins.ts
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stepplugin/model.ts
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stepplugin/modelfactory.ts
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stepplugin/plugins.ts
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stlplugin/model.ts
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stlplugin/modelfactory.ts
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/src/stlplugin/plugins.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/style/index.js
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/README.md
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jupytercad_core-2.0.0a6/PKG-INFO
```

### Comparing `jupytercad_core-2.0.0a5/extension.webpack.config.js` & `jupytercad_core-2.0.0a6/extension.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/package.json` & `jupytercad_core-2.0.0a6/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9724999999999999%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.6', '@jupytercad/occ-worker': "*

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
-        "@jupytercad/occ-worker": "^2.0.0-alpha.5",
-        "@jupytercad/schema": "^2.0.0-alpha.5",
+        "@jupytercad/base": "^2.0.0-alpha.6",
+        "@jupytercad/occ-worker": "^2.0.0-alpha.6",
+        "@jupytercad/schema": "^2.0.0-alpha.6",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
         "@jupyterlab/services": "^7.0.0",
@@ -116,9 +116,9 @@
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

### Comparing `jupytercad_core-2.0.0a5/tsconfig.tsbuildinfo` & `jupytercad_core-2.0.0a6/tsconfig.tsbuildinfo`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999067859806114%*

 * *Differences: {"'program'": "{'fileInfos': {insert: [(419, "*

 * *              "'14c1ba615330caba1a7f24bc8ed4ddbcfbe05a8750ee3691a99505b18b7605ca'), (503, "*

 * *              "'2b9acc85b8a75a1720300c969831f4fc6be44c4edbeba81286168ee262584512')], delete: [503, "*

 * *              '419]}}'}*

```diff
@@ -6206,15 +6206,15 @@
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
@@ -6320,15 +6320,15 @@
             "e3643474c1823585fb7b0ab772a17c668faa6bb6ad1e18254956d6d3e1a615c3",
             "3fdee1fdcbf954cdc5c4e84928f10f8d65c8cbde9db953e1cb0538bddf2f2331",
             "28cd8d1f6bb01be3681b2e82b03dfc9b0d796117762f9af7a9a0e17f21cd9cce",
             {
                 "signature": "ff98c70b5486ea9a33e433a36353094b70abcc1394cd59751e5fc48cb07c8362",
                 "version": "1ee7b1bf627087baa464397169e9f45d6a07e797164444e2ca2016bab1e24695"
             },
-            "61cd80f281d9f2f8283a5c5fd9f30d3b26f3af72c192faaf0a32730118fd7179",
+            "2b9acc85b8a75a1720300c969831f4fc6be44c4edbeba81286168ee262584512",
             {
                 "signature": "94f153dc366146b0b048372c38272a6189b5b18aee07ca6bba98f6f67ad28514",
                 "version": "09e72ffbe0d4f37f8aeaef3cceb166fed8598f8bd1217d93fb789d8f1721db4f"
             },
             {
                 "signature": "05c6dd04dae483ac84b2505ec19ea5ca902d31472f34c6e0f048ad3ccee6e7a4",
                 "version": "d2e394b11d5d2680edec1c830cf1d7279f3a5d1dff79f5e1e3b7091f2fe5fbe2"
```

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/__init__.py` & `jupytercad_core-2.0.0a6/jupytercad_core/__init__.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/handlers.py` & `jupytercad_core-2.0.0a6/jupytercad_core/handlers.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/jcad_ydoc.py` & `jupytercad_core-2.0.0a6/jupytercad_core/jcad_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/step_ydoc.py` & `jupytercad_core-2.0.0a6/jupytercad_core/step_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/stl_ydoc.py` & `jupytercad_core-2.0.0a6/jupytercad_core/stl_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/package.json` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9721527777777779%*

 * *Differences: {"'dependencies'": "{'@jupytercad/base': '^2.0.0-alpha.6', '@jupytercad/occ-worker': "*

 * *                   "'^2.0.0-alpha.6', '@jupytercad/schema': '^2.0.0-alpha.6'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.42b7768c40743ee87403.js'}}",*

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
-        "@jupytercad/occ-worker": "^2.0.0-alpha.5",
-        "@jupytercad/schema": "^2.0.0-alpha.5",
+        "@jupytercad/base": "^2.0.0-alpha.6",
+        "@jupytercad/occ-worker": "^2.0.0-alpha.6",
+        "@jupytercad/schema": "^2.0.0-alpha.6",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
         "@jupyterlab/services": "^7.0.0",
@@ -40,15 +40,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupytercad/jupytercad",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8944d87432fbcb496854.js",
+            "load": "static/remoteEntry.42b7768c40743ee87403.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupytercad_core"
                 },
@@ -121,9 +121,9 @@
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

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/197.93f84c7921605ea391a1.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/201.7c726c3797b41065333d.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/201.7c726c3797b41065333d.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/226.9d3aa6c870e5597b7470.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/279.04093e206c0c74048dd7.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/32.a95d615bf766af4875ef.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/32.249c6bd27daaea51e991.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2355,37 +2355,42 @@
                         d = new _e.XJ7(l.geometry),
                         c = new _e.mrM({
                             color: "black"
                         }),
                         h = new _e.DXC(d, c);
                     l.add(h), l.name = e, l.visible = !0, this._meshGroup && (this._meshGroup.add(l), null === (n = this._boundingGroup) || void 0 === n || n.expandByObject(l)), this._updateRefLength(!0)
                 }
-                _requestRender(e, t) {
+                async _requestRender(e, t) {
                     const {
                         shapes: n,
                         postShapes: i,
                         postResult: s
                     } = t;
                     if (null != n) {
                         this._shapeToMesh(t.shapes);
                         const e = {
                             binary: !0,
                             onlyVisible: !1
                         };
                         if (s && this._meshGroup) {
-                            const t = new ye.r;
-                            Object.values(s).forEach((n => {
-                                var i;
-                                const s = null === (i = n.jcObject.parameters) || void 0 === i ? void 0 : i.Object;
-                                if (!s) return;
-                                const o = this._meshGroup.getObjectByName(`${s}-group`);
-                                o && t.parse(o, (e => {
-                                    n.postShape = e
-                                }), e)
-                            })), this._mainViewModel.sendRawGeomeryToWorker(s)
+                            const t = new ye.r,
+                                n = [];
+                            Object.values(s).forEach((i => {
+                                var s;
+                                const o = null === (s = i.jcObject.parameters) || void 0 === s ? void 0 : s.Object;
+                                if (!o) return;
+                                const a = this._meshGroup.getObjectByName(`${o}-group`);
+                                if (!a) return;
+                                const r = new Promise((n => {
+                                    t.parse(a, (e => {
+                                        i.postShape = e, n()
+                                    }), e)
+                                }));
+                                n.push(r)
+                            })), await Promise.all(n), this._mainViewModel.sendRawGeometryToWorker(s)
                         }
                     }
                     null != i && Object.entries(i).forEach((([e, t]) => {
                         this._objToMesh(e, t)
                     }))
                 }
                 _updatePointers(e) {
@@ -2562,15 +2567,15 @@
                         }
                     }))
                 }
             }
             var Re = n(8859),
                 ze = n(8265),
                 Ve = n(4602),
-                Fe = n(3037);
+                Fe = n(3342);
             class Ge {
                 constructor(e) {
                     this.messageHandler = e => {
                         switch (e.action) {
                             case Fe.MainAction.DISPLAY_SHAPE: {
                                 const {
                                     result: t,
@@ -2587,15 +2592,15 @@
                                         postShapes: e,
                                         postResult: s
                                     }), this._firstRender = !1
                                 } else this._renderSignal.emit({
                                     shapes: t,
                                     postShapes: null,
                                     postResult: s
-                                }), this.sendRawGeomeryToWorker(i);
+                                }), this.sendRawGeometryToWorker(i);
                                 break
                             }
                             case Fe.MainAction.INITIALIZED: {
                                 if (!this._jcadModel) return;
                                 const e = this._jcadModel.getContent();
                                 this._postMessage({
                                     action: Fe.WorkerAction.LOAD_FILE,
@@ -2662,15 +2667,15 @@
                     }), this._workerRegistry.getAllWorkers().forEach((e => {
                         const t = e.register({
                             messageHandler: this.postProcessWorkerHandler.bind(this)
                         });
                         this._postWorkerId.set(t, e)
                     }))
                 }
-                sendRawGeomeryToWorker(e) {
+                sendRawGeometryToWorker(e) {
                     Object.values(e).forEach((e => {
                         this._postWorkerId.forEach(((t, n) => {
                             var i, s;
                             if (!e.jcObject.shape) return;
                             const {
                                 shapeFormat: o,
                                 workerId: a
```

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/341.dc0a046959cb1d02b85c.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/36.699cdc9ecc81734b4ed2.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/366.f05a9a2d265b69bc39df.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/413.ef292566c68bab717b65.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/413.e3edef5e15636d5f7630.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -149,15 +149,15 @@
                             }
                         }
                         r.push(c)
                     }
                     return r
                 }
             }
-            var n, s = r(3037),
+            var n, s = r(3342),
                 a = r(7262),
                 i = new Uint8Array(16);
 
             function p() {
                 if (!n && !(n = "undefined" != typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto) || "undefined" != typeof msCrypto && "function" == typeof msCrypto.getRandomValues && msCrypto.getRandomValues.bind(msCrypto))) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
                 return n(i)
             }
```

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/432.95862c204ad10cbf88b7.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/509.74b2abfe3e59889c4fb9.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/601.cf6a431ba637c1b317f2.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/702.ec2cae811960a903c14a.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/733.56e708a06e7632c214b0.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/794.ef97522617bcf473b833.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/794.55a891e10ed7a9b7a805.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -149,15 +149,15 @@
                             }
                         }
                         r.push(c)
                     }
                     return r
                 }
             }
-            var n, s = r(3037),
+            var n, s = r(3342),
                 a = r(7262),
                 i = new Uint8Array(16);
 
             function p() {
                 if (!n && !(n = "undefined" != typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto) || "undefined" != typeof msCrypto && "function" == typeof msCrypto.getRandomValues && msCrypto.getRandomValues.bind(msCrypto))) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
                 return n(i)
             }
```

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/813.f59d706f506dbfe48994.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/813.013761880a7e5d30e958.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,21 +4,21 @@
         2813: (e, t, r) => {
             r.r(t), r.d(t, {
                 JupyterCadWidgetFactory: () => l,
                 JupyterCadWorkerRegistry: () => S,
                 default: () => I
             });
             var i = r(4796),
-                n = r(3037),
+                n = r(3342),
                 o = r(7638),
                 a = r(9221),
                 s = r(1595),
                 c = r(7664),
                 d = r(8859),
-                p = r(597);
+                p = r(8626);
             class l extends d.ABCWidgetFactory {
                 constructor(e) {
                     const {
                         backendCheck: t,
                         externalCommandRegistry: r
                     } = e;
                     super(function(e, t) {
@@ -355,15 +355,15 @@
                             t.save(n)
                         })), r.themeChanged.connect(((e, t) => n.context.model.themeChanged.emit(t))), t.add(n), e.shell.activateById("jupytercad::leftControlPanel"), e.shell.activateById("jupytercad::rightControlPanel")
                     }))
                 }
             };
             var T = r(1381),
                 k = r(7714),
-                w = r(3503);
+                w = r(492);
             class S {
                 constructor() {
                     this._registry = new Map;
                     const e = new Worker(new URL(r.p + r.u(201), r.b));
                     this._defaultWorker = new w.OccWorker({
                         worker: e
                     })
@@ -380,15 +380,15 @@
                 getWorker(e) {
                     return this._registry.get(e)
                 }
                 getAllWorkers() {
                     return [...this._registry.values()]
                 }
             }
-            const R = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the object":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Post::Operator":{"type":"object","required":["Object"],"additionalProperties":true,"properties":{"Object":{"type":"string","description":"The name of input object"}}},"Part::Any":{"type":"object","required":["Content","Type"],"additionalProperties":false,"properties":{"Content":{"type":"string","description":"The string content of the object"},"Type":{"type":"string","enum":["brep","step","stl"]},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Chamfer":{"type":"object","required":["Base","Edge","Dist","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Dist":{"type":"number","description":"The distance of the symmetric chamfer"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Fillet":{"type":"object","required":["Base","Edge","Radius","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Radius":{"type":"number","description":"The radius for the fillet"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
+            const R = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the object":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Post::Operator":{"type":"object","required":["Object"],"additionalProperties":true,"properties":{"Object":{"type":"string","description":"The name of input object"}}},"Part::Any":{"type":"object","required":["Content","Type"],"additionalProperties":false,"properties":{"Content":{"type":"string","description":"The string content of the object"},"Type":{"type":"string","enum":["brep","step","stl"]},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Chamfer":{"type":"object","required":["Base","Edge","Dist","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Dist":{"type":"number","description":"The distance of the symmetric chamfer"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Fillet":{"type":"object","required":["Base","Edge","Radius","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The name of input object"},"Edge":{"type":"number","description":"The edge index"},"Radius":{"type":"number","description":"The radius for the fillet"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
             class v {
                 constructor() {
                     this._registry = new Map(Object.entries(R))
                 }
                 registerSchema(e, t) {
                     this._registry.has(e) ? console.error("Worker is already registered!") : this._registry.set(e, t)
                 }
```

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/jupytercad.opencascade.wasm` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/remoteEntry.8944d87432fbcb496854.js` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/remoteEntry.42b7768c40743ee87403.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,360 +1,360 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, a, t, o, n, f, l, u, c, i, d, s, p, b, h, v, m, y, g, j, w, P, S, k, E = {
-            2401: (e, r, a) => {
-                var t = {
-                        "./index": () => Promise.all([a.e(262), a.e(602), a.e(37), a.e(644), a.e(813)]).then((() => () => a(2813))),
-                        "./extension": () => Promise.all([a.e(262), a.e(602), a.e(37), a.e(644), a.e(813)]).then((() => () => a(2813))),
-                        "./style": () => a.e(432).then((() => () => a(1432)))
+    var e, r, t, a, o, n, d, f, l, u, i, c, s, p, b, h, v, m, y, g, j, w, P, S, k, E = {
+            2401: (e, r, t) => {
+                var a = {
+                        "./index": () => Promise.all([t.e(262), t.e(602), t.e(342), t.e(644), t.e(813)]).then((() => () => t(2813))),
+                        "./extension": () => Promise.all([t.e(262), t.e(602), t.e(342), t.e(644), t.e(813)]).then((() => () => t(2813))),
+                        "./style": () => t.e(432).then((() => () => t(1432)))
                     },
-                    o = (e, r) => (a.R = r, r = a.o(t, e) ? t[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
-                    })), a.R = void 0, r),
+                    })), t.R = void 0, r),
                     n = (e, r) => {
-                        if (a.S) {
-                            var t = "default",
-                                o = a.S[t];
+                        if (t.S) {
+                            var a = "default",
+                                o = t.S[a];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return a.S[t] = e, a.I(t, r)
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
-                a.d(r, {
+                t.d(r, {
                     get: () => o,
                     init: () => n
                 })
             }
         },
         _ = {};
 
     function x(e) {
         var r = _[e];
         if (void 0 !== r) return r.exports;
-        var a = _[e] = {
+        var t = _[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return E[e].call(a.exports, a, a.exports, x), a.loaded = !0, a.exports
+        return E[e].call(t.exports, t, t.exports, x), t.loaded = !0, t.exports
     }
     x.m = E, x.c = _, x.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return x.d(r, {
             a: r
         }), r
     }, x.d = (e, r) => {
-        for (var a in r) x.o(r, a) && !x.o(e, a) && Object.defineProperty(e, a, {
+        for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
-            get: r[a]
+            get: r[t]
         })
-    }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, a) => (x.f[a](e, r), r)), [])), x.u = e => e + "." + {
-        32: "a95d615bf766af4875ef",
+    }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
+        32: "249c6bd27daaea51e991",
         36: "699cdc9ecc81734b4ed2",
-        37: "a3720679bc8be37b0b7f",
         197: "93f84c7921605ea391a1",
         201: "7c726c3797b41065333d",
         226: "9d3aa6c870e5597b7470",
         262: "a4099c9aa3c3452ec3d3",
         279: "04093e206c0c74048dd7",
         341: "dc0a046959cb1d02b85c",
+        342: "c1128ed25dbde3d0f9fd",
         366: "f05a9a2d265b69bc39df",
-        413: "ef292566c68bab717b65",
+        413: "e3edef5e15636d5f7630",
         432: "95862c204ad10cbf88b7",
         509: "74b2abfe3e59889c4fb9",
         601: "cf6a431ba637c1b317f2",
         602: "4c95dde683ea2cdb62eb",
         644: "42ff2779d9e633efa2b0",
         702: "ec2cae811960a903c14a",
         733: "56e708a06e7632c214b0",
-        794: "ef97522617bcf473b833",
-        813: "f59d706f506dbfe48994"
+        794: "55a891e10ed7a9b7a805",
+        813: "013761880a7e5d30e958"
     } [e] + ".js?v=" + {
-        32: "a95d615bf766af4875ef",
+        32: "249c6bd27daaea51e991",
         36: "699cdc9ecc81734b4ed2",
-        37: "a3720679bc8be37b0b7f",
         197: "93f84c7921605ea391a1",
         201: "7c726c3797b41065333d",
         226: "9d3aa6c870e5597b7470",
         262: "a4099c9aa3c3452ec3d3",
         279: "04093e206c0c74048dd7",
         341: "dc0a046959cb1d02b85c",
+        342: "c1128ed25dbde3d0f9fd",
         366: "f05a9a2d265b69bc39df",
-        413: "ef292566c68bab717b65",
+        413: "e3edef5e15636d5f7630",
         432: "95862c204ad10cbf88b7",
         509: "74b2abfe3e59889c4fb9",
         601: "cf6a431ba637c1b317f2",
         602: "4c95dde683ea2cdb62eb",
         644: "42ff2779d9e633efa2b0",
         702: "ec2cae811960a903c14a",
         733: "56e708a06e7632c214b0",
-        794: "ef97522617bcf473b833",
-        813: "f59d706f506dbfe48994"
+        794: "55a891e10ed7a9b7a805",
+        813: "013761880a7e5d30e958"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupytercad/jupytercad-core:", x.l = (a, t, o, n) => {
-        if (e[a]) e[a].push(t);
+    }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupytercad/jupytercad-core:", x.l = (t, a, o, n) => {
+        if (e[t]) e[t].push(a);
         else {
-            var f, l;
+            var d, f;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), c = 0; c < u.length; c++) {
-                    var i = u[c];
-                    if (i.getAttribute("src") == a || i.getAttribute("data-webpack") == r + o) {
-                        f = i;
+                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
+                    var i = l[u];
+                    if (i.getAttribute("src") == t || i.getAttribute("data-webpack") == r + o) {
+                        d = i;
                         break
                     }
                 }
-            f || (l = !0, (f = document.createElement("script")).charset = "utf-8", f.timeout = 120, x.nc && f.setAttribute("nonce", x.nc), f.setAttribute("data-webpack", r + o), f.src = a), e[a] = [t];
-            var d = (r, t) => {
-                    f.onerror = f.onload = null, clearTimeout(s);
-                    var o = e[a];
-                    if (delete e[a], f.parentNode && f.parentNode.removeChild(f), o && o.forEach((e => e(t))), r) return r(t)
+            d || (f = !0, (d = document.createElement("script")).charset = "utf-8", d.timeout = 120, x.nc && d.setAttribute("nonce", x.nc), d.setAttribute("data-webpack", r + o), d.src = t), e[t] = [a];
+            var c = (r, a) => {
+                    d.onerror = d.onload = null, clearTimeout(s);
+                    var o = e[t];
+                    if (delete e[t], d.parentNode && d.parentNode.removeChild(d), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(d.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
-                    target: f
+                    target: d
                 }), 12e4);
-            f.onerror = d.bind(null, f.onerror), f.onload = d.bind(null, f.onload), l && document.head.appendChild(f)
+            d.onerror = c.bind(null, d.onerror), d.onload = c.bind(null, d.onload), f && document.head.appendChild(d)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, x.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         x.S = {};
         var e = {},
             r = {};
-        x.I = (a, t) => {
-            t || (t = []);
-            var o = r[a];
-            if (o || (o = r[a] = {}), !(t.indexOf(o) >= 0)) {
-                if (t.push(o), e[a]) return e[a];
-                x.o(x.S, a) || (x.S[a] = {});
-                var n = x.S[a],
-                    f = "@jupytercad/jupytercad-core",
-                    l = (e, r, a, t) => {
+        x.I = (t, a) => {
+            a || (a = []);
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
+                if (a.push(o), e[t]) return e[t];
+                x.o(x.S, t) || (x.S[t] = {});
+                var n = x.S[t],
+                    d = "@jupytercad/jupytercad-core",
+                    f = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!t != !l.eager ? t : f > l.from)) && (o[r] = {
-                            get: a,
-                            from: f,
-                            eager: !!t
+                            f = o[r];
+                        (!f || !f.loaded && (!a != !f.eager ? a : d > f.from)) && (o[r] = {
+                            get: t,
+                            from: d,
+                            eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === a && (l("@jupytercad/base", "2.0.0-alpha.5", (() => Promise.all([x.e(279), x.e(702), x.e(602), x.e(37), x.e(32), x.e(644)]).then((() => () => x(2070))))), l("@jupytercad/jupytercad-core", "2.0.0-alpha.5", (() => Promise.all([x.e(262), x.e(602), x.e(37), x.e(644), x.e(813)]).then((() => () => x(2813))))), l("@jupytercad/occ-worker", "2.0.0-alpha.5", (() => Promise.all([x.e(262), x.e(37), x.e(794)]).then((() => () => x(9794))))), l("@jupytercad/schema", "2.0.0-alpha.5", (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341)))))), e[a] = u.length ? Promise.all(u).then((() => e[a] = 1)) : 1
+                    l = [];
+                return "default" === t && (f("@jupytercad/base", "2.0.0-alpha.6", (() => Promise.all([x.e(279), x.e(702), x.e(602), x.e(342), x.e(32), x.e(644)]).then((() => () => x(2070))))), f("@jupytercad/jupytercad-core", "2.0.0-alpha.6", (() => Promise.all([x.e(262), x.e(602), x.e(342), x.e(644), x.e(813)]).then((() => () => x(2813))))), f("@jupytercad/occ-worker", "2.0.0-alpha.6", (() => Promise.all([x.e(262), x.e(342), x.e(794)]).then((() => () => x(9794))))), f("@jupytercad/schema", "2.0.0-alpha.6", (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
-            var a = r.getElementsByTagName("script");
-            if (a.length)
-                for (var t = a.length - 1; t > -1 && (!e || !/^http(s?):/.test(e));) e = a[t--].src
+            var t = r.getElementsByTagName("script");
+            if (t.length)
+                for (var a = t.length - 1; a > -1 && (!e || !/^http(s?):/.test(e));) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), x.p = e
-    })(), a = e => {
+    })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
-            a = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            t = a[1] ? r(a[1]) : [];
-        return a[2] && (t.length++, t.push.apply(t, r(a[2]))), a[3] && (t.push([]), t.push.apply(t, r(a[3]))), t
-    }, t = (e, r) => {
-        e = a(e), r = a(r);
-        for (var t = 0;;) {
-            if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
-            var o = e[t],
+            t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
+        e = t(e), r = t(r);
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var o = e[a],
                 n = (typeof o)[0];
-            if (t >= r.length) return "u" == n;
-            var f = r[t],
-                l = (typeof f)[0];
-            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
-            if ("o" != n && "u" != n && o != f) return o < f;
-            t++
+            if (a >= r.length) return "u" == n;
+            var d = r[a],
+                f = (typeof d)[0];
+            if (n != f) return "o" == n && "n" == f || "s" == f || "u" == n;
+            if ("o" != n && "u" != n && o != d) return o < d;
+            a++
         }
     }, o = e => {
         var r = e[0],
-            a = "";
+            t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
-            a += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var t = 1, n = 1; n < e.length; n++) t--, a += "u" == (typeof(l = e[n]))[0] ? "-" : (t > 0 ? "." : "") + (t = 2, l);
-            return a
+            t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
+            for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(f = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, f);
+            return t
         }
-        var f = [];
+        var d = [];
         for (n = 1; n < e.length; n++) {
-            var l = e[n];
-            f.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? f.pop() + " " + f.pop() : o(l))
+            var f = e[n];
+            d.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? d.pop() + " " + d.pop() : o(f))
         }
-        return u();
+        return l();
 
-        function u() {
-            return f.pop().replace(/^\((.+)\)$/, "$1")
+        function l() {
+            return d.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
-            r = a(r);
-            var t = e[0],
-                o = t < 0;
-            o && (t = -t - 1);
-            for (var f = 0, l = 1, u = !0;; l++, f++) {
-                var c, i, d = l < e.length ? (typeof e[l])[0] : "";
-                if (f >= r.length || "o" == (i = (typeof(c = r[f]))[0])) return !u || ("u" == d ? l > t && !o : "" == d != o);
+            r = t(r);
+            var a = e[0],
+                o = a < 0;
+            o && (a = -a - 1);
+            for (var d = 0, f = 1, l = !0;; f++, d++) {
+                var u, i, c = f < e.length ? (typeof e[f])[0] : "";
+                if (d >= r.length || "o" == (i = (typeof(u = r[d]))[0])) return !l || ("u" == c ? f > a && !o : "" == c != o);
                 if ("u" == i) {
-                    if (!u || "u" != d) return !1
-                } else if (u)
-                    if (d == i)
-                        if (l <= t) {
-                            if (c != e[l]) return !1
+                    if (!l || "u" != c) return !1
+                } else if (l)
+                    if (c == i)
+                        if (f <= a) {
+                            if (u != e[f]) return !1
                         } else {
-                            if (o ? c > e[l] : c < e[l]) return !1;
-                            c != e[l] && (u = !1)
+                            if (o ? u > e[f] : u < e[f]) return !1;
+                            u != e[f] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
-                    if (o || l <= t) return !1;
-                    u = !1, l--
+                else if ("s" != c && "n" != c) {
+                    if (o || f <= a) return !1;
+                    l = !1, f--
                 } else {
-                    if (l <= t || i < d != o) return !1;
-                    u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                    if (f <= a || i < c != o) return !1;
+                    l = !1
+                } else "s" != c && "n" != c && (l = !1, f--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
-        for (f = 1; f < e.length; f++) {
-            var b = e[f];
+        for (d = 1; d < e.length; d++) {
+            var b = e[d];
             s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? n(b, r) : !p())
         }
         return !!p()
+    }, d = (e, r) => {
+        var t = x.S[e];
+        if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        return t
     }, f = (e, r) => {
-        var a = x.S[e];
-        if (!a || !x.o(a, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
-        return a
+        var t = e[r];
+        return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !e || t(e, r) ? r : e), 0)) && a[r]
-    }, u = (e, r) => {
-        var a = e[r];
-        return Object.keys(a).reduce(((e, r) => !e || !a[e].loaded && t(e, r) ? r : e), 0)
-    }, c = (e, r, a, t) => "Unsatisfied version " + a + " from " + (a && e[r][a].from) + " of shared singleton module " + r + " (required " + o(t) + ")", i = (e, r, a, t) => {
-        var o = u(e, a);
-        return n(t, o) || p(c(e, a, o, t)), h(e[a][o])
-    }, d = (e, r, a) => {
+        var t = e[r];
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", i = (e, r, t, a) => {
+        var o = l(e, t);
+        return n(a, o) || p(u(e, t, o, a)), h(e[t][o])
+    }, c = (e, r, t) => {
         var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !n(a, r) || e && !t(e, r) ? e : r), 0)) && o[r]
-    }, s = (e, r, a, t) => {
-        var n = e[a];
-        return "No satisfying version (" + o(t) + ") of shared module " + a + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(n).map((e => e + " from " + n[e].from)).join(", ")
+        return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
+    }, s = (e, r, t, a) => {
+        var n = e[t];
+        return "No satisfying version (" + o(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(n).map((e => e + " from " + n[e].from)).join(", ")
     }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, b = (e, r, a, t) => {
-        p(s(e, r, a, t))
-    }, h = e => (e.loaded = 1, e.get()), m = (v = e => function(r, a, t, o) {
+    }, b = (e, r, t, a) => {
+        p(s(e, r, t, a))
+    }, h = e => (e.loaded = 1, e.get()), m = (v = e => function(r, t, a, o) {
         var n = x.I(r);
-        return n && n.then ? n.then(e.bind(e, r, x.S[r], a, t, o)) : e(r, x.S[r], a, t, o)
-    })(((e, r, a, t) => (f(e, a), h(d(r, a, t) || b(r, e, a, t) || l(r, a))))), y = v(((e, r, a, t) => (f(e, a), i(r, 0, a, t)))), g = v(((e, r, a, t, o) => r && x.o(r, a) ? i(r, 0, a, t) : o())), j = v(((e, r, a, t, o) => {
-        var n = r && x.o(r, a) && d(r, a, t);
+        return n && n.then ? n.then(e.bind(e, r, x.S[r], t, a, o)) : e(r, x.S[r], t, a, o)
+    })(((e, r, t, a) => (d(e, t), h(c(r, t, a) || b(r, e, t, a) || f(r, t))))), y = v(((e, r, t, a) => (d(e, t), i(r, 0, t, a)))), g = v(((e, r, t, a, o) => r && x.o(r, t) ? i(r, 0, t, a) : o())), j = v(((e, r, t, a, o) => {
+        var n = r && x.o(r, t) && c(r, t, a);
         return n ? h(n) : o()
     })), w = {}, P = {
         7262: () => y("default", "@lumino/coreutils", [1, 2, 0, 0]),
         4602: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
-        3037: () => g("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 5], (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341))))),
+        3342: () => g("default", "@jupytercad/schema", [1, 2, 0, 0, , "alpha", 6], (() => Promise.all([x.e(279), x.e(601), x.e(262), x.e(602), x.e(341)]).then((() => () => x(2341))))),
         7638: () => y("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
         7664: () => y("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
         7714: () => y("default", "@jupyterlab/translation", [1, 4, 1, 6]),
         8859: () => m("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
-        597: () => g("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 5], (() => Promise.all([x.e(279), x.e(702), x.e(32)]).then((() => () => x(2070))))),
+        492: () => j("default", "@jupytercad/occ-worker", [1, 2, 0, 0, , "alpha", 6], (() => x.e(413).then((() => () => x(9794))))),
         1381: () => y("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
         1595: () => y("default", "@jupyterlab/launcher", [1, 4, 1, 6]),
-        3503: () => j("default", "@jupytercad/occ-worker", [1, 2, 0, 0, , "alpha", 5], (() => x.e(413).then((() => () => x(9794))))),
         4796: () => y("default", "@jupyter/docprovider", [1, 2, 0, 0]),
+        8626: () => g("default", "@jupytercad/base", [1, 2, 0, 0, , "alpha", 6], (() => Promise.all([x.e(279), x.e(702), x.e(32)]).then((() => () => x(2070))))),
         9221: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
         2486: () => y("default", "@jupyterlab/services", [1, 7, 1, 6]),
         3345: () => y("default", "react", [1, 18, 2, 0]),
         4053: () => y("default", "@lumino/algorithm", [1, 2, 0, 0]),
         5256: () => y("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         6167: () => y("default", "@lumino/commands", [1, 2, 0, 1]),
         6230: () => y("default", "@lumino/messaging", [1, 2, 0, 0]),
         6597: () => y("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
         6901: () => y("default", "@jupyterlab/codemirror", [1, 4, 1, 6]),
         8265: () => m("default", "@jupyterlab/observables", [1, 5, 1, 6]),
         667: () => y("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         2206: () => y("default", "yjs", [1, 13, 5, 40])
     }, S = {
         32: [2486, 3345, 4053, 5256, 6167, 6230, 6597, 6901, 8265],
-        37: [3037],
         262: [7262],
         341: [667, 2206],
+        342: [3342],
         602: [4602],
         644: [7638, 7664, 7714, 8859],
-        813: [597, 1381, 1595, 3503, 4796, 9221]
+        813: [492, 1381, 1595, 4796, 8626, 9221]
     }, k = {}, x.f.consumes = (e, r) => {
         x.o(S, e) && S[e].forEach((e => {
             if (x.o(w, e)) return r.push(w[e]);
             if (!k[e]) {
-                var a = r => {
-                    w[e] = 0, x.m[e] = a => {
-                        delete x.c[e], a.exports = r()
+                var t = r => {
+                    w[e] = 0, x.m[e] = t => {
+                        delete x.c[e], t.exports = r()
                     }
                 };
                 k[e] = !0;
-                var t = r => {
-                    delete w[e], x.m[e] = a => {
+                var a = r => {
+                    delete w[e], x.m[e] = t => {
                         throw delete x.c[e], r
                     }
                 };
                 try {
                     var o = P[e]();
-                    o.then ? r.push(w[e] = o.then(a).catch(t)) : a(o)
+                    o.then ? r.push(w[e] = o.then(t).catch(a)) : t(o)
                 } catch (e) {
-                    t(e)
+                    a(e)
                 }
             }
         }))
     }, (() => {
         x.b = document.baseURI || self.location.href;
         var e = {
             490: 0
         };
-        x.f.j = (r, a) => {
-            var t = x.o(e, r) ? e[r] : void 0;
-            if (0 !== t)
-                if (t) a.push(t[2]);
-                else if (/^(262|37|602|644)$/.test(r)) e[r] = 0;
+        x.f.j = (r, t) => {
+            var a = x.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
+                else if (/^((26|34|60)2|644)$/.test(r)) e[r] = 0;
             else {
-                var o = new Promise(((a, o) => t = e[r] = [a, o]));
-                a.push(t[2] = o);
+                var o = new Promise(((t, o) => a = e[r] = [t, o]));
+                t.push(a[2] = o);
                 var n = x.p + x.u(r),
-                    f = new Error;
-                x.l(n, (a => {
-                    if (x.o(e, r) && (0 !== (t = e[r]) && (e[r] = void 0), t)) {
-                        var o = a && ("load" === a.type ? "missing" : a.type),
-                            n = a && a.target && a.target.src;
-                        f.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", f.name = "ChunkLoadError", f.type = o, f.request = n, t[1](f)
+                    d = new Error;
+                x.l(n, (t => {
+                    if (x.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                        var o = t && ("load" === t.type ? "missing" : t.type),
+                            n = t && t.target && t.target.src;
+                        d.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", d.name = "ChunkLoadError", d.type = o, d.request = n, a[1](d)
                     }
                 }), "chunk-" + r, r)
             }
         };
-        var r = (r, a) => {
-                var t, o, [n, f, l] = a,
-                    u = 0;
+        var r = (r, t) => {
+                var a, o, [n, d, f] = t,
+                    l = 0;
                 if (n.some((r => 0 !== e[r]))) {
-                    for (t in f) x.o(f, t) && (x.m[t] = f[t]);
-                    l && l(x)
+                    for (a in d) x.o(d, a) && (x.m[a] = d[a]);
+                    f && f(x)
                 }
-                for (r && r(a); u < n.length; u++) o = n[u], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < n.length; l++) o = n[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
-            a = self.webpackChunk_jupytercad_jupytercad_core = self.webpackChunk_jupytercad_jupytercad_core || [];
-        a.forEach(r.bind(null, 0)), a.push = r.bind(null, a.push.bind(a))
+            t = self.webpackChunk_jupytercad_jupytercad_core = self.webpackChunk_jupytercad_jupytercad_core || [];
+        t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), x.nc = void 0;
     var T = x(2401);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupytercad/jupytercad-core"] = T
 })();
```

### Comparing `jupytercad_core-2.0.0a5/jupytercad_core/labextension/static/third-party-licenses.json` & `jupytercad_core-2.0.0a6/jupytercad_core/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959239130434783%*

 * *Differences: {"'packages'": "{5: {'versionInfo': '2.0.0-alpha.6'}, 6: {'versionInfo': '2.0.0-alpha.6'}, 7: "*

 * *               "{'versionInfo': '2.0.0-alpha.6'}}"}*

```diff
@@ -30,27 +30,27 @@
             "name": "@emotion/unitless",
             "versionInfo": "0.7.5"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupytercad/base",
-            "versionInfo": "2.0.0-alpha.5"
+            "versionInfo": "2.0.0-alpha.6"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupytercad/occ-worker",
-            "versionInfo": "2.0.0-alpha.5"
+            "versionInfo": "2.0.0-alpha.6"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupytercad/schema",
-            "versionInfo": "2.0.0-alpha.5"
+            "versionInfo": "2.0.0-alpha.6"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyterlab/rendermime",
             "versionInfo": "3.6.7"
         },
```

### Comparing `jupytercad_core-2.0.0a5/lib/factory.d.ts` & `jupytercad_core-2.0.0a6/lib/factory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/factory.js` & `jupytercad_core-2.0.0a6/lib/factory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/index.d.ts` & `jupytercad_core-2.0.0a6/lib/index.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/index.js` & `jupytercad_core-2.0.0a6/lib/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/plugin.d.ts` & `jupytercad_core-2.0.0a6/lib/plugin.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/plugin.js` & `jupytercad_core-2.0.0a6/lib/plugin.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/schemaregistry.js` & `jupytercad_core-2.0.0a6/lib/schemaregistry.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/workerregistry.js` & `jupytercad_core-2.0.0a6/lib/workerregistry.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/jcadplugin/modelfactory.d.ts` & `jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/jcadplugin/modelfactory.js` & `jupytercad_core-2.0.0a6/lib/jcadplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/jcadplugin/plugins.js` & `jupytercad_core-2.0.0a6/lib/jcadplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stepplugin/model.d.ts` & `jupytercad_core-2.0.0a6/lib/stepplugin/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stepplugin/model.js` & `jupytercad_core-2.0.0a6/lib/stepplugin/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stepplugin/modelfactory.d.ts` & `jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stepplugin/modelfactory.js` & `jupytercad_core-2.0.0a6/lib/stepplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stepplugin/plugins.js` & `jupytercad_core-2.0.0a6/lib/stepplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stlplugin/model.js` & `jupytercad_core-2.0.0a6/lib/stlplugin/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stlplugin/modelfactory.d.ts` & `jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stlplugin/modelfactory.js` & `jupytercad_core-2.0.0a6/lib/stlplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/lib/stlplugin/plugins.js` & `jupytercad_core-2.0.0a6/lib/stlplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/factory.ts` & `jupytercad_core-2.0.0a6/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/index.ts` & `jupytercad_core-2.0.0a6/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/plugin.ts` & `jupytercad_core-2.0.0a6/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/schemaregistry.ts` & `jupytercad_core-2.0.0a6/src/schemaregistry.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/workerregistry.ts` & `jupytercad_core-2.0.0a6/src/workerregistry.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/jcadplugin/modelfactory.ts` & `jupytercad_core-2.0.0a6/src/jcadplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/jcadplugin/plugins.ts` & `jupytercad_core-2.0.0a6/src/jcadplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/stepplugin/model.ts` & `jupytercad_core-2.0.0a6/src/stepplugin/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/stepplugin/modelfactory.ts` & `jupytercad_core-2.0.0a6/src/stepplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/stepplugin/plugins.ts` & `jupytercad_core-2.0.0a6/src/stepplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/stlplugin/model.ts` & `jupytercad_core-2.0.0a6/src/stlplugin/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/stlplugin/modelfactory.ts` & `jupytercad_core-2.0.0a6/src/stlplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/src/stlplugin/plugins.ts` & `jupytercad_core-2.0.0a6/src/stlplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/LICENSE` & `jupytercad_core-2.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/pyproject.toml` & `jupytercad_core-2.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupytercad_core-2.0.0a5/PKG-INFO` & `jupytercad_core-2.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupytercad_core
-Version: 2.0.0a5
+Version: 2.0.0a6
 Dynamic: Keywords
 Summary: JupyterCad core extension
 Project-URL: Homepage, https://github.com/jupytercad/jupytercad
 Project-URL: Bug Tracker, https://github.com/jupytercad/jupytercad/issues
 Project-URL: Repository, https://github.com/jupytercad/jupytercad.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
```

