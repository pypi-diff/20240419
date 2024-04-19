# Comparing `tmp/trame_jupyter_extension-2.0.1.tar.gz` & `tmp/trame_jupyter_extension-2.1.0.tar.gz`

## Comparing `trame_jupyter_extension-2.0.1.tar` & `trame_jupyter_extension-2.1.0.tar`

### file list

```diff
@@ -1,42 +1,37 @@
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/.yarnrc.yml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/RELEASE.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/Untitled.ipynb
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/install.json
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/tsconfig.json
--rw-r--r--   0        0        0   235339 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/yarn.lock
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/examples/interrupt.ipynb
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/examples/requirements.txt
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/examples/test_trame_jupyter_comm.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/examples/untitled.txt
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/examples/vtk_remote_rendering.ipynb
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/examples/vue23.ipynb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/jupyter-config/server-config/trame_jupyter_extension.json
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/src/comm.ts
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/src/emitter.ts
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/src/index.ts
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/src/location.ts
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/src/manager.ts
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/src/registry.ts
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/src/websocket.ts
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/style/index.js
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/_version.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/handlers.py
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/labextension/package.json
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/labextension/static/747.e583e84008dcaf0209af.js
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/labextension/static/899.56ef666a9e3129c5301c.js
--rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/labextension/static/remoteEntry.eb1438c6091204ef3c24.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/trame_jupyter_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/LICENSE
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/README.md
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.yarnrc.yml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/RELEASE.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/install.json
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/tsconfig.json
+-rw-r--r--   0        0        0   227220 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/yarn.lock
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/interrupt.ipynb
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/requirements.txt
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/simple-test.ipynb
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/test_trame_jupyter_comm.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/untitled.txt
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/vtk_remote_rendering.ipynb
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/examples/vue23.ipynb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/jupyter-config/server-config/trame_jupyter_extension.json
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/comm.ts
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/emitter.ts
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/index.ts
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/location.ts
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/manager.ts
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/registry.ts
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/utils.ts
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/src/websocket.ts
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/style/index.js
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/trame_jupyter_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/trame_jupyter_extension/_version.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/trame_jupyter_extension/handlers.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/README.md
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 trame_jupyter_extension-2.1.0/PKG-INFO
```

### Comparing `trame_jupyter_extension-2.0.1/.copier-answers.yml` & `trame_jupyter_extension-2.1.0/.copier-answers.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 has_binder: false
 has_settings: false
 kind: server
 labextension_name: trame-jupyter-extension
 mimetype: ''
 mimetype_name: ''
 project_short_description: A JupyterLab extension for trame communication layer
-python_name: trame_jupyter_extension
+python_name: trame-jupyter-extension
 repository: https://github.com/Kitware/trame-jupyter-extension
 test: false
 viewer_name: ''
