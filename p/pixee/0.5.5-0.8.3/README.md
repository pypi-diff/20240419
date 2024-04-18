# Comparing `tmp/pixee-0.5.5.tar.gz` & `tmp/pixee-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixee-0.5.5.tar", last modified: Fri Dec 22 18:46:43 2023, max compression
+gzip compressed data, was "pixee-0.8.3.tar", last modified: Thu Apr 18 23:28:52 2024, max compression
```

## Comparing `pixee-0.5.5.tar` & `pixee-0.8.3.tar`

### file list

```diff
@@ -1,32 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:46:43.195312 pixee-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:46:43.183312 pixee-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:46:43.183312 pixee-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-22 18:46:28.000000 pixee-0.5.5/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-22 18:46:28.000000 pixee-0.5.5/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-22 18:46:28.000000 pixee-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-22 18:46:28.000000 pixee-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-22 18:46:28.000000 pixee-0.5.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-22 18:46:28.000000 pixee-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-22 18:46:28.000000 pixee-0.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    42563 2023-12-22 18:46:43.191312 pixee-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-22 18:46:28.000000 pixee-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:46:43.191312 pixee-0.5.5/img/
--rw-r--r--   0 runner    (1001) docker     (127)   246694 2023-12-22 18:46:28.000000 pixee-0.5.5/img/dark_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)  8327467 2023-12-22 18:46:28.000000 pixee-0.5.5/img/demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)   247004 2023-12-22 18:46:28.000000 pixee-0.5.5/img/light_mode_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   317595 2023-12-22 18:46:28.000000 pixee-0.5.5/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-22 18:46:28.000000 pixee-0.5.5/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-22 18:46:28.000000 pixee-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 18:46:43.195312 pixee-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:46:43.183312 pixee-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:46:43.191312 pixee-0.5.5/src/pixee/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-22 18:46:43.000000 pixee-0.5.5/src/pixee/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2023-12-22 18:46:28.000000 pixee-0.5.5/src/pixee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-12-22 18:46:28.000000 pixee-0.5.5/src/pixee/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 18:46:43.191312 pixee-0.5.5/src/pixee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42563 2023-12-22 18:46:43.000000 pixee-0.5.5/src/pixee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-22 18:46:43.000000 pixee-0.5.5/src/pixee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 18:46:43.000000 pixee-0.5.5/src/pixee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 18:46:43.000000 pixee-0.5.5/src/pixee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-12-22 18:46:43.000000 pixee-0.5.5/src/pixee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 18:46:43.000000 pixee-0.5.5/src/pixee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.969562 pixee-0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.949561 pixee-0.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.953561 pixee-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-18 23:28:41.000000 pixee-0.8.3/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-18 23:28:41.000000 pixee-0.8.3/.github/workflows/docker_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-18 23:28:41.000000 pixee-0.8.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 23:28:41.000000 pixee-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-18 23:28:41.000000 pixee-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 23:28:41.000000 pixee-0.8.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-18 23:28:41.000000 pixee-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 23:28:41.000000 pixee-0.8.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    42801 2024-04-18 23:28:52.969562 pixee-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-18 23:28:41.000000 pixee-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.953561 pixee-0.8.3/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.949561 pixee-0.8.3/ci/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.953561 pixee-0.8.3/ci/assets/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)   173449 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/assets/bitbucket/access_token_var.png
+-rw-r--r--   0 runner    (1001) docker     (127)   421324 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/assets/bitbucket/access_token_view.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66021 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/assets/bitbucket/access_tokens.png
+-rw-r--r--   0 runner    (1001) docker     (127)   164443 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/assets/bitbucket/scopes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74125 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/assets/bitbucket/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41727 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/assets/bitbucket/variables.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.953561 pixee-0.8.3/ci/bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/bitbucket/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/bitbucket/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/bitbucket/bitbucket-pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/bitbucket/bitbucket_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/bitbucket/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      417 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/bitbucket/pipe.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.957562 pixee-0.8.3/ci/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/examples/.gitlab-ci.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.957562 pixee-0.8.3/ci/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/gitlab/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/gitlab/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 23:28:41.000000 pixee-0.8.3/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.957562 pixee-0.8.3/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-18 23:28:41.000000 pixee-0.8.3/docker/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.957562 pixee-0.8.3/docker/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-18 23:28:41.000000 pixee-0.8.3/docker/bin/pixee-java-codemods
+-rwxr-xr-x   0 runner    (1001) docker     (127)       52 2024-04-18 23:28:41.000000 pixee-0.8.3/docker/bin/pixee-python-codemods
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.965562 pixee-0.8.3/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   246694 2024-04-18 23:28:41.000000 pixee-0.8.3/img/dark_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  8327467 2024-04-18 23:28:41.000000 pixee-0.8.3/img/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   247004 2024-04-18 23:28:41.000000 pixee-0.8.3/img/light_mode_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   317595 2024-04-18 23:28:41.000000 pixee-0.8.3/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 23:28:41.000000 pixee-0.8.3/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-18 23:28:41.000000 pixee-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-18 23:28:41.000000 pixee-0.8.3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 23:28:52.969562 pixee-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.949561 pixee-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.969562 pixee-0.8.3/src/pixee/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 23:28:52.000000 pixee-0.8.3/src/pixee/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14753 2024-04-18 23:28:41.000000 pixee-0.8.3/src/pixee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-18 23:28:41.000000 pixee-0.8.3/src/pixee/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:28:52.969562 pixee-0.8.3/src/pixee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42801 2024-04-18 23:28:52.000000 pixee-0.8.3/src/pixee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 23:28:52.000000 pixee-0.8.3/src/pixee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 23:28:52.000000 pixee-0.8.3/src/pixee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 23:28:52.000000 pixee-0.8.3/src/pixee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 23:28:52.000000 pixee-0.8.3/src/pixee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 23:28:52.000000 pixee-0.8.3/src/pixee.egg-info/top_level.txt
```

### Comparing `pixee-0.5.5/.github/workflows/deploy_to_pypi.yml` & `pixee-0.8.3/.github/workflows/deploy_to_pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   push:
     tags:
       - "[0-9]+.[0-9]+.[0-9]+"
 
 jobs:
   build-and-release:
     name: Build and Release
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     timeout-minutes: 5
     steps:
       - name: Set Up Python
         uses: actions/setup-python@v5
         with:
           python-version: '3.12'
       - name: Check out code
