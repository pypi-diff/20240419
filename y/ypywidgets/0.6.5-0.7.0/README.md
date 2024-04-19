# Comparing `tmp/ypywidgets-0.6.5.tar.gz` & `tmp/ypywidgets-0.7.0.tar.gz`

## Comparing `ypywidgets-0.6.5.tar` & `ypywidgets-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/ypywidgets/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/ypywidgets/comm.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/ypywidgets/reactive.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/ypywidgets/utils.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/ypywidgets/widget.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/LICENSE
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 ypywidgets-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/ypywidgets/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/ypywidgets/comm.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/ypywidgets/declare.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/ypywidgets/utils.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/ypywidgets/widget.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 ypywidgets-0.7.0/PKG-INFO
```

### Comparing `ypywidgets-0.6.5/ypywidgets/comm.py` & `ypywidgets-0.7.0/ypywidgets/comm.py`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.6.5/ypywidgets/utils.py` & `ypywidgets-0.7.0/ypywidgets/utils.py`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.6.5/ypywidgets/widget.py` & `ypywidgets-0.7.0/ypywidgets/widget.py`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.6.5/LICENSE` & `ypywidgets-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ypywidgets-0.6.5/README.md` & `ypywidgets-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Build Status](https://github.com/davidbrochart/ypywidgets/workflows/CI/badge.svg)](https://github.com/davidbrochart/ypywidgets/actions)
 
 # ypywidgets: Y-based Jupyter widgets for Python
 
 `ypywidgets` is a communication backend between a Jupyter kernel and clients. It allows to synchronize data structures that can be modified concurrently, and automatically resolves conflicts. To do so, it uses:
 - the Jupyter kernel [Comm](https://jupyter-client.readthedocs.io/en/stable/messaging.html#custom-messages) protocol as the transport layer, and the [comm](https://github.com/ipython/comm) implementation of it.
 - the [pycrdt](https://github.com/davidbrochart/pycrdt) CRDT implementation.
-- the [reacttrs](https://github.com/davidbrochart/reacttrs) package that implements the observer pattern.
+- the [declare](https://github.com/willmcgugan/declare) library that implements the observer pattern and validation.
 
 It is a replacement for (a part of) [ipywidgets](https://ipywidgets.readthedocs.io). When used with [yjs-widgets](https://github.com/davidbrochart/yjs-widgets), it supports JupyterLab clients that implement widgets. The difference with `ipywidgets` is that these widgets are collaborative: they can be manipulated concurrently from the kernel or from any client. The CRDT algorithm ensures that a widget state will eventually be consistent across all clients.
```

### Comparing `ypywidgets-0.6.5/pyproject.toml` & `ypywidgets-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "widgets",
     "jupyter",
     "yjs",
 ]
 dependencies = [
     "comm >=0.1.4,<1",
     "pycrdt >=0.8.2,<0.9.0",
-    "reacttrs >=0.1.4,<1",
+    "declare >=1.0.1,<2.0.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/davidbrochart/ypywidgets"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `ypywidgets-0.6.5/PKG-INFO` & `ypywidgets-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ypywidgets
-Version: 0.6.5
+Version: 0.7.0
 Summary: Y-based Jupyter widgets for Python
 Project-URL: Homepage, https://github.com/davidbrochart/ypywidgets
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: jupyter,widgets,yjs
 Requires-Python: >=3.8
 Requires-Dist: comm<1,>=0.1.4
+Requires-Dist: declare<2.0.0,>=1.0.1
 Requires-Dist: pycrdt<0.9.0,>=0.8.2
-Requires-Dist: reacttrs<1,>=0.1.4
 Provides-Extra: dev
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/davidbrochart/ypywidgets/workflows/CI/badge.svg)](https://github.com/davidbrochart/ypywidgets/actions)
 
 # ypywidgets: Y-based Jupyter widgets for Python
 
 `ypywidgets` is a communication backend between a Jupyter kernel and clients. It allows to synchronize data structures that can be modified concurrently, and automatically resolves conflicts. To do so, it uses:
 - the Jupyter kernel [Comm](https://jupyter-client.readthedocs.io/en/stable/messaging.html#custom-messages) protocol as the transport layer, and the [comm](https://github.com/ipython/comm) implementation of it.
 - the [pycrdt](https://github.com/davidbrochart/pycrdt) CRDT implementation.
-- the [reacttrs](https://github.com/davidbrochart/reacttrs) package that implements the observer pattern.
+- the [declare](https://github.com/willmcgugan/declare) library that implements the observer pattern and validation.
 
 It is a replacement for (a part of) [ipywidgets](https://ipywidgets.readthedocs.io). When used with [yjs-widgets](https://github.com/davidbrochart/yjs-widgets), it supports JupyterLab clients that implement widgets. The difference with `ipywidgets` is that these widgets are collaborative: they can be manipulated concurrently from the kernel or from any client. The CRDT algorithm ensures that a widget state will eventually be consistent across all clients.
```

