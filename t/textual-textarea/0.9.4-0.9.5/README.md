# Comparing `tmp/textual_textarea-0.9.4.tar.gz` & `tmp/textual_textarea-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.9.4.tar", max compression
+gzip compressed data, was "textual_textarea-0.9.5.tar", max compression
```

## Comparing `textual_textarea-0.9.4.tar` & `textual_textarea-0.9.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-12-18 17:16:56.614515 textual_textarea-0.9.4/LICENSE
--rw-r--r--   0        0        0     5740 2023-12-18 17:16:56.614515 textual_textarea-0.9.4/README.md
--rw-r--r--   0        0        0     1614 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      388 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0     1041 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/__main__.py
--rw-r--r--   0        0        0     7502 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/autocomplete.py
--rw-r--r--   0        0        0     7599 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     3510 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/comments.py
--rw-r--r--   0        0        0     1190 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2019 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0      292 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      887 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/messages.py
--rw-r--r--   0        0        0     4128 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/path_input.py
--rw-r--r--   0        0        0        0 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/py.typed
--rw-r--r--   0        0        0      450 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/serde.py
--rw-r--r--   0        0        0    42145 2023-12-18 17:16:56.618515 textual_textarea-0.9.4/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     6729 1970-01-01 00:00:00.000000 textual_textarea-0.9.4/setup.py
--rw-r--r--   0        0        0     6546 1970-01-01 00:00:00.000000 textual_textarea-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/LICENSE
+-rw-r--r--   0        0        0     5740 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/README.md
+-rw-r--r--   0        0        0     1614 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0     1041 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/__main__.py
+-rw-r--r--   0        0        0     7502 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/autocomplete.py
+-rw-r--r--   0        0        0     7599 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     3510 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/comments.py
+-rw-r--r--   0        0        0     1190 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2019 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0      292 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      887 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0     4128 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/path_input.py
+-rw-r--r--   0        0        0        0 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0      450 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/serde.py
+-rw-r--r--   0        0        0    42523 2023-12-18 19:38:52.165058 textual_textarea-0.9.5/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     6729 1970-01-01 00:00:00.000000 textual_textarea-0.9.5/setup.py
+-rw-r--r--   0        0        0     6546 1970-01-01 00:00:00.000000 textual_textarea-0.9.5/PKG-INFO
```

### Comparing `textual_textarea-0.9.4/LICENSE` & `textual_textarea-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/README.md` & `textual_textarea-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/pyproject.toml` & `textual_textarea-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.9.4"
+version = "0.9.5"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
```

### Comparing `textual_textarea-0.9.4/src/textual_textarea/__main__.py` & `textual_textarea-0.9.5/src/textual_textarea/__main__.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/autocomplete.py` & `textual_textarea-0.9.5/src/textual_textarea/autocomplete.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/colors.py` & `textual_textarea-0.9.5/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/comments.py` & `textual_textarea-0.9.5/src/textual_textarea/comments.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/containers.py` & `textual_textarea-0.9.5/src/textual_textarea/containers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/error_modal.py` & `textual_textarea-0.9.5/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/messages.py` & `textual_textarea-0.9.5/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/path_input.py` & `textual_textarea-0.9.5/src/textual_textarea/path_input.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.9.4/src/textual_textarea/textarea.py` & `textual_textarea-0.9.5/src/textual_textarea/textarea.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,23 @@
         self._create_undo_snapshot()
         self.undo_timer.pause()
 
     def on_focus(self) -> None:
         self.undo_timer.reset()
 
     def on_key(self, event: events.Key) -> None:
+        # Naked shift or ctrl keys on Windows get sent as NUL chars; Textual
+        # interprets these as `ctrl+@` presses, which is inconsistent with
+        # other platforms. We ignore these presses.
+        # https://github.com/Textualize/textual/issues/872
+        if event.key == "ctrl+@":
+            event.stop()
+            event.prevent_default()
+            return
+
         self.undo_timer.reset()
         if event.key in (
             "apostrophe",
             "quotation_mark",
             "left_parenthesis",
             "left_square_bracket",
             "left_curly_bracket",
```

### Comparing `textual_textarea-0.9.4/setup.py` & `textual_textarea-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyperclip>=1.8.2,<2.0.0', 'textual[syntax]>=0.41.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
     'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.svg)\n\n## Note: This is **NOT** the official TextArea widget!\n\nWith v0.38.0, Textual added a built-in TextArea widget. You probably want to use \nthat widget instead of this one. This project predated the official widget; versions < v0.8.0\nhad a completely separate implmentation.\n\nSince v0.8.0, this project uses the built-in TextArea widget, but adds the features outlined below.\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for Pygments themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>ctrl+Home/End</kbd>).\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Select text by double-, triple-, or quadruple-clicking.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="nord-darker", id="ta")\n\n    def on_mount(self) -> None:\n        ta = self.query_one("#id", expect_type=TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`. Some Linux users may need to apt-install `xclip` or `xsel` to enable the system clipboard features.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\nSimilarly, the TextArea exposes a `selected_text` property (read-only):\n```python\nta = self.query_one(TextArea)\nselection = ta.selected_text\n```\n\n#### Inserting Text\n\nYou can insert text at the current selection:\n```python\nta = self.query_one(TextArea)\nta.text = "01234"\nta.cursor = (0, 2)\nta.insert_text_at_selection("\\nabc\\n")\nassert ta.text == "01\\nabc\\n234"\nassert ta.cursor == Cursor(lno=2, pos=0)\n```\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\nSimilarly, there is a `selection_anchor` property (`Union[None, Cursor]`):\n\n```python\nta = self.query_one(TextArea)\nanchor = ta.selection_anchor # will be None if no text is selected\nta.selection_anchor = (999, 0)  # the anchor will move as close to line 999, pos 0 as possible\nta.selection_anchor = None # the selection will be cleared\n```\n\n#### Getting and Setting The Language\n\nSyntax highlighting and comment insertion depends on the configured language for the TextArea.\n\nThe TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:\n\n```python\nta = self.query_one(TextArea)\nold_language = ta.language\nta.language = "python"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
```

### Comparing `textual_textarea-0.9.4/PKG-INFO` & `textual_textarea-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-textarea
-Version: 0.9.4
+Version: 0.9.5
 Summary: A text area (multi-line input) with syntax highlighting for Textual
 Home-page: https://github.com/tconbeer/textual-textarea
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

