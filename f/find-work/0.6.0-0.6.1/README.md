# Comparing `tmp/find_work-0.6.0.tar.gz` & `tmp/find_work-0.6.1.tar.gz`

## Comparing `find_work-0.6.0.tar` & `find_work-0.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 find_work-0.6.0/Makefile
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/conf.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/configuration.rst
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/contributing.rst
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/getting-started.rst
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/index.rst
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/installation.rst
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/release-notes.rst
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/toc.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/_templates/git-alt.svg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/_templates/git-alt.svg.license
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/_templates/git-button.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 find_work-0.6.0/docs/_templates/git-button.html.license
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/__main__.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/cache.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/config.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/py.typed
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/types.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/utils.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/cli/__init__.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/cli/bugzilla.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/cli/execute.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/cli/pgo.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/cli/pkgcheck.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/cli/repology.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/data/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 find_work-0.6.0/find_work/data/default_config.toml
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 find_work-0.6.0/man/find-work.1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/test_bugzilla.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/test_cache.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/test_config.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/test_repology.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/cassettes/test_bugzilla/test_bugs_json_roundtrip.yaml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/data/alias_sample.toml
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/data/bug74072.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/data/bug74072.json.license
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 find_work-0.6.0/tests/data/flag_sample.toml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 find_work-0.6.0/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 find_work-0.6.0/LICENSE
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 find_work-0.6.0/README.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 find_work-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 find_work-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 find_work-0.6.1/Makefile
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/conf.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/configuration.rst
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/contributing.rst
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/getting-started.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/index.rst
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/installation.rst
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/release-notes.rst
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/toc.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-alt.svg
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-alt.svg.license
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-button.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 find_work-0.6.1/docs/_templates/git-button.html.license
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/__init__.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/__main__.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cache.py
+-rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/config.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/py.typed
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/types.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/utils.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/__init__.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/bugzilla.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/execute.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/pgo.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/pkgcheck.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/cli/repology.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/data/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 find_work-0.6.1/find_work/data/default_config.toml
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 find_work-0.6.1/man/find-work.1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_bugzilla.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_cache.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_config.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/test_repology.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/cassettes/test_bugzilla/test_bugs_json_roundtrip.yaml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/alias_sample.toml
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/bug74072.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/bug74072.json.license
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 find_work-0.6.1/tests/data/flag_sample.toml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 find_work-0.6.1/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 find_work-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 find_work-0.6.1/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 find_work-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 find_work-0.6.1/PKG-INFO
```

### Comparing `find_work-0.6.0/Makefile` & `find_work-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/docs/conf.py` & `find_work-0.6.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'find-work'
 author = 'Anna (cybertailor) Vyalkova'
 copyright = f'2024, {author}'
-release = '0.6.0'
+release = '0.6.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.extlinks',
     'sphinx.ext.intersphinx',
```

### Comparing `find_work-0.6.0/docs/configuration.rst` & `find_work-0.6.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/docs/contributing.rst` & `find_work-0.6.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/docs/getting-started.rst` & `find_work-0.6.1/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/docs/index.rst` & `find_work-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/docs/installation.rst` & `find_work-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/docs/release-notes.rst` & `find_work-0.6.1/docs/release-notes.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 .. SPDX-FileCopyrightText: 2024 Anna <cyber@sysrq.in>
 .. SPDX-License-Identifier: WTFPL
 .. No warranty.
 
 Release Notes
 =============
 
+0.6.1
+-----
+
+* [pkgcheck/scan]: drop ``--quiet`` flag. Before pkgcheck v0.10.21, this option
+  was used only in pkgcore internals. Now it's used to filter out non-error
+  results from pkgcheck.
+
 0.6.0
 -----
 
 * **New:** Define custom global flags to override global options.
 
 * **New:** Filter ``pkgcheck`` results by keyword or message.
```

### Comparing `find_work-0.6.0/docs/toc.rst` & `find_work-0.6.1/docs/toc.rst`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/docs/_templates/git-alt.svg` & `find_work-0.6.1/docs/_templates/git-alt.svg`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/__main__.py` & `find_work-0.6.1/find_work/__main__.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/cache.py` & `find_work-0.6.1/find_work/cache.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/config.py` & `find_work-0.6.1/find_work/config.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/constants.py` & `find_work-0.6.1/find_work/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """ All important constants in one place. """
 
 # Application package name.
 PACKAGE = "find-work"
 
 # Application version.
-VERSION = "0.6.0"
+VERSION = "0.6.1"
 
 # Application homepage.
 HOMEPAGE = "https://find-work.sysrq.in"
 
 # Application affiliation.
 ENTITY = "sysrq.in"
```

### Comparing `find_work-0.6.0/find_work/types.py` & `find_work-0.6.1/find_work/types.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/utils.py` & `find_work-0.6.1/find_work/utils.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/cli/__init__.py` & `find_work-0.6.1/find_work/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/cli/bugzilla.py` & `find_work-0.6.1/find_work/cli/bugzilla.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/cli/execute.py` & `find_work-0.6.1/find_work/cli/execute.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/cli/pgo.py` & `find_work-0.6.1/find_work/cli/pgo.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/cli/pkgcheck.py` & `find_work-0.6.1/find_work/cli/pkgcheck.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 def _do_scan(options: Options) -> SortedDict[str, SortedSet]:
     if options.only_installed or options.maintainer:
         pm = gentoopm.get_package_manager()
         if options.maintainer:
             repo_obj = pm.repositories[options.pkgcheck.repo]
 
     cli_opts = [
-        "--quiet",
         "--repo", options.pkgcheck.repo,
         "--scope", "pkg,ver",
         "--filter", "latest",  # TODO: become version-aware
     ]
     if options.pkgcheck.keywords:
         cli_opts += ["--keywords", ",".join(options.pkgcheck.keywords)]
```

### Comparing `find_work-0.6.0/find_work/cli/repology.py` & `find_work-0.6.1/find_work/cli/repology.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/find_work/data/default_config.toml` & `find_work-0.6.1/find_work/data/default_config.toml`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/man/find-work.1` & `find_work-0.6.1/man/find-work.1`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/tests/test_config.py` & `find_work-0.6.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/tests/test_repology.py` & `find_work-0.6.1/tests/test_repology.py`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/tests/cassettes/test_bugzilla/test_bugs_json_roundtrip.yaml` & `find_work-0.6.1/tests/cassettes/test_bugzilla/test_bugs_json_roundtrip.yaml`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/tests/data/bug74072.json` & `find_work-0.6.1/tests/data/bug74072.json`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/README.md` & `find_work-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/pyproject.toml` & `find_work-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `find_work-0.6.0/PKG-INFO` & `find_work-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: find-work
-Version: 0.6.0
+Version: 0.6.1
 Summary: Personal advice utility for Gentoo package maintainers
 Project-URL: Home, https://find-work.sysrq.in
 Project-URL: Source, https://git.sysrq.in/find-work
 Project-URL: Issues, https://bugs.sysrq.in/enter_bug.cgi?product=Software&component=find-work
 Project-URL: Changelog, https://find-work.sysrq.in/release-notes.html
 Author-email: Anna <cyber@sysrq.in>
 License-Expression: WTFPL
```

