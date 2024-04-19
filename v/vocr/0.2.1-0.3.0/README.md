# Comparing `tmp/vocr-0.2.1.tar.gz` & `tmp/vocr-0.3.0.tar.gz`

## Comparing `vocr-0.2.1.tar` & `vocr-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,25 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/__main__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/py.typed
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/vocr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/test_ocr.py
--rw-r--r--   0        0        0    16977 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/img/sample1.jpg
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/img/sample2.jpg
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 vocr-0.2.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 vocr-0.2.1/LICENSE
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 vocr-0.2.1/README.md
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 vocr-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 vocr-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 vocr-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 vocr-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 vocr-0.3.0/docs/modules.rst
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 vocr-0.3.0/docs/vocr.rst
+-rw-r--r--   0        0        0   204926 2020-02-02 00:00:00.000000 vocr-0.3.0/images/vocr.ico
+-rw-r--r--   0        0        0    40420 2020-02-02 00:00:00.000000 vocr-0.3.0/images/vocr.png
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 vocr-0.3.0/images/vocr.svg
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/__main__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/cli.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/gui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/py.typed
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/vocr.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/res/__init__.py
+-rw-r--r--   0        0        0   204926 2020-02-02 00:00:00.000000 vocr-0.3.0/src/vocr/res/vocr.ico
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vocr-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 vocr-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 vocr-0.3.0/tests/test_ocr.py
+-rw-r--r--   0        0        0    16977 2020-02-02 00:00:00.000000 vocr-0.3.0/tests/img/sample1.jpg
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 vocr-0.3.0/tests/img/sample2.jpg
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 vocr-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 vocr-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 vocr-0.3.0/README.md
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 vocr-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 vocr-0.3.0/PKG-INFO
```

### Comparing `vocr-0.2.1/src/vocr/cli.py` & `vocr-0.3.0/src/vocr/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import platform
 from pathlib import Path
 
 import click
 
 from vocr import __title__, __version__
+from vocr.gui import app_run
 from vocr.vocr import VietOCR
 
 
 @click.command(name="version")
 def version() -> None:
     """Show current version"""
     ver_msg = f"{__title__} v{__version__}"
@@ -44,15 +45,22 @@
 )
 def ocr(src: str, preprocess: str, output: str) -> None:
     """Performs OCR on file/directory"""
     instance = VietOCR(Path(src))
     instance.ocr(save_destination=output, preprocess=preprocess)  # type: ignore
 
 
+@click.command(name="gui")
+def gui() -> None:
+    """Run vocr with GUI"""
+    app_run()
+
+
 @click.group(name="cli")
 def cli() -> None:
     """vocr's command line interface"""
     pass
 
 
 cli.add_command(version)
 cli.add_command(ocr)
+cli.add_command(gui)
```

### Comparing `vocr-0.2.1/src/vocr/vocr.py` & `vocr-0.3.0/src/vocr/vocr.py`

 * *Files identical despite different names*

### Comparing `vocr-0.2.1/tests/conftest.py` & `vocr-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vocr-0.2.1/tests/img/sample1.jpg` & `vocr-0.3.0/tests/img/sample1.jpg`

 * *Files identical despite different names*

### Comparing `vocr-0.2.1/tests/img/sample2.jpg` & `vocr-0.3.0/tests/img/sample2.jpg`

 * *Files identical despite different names*

### Comparing `vocr-0.2.1/.gitignore` & `vocr-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vocr-0.2.1/LICENSE` & `vocr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vocr-0.2.1/README.md` & `vocr-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,35 +20,40 @@
 
 ## Install
 
 ```
 pip install vocr
 ```
 
-## Usage:
+## Usage
 
 ### Run in Terminal
 ```
 vocr --help
 ```
 ```
 Usage: vocr [OPTIONS] COMMAND [ARGS]...
 
   vocr's command line interface
 
 Options:
   --help  Show this message and exit.
 
 Commands:
+  gui      Run vocr with GUI
   ocr      Performs OCR on file/directory
   version  Show current version
 ```
 
 ### Run in script
 ```python
 from vocr import VietOCR
 VietOCR(<path>).ocr()
 ```
 