```

### Comparing `trame_jupyter_extension-2.0.1/RELEASE.md` & `trame_jupyter_extension-2.1.0/RELEASE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Making a new release of trame_jupyter_extension
+# Making a new release of trame-jupyter-extension
 
 The extension can be published to `PyPI` and `npm` manually or using the [Jupyter Releaser](https://github.com/jupyter-server/jupyter_releaser).
 
 ## Manual release
 
 ### Python package
```

### Comparing `trame_jupyter_extension-2.0.1/Untitled.ipynb` & `trame_jupyter_extension-2.1.0/examples/simple-test.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9358465608465609%*

 * *Differences: {"'cells'": "{0: {'id': '9e4d04e3-eeec-40a5-b3a6-0780a59cf99e', 'outputs': [OrderedDict([('name', "*

 * *            "'stdout'), ('output_type', 'stream'), ('text', "*

 * *            "['http://localhost:8888/trame-jupyter-server/servers/trame/index.html?ui=main&server=trame&wsProxy&reconnect=auto\\n'])]), "*

 * *            "OrderedDict([('data', OrderedDict([('text/html', ['<iframe "*

 * *            'id="trame_trame__template_main" '*

 * *            'src="http://localhost:8888/trame-jupyter-server/servers/trame/index.html?ui=ma […]*

```diff
@@ -1,67 +1,50 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "1a773f42-aafe-4773-82ff-866e7ed9874b",
+            "id": "9e4d04e3-eeec-40a5-b3a6-0780a59cf99e",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "http://localhost:8888/trame-jupyter-server/servers/trame/index.html?ui=main&server=trame&wsProxy&reconnect=auto\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<iframe id=\"trame_trame__template_main\" src=\"http://localhost:8888/trame-jupyter-server/servers/trame/index.html?ui=main&server=trame&wsProxy&reconnect=auto\" style=\"height: 200px; width: 100%; border: none;\" data-kernel-id=\"5dbccb26-b949-4493-8dee-d619dda4b05f\"></iframe>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
             "source": [
-                "import os\n",
+                "from trame.app.demo import Cone\n",
+                "cone = Cone()\n",
+                "await cone.ui.ready\n",
+                "cone.ui.iframe_style = \"height: 200px; width: 100%; border: none;\"\n",
                 "\n",
-                "def console_print(*args, sep=' ', end='\\n'):\n",
-                "    full_str = sep.join(str(arg) for arg in args) + end\n",
+                "print(cone.ui._jupyter_content().split('src=\"').pop().split('\"')[0])\n",
                 "\n",
-                "    os.write(1, full_str.encode())\n"
+                "cone.ui"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "id": "9802bdc9-fb43-4582-834c-f113401d3ffc",
+            "execution_count": null,
+            "id": "0ad6f9b2-dc6d-44b7-be88-b5c3ec9785ce",
             "metadata": {},
             "outputs": [],
-            "source": [
-                "kernel = get_ipython().kernel\n",
-                "\n",
-                "comm = None\n",
-                "\n",
-                "def on_message(*args, **kwargs):\n",
-                "    console_print(\"COMM MESSAGE\", args, kwargs)\n",
-                "\n",
-                "def on_close(*args, **kwargs):\n",
-                "    console_print(\"COMM CLOSED\", args, kwargs)\n",
-                "\n",
-                "    global comm\n",
-                "    comm = None\n",
-                "\n",
-                "def on_open(_comm, msg):\n",
-                "    console_print(\"COMM OPENED\", msg)\n",
-                "\n",
-                "    global comm\n",
-                "    comm = _comm\n",
-                "\n",
-                "    comm.on_msg(on_message)\n",
-                "\n",
-                "    comm.on_close(on_close)\n",
-                "\n",
-                "kernel.comm_manager.register_target('test', on_open)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "id": "ce165612-b333-4196-a19e-6d2a4beb99bf",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "if comm is not None:\n",
-                "    comm.send(\"from server to client\")"
-            ]
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -72,13 +55,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `trame_jupyter_extension-2.0.1/package.json` & `trame_jupyter_extension-2.1.0/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9719202898550724%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^4.1.6', '@types/json-schema': '^7.0.15', "*

 * *                      "'@types/react': '^18.2.79', '@types/react-addons-linked-state-mixin': "*

 * *                      "'^0.14.27', '@typescript-eslint/eslint-plugin': '^6.21.0', "*

 * *                      "'@typescript-eslint/parser': '^6.21.0', 'css-loader': '^6.11.0', 'eslint': "*

 * *                      "'^8.57.0', 'eslint-plugin-prettier': '^5.1.3', 'prettier': '^3.2.5', "*

 * *                      "'rimraf': '^5.0.5', 'sty […]*

```diff
@@ -10,37 +10,37 @@
         "@jupyterlab/application": "^3.5.0 || ^4.0.5",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/notebook": "^4.0.7",
         "@jupyterlab/services": "^7.0.0"
     },
     "description": "A JupyterLab extension for trame communication layer",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0",
-        "@types/json-schema": "^7.0.11",
-        "@types/react": "^18.0.26",
-        "@types/react-addons-linked-state-mixin": "^0.14.22",
-        "@typescript-eslint/eslint-plugin": "^6.1.0",
-        "@typescript-eslint/parser": "^6.1.0",
-        "css-loader": "^6.7.1",
-        "eslint": "^8.36.0",
+        "@jupyterlab/builder": "^4.1.6",
+        "@types/json-schema": "^7.0.15",
+        "@types/react": "^18.2.79",
+        "@types/react-addons-linked-state-mixin": "^0.14.27",
+        "@typescript-eslint/eslint-plugin": "^6.21.0",
+        "@typescript-eslint/parser": "^6.21.0",
+        "css-loader": "^6.11.0",
+        "eslint": "^8.57.0",
         "eslint-config-prettier": "^8.8.0",
-        "eslint-plugin-prettier": "^5.0.0",
+        "eslint-plugin-prettier": "^5.1.3",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^3.0.0",
-        "rimraf": "^5.0.1",
+        "prettier": "^3.2.5",
+        "rimraf": "^5.0.5",
         "source-map-loader": "^1.0.2",
-        "style-loader": "^3.3.1",
-        "stylelint": "^15.10.1",
+        "style-loader": "^3.3.4",
+        "stylelint": "^15.11.0",
         "stylelint-config-recommended": "^13.0.0",
         "stylelint-config-standard": "^34.0.0",
         "stylelint-csstree-validator": "^3.0.0",
-        "stylelint-prettier": "^4.0.0",
-        "typescript": "~5.0.2",
-        "yjs": "^13.5.0"
+        "stylelint-prettier": "^4.1.0",
+        "typescript": "~5.4.5",
+        "yjs": "^13.6.14"
     },
     "eslintConfig": {
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
             "plugin:prettier/recommended"
@@ -191,9 +191,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.0.1"
+    "version": "2.1.0"
 }
```

### Comparing `trame_jupyter_extension-2.0.1/tsconfig.json` & `trame_jupyter_extension-2.1.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/yarn.lock` & `trame_jupyter_extension-2.1.0/yarn.lock`

 * *Files 4% similar despite different names*

```diff
@@ -9,67 +9,68 @@
   version: 1.2.6
   resolution: "@aashutoshrathi/word-wrap@npm:1.2.6"
   checksum: ada901b9e7c680d190f1d012c84217ce0063d8f5c5a7725bb91ec3c5ed99bb7572680eb2d2938a531ccbaec39a95422fcd8a6b4a13110c7d98dd75402f66a0cd
   languageName: node
   linkType: hard
 
 "@babel/code-frame@npm:^7.0.0":
-  version: 7.22.13
-  resolution: "@babel/code-frame@npm:7.22.13"
+  version: 7.24.2
+  resolution: "@babel/code-frame@npm:7.24.2"
   dependencies:
-    "@babel/highlight": ^7.22.13
-    chalk: ^2.4.2
-  checksum: 22e342c8077c8b77eeb11f554ecca2ba14153f707b85294fcf6070b6f6150aae88a7b7436dd88d8c9289970585f3fe5b9b941c5aa3aa26a6d5a8ef3f292da058
+    "@babel/highlight": ^7.24.2
+    picocolors: ^1.0.0
+  checksum: 70e867340cfe09ca5488b2f36372c45cabf43c79a5b6426e6df5ef0611ff5dfa75a57dda841895693de6008f32c21a7c97027a8c7bcabd63a7d17416cbead6f8
   languageName: node
   linkType: hard
 
 "@babel/helper-validator-identifier@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-validator-identifier@npm:7.22.20"
   checksum: 136412784d9428266bcdd4d91c32bcf9ff0e8d25534a9d94b044f77fe76bc50f941a90319b05aafd1ec04f7d127cd57a179a3716009ff7f3412ef835ada95bdc
   languageName: node
   linkType: hard
 
-"@babel/highlight@npm:^7.22.13":
-  version: 7.22.20
-  resolution: "@babel/highlight@npm:7.22.20"
+"@babel/highlight@npm:^7.24.2":
+  version: 7.24.2
+  resolution: "@babel/highlight@npm:7.24.2"
   dependencies:
     "@babel/helper-validator-identifier": ^7.22.20
     chalk: ^2.4.2
     js-tokens: ^4.0.0
-  checksum: 84bd034dca309a5e680083cd827a766780ca63cef37308404f17653d32366ea76262bd2364b2d38776232f2d01b649f26721417d507e8b4b6da3e4e739f6d134
+    picocolors: ^1.0.0
+  checksum: 5f17b131cc3ebf3ab285a62cf98a404aef1bd71a6be045e748f8d5bf66d6a6e1aefd62f5972c84369472e8d9f22a614c58a89cd331eb60b7ba965b31b1bbeaf5
   languageName: node
   linkType: hard
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
-  version: 6.10.2
-  resolution: "@codemirror/autocomplete@npm:6.10.2"
+  version: 6.16.0
+  resolution: "@codemirror/autocomplete@npm:6.16.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 360cea6a87ae9c4e3c996903f636a8f47f8ea6cd44504181e69dd8ccf666bad3e8cc6d8935e0eedd8aa118fdfe86ea78f41bc15288f3a7517dbb87115e057563
+  checksum: e33d3d8c961c03dc4a70d1ac6f01aee5362d778da9d873a8335aed47f7de9430eab083589736e7922464b941d5da23c51ab6af05400413a8d1a07604ffcb99f7
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
-  version: 6.3.0
-  resolution: "@codemirror/commands@npm:6.3.0"
+  version: 6.4.0
+  resolution: "@codemirror/commands@npm:6.4.0"
   dependencies:
     "@codemirror/language": ^6.0.0
-    "@codemirror/state": ^6.2.0
+    "@codemirror/state": ^6.4.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.1.0
-  checksum: d6ade0ba7d4f80c2e44163935783d2f2f35c8b641a4b4f62452c0630211670abe5093786cf5a4af14147102d4284dae660a26f3ae58fd840e838685a81107d11
+  checksum: 92fb4ffe75e177186ce0801fdd1d1dacfd9a005122f8d032211e8d86fd9e81d4dd0440fa2bcf866df720be259dc7c91e7912884d44f5eb7fa8dce683ec820563
   languageName: node
   linkType: hard
 
 "@codemirror/lang-cpp@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-cpp@npm:6.0.2"
   dependencies:
@@ -89,77 +90,77 @@
     "@lezer/common": ^1.0.2
     "@lezer/css": ^1.0.0
   checksum: 5a8457ee8a4310030a969f2d3128429f549c4dc9b7907ee8888b42119c80b65af99093801432efdf659b8ec36a147d2a947bc1ecbbf69a759395214e3f4834a8
   languageName: node
   linkType: hard
 
 "@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.3":
-  version: 6.4.6
-  resolution: "@codemirror/lang-html@npm:6.4.6"
+  version: 6.4.9
+  resolution: "@codemirror/lang-html@npm:6.4.9"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/lang-css": ^6.0.0
     "@codemirror/lang-javascript": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/css": ^1.1.0
     "@lezer/html": ^1.3.0
-  checksum: 8f884f4423ffc783181ee933f7212ad4ece204695cf8af9535a593f95e901d36515a8561fc336a0fbcf5782369b9484eeb0d2cec2167622868238177c5e6eb36
+  checksum: ac8c3ceb0396f2e032752c5079bd950124dca708bc64e96fc147dc5fe7133e5cee0814fe951abdb953ec1d11fa540e4b30a712b5149d9a36016a197a28de45d7
   languageName: node
   linkType: hard
 
 "@codemirror/lang-java@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-java@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/java": ^1.0.0
   checksum: 4679104683cbffcd224ac04c7e5d144b787494697b26470b07017259035b7bb3fa62609d9a61bfbc566f1756d9f972f9f26d96a3c1362dd48881c1172f9a914d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
-  version: 6.2.1
-  resolution: "@codemirror/lang-javascript@npm:6.2.1"
+  version: 6.2.2
+  resolution: "@codemirror/lang-javascript@npm:6.2.2"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/javascript": ^1.0.0
-  checksum: 3df38c4cced06195283a9a2a9365aaa7c8c1b157852b331bc3a118403f774bbba57d2a392de52f5e28d2b344a323bc0146bcf7c8ef8be2473f167d815e4a37cd
+  checksum: 66379942a8347dff2bd76d10ed7cf313bca83872f8336fdd3e14accfef23e7b690cd913c9d11a3854fba2b32299da07fc3275995327642c9ee43c2a8e538c19d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-json@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-json@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/json": ^1.0.0
   checksum: e9e87d50ff7b81bd56a6ab50740b1dd54e9a93f1be585e1d59d0642e2148842ea1528ac7b7221eb4ddc7fe84bbc28065144cc3ab86f6e06c6aeb2d4b4e62acf1
   languageName: node
   linkType: hard
 
 "@codemirror/lang-markdown@npm:^6.1.1":
-  version: 6.2.2
-  resolution: "@codemirror/lang-markdown@npm:6.2.2"
+  version: 6.2.5
+  resolution: "@codemirror/lang-markdown@npm:6.2.5"
   dependencies:
     "@codemirror/autocomplete": ^6.7.1
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.3.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
-    "@lezer/common": ^1.0.0
+    "@lezer/common": ^1.2.1
     "@lezer/markdown": ^1.0.0
-  checksum: 36aa82a4fc07e5761e0e04108b54f112f0049ed210b3d4e81b7429a99be4677a1f9ef0e004c5243265dca3bac36525792cb1558999f6a224c689475e958d4aa8
+  checksum: 3d9e0817f888eddcb6d05ec8f0d8dacbde7b9ef7650303bc4ab8b08a550a986c60c65b1565212e06af389c31590330f1f5ed65e619a9446dc2979ff3dac0e874
   languageName: node
   linkType: hard
 
 "@codemirror/lang-php@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-php@npm:6.0.1"
   dependencies:
@@ -169,173 +170,171 @@
     "@lezer/common": ^1.0.0
     "@lezer/php": ^1.0.0
   checksum: c003a29a426486453fdfddbf7302982fa2aa7f059bf6f1ce4cbf08341b0162eee5e2f50e0d71c418dcd358491631780156d846fe352754d042576172c5d86721
   languageName: node
   linkType: hard
 
 "@codemirror/lang-python@npm:^6.1.3":
-  version: 6.1.3
-  resolution: "@codemirror/lang-python@npm:6.1.3"
+  version: 6.1.5
+  resolution: "@codemirror/lang-python@npm:6.1.5"
   dependencies:
     "@codemirror/autocomplete": ^6.3.2
     "@codemirror/language": ^6.8.0
+    "@codemirror/state": ^6.0.0
+    "@lezer/common": ^1.2.1
     "@lezer/python": ^1.1.4
-  checksum: 65a0276a4503e4e3b70dd28d1c93ef472632b6d2c4bf3ae92d305d14ee8cf60b0bbbf62d5ceb51294de9598d9e2d42eafcde26f317ee7b90d0a11dfa863c1d1a
+  checksum: 85934c9df78013e365c9a45bdd230de3d8a0e265f4d917440addb17a8ff60521b2cf67b86ad58c136a615a286ed091e5ce78b318cd934381c03fe84bfd2b9186
   languageName: node
   linkType: hard
 
 "@codemirror/lang-rust@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-rust@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
 "@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.5.4
-  resolution: "@codemirror/lang-sql@npm:6.5.4"
+  version: 6.6.3
+  resolution: "@codemirror/lang-sql@npm:6.6.3"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: face21b0231ac5a7981949b5bf6a99ed092d0d6f7eb83f35dcd31d56ecf07dafa19d21623e0bad36cec7a12e3149df7b45c3588aeee31eae41e9b05942c4fdd7
+  checksum: b8e554bda9107107283674a6397cdb4816ad8bb429afd739fdc5e0339ef60170f09bdd93e7dc3eaf7f24ffaec5c7477ee42af7c05cb471990657014fac2fea1e
   languageName: node
   linkType: hard
 
 "@codemirror/lang-wast@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "@codemirror/lang-wast@npm:6.0.1"
+  version: 6.0.2
+  resolution: "@codemirror/lang-wast@npm:6.0.2"
   dependencies:
     "@codemirror/language": ^6.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 600d98d3ea6a4e99292244ed707e39a2abd9f3abf62cfeff5c819a0cc0c7e86b8c5b91e91c1b7ea21233d9ea09c41abe61d8a40b2547bb5db74239c6df857934
+  checksum: 72119d4a7d726c54167aa227c982ae9fa785c8ad97a158d8350ae95eecfbd8028a803eef939f7e6c5c6e626fcecda1dc37e9dffc6d5d6ec105f686aeda6b2c24
   languageName: node
   linkType: hard
 
 "@codemirror/lang-xml@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "@codemirror/lang-xml@npm:6.0.2"
+  version: 6.1.0
+  resolution: "@codemirror/lang-xml@npm:6.1.0"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
+    "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/xml": ^1.0.0
-  checksum: e156ecafaa87e9b6ef4ab6812ccd00d8f3c6cb81f232837636b36336d80513b61936dfee6f4f6800574f236208b61e95a2abcb997cdcd7366585a6b796e0e13b
+  checksum: 3a1b7af07b29ad7e53b77bf584245580b613bc92256059f175f2b1d7c28c4e39b75654fe169b9a8a330a60164b53ff5254bdb5b8ee8c6e6766427ee115c4e229
   languageName: node
   linkType: hard
 
 "@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
-  version: 6.9.2
-  resolution: "@codemirror/language@npm:6.9.2"
+  version: 6.10.1
+  resolution: "@codemirror/language@npm:6.10.1"
   dependencies:
     "@codemirror/state": ^6.0.0
-    "@codemirror/view": ^6.0.0
+    "@codemirror/view": ^6.23.0
     "@lezer/common": ^1.1.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
-  checksum: eee7b861b5591114cac7502cd532d5b923639740081a4cd7e28696c252af8d759b14686aaf6d5eee7e0969ff647b7aaf03a5eea7235fb6d9858ee19433f1c74d
+  checksum: 453bbe122a84795752f29261412b69a8dcfdd7e4369eb7e112bffba36b9e527ad21adff1d3845e0dc44c9ab44eb0c6f823eb6ba790ddd00cc749847574eda779
   languageName: node
   linkType: hard
 
 "@codemirror/legacy-modes@npm:^6.3.2":
-  version: 6.3.3
-  resolution: "@codemirror/legacy-modes@npm:6.3.3"
+  version: 6.4.0
+  resolution: "@codemirror/legacy-modes@npm:6.4.0"
   dependencies:
     "@codemirror/language": ^6.0.0
-  checksum: 3cd32b0f011b0a193e0948e5901b625f38aa6d9a8b24344531d6e142eb6fbb3e6cb5969429102044f3d04fbe53c4deaebd9f659c05067a0b18d17766290c9e05
+  checksum: d382aa6f640a67418bd209e1e4b395340f96aac1b0cf185927fc2c7f98b62cfd0c59ef0f7048148ce8771622003ca844c78c2d18548235ecc57d0bcbfbbfe091
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
-  version: 6.4.2
-  resolution: "@codemirror/lint@npm:6.4.2"
+  version: 6.5.0
+  resolution: "@codemirror/lint@npm:6.5.0"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: 5e699960c1b28dbaa584fe091a3201978907bf4b9e52810fb15d3ceaf310e38053435e0b594da0985266ae812039a5cd6c36023284a6f8568664bdca04db137f
+  checksum: b4f3899d0f73e5a2b5e9bc1df8e13ecb9324b94c7d384e7c8dde794109dee051461fc86658338f41652b44879b2ccc12cdd51a8ac0bb16a5b18aafa8e57a843c
   languageName: node
   linkType: hard
 
 "@codemirror/search@npm:^6.3.0":
-  version: 6.5.4
-  resolution: "@codemirror/search@npm:6.5.4"
+  version: 6.5.6
+  resolution: "@codemirror/search@npm:6.5.6"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: 32a68e40486730949ee79f54b9fcc6c744559aef188d3c5bf82881f62e5fc9468fa21cf227507638160043c797eb054205802a649cf4a2350928fc161d5aac40
+  checksum: 19dc88d09fc750563347001e83c6194bbb2a25c874bd919d2d81809e1f98d6330222ddbd284aa9758a09eeb41fd153ec7c2cf810b2ee51452c25963d7f5833d5
   languageName: node
   linkType: hard
 
-"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.1.4":
-  version: 6.3.1
-  resolution: "@codemirror/state@npm:6.3.1"
-  checksum: 8e7e55b3824653936606b31f146737459cb6654c935d668e7f36113ad523e1951966640f647c1286ae4ef22e3f0c7e37a6dfcbbcdb7bbeacca43c17c80fcc918
-  languageName: node
-  linkType: hard
-
-"@codemirror/state@npm:^6.2.0":
-  version: 6.2.1
-  resolution: "@codemirror/state@npm:6.2.1"
-  checksum: d12a321d0471b264b9d3259042bff913a8b939e8d28d408ff452004538a71ca9d5329df3f8a1d8a9183f5b42a7ef5b200737bcab1065714f5ae8e0a5ba9d59d3
+"@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
+  version: 6.4.1
+  resolution: "@codemirror/state@npm:6.4.1"
+  checksum: b81b55574091349eed4d32fc0eadb0c9688f1f7c98b681318f59138ee0f527cb4c4a97831b70547c0640f02f3127647838ae6730782de4a3dd2cc58836125d01
   languageName: node
   linkType: hard
 
-"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.9.6":
-  version: 6.21.4
-  resolution: "@codemirror/view@npm:6.21.4"
+"@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
+  version: 6.26.3
+  resolution: "@codemirror/view@npm:6.26.3"
   dependencies:
-    "@codemirror/state": ^6.1.4
+    "@codemirror/state": ^6.4.0
     style-mod: ^4.1.0
     w3c-keyname: ^2.2.4
-  checksum: e320eb46a6556984081c97e0bf5a9f5d45de2a4db5d632e6ee689a32dc081b10bda87aa989c4563981e28bf25bb651d1be57158fc2e753b587e3c6f7e2e486b2
+  checksum: fdee35fb5e0bbba7b6f1a9b43a865880911bbfafd30360da5dda21b35f81ba2d080ff66b6c3d94dbe946b6b7ec98a76208786360b8f030ef10bcb054b816de05
   languageName: node
   linkType: hard
 
 "@csstools/css-parser-algorithms@npm:^2.3.1":
-  version: 2.3.1
-  resolution: "@csstools/css-parser-algorithms@npm:2.3.1"
+  version: 2.6.1
+  resolution: "@csstools/css-parser-algorithms@npm:2.6.1"
   peerDependencies:
-    "@csstools/css-tokenizer": ^2.2.0
-  checksum: 90c6aa391ff817b0fc2ae20b9cc5e3308e3906536d83c8eeb502171ec709730a2cd0458eb7646378f74db545c9079fd026e125dbdbe26030652f9466bacc1183
+    "@csstools/css-tokenizer": ^2.2.4
+  checksum: 365745c2d6b3eaf26c77d09306c66012552d2b2e4cf94fabc230e8a6a954dab57867b24ebedd8bd518c8ced844c7f988e89144b5d9c76cfbddff126cfb2f153d
   languageName: node
   linkType: hard
 
 "@csstools/css-tokenizer@npm:^2.2.0":
-  version: 2.2.0
-  resolution: "@csstools/css-tokenizer@npm:2.2.0"
-  checksum: d6b3ead496e187cbf89b5e08a55be7a8393676c2b93526f7f051418376d08146f9f533708aca5eec6a07d925ea6a7e65b0e0bb36aabeba657666e968b8d89cd0
+  version: 2.2.4
+  resolution: "@csstools/css-tokenizer@npm:2.2.4"
+  checksum: 306ce5603e1084d782e125caa86eadad2a3115e36ec824b855df7e48bb4821eec7ccf336990d37874d76cf18156586866975e46c6a75583f218c61735749af81
   languageName: node
   linkType: hard
 
 "@csstools/media-query-list-parser@npm:^2.1.4":
-  version: 2.1.4
-  resolution: "@csstools/media-query-list-parser@npm:2.1.4"
+  version: 2.1.9
+  resolution: "@csstools/media-query-list-parser@npm:2.1.9"
   peerDependencies:
-    "@csstools/css-parser-algorithms": ^2.3.1
-    "@csstools/css-tokenizer": ^2.2.0
-  checksum: 8fa5be6acea01af39f49e08b2f2e2f7f54c2881c2c8a7a8cc783f8668610404398e81f86092f44ae64914d0f7626a5177d721ce5d1858b1599b26c91687f311e
+    "@csstools/css-parser-algorithms": ^2.6.1
+    "@csstools/css-tokenizer": ^2.2.4
+  checksum: c10c39ac23c38ccf6f21cc075ecced5cf9c98f237c559818d248b7b7ac08da5d2a92f80685a2958ef5862fb8cba4f12054f2fced5a18f8392d545934f52b42ff
   languageName: node
   linkType: hard
 
 "@csstools/selector-specificity@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "@csstools/selector-specificity@npm:3.0.0"
+  version: 3.0.3
+  resolution: "@csstools/selector-specificity@npm:3.0.3"
   peerDependencies:
     postcss-selector-parser: ^6.0.13
-  checksum: 4a2dfe69998a499155d9dab4c2a0e7ae7594d8db98bb8a487d2d5347c0c501655051eb5eacad3fe323c86b0ba8212fe092c27fc883621e6ac2a27662edfc3528
+  checksum: 287f17aefe2f22a39cb1c01d45d9e2c4c8c7cf11d9af67c44fe14fa2ed2e11178406661d1b6b023c8a447cdb08933ac134352a0c1452d409af4e7db2570684f3
   languageName: node
   linkType: hard
 
 "@discoveryjs/json-ext@npm:^0.5.0":
   version: 0.5.7
   resolution: "@discoveryjs/json-ext@npm:0.5.7"
   checksum: 2176d301cc258ea5c2324402997cf8134ebb212469c0d397591636cea8d3c02f2b3cf9fd58dcb748c7a0dade77ebdc1b10284fa63e608c033a1db52fddc69918
@@ -350,73 +349,73 @@
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
   checksum: cdfe3ae42b4f572cbfb46d20edafe6f36fc5fb52bf2d90875c58aefe226892b9677fef60820e2832caf864a326fe4fc225714c46e8389ccca04d5f9288aabd22
   languageName: node
   linkType: hard
 
 "@eslint-community/regexpp@npm:^4.5.1, @eslint-community/regexpp@npm:^4.6.1":
-  version: 4.8.1
-  resolution: "@eslint-community/regexpp@npm:4.8.1"
-  checksum: 82d62c845ef42b810f268cfdc84d803a2da01735fb52e902fd34bdc09f92464a094fd8e4802839874b000b2f73f67c972859e813ba705233515d3e954f234bf2
+  version: 4.10.0
+  resolution: "@eslint-community/regexpp@npm:4.10.0"
+  checksum: 2a6e345429ea8382aaaf3a61f865cae16ed44d31ca917910033c02dc00d505d939f10b81e079fa14d43b51499c640138e153b7e40743c4c094d9df97d4e56f7b
   languageName: node
   linkType: hard
 
-"@eslint/eslintrc@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@eslint/eslintrc@npm:2.1.2"
+"@eslint/eslintrc@npm:^2.1.4":
+  version: 2.1.4
+  resolution: "@eslint/eslintrc@npm:2.1.4"
   dependencies:
     ajv: ^6.12.4
     debug: ^4.3.2
     espree: ^9.6.0
     globals: ^13.19.0
     ignore: ^5.2.0
     import-fresh: ^3.2.1
     js-yaml: ^4.1.0
     minimatch: ^3.1.2
     strip-json-comments: ^3.1.1
-  checksum: bc742a1e3b361f06fedb4afb6bf32cbd27171292ef7924f61c62f2aed73048367bcc7ac68f98c06d4245cd3fabc43270f844e3c1699936d4734b3ac5398814a7
+  checksum: 10957c7592b20ca0089262d8c2a8accbad14b4f6507e35416c32ee6b4dbf9cad67dfb77096bbd405405e9ada2b107f3797fe94362e1c55e0b09d6e90dd149127
   languageName: node
   linkType: hard
 
-"@eslint/js@npm:8.49.0":
-  version: 8.49.0
-  resolution: "@eslint/js@npm:8.49.0"
-  checksum: a6601807c8aeeefe866926ad92ed98007c034a735af20ff709009e39ad1337474243d47908500a3bde04e37bfba16bcf1d3452417f962e1345bc8756edd6b830
+"@eslint/js@npm:8.57.0":
+  version: 8.57.0
+  resolution: "@eslint/js@npm:8.57.0"
+  checksum: 315dc65b0e9893e2bff139bddace7ea601ad77ed47b4550e73da8c9c2d2766c7a575c3cddf17ef85b8fd6a36ff34f91729d0dcca56e73ca887c10df91a41b0bb
   languageName: node
   linkType: hard
 
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
   languageName: node
   linkType: hard
 
-"@humanwhocodes/config-array@npm:^0.11.11":
-  version: 0.11.11
-  resolution: "@humanwhocodes/config-array@npm:0.11.11"
+"@humanwhocodes/config-array@npm:^0.11.14":
+  version: 0.11.14
+  resolution: "@humanwhocodes/config-array@npm:0.11.14"
   dependencies:
-    "@humanwhocodes/object-schema": ^1.2.1
-    debug: ^4.1.1
+    "@humanwhocodes/object-schema": ^2.0.2
+    debug: ^4.3.1
     minimatch: ^3.0.5
-  checksum: db84507375ab77b8ffdd24f498a5b49ad6b64391d30dd2ac56885501d03964d29637e05b1ed5aefa09d57ac667e28028bc22d2da872bfcd619652fbdb5f4ca19
+  checksum: 861ccce9eaea5de19546653bccf75bf09fe878bc39c3aab00aeee2d2a0e654516adad38dd1098aab5e3af0145bbcbf3f309bdf4d964f8dab9dcd5834ae4c02f2
   languageName: node
   linkType: hard
 
 "@humanwhocodes/module-importer@npm:^1.0.1":
   version: 1.0.1
   resolution: "@humanwhocodes/module-importer@npm:1.0.1"
   checksum: 0fd22007db8034a2cdf2c764b140d37d9020bbfce8a49d3ec5c05290e77d4b0263b1b972b752df8c89e5eaa94073408f2b7d977aed131faf6cf396ebb5d7fb61
   languageName: node
   linkType: hard
 
-"@humanwhocodes/object-schema@npm:^1.2.1":
-  version: 1.2.1
-  resolution: "@humanwhocodes/object-schema@npm:1.2.1"
-  checksum: a824a1ec31591231e4bad5787641f59e9633827d0a2eaae131a288d33c9ef0290bd16fda8da6f7c0fcb014147865d12118df10db57f27f41e20da92369fcb3f1
+"@humanwhocodes/object-schema@npm:^2.0.2":
+  version: 2.0.3
+  resolution: "@humanwhocodes/object-schema@npm:2.0.3"
+  checksum: d3b78f6c5831888c6ecc899df0d03bcc25d46f3ad26a11d7ea52944dc36a35ef543fad965322174238d677a43d5c694434f6607532cff7077062513ad7022631
   languageName: node
   linkType: hard
 
 "@isaacs/cliui@npm:^8.0.2":
   version: 8.0.2
   resolution: "@isaacs/cliui@npm:8.0.2"
   dependencies:
@@ -426,196 +425,190 @@
     strip-ansi-cjs: "npm:strip-ansi@^6.0.1"
     wrap-ansi: ^8.1.0
     wrap-ansi-cjs: "npm:wrap-ansi@^7.0.0"
   checksum: 4a473b9b32a7d4d3cfb7a614226e555091ff0c5a29a1734c28c72a182c2f6699b26fc6b5c2131dfd841e86b185aea714c72201d7c98c2fba5f17709333a67aeb
   languageName: node
   linkType: hard
 
-"@jridgewell/gen-mapping@npm:^0.3.0":
-  version: 0.3.3
-  resolution: "@jridgewell/gen-mapping@npm:0.3.3"
+"@jridgewell/gen-mapping@npm:^0.3.5":
+  version: 0.3.5
+  resolution: "@jridgewell/gen-mapping@npm:0.3.5"
   dependencies:
-    "@jridgewell/set-array": ^1.0.1
+    "@jridgewell/set-array": ^1.2.1
     "@jridgewell/sourcemap-codec": ^1.4.10
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 4a74944bd31f22354fc01c3da32e83c19e519e3bbadafa114f6da4522ea77dd0c2842607e923a591d60a76699d819a2fbb6f3552e277efdb9b58b081390b60ab
+    "@jridgewell/trace-mapping": ^0.3.24
+  checksum: ff7a1764ebd76a5e129c8890aa3e2f46045109dabde62b0b6c6a250152227647178ff2069ea234753a690d8f3c4ac8b5e7b267bbee272bffb7f3b0a370ab6e52
   languageName: node
   linkType: hard
 
 "@jridgewell/resolve-uri@npm:^3.1.0":
-  version: 3.1.1
-  resolution: "@jridgewell/resolve-uri@npm:3.1.1"
-  checksum: f5b441fe7900eab4f9155b3b93f9800a916257f4e8563afbcd3b5a5337b55e52bd8ae6735453b1b745457d9f6cdb16d74cd6220bbdd98cf153239e13f6cbb653
+  version: 3.1.2
+  resolution: "@jridgewell/resolve-uri@npm:3.1.2"
+  checksum: 83b85f72c59d1c080b4cbec0fef84528963a1b5db34e4370fa4bd1e3ff64a0d80e0cee7369d11d73c704e0286fb2865b530acac7a871088fbe92b5edf1000870
   languageName: node
   linkType: hard
 
-"@jridgewell/set-array@npm:^1.0.1":
-  version: 1.1.2
-  resolution: "@jridgewell/set-array@npm:1.1.2"
-  checksum: 69a84d5980385f396ff60a175f7177af0b8da4ddb81824cb7016a9ef914eee9806c72b6b65942003c63f7983d4f39a5c6c27185bbca88eb4690b62075602e28e
+"@jridgewell/set-array@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "@jridgewell/set-array@npm:1.2.1"
+  checksum: 832e513a85a588f8ed4f27d1279420d8547743cc37fcad5a5a76fc74bb895b013dfe614d0eed9cb860048e6546b798f8f2652020b4b2ba0561b05caa8c654b10
   languageName: node
   linkType: hard
 
 "@jridgewell/source-map@npm:^0.3.3":
-  version: 0.3.5
-  resolution: "@jridgewell/source-map@npm:0.3.5"
+  version: 0.3.6
+  resolution: "@jridgewell/source-map@npm:0.3.6"
   dependencies:
-    "@jridgewell/gen-mapping": ^0.3.0
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 1ad4dec0bdafbade57920a50acec6634f88a0eb735851e0dda906fa9894e7f0549c492678aad1a10f8e144bfe87f238307bf2a914a1bc85b7781d345417e9f6f
+    "@jridgewell/gen-mapping": ^0.3.5
+    "@jridgewell/trace-mapping": ^0.3.25
+  checksum: c9dc7d899397df95e3c9ec287b93c0b56f8e4453cd20743e2b9c8e779b1949bc3cccf6c01bb302779e46560eb45f62ea38d19fedd25370d814734268450a9f30
   languageName: node
   linkType: hard
 
 "@jridgewell/sourcemap-codec@npm:^1.4.10, @jridgewell/sourcemap-codec@npm:^1.4.14":
   version: 1.4.15
   resolution: "@jridgewell/sourcemap-codec@npm:1.4.15"
   checksum: b881c7e503db3fc7f3c1f35a1dd2655a188cc51a3612d76efc8a6eb74728bef5606e6758ee77423e564092b4a518aba569bbb21c9bac5ab7a35b0c6ae7e344c8
   languageName: node
   linkType: hard
 
-"@jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.9":
-  version: 0.3.19
-  resolution: "@jridgewell/trace-mapping@npm:0.3.19"
+"@jridgewell/trace-mapping@npm:^0.3.20, @jridgewell/trace-mapping@npm:^0.3.24, @jridgewell/trace-mapping@npm:^0.3.25":
+  version: 0.3.25
+  resolution: "@jridgewell/trace-mapping@npm:0.3.25"
   dependencies:
     "@jridgewell/resolve-uri": ^3.1.0
     "@jridgewell/sourcemap-codec": ^1.4.14
-  checksum: 956a6f0f6fec060fb48c6bf1f5ec2064e13cd38c8be3873877d4b92b4a27ba58289a34071752671262a3e3c202abcc3fa2aac64d8447b4b0fa1ba3c9047f1c20
+  checksum: 9d3c40d225e139987b50c48988f8717a54a8c994d8a948ee42e1412e08988761d0754d7d10b803061cc3aebf35f92a5dbbab493bd0e1a9ef9e89a2130e83ba34
   languageName: node
   linkType: hard
 
-"@jupyter/ydoc@npm:^1.0.2":
-  version: 1.1.0
-  resolution: "@jupyter/ydoc@npm:1.1.0"
+"@jupyter/react-components@npm:^0.15.2":
+  version: 0.15.3
+  resolution: "@jupyter/react-components@npm:0.15.3"
+  dependencies:
+    "@jupyter/web-components": ^0.15.3
+    "@microsoft/fast-react-wrapper": ^0.3.22
+    react: ">=17.0.0 <19.0.0"
+  checksum: 1a6b256314259c6465c4b6d958575710536b82234a7bf0fba3e889a07e1f19ff8ab321450be354359876f92c45dbcc9d21a840237ff4a619806d9de696f55496
+  languageName: node
+  linkType: hard
+
+"@jupyter/web-components@npm:^0.15.2, @jupyter/web-components@npm:^0.15.3":
+  version: 0.15.3
+  resolution: "@jupyter/web-components@npm:0.15.3"
+  dependencies:
+    "@microsoft/fast-colors": ^5.3.1
+    "@microsoft/fast-element": ^1.12.0
+    "@microsoft/fast-foundation": ^2.49.4
+    "@microsoft/fast-web-utilities": ^5.4.1
+  checksum: a0980af934157bfdbdb6cc169c0816c1b2e57602d524c56bdcef746a4c25dfeb8f505150d83207c8695ed89b5486cf53d35a3382584d25ef64db666e4e16e45b
+  languageName: node
+  linkType: hard
+
+"@jupyter/ydoc@npm:^1.1.1":
+  version: 1.1.1
+  resolution: "@jupyter/ydoc@npm:1.1.1"
   dependencies:
     "@jupyterlab/nbformat": ^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0
     "@lumino/coreutils": ^1.11.0 || ^2.0.0
     "@lumino/disposable": ^1.10.0 || ^2.0.0
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
-  checksum: 75530fa80ee157763d20c53251d3f28a8f19396145a7b59b003abd0ba4b040f977e259aaf61e220a2f74340902a0620f7a71f9ed09a165276e0178f4821fc821
+  checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
   languageName: node
   linkType: hard
 
 "@jupyterlab/application@npm:^3.5.0 || ^4.0.5":
-  version: 4.0.6
-  resolution: "@jupyterlab/application@npm:4.0.6"
+  version: 4.1.6
+  resolution: "@jupyterlab/application@npm:4.1.6"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.1.6
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/docregistry": ^4.0.6
-    "@jupyterlab/rendermime": ^4.0.6
-    "@jupyterlab/rendermime-interfaces": ^3.8.6
-    "@jupyterlab/services": ^7.0.6
-    "@jupyterlab/statedb": ^4.0.6
-    "@jupyterlab/translation": ^4.0.6
-    "@jupyterlab/ui-components": ^4.0.6
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/docregistry": ^4.1.6
+    "@jupyterlab/rendermime": ^4.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/statedb": ^4.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
-    "@lumino/application": ^2.2.1
-    "@lumino/commands": ^2.1.3
+    "@lumino/application": ^2.3.0
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-  checksum: 1212b71d3717bc02543b3eee74e69be799634421bd9b291b7adf07ba27bf6f9c7db860c423c824eaced9c2524db2f6b58de2c58e7edd5de2f0d7fabbb2c94b8c
+    "@lumino/widgets": ^2.3.1
+  checksum: 7b240381f1c661b75c9d165686cb2cd6d376596d1450c1e40a4bdb4dc608bbe71622f7e6f0520da385c7ad1dc10f5d21e88a074cb8077d3ba57280f7dd65ed84
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.1.6":
-  version: 4.1.6
-  resolution: "@jupyterlab/apputils@npm:4.1.6"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/observables": ^5.0.6
-    "@jupyterlab/rendermime-interfaces": ^3.8.6
-    "@jupyterlab/services": ^7.0.6
-    "@jupyterlab/settingregistry": ^4.0.6
-    "@jupyterlab/statedb": ^4.0.6
-    "@jupyterlab/statusbar": ^4.0.6
-    "@jupyterlab/translation": ^4.0.6
-    "@jupyterlab/ui-components": ^4.0.6
+"@jupyterlab/apputils@npm:^4.2.6":
+  version: 4.2.6
+  resolution: "@jupyterlab/apputils@npm:4.2.6"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/settingregistry": ^4.1.6
+    "@jupyterlab/statedb": ^4.1.6
+    "@jupyterlab/statusbar": ^4.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: 40fb43f5a6464c665f1b941d164f3366ab8ea906fed72894ccf026ebeebf0734409edb6546a151ac267cbd4f945e23474251aed644f7f0f0dbf2548b9230ae22
+  checksum: 2ca507223fb1ca3a527ce6c544c6fc1433a0eef9a41db54031f1b159a3ef29f4908e7408c22ce0cbf6e8a2e46999ab3f9175e06df54412dd6f583a5bdf11fb6a
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.1.8":
-  version: 4.1.8
-  resolution: "@jupyterlab/apputils@npm:4.1.8"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/settingregistry": ^4.0.8
-    "@jupyterlab/statedb": ^4.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.1.3
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/domutils": ^2.0.1
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
-    "@types/react": ^18.0.26
-    react: ^18.2.0
-    sanitize-html: ~2.7.3
-  checksum: 1b028893ac0358d9f90585edd5fbb89a4fe251c31789cf6d809fb316b91c958c6ba33884d463dbe78dfdd864b579535e1e1849bcb9b16853002271a71418d31e
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/attachments@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/attachments@npm:4.0.8"
+"@jupyterlab/attachments@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/attachments@npm:4.1.6"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime": ^4.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-  checksum: 17e14257fb28006144bd7824e9f78e5c4c792c9dfa60e67efdd0bb6e6e33109b52e1e10b18d8a76f4d8e5e8d4ab9a22254e92f13d8c8f9ed0803961f5de8ece0
+  checksum: 94080c9c2b925315b221fbd3cef167740a7ba553d435813c3cca6da0740bdb556e73614440795a05d4027eb3114b3935e951f1aa10769afc1af7fa57c137b3e2
   languageName: node
   linkType: hard
 
-"@jupyterlab/builder@npm:^4.0.0":
-  version: 4.0.6
-  resolution: "@jupyterlab/builder@npm:4.0.6"
+"@jupyterlab/builder@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/builder@npm:4.1.6"
   dependencies:
     "@lumino/algorithm": ^2.0.1
-    "@lumino/application": ^2.2.1
-    "@lumino/commands": ^2.1.3
+    "@lumino/application": ^2.3.0
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     ajv: ^8.12.0
     commander: ^9.4.1
     css-loader: ^6.7.1
     duplicate-package-checker-webpack-plugin: ^3.0.0
     fs-extra: ^10.1.0
     glob: ~7.1.6
     license-webpack-plugin: ^2.3.14
@@ -629,103 +622,81 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 8ee8db483e07bcc99c45133616a60f57eb2f323898217961cecf82ef875343879327ad7e74adaa860577742d946e8325f16dfcb54845930db41faa9f4bdad70c
+  checksum: 7807bc85d319ed43cedba7431a100219b5fb36fde40088f78faaf03d161a04c3a9fa2811e7d7ff47882c478e3fc264b19cce7e7bc2994329fb391e3975fdfb4b
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/cells@npm:4.0.8"
+"@jupyterlab/cells@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/cells@npm:4.1.6"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/attachments": ^4.0.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/codemirror": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/documentsearch": ^4.0.8
-    "@jupyterlab/filebrowser": ^4.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/outputarea": ^4.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/toc": ^6.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/attachments": ^4.1.6
+    "@jupyterlab/codeeditor": ^4.1.6
+    "@jupyterlab/codemirror": ^4.1.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/documentsearch": ^4.1.6
+    "@jupyterlab/filebrowser": ^4.1.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/outputarea": ^4.1.6
+    "@jupyterlab/rendermime": ^4.1.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/toc": ^6.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
-    react: ^18.2.0
-  checksum: 42e4464574a603f48df299ccf2d84bf5f90f0aa39b0a9c680c9db5d254b416ee784ec3b5a1475ed72a10e6dcf1075715d66bf3afeee55e365c42656daea3f002
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/codeeditor@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/codeeditor@npm:4.0.6"
-  dependencies:
-    "@codemirror/state": ^6.2.0
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/nbformat": ^4.0.6
-    "@jupyterlab/observables": ^5.0.6
-    "@jupyterlab/statusbar": ^4.0.6
-    "@jupyterlab/translation": ^4.0.6
-    "@jupyterlab/ui-components": ^4.0.6
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/dragdrop": ^2.1.3
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 831d330273280781dbdc223325d575ac373c0db17fab208f327bce4e1c2286c62f8264d1d612da1a762bc006cd81dfb0eb5108dd3bd8f8298f9be8ecac98b2ca
+  checksum: 03c0d032a4a25795d5f086deae22343d52e0034fbd5098151565cfe5dcb17126bf6a277f5ef6e5d3358abc72a989e3000033e1b35e03b4fd4e2e3c45fbb0cde0
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/codeeditor@npm:4.0.8"
+"@jupyterlab/codeeditor@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/codeeditor@npm:4.1.6"
   dependencies:
     "@codemirror/state": ^6.2.0
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/statusbar": ^4.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 151be40c60bcedf463d01b9c53466afc4b4747dd341fb4d5c2b9fc8b3c181af2ba391f867e10e78bb948848cdd300139b4b112634dec9f8aac9c36c5a13e1654
+  checksum: 0c34e3f30e20aa590ac8308b00b1dc89a51b0b214cd0d548311b5b7392ae072db42e7823963ca0faf7761eadf5c4b62a1b25e467e44c93a0ccb9ac5ad645d1c3
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/codemirror@npm:4.0.8"
+"@jupyterlab/codemirror@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/codemirror@npm:4.1.6"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
@@ -739,788 +710,605 @@
     "@codemirror/lang-wast": ^6.0.1
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/documentsearch": ^4.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/codeeditor": ^4.1.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/documentsearch": ^4.1.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/translation": ^4.1.6
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
     "@lezer/markdown": ^1.0.2
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     yjs: ^13.5.40
-  checksum: 2edd2ac9d695f8107d444379289b4cecf3603c118d748608738abe2a1af9d311d0407c5709ccbe016dd0a16c3a52d7f0132446173678246841c8ddf8ade371c7
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/coreutils@npm:^6.0.0, @jupyterlab/coreutils@npm:^6.0.6":
-  version: 6.0.6
-  resolution: "@jupyterlab/coreutils@npm:6.0.6"
-  dependencies:
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/signaling": ^2.1.2
-    minimist: ~1.2.0
-    path-browserify: ^1.0.0
-    url-parse: ~1.5.4
-  checksum: cf3cfbc7c48cae20549f5514a949b253c2f9d67c79db107ab0a81c2b7a9c08e28f9fd264e3d944a05a8cb1bbb9676c6b4163b75c28788d1cb3a3cc523d44d802
+  checksum: 3083fad1754ef15d9ffc02a6c0d6f6c368cd90a40943245b92f321befc8c61ffe26a9bc260224e6ec32fc3df67feacf4fb925a51cc24aa90036d6ab3e7b7e9f2
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.8":
-  version: 6.0.8
-  resolution: "@jupyterlab/coreutils@npm:6.0.8"
+"@jupyterlab/coreutils@npm:^6.0.0, @jupyterlab/coreutils@npm:^6.1.6":
+  version: 6.1.6
+  resolution: "@jupyterlab/coreutils@npm:6.1.6"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: b56e3b95c0ce52745b79549ef5b18a27e620086b87cf997b3a743b59d18dc529e403c812751b7e294a4abc60ac957381301e14327e1a4b9c1afb232f181f3a4d
+  checksum: f351f327f9c7ab14ac291e4ca85a8f4289dd315e9f2e68fc6acb52efab6c47fde158f65a83ba780c382665459995bad68c7b1f9c4ffef6b9038ac81252a3f07a
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/docmanager@npm:4.0.8"
+"@jupyterlab/docmanager@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/docmanager@npm:4.1.6"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/docregistry": ^4.1.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/statusbar": ^4.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 70eea965bb9edd6a4042c92d2cb98f8b1b145b6727a354e12e3f5ab84ff2ab7207c5d9433c43c03d01f4377f9dc901359d789d0f47d2c725e56f41c487295550
+  checksum: 890a8f86fc3d96d896e86ed64ef3c713152d781c941eea99d1b2d021bf5d1844f2d0a52d8cb077b1e8a1d31f13a6253c118cbe70440e10df20a490ab2595bab2
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/docregistry@npm:4.0.6"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.6
-    "@jupyterlab/codeeditor": ^4.0.6
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/observables": ^5.0.6
-    "@jupyterlab/rendermime": ^4.0.6
-    "@jupyterlab/rendermime-interfaces": ^3.8.6
-    "@jupyterlab/services": ^7.0.6
-    "@jupyterlab/translation": ^4.0.6
-    "@jupyterlab/ui-components": ^4.0.6
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-  checksum: 57de3751ea04037f27596ffe782392fb4840f3fba1776a64bb7b0dc5936a3cee4de115b2133147cda23a697d3da7802daaec0effae10be329d6c774f102091ee
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/docregistry@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/docregistry@npm:4.0.8"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/docregistry@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/docregistry@npm:4.1.6"
+  dependencies:
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/codeeditor": ^4.1.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime": ^4.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-  checksum: 280697f97ca146cc711c5dafa1b27eaa89d96bc53fc92ade7d4b78c44c997feb9d2495b392c31e75ed3c836797865e2f3fa6ea8f3207f46a4ab2d26061dc9498
+    "@lumino/widgets": ^2.3.1
+    react: ^18.2.0
+  checksum: 0b7db803cd0013e1b65f0294b5bec2f6d4047cd7b191080ade3d67ff78d1d5a2d0e3a7016532dd316899b291bbc0b07561a958b2dd750dbcf3fc34927552c0d8
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/documentsearch@npm:4.0.8"
+"@jupyterlab/documentsearch@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/documentsearch@npm:4.1.6"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 5ee4c4b910af158b4ca488c617b12b2a84d391cfb6be94a38136a1eb80f639ec4b446fd862748a76732bc3eccd290750c0e9f6b6211d3c15d0776073173a5343
+  checksum: 911fd30871b5087c1ad8c3decd3c5ac184aa61ae02e3bd7577665ad941d4078082df6ddf25af2acf937f4674f7fc1f2347698eef352ebbac67702e1a4b296491
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/filebrowser@npm:4.0.8"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docmanager": ^4.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/statedb": ^4.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/filebrowser@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/filebrowser@npm:4.1.6"
+  dependencies:
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/docmanager": ^4.1.6
+    "@jupyterlab/docregistry": ^4.1.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/statedb": ^4.1.6
+    "@jupyterlab/statusbar": ^4.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 907dade3b9ab6bde667cdf2acc76c0fb2d631c06d794115a456cb6b1995a3b89b2a9f5c53a75824b337833cd05967c55fd919ca1311f24279aa5f067f948378a
+  checksum: 886d086b183b3d92af0dcafc7f752ef9bcaabd8e48af39794446897240091390989c5c9dd5e602d5f29a240e99ca4134f802d63c55b2a5f87168adf20a9bc26e
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/lsp@npm:4.0.8"
+"@jupyterlab/lsp@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/lsp@npm:4.1.6"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/codeeditor": ^4.1.6
+    "@jupyterlab/codemirror": ^4.1.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/docregistry": ^4.1.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/translation": ^4.1.6
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
+    "@lumino/widgets": ^2.3.1
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: baf2d42800a617a9d06d8cbb9c755e0cc40994c25c7c5d31bca1b7ac4fc4ad67d77fadb53de020e52d499a46e41dea1d84abb388b9bc20d468a5e888c687f301
+  checksum: d777321cdc78896a7a184394937fdccbab1c623d4f4897335c4da419862ef09e62919667ba7a5a5da5df10a474e9da1ebb0e8f8dde444c3efdf3d9ddaf4a2e67
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/nbformat@npm:4.0.6"
-  dependencies:
-    "@lumino/coreutils": ^2.1.2
-  checksum: 43ace863be98a82875a55a947828b9b987cff35bb484e6cb6474c97f60aadbf31027c5f2fdf81b4ee2d108dc735b92c15c9b35cded765b0e476ebf0c8fd670f6
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/nbformat@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/nbformat@npm:4.0.8"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/nbformat@npm:4.1.6"
   dependencies:
     "@lumino/coreutils": ^2.1.2
-  checksum: 2d8255ac7c7c20dbfa8497ce4d8d2f5840568adefb2feaec8eb8ddbb4892f50706ce60e8c4719113485c5523f720802f7e4e7b63ed43fac90f870ff1134bed7a
+  checksum: 4ef43fdaaecec06732528753c5316adaa883c77ae86d129fb5d1f0542124acc0e7bb5692aae799463722b8c47ce8934356572c040d682e0ce41548eca3ca421b
   languageName: node
   linkType: hard
 
 "@jupyterlab/notebook@npm:^4.0.7":
-  version: 4.0.8
-  resolution: "@jupyterlab/notebook@npm:4.0.8"
+  version: 4.1.6
+  resolution: "@jupyterlab/notebook@npm:4.1.6"
   dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/cells": ^4.0.8
-    "@jupyterlab/codeeditor": ^4.0.8
-    "@jupyterlab/codemirror": ^4.0.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/documentsearch": ^4.0.8
-    "@jupyterlab/lsp": ^4.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/settingregistry": ^4.0.8
-    "@jupyterlab/statusbar": ^4.0.8
-    "@jupyterlab/toc": ^6.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/cells": ^4.1.6
+    "@jupyterlab/codeeditor": ^4.1.6
+    "@jupyterlab/codemirror": ^4.1.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/docregistry": ^4.1.6
+    "@jupyterlab/documentsearch": ^4.1.6
+    "@jupyterlab/lsp": ^4.1.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime": ^4.1.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/settingregistry": ^4.1.6
+    "@jupyterlab/statusbar": ^4.1.6
+    "@jupyterlab/toc": ^6.1.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 64ea11e1923fcae46d263c732cfa6a69a51099bdd637f40599da5359fb884600179a3c5b6f3c176c6ffa725f425b33f435be6391f8d087b443e5fc6d6d11ced2
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/observables@npm:^5.0.6":
-  version: 5.0.6
-  resolution: "@jupyterlab/observables@npm:5.0.6"
-  dependencies:
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-  checksum: 23232972e6a049b2addeae1d445bc3a10bb6c9a3dd4794225a0344aaa1ff62421ee300ef8803a19a3f068d2bba2de8b9a8dec719a7f47019fbd77c8d5dafb7a0
+  checksum: 46401d9bd70bffec69d226a2cf35b6194cbdd4b47f2833a39e31fbd95e1f75b3ddc71c13286c25eed5c7e7092de566a89301fadb2923841ecf11e1802c874469
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.0.8":
-  version: 5.0.8
-  resolution: "@jupyterlab/observables@npm:5.0.8"
+"@jupyterlab/observables@npm:^5.1.6":
+  version: 5.1.6
+  resolution: "@jupyterlab/observables@npm:5.1.6"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 833c6af7f66a338d53e4ebfae2c10c57a55b8a1710730eed89e7a0103a4dd27b7b5634d0e7cf9c7db47d891fd4c8e72235de9816833482ef68356846200613be
+  checksum: 930e53ca38dd08232ec46585acf8d49ebbef9628a792619fbf51a1da13f3249da24a7a8b24c34a2c7ce3fa50145a4e647b65e19275ea5ce92946a2ad805faa82
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/outputarea@npm:4.0.8"
+"@jupyterlab/outputarea@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/outputarea@npm:4.1.6"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime": ^4.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/translation": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-  checksum: 4e97a367d6d06b05838056ef6da48891484fe84e5c06a08f0928f7359fa8362f48903434d033e8ddabdc193ef4b61859855fecbebda3949703583275fd099339
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/rendermime-interfaces@npm:^3.8.6":
-  version: 3.8.6
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.6"
-  dependencies:
-    "@lumino/coreutils": ^1.11.0 || ^2.1.2
-    "@lumino/widgets": ^1.37.2 || ^2.3.0
-  checksum: 84ba0c3979e6ace6246e00248d1248075afb112f55be202257bb89a553b235d36ca82879c56f46f58285a5fc6d39914e93fea203c53245e0ac8d1b5ef838bb50
+    "@lumino/widgets": ^2.3.1
+  checksum: e45e0db75b1d4def07ff48323ac84ef1b7eedfd09cff24a9c669db8da9bc846fd8186eaa34a210e66fdab2c0b6a9be93e406e7e54456063fbe879bf2c2ffcbea
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.8.8":
-  version: 3.8.8
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.8"
+"@jupyterlab/rendermime-interfaces@npm:^3.9.6":
+  version: 3.9.6
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.6"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
-    "@lumino/widgets": ^1.37.2 || ^2.3.0
-  checksum: b356cc18acedd7eebbf9e6f03329ad58f0aadb676ef7ef6b64dec610857a53593662df54752bb58780d34f39938ec35c6940918513e3a3cef7c5893bd0909684
+    "@lumino/widgets": ^1.37.2 || ^2.3.1
+  checksum: 9dd08d4c71ece6e68e2972b4ce950153e2d38cc876208bb1f0e5d533daf50b062bd6aa1711c94934ea2a1f8445cf49dc6370cda80e1372b3fbede0d4534b0235
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/rendermime@npm:4.0.6"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.6
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/nbformat": ^4.0.6
-    "@jupyterlab/observables": ^5.0.6
-    "@jupyterlab/rendermime-interfaces": ^3.8.6
-    "@jupyterlab/services": ^7.0.6
-    "@jupyterlab/translation": ^4.0.6
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-    lodash.escape: ^4.0.1
-  checksum: 8f44601ccd6abe9985f8f713dcabf48ae38246b8b5a17a3963ebfe298dc2a03cc49d1f99c6d3bfeadbe1eb74803d0b3138c01347693a99166d7d70cb832c400b
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/rendermime@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/rendermime@npm:4.0.8"
+"@jupyterlab/rendermime@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/rendermime@npm:4.1.6"
   dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/translation": ^4.1.6
     "@lumino/coreutils": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     lodash.escape: ^4.0.1
-  checksum: c1f9ebffc746fdc13c1b14a148fd2ae10132b5ca4e1eab27d18ac5bf3d3ae70cf2850b06f6c05a799f2c769792d81dab1447885d0cda7206c7cf63af10bbe4f2
+  checksum: f79430851e97c4a26938bdbd3d834a0beba2860630f5f8bcccda433a2b3c52d26b180e89d016ec7cd0fce28cbc71dc825307b8b37ca63951775965cb091381ab
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.0, @jupyterlab/services@npm:^7.0.6":
-  version: 7.0.6
-  resolution: "@jupyterlab/services@npm:7.0.6"
+"@jupyterlab/services@npm:^7.0.0, @jupyterlab/services@npm:^7.1.6":
+  version: 7.1.6
+  resolution: "@jupyterlab/services@npm:7.1.6"
   dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/nbformat": ^4.0.6
-    "@jupyterlab/settingregistry": ^4.0.6
-    "@jupyterlab/statedb": ^4.0.6
+    "@jupyter/ydoc": ^1.1.1
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/settingregistry": ^4.1.6
+    "@jupyterlab/statedb": ^4.1.6
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: 6e12ef309559977209e61ce3ec8ca74aa486d54f50d8f38211b684055fb2335a21c2ae6e846d2863e48524bffd7d6ac4d36dfc9f7ca610ae4b1c60752fa6c3a8
+  checksum: ad47d3c9b211be4be3aad2714f3028e66ad381a6367a57f347644c693f055ee9c7655d15630a637d9181b42e89c2b8183675abc561c3959820a6bc03d3f2af12
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.8":
-  version: 7.0.8
-  resolution: "@jupyterlab/services@npm:7.0.8"
-  dependencies:
-    "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/settingregistry": ^4.0.8
-    "@jupyterlab/statedb": ^4.0.8
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/polling": ^2.1.2
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    ws: ^8.11.0
-  checksum: b0112854d3014eff9d9855a6840d1efd0d866d4c011e7a9c4c1c5fba404dd13107b62de6ce845902d12cc6404aafdfee95127a2af43560ade53a00fc7b73378a
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/settingregistry@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/settingregistry@npm:4.0.6"
-  dependencies:
-    "@jupyterlab/nbformat": ^4.0.6
-    "@jupyterlab/statedb": ^4.0.6
-    "@lumino/commands": ^2.1.3
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/signaling": ^2.1.2
-    "@rjsf/utils": ^5.1.0
-    ajv: ^8.12.0
-    json5: ^2.2.3
-  peerDependencies:
-    react: ">=16"
-  checksum: 70b6fc44a25e0d4ec36501c1418fe2764b9a9415f892df0901c43480b608a1621141ec8045183dfbca5aedf11ebaf1518dd76e2e96373b9ebe0efa6586ce856d
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/settingregistry@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/settingregistry@npm:4.0.8"
+"@jupyterlab/settingregistry@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/settingregistry@npm:4.1.6"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.8
-    "@jupyterlab/statedb": ^4.0.8
-    "@lumino/commands": ^2.1.3
+    "@jupyterlab/nbformat": ^4.1.6
+    "@jupyterlab/statedb": ^4.1.6
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-    "@rjsf/utils": ^5.1.0
+    "@rjsf/utils": ^5.13.4
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: e9661539357edae60e4b300dff68b369e95e96acb343aeb25e23bdbcd6964c59dd40118ce3a856afaf969833958f3872c480e75cc488a5e882546cb88587c461
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/statedb@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/statedb@npm:4.0.6"
-  dependencies:
-    "@lumino/commands": ^2.1.3
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-  checksum: de507d094afcce7f7d12f9dc846788765616140b2f75ea22997f780056baaaadae0cf9683471a1d96c61d448b38860640c823302aeef0d5e5d7c9cf598074328
+  checksum: 93c1a4921a30243f2bd2c9591319e749e2f5cb5884f6962241857640afb6b67600cdba44fb308a23bffacc7defa3c6fc3d2ad15be52ff5946f0a8fd873b5fddd
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/statedb@npm:4.0.8"
+"@jupyterlab/statedb@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/statedb@npm:4.1.6"
   dependencies:
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: bfd016e91158daf47e07e760126c0c2c3f6d01ecc8e9cad3e17241e5873decbc5fdfce82bf039fa83633b8760245af8003008f38272dafba56b73ac24768a99f
+  checksum: 4aba49eeead6ac6306ec2d8146543230db9296e7bf088380290eb4b89698b66573c00ba630890b821047b584fc59716b64ba06a013d4698551adeaf20b034301
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/statusbar@npm:4.0.6"
-  dependencies:
-    "@jupyterlab/ui-components": ^4.0.6
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-    react: ^18.2.0
-  checksum: c5d579b101e19670182d87de0d601fc9c73c40b5a81120e18e6cd7853ee9fd744fa31524f24b2c92cb587bb2d6aa54c08f6e257d868426a73d968e48b1101b7c
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/statusbar@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/statusbar@npm:4.0.8"
+"@jupyterlab/statusbar@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/statusbar@npm:4.1.6"
   dependencies:
-    "@jupyterlab/ui-components": ^4.0.8
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: a07345a173e1c4500e5ce9aca6c8d619e5fecd928de0f6e88fd29241b39c09b85b26722279cc8119031d3015f2b32a0d3b9d85fd3cf9370c7605ebcd37d0d31a
+  checksum: ad8a7f366b8a3b3f1f6a4993a0b890192f5de99f0fe3b29aecb7a6474d568203798bee63b77012d4cfdc793b7b376ec8bd64b3c5e67cb26511b13801e7a75f77
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.0.8":
-  version: 6.0.8
-  resolution: "@jupyterlab/toc@npm:6.0.8"
-  dependencies:
-    "@jupyterlab/apputils": ^4.1.8
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/docregistry": ^4.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime": ^4.0.8
-    "@jupyterlab/translation": ^4.0.8
-    "@jupyterlab/ui-components": ^4.0.8
+"@jupyterlab/toc@npm:^6.1.6":
+  version: 6.1.6
+  resolution: "@jupyterlab/toc@npm:6.1.6"
+  dependencies:
+    "@jupyterlab/apputils": ^4.2.6
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/docregistry": ^4.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime": ^4.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/translation": ^4.1.6
+    "@jupyterlab/ui-components": ^4.1.6
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-    "@lumino/widgets": ^2.3.0
+    "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 5d4373c5e0b3ea302275cdf117e17a201a6ab8337288cbdb7e6048b87de2ed8e293e3dd203fb23f7d25db080e06e8271559b1d5aa5e33202130cc95d0972b95f
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/translation@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/translation@npm:4.0.6"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/rendermime-interfaces": ^3.8.6
-    "@jupyterlab/services": ^7.0.6
-    "@jupyterlab/statedb": ^4.0.6
-    "@lumino/coreutils": ^2.1.2
-  checksum: 490243a26898bbdcc1909e8e1649be90580c6d4502417590fd1b3ca24db5aeff2323e567dbfb1d528c56df89ed2e7717753ece784134f9e409d14df92bf25682
+  checksum: 45111e9a02f9e9bd96b6a7024d1374abacb00924dc4b5c2dce0a5f1cfb18d7a60b749a56d71196d6cab843f5c9f9a06ca18cdf8f176292bf0f13880fd332cfc7
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/translation@npm:4.0.8"
+"@jupyterlab/translation@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/translation@npm:4.1.6"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/services": ^7.0.8
-    "@jupyterlab/statedb": ^4.0.8
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/services": ^7.1.6
+    "@jupyterlab/statedb": ^4.1.6
     "@lumino/coreutils": ^2.1.2
-  checksum: 998d42d85ccd779237ac69abfaf2e341d865374ed5a1a4d234470337f498636511eec0562c741ad44a6a75fae930a510a0a76e176f72665499be2b7edb0dc5f8
+  checksum: 6de45e310d7ac83f2ed2e3e0c372ba71d087e597891d9e9a7ff791f6fc7fc3804d0d18dad5b152757c5a2b583d564ed7f4361561fa993be303e415a47e8b2fa6
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.6":
-  version: 4.0.6
-  resolution: "@jupyterlab/ui-components@npm:4.0.6"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.6
-    "@jupyterlab/observables": ^5.0.6
-    "@jupyterlab/rendermime-interfaces": ^3.8.6
-    "@jupyterlab/translation": ^4.0.6
-    "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.1.3
-    "@lumino/coreutils": ^2.1.2
-    "@lumino/disposable": ^2.1.2
-    "@lumino/messaging": ^2.0.1
-    "@lumino/polling": ^2.1.2
-    "@lumino/properties": ^2.0.1
-    "@lumino/signaling": ^2.1.2
-    "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
-    "@rjsf/core": ^5.1.0
-    "@rjsf/utils": ^5.1.0
-    react: ^18.2.0
-    react-dom: ^18.2.0
-    typestyle: ^2.0.4
-  peerDependencies:
-    react: ^18.2.0
-  checksum: 02997c3c35c15c0eda6a0d49fe9cfd12a3c5194c026b2ae8d8e53c7af80b769ba1598e7c24283450bacae7b8fab838d18f6c614d686c98d3d43e68f1f00b2528
-  languageName: node
-  linkType: hard
-
-"@jupyterlab/ui-components@npm:^4.0.8":
-  version: 4.0.8
-  resolution: "@jupyterlab/ui-components@npm:4.0.8"
+"@jupyterlab/ui-components@npm:^4.1.6":
+  version: 4.1.6
+  resolution: "@jupyterlab/ui-components@npm:4.1.6"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.8
-    "@jupyterlab/observables": ^5.0.8
-    "@jupyterlab/rendermime-interfaces": ^3.8.8
-    "@jupyterlab/translation": ^4.0.8
+    "@jupyter/react-components": ^0.15.2
+    "@jupyter/web-components": ^0.15.2
+    "@jupyterlab/coreutils": ^6.1.6
+    "@jupyterlab/observables": ^5.1.6
+    "@jupyterlab/rendermime-interfaces": ^3.9.6
+    "@jupyterlab/translation": ^4.1.6
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-    "@lumino/widgets": ^2.3.0
-    "@rjsf/core": ^5.1.0
-    "@rjsf/utils": ^5.1.0
+    "@lumino/widgets": ^2.3.1
+    "@rjsf/core": ^5.13.4
+    "@rjsf/utils": ^5.13.4
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: 7bf11f5ee3c1f88656175c0d3b290be0670d7787076a1eba944875e4780bc2b34c0b9a3af038806ff925620b3056cee36daff08f3ff91acc6c46fd1438bf004d
+  checksum: f555138b2345aac6ee5c580b517fd563b55b8a6b33f132de362d559a514bbbec970bd690970676173872674f802a5dd9de7ac75b897a0a2b09d7428dddc3c04d
   languageName: node
   linkType: hard
 
-"@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0":
-  version: 1.1.0
-  resolution: "@lezer/common@npm:1.1.0"
-  checksum: 93c208a44d1c0bdf7407853ba7c4ddcedf1c52d1b82170813d83b9bd6301aa23587405ac54332fe39ce8bc37f706936ab237ceb4d3d535d1dead650153b6474c
+"@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "@lezer/common@npm:1.2.1"
+  checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
   languageName: node
   linkType: hard
 
 "@lezer/cpp@npm:^1.0.0":
-  version: 1.1.1
-  resolution: "@lezer/cpp@npm:1.1.1"
+  version: 1.1.2
+  resolution: "@lezer/cpp@npm:1.1.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: c9e1db19776eafbfe0c3b8448d46c94d9a1d30f7fef630292e63bab82e6d5d6903a043ee8cf341bcbf84c00ee0d79b8c255bab8fd8e0a91355ae912b53c78935
+  checksum: a319cd46fd32affc07c9432e9b2b9954becf7766be0361176c525d03474bb794cc051aad9932f48c9df33833eee1d6bfdccab12e571f2b137b4ca765c60c75de
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.3
-  resolution: "@lezer/css@npm:1.1.3"
+  version: 1.1.8
+  resolution: "@lezer/css@npm:1.1.8"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: c8069ef0a6751441d2dc9180f7ebfd7aeb35df0ca2f1a748a2f26203a9ef6cc30f17f3074e2b49520453eb39329dadfdbbb901c6d9d067dc955ceb58c1f8cc6a
+  checksum: 1f5968360dbac7ba27f0c2a194143769f7b01824715274dd8507dacf13cc790bb8c48ce95de355e9c58be93bb3e271bf98b9fc51213f79e4ce918e7c7ebbef04
   languageName: node
   linkType: hard
 
 "@lezer/generator@npm:^1.2.2":
-  version: 1.5.1
-  resolution: "@lezer/generator@npm:1.5.1"
+  version: 1.7.0
+  resolution: "@lezer/generator@npm:1.7.0"
   dependencies:
-    "@lezer/common": ^1.0.2
+    "@lezer/common": ^1.1.0
     "@lezer/lr": ^1.3.0
   bin:
     lezer-generator: src/lezer-generator.cjs
-  checksum: 4d8267e6d356e48ca5214a234679b2b3b1d3706cb9dffecee4495b7a16c8a02502d6a078f8afdf5d8c79f94af34f2c1b5c08556aead8376d7b23795612b651d0
+  checksum: 69f4c6625446cb65adaa509480ec67502f27651707a8e45e99373e682d7f66f8842205669f174bcb138eade72c64ded0b54d6de6aa5af995ac1f1e805ef021fd
   languageName: node
   linkType: hard
 
 "@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
-  version: 1.1.6
-  resolution: "@lezer/highlight@npm:1.1.6"
+  version: 1.2.0
+  resolution: "@lezer/highlight@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: 411a702394c4c996b7d7f145a38f3a85a8cc698b3918acc7121c629255bb76d4ab383753f69009e011dc415210c6acbbb5b27bde613259ab67e600b29397b03b
+  checksum: 5b9dfe741f95db13f6124cb9556a43011cb8041ecf490be98d44a86b04d926a66e912bcd3a766f6a3d79e064410f1a2f60ab240b50b645a12c56987bf4870086
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.6
-  resolution: "@lezer/html@npm:1.3.6"
+  version: 1.3.9
+  resolution: "@lezer/html@npm:1.3.9"
   dependencies:
-    "@lezer/common": ^1.0.0
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 1d3af781660968505e5083a34f31ea3549fd5f3949227fa93cc318bca61bce76ffe977bd875624ba938a2039834ec1a33df5d365e94c48131c85dd26f980d92c
+  checksum: 40d89b0af4379768ce7d3e7162988e9ec73b42984e333e877c7451f7e2c10131e39e4b50150bc334093cbd84a3b34f9fc1a6ac62cbba51f503a495ad243e880b
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "@lezer/java@npm:1.0.4"
+  version: 1.1.1
+  resolution: "@lezer/java@npm:1.1.1"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 97f5a2c2d733afba5dc57a0da9a97515b19b5e63bb5937717dac4e8c9baed74d15c0cb5c1580858b678931f11d517c56d89f903968fa48931f9c62e2ea67a107
+  checksum: 8a071aca6b5e1ed1d22bffed22bbd29f21b102b7337a7ea5c956eb259e6ff20eee2d6e85b7dadff69859cb6615d6b1a3f0ba109673e87ce5a1f6cabdeee626fd
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.9
-  resolution: "@lezer/javascript@npm:1.4.9"
+  version: 1.4.14
+  resolution: "@lezer/javascript@npm:1.4.14"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: adac0048e4ab33dc48db42014f02d53a2eab81d12c990b23f237a3e83b125bda271607442aaa50dc0ac870a803e678135111366235f7c29a5052a288c1003960
+  checksum: 4880026f72bcfcd13f204cc57f1469ba04597304ba79d1331048be1e2b0bcb879e9d4b7e57a6a273f38ac66385740b15a6edb4249ecfcc971b94804298399256
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/json@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/json@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: fcd17178f6a58e71c83e08fdc047e3708528b28591ba8f08ed35268f370d1ec9b63af0afa9d82a77fec26e9eb477ab3cfdc31c951e080d118ef607f9f9bb52e3
+  checksum: f899d13765d95599c9199fc3404cb57969031dc40ce07de30f4e648979153966581f0bee02e2f8f70463b0a5322206a97c2fe8d5d14f218888c72a6dcedf90ef
   languageName: node
   linkType: hard
 
 "@lezer/lr@npm:^1.0.0, @lezer/lr@npm:^1.1.0, @lezer/lr@npm:^1.3.0":
-  version: 1.3.13
-  resolution: "@lezer/lr@npm:1.3.13"
+  version: 1.4.0
+  resolution: "@lezer/lr@npm:1.4.0"
   dependencies:
     "@lezer/common": ^1.0.0
-  checksum: aad0cb8908796a6b49116842fd490093aa0de54b48150a60a4f418815c014f7a1b4355615832e305caea5c0ba8c5ab577f82aebcd0ea04586b8199284ef0fec8
+  checksum: 4c8517017e9803415c6c5cb8230d8764107eafd7d0b847676cd1023abb863a4b268d0d01c7ce3cf1702c4749527c68f0a26b07c329cb7b68c36ed88362d7b193
   languageName: node
   linkType: hard
 
 "@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
-  version: 1.1.0
-  resolution: "@lezer/markdown@npm:1.1.0"
+  version: 1.3.0
+  resolution: "@lezer/markdown@npm:1.3.0"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
-  checksum: b3699c0724dd41e3e6e3078a0e1bcd272ccaebf17b20e5160de3ecf26200cdaa59aa19c9542aac5ab8c7e3aecce1003544b016bb5c32e458bbd5982add8ca0bf
+  checksum: 13eb2720e4cb84278349bad8af116f748813094f99fad02680010c3a8c5985e0358c344487990f87a31ef0d6c1a2be582301f914c0e4a6e9cfa22647b6cd6545
   languageName: node
   linkType: hard
 
 "@lezer/php@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/php@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/php@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
-  checksum: a847c255c030b4d38913ddf1d5bd7324d83be7ef8d1d244542870be03b9bf7dc71283afeb2415c40dfd188cb99f0cc44bad760b5f3b7c35c3b8e5e00253848fc
+  checksum: c85ef18571d37826b687dd141a0fe110f5814adaf9d1a391e7e482020d7f81df189ca89ec0dd141c1433d48eff4c6e53648b46f008dea8ad2dc574f35f1d4d79
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.1.4":
-  version: 1.1.9
-  resolution: "@lezer/python@npm:1.1.9"
+  version: 1.1.13
+  resolution: "@lezer/python@npm:1.1.13"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: cc7e712665f0b7990fd00ba798c2e377f8393d0034a85da33b370e256322d92f668f51b70aa91585ed165718bad60fba6e86203f877d537819874be2549ec31f
+  checksum: 43465f3289063e16caac9a109f61b8f810dd6a0e1043874df1b4d0f1cee5fba39cfd8c78fa2e507c0aa8f50cee8c48fe36df549ac1f959dae8d51c06e8ec0d0b
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@lezer/rust@npm:1.0.1"
+  version: 1.0.2
+  resolution: "@lezer/rust@npm:1.0.2"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 1e02fdf09206979e7d4f87b020589f410c4c5e452a7b7b0296f6772ce3571c1bd7ed37495fbeeecf3d4423000f2efdabd462ba8a949c2b351fd35550327a7613
+  checksum: fc5e97852b42beeb44a0ebe316dc64e3cc49ff481c22e3e67d6003fc4a5c257fcd94959cfcc76cd154fa172db9b3b4b28de5c09f10550d6e5f14869ddc274e5b
   languageName: node
   linkType: hard
 
 "@lezer/xml@npm:^1.0.0":
-  version: 1.0.3
-  resolution: "@lezer/xml@npm:1.0.3"
+  version: 1.0.5
+  resolution: "@lezer/xml@npm:1.0.5"
   dependencies:
+    "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: a4758859abcab3bc3f8680f79f7fb7dbbb6842c7d552888f95cc85a845450342a18731fbf49cbaec5f39970b9e5b96a66c8381eda036d3ebf7c952da5ddd7666
+  checksum: a0a077b9e455b03593b93a7fdff2a4eab2cb7b230c8e1b878a8bebe80184632b9cc75ca018f1f9e2acb3a26e1386f4777385ab6e87aea70ccf479cde5ca268ee
   languageName: node
   linkType: hard
 
 "@lumino/algorithm@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/algorithm@npm:2.0.1"
   checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
   languageName: node
   linkType: hard
 
-"@lumino/application@npm:^2.2.1":
-  version: 2.2.1
-  resolution: "@lumino/application@npm:2.2.1"
+"@lumino/application@npm:^2.3.0":
+  version: 2.3.1
+  resolution: "@lumino/application@npm:2.3.1"
   dependencies:
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
-    "@lumino/widgets": ^2.3.0
-  checksum: a33e661703728440bc7d2ddb4674261f4de0d20eb8c9846646cbd6debac03b5c65e78d739a500903550fd83b8f47b47fa82ec178c97bc9967ca3ac4014075cde
+    "@lumino/widgets": ^2.3.2
+  checksum: c112789d99baf62e5c2cee98834bc3efb5027bbca1aac81f10ea8855c0cd2538ec0a7c56c3f5dd42dce244e6892ef5bf8ef356f97e1cd4c161b99eb2068c195c
   languageName: node
   linkType: hard
 
 "@lumino/collections@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/collections@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: 8a29b7973a388a33c5beda0819dcd2dc2aad51a8406dcfd4581b055a9f77a39dc5800f7a8b4ae3c0bb97ae7b56a7a869e2560ffb7a920a28e93b477ba05907d6
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.1.3":
-  version: 2.1.3
-  resolution: "@lumino/commands@npm:2.1.3"
+"@lumino/commands@npm:^2.2.0, @lumino/commands@npm:^2.3.0":
+  version: 2.3.0
+  resolution: "@lumino/commands@npm:2.3.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/keyboard": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: e4e3ee279f2a5e8d68e4ce142c880333f5542f90c684972402356936ecb5cf5e07163800b59e7cb8c911cbdb4e5089edcc5dd2990bc8db10c87517268de1fc5d
+  checksum: a9b83bbfcc0421ff501e818dd234c65db438a8abb450628db0dea9ee05e8077d10b2275e7e2289f6df9c20dc26d2af458b1db88ccf43ec69f185eb207dbad419
   languageName: node
   linkType: hard
 
 "@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.2, @lumino/coreutils@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/coreutils@npm:2.1.2"
   checksum: 7865317ac0676b448d108eb57ab5d8b2a17c101995c0f7a7106662d9fe6c859570104525f83ee3cda12ae2e326803372206d6f4c1f415a5b59e4158a7b81066f
@@ -1539,21 +1327,21 @@
 "@lumino/domutils@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/domutils@npm:2.0.1"
   checksum: 61fa0ab226869dfbb763fc426790cf5a43b7d6f4cea1364c6dd56d61c44bff05eea188d33ff847449608ef58ed343161bee15c19b96f35410e4ee35815dc611a
   languageName: node
   linkType: hard
 
-"@lumino/dragdrop@npm:^2.1.3":
-  version: 2.1.3
-  resolution: "@lumino/dragdrop@npm:2.1.3"
+"@lumino/dragdrop@npm:^2.1.4":
+  version: 2.1.4
+  resolution: "@lumino/dragdrop@npm:2.1.4"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
-  checksum: d5f7eb4cc9f9a084cb9af10f02d6741b25d683350878ecbc324e24ba9d4b5246451a410e2ca5fff227aab1c191d1e73a2faf431f93e13111d67a4e426e126258
+  checksum: 43d82484b13b38b612e7dfb424a840ed6a38d0db778af10655c4ba235c67b5b12db1683929b35a36ab2845f77466066dfd1ee25c1c273e8e175677eba9dc560d
   languageName: node
   linkType: hard
 
 "@lumino/keyboard@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/keyboard@npm:2.0.1"
   checksum: cf33f13427a418efd7cc91061233321e860d5404f3d86397781028309bef86c8ad2d88276ffe335c1db0fe619bd9d1e60641c81f881696957a58703ee4652c3e
@@ -1603,30 +1391,77 @@
   resolution: "@lumino/virtualdom@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.3.0, @lumino/widgets@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "@lumino/widgets@npm:2.3.0"
+"@lumino/widgets@npm:^1.37.2 || ^2.3.1, @lumino/widgets@npm:^2.3.1, @lumino/widgets@npm:^2.3.2":
+  version: 2.3.2
+  resolution: "@lumino/widgets@npm:2.3.2"
   dependencies:
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.1.3
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
-    "@lumino/dragdrop": ^2.1.3
+    "@lumino/dragdrop": ^2.1.4
     "@lumino/keyboard": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: a8559bd3574b7fc16e7679e05994c515b0d3e78dada35786d161f67c639941d134e92ce31d95c2e4ac06709cdf83b0e7fb4b6414a3f7779579222a2fb525d025
+  checksum: 954fe066b0826cf00c019731bb3f70e635c63be4a0ce27f7573dbe6bd59e2154f511594b50e8f58f44877cf514084128c1e894ecbbbfd6e20d937e5cfb69ca8b
+  languageName: node
+  linkType: hard
+
+"@microsoft/fast-colors@npm:^5.3.1":
+  version: 5.3.1
+  resolution: "@microsoft/fast-colors@npm:5.3.1"
+  checksum: ff87f402faadb4b5aeee3d27762566c11807f927cd4012b8bbc7f073ca68de0e2197f95330ff5dfd7038f4b4f0e2f51b11feb64c5d570f5c598d37850a5daf60
+  languageName: node
+  linkType: hard
+
+"@microsoft/fast-element@npm:^1.12.0, @microsoft/fast-element@npm:^1.13.0":
+  version: 1.13.0
+  resolution: "@microsoft/fast-element@npm:1.13.0"
+  checksum: 1cb7b4cfb7531116a3542d3f59bf1dd35106194f5764205403590250aaff744de79e35a5a1f36b4941c4eda9edc088148d4d629fb80be15fdf25f6be01770f3a
+  languageName: node
+  linkType: hard
+
+"@microsoft/fast-foundation@npm:^2.49.4, @microsoft/fast-foundation@npm:^2.49.6":
+  version: 2.49.6
+  resolution: "@microsoft/fast-foundation@npm:2.49.6"
+  dependencies:
+    "@microsoft/fast-element": ^1.13.0
+    "@microsoft/fast-web-utilities": ^5.4.1
+    tabbable: ^5.2.0
+    tslib: ^1.13.0
+  checksum: 15fdf9dd0b910a72a9cff140f765d522304df11f8a78d5a97a815e2bbae25027c2b336e94f89ca31e650d6aabe17b590b7453acc0d2cb7340c219eb76350a942
+  languageName: node
+  linkType: hard
+
+"@microsoft/fast-react-wrapper@npm:^0.3.22":
+  version: 0.3.24
+  resolution: "@microsoft/fast-react-wrapper@npm:0.3.24"
+  dependencies:
+    "@microsoft/fast-element": ^1.13.0
+    "@microsoft/fast-foundation": ^2.49.6
+  peerDependencies:
+    react: ">=16.9.0"
+  checksum: 1d7a87509c22872bafc9b5c64f66659e52ba0cfdff484d7204125e503dafdea143f5e1bd2a643e2f3fbba6cc7567d916393369433f19dab9f0adcbe7a88b7d98
+  languageName: node
+  linkType: hard
+
+"@microsoft/fast-web-utilities@npm:^5.4.1":
+  version: 5.4.1
+  resolution: "@microsoft/fast-web-utilities@npm:5.4.1"
+  dependencies:
+    exenv-es6: ^1.1.1
+  checksum: 303e87847f962944f474e3716c3eb305668243916ca9e0719e26bb9a32346144bc958d915c103776b3e552cea0f0f6233f839fad66adfdf96a8436b947288ca7
   languageName: node
   linkType: hard
 
 "@nodelib/fs.scandir@npm:2.1.5":
   version: 2.1.5
   resolution: "@nodelib/fs.scandir@npm:2.1.5"
   dependencies:
@@ -1656,302 +1491,308 @@
 "@pkgjs/parseargs@npm:^0.11.0":
   version: 0.11.0
   resolution: "@pkgjs/parseargs@npm:0.11.0"
   checksum: 6ad6a00fc4f2f2cfc6bff76fb1d88b8ee20bc0601e18ebb01b6d4be583733a860239a521a7fbca73b612e66705078809483549d2b18f370eb346c5155c8e4a0f
   languageName: node
   linkType: hard
 
-"@pkgr/utils@npm:^2.3.1":
-  version: 2.4.2
-  resolution: "@pkgr/utils@npm:2.4.2"
-  dependencies:
-    cross-spawn: ^7.0.3
-    fast-glob: ^3.3.0
-    is-glob: ^4.0.3
-    open: ^9.1.0
-    picocolors: ^1.0.0
-    tslib: ^2.6.0
-  checksum: 24e04c121269317d259614cd32beea3af38277151c4002df5883c4be920b8e3490bb897748e844f9d46bf68230f86dabd4e8f093773130e7e60529a769a132fc
+"@pkgr/core@npm:^0.1.0":
+  version: 0.1.1
+  resolution: "@pkgr/core@npm:0.1.1"
+  checksum: 6f25fd2e3008f259c77207ac9915b02f1628420403b2630c92a07ff963129238c9262afc9e84344c7a23b5cc1f3965e2cd17e3798219f5fd78a63d144d3cceba
   languageName: node
   linkType: hard
 
-"@rjsf/core@npm:^5.1.0":
-  version: 5.13.0
-  resolution: "@rjsf/core@npm:5.13.0"
+"@rjsf/core@npm:^5.13.4":
+  version: 5.18.2
+  resolution: "@rjsf/core@npm:5.18.2"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
-    markdown-to-jsx: ^7.3.2
-    nanoid: ^3.3.6
+    markdown-to-jsx: ^7.4.1
+    nanoid: ^3.3.7
     prop-types: ^15.8.1
   peerDependencies:
-    "@rjsf/utils": ^5.12.x
+    "@rjsf/utils": ^5.18.x
     react: ^16.14.0 || >=17
-  checksum: d7d66d20fcdf310f4b152c22e1ac1ca8abe5f40b502711c9cabc4241b3252ec0e58345aa194529d2bdfb7a51b9f1179c9ddefc0cdc7fd9f94ad10c5e5b1032b8
+  checksum: b8b20bd75090b15b19e176aa766c037f3a7f1a27dbbde07ab095376a85e0027fd441b6e37355c8d3b389393db1f1b27699769034146040864c63a8f110d5e2d7
   languageName: node
   linkType: hard
 
-"@rjsf/utils@npm:^5.1.0":
-  version: 5.13.0
-  resolution: "@rjsf/utils@npm:5.13.0"
+"@rjsf/utils@npm:^5.13.4":
+  version: 5.18.2
+  resolution: "@rjsf/utils@npm:5.18.2"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 283e2b405eac2f4fdd243b2e35ade7e83a4bf7551eb5e075499e8eb5d3a3ae161e9c047bcf63d2e6fef7c6b2e7438f1a150f353b909df992e85194940c311f9b
+  checksum: 19342ce160f5f2ff1b1448bc61b0767c9b19a3c365fe3dca221c9178dff6b54123bdfe9dd4b0314aa7965011edb0e76029f7e76226936066bfacbaaa619546b4
+  languageName: node
+  linkType: hard
+
+"@types/create-react-class@npm:*":
+  version: 15.6.8
+  resolution: "@types/create-react-class@npm:15.6.8"
+  dependencies:
+    "@types/prop-types": "*"
+    "@types/react": "*"
+  checksum: a4237559499c77205c7e73269e53db6ada257e21a638f7222f20ffcd66d1a9c2ed1819ceca067a3edbdb47960d8a60ecd2c6de5a0cb9ed8e9de03e4ced144397
   languageName: node
   linkType: hard
 
 "@types/eslint-scope@npm:^3.7.3":
-  version: 3.7.4
-  resolution: "@types/eslint-scope@npm:3.7.4"
+  version: 3.7.7
+  resolution: "@types/eslint-scope@npm:3.7.7"
   dependencies:
     "@types/eslint": "*"
     "@types/estree": "*"
-  checksum: ea6a9363e92f301cd3888194469f9ec9d0021fe0a397a97a6dd689e7545c75de0bd2153dfb13d3ab532853a278b6572c6f678ce846980669e41029d205653460
+  checksum: e2889a124aaab0b89af1bab5959847c5bec09809209255de0e63b9f54c629a94781daa04adb66bffcdd742f5e25a17614fb933965093c0eea64aacda4309380e
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.44.2
-  resolution: "@types/eslint@npm:8.44.2"
+  version: 8.56.9
+  resolution: "@types/eslint@npm:8.56.9"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 25b3ef61bae96350026593c9914c8a61ee02fde48ab8d568a73ee45032f13c0028c62e47a5ff78715af488dfe8e8bba913f7d30f859f60c7f9e639d328e80482
+  checksum: c0c033fc724774b791bf97465cfe246814eda1f82460aff2daa64dfce1b1a01626c75f4281d2ab10dcd9176446df0b4bf57e8ac542da6476902e28683e89137d
   languageName: node
   linkType: hard
 
-"@types/estree@npm:*, @types/estree@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@types/estree@npm:1.0.1"
-  checksum: e9aa175eacb797216fafce4d41e8202c7a75555bc55232dee0f9903d7171f8f19f0ae7d5191bb1a88cb90e65468be508c0df850a9fb81b4433b293a5a749899d
+"@types/estree@npm:*, @types/estree@npm:^1.0.5":
+  version: 1.0.5
+  resolution: "@types/estree@npm:1.0.5"
+  checksum: dd8b5bed28e6213b7acd0fb665a84e693554d850b0df423ac8076cc3ad5823a6bc26b0251d080bdc545af83179ede51dd3f6fa78cad2c46ed1f29624ddf3e41a
   languageName: node
   linkType: hard
 
-"@types/json-schema@npm:*, @types/json-schema@npm:^7.0.11, @types/json-schema@npm:^7.0.12, @types/json-schema@npm:^7.0.5, @types/json-schema@npm:^7.0.8, @types/json-schema@npm:^7.0.9":
-  version: 7.0.13
-  resolution: "@types/json-schema@npm:7.0.13"
-  checksum: 345df21a678fa72fb389f35f33de77833d09d4a142bb2bcb27c18690efa4cf70fc2876e43843cefb3fbdb9fcb12cd3e970a90936df30f53bbee899865ff605ab
+"@types/json-schema@npm:*, @types/json-schema@npm:^7.0.12, @types/json-schema@npm:^7.0.15, @types/json-schema@npm:^7.0.5, @types/json-schema@npm:^7.0.8, @types/json-schema@npm:^7.0.9":
+  version: 7.0.15
+  resolution: "@types/json-schema@npm:7.0.15"
+  checksum: 97ed0cb44d4070aecea772b7b2e2ed971e10c81ec87dd4ecc160322ffa55ff330dace1793489540e3e318d90942064bb697cc0f8989391797792d919737b3b98
   languageName: node
   linkType: hard
 
 "@types/minimist@npm:^1.2.2":
-  version: 1.2.2
-  resolution: "@types/minimist@npm:1.2.2"
-  checksum: b8da83c66eb4aac0440e64674b19564d9d86c80ae273144db9681e5eeff66f238ade9515f5006ffbfa955ceff8b89ad2bd8ec577d7caee74ba101431fb07045d
+  version: 1.2.5
+  resolution: "@types/minimist@npm:1.2.5"
+  checksum: 477047b606005058ab0263c4f58097136268007f320003c348794f74adedc3166ffc47c80ec3e94687787f2ab7f4e72c468223946e79892cf0fd9e25e9970a90
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.6.3
-  resolution: "@types/node@npm:20.6.3"
-  checksum: 444a6f1f41cfa8d3e20ce0108e6e43960fb2ae0e481f233bb1c14d6252aa63a92e021de561cd317d9fdb411688f871065f40175a1f18763282dee2613a08f8a3
+  version: 20.12.7
+  resolution: "@types/node@npm:20.12.7"
+  dependencies:
+    undici-types: ~5.26.4
+  checksum: 7cc979f7e2ca9a339ec71318c3901b9978555257929ef3666987f3e447123bc6dc92afcc89f6347e09e07d602fde7d51bcddea626c23aa2bb74aeaacfd1e1686
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
-  version: 2.4.1
-  resolution: "@types/normalize-package-data@npm:2.4.1"
-  checksum: e87bccbf11f95035c89a132b52b79ce69a1e3652fe55962363063c9c0dae0fe2477ebc585e03a9652adc6f381d24ba5589cc5e51849df4ced3d3e004a7d40ed5
+  version: 2.4.4
+  resolution: "@types/normalize-package-data@npm:2.4.4"
+  checksum: 65dff72b543997b7be8b0265eca7ace0e34b75c3e5fee31de11179d08fa7124a7a5587265d53d0409532ecb7f7fba662c2012807963e1f9b059653ec2c83ee05
   languageName: node
   linkType: hard
 
 "@types/prop-types@npm:*":
-  version: 15.7.6
-  resolution: "@types/prop-types@npm:15.7.6"
-  checksum: 5f2796c7330461a556c4d18035fb914b372f96b1619a4f8302d07e1ea708e06a2dbe666dfcd8ff03f64c625aa4c12b31f677d0298a32910f5ab7ee51521d8086
+  version: 15.7.12
+  resolution: "@types/prop-types@npm:15.7.12"
+  checksum: ac16cc3d0a84431ffa5cfdf89579ad1e2269549f32ce0c769321fdd078f84db4fbe1b461ed5a1a496caf09e637c0e367d600c541435716a55b1d9713f5035dfe
   languageName: node
   linkType: hard
 
-"@types/react-addons-linked-state-mixin@npm:^0.14.22":
-  version: 0.14.22
-  resolution: "@types/react-addons-linked-state-mixin@npm:0.14.22"
+"@types/react-addons-linked-state-mixin@npm:^0.14.27":
+  version: 0.14.27
+  resolution: "@types/react-addons-linked-state-mixin@npm:0.14.27"
   dependencies:
+    "@types/create-react-class": "*"
     "@types/react": "*"
-  checksum: f0216424eed2008845acdca7565d661ed67310cf16179da7cdc97056070552f77bb7bad6d5beb3598a46b7322dfa29e29945259d834d529c3d68c75afea9a8dc
+  checksum: a78007698a236335a50c74ddd27669028213ff363219f97a6ea1f000ddb8714c83838002ea07c33024f964112a229e447127b457fa3f9b3db352dd41d6b8d328
   languageName: node
   linkType: hard
 
-"@types/react@npm:*, @types/react@npm:^18.0.26":
-  version: 18.2.22
-  resolution: "@types/react@npm:18.2.22"
+"@types/react@npm:*, @types/react@npm:^18.0.26, @types/react@npm:^18.2.79":
+  version: 18.2.79
+  resolution: "@types/react@npm:18.2.79"
   dependencies:
     "@types/prop-types": "*"
-    "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: 44289523dabaadcd3fd85689abb98f9ebcc8492d7e978348d1c986138acef4801030b279e89a19e38a6319e294bcea77559e37e0c803e4bacf2b8ae3a56ba587
-  languageName: node
-  linkType: hard
-
-"@types/scheduler@npm:*":
-  version: 0.16.3
-  resolution: "@types/scheduler@npm:0.16.3"
-  checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
+  checksum: 85aa96e0e88725c84d8fc5f04f10a4da6a1f507dde33557ac9cc211414756867721264bfefd9e02bae1288ce2905351d949b652b931e734ea24519ee5c625138
   languageName: node
   linkType: hard
 
 "@types/semver@npm:^7.5.0":
-  version: 7.5.2
-  resolution: "@types/semver@npm:7.5.2"
-  checksum: 743aa8a2b58e20b329c19bd2459152cb049d12fafab7279b90ac11e0f268c97efbcb606ea0c681cca03f79015381b40d9b1244349b354270bec3f939ed49f6e9
+  version: 7.5.8
+  resolution: "@types/semver@npm:7.5.8"
+  checksum: ea6f5276f5b84c55921785a3a27a3cd37afee0111dfe2bcb3e03c31819c197c782598f17f0b150a69d453c9584cd14c4c4d7b9a55d2c5e6cacd4d66fdb3b3663
   languageName: node
   linkType: hard
 
 "@types/source-list-map@npm:*":
-  version: 0.1.2
-  resolution: "@types/source-list-map@npm:0.1.2"
-  checksum: fda8f37537aca9d3ed860d559289ab1dddb6897e642e6f53e909bbd18a7ac3129a8faa2a7d093847c91346cf09c86ef36e350c715406fba1f2271759b449adf6
+  version: 0.1.6
+  resolution: "@types/source-list-map@npm:0.1.6"
+  checksum: 9cd294c121f1562062de5d241fe4d10780b1131b01c57434845fe50968e9dcf67ede444591c2b1ad6d3f9b6bc646ac02cc8f51a3577c795f9c64cf4573dcc6b1
   languageName: node
   linkType: hard
 
 "@types/webpack-sources@npm:^0.1.5":
-  version: 0.1.9
-  resolution: "@types/webpack-sources@npm:0.1.9"
+  version: 0.1.12
+  resolution: "@types/webpack-sources@npm:0.1.12"
   dependencies:
     "@types/node": "*"
     "@types/source-list-map": "*"
     source-map: ^0.6.1
-  checksum: bc09c584c7047e8aed29801a3981787dee3898e9e7a99891a362df114fcac3879eea5a00932314866a01b25220391839be09fe1487b16d4970ff4a7afd5b9725
+  checksum: 75342659a9889478969f7bb7360b998aa084ba11ab523c172ded6a807dac43ab2a9e1212078ef8bbf0f33e4fadd2c8a91b75d38184d8030d96a32fe819c9bb57
   languageName: node
   linkType: hard
 
-"@typescript-eslint/eslint-plugin@npm:^6.1.0":
-  version: 6.7.2
-  resolution: "@typescript-eslint/eslint-plugin@npm:6.7.2"
+"@typescript-eslint/eslint-plugin@npm:^6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/eslint-plugin@npm:6.21.0"
   dependencies:
     "@eslint-community/regexpp": ^4.5.1
-    "@typescript-eslint/scope-manager": 6.7.2
-    "@typescript-eslint/type-utils": 6.7.2
-    "@typescript-eslint/utils": 6.7.2
-    "@typescript-eslint/visitor-keys": 6.7.2
+    "@typescript-eslint/scope-manager": 6.21.0
+    "@typescript-eslint/type-utils": 6.21.0
+    "@typescript-eslint/utils": 6.21.0
+    "@typescript-eslint/visitor-keys": 6.21.0
     debug: ^4.3.4
     graphemer: ^1.4.0
     ignore: ^5.2.4
     natural-compare: ^1.4.0
     semver: ^7.5.4
     ts-api-utils: ^1.0.1
   peerDependencies:
     "@typescript-eslint/parser": ^6.0.0 || ^6.0.0-alpha
     eslint: ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: 4d6f612619282a20518cd6581bce16cd7c50ac4e49f5eeca2ab916a923049379aa382817568c929216381fb2c1bfbc1c4e6fde16ac8bfdd63862a9126f0ab797
+  checksum: 5ef2c502255e643e98051e87eb682c2a257e87afd8ec3b9f6274277615e1c2caf3131b352244cfb1987b8b2c415645eeacb9113fa841fc4c9b2ac46e8aed6efd
   languageName: node
   linkType: hard
 
-"@typescript-eslint/parser@npm:^6.1.0":
-  version: 6.7.2
-  resolution: "@typescript-eslint/parser@npm:6.7.2"
+"@typescript-eslint/parser@npm:^6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/parser@npm:6.21.0"
   dependencies:
-    "@typescript-eslint/scope-manager": 6.7.2
-    "@typescript-eslint/types": 6.7.2
-    "@typescript-eslint/typescript-estree": 6.7.2
-    "@typescript-eslint/visitor-keys": 6.7.2
+    "@typescript-eslint/scope-manager": 6.21.0
+    "@typescript-eslint/types": 6.21.0
+    "@typescript-eslint/typescript-estree": 6.21.0
+    "@typescript-eslint/visitor-keys": 6.21.0
     debug: ^4.3.4
   peerDependencies:
     eslint: ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: 9e93d3eb432ed5457a852e25a31782d07518f728966cd477620175ae64db9be04f5d8e605f3561dbfe9a365f209a83b2a3788efb9b3cf33669c8bca17f1bcf6f
+  checksum: 162fe3a867eeeffda7328bce32dae45b52283c68c8cb23258fb9f44971f761991af61f71b8c9fe1aa389e93dfe6386f8509c1273d870736c507d76dd40647b68
   languageName: node
   linkType: hard
 
-"@typescript-eslint/scope-manager@npm:6.7.2":
-  version: 6.7.2
-  resolution: "@typescript-eslint/scope-manager@npm:6.7.2"
+"@typescript-eslint/scope-manager@npm:6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/scope-manager@npm:6.21.0"
   dependencies:
-    "@typescript-eslint/types": 6.7.2
-    "@typescript-eslint/visitor-keys": 6.7.2
-  checksum: e35fa23ecb16252c3ad00b5f1ec05d9b8d33ee30d4c57543892f900443ed77926be9bd2836f06463c31b483f5f0f79070273bc51c4a606f55ac3cd1d9c9cd542
+    "@typescript-eslint/types": 6.21.0
+    "@typescript-eslint/visitor-keys": 6.21.0
+  checksum: 71028b757da9694528c4c3294a96cc80bc7d396e383a405eab3bc224cda7341b88e0fc292120b35d3f31f47beac69f7083196c70616434072fbcd3d3e62d3376
   languageName: node
   linkType: hard
 
-"@typescript-eslint/type-utils@npm:6.7.2":
-  version: 6.7.2
-  resolution: "@typescript-eslint/type-utils@npm:6.7.2"
+"@typescript-eslint/type-utils@npm:6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/type-utils@npm:6.21.0"
   dependencies:
-    "@typescript-eslint/typescript-estree": 6.7.2
-    "@typescript-eslint/utils": 6.7.2
+    "@typescript-eslint/typescript-estree": 6.21.0
+    "@typescript-eslint/utils": 6.21.0
     debug: ^4.3.4
     ts-api-utils: ^1.0.1
   peerDependencies:
     eslint: ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: 67743f8e4b77d0ab3d82907eda0411ffd221357b60ac9cbd29683d5b8c77127369ebfafcf0bfc30a1f1828927ccd5635fab5b2eaf2b2f1d12a9361549cab3e62
+  checksum: 77025473f4d80acf1fafcce99c5c283e557686a61861febeba9c9913331f8a41e930bf5cd8b7a54db502a57b6eb8ea6d155cbd4f41349ed00e3d7aeb1f477ddc
   languageName: node
   linkType: hard
 
-"@typescript-eslint/types@npm:6.7.2":
-  version: 6.7.2
-  resolution: "@typescript-eslint/types@npm:6.7.2"
-  checksum: 5a7c4cd456f721649757d2edb4cae71d1405c1c2c35672031f012b27007b9d49b7118297eec746dc3351370e6aa414e5d2c493fb658c7b910154b7998c0278e1
+"@typescript-eslint/types@npm:6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/types@npm:6.21.0"
+  checksum: 9501b47d7403417af95fc1fb72b2038c5ac46feac0e1598a46bcb43e56a606c387e9dcd8a2a0abe174c91b509f2d2a8078b093786219eb9a01ab2fbf9ee7b684
   languageName: node
   linkType: hard
 
-"@typescript-eslint/typescript-estree@npm:6.7.2":
-  version: 6.7.2
-  resolution: "@typescript-eslint/typescript-estree@npm:6.7.2"
+"@typescript-eslint/typescript-estree@npm:6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/typescript-estree@npm:6.21.0"
   dependencies:
-    "@typescript-eslint/types": 6.7.2
-    "@typescript-eslint/visitor-keys": 6.7.2
+    "@typescript-eslint/types": 6.21.0
+    "@typescript-eslint/visitor-keys": 6.21.0
     debug: ^4.3.4
     globby: ^11.1.0
     is-glob: ^4.0.3
+    minimatch: 9.0.3
     semver: ^7.5.4
     ts-api-utils: ^1.0.1
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: c30b9803567c37527e2806badd98f3083ae125db9a430d8a28647b153e446e6a4b830833f229cca27d5aa0ff5497c149aaa524aa3a6dbf932b557c60d0bfd4f9
+  checksum: dec02dc107c4a541e14fb0c96148f3764b92117c3b635db3a577b5a56fc48df7a556fa853fb82b07c0663b4bf2c484c9f245c28ba3e17e5cb0918ea4cab2ea21
   languageName: node
   linkType: hard
 
-"@typescript-eslint/utils@npm:6.7.2":
-  version: 6.7.2
-  resolution: "@typescript-eslint/utils@npm:6.7.2"
+"@typescript-eslint/utils@npm:6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/utils@npm:6.21.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.4.0
     "@types/json-schema": ^7.0.12
     "@types/semver": ^7.5.0
-    "@typescript-eslint/scope-manager": 6.7.2
-    "@typescript-eslint/types": 6.7.2
-    "@typescript-eslint/typescript-estree": 6.7.2
+    "@typescript-eslint/scope-manager": 6.21.0
+    "@typescript-eslint/types": 6.21.0
+    "@typescript-eslint/typescript-estree": 6.21.0
     semver: ^7.5.4
   peerDependencies:
     eslint: ^7.0.0 || ^8.0.0
-  checksum: 97f950562dba2bda63ffe64672f643ef940123cf74007bc878afcf31c75f905c99934a3ad77da3d5a4fe7807d5d69c791b20c429712ad5a5525e331ebc313756
+  checksum: b129b3a4aebec8468259f4589985cb59ea808afbfdb9c54f02fad11e17d185e2bf72bb332f7c36ec3c09b31f18fc41368678b076323e6e019d06f74ee93f7bf2
   languageName: node
   linkType: hard
 
-"@typescript-eslint/visitor-keys@npm:6.7.2":
-  version: 6.7.2
-  resolution: "@typescript-eslint/visitor-keys@npm:6.7.2"
+"@typescript-eslint/visitor-keys@npm:6.21.0":
+  version: 6.21.0
+  resolution: "@typescript-eslint/visitor-keys@npm:6.21.0"
   dependencies:
-    "@typescript-eslint/types": 6.7.2
+    "@typescript-eslint/types": 6.21.0
     eslint-visitor-keys: ^3.4.1
-  checksum: b4915fbc0f3d44c81b92b7151830b698e8b6ed2dee8587bb65540c888c7a84300d3fd6b0c159e2131c7c6df1bebe49fb0d21c347ecdbf7f3e4aec05acebbb0bc
+  checksum: 67c7e6003d5af042d8703d11538fca9d76899f0119130b373402819ae43f0bc90d18656aa7add25a24427ccf1a0efd0804157ba83b0d4e145f06107d7d1b7433
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/ast@npm:1.11.6"
+"@ungap/structured-clone@npm:^1.2.0":
+  version: 1.2.0
+  resolution: "@ungap/structured-clone@npm:1.2.0"
+  checksum: 4f656b7b4672f2ce6e272f2427d8b0824ed11546a601d8d5412b9d7704e83db38a8d9f402ecdf2b9063fc164af842ad0ec4a55819f621ed7e7ea4d1efcc74524
+  languageName: node
+  linkType: hard
+
+"@webassemblyjs/ast@npm:1.12.1, @webassemblyjs/ast@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/ast@npm:1.12.1"
   dependencies:
     "@webassemblyjs/helper-numbers": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-  checksum: 38ef1b526ca47c210f30975b06df2faf1a8170b1636ce239fc5738fc231ce28389dd61ecedd1bacfc03cbe95b16d1af848c805652080cb60982836eb4ed2c6cf
+  checksum: 31bcc64147236bd7b1b6d29d1f419c1f5845c785e1e42dc9e3f8ca2e05a029e9393a271b84f3a5bff2a32d35f51ff59e2181a6e5f953fe88576acd6750506202
   languageName: node
   linkType: hard
 
 "@webassemblyjs/floating-point-hex-parser@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.6"
   checksum: 29b08758841fd8b299c7152eda36b9eb4921e9c584eb4594437b5cd90ed6b920523606eae7316175f89c20628da14326801090167cc7fbffc77af448ac84b7e2
@@ -1961,18 +1802,18 @@
 "@webassemblyjs/helper-api-error@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-api-error@npm:1.11.6"
   checksum: e8563df85161096343008f9161adb138a6e8f3c2cc338d6a36011aa55eabb32f2fd138ffe63bc278d009ada001cc41d263dadd1c0be01be6c2ed99076103689f
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-buffer@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/helper-buffer@npm:1.11.6"
-  checksum: b14d0573bf680d22b2522e8a341ec451fddd645d1f9c6bd9012ccb7e587a2973b86ab7b89fe91e1c79939ba96095f503af04369a3b356c8023c13a5893221644
+"@webassemblyjs/helper-buffer@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/helper-buffer@npm:1.12.1"
+  checksum: c3ffb723024130308db608e86e2bdccd4868bbb62dffb0a9a1530606496f79c87f8565bd8e02805ce64912b71f1a70ee5fb00307258b0c082c3abf961d097eca
   languageName: node
   linkType: hard
 
 "@webassemblyjs/helper-numbers@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-numbers@npm:1.11.6"
   dependencies:
@@ -1986,23 +1827,23 @@
 "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6"
   checksum: 3535ef4f1fba38de3475e383b3980f4bbf3de72bbb631c2b6584c7df45be4eccd62c6ff48b5edd3f1bcff275cfd605a37679ec199fc91fd0a7705d7f1e3972dc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-section@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.6"
+"@webassemblyjs/helper-wasm-section@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/helper-wasm-section@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-  checksum: b2cf751bf4552b5b9999d27bbb7692d0aca75260140195cb58ea6374d7b9c2dc69b61e10b211a0e773f66209c3ddd612137ed66097e3684d7816f854997682e9
+    "@webassemblyjs/wasm-gen": 1.12.1
+  checksum: c19810cdd2c90ff574139b6d8c0dda254d42d168a9e5b3d353d1bc085f1d7164ccd1b3c05592a45a939c47f7e403dc8d03572bb686642f06a3d02932f6f0bc8f
   languageName: node
   linkType: hard
 
 "@webassemblyjs/ieee754@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/ieee754@npm:1.11.6"
   dependencies:
@@ -2023,76 +1864,76 @@
 "@webassemblyjs/utf8@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/utf8@npm:1.11.6"
   checksum: 807fe5b5ce10c390cfdd93e0fb92abda8aebabb5199980681e7c3743ee3306a75729bcd1e56a3903980e96c885ee53ef901fcbaac8efdfa480f9c0dae1d08713
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-edit@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-edit@npm:1.11.6"
+"@webassemblyjs/wasm-edit@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-edit@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-    "@webassemblyjs/helper-wasm-section": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-    "@webassemblyjs/wasm-opt": 1.11.6
-    "@webassemblyjs/wasm-parser": 1.11.6
-    "@webassemblyjs/wast-printer": 1.11.6
-  checksum: 29ce75870496d6fad864d815ebb072395a8a3a04dc9c3f4e1ffdc63fc5fa58b1f34304a1117296d8240054cfdbc38aca88e71fb51483cf29ffab0a61ef27b481
+    "@webassemblyjs/helper-wasm-section": 1.12.1
+    "@webassemblyjs/wasm-gen": 1.12.1
+    "@webassemblyjs/wasm-opt": 1.12.1
+    "@webassemblyjs/wasm-parser": 1.12.1
+    "@webassemblyjs/wast-printer": 1.12.1
+  checksum: ae23642303f030af888d30c4ef37b08dfec7eab6851a9575a616e65d1219f880d9223913a39056dd654e49049d76e97555b285d1f7e56935047abf578cce0692
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-gen@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-gen@npm:1.11.6"
+"@webassemblyjs/wasm-gen@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-gen@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
-  checksum: a645a2eecbea24833c3260a249704a7f554ef4a94c6000984728e94bb2bc9140a68dfd6fd21d5e0bbb09f6dfc98e083a45760a83ae0417b41a0196ff6d45a23a
+  checksum: 5787626bb7f0b033044471ddd00ce0c9fe1ee4584e8b73e232051e3a4c99ba1a102700d75337151c8b6055bae77eefa4548960c610a5e4a504e356bd872138ff
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-opt@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-opt@npm:1.11.6"
+"@webassemblyjs/wasm-opt@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-opt@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-    "@webassemblyjs/wasm-parser": 1.11.6
-  checksum: b4557f195487f8e97336ddf79f7bef40d788239169aac707f6eaa2fa5fe243557c2d74e550a8e57f2788e70c7ae4e7d32f7be16101afe183d597b747a3bdd528
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
+    "@webassemblyjs/wasm-gen": 1.12.1
+    "@webassemblyjs/wasm-parser": 1.12.1
+  checksum: 0e8fa8a0645304a1e18ff40d3db5a2e9233ebaa169b19fcc651d6fc9fe2cac0ce092ddee927318015ae735d9cd9c5d97c0cafb6a51dcd2932ac73587b62df991
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-parser@npm:1.11.6, @webassemblyjs/wasm-parser@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-parser@npm:1.11.6"
+"@webassemblyjs/wasm-parser@npm:1.12.1, @webassemblyjs/wasm-parser@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-parser@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@webassemblyjs/helper-api-error": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
-  checksum: 8200a8d77c15621724a23fdabe58d5571415cda98a7058f542e670ea965dd75499f5e34a48675184947c66f3df23adf55df060312e6d72d57908e3f049620d8a
+  checksum: 176015de3551ac068cd4505d837414f258d9ade7442bd71efb1232fa26c9f6d7d4e11a5c816caeed389943f409af7ebff6899289a992d7a70343cb47009d21a8
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wast-printer@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wast-printer@npm:1.11.6"
+"@webassemblyjs/wast-printer@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wast-printer@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@xtuc/long": 4.2.2
-  checksum: d2fa6a4c427325ec81463e9c809aa6572af6d47f619f3091bf4c4a6fc34f1da3df7caddaac50b8e7a457f8784c62cd58c6311b6cb69b0162ccd8d4c072f79cf8
+  checksum: 2974b5dda8d769145ba0efd886ea94a601e61fb37114c14f9a9a7606afc23456799af652ac3052f284909bd42edc3665a76bc9b50f95f0794c053a8a1757b713
   languageName: node
   linkType: hard
 
 "@webpack-cli/configtest@npm:^2.1.1":
   version: 2.1.1
   resolution: "@webpack-cli/configtest@npm:2.1.1"
   peerDependencies:
@@ -2161,19 +2002,19 @@
   peerDependencies:
     acorn: ^6.0.0 || ^7.0.0 || ^8.0.0
   checksum: c3d3b2a89c9a056b205b69530a37b972b404ee46ec8e5b341666f9513d3163e2a4f214a71f4dfc7370f5a9c07472d2fd1c11c91c3f03d093e37637d95da98950
   languageName: node
   linkType: hard
 
 "acorn@npm:^8.7.1, acorn@npm:^8.8.2, acorn@npm:^8.9.0":
-  version: 8.10.0
-  resolution: "acorn@npm:8.10.0"
+  version: 8.11.3
+  resolution: "acorn@npm:8.11.3"
   bin:
     acorn: bin/acorn
-  checksum: 538ba38af0cc9e5ef983aee196c4b8b4d87c0c94532334fa7e065b2c8a1f85863467bb774231aae91613fcda5e68740c15d97b1967ae3394d20faddddd8af61d
+  checksum: 76d8e7d559512566b43ab4aadc374f11f563f0a9e21626dd59cb2888444e9445923ae9f3699972767f18af61df89cd89f5eaaf772d1327b055b45cb829b4a88c
   languageName: node
   linkType: hard
 
 "ajv-formats@npm:^2.1.1":
   version: 2.1.1
   resolution: "ajv-formats@npm:2.1.1"
   dependencies:
@@ -2273,43 +2114,44 @@
 "argparse@npm:^2.0.1":
   version: 2.0.1
   resolution: "argparse@npm:2.0.1"
   checksum: 83644b56493e89a254bae05702abf3a1101b4fa4d0ca31df1c9985275a5a5bd47b3c27b7fa0b71098d41114d8ca000e6ed90cad764b306f8a503665e4d517ced
   languageName: node
   linkType: hard
 
-"array-buffer-byte-length@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "array-buffer-byte-length@npm:1.0.0"
+"array-buffer-byte-length@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "array-buffer-byte-length@npm:1.0.1"
   dependencies:
-    call-bind: ^1.0.2
-    is-array-buffer: ^3.0.1
-  checksum: 044e101ce150f4804ad19c51d6c4d4cfa505c5b2577bd179256e4aa3f3f6a0a5e9874c78cd428ee566ac574c8a04d7ce21af9fe52e844abfdccb82b33035a7c3
+    call-bind: ^1.0.5
+    is-array-buffer: ^3.0.4
+  checksum: 53524e08f40867f6a9f35318fafe467c32e45e9c682ba67b11943e167344d2febc0f6977a17e699b05699e805c3e8f073d876f8bbf1b559ed494ad2cd0fae09e
   languageName: node
   linkType: hard
 
 "array-union@npm:^2.1.0":
   version: 2.1.0
   resolution: "array-union@npm:2.1.0"
   checksum: 5bee12395cba82da674931df6d0fea23c4aa4660cb3b338ced9f828782a65caa232573e6bf3968f23e0c5eb301764a382cef2f128b170a9dc59de0e36c39f98d
   languageName: node
   linkType: hard
 
-"arraybuffer.prototype.slice@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "arraybuffer.prototype.slice@npm:1.0.2"
+"arraybuffer.prototype.slice@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "arraybuffer.prototype.slice@npm:1.0.3"
   dependencies:
-    array-buffer-byte-length: ^1.0.0
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-    get-intrinsic: ^1.2.1
-    is-array-buffer: ^3.0.2
+    array-buffer-byte-length: ^1.0.1
+    call-bind: ^1.0.5
+    define-properties: ^1.2.1
+    es-abstract: ^1.22.3
+    es-errors: ^1.2.1
+    get-intrinsic: ^1.2.3
+    is-array-buffer: ^3.0.4
     is-shared-array-buffer: ^1.0.2
-  checksum: c200faf437786f5b2c80d4564ff5481c886a16dee642ef02abdc7306c7edd523d1f01d1dd12b769c7eb42ac9bc53874510db19a92a2c035c0f6696172aafa5d3
+  checksum: 352259cba534dcdd969c92ab002efd2ba5025b2e3b9bead3973150edbdf0696c629d7f4b3f061c5931511e8207bdc2306da614703c820b45dabce39e3daf7e3e
   languageName: node
   linkType: hard
 
 "arrify@npm:^1.0.1":
   version: 1.0.1
   resolution: "arrify@npm:1.0.1"
   checksum: 745075dd4a4624ff0225c331dacb99be501a515d39bcb7c84d24660314a6ec28e68131b137e6f7e16318170842ce97538cd298fc4cd6b2cc798e0b957f2747e7
@@ -2319,18 +2161,20 @@
 "astral-regex@npm:^2.0.0":
   version: 2.0.0
   resolution: "astral-regex@npm:2.0.0"
   checksum: 876231688c66400473ba505731df37ea436e574dd524520294cc3bbc54ea40334865e01fa0d074d74d036ee874ee7e62f486ea38bc421ee8e6a871c06f011766
   languageName: node
   linkType: hard
 
-"available-typed-arrays@npm:^1.0.5":
-  version: 1.0.5
-  resolution: "available-typed-arrays@npm:1.0.5"
-  checksum: 20eb47b3cefd7db027b9bbb993c658abd36d4edd3fe1060e83699a03ee275b0c9b216cc076ff3f2db29073225fb70e7613987af14269ac1fe2a19803ccc97f1a
+"available-typed-arrays@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "available-typed-arrays@npm:1.0.7"
+  dependencies:
+    possible-typed-array-names: ^1.0.0
+  checksum: 1aa3ffbfe6578276996de660848b6e95669d9a95ad149e3dd0c0cda77db6ee1dbd9d1dd723b65b6d277b882dd0c4b91a654ae9d3cf9e1254b7e93e4908d78fd3
   languageName: node
   linkType: hard
 
 "balanced-match@npm:^1.0.0":
   version: 1.0.2
   resolution: "balanced-match@npm:1.0.2"
   checksum: 9706c088a283058a8a99e0bf91b0a2f75497f185980d9ffa8b304de1d9e58ebda7c72c07ebf01dadedaac5b2907b2c6f566f660d62bd336c3468e960403b9d65
@@ -2340,37 +2184,21 @@
 "balanced-match@npm:^2.0.0":
   version: 2.0.0
   resolution: "balanced-match@npm:2.0.0"
   checksum: 9a5caad6a292c5df164cc6d0c38e0eedf9a1413f42e5fece733640949d74d0052cfa9587c1a1681f772147fb79be495121325a649526957fd75b3a216d1fbc68
   languageName: node
   linkType: hard
 
-"big-integer@npm:^1.6.44":
-  version: 1.6.51
-  resolution: "big-integer@npm:1.6.51"
-  checksum: 3d444173d1b2e20747e2c175568bedeebd8315b0637ea95d75fd27830d3b8e8ba36c6af40374f36bdaea7b5de376dcada1b07587cb2a79a928fccdb6e6e3c518
-  languageName: node
-  linkType: hard
-
 "big.js@npm:^5.2.2":
   version: 5.2.2
   resolution: "big.js@npm:5.2.2"
   checksum: b89b6e8419b097a8fb4ed2399a1931a68c612bce3cfd5ca8c214b2d017531191070f990598de2fc6f3f993d91c0f08aa82697717f6b3b8732c9731866d233c9e
   languageName: node
   linkType: hard
 
-"bplist-parser@npm:^0.2.0":
-  version: 0.2.0
-  resolution: "bplist-parser@npm:0.2.0"
-  dependencies:
-    big-integer: ^1.6.44
-  checksum: d5339dd16afc51de6c88f88f58a45b72ed6a06aa31f5557d09877575f220b7c1d3fbe375da0b62e6a10d4b8ed80523567e351f24014f5bc886ad523758142cdd
-  languageName: node
-  linkType: hard
-
 "brace-expansion@npm:^1.1.7":
   version: 1.1.11
   resolution: "brace-expansion@npm:1.1.11"
   dependencies:
     balanced-match: ^1.0.0
     concat-map: 0.0.1
   checksum: faf34a7bb0c3fcf4b59c7808bc5d2a96a40988addf2e7e09dfbb67a2251800e0d14cd2bfc1aa79174f2f5095c54ff27f46fb1289fe2d77dac755b5eb3434cc07
@@ -2391,51 +2219,45 @@
   resolution: "braces@npm:3.0.2"
   dependencies:
     fill-range: ^7.0.1
   checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
   languageName: node
   linkType: hard
 
-"browserslist@npm:^4.14.5":
-  version: 4.21.11
-  resolution: "browserslist@npm:4.21.11"
-  dependencies:
-    caniuse-lite: ^1.0.30001538
-    electron-to-chromium: ^1.4.526
-    node-releases: ^2.0.13
+"browserslist@npm:^4.21.10":
+  version: 4.23.0
+  resolution: "browserslist@npm:4.23.0"
+  dependencies:
+    caniuse-lite: ^1.0.30001587
+    electron-to-chromium: ^1.4.668
+    node-releases: ^2.0.14
     update-browserslist-db: ^1.0.13
   bin:
     browserslist: cli.js
-  checksum: 89377745428d32c7bbec37055bc4b9e48aa859418ea3886b13218d825f8ea3053640f90d8652844ae855941fec0bffd2d69cf933035d6f9224b427d48d31eddf
+  checksum: 436f49e796782ca751ebab7edc010cfc9c29f68536f387666cd70ea22f7105563f04dd62c6ff89cb24cc3254d17cba385f979eeeb3484d43e012412ff7e75def
   languageName: node
   linkType: hard
 
 "buffer-from@npm:^1.0.0":
   version: 1.1.2
   resolution: "buffer-from@npm:1.1.2"
   checksum: 0448524a562b37d4d7ed9efd91685a5b77a50672c556ea254ac9a6d30e3403a517d8981f10e565db24e8339413b43c97ca2951f10e399c6125a0d8911f5679bb
   languageName: node
   linkType: hard
 
-"bundle-name@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "bundle-name@npm:3.0.0"
-  dependencies:
-    run-applescript: ^5.0.0
-  checksum: edf2b1fbe6096ed32e7566947ace2ea937ee427391744d7510a2880c4b9a5b3543d3f6c551236a29e5c87d3195f8e2912516290e638c15bcbede7b37cc375615
-  languageName: node
-  linkType: hard
-
-"call-bind@npm:^1.0.0, call-bind@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "call-bind@npm:1.0.2"
+"call-bind@npm:^1.0.2, call-bind@npm:^1.0.5, call-bind@npm:^1.0.6, call-bind@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "call-bind@npm:1.0.7"
   dependencies:
-    function-bind: ^1.1.1
-    get-intrinsic: ^1.0.2
-  checksum: f8e31de9d19988a4b80f3e704788c4a2d6b6f3d17cfec4f57dc29ced450c53a49270dc66bf0fbd693329ee948dd33e6c90a329519aef17474a4d961e8d6426b0
+    es-define-property: ^1.0.0
+    es-errors: ^1.3.0
+    function-bind: ^1.1.2
+    get-intrinsic: ^1.2.4
+    set-function-length: ^1.2.1
+  checksum: 295c0c62b90dd6522e6db3b0ab1ce26bdf9e7404215bda13cfee25b626b5ff1a7761324d58d38b1ef1607fc65aca2d06e44d2e18d0dfc6c14b465b00d8660029
   languageName: node
   linkType: hard
 
 "callsites@npm:^3.0.0":
   version: 3.1.0
   resolution: "callsites@npm:3.1.0"
   checksum: 072d17b6abb459c2ba96598918b55868af677154bec7e73d222ef95a8fdb9bbf7dae96a8421085cdad8cd190d86653b5b6dc55a4484f2e5b2e27d5e0c3fc15b3
@@ -2457,18 +2279,18 @@
 "camelcase@npm:^6.3.0":
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
-"caniuse-lite@npm:^1.0.30001538":
-  version: 1.0.30001538
-  resolution: "caniuse-lite@npm:1.0.30001538"
-  checksum: 94c5d55757a339c7cc175f08a024671e2b4e7c04f130b1015793303d637061347efb6ad84447c3b8137333e742d150b8ad9672716bbf2482646c2e63a56f6c55
+"caniuse-lite@npm:^1.0.30001587":
+  version: 1.0.30001611
+  resolution: "caniuse-lite@npm:1.0.30001611"
+  checksum: c5beb4a0aaabe24b01a577122c61e20ca0614d2e3adfd2e4de8dbdb8529eb9dba9922be8fd8be9eba48b6cadaada0b338aa3e0d0a17f42f6b3e9a614492c029a
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.3.0, chalk@npm:^2.4.1, chalk@npm:^2.4.2":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -2648,36 +2470,42 @@
     path-key: ^3.1.0
     shebang-command: ^2.0.0
     which: ^2.0.1
   checksum: 671cc7c7288c3a8406f3c69a3ae2fc85555c04169e9d611def9a675635472614f1c0ed0ef80955d5b6d4e724f6ced67f0ad1bb006c2ea643488fcfef994d7f52
   languageName: node
   linkType: hard
 
-"css-functions-list@npm:^3.2.0":
-  version: 3.2.0
-  resolution: "css-functions-list@npm:3.2.0"
-  checksum: fe912ea852fad500aef9a4f04db9a0371c7b0eb1ac1a45fbd8df0156ae0538cee7492ebd620b9bb502fe5bf2b5ed3bf3c16b6659cf67c7144eff0b597bcc3891
+"css-functions-list@npm:^3.2.1":
+  version: 3.2.1
+  resolution: "css-functions-list@npm:3.2.1"
+  checksum: 57d7deb3b05e84d95b88ba9b3244cf60d33b40652b3357f084c805b24a9febda5987ade44ef25a56be41e73249a7dcc157abd704d8a0e998b2c1c2e2d5de6461
   languageName: node
   linkType: hard
 
-"css-loader@npm:^6.7.1":
-  version: 6.8.1
-  resolution: "css-loader@npm:6.8.1"
+"css-loader@npm:^6.11.0, css-loader@npm:^6.7.1":
+  version: 6.11.0
+  resolution: "css-loader@npm:6.11.0"
   dependencies:
     icss-utils: ^5.1.0
-    postcss: ^8.4.21
-    postcss-modules-extract-imports: ^3.0.0
-    postcss-modules-local-by-default: ^4.0.3
-    postcss-modules-scope: ^3.0.0
+    postcss: ^8.4.33
+    postcss-modules-extract-imports: ^3.1.0
+    postcss-modules-local-by-default: ^4.0.5
+    postcss-modules-scope: ^3.2.0
     postcss-modules-values: ^4.0.0
     postcss-value-parser: ^4.2.0
-    semver: ^7.3.8
+    semver: ^7.5.4
   peerDependencies:
+    "@rspack/core": 0.x || 1.x
     webpack: ^5.0.0
-  checksum: 7c1784247bdbe76dc5c55fb1ac84f1d4177a74c47259942c9cfdb7a8e6baef11967a0bc85ac285f26bd26d5059decb848af8154a03fdb4f4894f41212f45eef3
+  peerDependenciesMeta:
+    "@rspack/core":
+      optional: true
+    webpack:
+      optional: true
+  checksum: 5c8d35975a7121334905394e88e28f05df72f037dbed2fb8fec4be5f0b313ae73a13894ba791867d4a4190c35896da84a7fd0c54fb426db55d85ba5e714edbe3
   languageName: node
   linkType: hard
 
 "css-tree@npm:^2.3.1":
   version: 2.3.1
   resolution: "css-tree@npm:2.3.1"
   dependencies:
@@ -2700,32 +2528,65 @@
   version: 3.0.10
   resolution: "csstype@npm:3.0.10"
   checksum: 20a8fa324f2b33ddf94aa7507d1b6ab3daa6f3cc308888dc50126585d7952f2471de69b2dbe0635d1fdc31223fef8e070842691877e725caf456e2378685a631
   languageName: node
   linkType: hard
 
 "csstype@npm:^3.0.2":
-  version: 3.1.2
-  resolution: "csstype@npm:3.1.2"
-  checksum: e1a52e6c25c1314d6beef5168da704ab29c5186b877c07d822bd0806717d9a265e8493a2e35ca7e68d0f5d472d43fac1cdce70fd79fd0853dff81f3028d857b5
+  version: 3.1.3
+  resolution: "csstype@npm:3.1.3"
+  checksum: 8db785cc92d259102725b3c694ec0c823f5619a84741b5c7991b8ad135dfaa66093038a1cc63e03361a6cd28d122be48f2106ae72334e067dd619a51f49eddf7
   languageName: node
   linkType: hard
 
 "data-urls@npm:^2.0.0":
   version: 2.0.0
   resolution: "data-urls@npm:2.0.0"
   dependencies:
     abab: ^2.0.3
     whatwg-mimetype: ^2.3.0
     whatwg-url: ^8.0.0
   checksum: 97caf828aac25e25e04ba6869db0f99c75e6859bb5b424ada28d3e7841941ebf08ddff3c1b1bb4585986bd507a5d54c2a716853ea6cb98af877400e637393e71
   languageName: node
   linkType: hard
 
-"debug@npm:^4.1.1, debug@npm:^4.3.2, debug@npm:^4.3.4":
+"data-view-buffer@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "data-view-buffer@npm:1.0.1"
+  dependencies:
+    call-bind: ^1.0.6
+    es-errors: ^1.3.0
+    is-data-view: ^1.0.1
+  checksum: ce24348f3c6231223b216da92e7e6a57a12b4af81a23f27eff8feabdf06acfb16c00639c8b705ca4d167f761cfc756e27e5f065d0a1f840c10b907fdaf8b988c
+  languageName: node
+  linkType: hard
+
+"data-view-byte-length@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "data-view-byte-length@npm:1.0.1"
+  dependencies:
+    call-bind: ^1.0.7
+    es-errors: ^1.3.0
+    is-data-view: ^1.0.1
+  checksum: dbb3200edcb7c1ef0d68979834f81d64fd8cab2f7691b3a4c6b97e67f22182f3ec2c8602efd7b76997b55af6ff8bce485829c1feda4fa2165a6b71fb7baa4269
+  languageName: node
+  linkType: hard
+
+"data-view-byte-offset@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "data-view-byte-offset@npm:1.0.0"
+  dependencies:
+    call-bind: ^1.0.6
+    es-errors: ^1.3.0
+    is-data-view: ^1.0.1
+  checksum: 7f0bf8720b7414ca719eedf1846aeec392f2054d7af707c5dc9a753cc77eb8625f067fa901e0b5127e831f9da9056138d894b9c2be79c27a21f6db5824f009c2
+  languageName: node
+  linkType: hard
+
+"debug@npm:^4.3.1, debug@npm:^4.3.2, debug@npm:^4.3.4":
   version: 4.3.4
   resolution: "debug@npm:4.3.4"
   dependencies:
     ms: 2.1.2
   peerDependenciesMeta:
     supports-color:
       optional: true
@@ -2767,55 +2628,26 @@
 "deepmerge@npm:^4.2.2":
   version: 4.3.1
   resolution: "deepmerge@npm:4.3.1"
   checksum: 2024c6a980a1b7128084170c4cf56b0fd58a63f2da1660dcfe977415f27b17dbe5888668b59d0b063753f3220719d5e400b7f113609489c90160bb9a5518d052
   languageName: node
   linkType: hard
 
-"default-browser-id@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "default-browser-id@npm:3.0.0"
-  dependencies:
-    bplist-parser: ^0.2.0
-    untildify: ^4.0.0
-  checksum: 279c7ad492542e5556336b6c254a4eaf31b2c63a5433265655ae6e47301197b6cfb15c595a6fdc6463b2ff8e1a1a1ed3cba56038a60e1527ba4ab1628c6b9941
-  languageName: node
-  linkType: hard
-
-"default-browser@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "default-browser@npm:4.0.0"
-  dependencies:
-    bundle-name: ^3.0.0
-    default-browser-id: ^3.0.0
-    execa: ^7.1.1
-    titleize: ^3.0.0
-  checksum: 40c5af984799042b140300be5639c9742599bda76dc9eba5ac9ad5943c83dd36cebc4471eafcfddf8e0ec817166d5ba89d56f08e66a126c7c7908a179cead1a7
-  languageName: node
-  linkType: hard
-
-"define-data-property@npm:^1.0.1":
-  version: 1.1.0
-  resolution: "define-data-property@npm:1.1.0"
+"define-data-property@npm:^1.0.1, define-data-property@npm:^1.1.4":
+  version: 1.1.4
+  resolution: "define-data-property@npm:1.1.4"
   dependencies:
-    get-intrinsic: ^1.2.1
+    es-define-property: ^1.0.0
+    es-errors: ^1.3.0
     gopd: ^1.0.1
-    has-property-descriptors: ^1.0.0
-  checksum: 7ad4ee84cca8ad427a4831f5693526804b62ce9dfd4efac77214e95a4382aed930072251d4075dc8dc9fc949a353ed51f19f5285a84a788ba9216cc51472a093
+  checksum: 8068ee6cab694d409ac25936eb861eea704b7763f7f342adbdfe337fc27c78d7ae0eff2364b2917b58c508d723c7a074326d068eef2e45c4edcd85cf94d0313b
   languageName: node
   linkType: hard
 
-"define-lazy-prop@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "define-lazy-prop@npm:3.0.0"
-  checksum: 54884f94caac0791bf6395a3ec530ce901cf71c47b0196b8754f3fd17edb6c0e80149c1214429d851873bb0d689dbe08dcedbb2306dc45c8534a5934723851b6
-  languageName: node
-  linkType: hard
-
-"define-properties@npm:^1.1.3, define-properties@npm:^1.1.4, define-properties@npm:^1.2.0":
+"define-properties@npm:^1.1.3, define-properties@npm:^1.2.0, define-properties@npm:^1.2.1":
   version: 1.2.1
   resolution: "define-properties@npm:1.2.1"
   dependencies:
     define-data-property: ^1.0.1
     has-property-descriptors: ^1.0.0
     object-keys: ^1.1.1
   checksum: b4ccd00597dd46cb2d4a379398f5b19fca84a16f3374e2249201992f36b30f6835949a9429669ee6b41b6e837205a163eadd745e472069e70dfc10f03e5fcc12
@@ -2893,18 +2725,18 @@
 "eastasianwidth@npm:^0.2.0":
   version: 0.2.0
   resolution: "eastasianwidth@npm:0.2.0"
   checksum: 7d00d7cd8e49b9afa762a813faac332dee781932d6f2c848dc348939c4253f1d4564341b7af1d041853bc3f32c2ef141b58e0a4d9862c17a7f08f68df1e0f1ed
   languageName: node
   linkType: hard
 
-"electron-to-chromium@npm:^1.4.526":
-  version: 1.4.527
-  resolution: "electron-to-chromium@npm:1.4.527"
-  checksum: 9e5667b78189cf79a4b66f1c6924bc19ad42f8ce326702c916d866cad5b571545d0157efeeb839fe8b669a73c1636e1a097bd8174bfa1db0c9579316b3beabce
+"electron-to-chromium@npm:^1.4.668":
+  version: 1.4.741
+  resolution: "electron-to-chromium@npm:1.4.741"
+  checksum: 4475477800400befd754e3a173f21eee7f36960ae3868bff443f5f1f30ff494829167d5da46b9738db468f1a8daaf08e2a60f8f56dc122158292ff649686d858
   languageName: node
   linkType: hard
 
 "emoji-regex@npm:^8.0.0":
   version: 8.0.0
   resolution: "emoji-regex@npm:8.0.0"
   checksum: d4c5c39d5a9868b5fa152f00cada8a936868fd3367f33f71be515ecee4c803132d11b31a6222b2571b1e5f7e13890156a94880345594d0ce7e3c9895f560f192
@@ -2921,111 +2753,143 @@
 "emojis-list@npm:^3.0.0":
   version: 3.0.0
   resolution: "emojis-list@npm:3.0.0"
   checksum: ddaaa02542e1e9436c03970eeed445f4ed29a5337dfba0fe0c38dfdd2af5da2429c2a0821304e8a8d1cadf27fdd5b22ff793571fa803ae16852a6975c65e8e70
   languageName: node
   linkType: hard
 
-"enhanced-resolve@npm:^5.15.0":
-  version: 5.15.0
-  resolution: "enhanced-resolve@npm:5.15.0"
+"enhanced-resolve@npm:^5.16.0":
+  version: 5.16.0
+  resolution: "enhanced-resolve@npm:5.16.0"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: fbd8cdc9263be71cc737aa8a7d6c57b43d6aa38f6cc75dde6fcd3598a130cc465f979d2f4d01bb3bf475acb43817749c79f8eef9be048683602ca91ab52e4f11
+  checksum: ccfd01850ecf2aa51e8554d539973319ff7d8a539ef1e0ba3460a0ccad6223c4ef6e19165ee64161b459cd8a48df10f52af4434c60023c65fde6afa32d475f7e
   languageName: node
   linkType: hard
 
 "entities@npm:^2.0.0":
   version: 2.2.0
   resolution: "entities@npm:2.2.0"
   checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
   languageName: node
   linkType: hard
 
 "envinfo@npm:^7.7.3":
-  version: 7.10.0
-  resolution: "envinfo@npm:7.10.0"
+  version: 7.12.0
+  resolution: "envinfo@npm:7.12.0"
   bin:
     envinfo: dist/cli.js
-  checksum: 05e81a5768c42cbd5c580dc3f274db3401facadd53e9bd52e2aa49dfbb5d8b26f6181c25a6652d79618a6994185bd2b1c137673101690b147f758e4e71d42f7d
+  checksum: 4c83a55768cf8b7e553155c29e7fa7bbdb0fb2c1156208efc373fc030045c6aca5e8e642e96027d3eb0c752156922ea3fca6183d9e13f38507f0e02ec82c23a1
   languageName: node
   linkType: hard
 
 "error-ex@npm:^1.3.1":
   version: 1.3.2
   resolution: "error-ex@npm:1.3.2"
   dependencies:
     is-arrayish: ^0.2.1
   checksum: c1c2b8b65f9c91b0f9d75f0debaa7ec5b35c266c2cac5de412c1a6de86d4cbae04ae44e510378cb14d032d0645a36925d0186f8bb7367bcc629db256b743a001
   languageName: node
   linkType: hard
 
-"es-abstract@npm:^1.22.1":
-  version: 1.22.2
-  resolution: "es-abstract@npm:1.22.2"
-  dependencies:
-    array-buffer-byte-length: ^1.0.0
-    arraybuffer.prototype.slice: ^1.0.2
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
-    es-set-tostringtag: ^2.0.1
+"es-abstract@npm:^1.22.1, es-abstract@npm:^1.22.3, es-abstract@npm:^1.23.0, es-abstract@npm:^1.23.2":
+  version: 1.23.3
+  resolution: "es-abstract@npm:1.23.3"
+  dependencies:
+    array-buffer-byte-length: ^1.0.1
+    arraybuffer.prototype.slice: ^1.0.3
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
+    data-view-buffer: ^1.0.1
+    data-view-byte-length: ^1.0.1
+    data-view-byte-offset: ^1.0.0
+    es-define-property: ^1.0.0
+    es-errors: ^1.3.0
+    es-object-atoms: ^1.0.0
+    es-set-tostringtag: ^2.0.3
     es-to-primitive: ^1.2.1
     function.prototype.name: ^1.1.6
-    get-intrinsic: ^1.2.1
-    get-symbol-description: ^1.0.0
+    get-intrinsic: ^1.2.4
+    get-symbol-description: ^1.0.2
     globalthis: ^1.0.3
     gopd: ^1.0.1
-    has: ^1.0.3
-    has-property-descriptors: ^1.0.0
-    has-proto: ^1.0.1
+    has-property-descriptors: ^1.0.2
+    has-proto: ^1.0.3
     has-symbols: ^1.0.3
-    internal-slot: ^1.0.5
-    is-array-buffer: ^3.0.2
+    hasown: ^2.0.2
+    internal-slot: ^1.0.7
+    is-array-buffer: ^3.0.4
     is-callable: ^1.2.7
-    is-negative-zero: ^2.0.2
+    is-data-view: ^1.0.1
+    is-negative-zero: ^2.0.3
     is-regex: ^1.1.4
-    is-shared-array-buffer: ^1.0.2
+    is-shared-array-buffer: ^1.0.3
     is-string: ^1.0.7
-    is-typed-array: ^1.1.12
+    is-typed-array: ^1.1.13
     is-weakref: ^1.0.2
-    object-inspect: ^1.12.3
+    object-inspect: ^1.13.1
     object-keys: ^1.1.1
-    object.assign: ^4.1.4
-    regexp.prototype.flags: ^1.5.1
-    safe-array-concat: ^1.0.1
-    safe-regex-test: ^1.0.0
-    string.prototype.trim: ^1.2.8
-    string.prototype.trimend: ^1.0.7
-    string.prototype.trimstart: ^1.0.7
-    typed-array-buffer: ^1.0.0
-    typed-array-byte-length: ^1.0.0
-    typed-array-byte-offset: ^1.0.0
-    typed-array-length: ^1.0.4
+    object.assign: ^4.1.5
+    regexp.prototype.flags: ^1.5.2
+    safe-array-concat: ^1.1.2
+    safe-regex-test: ^1.0.3
+    string.prototype.trim: ^1.2.9
+    string.prototype.trimend: ^1.0.8
+    string.prototype.trimstart: ^1.0.8
+    typed-array-buffer: ^1.0.2
+    typed-array-byte-length: ^1.0.1
+    typed-array-byte-offset: ^1.0.2
+    typed-array-length: ^1.0.6
     unbox-primitive: ^1.0.2
-    which-typed-array: ^1.1.11
-  checksum: cc70e592d360d7d729859013dee7a610c6b27ed8630df0547c16b0d16d9fe6505a70ee14d1af08d970fdd132b3f88c9ca7815ce72c9011608abf8ab0e55fc515
+    which-typed-array: ^1.1.15
+  checksum: f840cf161224252512f9527306b57117192696571e07920f777cb893454e32999206198b4f075516112af6459daca282826d1735c450528470356d09eff3a9ae
+  languageName: node
+  linkType: hard
+
+"es-define-property@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "es-define-property@npm:1.0.0"
+  dependencies:
+    get-intrinsic: ^1.2.4
+  checksum: f66ece0a887b6dca71848fa71f70461357c0e4e7249696f81bad0a1f347eed7b31262af4a29f5d726dc026426f085483b6b90301855e647aa8e21936f07293c6
+  languageName: node
+  linkType: hard
+
+"es-errors@npm:^1.2.1, es-errors@npm:^1.3.0":
+  version: 1.3.0
+  resolution: "es-errors@npm:1.3.0"
+  checksum: ec1414527a0ccacd7f15f4a3bc66e215f04f595ba23ca75cdae0927af099b5ec865f9f4d33e9d7e86f512f252876ac77d4281a7871531a50678132429b1271b5
   languageName: node
   linkType: hard
 
 "es-module-lexer@npm:^1.2.1":
-  version: 1.3.1
-  resolution: "es-module-lexer@npm:1.3.1"
-  checksum: 3beafa7e171eb1e8cc45695edf8d51638488dddf65294d7911f8d6a96249da6a9838c87529262cc6ea53988d8272cec0f4bff93f476ed031a54ba3afb51a0ed3
+  version: 1.5.0
+  resolution: "es-module-lexer@npm:1.5.0"
+  checksum: adbe0772701e226b4b853f758fd89c0bbfe8357ab93babde7b1cdb4f88c3a31460c908cbe578817e241d116cc4fcf569f7c6f29c4fbfa0aadb0def90f1ad4dd2
   languageName: node
   linkType: hard
 
-"es-set-tostringtag@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "es-set-tostringtag@npm:2.0.1"
+"es-object-atoms@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "es-object-atoms@npm:1.0.0"
   dependencies:
-    get-intrinsic: ^1.1.3
-    has: ^1.0.3
-    has-tostringtag: ^1.0.0
-  checksum: ec416a12948cefb4b2a5932e62093a7cf36ddc3efd58d6c58ca7ae7064475ace556434b869b0bbeb0c365f1032a8ccd577211101234b69837ad83ad204fff884
+    es-errors: ^1.3.0
+  checksum: 26f0ff78ab93b63394e8403c353842b2272836968de4eafe97656adfb8a7c84b9099bf0fe96ed58f4a4cddc860f6e34c77f91649a58a5daa4a9c40b902744e3c
+  languageName: node
+  linkType: hard
+
+"es-set-tostringtag@npm:^2.0.3":
+  version: 2.0.3
+  resolution: "es-set-tostringtag@npm:2.0.3"
+  dependencies:
+    get-intrinsic: ^1.2.4
+    has-tostringtag: ^1.0.2
+    hasown: ^2.0.1
+  checksum: 7227fa48a41c0ce83e0377b11130d324ac797390688135b8da5c28994c0165be8b252e15cd1de41e1325e5a5412511586960213e88f9ab4a5e7d028895db5129
   languageName: node
   linkType: hard
 
 "es-to-primitive@npm:^1.2.1":
   version: 1.2.1
   resolution: "es-to-primitive@npm:1.2.1"
   dependencies:
@@ -3033,17 +2897,17 @@
     is-date-object: ^1.0.1
     is-symbol: ^1.0.2
   checksum: 4ead6671a2c1402619bdd77f3503991232ca15e17e46222b0a41a5d81aebc8740a77822f5b3c965008e631153e9ef0580540007744521e72de8e33599fca2eed
   languageName: node
   linkType: hard
 
 "escalade@npm:^3.1.1":
-  version: 3.1.1
-  resolution: "escalade@npm:3.1.1"
-  checksum: a3e2a99f07acb74b3ad4989c48ca0c3140f69f923e56d0cba0526240ee470b91010f9d39001f2a4a313841d237ede70a729e92125191ba5d21e74b106800b133
+  version: 3.1.2
+  resolution: "escalade@npm:3.1.2"
+  checksum: 1ec0977aa2772075493002bdbd549d595ff6e9393b1cb0d7d6fcaf78c750da0c158f180938365486f75cb69fba20294351caddfce1b46552a7b6c3cde52eaa02
   languageName: node
   linkType: hard
 
 "escape-string-regexp@npm:^1.0.5":
   version: 1.0.5
   resolution: "escape-string-regexp@npm:1.0.5"
   checksum: 6092fda75c63b110c706b6a9bfde8a612ad595b628f0bd2147eea1d3406723020810e591effc7db1da91d80a71a737a313567c5abb3813e8d9c71f4aa595b410
@@ -3064,30 +2928,31 @@
     eslint: ">=7.0.0"
   bin:
     eslint-config-prettier: bin/cli.js
   checksum: 153266badd477e49b0759816246b2132f1dbdb6c7f313ca60a9af5822fd1071c2bc5684a3720d78b725452bbac04bb130878b2513aea5e72b1b792de5a69fec8
   languageName: node
   linkType: hard
 
-"eslint-plugin-prettier@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "eslint-plugin-prettier@npm:5.0.0"
+"eslint-plugin-prettier@npm:^5.1.3":
+  version: 5.1.3
+  resolution: "eslint-plugin-prettier@npm:5.1.3"
   dependencies:
     prettier-linter-helpers: ^1.0.0
-    synckit: ^0.8.5
+    synckit: ^0.8.6
   peerDependencies:
     "@types/eslint": ">=8.0.0"
     eslint: ">=8.0.0"
+    eslint-config-prettier: "*"
     prettier: ">=3.0.0"
   peerDependenciesMeta:
     "@types/eslint":
       optional: true
     eslint-config-prettier:
       optional: true
-  checksum: 84e88744b9050f2d5ef31b94e85294dda16f3a53c2449f9d33eac8ae6264889b459bf35a68e438fb6b329c2a1d6491aac4bfa00d86317e7009de3dad0311bec6
+  checksum: eb2a7d46a1887e1b93788ee8f8eb81e0b6b2a6f5a66a62bc6f375b033fc4e7ca16448da99380be800042786e76cf5c0df9c87a51a2c9b960ed47acbd7c0b9381
   languageName: node
   linkType: hard
 
 "eslint-scope@npm:5.1.1":
   version: 5.1.1
   resolution: "eslint-scope@npm:5.1.1"
   dependencies:
@@ -3110,25 +2975,26 @@
 "eslint-visitor-keys@npm:^3.3.0, eslint-visitor-keys@npm:^3.4.1, eslint-visitor-keys@npm:^3.4.3":
   version: 3.4.3
   resolution: "eslint-visitor-keys@npm:3.4.3"
   checksum: 36e9ef87fca698b6fd7ca5ca35d7b2b6eeaaf106572e2f7fd31c12d3bfdaccdb587bba6d3621067e5aece31c8c3a348b93922ab8f7b2cbc6aaab5e1d89040c60
   languageName: node
   linkType: hard
 
-"eslint@npm:^8.36.0":
-  version: 8.49.0
-  resolution: "eslint@npm:8.49.0"
+"eslint@npm:^8.57.0":
+  version: 8.57.0
+  resolution: "eslint@npm:8.57.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@eslint-community/regexpp": ^4.6.1
-    "@eslint/eslintrc": ^2.1.2
-    "@eslint/js": 8.49.0
-    "@humanwhocodes/config-array": ^0.11.11
+    "@eslint/eslintrc": ^2.1.4
+    "@eslint/js": 8.57.0
+    "@humanwhocodes/config-array": ^0.11.14
     "@humanwhocodes/module-importer": ^1.0.1
     "@nodelib/fs.walk": ^1.2.8
+    "@ungap/structured-clone": ^1.2.0
     ajv: ^6.12.4
     chalk: ^4.0.0
     cross-spawn: ^7.0.2
     debug: ^4.3.2
     doctrine: ^3.0.0
     escape-string-regexp: ^4.0.0
     eslint-scope: ^7.2.2
@@ -3153,15 +3019,15 @@
     minimatch: ^3.1.2
     natural-compare: ^1.4.0
     optionator: ^0.9.3
     strip-ansi: ^6.0.1
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
-  checksum: 4dfe257e1e42da2f9da872b05aaaf99b0f5aa022c1a91eee8f2af1ab72651b596366320c575ccd4e0469f7b4c97aff5bb85ae3323ebd6a293c3faef4028b0d81
+  checksum: 3a48d7ff85ab420a8447e9810d8087aea5b1df9ef68c9151732b478de698389ee656fd895635b5f2871c89ee5a2652b3f343d11e9db6f8486880374ebc74a2d9
   languageName: node
   linkType: hard
 
 "espree@npm:^9.6.0, espree@npm:^9.6.1":
   version: 9.6.1
   resolution: "espree@npm:9.6.1"
   dependencies:
@@ -3214,45 +3080,18 @@
 "events@npm:^3.2.0":
   version: 3.3.0
   resolution: "events@npm:3.3.0"
   checksum: f6f487ad2198aa41d878fa31452f1a3c00958f46e9019286ff4787c84aac329332ab45c9cdc8c445928fc6d7ded294b9e005a7fce9426488518017831b272780
   languageName: node
   linkType: hard
 
-"execa@npm:^5.0.0":
-  version: 5.1.1
-  resolution: "execa@npm:5.1.1"
-  dependencies:
-    cross-spawn: ^7.0.3
-    get-stream: ^6.0.0
-    human-signals: ^2.1.0
-    is-stream: ^2.0.0
-    merge-stream: ^2.0.0
-    npm-run-path: ^4.0.1
-    onetime: ^5.1.2
-    signal-exit: ^3.0.3
-    strip-final-newline: ^2.0.0
-  checksum: fba9022c8c8c15ed862847e94c252b3d946036d7547af310e344a527e59021fd8b6bb0723883ea87044dc4f0201f949046993124a42ccb0855cae5bf8c786343
-  languageName: node
-  linkType: hard
-
-"execa@npm:^7.1.1":
-  version: 7.2.0
-  resolution: "execa@npm:7.2.0"
-  dependencies:
-    cross-spawn: ^7.0.3
-    get-stream: ^6.0.1
-    human-signals: ^4.3.0
-    is-stream: ^3.0.0
-    merge-stream: ^2.0.0
-    npm-run-path: ^5.1.0
-    onetime: ^6.0.0
-    signal-exit: ^3.0.7
-    strip-final-newline: ^3.0.0
-  checksum: 14fd17ba0ca8c87b277584d93b1d9fc24f2a65e5152b31d5eb159a3b814854283eaae5f51efa9525e304447e2f757c691877f7adff8fde5746aae67eb1edd1cc
+"exenv-es6@npm:^1.1.1":
+  version: 1.1.1
+  resolution: "exenv-es6@npm:1.1.1"
+  checksum: 7f2aa12025e6f06c48dc286f380cf3183bb19c6017b36d91695034a3e5124a7235c4f8ff24ca2eb88ae801322f0f99605cedfcfd996a5fcbba7669320e2a448e
   languageName: node
   linkType: hard
 
 "fast-deep-equal@npm:^3.1.1, fast-deep-equal@npm:^3.1.3":
   version: 3.1.3
   resolution: "fast-deep-equal@npm:3.1.3"
   checksum: e21a9d8d84f53493b6aa15efc9cfd53dd5b714a1f23f67fb5dc8f574af80df889b3bce25dc081887c6d25457cce704e636395333abad896ccdec03abaf1f3f9d
@@ -3262,24 +3101,24 @@
 "fast-diff@npm:^1.1.2":
   version: 1.3.0
   resolution: "fast-diff@npm:1.3.0"
   checksum: d22d371b994fdc8cce9ff510d7b8dc4da70ac327bcba20df607dd5b9cae9f908f4d1028f5fe467650f058d1e7270235ae0b8230809a262b4df587a3b3aa216c3
   languageName: node
   linkType: hard
 
-"fast-glob@npm:^3.2.9, fast-glob@npm:^3.3.0, fast-glob@npm:^3.3.1":
-  version: 3.3.1
-  resolution: "fast-glob@npm:3.3.1"
+"fast-glob@npm:^3.2.9, fast-glob@npm:^3.3.1":
+  version: 3.3.2
+  resolution: "fast-glob@npm:3.3.2"
   dependencies:
     "@nodelib/fs.stat": ^2.0.2
     "@nodelib/fs.walk": ^1.2.3
     glob-parent: ^5.1.2
     merge2: ^1.3.0
     micromatch: ^4.0.4
-  checksum: b6f3add6403e02cf3a798bfbb1183d0f6da2afd368f27456010c0bc1f9640aea308243d4cb2c0ab142f618276e65ecb8be1661d7c62a7b4e5ba774b9ce5432e5
+  checksum: 900e4979f4dbc3313840078419245621259f349950411ca2fa445a2f9a1a6d98c3b5e7e0660c5ccd563aa61abe133a21765c6c0dec8e57da1ba71d8000b05ec1
   languageName: node
   linkType: hard
 
 "fast-json-stable-stringify@npm:^2.0.0":
   version: 2.1.0
   resolution: "fast-json-stable-stringify@npm:2.1.0"
   checksum: b191531e36c607977e5b1c47811158733c34ccb3bfde92c44798929e9b4154884378536d26ad90dfecd32e1ffc09c545d23535ad91b3161a27ddbb8ebe0cbecb
@@ -3297,31 +3136,40 @@
   version: 1.0.16
   resolution: "fastest-levenshtein@npm:1.0.16"
   checksum: a78d44285c9e2ae2c25f3ef0f8a73f332c1247b7ea7fb4a191e6bb51aa6ee1ef0dfb3ed113616dcdc7023e18e35a8db41f61c8d88988e877cf510df8edafbc71
   languageName: node
   linkType: hard
 
 "fastq@npm:^1.6.0":
-  version: 1.15.0
-  resolution: "fastq@npm:1.15.0"
+  version: 1.17.1
+  resolution: "fastq@npm:1.17.1"
   dependencies:
     reusify: ^1.0.4
-  checksum: 0170e6bfcd5d57a70412440b8ef600da6de3b2a6c5966aeaf0a852d542daff506a0ee92d6de7679d1de82e644bce69d7a574a6c93f0b03964b5337eed75ada1a
+  checksum: a8c5b26788d5a1763f88bae56a8ddeee579f935a831c5fe7a8268cea5b0a91fbfe705f612209e02d639b881d7b48e461a50da4a10cfaa40da5ca7cc9da098d88
   languageName: node
   linkType: hard
 
 "file-entry-cache@npm:^6.0.1":
   version: 6.0.1
   resolution: "file-entry-cache@npm:6.0.1"
   dependencies:
     flat-cache: ^3.0.4
   checksum: f49701feaa6314c8127c3c2f6173cfefff17612f5ed2daaafc6da13b5c91fd43e3b2a58fd0d63f9f94478a501b167615931e7200e31485e320f74a33885a9c74
   languageName: node
   linkType: hard
 
+"file-entry-cache@npm:^7.0.0":
+  version: 7.0.2
+  resolution: "file-entry-cache@npm:7.0.2"
+  dependencies:
+    flat-cache: ^3.2.0
+  checksum: 283c674fc26bed1c44e74cf25c2640c813e222ea30a2536404b53511ca311d4a2502ee8145a01aecd12b9a910eb4162364776be27a9683e8447332054e9d712f
+  languageName: node
+  linkType: hard
+
 "fill-range@npm:^7.0.1":
   version: 7.0.1
   resolution: "fill-range@npm:7.0.1"
   dependencies:
     to-regex-range: ^5.0.1
   checksum: cc283f4e65b504259e64fd969bcf4def4eb08d85565e906b7d36516e87819db52029a76b6363d0f02d0d532f0033c9603b9e2d943d56ee3b0d4f7ad3328ff917
   languageName: node
@@ -3350,29 +3198,38 @@
   dependencies:
     locate-path: ^6.0.0
     path-exists: ^4.0.0
   checksum: 07955e357348f34660bde7920783204ff5a26ac2cafcaa28bace494027158a97b9f56faaf2d89a6106211a8174db650dd9f503f9c0d526b1202d5554a00b9095
   languageName: node
   linkType: hard
 
-"flat-cache@npm:^3.0.4":
-  version: 3.1.0
-  resolution: "flat-cache@npm:3.1.0"
+"flat-cache@npm:^3.0.4, flat-cache@npm:^3.2.0":
+  version: 3.2.0
+  resolution: "flat-cache@npm:3.2.0"
   dependencies:
-    flatted: ^3.2.7
+    flatted: ^3.2.9
     keyv: ^4.5.3
     rimraf: ^3.0.2
-  checksum: 99312601d5b90f44aef403f17f056dc09be7e437703740b166cdc9386d99e681f74e6b6e8bd7d010bda66904ea643c9527276b1b80308a2119741d94108a4d8f
+  checksum: e7e0f59801e288b54bee5cb9681e9ee21ee28ef309f886b312c9d08415b79fc0f24ac842f84356ce80f47d6a53de62197ce0e6e148dc42d5db005992e2a756ec
   languageName: node
   linkType: hard
 
-"flatted@npm:^3.2.7":
-  version: 3.2.9
-  resolution: "flatted@npm:3.2.9"
-  checksum: f14167fbe26a9d20f6fca8d998e8f1f41df72c8e81f9f2c9d61ed2bea058248f5e1cbd05e7f88c0e5087a6a0b822a1e5e2b446e879f3cfbe0b07ba2d7f80b026
+"flat@npm:^5.0.2":
+  version: 5.0.2
+  resolution: "flat@npm:5.0.2"
+  bin:
+    flat: cli.js
+  checksum: 12a1536ac746db74881316a181499a78ef953632ddd28050b7a3a43c62ef5462e3357c8c29d76072bb635f147f7a9a1f0c02efef6b4be28f8db62ceb3d5c7f5d
+  languageName: node
+  linkType: hard
+
+"flatted@npm:^3.2.9":
+  version: 3.3.1
+  resolution: "flatted@npm:3.3.1"
+  checksum: 85ae7181650bb728c221e7644cbc9f4bf28bc556f2fc89bb21266962bdf0ce1029cc7acc44bb646cd469d9baac7c317f64e841c4c4c00516afa97320cdac7f94
   languageName: node
   linkType: hard
 
 "for-each@npm:^0.3.3":
   version: 0.3.3
   resolution: "for-each@npm:0.3.3"
   dependencies:
@@ -3412,18 +3269,18 @@
 "fs.realpath@npm:^1.0.0":
   version: 1.0.0
   resolution: "fs.realpath@npm:1.0.0"
   checksum: 99ddea01a7e75aa276c250a04eedeffe5662bce66c65c07164ad6264f9de18fb21be9433ead460e54cff20e31721c811f4fb5d70591799df5f85dce6d6746fd0
   languageName: node
   linkType: hard
 
-"function-bind@npm:^1.1.1":
-  version: 1.1.1
-  resolution: "function-bind@npm:1.1.1"
-  checksum: b32fbaebb3f8ec4969f033073b43f5c8befbb58f1a79e12f1d7490358150359ebd92f49e72ff0144f65f2c48ea2a605bff2d07965f548f6474fd8efd95bf361a
+"function-bind@npm:^1.1.2":
+  version: 1.1.2
+  resolution: "function-bind@npm:1.1.2"
+  checksum: 2b0ff4ce708d99715ad14a6d1f894e2a83242e4a52ccfcefaee5e40050562e5f6dafc1adbb4ce2d4ab47279a45dc736ab91ea5042d843c3c092820dfe032efb1
   languageName: node
   linkType: hard
 
 "function.prototype.name@npm:^1.1.6":
   version: 1.1.6
   resolution: "function.prototype.name@npm:1.1.6"
   dependencies:
@@ -3438,40 +3295,35 @@
 "functions-have-names@npm:^1.2.3":
   version: 1.2.3
   resolution: "functions-have-names@npm:1.2.3"
   checksum: c3f1f5ba20f4e962efb71344ce0a40722163e85bee2101ce25f88214e78182d2d2476aa85ef37950c579eb6cf6ee811c17b3101bb84004bb75655f3e33f3fdb5
   languageName: node
   linkType: hard
 
-"get-intrinsic@npm:^1.0.2, get-intrinsic@npm:^1.1.1, get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.0, get-intrinsic@npm:^1.2.1":
-  version: 1.2.1
-  resolution: "get-intrinsic@npm:1.2.1"
+"get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.1, get-intrinsic@npm:^1.2.3, get-intrinsic@npm:^1.2.4":
+  version: 1.2.4
+  resolution: "get-intrinsic@npm:1.2.4"
   dependencies:
-    function-bind: ^1.1.1
-    has: ^1.0.3
+    es-errors: ^1.3.0
+    function-bind: ^1.1.2
     has-proto: ^1.0.1
     has-symbols: ^1.0.3
-  checksum: 5b61d88552c24b0cf6fa2d1b3bc5459d7306f699de060d76442cce49a4721f52b8c560a33ab392cf5575b7810277d54ded9d4d39a1ea61855619ebc005aa7e5f
-  languageName: node
-  linkType: hard
-
-"get-stream@npm:^6.0.0, get-stream@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "get-stream@npm:6.0.1"
-  checksum: e04ecece32c92eebf5b8c940f51468cd53554dcbb0ea725b2748be583c9523d00128137966afce410b9b051eb2ef16d657cd2b120ca8edafcf5a65e81af63cad
+    hasown: ^2.0.0
+  checksum: 414e3cdf2c203d1b9d7d33111df746a4512a1aa622770b361dadddf8ed0b5aeb26c560f49ca077e24bfafb0acb55ca908d1f709216ccba33ffc548ec8a79a951
   languageName: node
   linkType: hard
 
-"get-symbol-description@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "get-symbol-description@npm:1.0.0"
+"get-symbol-description@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "get-symbol-description@npm:1.0.2"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.1.1
-  checksum: 9ceff8fe968f9270a37a1f73bf3f1f7bda69ca80f4f80850670e0e7b9444ff99323f7ac52f96567f8b5f5fbe7ac717a0d81d3407c7313e82810c6199446a5247
+    call-bind: ^1.0.5
+    es-errors: ^1.3.0
+    get-intrinsic: ^1.2.4
+  checksum: e1cb53bc211f9dbe9691a4f97a46837a553c4e7caadd0488dc24ac694db8a390b93edd412b48dcdd0b4bbb4c595de1709effc75fc87c0839deedc6968f5bd973
   languageName: node
   linkType: hard
 
 "glob-parent@npm:^5.1.2":
   version: 5.1.2
   resolution: "glob-parent@npm:5.1.2"
   dependencies:
@@ -3492,26 +3344,26 @@
 "glob-to-regexp@npm:^0.4.1":
   version: 0.4.1
   resolution: "glob-to-regexp@npm:0.4.1"
   checksum: e795f4e8f06d2a15e86f76e4d92751cf8bbfcf0157cea5c2f0f35678a8195a750b34096b1256e436f0cebc1883b5ff0888c47348443e69546a5a87f9e1eb1167
   languageName: node
   linkType: hard
 
-"glob@npm:^10.2.5":
-  version: 10.3.5
-  resolution: "glob@npm:10.3.5"
+"glob@npm:^10.3.7":
+  version: 10.3.12
+  resolution: "glob@npm:10.3.12"
   dependencies:
     foreground-child: ^3.1.0
-    jackspeak: ^2.0.3
+    jackspeak: ^2.3.6
     minimatch: ^9.0.1
-    minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
-    path-scurry: ^1.10.1
+    minipass: ^7.0.4
+    path-scurry: ^1.10.2
   bin:
-    glob: dist/cjs/src/bin.js
-  checksum: 564f4799cae48c0bcc841c88a20b539b5701c27ed5596f8623f588b3c523262d3fc20eb1ea89cab9c75b0912faf40ca5501fc835f982225d0d0599282b09e97a
+    glob: dist/esm/bin.mjs
+  checksum: 2b0949d6363021aaa561b108ac317bf5a97271b8a5d7a5fac1a176e40e8068ecdcccc992f8a7e958593d501103ac06d673de92adc1efcbdab45edefe35f8d7c6
   languageName: node
   linkType: hard
 
 "glob@npm:^7.1.3":
   version: 7.2.3
   resolution: "glob@npm:7.2.3"
   dependencies:
@@ -3556,19 +3408,19 @@
     kind-of: ^6.0.2
     which: ^1.3.1
   checksum: 8a82fc1d6f22c45484a4e34656cc91bf021a03e03213b0035098d605bfc612d7141f1e14a21097e8a0413b4884afd5b260df0b6a25605ce9d722e11f1df2881d
   languageName: node
   linkType: hard
 
 "globals@npm:^13.19.0":
-  version: 13.22.0
-  resolution: "globals@npm:13.22.0"
+  version: 13.24.0
+  resolution: "globals@npm:13.24.0"
   dependencies:
     type-fest: ^0.20.2
-  checksum: 64af5a09565341432770444085f7aa98b54331c3b69732e0de411003921fa2dd060222ae7b50bec0b98f29c4d00b4f49bf434049ba9f7c36ca4ee1773f60458c
+  checksum: 56066ef058f6867c04ff203b8a44c15b038346a62efbc3060052a1016be9f56f4cf0b2cd45b74b22b81e521a889fc7786c73691b0549c2f3a6e825b3d394f43c
   languageName: node
   linkType: hard
 
 "globalthis@npm:^1.0.3":
   version: 1.0.3
   resolution: "globalthis@npm:1.0.3"
   dependencies:
@@ -3603,15 +3455,15 @@
   resolution: "gopd@npm:1.0.1"
   dependencies:
     get-intrinsic: ^1.1.3
   checksum: a5ccfb8806e0917a94e0b3de2af2ea4979c1da920bc381667c260e00e7cafdbe844e2cb9c5bcfef4e5412e8bf73bab837285bc35c7ba73aaaf0134d4583393a6
   languageName: node
   linkType: hard
 
-"graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.9":
+"graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.11, graceful-fs@npm:^4.2.4":
   version: 4.2.11
   resolution: "graceful-fs@npm:4.2.11"
   checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
   languageName: node
   linkType: hard
 
 "graphemer@npm:^1.4.0":
@@ -3645,52 +3497,52 @@
 "has-flag@npm:^4.0.0":
   version: 4.0.0
   resolution: "has-flag@npm:4.0.0"
   checksum: 261a1357037ead75e338156b1f9452c016a37dcd3283a972a30d9e4a87441ba372c8b81f818cd0fbcd9c0354b4ae7e18b9e1afa1971164aef6d18c2b6095a8ad
   languageName: node
   linkType: hard
 
-"has-property-descriptors@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "has-property-descriptors@npm:1.0.0"
+"has-property-descriptors@npm:^1.0.0, has-property-descriptors@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "has-property-descriptors@npm:1.0.2"
   dependencies:
-    get-intrinsic: ^1.1.1
-  checksum: a6d3f0a266d0294d972e354782e872e2fe1b6495b321e6ef678c9b7a06a40408a6891817350c62e752adced73a94ac903c54734fee05bf65b1905ee1368194bb
+    es-define-property: ^1.0.0
+  checksum: fcbb246ea2838058be39887935231c6d5788babed499d0e9d0cc5737494c48aba4fe17ba1449e0d0fbbb1e36175442faa37f9c427ae357d6ccb1d895fbcd3de3
   languageName: node
   linkType: hard
 
-"has-proto@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "has-proto@npm:1.0.1"
-  checksum: febc5b5b531de8022806ad7407935e2135f1cc9e64636c3916c6842bd7995994ca3b29871ecd7954bd35f9e2986c17b3b227880484d22259e2f8e6ce63fd383e
+"has-proto@npm:^1.0.1, has-proto@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "has-proto@npm:1.0.3"
+  checksum: fe7c3d50b33f50f3933a04413ed1f69441d21d2d2944f81036276d30635cad9279f6b43bc8f32036c31ebdfcf6e731150f46c1907ad90c669ffe9b066c3ba5c4
   languageName: node
   linkType: hard
 
 "has-symbols@npm:^1.0.2, has-symbols@npm:^1.0.3":
   version: 1.0.3
   resolution: "has-symbols@npm:1.0.3"
   checksum: a054c40c631c0d5741a8285010a0777ea0c068f99ed43e5d6eb12972da223f8af553a455132fdb0801bdcfa0e0f443c0c03a68d8555aa529b3144b446c3f2410
   languageName: node
   linkType: hard
 
-"has-tostringtag@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "has-tostringtag@npm:1.0.0"
+"has-tostringtag@npm:^1.0.0, has-tostringtag@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "has-tostringtag@npm:1.0.2"
   dependencies:
-    has-symbols: ^1.0.2
-  checksum: cc12eb28cb6ae22369ebaad3a8ab0799ed61270991be88f208d508076a1e99abe4198c965935ce85ea90b60c94ddda73693b0920b58e7ead048b4a391b502c1c
+    has-symbols: ^1.0.3
+  checksum: 999d60bb753ad714356b2c6c87b7fb74f32463b8426e159397da4bde5bca7e598ab1073f4d8d4deafac297f2eb311484cd177af242776bf05f0d11565680468d
   languageName: node
   linkType: hard
 
-"has@npm:^1.0.3":
-  version: 1.0.3
-  resolution: "has@npm:1.0.3"
+"hasown@npm:^2.0.0, hasown@npm:^2.0.1, hasown@npm:^2.0.2":
+  version: 2.0.2
+  resolution: "hasown@npm:2.0.2"
   dependencies:
-    function-bind: ^1.1.1
-  checksum: b9ad53d53be4af90ce5d1c38331e712522417d017d5ef1ebd0507e07c2fbad8686fffb8e12ddecd4c39ca9b9b47431afbb975b8abf7f3c3b82c98e9aad052792
+    function-bind: ^1.1.2
+  checksum: e8516f776a15149ca6c6ed2ae3110c417a00b62260e222590e54aa367cbcd6ed99122020b37b7fbdf05748df57b265e70095d7bf35a47660587619b15ffb93db
   languageName: node
   linkType: hard
 
 "hosted-git-info@npm:^2.1.4":
   version: 2.8.9
   resolution: "hosted-git-info@npm:2.8.9"
   checksum: c955394bdab888a1e9bb10eb33029e0f7ce5a2ac7b3f158099dc8c486c99e73809dca609f5694b223920ca2174db33d32b12f9a2a47141dc59607c29da5a62dd
@@ -3721,28 +3573,14 @@
     domhandler: ^4.0.0
     domutils: ^2.5.2
     entities: ^2.0.0
   checksum: 81a7b3d9c3bb9acb568a02fc9b1b81ffbfa55eae7f1c41ae0bf840006d1dbf54cb3aa245b2553e2c94db674840a9f0fdad7027c9a9d01a062065314039058c4e
   languageName: node
   linkType: hard
 
-"human-signals@npm:^2.1.0":
-  version: 2.1.0
-  resolution: "human-signals@npm:2.1.0"
-  checksum: b87fd89fce72391625271454e70f67fe405277415b48bcc0117ca73d31fa23a4241787afdc8d67f5a116cf37258c052f59ea82daffa72364d61351423848e3b8
-  languageName: node
-  linkType: hard
-
-"human-signals@npm:^4.3.0":
-  version: 4.3.1
-  resolution: "human-signals@npm:4.3.1"
-  checksum: 6f12958df3f21b6fdaf02d90896c271df00636a31e2bbea05bddf817a35c66b38a6fdac5863e2df85bd52f34958997f1f50350ff97249e1dff8452865d5235d1
-  languageName: node
-  linkType: hard
-
 "iconv-lite@npm:^0.6.2":
   version: 0.6.3
   resolution: "iconv-lite@npm:0.6.3"
   dependencies:
     safer-buffer: ">= 2.1.2 < 3.0.0"
   checksum: 3f60d47a5c8fc3313317edfd29a00a692cc87a19cac0159e2ce711d0ebc9019064108323b5e493625e25594f11c6236647d8e256fbe7a58f4a3b33b89e6d30bf
   languageName: node
@@ -3754,17 +3592,17 @@
   peerDependencies:
     postcss: ^8.1.0
   checksum: 5c324d283552b1269cfc13a503aaaa172a280f914e5b81544f3803bc6f06a3b585fb79f66f7c771a2c052db7982c18bf92d001e3b47282e3abbbb4c4cc488d68
   languageName: node
   linkType: hard
 
 "ignore@npm:^5.2.0, ignore@npm:^5.2.4":
-  version: 5.2.4
-  resolution: "ignore@npm:5.2.4"
-  checksum: 3d4c309c6006e2621659311783eaea7ebcd41fe4ca1d78c91c473157ad6666a57a2df790fe0d07a12300d9aac2888204d7be8d59f9aaf665b1c7fcdb432517ef
+  version: 5.3.1
+  resolution: "ignore@npm:5.3.1"
+  checksum: 71d7bb4c1dbe020f915fd881108cbe85a0db3d636a0ea3ba911393c53946711d13a9b1143c7e70db06d571a5822c0a324a6bcde5c9904e7ca5047f01f1bf8cd3
   languageName: node
   linkType: hard
 
 "import-fresh@npm:^3.2.1, import-fresh@npm:^3.3.0":
   version: 3.3.0
   resolution: "import-fresh@npm:3.3.0"
   dependencies:
@@ -3827,40 +3665,39 @@
 "ini@npm:^1.3.5":
   version: 1.3.8
   resolution: "ini@npm:1.3.8"
   checksum: dfd98b0ca3a4fc1e323e38a6c8eb8936e31a97a918d3b377649ea15bdb15d481207a0dda1021efbd86b464cae29a0d33c1d7dcaf6c5672bee17fa849bc50a1b3
   languageName: node
   linkType: hard
 
-"internal-slot@npm:^1.0.5":
-  version: 1.0.5
-  resolution: "internal-slot@npm:1.0.5"
+"internal-slot@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "internal-slot@npm:1.0.7"
   dependencies:
-    get-intrinsic: ^1.2.0
-    has: ^1.0.3
+    es-errors: ^1.3.0
+    hasown: ^2.0.0
     side-channel: ^1.0.4
-  checksum: 97e84046bf9e7574d0956bd98d7162313ce7057883b6db6c5c7b5e5f05688864b0978ba07610c726d15d66544ffe4b1050107d93f8a39ebc59b15d8b429b497a
+  checksum: cadc5eea5d7d9bc2342e93aae9f31f04c196afebb11bde97448327049f492cd7081e18623ae71388aac9cd237b692ca3a105be9c68ac39c1dec679d7409e33eb
   languageName: node
   linkType: hard
 
 "interpret@npm:^3.1.1":
   version: 3.1.1
   resolution: "interpret@npm:3.1.1"
   checksum: 35cebcf48c7351130437596d9ab8c8fe131ce4038da4561e6d665f25640e0034702a031cf7e3a5cea60ac7ac548bf17465e0571ede126f3d3a6933152171ac82
   languageName: node
   linkType: hard
 
-"is-array-buffer@npm:^3.0.1, is-array-buffer@npm:^3.0.2":
-  version: 3.0.2
-  resolution: "is-array-buffer@npm:3.0.2"
+"is-array-buffer@npm:^3.0.4":
+  version: 3.0.4
+  resolution: "is-array-buffer@npm:3.0.4"
   dependencies:
     call-bind: ^1.0.2
-    get-intrinsic: ^1.2.0
-    is-typed-array: ^1.1.10
-  checksum: dcac9dda66ff17df9cabdc58214172bf41082f956eab30bb0d86bc0fab1e44b690fc8e1f855cf2481245caf4e8a5a006a982a71ddccec84032ed41f9d8da8c14
+    get-intrinsic: ^1.2.1
+  checksum: e4e3e6ef0ff2239e75371d221f74bc3c26a03564a22efb39f6bb02609b598917ddeecef4e8c877df2a25888f247a98198959842a5e73236bc7f22cabdf6351a7
   languageName: node
   linkType: hard
 
 "is-arrayish@npm:^0.2.1":
   version: 0.2.1
   resolution: "is-arrayish@npm:0.2.1"
   checksum: eef4417e3c10e60e2c810b6084942b3ead455af16c4509959a27e490e7aee87cfb3f38e01bbde92220b528a0ee1a18d52b787e1458ee86174d8c7f0e58cd488f
@@ -3890,49 +3727,40 @@
   version: 1.2.7
   resolution: "is-callable@npm:1.2.7"
   checksum: 61fd57d03b0d984e2ed3720fb1c7a897827ea174bd44402878e059542ea8c4aeedee0ea0985998aa5cc2736b2fa6e271c08587addb5b3959ac52cf665173d1ac
   languageName: node
   linkType: hard
 
 "is-core-module@npm:^2.13.0, is-core-module@npm:^2.5.0":
-  version: 2.13.0
-  resolution: "is-core-module@npm:2.13.0"
+  version: 2.13.1
+  resolution: "is-core-module@npm:2.13.1"
   dependencies:
-    has: ^1.0.3
-  checksum: 053ab101fb390bfeb2333360fd131387bed54e476b26860dc7f5a700bbf34a0ec4454f7c8c4d43e8a0030957e4b3db6e16d35e1890ea6fb654c833095e040355
+    hasown: ^2.0.0
+  checksum: 256559ee8a9488af90e4bad16f5583c6d59e92f0742e9e8bb4331e758521ee86b810b93bae44f390766ffbc518a0488b18d9dab7da9a5ff997d499efc9403f7c
+  languageName: node
+  linkType: hard
+
+"is-data-view@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "is-data-view@npm:1.0.1"
+  dependencies:
+    is-typed-array: ^1.1.13
+  checksum: 4ba4562ac2b2ec005fefe48269d6bd0152785458cd253c746154ffb8a8ab506a29d0cfb3b74af87513843776a88e4981ae25c89457bf640a33748eab1a7216b5
   languageName: node
   linkType: hard
 
 "is-date-object@npm:^1.0.1":
   version: 1.0.5
   resolution: "is-date-object@npm:1.0.5"
   dependencies:
     has-tostringtag: ^1.0.0
   checksum: baa9077cdf15eb7b58c79398604ca57379b2fc4cf9aa7a9b9e295278648f628c9b201400c01c5e0f7afae56507d741185730307cbe7cad3b9f90a77e5ee342fc
   languageName: node
   linkType: hard
 
-"is-docker@npm:^2.0.0":
-  version: 2.2.1
-  resolution: "is-docker@npm:2.2.1"
-  bin:
-    is-docker: cli.js
-  checksum: 3fef7ddbf0be25958e8991ad941901bf5922ab2753c46980b60b05c1bf9c9c2402d35e6dc32e4380b980ef5e1970a5d9d5e5aa2e02d77727c3b6b5e918474c56
-  languageName: node
-  linkType: hard
-
-"is-docker@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "is-docker@npm:3.0.0"
-  bin:
-    is-docker: cli.js
-  checksum: b698118f04feb7eaf3338922bd79cba064ea54a1c3db6ec8c0c8d8ee7613e7e5854d802d3ef646812a8a3ace81182a085dfa0a71cc68b06f3fa794b9783b3c90
-  languageName: node
-  linkType: hard
-
 "is-extglob@npm:^2.1.1":
   version: 2.1.1
   resolution: "is-extglob@npm:2.1.1"
   checksum: df033653d06d0eb567461e58a7a8c9f940bd8c22274b94bf7671ab36df5719791aae15eef6d83bbb5e23283967f2f984b8914559d4449efda578c775c4be6f85
   languageName: node
   linkType: hard
 
@@ -3948,29 +3776,18 @@
   resolution: "is-glob@npm:4.0.3"
   dependencies:
     is-extglob: ^2.1.1
   checksum: d381c1319fcb69d341cc6e6c7cd588e17cd94722d9a32dbd60660b993c4fb7d0f19438674e68dfec686d09b7c73139c9166b47597f846af387450224a8101ab4
   languageName: node
   linkType: hard
 
-"is-inside-container@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "is-inside-container@npm:1.0.0"
-  dependencies:
-    is-docker: ^3.0.0
-  bin:
-    is-inside-container: cli.js
-  checksum: c50b75a2ab66ab3e8b92b3bc534e1ea72ca25766832c0623ac22d134116a98bcf012197d1caabe1d1c4bd5f84363d4aa5c36bb4b585fbcaf57be172cd10a1a03
-  languageName: node
-  linkType: hard
-
-"is-negative-zero@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "is-negative-zero@npm:2.0.2"
-  checksum: f3232194c47a549da60c3d509c9a09be442507616b69454716692e37ae9f37c4dea264fb208ad0c9f3efd15a796a46b79df07c7e53c6227c32170608b809149a
+"is-negative-zero@npm:^2.0.3":
+  version: 2.0.3
+  resolution: "is-negative-zero@npm:2.0.3"
+  checksum: c1e6b23d2070c0539d7b36022d5a94407132411d01aba39ec549af824231f3804b1aea90b5e4e58e807a65d23ceb538ed6e355ce76b267bdd86edb757ffcbdcd
   languageName: node
   linkType: hard
 
 "is-number-object@npm:^1.0.4":
   version: 1.0.7
   resolution: "is-number-object@npm:1.0.7"
   dependencies:
@@ -4022,34 +3839,20 @@
   dependencies:
     call-bind: ^1.0.2
     has-tostringtag: ^1.0.0
   checksum: 362399b33535bc8f386d96c45c9feb04cf7f8b41c182f54174c1a45c9abbbe5e31290bbad09a458583ff6bf3b2048672cdb1881b13289569a7c548370856a652
   languageName: node
   linkType: hard
 
-"is-shared-array-buffer@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "is-shared-array-buffer@npm:1.0.2"
+"is-shared-array-buffer@npm:^1.0.2, is-shared-array-buffer@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "is-shared-array-buffer@npm:1.0.3"
   dependencies:
-    call-bind: ^1.0.2
-  checksum: 9508929cf14fdc1afc9d61d723c6e8d34f5e117f0bffda4d97e7a5d88c3a8681f633a74f8e3ad1fe92d5113f9b921dc5ca44356492079612f9a247efbce7032a
-  languageName: node
-  linkType: hard
-
-"is-stream@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "is-stream@npm:2.0.1"
-  checksum: b8e05ccdf96ac330ea83c12450304d4a591f9958c11fd17bed240af8d5ffe08aedafa4c0f4cfccd4d28dc9d4d129daca1023633d5c11601a6cbc77521f6fae66
-  languageName: node
-  linkType: hard
-
-"is-stream@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "is-stream@npm:3.0.0"
-  checksum: 172093fe99119ffd07611ab6d1bcccfe8bc4aa80d864b15f43e63e54b7abc71e779acd69afdb854c4e2a67fdc16ae710e370eda40088d1cfc956a50ed82d8f16
+    call-bind: ^1.0.7
+  checksum: a4fff602c309e64ccaa83b859255a43bb011145a42d3f56f67d9268b55bc7e6d98a5981a1d834186ad3105d6739d21547083fe7259c76c0468483fc538e716d8
   languageName: node
   linkType: hard
 
 "is-string@npm:^1.0.5, is-string@npm:^1.0.7":
   version: 1.0.7
   resolution: "is-string@npm:1.0.7"
   dependencies:
@@ -4063,41 +3866,32 @@
   resolution: "is-symbol@npm:1.0.4"
   dependencies:
     has-symbols: ^1.0.2
   checksum: 92805812ef590738d9de49d677cd17dfd486794773fb6fa0032d16452af46e9b91bb43ffe82c983570f015b37136f4b53b28b8523bfb10b0ece7a66c31a54510
   languageName: node
   linkType: hard
 
-"is-typed-array@npm:^1.1.10, is-typed-array@npm:^1.1.12, is-typed-array@npm:^1.1.9":
-  version: 1.1.12
-  resolution: "is-typed-array@npm:1.1.12"
+"is-typed-array@npm:^1.1.13":
+  version: 1.1.13
+  resolution: "is-typed-array@npm:1.1.13"
   dependencies:
-    which-typed-array: ^1.1.11
-  checksum: 4c89c4a3be07186caddadf92197b17fda663a9d259ea0d44a85f171558270d36059d1c386d34a12cba22dfade5aba497ce22778e866adc9406098c8fc4771796
+    which-typed-array: ^1.1.14
+  checksum: 150f9ada183a61554c91e1c4290086d2c100b0dff45f60b028519be72a8db964da403c48760723bf5253979b8dffe7b544246e0e5351dcd05c5fdb1dcc1dc0f0
   languageName: node
   linkType: hard
 
 "is-weakref@npm:^1.0.2":
   version: 1.0.2
   resolution: "is-weakref@npm:1.0.2"
   dependencies:
     call-bind: ^1.0.2
   checksum: 95bd9a57cdcb58c63b1c401c60a474b0f45b94719c30f548c891860f051bc2231575c290a6b420c6bc6e7ed99459d424c652bd5bf9a1d5259505dc35b4bf83de
   languageName: node
   linkType: hard
 
-"is-wsl@npm:^2.2.0":
-  version: 2.2.0
-  resolution: "is-wsl@npm:2.2.0"
-  dependencies:
-    is-docker: ^2.0.0
-  checksum: 20849846ae414997d290b75e16868e5261e86ff5047f104027026fd61d8b5a9b0b3ade16239f35e1a067b3c7cc02f70183cb661010ed16f4b6c7c93dad1b19d8
-  languageName: node
-  linkType: hard
-
 "isarray@npm:^2.0.5":
   version: 2.0.5
   resolution: "isarray@npm:2.0.5"
   checksum: bd5bbe4104438c4196ba58a54650116007fa0262eccef13a4c55b2e09a5b36b59f1e75b9fcc49883dd9d4953892e6fc007eef9e9155648ceea036e184b0f930a
   languageName: node
   linkType: hard
 
@@ -4118,24 +3912,24 @@
 "isomorphic.js@npm:^0.2.4":
   version: 0.2.5
   resolution: "isomorphic.js@npm:0.2.5"
   checksum: d8d1b083f05f3c337a06628b982ac3ce6db953bbef14a9de8ad49131250c3592f864b73c12030fdc9ef138ce97b76ef55c7d96a849561ac215b1b4b9d301c8e9
   languageName: node
   linkType: hard
 
-"jackspeak@npm:^2.0.3":
-  version: 2.3.3
-  resolution: "jackspeak@npm:2.3.3"
+"jackspeak@npm:^2.3.6":
+  version: 2.3.6
+  resolution: "jackspeak@npm:2.3.6"
   dependencies:
     "@isaacs/cliui": ^8.0.2
     "@pkgjs/parseargs": ^0.11.0
   dependenciesMeta:
     "@pkgjs/parseargs":
       optional: true
-  checksum: 4313a7c0cc44c7753c4cb9869935f0b06f4cf96827515f63f58ff46b3d2f6e29aba6b3b5151778397c3f5ae67ef8bfc48871967bd10343c27e90cff198ec7808
+  checksum: 57d43ad11eadc98cdfe7496612f6bbb5255ea69fe51ea431162db302c2a11011642f50cfad57288bd0aea78384a0612b16e131944ad8ecd09d619041c8531b54
   languageName: node
   linkType: hard
 
 "jest-worker@npm:^27.4.5":
   version: 27.5.1
   resolution: "jest-worker@npm:27.5.1"
   dependencies:
@@ -4252,55 +4046,56 @@
   version: 5.0.1
   resolution: "jsonpointer@npm:5.0.1"
   checksum: 0b40f712900ad0c846681ea2db23b6684b9d5eedf55807b4708c656f5894b63507d0e28ae10aa1bddbea551241035afe62b6df0800fc94c2e2806a7f3adecd7c
   languageName: node
   linkType: hard
 
 "keyv@npm:^4.5.3":
-  version: 4.5.3
-  resolution: "keyv@npm:4.5.3"
+  version: 4.5.4
+  resolution: "keyv@npm:4.5.4"
   dependencies:
     json-buffer: 3.0.1
-  checksum: 3ffb4d5b72b6b4b4af443bbb75ca2526b23c750fccb5ac4c267c6116888b4b65681015c2833cb20d26cf3e6e32dac6b988c77f7f022e1a571b7d90f1442257da
+  checksum: 74a24395b1c34bd44ad5cb2b49140d087553e170625240b86755a6604cd65aa16efdbdeae5cdb17ba1284a0fbb25ad06263755dbc71b8d8b06f74232ce3cdd72
   languageName: node
   linkType: hard
 
 "kind-of@npm:^6.0.2, kind-of@npm:^6.0.3":
   version: 6.0.3
   resolution: "kind-of@npm:6.0.3"
   checksum: 3ab01e7b1d440b22fe4c31f23d8d38b4d9b91d9f291df683476576493d5dfd2e03848a8b05813dd0c3f0e835bc63f433007ddeceb71f05cb25c45ae1b19c6d3b
   languageName: node
   linkType: hard
 
-"known-css-properties@npm:^0.28.0":
-  version: 0.28.0
-  resolution: "known-css-properties@npm:0.28.0"
-  checksum: c9e0d6948e31386e872d348eb955e9db80edd58f9d7f7fc9b072180bfb26708a629d5942d4478f66fc766fb913c4552a220950730cef85f8c3bc9830e33b00c8
+"known-css-properties@npm:^0.29.0":
+  version: 0.29.0
+  resolution: "known-css-properties@npm:0.29.0"
+  checksum: daa6562e907f856cbfd58a00c42f532c9bba283388984da6a3bffb494e56612e5f23c52f30b0d9885f0ea07ad5d88bfa0470ee65017a6ce6c565289a1afd78af
   languageName: node
   linkType: hard
 
 "levn@npm:^0.4.1":
   version: 0.4.1
   resolution: "levn@npm:0.4.1"
   dependencies:
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
-"lib0@npm:^0.2.74, lib0@npm:^0.2.85":
-  version: 0.2.85
-  resolution: "lib0@npm:0.2.85"
+"lib0@npm:^0.2.85, lib0@npm:^0.2.86":
+  version: 0.2.93
+  resolution: "lib0@npm:0.2.93"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
+    0ecdsa-generate-keypair: bin/0ecdsa-generate-keypair.js
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: 6a3c5c5c3f37f0940eff9309b2595f9a77822f521773db773e0d809309ccf5e6ecab8f39cc47b55b6b167f60b3824c44bb7d92b5c9ffb81a3f331b21277906d2
+  checksum: 4c482aba249c471316fdec360ee4ace2a70ae42faad5fb6862aebb6786e187de9470eb082a5675489c59ffe54b005a15711a3d7dba33764bcab56349e61a1520
   languageName: node
   linkType: hard
 
 "license-webpack-plugin@npm:^2.3.14":
   version: 2.3.21
   resolution: "license-webpack-plugin@npm:2.3.21"
   dependencies:
@@ -4417,50 +4212,50 @@
     js-tokens: ^3.0.0 || ^4.0.0
   bin:
     loose-envify: cli.js
   checksum: 6517e24e0cad87ec9888f500c5b5947032cdfe6ef65e1c1936a0c48a524b81e65542c9c3edc91c97d5bddc806ee2a985dbc79be89215d613b1de5db6d1cfe6f4
   languageName: node
   linkType: hard
 
+"lru-cache@npm:^10.2.0":
+  version: 10.2.0
+  resolution: "lru-cache@npm:10.2.0"
+  checksum: eee7ddda4a7475deac51ac81d7dd78709095c6fa46e8350dc2d22462559a1faa3b81ed931d5464b13d48cbd7e08b46100b6f768c76833912bc444b99c37e25db
+  languageName: node
+  linkType: hard
+
 "lru-cache@npm:^6.0.0":
   version: 6.0.0
   resolution: "lru-cache@npm:6.0.0"
   dependencies:
     yallist: ^4.0.0
   checksum: f97f499f898f23e4585742138a22f22526254fdba6d75d41a1c2526b3b6cc5747ef59c5612ba7375f42aca4f8461950e925ba08c991ead0651b4918b7c978297
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^9.1.1 || ^10.0.0":
-  version: 10.0.1
-  resolution: "lru-cache@npm:10.0.1"
-  checksum: 06f8d0e1ceabd76bb6f644a26dbb0b4c471b79c7b514c13c6856113879b3bf369eb7b497dad4ff2b7e2636db202412394865b33c332100876d838ad1372f0181
-  languageName: node
-  linkType: hard
-
 "map-obj@npm:^1.0.0":
   version: 1.0.1
   resolution: "map-obj@npm:1.0.1"
   checksum: 9949e7baec2a336e63b8d4dc71018c117c3ce6e39d2451ccbfd3b8350c547c4f6af331a4cbe1c83193d7c6b786082b6256bde843db90cb7da2a21e8fcc28afed
   languageName: node
   linkType: hard
 
 "map-obj@npm:^4.1.0":
   version: 4.3.0
   resolution: "map-obj@npm:4.3.0"
   checksum: fbc554934d1a27a1910e842bc87b177b1a556609dd803747c85ece420692380827c6ae94a95cce4407c054fa0964be3bf8226f7f2cb2e9eeee432c7c1985684e
   languageName: node
   linkType: hard
 
-"markdown-to-jsx@npm:^7.3.2":
-  version: 7.3.2
-  resolution: "markdown-to-jsx@npm:7.3.2"
+"markdown-to-jsx@npm:^7.4.1":
+  version: 7.4.7
+  resolution: "markdown-to-jsx@npm:7.4.7"
   peerDependencies:
     react: ">= 0.14.0"
-  checksum: 8885c6343b71570b0a7ec16cd85a49b853a830234790ee7430e2517ea5d8d361ff138bd52147f650790f3e7b3a28a15c755fc16f8856dd01ddf09a6161782e06
+  checksum: bb8a696c8a95dd67ac1eb44255f31cf17e60b6c2ff03bfcd51b5e28da17856c57d7a16da59fda7f3a4eedb01d7e92eeef57a10ff3abd5431e5c80059d4565016
   languageName: node
   linkType: hard
 
 "mathml-tag-names@npm:^2.1.3":
   version: 2.1.3
   resolution: "mathml-tag-names@npm:2.1.3"
   checksum: 1201a25a137d6b9e328facd67912058b8b45b19a6c4cc62641c9476195da28a275ca6e0eca070af5378b905c2b11abc1114676ba703411db0b9ce007de921ad0
@@ -4537,70 +4332,66 @@
   resolution: "mime-types@npm:2.1.35"
   dependencies:
     mime-db: 1.52.0
   checksum: 89a5b7f1def9f3af5dad6496c5ed50191ae4331cc5389d7c521c8ad28d5fdad2d06fd81baf38fed813dc4e46bb55c8145bb0ff406330818c9cf712fb2e9b3836
   languageName: node
   linkType: hard
 
-"mimic-fn@npm:^2.1.0":
-  version: 2.1.0
-  resolution: "mimic-fn@npm:2.1.0"
-  checksum: d2421a3444848ce7f84bd49115ddacff29c15745db73f54041edc906c14b131a38d05298dae3081667627a59b2eb1ca4b436ff2e1b80f69679522410418b478a
-  languageName: node
-  linkType: hard
-
-"mimic-fn@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "mimic-fn@npm:4.0.0"
-  checksum: 995dcece15ee29aa16e188de6633d43a3db4611bcf93620e7e62109ec41c79c0f34277165b8ce5e361205049766e371851264c21ac64ca35499acb5421c2ba56
-  languageName: node
-  linkType: hard
-
 "min-indent@npm:^1.0.1":
   version: 1.0.1
   resolution: "min-indent@npm:1.0.1"
   checksum: bfc6dd03c5eaf623a4963ebd94d087f6f4bbbfd8c41329a7f09706b0cb66969c4ddd336abeb587bc44bc6f08e13bf90f0b374f9d71f9f01e04adc2cd6f083ef1
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
-  version: 2.7.6
-  resolution: "mini-css-extract-plugin@npm:2.7.6"
+  version: 2.9.0
+  resolution: "mini-css-extract-plugin@npm:2.9.0"
   dependencies:
     schema-utils: ^4.0.0
+    tapable: ^2.2.1
   peerDependencies:
     webpack: ^5.0.0
-  checksum: be6f7cefc6275168eb0a6b8fe977083a18c743c9612c9f00e6c1a62c3393ca7960e93fba1a7ebb09b75f36a0204ad087d772c1ef574bc29c90c0e8175a3c0b83
+  checksum: ae192c67ba85ac8bffeab66774635bf90181f00d5dd6cf95412426192599ddf5506fb4b1550acbd7a5476476e39db53c770dd40f8378f7baf5de96e3fec4e6e9
   languageName: node
   linkType: hard
 
 "mini-svg-data-uri@npm:^1.4.4":
   version: 1.4.4
   resolution: "mini-svg-data-uri@npm:1.4.4"
   bin:
     mini-svg-data-uri: cli.js
   checksum: 997f1fbd8d59a70f03761e18626d335197a3479cb9d1ff75678e4b64b864d32a0b8fc18115eabde035e5299b8b4a354a78e57dd6ac10f9d604162a6170898d09
   languageName: node
   linkType: hard
 
+"minimatch@npm:9.0.3":
+  version: 9.0.3
+  resolution: "minimatch@npm:9.0.3"
+  dependencies:
+    brace-expansion: ^2.0.1
+  checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
+  languageName: node
+  linkType: hard
+
 "minimatch@npm:^3.0.4, minimatch@npm:^3.0.5, minimatch@npm:^3.1.1, minimatch@npm:^3.1.2":
   version: 3.1.2
   resolution: "minimatch@npm:3.1.2"
   dependencies:
     brace-expansion: ^1.1.7
   checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
   languageName: node
   linkType: hard
 
 "minimatch@npm:^9.0.1":
-  version: 9.0.3
-  resolution: "minimatch@npm:9.0.3"
+  version: 9.0.4
+  resolution: "minimatch@npm:9.0.4"
   dependencies:
     brace-expansion: ^2.0.1
-  checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
+  checksum: cf717f597ec3eed7dabc33153482a2e8d49f4fd3c26e58fd9c71a94c5029a0838728841b93f46bf1263b65a8010e2ee800d0dc9b004ab8ba8b6d1ec07cc115b5
   languageName: node
   linkType: hard
 
 "minimist-options@npm:4.1.0":
   version: 4.1.0
   resolution: "minimist-options@npm:4.1.0"
   dependencies:
@@ -4614,18 +4405,18 @@
 "minimist@npm:~1.2.0":
   version: 1.2.8
   resolution: "minimist@npm:1.2.8"
   checksum: 75a6d645fb122dad29c06a7597bddea977258957ed88d7a6df59b5cd3fe4a527e253e9bbf2e783e4b73657f9098b96a5fe96ab8a113655d4109108577ecf85b0
   languageName: node
   linkType: hard
 
-"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0":
-  version: 7.0.3
-  resolution: "minipass@npm:7.0.3"
-  checksum: 6f1614f5b5b55568a46bca5fec0e7c46dac027691db27d0e1923a8192866903144cd962ac772c0e9f89b608ea818b702709c042bce98e190d258847d85461531
+"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0, minipass@npm:^7.0.4":
+  version: 7.0.4
+  resolution: "minipass@npm:7.0.4"
+  checksum: 87585e258b9488caf2e7acea242fd7856bbe9a2c84a7807643513a338d66f368c7d518200ad7b70a508664d408aa000517647b2930c259a8b1f9f0984f344a21
   languageName: node
   linkType: hard
 
 "mkdirp@npm:^1.0.3":
   version: 1.0.4
   resolution: "mkdirp@npm:1.0.4"
   bin:
@@ -4637,20 +4428,20 @@
 "ms@npm:2.1.2":
   version: 2.1.2
   resolution: "ms@npm:2.1.2"
   checksum: 673cdb2c3133eb050c745908d8ce632ed2c02d85640e2edb3ace856a2266a813b30c613569bf3354fdf4ea7d1a1494add3bfa95e2713baa27d0c2c71fc44f58f
   languageName: node
   linkType: hard
 
-"nanoid@npm:^3.3.6":
-  version: 3.3.6
-  resolution: "nanoid@npm:3.3.6"
+"nanoid@npm:^3.3.7":
+  version: 3.3.7
+  resolution: "nanoid@npm:3.3.7"
   bin:
     nanoid: bin/nanoid.cjs
-  checksum: 7d0eda657002738aa5206107bd0580aead6c95c460ef1bdd0b1a87a9c7ae6277ac2e9b945306aaa5b32c6dcb7feaf462d0f552e7f8b5718abfc6ead5c94a71b3
+  checksum: d36c427e530713e4ac6567d488b489a36582ef89da1d6d4e3b87eded11eb10d7042a877958c6f104929809b2ab0bafa17652b076cdf84324aa75b30b722204f2
   languageName: node
   linkType: hard
 
 "natural-compare@npm:^1.4.0":
   version: 1.4.0
   resolution: "natural-compare@npm:1.4.0"
   checksum: 23ad088b08f898fc9b53011d7bb78ec48e79de7627e01ab5518e806033861bef68d5b0cd0e2205c2f36690ac9571ff6bcb05eb777ced2eeda8d4ac5b44592c3d
@@ -4667,18 +4458,18 @@
 "nice-try@npm:^1.0.4":
   version: 1.0.5
   resolution: "nice-try@npm:1.0.5"
   checksum: 0b4af3b5bb5d86c289f7a026303d192a7eb4417231fe47245c460baeabae7277bcd8fd9c728fb6bd62c30b3e15cd6620373e2cf33353b095d8b403d3e8a15aff
   languageName: node
   linkType: hard
 
-"node-releases@npm:^2.0.13":
-  version: 2.0.13
-  resolution: "node-releases@npm:2.0.13"
-  checksum: 17ec8f315dba62710cae71a8dad3cd0288ba943d2ece43504b3b1aa8625bf138637798ab470b1d9035b0545996f63000a8a926e0f6d35d0996424f8b6d36dda3
+"node-releases@npm:^2.0.14":
+  version: 2.0.14
+  resolution: "node-releases@npm:2.0.14"
+  checksum: 59443a2f77acac854c42d321bf1b43dea0aef55cd544c6a686e9816a697300458d4e82239e2d794ea05f7bbbc8a94500332e2d3ac3f11f52e4b16cbe638b3c41
   languageName: node
   linkType: hard
 
 "normalize-package-data@npm:^2.3.2":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
@@ -4726,104 +4517,56 @@
     npm-run-all: bin/npm-run-all/index.js
     run-p: bin/run-p/index.js
     run-s: bin/run-s/index.js
   checksum: 373b72c6a36564da13c1642c1fd9bb4dcc756bce7a3648f883772f02661095319820834ff813762d2fee403e9b40c1cd27c8685807c107440f10eb19c006d4a0
   languageName: node
   linkType: hard
 
-"npm-run-path@npm:^4.0.1":
-  version: 4.0.1
-  resolution: "npm-run-path@npm:4.0.1"
-  dependencies:
-    path-key: ^3.0.0
-  checksum: 5374c0cea4b0bbfdfae62da7bbdf1e1558d338335f4cacf2515c282ff358ff27b2ecb91ffa5330a8b14390ac66a1e146e10700440c1ab868208430f56b5f4d23
-  languageName: node
-  linkType: hard
-
-"npm-run-path@npm:^5.1.0":
-  version: 5.1.0
-  resolution: "npm-run-path@npm:5.1.0"
-  dependencies:
-    path-key: ^4.0.0
-  checksum: dc184eb5ec239d6a2b990b43236845332ef12f4e0beaa9701de724aa797fe40b6bbd0157fb7639d24d3ab13f5d5cf22d223a19c6300846b8126f335f788bee66
-  languageName: node
-  linkType: hard
-
 "object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
   languageName: node
   linkType: hard
 
-"object-inspect@npm:^1.12.3, object-inspect@npm:^1.9.0":
-  version: 1.12.3
-  resolution: "object-inspect@npm:1.12.3"
-  checksum: dabfd824d97a5f407e6d5d24810d888859f6be394d8b733a77442b277e0808860555176719c5905e765e3743a7cada6b8b0a3b85e5331c530fd418cc8ae991db
+"object-inspect@npm:^1.13.1":
+  version: 1.13.1
+  resolution: "object-inspect@npm:1.13.1"
+  checksum: 7d9fa9221de3311dcb5c7c307ee5dc011cdd31dc43624b7c184b3840514e118e05ef0002be5388304c416c0eb592feb46e983db12577fc47e47d5752fbbfb61f
   languageName: node
   linkType: hard
 
 "object-keys@npm:^1.1.1":
   version: 1.1.1
   resolution: "object-keys@npm:1.1.1"
   checksum: b363c5e7644b1e1b04aa507e88dcb8e3a2f52b6ffd0ea801e4c7a62d5aa559affe21c55a07fd4b1fd55fc03a33c610d73426664b20032405d7b92a1414c34d6a
   languageName: node
   linkType: hard
 
-"object.assign@npm:^4.1.4":
-  version: 4.1.4
-  resolution: "object.assign@npm:4.1.4"
+"object.assign@npm:^4.1.5":
+  version: 4.1.5
+  resolution: "object.assign@npm:4.1.5"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.1.4
+    call-bind: ^1.0.5
+    define-properties: ^1.2.1
     has-symbols: ^1.0.3
     object-keys: ^1.1.1
-  checksum: 76cab513a5999acbfe0ff355f15a6a125e71805fcf53de4e9d4e082e1989bdb81d1e329291e1e4e0ae7719f0e4ef80e88fb2d367ae60500d79d25a6224ac8864
+  checksum: f9aeac0541661370a1fc86e6a8065eb1668d3e771f7dbb33ee54578201336c057b21ee61207a186dd42db0c62201d91aac703d20d12a79fc79c353eed44d4e25
   languageName: node
   linkType: hard
 
 "once@npm:^1.3.0":
   version: 1.4.0
   resolution: "once@npm:1.4.0"
   dependencies:
     wrappy: 1
   checksum: cd0a88501333edd640d95f0d2700fbde6bff20b3d4d9bdc521bdd31af0656b5706570d6c6afe532045a20bb8dc0849f8332d6f2a416e0ba6d3d3b98806c7db68
   languageName: node
   linkType: hard
 
-"onetime@npm:^5.1.2":
-  version: 5.1.2
-  resolution: "onetime@npm:5.1.2"
-  dependencies:
-    mimic-fn: ^2.1.0
-  checksum: 2478859ef817fc5d4e9c2f9e5728512ddd1dbc9fb7829ad263765bb6d3b91ce699d6e2332eef6b7dff183c2f490bd3349f1666427eaba4469fba0ac38dfd0d34
-  languageName: node
-  linkType: hard
-
-"onetime@npm:^6.0.0":
-  version: 6.0.0
-  resolution: "onetime@npm:6.0.0"
-  dependencies:
-    mimic-fn: ^4.0.0
-  checksum: 0846ce78e440841335d4e9182ef69d5762e9f38aa7499b19f42ea1c4cd40f0b4446094c455c713f9adac3f4ae86f613bb5e30c99e52652764d06a89f709b3788
-  languageName: node
-  linkType: hard
-
-"open@npm:^9.1.0":
-  version: 9.1.0
-  resolution: "open@npm:9.1.0"
-  dependencies:
-    default-browser: ^4.0.0
-    define-lazy-prop: ^3.0.0
-    is-inside-container: ^1.0.0
-    is-wsl: ^2.2.0
-  checksum: 3993c0f61d51fed8ac290e99c9c3cf45d3b6cfb3e2aa2b74cafd312c3486c22fd81df16ac8f3ab91dd8a4e3e729a16fc2480cfc406c4833416cf908acf1ae7c9
-  languageName: node
-  linkType: hard
-
 "optionator@npm:^0.9.3":
   version: 0.9.3
   resolution: "optionator@npm:0.9.3"
   dependencies:
     "@aashutoshrathi/word-wrap": ^1.2.3
     deep-is: ^0.1.3
     fast-levenshtein: ^2.0.6
@@ -4939,42 +4682,35 @@
 "path-key@npm:^2.0.1":
   version: 2.0.1
   resolution: "path-key@npm:2.0.1"
   checksum: f7ab0ad42fe3fb8c7f11d0c4f849871e28fbd8e1add65c370e422512fc5887097b9cf34d09c1747d45c942a8c1e26468d6356e2df3f740bf177ab8ca7301ebfd
   languageName: node
   linkType: hard
 
-"path-key@npm:^3.0.0, path-key@npm:^3.1.0":
+"path-key@npm:^3.1.0":
   version: 3.1.1
   resolution: "path-key@npm:3.1.1"
   checksum: 55cd7a9dd4b343412a8386a743f9c746ef196e57c823d90ca3ab917f90ab9f13dd0ded27252ba49dbdfcab2b091d998bc446f6220cd3cea65db407502a740020
   languageName: node
   linkType: hard
 
-"path-key@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "path-key@npm:4.0.0"
-  checksum: 8e6c314ae6d16b83e93032c61020129f6f4484590a777eed709c4a01b50e498822b00f76ceaf94bc64dbd90b327df56ceadce27da3d83393790f1219e07721d7
-  languageName: node
-  linkType: hard
-
 "path-parse@npm:^1.0.7":
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
-"path-scurry@npm:^1.10.1":
-  version: 1.10.1
-  resolution: "path-scurry@npm:1.10.1"
+"path-scurry@npm:^1.10.2":
+  version: 1.10.2
+  resolution: "path-scurry@npm:1.10.2"
   dependencies:
-    lru-cache: ^9.1.1 || ^10.0.0
+    lru-cache: ^10.2.0
     minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
-  checksum: e2557cff3a8fb8bc07afdd6ab163a92587884f9969b05bbbaf6fe7379348bfb09af9ed292af12ed32398b15fb443e81692047b786d1eeb6d898a51eb17ed7d90
+  checksum: 6739b4290f7d1a949c61c758b481c07ac7d1a841964c68cf5e1fa153d7e18cbde4872b37aadf9c5173c800d627f219c47945859159de36c977dd82419997b9b8
   languageName: node
   linkType: hard
 
 "path-type@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-type@npm:3.0.0"
   dependencies:
@@ -5025,44 +4761,51 @@
   resolution: "pkg-dir@npm:4.2.0"
   dependencies:
     find-up: ^4.0.0
   checksum: 9863e3f35132bf99ae1636d31ff1e1e3501251d480336edb1c211133c8d58906bed80f154a1d723652df1fda91e01c7442c2eeaf9dc83157c7ae89087e43c8d6
   languageName: node
   linkType: hard
 
-"postcss-modules-extract-imports@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "postcss-modules-extract-imports@npm:3.0.0"
+"possible-typed-array-names@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "possible-typed-array-names@npm:1.0.0"
+  checksum: b32d403ece71e042385cc7856385cecf1cd8e144fa74d2f1de40d1e16035dba097bc189715925e79b67bdd1472796ff168d3a90d296356c9c94d272d5b95f3ae
+  languageName: node
+  linkType: hard
+
+"postcss-modules-extract-imports@npm:^3.1.0":
+  version: 3.1.0
+  resolution: "postcss-modules-extract-imports@npm:3.1.0"
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 4b65f2f1382d89c4bc3c0a1bdc5942f52f3cb19c110c57bd591ffab3a5fee03fcf831604168205b0c1b631a3dce2255c70b61aaae3ef39d69cd7eb450c2552d2
+  checksum: b9192e0f4fb3d19431558be6f8af7ca45fc92baaad9b2778d1732a5880cd25c3df2074ce5484ae491e224f0d21345ffc2d419bd51c25b019af76d7a7af88c17f
   languageName: node
   linkType: hard
 
-"postcss-modules-local-by-default@npm:^4.0.3":
-  version: 4.0.3
-  resolution: "postcss-modules-local-by-default@npm:4.0.3"
+"postcss-modules-local-by-default@npm:^4.0.5":
+  version: 4.0.5
+  resolution: "postcss-modules-local-by-default@npm:4.0.5"
   dependencies:
     icss-utils: ^5.0.0
     postcss-selector-parser: ^6.0.2
     postcss-value-parser: ^4.1.0
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 2f8083687f3d6067885f8863dd32dbbb4f779cfcc7e52c17abede9311d84faf6d3ed8760e7c54c6380281732ae1f78e5e56a28baf3c271b33f450a11c9e30485
+  checksum: ca9b01f4a0a3dfb33e016299e2dfb7e85c3123292f7aec2efc0c6771b9955648598bfb4c1561f7ee9732fb27fb073681233661b32eef98baab43743f96735452
   languageName: node
   linkType: hard
 
-"postcss-modules-scope@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "postcss-modules-scope@npm:3.0.0"
+"postcss-modules-scope@npm:^3.2.0":
+  version: 3.2.0
+  resolution: "postcss-modules-scope@npm:3.2.0"
   dependencies:
     postcss-selector-parser: ^6.0.4
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 330b9398dbd44c992c92b0dc612c0626135e2cc840fee41841eb61247a6cfed95af2bd6f67ead9dd9d0bb41f5b0367129d93c6e434fa3e9c58ade391d9a5a138
+  checksum: 2ffe7e98c1fa993192a39c8dd8ade93fc4f59fbd1336ce34fcedaee0ee3bafb29e2e23fb49189256895b30e4f21af661c6a6a16ef7b17ae2c859301e4a4459ae
   languageName: node
   linkType: hard
 
 "postcss-modules-values@npm:^4.0.0":
   version: 4.0.0
   resolution: "postcss-modules-values@npm:4.0.0"
   dependencies:
@@ -5086,38 +4829,38 @@
   peerDependencies:
     postcss: ^8.3.3
   checksum: 06c733eaad83a3954367e7ee02ddfe3796e7a44d4299ccf9239f40964a4daac153c7d77613f32964b5a86c0c6c2f6167738f31d578b73b17cb69d0c4446f0ebe
   languageName: node
   linkType: hard
 
 "postcss-selector-parser@npm:^6.0.13, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
-  version: 6.0.13
-  resolution: "postcss-selector-parser@npm:6.0.13"
+  version: 6.0.16
+  resolution: "postcss-selector-parser@npm:6.0.16"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
-  checksum: f89163338a1ce3b8ece8e9055cd5a3165e79a15e1c408e18de5ad8f87796b61ec2d48a2902d179ae0c4b5de10fccd3a325a4e660596549b040bc5ad1b465f096
+  checksum: e1cd68e33a39e3dc1e1e5bd8717be5bbe3cc23a4cecb466c3acb2f3a77daad7a47df4d6137a76f8db74cf160d2fb16b2cfdb4ccbebdfda844690f8d545fe281d
   languageName: node
   linkType: hard
 
 "postcss-value-parser@npm:^4.1.0, postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
-"postcss@npm:^8.3.11, postcss@npm:^8.4.21, postcss@npm:^8.4.27":
-  version: 8.4.30
-  resolution: "postcss@npm:8.4.30"
+"postcss@npm:^8.3.11, postcss@npm:^8.4.28, postcss@npm:^8.4.33":
+  version: 8.4.38
+  resolution: "postcss@npm:8.4.38"
   dependencies:
-    nanoid: ^3.3.6
+    nanoid: ^3.3.7
     picocolors: ^1.0.0
-    source-map-js: ^1.0.2
-  checksum: 6c810c10c9bd3e03ca016e0b6b6756261e640aba1a9a7b1200b55502bc34b9165e38f590aef3493afc2f30ab55cdfcd43fd0f8408d69a77318ddbcf2a8ad164b
+    source-map-js: ^1.2.0
+  checksum: 649f9e60a763ca4b5a7bbec446a069edf07f057f6d780a5a0070576b841538d1ecf7dd888f2fbfd1f76200e26c969e405aeeae66332e6927dbdc8bdcb90b9451
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
@@ -5129,20 +4872,20 @@
   resolution: "prettier-linter-helpers@npm:1.0.0"
   dependencies:
     fast-diff: ^1.1.2
   checksum: 00ce8011cf6430158d27f9c92cfea0a7699405633f7f1d4a45f07e21bf78e99895911cbcdc3853db3a824201a7c745bd49bfea8abd5fb9883e765a90f74f8392
   languageName: node
   linkType: hard
 
-"prettier@npm:^3.0.0":
-  version: 3.0.3
-  resolution: "prettier@npm:3.0.3"
+"prettier@npm:^3.2.5":
+  version: 3.2.5
+  resolution: "prettier@npm:3.2.5"
   bin:
     prettier: bin/prettier.cjs
-  checksum: e10b9af02b281f6c617362ebd2571b1d7fc9fb8a3bd17e371754428cda992e5e8d8b7a046e8f7d3e2da1dcd21aa001e2e3c797402ebb6111b5cd19609dd228e0
+  checksum: 2ee4e1417572372afb7a13bb446b34f20f1bf1747db77cf6ccaf57a9be005f2f15c40f903d41a6b79eec3f57fff14d32a20fb6dee1f126da48908926fe43c311
   languageName: node
   linkType: hard
 
 "process@npm:^0.11.10":
   version: 0.11.10
   resolution: "process@npm:0.11.10"
   checksum: bfcce49814f7d172a6e6a14d5fa3ac92cc3d0c3b9feb1279774708a719e19acd673995226351a082a9ae99978254e320ccda4240ddc474ba31a76c79491ca7c3
@@ -5157,17 +4900,17 @@
     object-assign: ^4.1.1
     react-is: ^16.13.1
   checksum: c056d3f1c057cb7ff8344c645450e14f088a915d078dcda795041765047fa080d38e5d626560ccaac94a4e16e3aa15f3557c1a9a8d1174530955e992c675e459
   languageName: node
   linkType: hard
 
 "punycode@npm:^2.1.0, punycode@npm:^2.1.1":
-  version: 2.3.0
-  resolution: "punycode@npm:2.3.0"
-  checksum: 39f760e09a2a3bbfe8f5287cf733ecdad69d6af2fe6f97ca95f24b8921858b91e9ea3c9eeec6e08cede96181b3bb33f95c6ffd8c77e63986508aa2e8159fa200
+  version: 2.3.1
+  resolution: "punycode@npm:2.3.1"
+  checksum: bb0a0ceedca4c3c57a9b981b90601579058903c62be23c5e8e843d2c2d4148a3ecf029d5133486fb0e1822b098ba8bba09e89d6b21742d02fa26bda6441a6fb2
   languageName: node
   linkType: hard
 
 "querystringify@npm:^2.1.1":
   version: 2.2.0
   resolution: "querystringify@npm:2.2.0"
   checksum: 5641ea231bad7ef6d64d9998faca95611ed4b11c2591a8cae741e178a974f6a8e0ebde008475259abe1621cb15e692404e6b6626e927f7b849d5c09392604b15
@@ -5219,15 +4962,15 @@
 "react-is@npm:^18.2.0":
   version: 18.2.0
   resolution: "react-is@npm:18.2.0"
   checksum: e72d0ba81b5922759e4aff17e0252bd29988f9642ed817f56b25a3e217e13eea8a7f2322af99a06edb779da12d5d636e9fda473d620df9a3da0df2a74141d53e
   languageName: node
   linkType: hard
 
-"react@npm:^18.2.0":
+"react@npm:>=17.0.0 <19.0.0, react@npm:^18.2.0":
   version: 18.2.0
   resolution: "react@npm:18.2.0"
   dependencies:
     loose-envify: ^1.1.0
   checksum: 88e38092da8839b830cda6feef2e8505dec8ace60579e46aa5490fc3dc9bba0bd50336507dc166f43e3afc1c42939c09fe33b25fae889d6f402721dcd78fca1b
   languageName: node
   linkType: hard
@@ -5281,22 +5024,23 @@
   dependencies:
     indent-string: ^5.0.0
     strip-indent: ^4.0.0
   checksum: 6944e7b1d8f3fd28c2515f5c605b9f7f0ea0f4edddf41890bbbdd4d9ee35abb7540c3b278f03ff827bd278bb6ff4a5bd8692ca406b748c5c1c3ce7355e9fbf8f
   languageName: node
   linkType: hard
 
-"regexp.prototype.flags@npm:^1.5.1":
-  version: 1.5.1
-  resolution: "regexp.prototype.flags@npm:1.5.1"
-  dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    set-function-name: ^2.0.0
-  checksum: 869edff00288442f8d7fa4c9327f91d85f3b3acf8cbbef9ea7a220345cf23e9241b6def9263d2c1ebcf3a316b0aa52ad26a43a84aa02baca3381717b3e307f47
+"regexp.prototype.flags@npm:^1.5.2":
+  version: 1.5.2
+  resolution: "regexp.prototype.flags@npm:1.5.2"
+  dependencies:
+    call-bind: ^1.0.6
+    define-properties: ^1.2.1
+    es-errors: ^1.3.0
+    set-function-name: ^2.0.1
+  checksum: d7f333667d5c564e2d7a97c56c3075d64c722c9bb51b2b4df6822b2e8096d623a5e63088fb4c83df919b6951ef8113841de8b47de7224872fa6838bc5d8a7d64
   languageName: node
   linkType: hard
 
 "require-from-string@npm:^2.0.2":
   version: 2.0.2
   resolution: "require-from-string@npm:2.0.2"
   checksum: a03ef6895445f33a4015300c426699bc66b2b044ba7b670aa238610381b56d3f07c686251740d575e22f4c87531ba662d06937508f0f3c0f1ddc04db3130560b
@@ -5330,36 +5074,36 @@
   version: 5.0.0
   resolution: "resolve-from@npm:5.0.0"
   checksum: 4ceeb9113e1b1372d0cd969f3468fa042daa1dd9527b1b6bb88acb6ab55d8b9cd65dbf18819f9f9ddf0db804990901dcdaade80a215e7b2c23daae38e64f5bdf
   languageName: node
   linkType: hard
 
 "resolve@npm:^1.10.0, resolve@npm:^1.20.0":
-  version: 1.22.6
-  resolution: "resolve@npm:1.22.6"
+  version: 1.22.8
+  resolution: "resolve@npm:1.22.8"
   dependencies:
     is-core-module: ^2.13.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: d13bf66d4e2ee30d291491f16f2fa44edd4e0cefb85d53249dd6f93e70b2b8c20ec62f01b18662e3cd40e50a7528f18c4087a99490048992a3bb954cf3201a5b
+  checksum: f8a26958aa572c9b064562750b52131a37c29d072478ea32e129063e2da7f83e31f7f11e7087a18225a8561cfe8d2f0df9dbea7c9d331a897571c0a2527dbb4c
   languageName: node
   linkType: hard
 
 "resolve@patch:resolve@^1.10.0#~builtin<compat/resolve>, resolve@patch:resolve@^1.20.0#~builtin<compat/resolve>":
-  version: 1.22.6
-  resolution: "resolve@patch:resolve@npm%3A1.22.6#~builtin<compat/resolve>::version=1.22.6&hash=c3c19d"
+  version: 1.22.8
+  resolution: "resolve@patch:resolve@npm%3A1.22.8#~builtin<compat/resolve>::version=1.22.8&hash=c3c19d"
   dependencies:
     is-core-module: ^2.13.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: 9d3b3c67aefd12cecbe5f10ca4d1f51ea190891096497c43f301b086883b426466918c3a64f1bbf1788fabb52b579d58809614006c5d0b49186702b3b8fb746a
+  checksum: 5479b7d431cacd5185f8db64bfcb7286ae5e31eb299f4c4f404ad8aa6098b77599563ac4257cb2c37a42f59dfc06a1bec2bcf283bb448f319e37f0feb9a09847
   languageName: node
   linkType: hard
 
 "reusify@npm:^1.0.4":
   version: 1.0.4
   resolution: "reusify@npm:1.0.4"
   checksum: c3076ebcc22a6bc252cb0b9c77561795256c22b757f40c0d8110b1300723f15ec0fc8685e8d4ea6d7666f36c79ccc793b1939c748bf36f18f542744a4e379fcc
@@ -5373,70 +5117,61 @@
     glob: ^7.1.3
   bin:
     rimraf: bin.js
   checksum: 87f4164e396f0171b0a3386cc1877a817f572148ee13a7e113b238e48e8a9f2f31d009a92ec38a591ff1567d9662c6b67fd8818a2dbbaed74bc26a87a2a4a9a0
   languageName: node
   linkType: hard
 
-"rimraf@npm:^5.0.1":
-  version: 5.0.1
-  resolution: "rimraf@npm:5.0.1"
+"rimraf@npm:^5.0.5":
+  version: 5.0.5
+  resolution: "rimraf@npm:5.0.5"
   dependencies:
-    glob: ^10.2.5
+    glob: ^10.3.7
   bin:
-    rimraf: dist/cjs/src/bin.js
-  checksum: bafce85391349a2d960847980bf9b5caa2a8887f481af630f1ea27e08288217293cec72d75e9a2ba35495c212789f66a7f3d23366ba6197026ab71c535126857
-  languageName: node
-  linkType: hard
-
-"run-applescript@npm:^5.0.0":
-  version: 5.0.0
-  resolution: "run-applescript@npm:5.0.0"
-  dependencies:
-    execa: ^5.0.0
-  checksum: d00c2dbfa5b2d774de7451194b8b125f40f65fc183de7d9dcae97f57f59433586d3c39b9001e111c38bfa24c3436c99df1bb4066a2a0c90d39a8c4cd6889af77
+    rimraf: dist/esm/bin.mjs
+  checksum: d66eef829b2e23b16445f34e73d75c7b7cf4cbc8834b04720def1c8f298eb0753c3d76df77325fad79d0a2c60470525d95f89c2475283ad985fd7441c32732d1
   languageName: node
   linkType: hard
 
 "run-parallel@npm:^1.1.9":
   version: 1.2.0
   resolution: "run-parallel@npm:1.2.0"
   dependencies:
     queue-microtask: ^1.2.2
   checksum: cb4f97ad25a75ebc11a8ef4e33bb962f8af8516bb2001082ceabd8902e15b98f4b84b4f8a9b222e5d57fc3bd1379c483886ed4619367a7680dad65316993021d
   languageName: node
   linkType: hard
 
-"safe-array-concat@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "safe-array-concat@npm:1.0.1"
+"safe-array-concat@npm:^1.1.2":
+  version: 1.1.2
+  resolution: "safe-array-concat@npm:1.1.2"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.2.1
+    call-bind: ^1.0.7
+    get-intrinsic: ^1.2.4
     has-symbols: ^1.0.3
     isarray: ^2.0.5
-  checksum: 001ecf1d8af398251cbfabaf30ed66e3855127fbceee178179524b24160b49d15442f94ed6c0db0b2e796da76bb05b73bf3cc241490ec9c2b741b41d33058581
+  checksum: a3b259694754ddfb73ae0663829e396977b99ff21cbe8607f35a469655656da8e271753497e59da8a7575baa94d2e684bea3e10ddd74ba046c0c9b4418ffa0c4
   languageName: node
   linkType: hard
 
 "safe-buffer@npm:^5.1.0":
   version: 5.2.1
   resolution: "safe-buffer@npm:5.2.1"
   checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
   languageName: node
   linkType: hard
 
-"safe-regex-test@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "safe-regex-test@npm:1.0.0"
+"safe-regex-test@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "safe-regex-test@npm:1.0.3"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.1.3
+    call-bind: ^1.0.6
+    es-errors: ^1.3.0
     is-regex: ^1.1.4
-  checksum: bc566d8beb8b43c01b94e67de3f070fd2781685e835959bbbaaec91cc53381145ca91f69bd837ce6ec244817afa0a5e974fc4e40a2957f0aca68ac3add1ddd34
+  checksum: 6c7d392ff1ae7a3ae85273450ed02d1d131f1d2c76e177d6b03eb88e6df8fa062639070e7d311802c1615f351f18dc58f9454501c58e28d5ffd9b8f502ba6489
   languageName: node
   linkType: hard
 
 "safer-buffer@npm:>= 2.1.2 < 3.0.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
@@ -5505,42 +5240,57 @@
   resolution: "semver@npm:5.7.2"
   bin:
     semver: bin/semver
   checksum: fb4ab5e0dd1c22ce0c937ea390b4a822147a9c53dbd2a9a0132f12fe382902beef4fbf12cf51bb955248d8d15874ce8cd89532569756384f994309825f10b686
   languageName: node
   linkType: hard
 
-"semver@npm:^7.3.4, semver@npm:^7.3.8, semver@npm:^7.5.4":
-  version: 7.5.4
-  resolution: "semver@npm:7.5.4"
+"semver@npm:^7.3.4, semver@npm:^7.5.4":
+  version: 7.6.0
+  resolution: "semver@npm:7.6.0"
   dependencies:
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
-  checksum: 12d8ad952fa353b0995bf180cdac205a4068b759a140e5d3c608317098b3575ac2f1e09182206bf2eb26120e1c0ed8fb92c48c592f6099680de56bb071423ca3
+  checksum: 7427f05b70786c696640edc29fdd4bc33b2acf3bbe1740b955029044f80575fc664e1a512e4113c3af21e767154a94b4aa214bf6cd6e42a1f6dba5914e0b208c
   languageName: node
   linkType: hard
 
 "serialize-javascript@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "serialize-javascript@npm:6.0.1"
+  version: 6.0.2
+  resolution: "serialize-javascript@npm:6.0.2"
   dependencies:
     randombytes: ^2.1.0
-  checksum: 3c4f4cb61d0893b988415bdb67243637333f3f574e9e9cc9a006a2ced0b390b0b3b44aef8d51c951272a9002ec50885eefdc0298891bc27eb2fe7510ea87dc4f
+  checksum: c4839c6206c1d143c0f80763997a361310305751171dd95e4b57efee69b8f6edd8960a0b7fbfc45042aadff98b206d55428aee0dc276efe54f100899c7fa8ab7
   languageName: node
   linkType: hard
 
-"set-function-name@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "set-function-name@npm:2.0.1"
+"set-function-length@npm:^1.2.1":
+  version: 1.2.2
+  resolution: "set-function-length@npm:1.2.2"
   dependencies:
-    define-data-property: ^1.0.1
+    define-data-property: ^1.1.4
+    es-errors: ^1.3.0
+    function-bind: ^1.1.2
+    get-intrinsic: ^1.2.4
+    gopd: ^1.0.1
+    has-property-descriptors: ^1.0.2
+  checksum: a8248bdacdf84cb0fab4637774d9fb3c7a8e6089866d04c817583ff48e14149c87044ce683d7f50759a8c50fb87c7a7e173535b06169c87ef76f5fb276dfff72
+  languageName: node
+  linkType: hard
+
+"set-function-name@npm:^2.0.1":
+  version: 2.0.2
+  resolution: "set-function-name@npm:2.0.2"
+  dependencies:
+    define-data-property: ^1.1.4
+    es-errors: ^1.3.0
     functions-have-names: ^1.2.3
-    has-property-descriptors: ^1.0.0
-  checksum: 4975d17d90c40168eee2c7c9c59d023429f0a1690a89d75656306481ece0c3c1fb1ebcc0150ea546d1913e35fbd037bace91372c69e543e51fc5d1f31a9fa126
+    has-property-descriptors: ^1.0.2
+  checksum: d6229a71527fd0404399fc6227e0ff0652800362510822a291925c9d7b48a1ca1a468b11b281471c34cd5a2da0db4f5d7ff315a61d26655e77f6e971e6d0c80f
   languageName: node
   linkType: hard
 
 "shallow-clone@npm:^3.0.0":
   version: 3.0.1
   resolution: "shallow-clone@npm:3.0.1"
   dependencies:
@@ -5585,28 +5335,22 @@
   version: 1.8.1
   resolution: "shell-quote@npm:1.8.1"
   checksum: 5f01201f4ef504d4c6a9d0d283fa17075f6770bfbe4c5850b074974c68062f37929ca61700d95ad2ac8822e14e8c4b990ca0e6e9272e64befd74ce5e19f0736b
   languageName: node
   linkType: hard
 
 "side-channel@npm:^1.0.4":
-  version: 1.0.4
-  resolution: "side-channel@npm:1.0.4"
+  version: 1.0.6
+  resolution: "side-channel@npm:1.0.6"
   dependencies:
-    call-bind: ^1.0.0
-    get-intrinsic: ^1.0.2
-    object-inspect: ^1.9.0
-  checksum: 351e41b947079c10bd0858364f32bb3a7379514c399edb64ab3dce683933483fc63fb5e4efe0a15a2e8a7e3c436b6a91736ddb8d8c6591b0460a24bb4a1ee245
-  languageName: node
-  linkType: hard
-
-"signal-exit@npm:^3.0.3, signal-exit@npm:^3.0.7":
-  version: 3.0.7
-  resolution: "signal-exit@npm:3.0.7"
-  checksum: a2f098f247adc367dffc27845853e9959b9e88b01cb301658cfe4194352d8d2bb32e18467c786a7fe15f1d44b233ea35633d076d5e737870b7139949d1ab6318
+    call-bind: ^1.0.7
+    es-errors: ^1.3.0
+    get-intrinsic: ^1.2.4
+    object-inspect: ^1.13.1
+  checksum: bfc1afc1827d712271453e91b7cd3878ac0efd767495fd4e594c4c2afaa7963b7b510e249572bfd54b0527e66e4a12b61b80c061389e129755f34c493aad9b97
   languageName: node
   linkType: hard
 
 "signal-exit@npm:^4.0.1":
   version: 4.1.0
   resolution: "signal-exit@npm:4.1.0"
   checksum: 64c757b498cb8629ffa5f75485340594d2f8189e9b08700e69199069c8e3070fb3e255f7ab873c05dc0b3cec412aea7402e10a5990cb6a050bd33ba062a6c549
@@ -5634,18 +5378,18 @@
 "source-list-map@npm:^2.0.0":
   version: 2.0.1
   resolution: "source-list-map@npm:2.0.1"
   checksum: 806efc6f75e7cd31e4815e7a3aaf75a45c704871ea4075cb2eb49882c6fca28998f44fc5ac91adb6de03b2882ee6fb02f951fdc85e6a22b338c32bfe19557938
   languageName: node
   linkType: hard
 
-"source-map-js@npm:^1.0.1, source-map-js@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "source-map-js@npm:1.0.2"
-  checksum: c049a7fc4deb9a7e9b481ae3d424cc793cb4845daa690bc5a05d428bf41bf231ced49b4cf0c9e77f9d42fdb3d20d6187619fc586605f5eabe995a316da8d377c
+"source-map-js@npm:^1.0.1, source-map-js@npm:^1.2.0":
+  version: 1.2.0
+  resolution: "source-map-js@npm:1.2.0"
+  checksum: 791a43306d9223792e84293b00458bf102a8946e7188f3db0e4e22d8d530b5f80a4ce468eb5ec0bf585443ad55ebbd630bf379c98db0b1f317fd902500217f97
   languageName: node
   linkType: hard
 
 "source-map-loader@npm:^1.0.2":
   version: 1.1.3
   resolution: "source-map-loader@npm:1.1.3"
   dependencies:
@@ -5700,34 +5444,34 @@
     spdx-expression-parse: ^3.0.0
     spdx-license-ids: ^3.0.0
   checksum: e9ae98d22f69c88e7aff5b8778dc01c361ef635580e82d29e5c60a6533cc8f4d820803e67d7432581af0cc4fb49973125076ee3b90df191d153e223c004193b2
   languageName: node
   linkType: hard
 
 "spdx-exceptions@npm:^2.1.0":
-  version: 2.3.0
-  resolution: "spdx-exceptions@npm:2.3.0"
-  checksum: cb69a26fa3b46305637123cd37c85f75610e8c477b6476fa7354eb67c08128d159f1d36715f19be6f9daf4b680337deb8c65acdcae7f2608ba51931540687ac0
+  version: 2.5.0
+  resolution: "spdx-exceptions@npm:2.5.0"
+  checksum: bb127d6e2532de65b912f7c99fc66097cdea7d64c10d3ec9b5e96524dbbd7d20e01cba818a6ddb2ae75e62bb0c63d5e277a7e555a85cbc8ab40044984fa4ae15
   languageName: node
   linkType: hard
 
 "spdx-expression-parse@npm:^3.0.0":
   version: 3.0.1
   resolution: "spdx-expression-parse@npm:3.0.1"
   dependencies:
     spdx-exceptions: ^2.1.0
     spdx-license-ids: ^3.0.0
   checksum: a1c6e104a2cbada7a593eaa9f430bd5e148ef5290d4c0409899855ce8b1c39652bcc88a725259491a82601159d6dc790bedefc9016c7472f7de8de7361f8ccde
   languageName: node
   linkType: hard
 
 "spdx-license-ids@npm:^3.0.0":
-  version: 3.0.15
-  resolution: "spdx-license-ids@npm:3.0.15"
-  checksum: 99d567875b50504e1a7359f6da7d03e28db2b855b412ced18310679d091565a44f61ffd2585f19ea53a1192c35f2156c143507b12339dda26ef928547df32002
+  version: 3.0.17
+  resolution: "spdx-license-ids@npm:3.0.17"
+  checksum: 0aba5d16292ff604dd20982200e23b4d425f6ba364765039bdbde2f6c956b9909fce1ad040a897916a5f87388e85e001f90cb64bf706b6e319f3908cfc445a59
   languageName: node
   linkType: hard
 
 "string-width-cjs@npm:string-width@^4.2.0, string-width@npm:^4.1.0, string-width@npm:^4.2.3":
   version: 4.2.3
   resolution: "string-width@npm:4.2.3"
   dependencies:
@@ -5746,54 +5490,56 @@
     emoji-regex: ^9.2.2
     strip-ansi: ^7.0.1
   checksum: 7369deaa29f21dda9a438686154b62c2c5f661f8dda60449088f9f980196f7908fc39fdd1803e3e01541970287cf5deae336798337e9319a7055af89dafa7193
   languageName: node
   linkType: hard
 
 "string.prototype.padend@npm:^3.0.0":
-  version: 3.1.5
-  resolution: "string.prototype.padend@npm:3.1.5"
+  version: 3.1.6
+  resolution: "string.prototype.padend@npm:3.1.6"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: fc915e0b6ae1dce07a9f5088429d84fda2c1c0ac9a05bc14a602f173cc2fdef32e4893dfba5656f8f955450c9c16deebdb8d303d27613a367bc6d8508a94cd5e
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-abstract: ^1.23.2
+    es-object-atoms: ^1.0.0
+  checksum: d9fc23c21bdfb6850756002ef09cebc420882003f29eafbd8322df77a90726bc2a64892d01f94f1fc9fc6f809414fbcbd8615610bb3cddd33512c12b6b3643a2
   languageName: node
   linkType: hard
 
-"string.prototype.trim@npm:^1.2.8":
-  version: 1.2.8
-  resolution: "string.prototype.trim@npm:1.2.8"
+"string.prototype.trim@npm:^1.2.9":
+  version: 1.2.9
+  resolution: "string.prototype.trim@npm:1.2.9"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: 49eb1a862a53aba73c3fb6c2a53f5463173cb1f4512374b623bcd6b43ad49dd559a06fb5789bdec771a40fc4d2a564411c0a75d35fb27e76bbe738c211ecff07
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-abstract: ^1.23.0
+    es-object-atoms: ^1.0.0
+  checksum: ea2df6ec1e914c9d4e2dc856fa08228e8b1be59b59e50b17578c94a66a176888f417264bb763d4aac638ad3b3dad56e7a03d9317086a178078d131aa293ba193
   languageName: node
   linkType: hard
 
-"string.prototype.trimend@npm:^1.0.7":
-  version: 1.0.7
-  resolution: "string.prototype.trimend@npm:1.0.7"
+"string.prototype.trimend@npm:^1.0.8":
+  version: 1.0.8
+  resolution: "string.prototype.trimend@npm:1.0.8"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: 2375516272fd1ba75992f4c4aa88a7b5f3c7a9ca308d963bcd5645adf689eba6f8a04ebab80c33e30ec0aefc6554181a3a8416015c38da0aa118e60ec896310c
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-object-atoms: ^1.0.0
+  checksum: cc3bd2de08d8968a28787deba9a3cb3f17ca5f9f770c91e7e8fa3e7d47f079bad70fadce16f05dda9f261788be2c6e84a942f618c3bed31e42abc5c1084f8dfd
   languageName: node
   linkType: hard
 
-"string.prototype.trimstart@npm:^1.0.7":
-  version: 1.0.7
-  resolution: "string.prototype.trimstart@npm:1.0.7"
+"string.prototype.trimstart@npm:^1.0.8":
+  version: 1.0.8
+  resolution: "string.prototype.trimstart@npm:1.0.8"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: 13d0c2cb0d5ff9e926fa0bec559158b062eed2b68cd5be777ffba782c96b2b492944e47057274e064549b94dd27cf81f48b27a31fee8af5b574cff253e7eb613
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-object-atoms: ^1.0.0
+  checksum: df1007a7f580a49d692375d996521dc14fd103acda7f3034b3c558a60b82beeed3a64fa91e494e164581793a8ab0ae2f59578a49896a7af6583c1f20472bce96
   languageName: node
   linkType: hard
 
 "strip-ansi-cjs@npm:strip-ansi@^6.0.1, strip-ansi@npm:^6.0.0, strip-ansi@npm:^6.0.1":
   version: 6.0.1
   resolution: "strip-ansi@npm:6.0.1"
   dependencies:
@@ -5814,28 +5560,14 @@
 "strip-bom@npm:^3.0.0":
   version: 3.0.0
   resolution: "strip-bom@npm:3.0.0"
   checksum: 8d50ff27b7ebe5ecc78f1fe1e00fcdff7af014e73cf724b46fb81ef889eeb1015fc5184b64e81a2efe002180f3ba431bdd77e300da5c6685d702780fbf0c8d5b
   languageName: node
   linkType: hard
 
-"strip-final-newline@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "strip-final-newline@npm:2.0.0"
-  checksum: 69412b5e25731e1938184b5d489c32e340605bb611d6140344abc3421b7f3c6f9984b21dff296dfcf056681b82caa3bb4cc996a965ce37bcfad663e92eae9c64
-  languageName: node
-  linkType: hard
-
-"strip-final-newline@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "strip-final-newline@npm:3.0.0"
-  checksum: 23ee263adfa2070cd0f23d1ac14e2ed2f000c9b44229aec9c799f1367ec001478469560abefd00c5c99ee6f0b31c137d53ec6029c53e9f32a93804e18c201050
-  languageName: node
-  linkType: hard
-
 "strip-indent@npm:^4.0.0":
   version: 4.0.0
   resolution: "strip-indent@npm:4.0.0"
   dependencies:
     min-indent: ^1.0.1
   checksum: 06cbcd93da721c46bc13caeb1c00af93a9b18146a1c95927672d2decab6a25ad83662772417cea9317a2507fb143253ecc23c4415b64f5828cef9b638a744598
   languageName: node
@@ -5844,27 +5576,27 @@
 "strip-json-comments@npm:^3.1.1":
   version: 3.1.1
   resolution: "strip-json-comments@npm:3.1.1"
   checksum: 492f73e27268f9b1c122733f28ecb0e7e8d8a531a6662efbd08e22cccb3f9475e90a1b82cab06a392f6afae6d2de636f977e231296400d0ec5304ba70f166443
   languageName: node
   linkType: hard
 
-"style-loader@npm:^3.3.1, style-loader@npm:~3.3.1":
-  version: 3.3.3
-  resolution: "style-loader@npm:3.3.3"
+"style-loader@npm:^3.3.4, style-loader@npm:~3.3.1":
+  version: 3.3.4
+  resolution: "style-loader@npm:3.3.4"
   peerDependencies:
     webpack: ^5.0.0
-  checksum: f59c953f56f6a935bd6a1dfa409f1128fed2b66b48ce4a7a75b85862a7156e5e90ab163878962762f528ec4d510903d828da645e143fbffd26f055dc1c094078
+  checksum: caac3f2fe2c3c89e49b7a2a9329e1cfa515ecf5f36b9c4885f9b218019fda207a9029939b2c35821dec177a264a007e7c391ccdd3ff7401881ce6287b9c8f38b
   languageName: node
   linkType: hard
 
 "style-mod@npm:^4.0.0, style-mod@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "style-mod@npm:4.1.0"
-  checksum: 8402b14ca11113a3640d46b3cf7ba49f05452df7846bc5185a3535d9b6a64a3019e7fb636b59ccbb7816aeb0725b24723e77a85b05612a9360e419958e13b4e6
+  version: 4.1.2
+  resolution: "style-mod@npm:4.1.2"
+  checksum: 7c5c3e82747f9bcf5f288d8d07f50848e4630fe5ff7bfe4d94cc87d6b6a2588227cbf21b4c792ac6406e5852293300a75e710714479a5c59a06af677f0825ef8
   languageName: node
   linkType: hard
 
 "style-search@npm:^0.1.0":
   version: 0.1.0
   resolution: "style-search@npm:0.1.0"
   checksum: 3cfefe335033aad6d47da0725cb48f5db91a73935954c77eab77d9e415e6668cdb406da4a4f7ef9f1aca77853cf5ba7952c45e869caa5bd6439691d88098d468
@@ -5898,73 +5630,73 @@
     css-tree: ^2.3.1
   peerDependencies:
     stylelint: ">=7.0.0 <16.0.0"
   checksum: e518c8c17714022946b7637c23a6816fd2ccdd6052a19c5a138b3f7ce9b913ead9c612ac4401e102f14800a19967dbfd4b588b44cbf3f3c6a5984bef7bda4017
   languageName: node
   linkType: hard
 
-"stylelint-prettier@npm:^4.0.0":
-  version: 4.0.2
-  resolution: "stylelint-prettier@npm:4.0.2"
+"stylelint-prettier@npm:^4.1.0":
+  version: 4.1.0
+  resolution: "stylelint-prettier@npm:4.1.0"
   dependencies:
     prettier-linter-helpers: ^1.0.0
   peerDependencies:
     prettier: ">=3.0.0"
     stylelint: ">=15.8.0"
-  checksum: b60112c10b8f31456211d65b4c17238fdaf46ee9f80ab035621f2eb86b47505a4b9582d99f4334dfe370cc8104de870f7fcc256737d0f2e68f4357239f739054
+  checksum: bbeb7e0dd49099c43297e88a61385b39f4b5810c8bfcc972d5b2706b6a7e14a8eefd5f9e623841cf3127111a8859eb624a3e7cc1bc5197c83c55c6c9a616a4d2
   languageName: node
   linkType: hard
 
-"stylelint@npm:^15.10.1":
-  version: 15.10.3
-  resolution: "stylelint@npm:15.10.3"
+"stylelint@npm:^15.11.0":
+  version: 15.11.0
+  resolution: "stylelint@npm:15.11.0"
   dependencies:
     "@csstools/css-parser-algorithms": ^2.3.1
     "@csstools/css-tokenizer": ^2.2.0
     "@csstools/media-query-list-parser": ^2.1.4
     "@csstools/selector-specificity": ^3.0.0
     balanced-match: ^2.0.0
     colord: ^2.9.3
     cosmiconfig: ^8.2.0
-    css-functions-list: ^3.2.0
+    css-functions-list: ^3.2.1
     css-tree: ^2.3.1
     debug: ^4.3.4
     fast-glob: ^3.3.1
     fastest-levenshtein: ^1.0.16
-    file-entry-cache: ^6.0.1
+    file-entry-cache: ^7.0.0
     global-modules: ^2.0.0
     globby: ^11.1.0
     globjoin: ^0.1.4
     html-tags: ^3.3.1
     ignore: ^5.2.4
     import-lazy: ^4.0.0
     imurmurhash: ^0.1.4
     is-plain-object: ^5.0.0
-    known-css-properties: ^0.28.0
+    known-css-properties: ^0.29.0
     mathml-tag-names: ^2.1.3
     meow: ^10.1.5
     micromatch: ^4.0.5
     normalize-path: ^3.0.0
     picocolors: ^1.0.0
-    postcss: ^8.4.27
+    postcss: ^8.4.28
     postcss-resolve-nested-selector: ^0.1.1
     postcss-safe-parser: ^6.0.0
     postcss-selector-parser: ^6.0.13
     postcss-value-parser: ^4.2.0
     resolve-from: ^5.0.0
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
     style-search: ^0.1.0
     supports-hyperlinks: ^3.0.0
     svg-tags: ^1.0.0
     table: ^6.8.1
     write-file-atomic: ^5.0.1
   bin:
     stylelint: bin/stylelint.mjs
-  checksum: eb70dd0e4d500141f4868ddb7403ad7eb8732b02a3f2fe3907d0859369cedd395b60b0075da758b5be07de771c586b1bf64de4eead8159d46b0d16beff827e67
+  checksum: 9835f8a3e3976a3b81a35569d08f5f4a9c3b5cff415f1345a505870afc0c3231acff27f119d937c5bb11fdbc98d554af564c2a648a52604280a59a11974fcbfc
   languageName: node
   linkType: hard
 
 "supports-color@npm:^5.3.0":
   version: 5.5.0
   resolution: "supports-color@npm:5.5.0"
   dependencies:
@@ -6011,94 +5743,94 @@
 "svg-tags@npm:^1.0.0":
   version: 1.0.0
   resolution: "svg-tags@npm:1.0.0"
   checksum: 407e5ef87cfa2fb81c61d738081c2decd022ce13b922d035b214b49810630bf5d1409255a4beb3a940b77b32f6957806deff16f1bf0ce1ab11c7a184115a0b7f
   languageName: node
   linkType: hard
 
-"synckit@npm:^0.8.5":
-  version: 0.8.5
-  resolution: "synckit@npm:0.8.5"
-  dependencies:
-    "@pkgr/utils": ^2.3.1
-    tslib: ^2.5.0
-  checksum: 8a9560e5d8f3d94dc3cf5f7b9c83490ffa30d320093560a37b88f59483040771fd1750e76b9939abfbb1b5a23fd6dfbae77f6b338abffe7cae7329cd9b9bb86b
+"synckit@npm:^0.8.6":
+  version: 0.8.8
+  resolution: "synckit@npm:0.8.8"
+  dependencies:
+    "@pkgr/core": ^0.1.0
+    tslib: ^2.6.2
+  checksum: 9ed5d33abb785f5f24e2531efd53b2782ca77abf7912f734d170134552b99001915531be5a50297aa45c5701b5c9041e8762e6cd7a38e41e2461c1e7fccdedf8
+  languageName: node
+  linkType: hard
+
+"tabbable@npm:^5.2.0":
+  version: 5.3.3
+  resolution: "tabbable@npm:5.3.3"
+  checksum: 1aa56e1bb617cc10616c407f4e756f0607f3e2d30f9803664d70b85db037ca27e75918ed1c71443f3dc902e21dc9f991ce4b52d63a538c9b69b3218d3babcd70
   languageName: node
   linkType: hard
 
 "table@npm:^6.8.1":
-  version: 6.8.1
-  resolution: "table@npm:6.8.1"
+  version: 6.8.2
+  resolution: "table@npm:6.8.2"
   dependencies:
     ajv: ^8.0.1
     lodash.truncate: ^4.4.2
     slice-ansi: ^4.0.0
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
-  checksum: 08249c7046125d9d0a944a6e96cfe9ec66908d6b8a9db125531be6eb05fa0de047fd5542e9d43b4f987057f00a093b276b8d3e19af162a9c40db2681058fd306
+  checksum: 61188652f53a980d1759ca460ca8dea5c5322aece3210457e7084882f053c2b6a870041295e08a82cb1d676e31b056406845d94b0abf3c79a4b104777bec413b
   languageName: node
   linkType: hard
 
-"tapable@npm:^2.1.1, tapable@npm:^2.2.0":
+"tapable@npm:^2.1.1, tapable@npm:^2.2.0, tapable@npm:^2.2.1":
   version: 2.2.1
   resolution: "tapable@npm:2.2.1"
   checksum: 3b7a1b4d86fa940aad46d9e73d1e8739335efd4c48322cb37d073eb6f80f5281889bf0320c6d8ffcfa1a0dd5bfdbd0f9d037e252ef972aca595330538aac4d51
   languageName: node
   linkType: hard
 
-"terser-webpack-plugin@npm:^5.3.7":
-  version: 5.3.9
-  resolution: "terser-webpack-plugin@npm:5.3.9"
+"terser-webpack-plugin@npm:^5.3.10, terser-webpack-plugin@npm:^5.3.7":
+  version: 5.3.10
+  resolution: "terser-webpack-plugin@npm:5.3.10"
   dependencies:
-    "@jridgewell/trace-mapping": ^0.3.17
+    "@jridgewell/trace-mapping": ^0.3.20
     jest-worker: ^27.4.5
     schema-utils: ^3.1.1
     serialize-javascript: ^6.0.1
-    terser: ^5.16.8
+    terser: ^5.26.0
   peerDependencies:
     webpack: ^5.1.0
   peerDependenciesMeta:
     "@swc/core":
       optional: true
     esbuild:
       optional: true
     uglify-js:
       optional: true
-  checksum: 41705713d6f9cb83287936b21e27c658891c78c4392159f5148b5623f0e8c48559869779619b058382a4c9758e7820ea034695e57dc7c474b4962b79f553bc5f
+  checksum: bd6e7596cf815f3353e2a53e79cbdec959a1b0276f5e5d4e63e9d7c3c5bb5306df567729da287d1c7b39d79093e56863c569c42c6c24cc34c76aa313bd2cbcea
   languageName: node
   linkType: hard
 
-"terser@npm:^5.16.8":
-  version: 5.20.0
-  resolution: "terser@npm:5.20.0"
+"terser@npm:^5.26.0":
+  version: 5.30.3
+  resolution: "terser@npm:5.30.3"
   dependencies:
     "@jridgewell/source-map": ^0.3.3
     acorn: ^8.8.2
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: 251d1b62d7c651ace29f997cf336ff5d5f8e30c65c8698ab7b831764d9e012ab0640895cb609906fb939a5bdf5143d73b5781c5c8c67b9216c77ce92dafdc0bc
+  checksum: 8c680ed32a948f806fade0969c52aab94b6de174e4a78610f5d3abf9993b161eb19b88b2ceadff09b153858727c02deb6709635e4bfbd519f67d54e0394e2983
   languageName: node
   linkType: hard
 
 "text-table@npm:^0.2.0":
   version: 0.2.0
   resolution: "text-table@npm:0.2.0"
   checksum: b6937a38c80c7f84d9c11dd75e49d5c44f71d95e810a3250bd1f1797fc7117c57698204adf676b71497acc205d769d65c16ae8fa10afad832ae1322630aef10a
   languageName: node
   linkType: hard
 
-"titleize@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "titleize@npm:3.0.0"
-  checksum: 71fbbeabbfb36ccd840559f67f21e356e1d03da2915b32d2ae1a60ddcc13a124be2739f696d2feb884983441d159a18649e8d956648d591bdad35c430a6b6d28
-  languageName: node
-  linkType: hard
-
 "to-regex-range@npm:^5.0.1":
   version: 5.0.1
   resolution: "to-regex-range@npm:5.0.1"
   dependencies:
     is-number: ^7.0.0
   checksum: f76fa01b3d5be85db6a2a143e24df9f60dd047d151062d0ba3df62953f2f697b16fe5dad9b0ac6191c7efc7b1d9dcaa4b768174b7b29da89d4428e64bc0a20ed
   languageName: node
@@ -6114,60 +5846,67 @@
   linkType: hard
 
 "trame-jupyter-extension@workspace:.":
   version: 0.0.0-use.local
   resolution: "trame-jupyter-extension@workspace:."
   dependencies:
     "@jupyterlab/application": ^3.5.0 || ^4.0.5
-    "@jupyterlab/builder": ^4.0.0
+    "@jupyterlab/builder": ^4.1.6
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/notebook": ^4.0.7
     "@jupyterlab/services": ^7.0.0
-    "@types/json-schema": ^7.0.11
-    "@types/react": ^18.0.26
-    "@types/react-addons-linked-state-mixin": ^0.14.22
-    "@typescript-eslint/eslint-plugin": ^6.1.0
-    "@typescript-eslint/parser": ^6.1.0
-    css-loader: ^6.7.1
-    eslint: ^8.36.0
+    "@types/json-schema": ^7.0.15
+    "@types/react": ^18.2.79
+    "@types/react-addons-linked-state-mixin": ^0.14.27
+    "@typescript-eslint/eslint-plugin": ^6.21.0
+    "@typescript-eslint/parser": ^6.21.0
+    css-loader: ^6.11.0
+    eslint: ^8.57.0
     eslint-config-prettier: ^8.8.0
-    eslint-plugin-prettier: ^5.0.0
+    eslint-plugin-prettier: ^5.1.3
     mkdirp: ^1.0.3
     npm-run-all: ^4.1.5
-    prettier: ^3.0.0
-    rimraf: ^5.0.1
+    prettier: ^3.2.5
+    rimraf: ^5.0.5
     source-map-loader: ^1.0.2
-    style-loader: ^3.3.1
-    stylelint: ^15.10.1
+    style-loader: ^3.3.4
+    stylelint: ^15.11.0
     stylelint-config-recommended: ^13.0.0
     stylelint-config-standard: ^34.0.0
     stylelint-csstree-validator: ^3.0.0
-    stylelint-prettier: ^4.0.0
-    typescript: ~5.0.2
-    yjs: ^13.5.0
+    stylelint-prettier: ^4.1.0
+    typescript: ~5.4.5
+    yjs: ^13.6.14
   languageName: unknown
   linkType: soft
 
 "trim-newlines@npm:^4.0.2":
   version: 4.1.1
   resolution: "trim-newlines@npm:4.1.1"
   checksum: 5b09f8e329e8f33c1111ef26906332ba7ba7248cde3e26fc054bb3d69f2858bf5feedca9559c572ff91f33e52977c28e0d41c387df6a02a633cbb8c2d8238627
   languageName: node
   linkType: hard
 
 "ts-api-utils@npm:^1.0.1":
-  version: 1.0.3
-  resolution: "ts-api-utils@npm:1.0.3"
+  version: 1.3.0
+  resolution: "ts-api-utils@npm:1.3.0"
   peerDependencies:
     typescript: ">=4.2.0"
-  checksum: 441cc4489d65fd515ae6b0f4eb8690057add6f3b6a63a36073753547fb6ce0c9ea0e0530220a0b282b0eec535f52c4dfc315d35f8a4c9a91c0def0707a714ca6
+  checksum: c746ddabfdffbf16cb0b0db32bb287236a19e583057f8649ee7c49995bb776e1d3ef384685181c11a1a480369e022ca97512cb08c517b2d2bd82c83754c97012
   languageName: node
   linkType: hard
 
-"tslib@npm:^2.5.0, tslib@npm:^2.6.0":
+"tslib@npm:^1.13.0":
+  version: 1.14.1
+  resolution: "tslib@npm:1.14.1"
+  checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
+  languageName: node
+  linkType: hard
+
+"tslib@npm:^2.6.2":
   version: 2.6.2
   resolution: "tslib@npm:2.6.2"
   checksum: 329ea56123005922f39642318e3d1f0f8265d1e7fcb92c633e0809521da75eeaca28d2cf96d7248229deb40e5c19adf408259f4b9640afd20d13aecc1430f3ad
   languageName: node
   linkType: hard
 
 "type-check@npm:^0.4.0, type-check@npm:~0.4.0":
@@ -6189,78 +5928,83 @@
 "type-fest@npm:^1.0.1, type-fest@npm:^1.2.1, type-fest@npm:^1.2.2":
   version: 1.4.0
   resolution: "type-fest@npm:1.4.0"
   checksum: b011c3388665b097ae6a109a437a04d6f61d81b7357f74cbcb02246f2f5bd72b888ae33631b99871388122ba0a87f4ff1c94078e7119ff22c70e52c0ff828201
   languageName: node
   linkType: hard
 
-"typed-array-buffer@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "typed-array-buffer@npm:1.0.0"
+"typed-array-buffer@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "typed-array-buffer@npm:1.0.2"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.2.1
-    is-typed-array: ^1.1.10
-  checksum: 3e0281c79b2a40cd97fe715db803884301993f4e8c18e8d79d75fd18f796e8cd203310fec8c7fdb5e6c09bedf0af4f6ab8b75eb3d3a85da69328f28a80456bd3
+    call-bind: ^1.0.7
+    es-errors: ^1.3.0
+    is-typed-array: ^1.1.13
+  checksum: 02ffc185d29c6df07968272b15d5319a1610817916ec8d4cd670ded5d1efe72901541ff2202fcc622730d8a549c76e198a2f74e312eabbfb712ed907d45cbb0b
   languageName: node
   linkType: hard
 
-"typed-array-byte-length@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "typed-array-byte-length@npm:1.0.0"
+"typed-array-byte-length@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "typed-array-byte-length@npm:1.0.1"
   dependencies:
-    call-bind: ^1.0.2
+    call-bind: ^1.0.7
     for-each: ^0.3.3
-    has-proto: ^1.0.1
-    is-typed-array: ^1.1.10
-  checksum: b03db16458322b263d87a702ff25388293f1356326c8a678d7515767ef563ef80e1e67ce648b821ec13178dd628eb2afdc19f97001ceae7a31acf674c849af94
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+  checksum: f65e5ecd1cf76b1a2d0d6f631f3ea3cdb5e08da106c6703ffe687d583e49954d570cc80434816d3746e18be889ffe53c58bf3e538081ea4077c26a41055b216d
   languageName: node
   linkType: hard
 
-"typed-array-byte-offset@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "typed-array-byte-offset@npm:1.0.0"
+"typed-array-byte-offset@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "typed-array-byte-offset@npm:1.0.2"
   dependencies:
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
     for-each: ^0.3.3
-    has-proto: ^1.0.1
-    is-typed-array: ^1.1.10
-  checksum: 04f6f02d0e9a948a95fbfe0d5a70b002191fae0b8fe0fe3130a9b2336f043daf7a3dda56a31333c35a067a97e13f539949ab261ca0f3692c41603a46a94e960b
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+  checksum: c8645c8794a621a0adcc142e0e2c57b1823bbfa4d590ad2c76b266aa3823895cf7afb9a893bf6685e18454ab1b0241e1a8d885a2d1340948efa4b56add4b5f67
   languageName: node
   linkType: hard
 
-"typed-array-length@npm:^1.0.4":
-  version: 1.0.4
-  resolution: "typed-array-length@npm:1.0.4"
+"typed-array-length@npm:^1.0.6":
+  version: 1.0.6
+  resolution: "typed-array-length@npm:1.0.6"
   dependencies:
-    call-bind: ^1.0.2
+    call-bind: ^1.0.7
     for-each: ^0.3.3
-    is-typed-array: ^1.1.9
-  checksum: 2228febc93c7feff142b8c96a58d4a0d7623ecde6c7a24b2b98eb3170e99f7c7eff8c114f9b283085cd59dcd2bd43aadf20e25bba4b034a53c5bb292f71f8956
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+    possible-typed-array-names: ^1.0.0
+  checksum: f0315e5b8f0168c29d390ff410ad13e4d511c78e6006df4a104576844812ee447fcc32daab1f3a76c9ef4f64eff808e134528b5b2439de335586b392e9750e5c
   languageName: node
   linkType: hard
 
-"typescript@npm:~5.0.2":
-  version: 5.0.4
-  resolution: "typescript@npm:5.0.4"
+"typescript@npm:~5.4.5":
+  version: 5.4.5
+  resolution: "typescript@npm:5.4.5"
   bin:
     tsc: bin/tsc
     tsserver: bin/tsserver
-  checksum: 82b94da3f4604a8946da585f7d6c3025fff8410779e5bde2855ab130d05e4fd08938b9e593b6ebed165bda6ad9292b230984f10952cf82f0a0ca07bbeaa08172
+  checksum: 53c879c6fa1e3bcb194b274d4501ba1985894b2c2692fa079db03c5a5a7140587a1e04e1ba03184605d35f439b40192d9e138eb3279ca8eee313c081c8bcd9b0
   languageName: node
   linkType: hard
 
-"typescript@patch:typescript@~5.0.2#~builtin<compat/typescript>":
-  version: 5.0.4
-  resolution: "typescript@patch:typescript@npm%3A5.0.4#~builtin<compat/typescript>::version=5.0.4&hash=85af82"
+"typescript@patch:typescript@~5.4.5#~builtin<compat/typescript>":
+  version: 5.4.5
+  resolution: "typescript@patch:typescript@npm%3A5.4.5#~builtin<compat/typescript>::version=5.4.5&hash=85af82"
   bin:
     tsc: bin/tsc
     tsserver: bin/tsserver
-  checksum: bb309d320c59a26565fb3793dba550576ab861018ff3fd1b7fccabbe46ae4a35546bc45f342c0a0b6f265c801ccdf64ffd68f548f117ceb7f0eac4b805cd52a9
+  checksum: 2373c693f3b328f3b2387c3efafe6d257b057a142f9a79291854b14ff4d5367d3d730810aee981726b677ae0fd8329b23309da3b6aaab8263dbdccf1da07a3ba
   languageName: node
   linkType: hard
 
 "typestyle@npm:^2.0.4":
   version: 2.4.0
   resolution: "typestyle@npm:2.4.0"
   dependencies:
@@ -6278,25 +6022,25 @@
     has-bigints: ^1.0.2
     has-symbols: ^1.0.3
     which-boxed-primitive: ^1.0.2
   checksum: b7a1cf5862b5e4b5deb091672ffa579aa274f648410009c81cca63fed3b62b610c4f3b773f912ce545bb4e31edc3138975b5bc777fc6e4817dca51affb6380e9
   languageName: node
   linkType: hard
 
-"universalify@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "universalify@npm:2.0.0"
-  checksum: 2406a4edf4a8830aa6813278bab1f953a8e40f2f63a37873ffa9a3bc8f9745d06cc8e88f3572cb899b7e509013f7f6fcc3e37e8a6d914167a5381d8440518c44
+"undici-types@npm:~5.26.4":
+  version: 5.26.5
+  resolution: "undici-types@npm:5.26.5"
+  checksum: 3192ef6f3fd5df652f2dc1cd782b49d6ff14dc98e5dced492aa8a8c65425227da5da6aafe22523c67f035a272c599bb89cfe803c1db6311e44bed3042fc25487
   languageName: node
   linkType: hard
 
-"untildify@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "untildify@npm:4.0.0"
-  checksum: 39ced9c418a74f73f0a56e1ba4634b4d959422dff61f4c72a8e39f60b99380c1b45ed776fbaa0a4101b157e4310d873ad7d114e8534ca02609b4916bb4187fb9
+"universalify@npm:^2.0.0":
+  version: 2.0.1
+  resolution: "universalify@npm:2.0.1"
+  checksum: ecd8469fe0db28e7de9e5289d32bd1b6ba8f7183db34f3bfc4ca53c49891c2d6aa05f3fb3936a81285a905cc509fb641a0c3fc131ec786167eff41236ae32e60
   languageName: node
   linkType: hard
 
 "update-browserslist-db@npm:^1.0.13":
   version: 1.0.13
   resolution: "update-browserslist-db@npm:1.0.13"
   dependencies:
@@ -6429,21 +6173,21 @@
 "w3c-keyname@npm:^2.2.4":
   version: 2.2.8
   resolution: "w3c-keyname@npm:2.2.8"
   checksum: 95bafa4c04fa2f685a86ca1000069c1ec43ace1f8776c10f226a73296caeddd83f893db885c2c220ebeb6c52d424e3b54d7c0c1e963bbf204038ff1a944fbb07
   languageName: node
   linkType: hard
 
-"watchpack@npm:^2.4.0":
-  version: 2.4.0
-  resolution: "watchpack@npm:2.4.0"
+"watchpack@npm:^2.4.1":
+  version: 2.4.1
+  resolution: "watchpack@npm:2.4.1"
   dependencies:
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.1.2
-  checksum: 23d4bc58634dbe13b86093e01c6a68d8096028b664ab7139d58f0c37d962d549a940e98f2f201cecdabd6f9c340338dc73ef8bf094a2249ef582f35183d1a131
+  checksum: 5b0179348655dcdf19cac7cb4ff923fdc024d630650c0bf6bec8899cf47c60e19d4f810a88dba692ed0e7f684cf0fcffea86efdbf6c35d81f031e328043b7fab
   languageName: node
   linkType: hard
 
 "webidl-conversions@npm:^6.1.0":
   version: 6.1.0
   resolution: "webidl-conversions@npm:6.1.0"
   checksum: 1f526507aa491f972a0c1409d07f8444e1d28778dfa269a9971f2e157182f3d496dc33296e4ed45b157fdb3bf535bb90c90bf10c50dcf1dd6caacb2a34cc84fb
@@ -6479,20 +6223,21 @@
   bin:
     webpack-cli: bin/cli.js
   checksum: 3a4ad0d0342a6815c850ee4633cc2a8a5dae04f918e7847f180bf24ab400803cf8a8943707ffbed03eb20fe6ce647f996f60a2aade87b0b4a9954da3da172ce0
   languageName: node
   linkType: hard
 
 "webpack-merge@npm:^5.7.3, webpack-merge@npm:^5.8.0":
-  version: 5.9.0
-  resolution: "webpack-merge@npm:5.9.0"
+  version: 5.10.0
+  resolution: "webpack-merge@npm:5.10.0"
   dependencies:
     clone-deep: ^4.0.1
+    flat: ^5.0.2
     wildcard: ^2.0.0
-  checksum: 64fe2c23aacc5f19684452a0e84ec02c46b990423aee6fcc5c18d7d471155bd14e9a6adb02bd3656eb3e0ac2532c8e97d69412ad14c97eeafe32fa6d10050872
+  checksum: 1fe8bf5309add7298e1ac72fb3f2090e1dfa80c48c7e79fa48aa60b5961332c7d0d61efa8851acb805e6b91a4584537a347bc106e05e9aec87fa4f7088c62f2f
   languageName: node
   linkType: hard
 
 "webpack-sources@npm:^1.2.0":
   version: 1.4.3
   resolution: "webpack-sources@npm:1.4.3"
   dependencies:
@@ -6506,47 +6251,47 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.88.2
-  resolution: "webpack@npm:5.88.2"
+  version: 5.91.0
+  resolution: "webpack@npm:5.91.0"
   dependencies:
     "@types/eslint-scope": ^3.7.3
-    "@types/estree": ^1.0.0
-    "@webassemblyjs/ast": ^1.11.5
-    "@webassemblyjs/wasm-edit": ^1.11.5
-    "@webassemblyjs/wasm-parser": ^1.11.5
+    "@types/estree": ^1.0.5
+    "@webassemblyjs/ast": ^1.12.1
+    "@webassemblyjs/wasm-edit": ^1.12.1
+    "@webassemblyjs/wasm-parser": ^1.12.1
     acorn: ^8.7.1
     acorn-import-assertions: ^1.9.0
-    browserslist: ^4.14.5
+    browserslist: ^4.21.10
     chrome-trace-event: ^1.0.2
-    enhanced-resolve: ^5.15.0
+    enhanced-resolve: ^5.16.0
     es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
-    graceful-fs: ^4.2.9
+    graceful-fs: ^4.2.11
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
     mime-types: ^2.1.27
     neo-async: ^2.6.2
     schema-utils: ^3.2.0
     tapable: ^2.1.1
-    terser-webpack-plugin: ^5.3.7
-    watchpack: ^2.4.0
+    terser-webpack-plugin: ^5.3.10
+    watchpack: ^2.4.1
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 79476a782da31a21f6dd38fbbd06b68da93baf6a62f0d08ca99222367f3b8668f5a1f2086b7bb78e23172e31fa6df6fa7ab09b25e827866c4fc4dc2b30443ce2
+  checksum: f1073715dbb1ed5c070affef293d800a867708bcbc5aba4d8baee87660e0cf53c55966a6f36fab078d1d6c9567cdcd0a9086bdfb607cab87ea68c6449791b9a3
   languageName: node
   linkType: hard
 
 "whatwg-mimetype@npm:^2.3.0":
   version: 2.3.0
   resolution: "whatwg-mimetype@npm:2.3.0"
   checksum: 23eb885940bcbcca4ff841c40a78e9cbb893ec42743993a42bf7aed16085b048b44b06f3402018931687153550f9a32d259dfa524e4f03577ab898b6965e5383
@@ -6573,24 +6318,24 @@
     is-number-object: ^1.0.4
     is-string: ^1.0.5
     is-symbol: ^1.0.3
   checksum: 53ce774c7379071729533922adcca47220228405e1895f26673bbd71bdf7fb09bee38c1d6399395927c6289476b5ae0629863427fd151491b71c4b6cb04f3a5e
   languageName: node
   linkType: hard
 
-"which-typed-array@npm:^1.1.11":
-  version: 1.1.11
-  resolution: "which-typed-array@npm:1.1.11"
+"which-typed-array@npm:^1.1.14, which-typed-array@npm:^1.1.15":
+  version: 1.1.15
+  resolution: "which-typed-array@npm:1.1.15"
   dependencies:
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
     for-each: ^0.3.3
     gopd: ^1.0.1
-    has-tostringtag: ^1.0.0
-  checksum: 711ffc8ef891ca6597b19539075ec3e08bb9b4c2ca1f78887e3c07a977ab91ac1421940505a197758fb5939aa9524976d0a5bbcac34d07ed6faa75cedbb17206
+    has-tostringtag: ^1.0.2
+  checksum: 65227dcbfadf5677aacc43ec84356d17b5500cb8b8753059bb4397de5cd0c2de681d24e1a7bd575633f976a95f88233abfd6549c2105ef4ebd58af8aa1807c75
   languageName: node
   linkType: hard
 
 "which@npm:^1.2.9, which@npm:^1.3.1":
   version: 1.3.1
   resolution: "which@npm:1.3.1"
   dependencies:
@@ -6667,25 +6412,25 @@
     imurmurhash: ^0.1.4
     signal-exit: ^4.0.1
   checksum: 8dbb0e2512c2f72ccc20ccedab9986c7d02d04039ed6e8780c987dc4940b793339c50172a1008eed7747001bfacc0ca47562668a069a7506c46c77d7ba3926a9
   languageName: node
   linkType: hard
 
 "ws@npm:^8.11.0":
-  version: 8.14.2
-  resolution: "ws@npm:8.14.2"
+  version: 8.16.0
+  resolution: "ws@npm:8.16.0"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ">=5.0.2"
   peerDependenciesMeta:
     bufferutil:
       optional: true
     utf-8-validate:
       optional: true
-  checksum: 3ca0dad26e8cc6515ff392b622a1467430814c463b3368b0258e33696b1d4bed7510bc7030f7b72838b9fdeb8dbd8839cbf808367d6aae2e1d668ce741d4308b
+  checksum: feb3eecd2bae82fa8a8beef800290ce437d8b8063bdc69712725f21aef77c49cb2ff45c6e5e7fce622248f9c7abaee506bae0a9064067ffd6935460c7357321b
   languageName: node
   linkType: hard
 
 "y-protocols@npm:^1.0.5":
   version: 1.0.6
   resolution: "y-protocols@npm:1.0.6"
   dependencies:
@@ -6706,20 +6451,20 @@
 "yargs-parser@npm:^20.2.9":
   version: 20.2.9
   resolution: "yargs-parser@npm:20.2.9"
   checksum: 8bb69015f2b0ff9e17b2c8e6bfe224ab463dd00ca211eece72a4cd8a906224d2703fb8a326d36fdd0e68701e201b2a60ed7cf81ce0fd9b3799f9fe7745977ae3
   languageName: node
   linkType: hard
 
-"yjs@npm:^13.5.0, yjs@npm:^13.5.40":
-  version: 13.6.8
-  resolution: "yjs@npm:13.6.8"
+"yjs@npm:^13.5.40, yjs@npm:^13.6.14":
+  version: 13.6.14
+  resolution: "yjs@npm:13.6.14"
   dependencies:
-    lib0: ^0.2.74
-  checksum: a2a6fd17a2cce6461b64bedd69f66845b9dfd4702e285be0b5e382840337232e54ba5cf5d48f871263074de625d3902d17ab8a1766695af3fc05a0b4da8d95e0
+    lib0: ^0.2.86
+  checksum: df399049049820d32d5759a7bd9d70cf30602408ca2a9771324f1b459f703bb6073fb35b5bcde7493fab3721d64e3c1b60eb88415b184e95a73fbce2947741cb
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `trame_jupyter_extension-2.0.1/examples/interrupt.ipynb` & `trame_jupyter_extension-2.1.0/examples/interrupt.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/examples/test_trame_jupyter_comm.ipynb` & `trame_jupyter_extension-2.1.0/examples/test_trame_jupyter_comm.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/examples/vtk_remote_rendering.ipynb` & `trame_jupyter_extension-2.1.0/examples/vtk_remote_rendering.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/examples/vue23.ipynb` & `trame_jupyter_extension-2.1.0/examples/vue23.ipynb`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/src/comm.ts` & `trame_jupyter_extension-2.1.0/src/comm.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/src/emitter.ts` & `trame_jupyter_extension-2.1.0/src/emitter.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/src/index.ts` & `trame_jupyter_extension-2.1.0/src/index.ts`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import { Kernel } from '@jupyterlab/services';
 
 import { TrameJupyterComm } from './comm';
 import { TrameJupyterWebSocket } from './websocket';
 import { ContextManager } from './manager';
 import { Registry } from './registry';
 import { getExtensionLocation } from './location';
+import { updateOutputs } from './utils';
 
 /**
  * A notebook widget extension that creates a kernel manager each time a notebook is opened.
  */
 export class WidgetExtension
   implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
 {
@@ -30,15 +31,14 @@
   }
 
   createNew(
     _panel: NotebookPanel,
     context: DocumentRegistry.IContext<INotebookModel>
   ): IDisposable {
     const manager = new ContextManager(context, this._endpoint, this._www);
-
     return manager;
   }
 }
 
 /**
  * Initialization data for the trame-jupyter-extension extension.
  */
@@ -66,26 +66,30 @@
         comm.open();
         commsRegistry.setItem(kernelId, comm);
         comm.addEventListener('close', () => {
           commsRegistry.setItem(kernelId, null);
         });
       }
 
