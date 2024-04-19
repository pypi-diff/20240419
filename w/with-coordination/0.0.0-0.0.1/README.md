# Comparing `tmp/with_coordination-0.0.0.tar.gz` & `tmp/with_coordination-0.0.1.tar.gz`

## Comparing `with_coordination-0.0.0.tar` & `with_coordination-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 with_coordination-0.0.0/.python-version
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 with_coordination-0.0.0/requirements-dev.lock
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 with_coordination-0.0.0/requirements.lock
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 with_coordination-0.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 with_coordination-0.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 with_coordination-0.0.0/src/with_coordination/__init__.py
--rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 with_coordination-0.0.0/tests/test_with_coordination.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 with_coordination-0.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 with_coordination-0.0.0/LICENSE
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 with_coordination-0.0.0/README.md
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 with_coordination-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 with_coordination-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 with_coordination-0.0.1/.python-version
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 with_coordination-0.0.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 with_coordination-0.0.1/requirements.lock
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 with_coordination-0.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 with_coordination-0.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 with_coordination-0.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 with_coordination-0.0.1/src/with_coordination/__init__.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 with_coordination-0.0.1/tests/test_with_coordination.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 with_coordination-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 with_coordination-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 with_coordination-0.0.1/README.md
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 with_coordination-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 with_coordination-0.0.1/PKG-INFO
```

### Comparing `with_coordination-0.0.0/requirements-dev.lock` & `with_coordination-0.0.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `with_coordination-0.0.0/requirements.lock` & `with_coordination-0.0.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `with_coordination-0.0.0/.github/workflows/ci.yml` & `with_coordination-0.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `with_coordination-0.0.0/.github/workflows/release.yml` & `with_coordination-0.0.1/.github/workflows/release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -5,36 +5,39 @@
     tags:
       - "v*"
 
 jobs:
 
   Release:
     runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/p/with-coordination
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
       # For generating GitHub Releases + Release notes
       # ref: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#permissions
       contents: write
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - run: |
           pip install uv
           uv pip install --system build
           python -m build
 
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
 
-      - uses: actions/setup-node@v3
+      - uses: actions/setup-node@v4
         with:
           node-version: 18.x
       - run: npx changelogithub@0.12
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `with_coordination-0.0.0/src/with_coordination/__init__.py` & `with_coordination-0.0.1/src/with_coordination/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 with Coordination("config.json") as c:
     c.use_widget(slider1, view_id"slider1", aliases={"value": "sliderValue"})
     c.use_widget(slider2, view_id"slider2", aliases={"value": "sliderValue"})
     c.use_widget(slider3, view_id"slider3", aliases={"value": "sliderValue"})
 ```
 """
 
-import dataclasses
 import pathlib
 import typing
 import weakref
 
 import ipywidgets
 import msgspec
 
@@ -64,55 +63,65 @@
     name: str
     value: typing.Any
 
 
 class View(msgspec.Struct):
     widget: ipywidgets.Widget
     aliases: typing.Dict[str, str] = {}
+    jslinks: typing.Set[str] = set()
 
     def alias(self, **kwargs):
         self.aliases.update({v: k for k, v in kwargs.items()})
         return self
 
+    def jslink(self, field: str):
+        self.jslinks.add(field)
+        return self
+
 
 def _resolve_scope_and_link(
     config: CoordinationConfig, scope: CoordinationScope, views: typing.Dict[str, View]
 ):
-    resolved: list[tuple[ipywidgets.Widget, str]] = []
+    resolved: list[tuple[ipywidgets.Widget, str, bool]] = []
     for view_name, view_config in config.view_coordination.items():
         view_scopes = view_config.coordination_scopes
         if scope.type not in view_scopes or scope.name not in view_scopes[scope.type]:
             continue
 
         # get the coresponding view
         view = views[view_name]
         # resolve the alias, fallback to scope name
         field = view.aliases.get(scope.type, scope.type)
         # set the current value to the scope
         setattr(view.widget, field, scope.value)
         # keep the resolved so we can link them together
-        resolved.append((view.widget, field))
+        resolved.append((view.widget, field, field in view.jslinks))
 
     if len(resolved) == 0:
         return []
 
     links: list[ipywidgets.link] = []
 
     # link all the resolved scopes together
     # TODO: there probably is a better way to do this.
     # Ideally, on the Python side we have one "Model" for the scope
     # and on the JS side the same. But maybe for now this is fine...
-    v1, f1 = resolved[0]
-    for view, field in resolved[1:]:
-        link = ipywidgets.link((v1, f1), (view, field))
+    v1, f1, should_jslink1 = resolved[0]
+    for view, field, should_jslink in resolved[1:]:
+        if should_jslink1 and should_jslink:
+            link = ipywidgets.jslink((v1, f1), (view, field))
+        else:
+            link = ipywidgets.link((v1, f1), (view, field))
         links.append(link)
     return links
 
 
-WIDGET_COORDINATION_IDS = weakref.WeakKeyDictionary()
+WIDGET_COORDINATION_IDS: "weakref.WeakKeyDictionary[ipywidgets.Widget, int]" = (
+    weakref.WeakKeyDictionary()
+)
 # TODO: We should try to use weakrefs here as well
 LINKS = {}
 
 
 class Coordination:
     """Register and coordinate Jupyter widgets with a declarative API.
 
@@ -129,33 +138,43 @@
         else:
             contents = pathlib.Path(config).read_text(encoding="utf-8")
             self._config = msgspec.json.decode(contents, type=CoordinationConfig)
         self._views: typing.Dict[str, View] = {}
         self._unknown_view_id = 0
 
     def use_widget(
-        self, widget: ipywidgets.Widget, view_id: str, aliases: dict
+        self,
+        widget: ipywidgets.Widget,
+        view_id: str,
+        aliases: typing.Union[typing.Dict[str, str], None] = None,
+        jslinks: typing.Union[typing.Set[str], None] = None,
     ) -> None:
         """Register a widget as a view in the coordination space.
 
         Parameters
         ----------
         widget : ipywidgets.Widget
             The widget to be registered.
         view_id : str
             The view id of the widget.
-        aliases : dict
+        aliases : dict (optional)
             A dictionary mapping widget fields to coordination types in the
             coordination space.
+        jslinks : set (optional)
+            A set of widget fields that should be linked using ipywidgets.jslink.
         """
-        self._views[view_id] = View(widget).alias(**aliases)
+        self._views[view_id] = View(
+            widget,
+            jslinks=jslinks or set(),
+            aliases={v: k for k, v in (aliases or {}).items()},
+        )
 
-    def type(self, type: str) -> "CoordinationTypeContext":
+    def type(self, type: str, jslink: bool = False) -> "CoordinationTypeContext":
         """Enter the coordination type context."""
-        return CoordinationTypeContext(_coord=self, _type=type)
+        return CoordinationTypeContext(coordination=self, type=type, jslink=jslink)
 
     def __enter__(self) -> "Coordination":
         """Enter the coordination context."""
         return self
 
     def __exit__(self, *_: object) -> None:
         """Exit the coordination context.
@@ -194,82 +213,102 @@
         """Serialize the coordination configuration to use-coordination JSON format."""
         return msgspec.json.encode(self._config).decode("utf-8")
 
 
 T = typing.TypeVar("T")
 
 
-@dataclasses.dataclass
 class CoordinationTypeContext:
-    _coord: Coordination
-    _type: str
+    def __init__(self, coordination: Coordination, type: str, jslink: bool = False):
+        self._coord = coordination
+        self._type = type
+        self._jslink = jslink
 
     def __enter__(self):
         """Enter the coordination type context."""
         return self
 
     def __exit__(self, *_: object):
         """Exit the coordination type context."""
         pass
 
-    def scope(self, name: str, value: T) -> "CoordinationScopeContext[T]":
+    def scope(
+        self, name: str, value: T, jslink: bool = False
+    ) -> "CoordinationScopeContext[T]":
         """Enter the coordination scope context.
 
         Parameters
         ----------
         name : str
             The name of the coordination scope.
         value : T
             The value of the coordination scope.
+        jslink : bool
+            Whether to use ipywidgets.jslink when linking views for this scope.
 
         Returns
         -------
         CoordinationScopeContext
             The coordination scope context.
         """
         self._coord._config.coordination_space[self._type] = (
             self._coord._config.coordination_space.get(self._type, {})
         )
         self._coord._config.coordination_space[self._type][name] = value
         return CoordinationScopeContext(
-            _cood=self._coord, _type=self._type, _name=name, _value=value
+            coordination=self._coord,
+            type=self._type,
+            name=name,
+            value=value,
+            jslink=jslink or self._jslink,
         )
 
 
-@dataclasses.dataclass
 class CoordinationScopeContext(typing.Generic[T]):
-    _cood: Coordination
-    _type: str
-    _name: str
-    _value: T
+    def __init__(
+        self,
+        coordination: Coordination,
+        type: str,
+        name: str,
+        value: T,
+        jslink: bool,
+    ):
+        self._coord = coordination
+        self._type = type
+        self._name = name
+        self._value = value
+        self._jslink = jslink
 
     def __enter__(self):
         """Enter the coordination scope context."""
         return self
 
     def __exit__(self, *_: object):
         """Exit the coordination scope context."""
         pass
 
     def view(
         self,
         widget: typing.Union[ipywidgets.Widget, None] = None,
         id: typing.Union[str, None] = None,
         alias: typing.Union[str, None] = None,
+        jslink: bool = False,
     ):
         """Register a widget as a view in the coordination space.
 
         Parameters
         ----------
         widget : ipywidgets.Widget
             The widget to be registered.
         id : str
             The view id of the widget.
         alias : str
             The alias of the widget field in the coordination space.
+        jslink : bool
+            Whether to use ipywidgets.jslink to link this view this scope.
 
         Raises
         ------
         ValueError
             If neither widget nor id is provided.
 
         Notes
@@ -280,31 +319,36 @@
         if widget is None and id is None:
             raise ValueError("Either widget or id must be provided")
 
         view_id = id
 
         if view_id is None:
             # Check if we have a for this widget already
-            for vid, view in self._cood._views.items():
+            for vid, view in self._coord._views.items():
                 if view.widget == widget:
                     view_id = vid
                     break
             else:
                 # If not, create a new one
-                view_id = f"view_{self._cood._unknown_view_id}"
-                self._cood._unknown_view_id += 1
+                view_id = f"view_{self._coord._unknown_view_id}"
+                self._coord._unknown_view_id += 1
 
         # write to the view coordination config
-        self._cood._config.view_coordination[view_id] = (
-            self._cood._config.view_coordination.get(view_id, ViewCoordinationConfig())
+        self._coord._config.view_coordination[view_id] = (
+            self._coord._config.view_coordination.get(view_id, ViewCoordinationConfig())
         )
-        self._cood._config.view_coordination[view_id].coordination_scopes[
+        self._coord._config.view_coordination[view_id].coordination_scopes[
             self._type
         ] = self._name
 
         if widget is None:
             return
 
         # register the widget view
-        self._cood._views[view_id] = self._cood._views.get(view_id, View(widget))
+        self._coord._views[view_id] = self._coord._views.get(view_id, View(widget))
+
         if alias is not None:
-            self._cood._views[view_id].alias(**{alias: self._type})
+            self._coord._views[view_id].alias(**{alias: self._type})
+
+        if jslink or self._jslink:
+            # tag the widget for jslinking later
+            self._coord._views[view_id].jslink(alias or self._type)
```