```

### Comparing `pixee-0.5.5/.github/workflows/lint.yml` & `pixee-0.8.3/.github/workflows/lint.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 concurrency:
   group: (${{ github.workflow }}-${{ github.event.inputs.branch || github.event.pull_request.head.ref }})
   cancel-in-progress: true
 
 jobs:
   linting:
     name: Pylint Checks
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     timeout-minutes: 5
     steps:
       - name: Set Up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.11'
       - name: Check out code
         uses: actions/checkout@v4
       - name: Install Package
         run: pip install .
       - name: Install Dependencies
@@ -34,9 +34,9 @@
       - name: Run pylint
         run: make lint
 
   pre-commit:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
     - uses: pre-commit/action@v3.0.0
```

### Comparing `pixee-0.5.5/LICENSE` & `pixee-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pixee-0.5.5/PKG-INFO` & `pixee-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.5.5
+Version: 0.8.3
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -665,15 +665,15 @@
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://pixee.ai
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: codemodder
+Requires-Dist: codemodder==0.91.0
 Requires-Dist: click
 Requires-Dist: prompt-toolkit
 Requires-Dist: questionary~=2.0.0
 Requires-Dist: security~=1.2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
@@ -712,23 +712,29 @@
 ```
 brew tap pixee/pixee
 brew install pixee
 ```
 
 ## Usage
 
-After installation, run the `pixee` command to see instructions and options.
+After installation, you can run the `pixee` command to see instructions and options. 
+
+To simply scan some code and see possible changes to make:
+
+```
+pixee fix /my/project/directory/
+```
 
 ## F.A.Q.
 
 ### What languages are supported for fixes?
 Currently we support codemods for Java and Python. Stay tuned for additional language support at https://pixee.ai!
 
 ### What happens to my code?