+      // Enable fullscreen output if any
+      updateOutputs();
+
       return {
         createWebSocket: () => {
           return new TrameJupyterWebSocket(childWindow, comm!);
         }
       };
     }
 
     const namespace = {
       app,
       kernelsRegistry,
       commsRegistry,
-      init
+      init,
+      updateOutputs
     };
 
     (window as any).trameJupyter = namespace;
 
     const { endpoint, www } = await getExtensionLocation();
 
     app.docRegistry.addWidgetExtension(
```

### Comparing `trame_jupyter_extension-2.0.1/src/location.ts` & `trame_jupyter_extension-2.1.0/src/location.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/src/manager.ts` & `trame_jupyter_extension-2.1.0/src/manager.ts`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/src/websocket.ts` & `trame_jupyter_extension-2.1.0/src/websocket.ts`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 import { ConcreteEmitter } from './emitter';
 import { TrameJupyterComm, type CommMessage } from './comm';
 
 type WebsocketMessage<T> = { data: T };
 
+function toBuffer(msgpack: any) {
+  if (msgpack.buffer) {
+    if (msgpack.buffer.byteLength !== msgpack.length) {
+      console.warn('toBuffer: deep copy');
+      const tmp = new Uint8Array(msgpack.length);
+      tmp.set(msgpack);
+      return tmp.buffer;
+    }
+    return msgpack.buffer;
+  }
+  return msgpack;
+}
+
 export type WebSocketEvents = {
   open: any;
   message: WebsocketMessage<any>;
   error: any;
   close: any;
 };
 
@@ -17,20 +30,14 @@
     __id += 1;
     return id.toString();
   };
 }
 
 const uniqueId = createUniqueIdFn();
 
