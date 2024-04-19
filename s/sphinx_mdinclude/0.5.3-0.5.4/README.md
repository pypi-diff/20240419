# Comparing `tmp/sphinx_mdinclude-0.5.3.tar.gz` & `tmp/sphinx_mdinclude-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_mdinclude-0.5.3.tar", last modified: Mon Oct 10 02:53:38 2022, max compression
+gzip compressed data, was "sphinx_mdinclude-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_mdinclude-0.5.3.tar` & `sphinx_mdinclude-0.5.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      180 2022-10-10 02:10:54.817284 sphinx_mdinclude-0.5.3/.flake8
--rw-r--r--   0        0        0      129 2022-10-10 02:10:54.817469 sphinx_mdinclude-0.5.3/.github/dependabot.yml
--rw-r--r--   0        0        0      139 2022-10-10 02:10:54.817583 sphinx_mdinclude-0.5.3/.github/issue_template.md
--rw-r--r--   0        0        0       61 2022-10-10 02:10:54.817683 sphinx_mdinclude-0.5.3/.github/pull_request_template.md
--rw-r--r--   0        0        0     1236 2022-10-10 02:10:54.817861 sphinx_mdinclude-0.5.3/.github/workflows/build.yml
--rw-r--r--   0        0        0     1091 2022-10-10 02:10:54.817997 sphinx_mdinclude-0.5.3/.gitignore
--rw-r--r--   0        0        0      156 2022-10-10 02:10:54.818105 sphinx_mdinclude-0.5.3/.readthedocs.yml
--rw-r--r--   0        0        0     6502 2022-10-10 02:44:48.647296 sphinx_mdinclude-0.5.3/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2022-10-10 02:10:54.818388 sphinx_mdinclude-0.5.3/LICENSE
--rw-r--r--   0        0        0     3026 2022-10-10 02:39:46.673444 sphinx_mdinclude-0.5.3/README.md
--rw-r--r--   0        0        0      598 2022-10-10 02:39:46.673757 sphinx_mdinclude-0.5.3/docs/_static/custom.css
--rw-r--r--   0        0        0    42080 2022-10-10 02:39:46.674177 sphinx_mdinclude-0.5.3/docs/_static/omnilib.png
--rw-r--r--   0        0        0      342 2022-10-10 02:23:46.061822 sphinx_mdinclude-0.5.3/docs/_templates/badges.html
--rw-r--r--   0        0        0     1145 2022-10-10 02:39:46.674374 sphinx_mdinclude-0.5.3/docs/_templates/omnilib.html
--rw-r--r--   0        0        0       71 2022-10-10 02:10:54.819195 sphinx_mdinclude-0.5.3/docs/changelog.rst
--rw-r--r--   0        0        0     2703 2022-10-10 02:39:46.674553 sphinx_mdinclude-0.5.3/docs/conf.py
--rw-r--r--   0        0        0     2988 2022-10-10 02:39:46.674723 sphinx_mdinclude-0.5.3/docs/example.md
--rw-r--r--   0        0        0       51 2022-10-10 02:10:54.819593 sphinx_mdinclude-0.5.3/docs/included.md
--rw-r--r--   0        0        0       99 2022-10-10 02:10:54.819731 sphinx_mdinclude-0.5.3/docs/index.md
--rw-r--r--   0        0        0      886 2022-10-10 02:10:54.819862 sphinx_mdinclude-0.5.3/makefile
--rw-r--r--   0        0        0     1577 2022-10-10 02:39:46.674921 sphinx_mdinclude-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      269 2022-10-10 02:10:54.820144 sphinx_mdinclude-0.5.3/requirements-dev.txt
--rw-r--r--   0        0        0       96 2022-10-10 02:10:54.820260 sphinx_mdinclude-0.5.3/requirements.txt
--rw-r--r--   0        0        0      310 2022-10-10 02:10:54.820443 sphinx_mdinclude-0.5.3/sphinx_mdinclude/__init__.py
--rw-r--r--   0        0        0      156 2022-10-10 02:44:48.652455 sphinx_mdinclude-0.5.3/sphinx_mdinclude/__version__.py
--rw-r--r--   0        0        0    15230 2022-10-10 02:10:54.820743 sphinx_mdinclude-0.5.3/sphinx_mdinclude/legacy.py
--rw-r--r--   0        0        0     3514 2022-10-10 02:10:54.820861 sphinx_mdinclude-0.5.3/sphinx_mdinclude/parse.py
--rw-r--r--   0        0        0     9691 2022-10-10 02:10:54.821053 sphinx_mdinclude-0.5.3/sphinx_mdinclude/render.py
--rw-r--r--   0        0        0     5107 2022-10-10 02:10:54.821253 sphinx_mdinclude-0.5.3/sphinx_mdinclude/sphinx.py
--rw-r--r--   0        0        0      246 2022-10-10 02:10:54.821505 sphinx_mdinclude-0.5.3/sphinx_mdinclude/tests/__init__.py
--rw-r--r--   0        0        0      167 2022-10-10 02:10:54.821624 sphinx_mdinclude-0.5.3/sphinx_mdinclude/tests/__main__.py
--rw-r--r--   0        0        0      357 2022-10-10 02:10:54.821732 sphinx_mdinclude-0.5.3/sphinx_mdinclude/tests/test.md
--rw-r--r--   0        0        0      422 2022-10-10 02:10:54.821830 sphinx_mdinclude-0.5.3/sphinx_mdinclude/tests/test.rst
--rw-r--r--   0        0        0    22034 2022-10-10 02:10:54.822033 sphinx_mdinclude-0.5.3/sphinx_mdinclude/tests/test_renderer.py
--rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 sphinx_mdinclude-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      180 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.flake8
+-rw-r--r--   0        0        0      207 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      139 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.github/issue_template.md
+-rw-r--r--   0        0        0       61 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.github/pull_request_template.md
+-rw-r--r--   0        0        0      682 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1091 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.gitignore
+-rw-r--r--   0        0        0       50 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.mailmap
+-rw-r--r--   0        0        0      194 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.readthedocs.yml
+-rw-r--r--   0        0        0     6845 2024-04-19 06:14:55.165367 sphinx_mdinclude-0.5.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3026 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/README.md
+-rw-r--r--   0        0        0      598 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/_static/custom.css
+-rw-r--r--   0        0        0    42080 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/_static/omnilib.png
+-rw-r--r--   0        0        0      342 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/_templates/badges.html
+-rw-r--r--   0        0        0     1145 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0       71 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/changelog.rst
+-rw-r--r--   0        0        0     2703 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/conf.py
+-rw-r--r--   0        0        0     2988 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/example.md
+-rw-r--r--   0        0        0       51 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/included.md
+-rw-r--r--   0        0        0       99 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/index.md
+-rw-r--r--   0        0        0      812 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/makefile
+-rw-r--r--   0        0        0     1806 2024-04-19 06:09:05.540177 sphinx_mdinclude-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-19 06:14:55.169367 sphinx_mdinclude-0.5.4/sphinx_mdinclude/__version__.py
+-rw-r--r--   0        0        0    15230 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/legacy.py
+-rw-r--r--   0        0        0     3514 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/parse.py
+-rw-r--r--   0        0        0     9691 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/render.py
+-rw-r--r--   0        0        0     5086 2024-04-19 05:15:04.198993 sphinx_mdinclude-0.5.4/sphinx_mdinclude/sphinx.py
+-rw-r--r--   0        0        0      280 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/__main__.py
+-rw-r--r--   0        0        0      357 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test.md
+-rw-r--r--   0        0        0      419 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test.rst
+-rw-r--r--   0        0        0    22034 2024-04-19 04:44:52.362949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test_renderer.py
+-rw-r--r--   0        0        0     2105 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test_smoke.py
+-rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 sphinx_mdinclude-0.5.4/PKG-INFO
```

### Comparing `sphinx_mdinclude-0.5.3/.gitignore` & `sphinx_mdinclude-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/CHANGELOG.md` & `sphinx_mdinclude-0.5.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 sphinx-mdinclude
 ================
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v0.5.4
+------
+
+Maintenance release
+
+- Better testing of sphinx extension and docutils directive (#48)
+- Support fixes for docutils v0.21 (#55)
+- Add support for Python 3.11 and 3.12 (#25, #39)
+- Drop support for Python 3.7 (#25)
+
+```text
+$ git shortlog -s v0.5.3...v0.5.4
+     8	Amethyst Reese
+    16	dependabot[bot]
+```
+
+
 v0.5.3
 ------
 
 Bugfix release
 
 - Fix deprecation warnings from docutils (#11)
 - Fix dependency ranges and validate compatibility
@@ -41,44 +58,44 @@
 
 Bugfix release
 
 - Fix autolinks (#3, #2)
 
 ```text
 $ git shortlog -s v0.5.0...v0.5.1
-     3	John Reese
+     3	Amethyst Reese
      2	Tim Hatch
 ```
 
 
 v0.5.0
 ------
 
 Feature release
 
 - Support for mistune 2.0 with major refactoring of codebase
 - Removal of sphinx configuration options with better defaults
 
 ```text
 $ git shortlog -s v0.5.0b1...v0.5.0
-     3	John Reese
+     3	Amethyst Reese
 ```
 
 
 v0.5.0b1
 --------
 
 Feature release
 
 - Support for mistune 2.0 with major refactoring of codebase
 - Removal of sphinx configuration options with better defaults
 
 ```text
 $ git shortlog -s v0.4.0...v0.5.0b1
-     7	John Reese
+     7	Amethyst Reese
 ```
 
 
 v0.4.0
 ------
 
 Feature release
@@ -91,15 +108,15 @@
 - Move tests into `sphinx_mdinclude` namespace
 - Pin dependencies to mistune<1.0 and docutils<0.18
 - Build using flit instead of setuptools
 - Formatted with latest black and µsort
 
 ```text
 $ git shortlog -s v0.4.0b1...v0.4.0
-     4	John Reese
+     4	Amethyst Reese
      1	dependabot[bot]
 ```
 
 
 v0.4.0b1
 --------
 
@@ -112,17 +129,17 @@
 * Move tests into `sphinx_mdinclude` namespace
 * Pin dependencies to mistune<1.0 and docutils<0.18
 * Build using flit instead of setuptools
 * Formatted with latest black and µsort
 
 ```text
 $ git shortlog -s v0.2.7...v0.4.0b1
+    18	Amethyst Reese
     10	CrossNox
      1	Ezequiel Rosas
-    18	John Reese
      1	illes
      1	kalvdans
 ```
 
 
 v0.3.1
 ------
```

### Comparing `sphinx_mdinclude-0.5.3/LICENSE` & `sphinx_mdinclude-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/README.md` & `sphinx_mdinclude-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/docs/_static/custom.css` & `sphinx_mdinclude-0.5.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/docs/_static/omnilib.png` & `sphinx_mdinclude-0.5.4/docs/_static/omnilib.png`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/docs/_templates/omnilib.html` & `sphinx_mdinclude-0.5.4/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/docs/conf.py` & `sphinx_mdinclude-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/docs/example.md` & `sphinx_mdinclude-0.5.4/docs/example.md`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/makefile` & `sphinx_mdinclude-0.5.4/makefile`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 SRCS:=sphinx_mdinclude
 
 .venv:
 	python -m venv .venv
-	source .venv/bin/activate && make setup dev
+	source .venv/bin/activate && make install
 	echo 'run `source .venv/bin/activate` to use virtualenv'
 
 venv: .venv
 
-dev:
-	flit install --symlink
-
-setup:
+install:
 	python -m pip install -U pip
-	python -m pip install -Ur requirements-dev.txt
-	python -m pip install -Ur requirements.txt
+	python -m pip install -Ue .[dev]
 
 release: lint test clean
 	flit publish
 
 format:
 	python -m ufmt format $(SRCS)
 
@@ -29,15 +25,16 @@
 	python -m coverage run -m $(SRCS).tests
 	python -m coverage report
 	python -m mypy --install-types --non-interactive -p $(SRCS)
 
 deps:
 	python -m pessimist --requirements= -c 'python -m sphinx_mdinclude.tests' .
 
+.PHONY: html
 html: .venv README.md docs/*.md docs/conf.py
-	source .venv/bin/activate && sphinx-build -b html docs html
+	source .venv/bin/activate && sphinx-build -ab html docs html
 
 clean:
 	rm -rf build dist html *.egg-info .mypy_cache
 
 distclean: clean
 	rm -rf .venv
```

### Comparing `sphinx_mdinclude-0.5.3/pyproject.toml` & `sphinx_mdinclude-0.5.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,76 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
+requires = ["flit_core >=3.8,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sphinx_mdinclude"
 authors = [
     {name = "Hiroyuki Takagi", email = "miyako.dev@gmail.com"},
     {name = "CrossNox", email = "ijmermet+m2r2@gmail.com"},
     {name = "Amethyst Reese", email = "amy@noswap.com"},
 ]
 maintainers = [
     {name = "Amethyst Reese", email = "amy@noswap.com"},
 ]
 readme = "README.md"
-requires-python = ">=3.6"
-dependencies = [
-    "mistune >=2.0,<3.0",
-    "docutils >=0.16,<1.0",
-    "pygments >= 2.8",
-]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Topic :: Text Processing",
 ]
 keywords = ["Markdown", "reStructuredText", "sphinx-extension"]
 dynamic = ["version", "description"]
+requires-python = ">=3.8"
+dependencies = [
+    "mistune >=2.0,<3.0",
+    "docutils >=0.16,<1.0",
+    "pygments >= 2.8",
+]
+
+[project.optional-dependencies]
+dev = [
+    "docutils==0.20.1; python_version < '3.9'",
+    "docutils==0.21.1; python_version >= '3.9'",
+    "mistune==2.0.4",
+
+    "attribution==1.6.2",
+    "black==24.4.0",
+    "coverage==7.3.2",
+    "flake8==7.0.0",
+    "flit==3.9.0",
+    "mypy==1.9.0",
+    "sphinx==7.1.2; python_version < '3.9'",
+    "sphinx==7.3.7; python_version >= '3.9'",
+    "ufmt==2.5.1",
+    "usort==1.0.7",
+]
 
 [project.urls]
 Github = "https://github.com/omnilib/sphinx-mdinclude"
 
 
 [tool.attribution]
 name = "sphinx-mdinclude"
 package = "sphinx_mdinclude"
 signed_tags = true
 version_file = true
+ignored_authors = ["dependabot"]
 
 [tool.coverage.run]
 branch = true
 include = ["sphinx_mdinclude/*"]
 omit = ["sphinx_mdinclude/tests/*"]
 
 [tool.coverage.report]
 fail_under = 50
 precision = 1
 show_missing = true
 skip_covered = true
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 # strict = true
 ignore_missing_imports = true
```

### Comparing `sphinx_mdinclude-0.5.3/sphinx_mdinclude/legacy.py` & `sphinx_mdinclude-0.5.4/sphinx_mdinclude/legacy.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/sphinx_mdinclude/parse.py` & `sphinx_mdinclude-0.5.4/sphinx_mdinclude/parse.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/sphinx_mdinclude/render.py` & `sphinx_mdinclude-0.5.4/sphinx_mdinclude/render.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/sphinx_mdinclude/sphinx.py` & `sphinx_mdinclude-0.5.4/sphinx_mdinclude/sphinx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Sphinx extension
 """
 
 import os
 import os.path
 
-from docutils import io, nodes, statemachine, utils
+from docutils import io, statemachine, utils
 from docutils.parsers import rst
 from docutils.parsers.rst import directives as rst_directives
 
 try:  # new
     from docutils.io import (  # type: ignore  # typeshed  #8716
         error_string as ErrorString,
     )
@@ -67,15 +67,15 @@
         source = self.state_machine.input_lines.source(
             self.lineno - self.state_machine.input_offset - 1
         )
         source_dir = os.path.dirname(os.path.abspath(source))
         path = rst_directives.path(self.arguments[0])
         path = os.path.normpath(os.path.join(source_dir, path))
         path = utils.relative_path(None, path)
-        path = nodes.reprunicode(path)
+        path = str(path)
 
         # get options (currently not use directive-specific options)
         encoding = self.options.get(
             "encoding", self.state.document.settings.input_encoding
         )
         e_handler = self.state.document.settings.input_encoding_error_handler
         tab_width = self.options.get(
```

### Comparing `sphinx_mdinclude-0.5.3/sphinx_mdinclude/tests/test_renderer.py` & `sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.3/PKG-INFO` & `sphinx_mdinclude-0.5.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: sphinx_mdinclude
-Version: 0.5.3
+Version: 0.5.4
 Summary: Markdown extension for Sphinx
 Keywords: Markdown,reStructuredText,sphinx-extension
 Author-email: Hiroyuki Takagi <miyako.dev@gmail.com>, CrossNox <ijmermet+m2r2@gmail.com>, Amethyst Reese <amy@noswap.com>
 Maintainer-email: Amethyst Reese <amy@noswap.com>
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Text Processing
 Requires-Dist: mistune >=2.0,<3.0
 Requires-Dist: docutils >=0.16,<1.0
 Requires-Dist: pygments >= 2.8
+Requires-Dist: docutils==0.20.1 ; extra == "dev" and ( python_version < '3.9')
+Requires-Dist: docutils==0.21.1 ; extra == "dev" and ( python_version >= '3.9')
+Requires-Dist: mistune==2.0.4 ; extra == "dev"
+Requires-Dist: attribution==1.6.2 ; extra == "dev"
+Requires-Dist: black==24.4.0 ; extra == "dev"
+Requires-Dist: coverage==7.3.2 ; extra == "dev"
+Requires-Dist: flake8==7.0.0 ; extra == "dev"
+Requires-Dist: flit==3.9.0 ; extra == "dev"
+Requires-Dist: mypy==1.9.0 ; extra == "dev"
+Requires-Dist: sphinx==7.1.2 ; extra == "dev" and ( python_version < '3.9')
+Requires-Dist: sphinx==7.3.7 ; extra == "dev" and ( python_version >= '3.9')
+Requires-Dist: ufmt==2.5.1 ; extra == "dev"
+Requires-Dist: usort==1.0.7 ; extra == "dev"
 Project-URL: Github, https://github.com/omnilib/sphinx-mdinclude
+Provides-Extra: dev
 
 sphinx-mdinclude
 ================
 
 Sphinx extension for including or writing pages in Markdown format.
 
 [![version](https://img.shields.io/pypi/v/sphinx-mdinclude.svg)](https://pypi.python.org/pypi/sphinx-mdinclude)
```