### Comparing `with_coordination-0.0.0/tests/test_with_coordination.py` & `with_coordination-0.0.1/tests/test_with_coordination.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+from unittest.mock import patch
 
 import pytest
 from inline_snapshot import snapshot
 from ipywidgets import FloatSlider
 
 from with_coordination import Coordination
 
@@ -159,7 +160,42 @@
     assert slider2.value == 0.75
     assert slider3.value == 0.75
 
     slider2.value = 0.8
     assert slider1.value == 0.6
     assert slider2.value == 0.8
     assert slider3.value == 0.8
+
+
+def test_jslink_for_type():
+    slider1 = FloatSlider()
+    slider2 = FloatSlider()
+
+    with patch("ipywidgets.jslink") as jslink:
+        with Coordination() as c:
+            with c.type("sliderValue", jslink=True) as t:
+                with t.scope("A", 10) as s:
+                    s.view(slider1, alias="value")
+                    s.view(slider2, alias="value")
+
+        assert jslink.call_count == 1
+
+
+def test_jslink_for_scope():
+    slider1 = FloatSlider()
+    slider2 = FloatSlider()
+
+    slider3 = FloatSlider()
+    slider4 = FloatSlider()
+
+    with patch("ipywidgets.jslink") as jslink:
+        with Coordination() as c:
+            with c.type("sliderValue") as t:
+                with t.scope("A", 10, jslink=True) as s:
+                    s.view(slider1, alias="value")
+                    s.view(slider2, alias="value")
+
+                with t.scope("B", 4.0) as s:
+                    s.view(slider3, alias="value")
+                    s.view(slider4, alias="value")
+
+        assert jslink.call_count == 1
```

### Comparing `with_coordination-0.0.0/LICENSE` & `with_coordination-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `with_coordination-0.0.0/README.md` & `with_coordination-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `with_coordination-0.0.0/pyproject.toml` & `with_coordination-0.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [project]
 name = "with-coordination"
-version = "0.0.0"
-description = "Add your description here"
+dynamic = ["version"]
+description = "Declarative coordinated multiple views for Jupyter Widgets"
 authors = [{ name = "Trevor Manz", email = "trevor.j.manz@gmail.com" }]
 dependencies = ["ipywidgets>=8.1.2", "traitlets>=5.14.2", "msgspec>=0.18.6"]
 readme = "README.md"
 requires-python = ">= 3.8"
 
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "jupyterlab-vim>=4.1.3",
     "jupyterlab>=4.1.6",
     "pytest>=8.1.1",
     "inline-snapshot>=0.8.0",
 ]
 
+[tool.hatch.version]
+source = "vcs"
+
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/with_coordination"]
 
 [tool.ruff]
```

### Comparing `with_coordination-0.0.0/PKG-INFO` & `with_coordination-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: with-coordination
-Version: 0.0.0
-Summary: Add your description here
+Version: 0.0.1
+Summary: Declarative coordinated multiple views for Jupyter Widgets
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: ipywidgets>=8.1.2
 Requires-Dist: msgspec>=0.18.6
 Requires-Dist: traitlets>=5.14.2
 Description-Content-Type: text/markdown
```