-function isArrayBufferView(
-  array: ArrayBuffer | ArrayBufferView
-): array is ArrayBufferView {
-  return !!(array as any)?.buffer;
-}
-
 export class TrameJupyterWebSocket extends ConcreteEmitter<WebSocketEvents> {
   private window: any;
   private comm: TrameJupyterComm;
   private clientId: string;
   private serverName: string;
   private commMessageListener: (msg: CommMessage) => void;
   private commCloseListener: () => void;
@@ -57,24 +64,21 @@
       const { server, client, payload } = data;
 
       if (client !== this.clientId || server !== this.serverName) {
         return;
       }
 
       if (buffers && buffers.length > 0) {
-        const buffer: ArrayBuffer = isArrayBufferView(buffers[0])
-          ? buffers[0].buffer
-          : buffers[0];
-
-        // Buffer is ArrayBuffer, but it doesn't pass instanceof ArrayBuffer test in session.js (??!)
-        // make it!
-        (buffer as any).constructor = this.window.ArrayBuffer;
-        (buffer as any).__proto__ = this.window.ArrayBuffer.prototype;
+        const blob = new Blob(buffers);
+
+        // Make it a blob for wslink
+        blob.constructor = this.window.Blob;
+        (blob as any).__proto__ = this.window.Blob.prototype;
 
-        this.emit('message', { data: buffer });
+        this.emit('message', { data: blob });
       } else {
         this.emit('message', { data: payload });
       }
     };
 
     this.commCloseListener = () => this.close();
 
