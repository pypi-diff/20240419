# Comparing `tmp/outspin-0.3.0.tar.gz` & `tmp/outspin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outspin-0.3.0.tar", max compression
+gzip compressed data, was "outspin-0.3.1.tar", max compression
```

## Comparing `outspin-0.3.0.tar` & `outspin-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1057 2024-01-28 15:05:03.231433 outspin-0.3.0/LICENSE
--rw-r--r--   0        0        0     6968 2024-01-28 15:12:03.320979 outspin-0.3.0/README.md
--rw-r--r--   0        0        0     1053 2024-01-28 15:14:07.867531 outspin-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      720 2024-01-28 13:51:06.216032 outspin-0.3.0/src/outspin/__init__.py
--rw-r--r--   0        0        0      285 2024-01-28 13:30:06.837380 outspin-0.3.0/src/outspin/constants.py
--rw-r--r--   0        0        0      321 2024-01-28 13:37:17.150786 outspin-0.3.0/src/outspin/exceptions.py
--rw-r--r--   0        0        0     2278 2024-01-28 14:01:30.665428 outspin-0.3.0/src/outspin/unix.py
--rw-r--r--   0        0        0     1709 2024-01-28 14:14:20.364442 outspin-0.3.0/src/outspin/windows.py
--rw-r--r--   0        0        0     7514 1970-01-01 00:00:00.000000 outspin-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-01-28 15:05:03.231433 outspin-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7000 2024-04-03 21:43:21.246732 outspin-0.3.1/README.md
+-rw-r--r--   0        0        0     1125 2024-04-09 19:53:54.397507 outspin-0.3.1/outspin/__init__.py
+-rw-r--r--   0        0        0      285 2024-01-28 13:30:06.837380 outspin-0.3.1/outspin/constants.py
+-rw-r--r--   0        0        0      321 2024-01-28 13:37:17.150786 outspin-0.3.1/outspin/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:53:20.976750 outspin-0.3.1/outspin/py.typed
+-rw-r--r--   0        0        0     2472 2024-04-09 19:46:12.969478 outspin-0.3.1/outspin/unix.py
+-rw-r--r--   0        0        0     1891 2024-04-14 18:16:33.560291 outspin-0.3.1/outspin/windows.py
+-rw-r--r--   0        0        0     1093 2024-04-19 20:56:04.935037 outspin-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 outspin-0.3.1/PKG-INFO
```

### Comparing `outspin-0.3.0/LICENSE` & `outspin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `outspin-0.3.0/README.md` & `outspin-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     main(int(sys.argv[1] if len(sys.argv) > 1 else 30))
 ```
 </details>
 
 ## Reference
 
 ### `get_key`
-> Signature: `() -> None`
+> Signature: `() -> str`
 
 Returns a keypress from standard input. It exclusively identifies keypresses
 that result in tangible inputs, therefore modifier keys like `shift` or
 `caps lock` are ignored. `outspin` also returns the actual input, meaning that
 pressing, for instance, `shift+a` will make `get_key()` return `A`.
 
 > [!Note]
@@ -221,32 +221,27 @@
 * Some combinations (like `shift+up` or `alt+shift+right`) may not work
   correctly on Windows.
 
 ## Contributing
 
 Contributions are welcome! 
 