-The Pixee CLI currently runs most detection and fixes locally to your own host machine. Any features that require network access to a third-party service (e.g. OpenAI) will require explicit opt-in. We promise to be transparent when this is the case.
+The Pixee CLI currently runs most detection and fixes locally to your own host machine. Any features that require network access to a third-party service (e.g. OpenAI) will require explicit opt-in. We promise to be transparent when this is the case. **Your code will not leave your host machine unless you explicitly opt-in to a feature that requires network access.**
 
 ### How can I install the GitHub application?
 Get the most out of Pixee by installing the Pixeebot GitHub app at https://app.pixee.ai. Or find us on [GitHub Marketplace](https://github.com/apps/pixeebot).
 
 ### Where can I request features and report issues?
 For CLI feature requests and bug reports please use our GitHub issue tracker: https://github.com/pixee/pixee-cli/issues
```

### Comparing `pixee-0.5.5/README.md` & `pixee-0.8.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -28,23 +28,29 @@
 ```
 brew tap pixee/pixee
 brew install pixee
 ```
 
 ## Usage
 
-After installation, run the `pixee` command to see instructions and options.
+After installation, you can run the `pixee` command to see instructions and options. 
+
+To simply scan some code and see possible changes to make:
+
+```
+pixee fix /my/project/directory/
+```
 
 ## F.A.Q.
 
 ### What languages are supported for fixes?
 Currently we support codemods for Java and Python. Stay tuned for additional language support at https://pixee.ai!
 
 ### What happens to my code?
-The Pixee CLI currently runs most detection and fixes locally to your own host machine. Any features that require network access to a third-party service (e.g. OpenAI) will require explicit opt-in. We promise to be transparent when this is the case.
+The Pixee CLI currently runs most detection and fixes locally to your own host machine. Any features that require network access to a third-party service (e.g. OpenAI) will require explicit opt-in. We promise to be transparent when this is the case. **Your code will not leave your host machine unless you explicitly opt-in to a feature that requires network access.**
 
 ### How can I install the GitHub application?
 Get the most out of Pixee by installing the Pixeebot GitHub app at https://app.pixee.ai. Or find us on [GitHub Marketplace](https://github.com/apps/pixeebot).
 
 ### Where can I request features and report issues?
 For CLI feature requests and bug reports please use our GitHub issue tracker: https://github.com/pixee/pixee-cli/issues
```

### Comparing `pixee-0.5.5/img/dark_mode_logo.png` & `pixee-0.8.3/img/dark_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.5.5/img/demo.gif` & `pixee-0.8.3/img/demo.gif`

 * *Files identical despite different names*

### Comparing `pixee-0.5.5/img/light_mode_logo.png` & `pixee-0.8.3/img/light_mode_logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.5.5/img/logo.png` & `pixee-0.8.3/img/logo.png`

 * *Files identical despite different names*

### Comparing `pixee-0.5.5/pylintrc` & `pixee-0.8.3/pylintrc`

 * *Files identical despite different names*

### Comparing `pixee-0.5.5/pyproject.toml` & `pixee-0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 name = "pixee"
 requires-python = ">=3.10.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "Pixee CLI"
 dependencies = [
-    "codemodder",
+    "codemodder==0.91.0",
     "click",
     "prompt-toolkit",
     "questionary~=2.0.0",
     "security~=1.2.0",
 ]
 
 [project.urls]
```

### Comparing `pixee-0.5.5/src/pixee/cli.py` & `pixee-0.8.3/src/pixee/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,20 +342,15 @@
             console.print(Markdown(description))
             prompt("Press Enter to see the updated files")
             for entry in result["changeset"]:
                 console.print(f"File: {entry['path']}", style="bold")
                 console.print(Markdown(f"```diff\n{entry['diff']}```"))
             prompt("Press Enter to continue...")
 