@@ -118,15 +122,15 @@
         server: this.serverName,
         client: this.clientId
       },
       buffers: []
     };
 
     if (isBinary) {
-      message.buffers = [data];
+      message.buffers = [toBuffer(data)];
     } else {
       message.data.payload = data;
     }
 
     this.comm.send(message);
   }
```

### Comparing `trame_jupyter_extension-2.0.1/trame_jupyter_extension/__init__.py` & `trame_jupyter_extension-2.1.0/trame_jupyter_extension/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 
     Parameters
     ----------
     server_app: jupyterlab.labapp.LabApp
         JupyterLab application instance
     """
     setup_handlers(server_app.web_app)
-    name = "trame_jupyter_extension"
+    name = "trame-jupyter-extension"
     server_app.log.info(f"Registered {name} server extension")
```

### Comparing `trame_jupyter_extension-2.0.1/trame_jupyter_extension/handlers.py` & `trame_jupyter_extension-2.1.0/trame_jupyter_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/.gitignore` & `trame_jupyter_extension-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/LICENSE` & `trame_jupyter_extension-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame_jupyter_extension-2.0.1/README.md` & `trame_jupyter_extension-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# trame_jupyter_extension
+# trame-jupyter-extension
 
 [![Github Actions Status](https://github.com/Kitware/trame-jupyter-extension/workflows/Build/badge.svg)](https://github.com/Kitware/trame-jupyter-extension/actions/workflows/build.yml)
 A JupyterLab extension for trame communication layer
 
-This extension is composed of a Python package named `trame_jupyter_extension`
+This extension is composed of a Python package named `trame-jupyter-extension`
 for the server extension and a NPM package named `trame-jupyter-extension`
 for the frontend extension.
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install trame_jupyter_extension
+pip install trame-jupyter-extension
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall trame_jupyter_extension
+pip uninstall trame-jupyter-extension
 ```
 
 ## Troubleshoot
 
 If you are seeing the frontend extension, but it is not working, check
 that the server extension is enabled:
 
@@ -51,21 +51,21 @@
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
-# Change directory to the trame_jupyter_extension directory
+# Change directory to the trame-jupyter-extension directory
 # Install package in development mode
 pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Server extension must be manually installed in develop mode
-jupyter server extension enable trame_jupyter_extension
+jupyter server extension enable trame-jupyter-extension
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
@@ -83,16 +83,16 @@
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
 # Server extension must be manually disabled in develop mode
-jupyter server extension disable trame_jupyter_extension
-pip uninstall trame_jupyter_extension
+jupyter server extension disable trame-jupyter-extension
+pip uninstall trame-jupyter-extension
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `trame-jupyter-extension` within that folder.
 
 ### Packaging the extension
```

### Comparing `trame_jupyter_extension-2.0.1/pyproject.toml` & `trame_jupyter_extension-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version>=0.3.2"]
 build-backend = "hatchling.build"
 
 [project]
-name = "trame_jupyter_extension"
+name = "trame-jupyter-extension"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 4",
```

### Comparing `trame_jupyter_extension-2.0.1/PKG-INFO` & `trame_jupyter_extension-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
-Name: trame_jupyter_extension
-Version: 2.0.1
+Metadata-Version: 2.3
+Name: trame-jupyter-extension
+Version: 2.1.0
+Dynamic: Keywords
 Summary: A JupyterLab extension for trame communication layer
 Project-URL: Homepage, https://github.com/Kitware/trame-jupyter-extension
 Project-URL: Bug Tracker, https://github.com/Kitware/trame-jupyter-extension/issues
 Project-URL: Repository, https://github.com/Kitware/trame-jupyter-extension.git
 Author-email: "Kitware Inc." <sebastien.jourdain@kitware.com>
 License: BSD 3-Clause License
         
@@ -50,41 +51,41 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: jupyter-server<3,>=2.0.1
 Requires-Dist: jupyterlab<5,>=4
 Requires-Dist: trame>=3.2.7
 Description-Content-Type: text/markdown
 
-# trame_jupyter_extension
+# trame-jupyter-extension
 
 [![Github Actions Status](https://github.com/Kitware/trame-jupyter-extension/workflows/Build/badge.svg)](https://github.com/Kitware/trame-jupyter-extension/actions/workflows/build.yml)
 A JupyterLab extension for trame communication layer
 
-This extension is composed of a Python package named `trame_jupyter_extension`
+This extension is composed of a Python package named `trame-jupyter-extension`
 for the server extension and a NPM package named `trame-jupyter-extension`
 for the frontend extension.
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install trame_jupyter_extension
+pip install trame-jupyter-extension
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall trame_jupyter_extension
+pip uninstall trame-jupyter-extension
 ```
 
 ## Troubleshoot
 
 If you are seeing the frontend extension, but it is not working, check
 that the server extension is enabled:
 
@@ -107,21 +108,21 @@
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
-# Change directory to the trame_jupyter_extension directory
+# Change directory to the trame-jupyter-extension directory
 # Install package in development mode
 pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Server extension must be manually installed in develop mode
-jupyter server extension enable trame_jupyter_extension
+jupyter server extension enable trame-jupyter-extension
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
@@ -139,16 +140,16 @@
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
 # Server extension must be manually disabled in develop mode
-jupyter server extension disable trame_jupyter_extension
-pip uninstall trame_jupyter_extension
+jupyter server extension disable trame-jupyter-extension
+pip uninstall trame-jupyter-extension
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `trame-jupyter-extension` within that folder.
 
 ### Packaging the extension
```