-Please open an issue before submitting a pull request
-(doesn't apply to minor changes like typos).
+Please open an issue before submitting a pull request (unless it's a minor
+change like fixing a typo).
 
 To get started:
-
-1. Clone the project:
-```bash
-git clone https://github.com/trag1c/outspin.git
-```
-
+1. Clone your fork of the project.
 2. Set up the project with [just] (make sure you have [poetry] installed):
 ```bash
 just install
 ```
 
 > [!Note]
 > If you don't want to install `just`, simply look up the recipes
-> in the project's `justfile`.
+> in the project's [`justfile`][justfile].
 
 3. After you're done, use the following `just` recipes to check your changes:
 ```bash
 just check     # pytest, mypy, ruff 
 just coverage  # pytest (with coverage), interrogate (docstring coverage)
 ```
 
@@ -255,8 +250,9 @@
 © [trag1c], 2023–2024
 
 [MIT License]: https://opensource.org/license/mit/
 [poetry]: https://python-poetry.org/
 [just]: https://github.com/casey/just/
 [trag1c]: https://github.com/trag1c/
 [dahlia]: https://github.com/dahlia-lib/dahlia/
-[nouns.txt]: https://gist.github.com/trag1c/f74b2ab3589bc4ce5706f934616f6195/
+[nouns.txt]: https://gist.github.com/trag1c/f74b2ab3589bc4ce5706f934616f6195/
+[justfile]: https://github.com/trag1c/outspin/blob/main/justfile
```

### Comparing `outspin-0.3.0/src/outspin/unix.py` & `outspin-0.3.1/outspin/unix.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     raise OutspinImportError(msg)
 
 import os
 import termios
 import tty
 from string import ascii_uppercase
 
+assert sys.platform != "win32" and sys.platform != "cygwin"  # noqa: S101
+
 _MODS = {
     "\x1b": "esc",
     "\x7f": "backspace",
     "\x1b[3~": "delete",
     "\x1b[A": "up",
     "\x1b[B": "down",
     "\x1b[C": "right",
@@ -49,14 +51,18 @@
     "\x1b[1;4B": "shift+alt+down",
     "\x1b[1;4C": "shift+alt+right",
     "\x1b[1;4D": "shift+alt+left",
     "\x1b[1;10A": "shift+alt+up",
     "\x1b[1;10B": "shift+alt+down",
     "\x1b[1;10C": "shift+alt+right",
     "\x1b[1;10D": "shift+alt+left",
+    "\x1b[1;5A": "ctrl+up",
+    "\x1b[1;5B": "ctrl+down",
+    "\x1b[1;5D": "ctrl+left",
+    "\x1b[1;5C": "ctrl+right",
     "\x1b[1;6A": "shift+ctrl+up",
     "\x1b[1;6B": "shift+ctrl+down",
     "\x1b[1;6C": "shift+ctrl+right",
     "\x1b[1;6D": "shift+ctrl+left",
     "\x1b[1;2P": "shift+f1",
     "\x1b[1;2Q": "shift+f2",
     "\x1b[1;2R": "shift+f3",
```

### Comparing `outspin-0.3.0/src/outspin/windows.py` & `outspin-0.3.1/outspin/windows.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
     msg = "This module is only available on Windows."
     raise OutspinImportError(msg)
 
 import msvcrt
 from string import ascii_uppercase
 
+assert sys.platform == "win32" or sys.platform == "cygwin"  # noqa: S101
+
 _MODS = {
     b"\x1b": "esc",
     b"\x08": "backspace",
     b"\xe0S": "delete",
     b"\xe0H": "up",
     b"\xe0P": "down",
     b"\xe0M": "right",
@@ -67,8 +69,13 @@
     if ks in b"\x00\xe0":
         ks += msvcrt.getch()
     return ks
 
 
 def get_key() -> str:
     """Return a keypress from standard input."""
-    return _MODS.get(ch := _getch(), ch.decode("cp1252"))
+    if decoded := _MODS.get(ch := _getch()):
+        return decoded
+    try:
+        return ch.decode("cp1252")
+    except UnicodeDecodeError:
+        return str(ch)
```

### Comparing `outspin-0.3.0/PKG-INFO` & `outspin-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: outspin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Conveniently read single char inputs in the console.
 License: MIT
 Author: trag1c
 Author-email: trag1cdev@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # outspin
 
 `outspin` is a tiny, low-abstraction library bringing C's `getch()`
 functionality to Python, with a sane API. An ideal choice for developers seeking
 direct control over their TUI applications.
@@ -185,15 +186,15 @@
     main(int(sys.argv[1] if len(sys.argv) > 1 else 30))
 ```
 </details>
 
 ## Reference
 
 ### `get_key`
-> Signature: `() -> None`
+> Signature: `() -> str`
 
 Returns a keypress from standard input. It exclusively identifies keypresses
 that result in tangible inputs, therefore modifier keys like `shift` or
 `caps lock` are ignored. `outspin` also returns the actual input, meaning that
 pressing, for instance, `shift+a` will make `get_key()` return `A`.
 
 > [!Note]
@@ -237,32 +238,27 @@
 * Some combinations (like `shift+up` or `alt+shift+right`) may not work
   correctly on Windows.
 
 ## Contributing
 
 Contributions are welcome! 
 
-Please open an issue before submitting a pull request
-(doesn't apply to minor changes like typos).
+Please open an issue before submitting a pull request (unless it's a minor
+change like fixing a typo).
 
 To get started:
-
-1. Clone the project:
-```bash
-git clone https://github.com/trag1c/outspin.git
-```
-
+1. Clone your fork of the project.
 2. Set up the project with [just] (make sure you have [poetry] installed):
 ```bash
 just install
 ```
 
 > [!Note]
 > If you don't want to install `just`, simply look up the recipes
-> in the project's `justfile`.
+> in the project's [`justfile`][justfile].
 
 3. After you're done, use the following `just` recipes to check your changes:
 ```bash
 just check     # pytest, mypy, ruff 
 just coverage  # pytest (with coverage), interrogate (docstring coverage)
 ```
 
@@ -272,7 +268,9 @@
 
 [MIT License]: https://opensource.org/license/mit/
 [poetry]: https://python-poetry.org/
 [just]: https://github.com/casey/just/
 [trag1c]: https://github.com/trag1c/
 [dahlia]: https://github.com/dahlia-lib/dahlia/
 [nouns.txt]: https://gist.github.com/trag1c/f74b2ab3589bc4ce5706f934616f6195/
+[justfile]: https://github.com/trag1c/outspin/blob/main/justfile
+
```