-    result_file = Path(output or DEFAULT_CODETF_PATH)
-
-    Path(result_file).write_text(json.dumps(combined_codetf, indent=2))
-    console.print(f"Results written to {result_file}", style="bold")
-
-    summarize_results(combined_codetf)
+    summarize_results(combined_codetf, output, saved_to_file=True)
 
 
 @main.command()
 @click.argument("path", nargs=1, required=False, type=click.Path(exists=True))
 def explain(path):
     """
     Interactively explain codemodder results (use after fix)
@@ -380,14 +375,18 @@
 
     results = [
         result for result in combined_codetf["results"] if len(result["changeset"])
     ]
 
     console.print(f"Reading results from `{result_file}`", style="bold")
     summarize_results(combined_codetf)
+
+    if not results:
+        return 0
+
     if (
         codemod := select(
             "Which codemod result would you like to explain?",
             choices=[result["codemod"] for result in results],
         ).ask()
     ) is None:
         return 0
@@ -411,22 +410,27 @@
     entry = next(entry for entry in result["changeset"] if entry["path"] == filename)
     console.print(f"\n\nFile: {entry['path']}", style="bold")
     console.print(Markdown(f"```diff\n{entry['diff']}```"))
 
     return 0
 
 
-def summarize_results(combined_codetf):
+def summarize_results(combined_codetf, output=None, saved_to_file=False):
     results = [
         result for result in combined_codetf["results"] if len(result["changeset"])
     ]
     if not len(results):
         console.print("No changes applied", style="bold")
         return
 
+    if saved_to_file and results:
+        result_file = Path(output or DEFAULT_CODETF_PATH)
+        Path(result_file).write_text(json.dumps(combined_codetf, indent=2))
+        console.print(f"Results written to {result_file}", style="bold")
+
     console.print(
         f"Found {len(results)} opportunities to harden and improve your code:",
         style="bold",
     )
     table = Table(show_header=True, header_style="bold")
     table.add_column("Codemod", style="dim")
     table.add_column("Summary", style="bold")
```

### Comparing `pixee-0.5.5/src/pixee/logo.py` & `pixee-0.8.3/src/pixee/logo.py`

 * *Files identical despite different names*

### Comparing `pixee-0.5.5/src/pixee.egg-info/PKG-INFO` & `pixee-0.8.3/src/pixee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixee
-Version: 0.5.5
+Version: 0.8.3
 Summary: Pixee CLI
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -665,15 +665,15 @@
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://pixee.ai
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: codemodder
+Requires-Dist: codemodder==0.91.0
 Requires-Dist: click
 Requires-Dist: prompt-toolkit
 Requires-Dist: questionary~=2.0.0
 Requires-Dist: security~=1.2.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
@@ -712,23 +712,29 @@
 ```
 brew tap pixee/pixee
 brew install pixee
 ```
 
 ## Usage
 
-After installation, run the `pixee` command to see instructions and options.
+After installation, you can run the `pixee` command to see instructions and options. 
+
+To simply scan some code and see possible changes to make:
+
+```
+pixee fix /my/project/directory/
+```
 
 ## F.A.Q.
 
 ### What languages are supported for fixes?
 Currently we support codemods for Java and Python. Stay tuned for additional language support at https://pixee.ai!
 
 ### What happens to my code?
-The Pixee CLI currently runs most detection and fixes locally to your own host machine. Any features that require network access to a third-party service (e.g. OpenAI) will require explicit opt-in. We promise to be transparent when this is the case.
+The Pixee CLI currently runs most detection and fixes locally to your own host machine. Any features that require network access to a third-party service (e.g. OpenAI) will require explicit opt-in. We promise to be transparent when this is the case. **Your code will not leave your host machine unless you explicitly opt-in to a feature that requires network access.**
 
 ### How can I install the GitHub application?
 Get the most out of Pixee by installing the Pixeebot GitHub app at https://app.pixee.ai. Or find us on [GitHub Marketplace](https://github.com/apps/pixeebot).
 
 ### Where can I request features and report issues?
 For CLI feature requests and bug reports please use our GitHub issue tracker: https://github.com/pixee/pixee-cli/issues
```