+## Supported file
+
+- `.jpg`, `.jpeg`, `.png`
+
 ## LICENSE
 
 MIT License
```

### Comparing `vocr-0.2.1/pyproject.toml` & `vocr-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     # "Development Status :: 5 - Production/Stable",
     "Natural Language :: English",
 ]
 dependencies = [
     "click>=8.0.0",
+    "customtkinter",
+    "importlib_resources; python_version < '3.10'",
     "joblib",
     "opencv-python",
     "pillow",
     "pytesseract",
     "tqdm",
 ]
 dynamic = ["version"]
@@ -41,20 +43,23 @@
 
 [project.optional-dependencies]
 dev = ["hatch", "pytest>=7.0.0"]
 
 [project.scripts]
 vocr = "vocr.__main__:main"
 
+[project.gui-scripts]
+vocr-gui = "vocr.gui:app_run"
+
 # ========== TOOL ==========
 [tool.hatch.version]
 path = "src/vocr/__init__.py"
 
 [tool.hatch.build.targets.sdist]
-only-include = ["src", "tests"]
+only-include = ["src", "tests", "docs", "images"]
 exclude = ["tests/output"]
 
 [tool.hatch.envs.default]
 dependencies = ["coverage[toml]", "pytest-cov", "pytest"]
 description = """
 Default environment
 
@@ -164,13 +169,13 @@
 indent-width = 4
 target-version = "py38"
 include = ["pyproject.toml", "src/**", "tests/**"]
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
-exclude = ["*.json", "*.pkl", "*.jpg", "*.png", "*.jpeg", "*.txt"]
+exclude = ["*.json", "*.pkl", "*.jpg", "*.png", "*.jpeg", "*.txt", "*.ico"]
 
 [tool.ruff.lint]
 select = ["E4", "E7", "E9", "F", "B", "Q"]
 unfixable = ["B"]
-exclude = ["*.json", "*.pkl", "*.jpg", "*.png", "*.jpeg", "*.txt"]
+exclude = ["*.json", "*.pkl", "*.jpg", "*.png", "*.jpeg", "*.txt", "*.ico"]
```

### Comparing `vocr-0.2.1/PKG-INFO` & `vocr-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocr
-Version: 0.2.1
+Version: 0.3.0
 Summary: Vietnamese OCR
 Project-URL: Homepage, https://github.com/AbsoluteWinter/vocr
 Project-URL: Repository, https://github.com/AbsoluteWinter/vocr
 Project-URL: Issues, https://github.com/AbsoluteWinter/vocr/issues
 Author: AbsoluteWinter
 License: MIT License
 License-File: LICENSE
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <4,>=3.8
 Requires-Dist: click>=8.0.0
+Requires-Dist: customtkinter
+Requires-Dist: importlib-resources; python_version < '3.10'
 Requires-Dist: joblib
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 Requires-Dist: pytesseract
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
@@ -52,35 +54,40 @@
 
 ## Install
 
 ```
 pip install vocr
 ```
 
-## Usage:
+## Usage
 
 ### Run in Terminal
 ```
 vocr --help
 ```
 ```
 Usage: vocr [OPTIONS] COMMAND [ARGS]...
 
   vocr's command line interface
 
 Options:
   --help  Show this message and exit.
 
 Commands:
+  gui      Run vocr with GUI
   ocr      Performs OCR on file/directory
   version  Show current version
 ```
 
 ### Run in script
 ```python
 from vocr import VietOCR
 VietOCR(<path>).ocr()
 ```
 
+## Supported file
+
+- `.jpg`, `.jpeg`, `.png`
+
 ## LICENSE
 
 MIT License
```

