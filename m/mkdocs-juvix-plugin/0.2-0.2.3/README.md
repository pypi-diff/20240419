# Comparing `tmp/mkdocs-juvix-plugin-0.2.tar.gz` & `tmp/mkdocs-juvix-plugin-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-juvix-plugin-0.2.tar", last modified: Wed Apr 17 11:48:20 2024, max compression
+gzip compressed data, was "mkdocs-juvix-plugin-0.2.3.tar", last modified: Fri Apr 19 12:50:52 2024, max compression
```

## Comparing `mkdocs-juvix-plugin-0.2.tar` & `mkdocs-juvix-plugin-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-17 11:48:20.453224 mkdocs-juvix-plugin-0.2/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      491 2024-04-17 11:48:20.452958 mkdocs-juvix-plugin-0.2/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)     2459 2024-04-17 09:44:23.000000 mkdocs-juvix-plugin-0.2/README.md
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-17 11:48:20.451431 mkdocs-juvix-plugin-0.2/mkdocs_juvix/
--rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix/__init__.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)    19264 2024-04-17 11:48:01.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix/plugin.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     3364 2024-04-17 09:42:21.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix/standalone.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     2438 2024-04-17 09:46:29.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix/utils.py
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-17 11:48:20.452627 mkdocs-juvix-plugin-0.2/mkdocs_juvix_plugin.egg-info/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      491 2024-04-17 11:48:20.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix_plugin.egg-info/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)      375 2024-04-17 11:48:20.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2024-04-17 11:48:20.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2024-04-17 11:48:20.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix_plugin.egg-info/entry_points.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       40 2024-04-17 11:48:20.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix_plugin.egg-info/requires.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2024-04-17 11:48:20.000000 mkdocs-juvix-plugin-0.2/mkdocs_juvix_plugin.egg-info/top_level.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2024-04-17 11:48:20.453281 mkdocs-juvix-plugin-0.2/setup.cfg
--rw-r--r--   0 jonaprieto   (501) staff       (20)      825 2024-04-17 11:48:07.000000 mkdocs-juvix-plugin-0.2/setup.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-19 12:50:52.627459 mkdocs-juvix-plugin-0.2.3/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      493 2024-04-19 12:50:52.627178 mkdocs-juvix-plugin-0.2.3/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     1882 2024-04-19 12:50:37.000000 mkdocs-juvix-plugin-0.2.3/README.md
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-19 12:50:52.625582 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/__init__.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)    18558 2024-04-19 12:49:33.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/plugin.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     3364 2024-04-17 09:42:21.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/standalone.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     2438 2024-04-17 09:46:29.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/utils.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-19 12:50:52.626881 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix_plugin.egg-info/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      493 2024-04-19 12:50:52.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      375 2024-04-19 12:50:52.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2024-04-19 12:50:52.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2024-04-19 12:50:52.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       40 2024-04-19 12:50:52.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix_plugin.egg-info/requires.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2024-04-19 12:50:52.000000 mkdocs-juvix-plugin-0.2.3/mkdocs_juvix_plugin.egg-info/top_level.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2024-04-19 12:50:52.627512 mkdocs-juvix-plugin-0.2.3/setup.cfg
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      827 2024-04-19 12:50:49.000000 mkdocs-juvix-plugin-0.2.3/setup.py
```

### Comparing `mkdocs-juvix-plugin-0.2/README.md` & `mkdocs-juvix-plugin-0.2.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -68,23 +68,8 @@
 you get after initializing the project using `mkdocs new myproject`.
 
 ```yaml
 # mkdocs.yaml
 ...
 plugins:
   - juvix
-
-markdown_extensions:
-  pymdownx.superfences:
-      custom_fences:
-        - name: juvix
-          class: juvix
-          format: !!python/name:juvix-mkdocs.render.render
-...
-```
-
-One minimal example of this file configured to work with this plugin can be found
-[here](https://github.com/anoma/kudos-snippets/blob/main/mkdocs.yml) and the final
-output is as [on this page](https://anoma.github.io/kudos-snippets/kudos/).
-
-To setup your GitHub CI to replicate this, you can use as template [this
-example](https://github.com/anoma/kudos-snippets/blob/main/.github/workflows/ci.yml).
+```
```

### Comparing `mkdocs-juvix-plugin-0.2/mkdocs_juvix/plugin.py` & `mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import os
 import shutil
 import subprocess
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple
 from urllib.parse import urljoin
-from mkdocs.config import base, config_options as c
+
 import pathspec
-from mkdocs import utils as mkdocs_utils
-from mkdocs.config import Config, config_options
+from mkdocs.config import config_options as c
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
 from watchdog.events import FileSystemEvent
 
 from mkdocs_juvix.utils import (
@@ -26,61 +25,63 @@
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class JuvixPlugin(BasePlugin):
 
     mkconfig: MkDocsConfig
-
     juvix_md_files: List[Dict[str, Any]]
+
     site_dir: Optional[str]
     site_url: str
     ROOT_DIR: Path
     DOCS_DIR: Path
     CACHE_DIR: Path
     MARKDOWN_JUVIX_OUTPUT: Path
 
-    JUVIX_ENABLED: bool = bool(os.environ.get("JUVIX_ENABLED", False))
+    JUVIX_ENABLED: bool = bool(os.environ.get("JUVIX_ENABLED", True))
     REMOVE_CACHE: bool = bool(os.environ.get("REMOVE_CACHE", False))
-    JUVIX_AVAILABLE: bool = True
+    JUVIX_AVAILABLE: bool
 
-    JUVIX_VERSION: Optional[str]
-    JUVIX_BIN: str = "juvix"
+    JUVIX_VERSION: Optional[str] = None
+    JUVIX_BIN: str = os.environ.get("JUVIX_BIN", "juvix")
     JUVIXCODE_CACHE_DIR: Path
     JUVIXCODE_HASH_FILE: Path
     HASH_DIR: Path
     HTML_CACHE_DIR: Path
     FIRST_RUN: bool
 
-    def create_cache_dirs(self):
-        self.MARKDOWN_JUVIX_OUTPUT.mkdir(parents=True, exist_ok=True)
-        self.JUVIXCODE_CACHE_DIR.mkdir(parents=True, exist_ok=True)
-        self.HASH_DIR.mkdir(parents=True, exist_ok=True)
-        self.HTML_CACHE_DIR.mkdir(parents=True, exist_ok=True)
-
-    def on_startup(self, command, dirty):
-        return
-
     def on_config(self, config: MkDocsConfig, **kwargs) -> MkDocsConfig:
 
         config_file = config.config_file_path
-
         self.ROOT_DIR = Path(config_file).parent.absolute()
 
-        self.DOCS_DIR: Path = self.ROOT_DIR / "docs"
-        self.CACHE_DIR: Path = self.ROOT_DIR / ".hooks"
-        self.MARKDOWN_JUVIX_OUTPUT: Path = self.CACHE_DIR / ".md"
+        self.DOCS_DIR = self.ROOT_DIR / config.get("docs_dir", "docs")
+        self.CACHE_DIR = self.ROOT_DIR / ".hooks"
+
+        if self.REMOVE_CACHE:
+            log.info("Removing Juvix Plugin cache directories.")
+            shutil.rmtree(self.CACHE_DIR, ignore_errors=True)
+
+        self.MARKDOWN_JUVIX_OUTPUT = self.CACHE_DIR / ".MD"
+        self.MARKDOWN_JUVIX_OUTPUT.mkdir(parents=True, exist_ok=True)
+
+        self.JUVIXCODE_CACHE_DIR = self.CACHE_DIR / ".JUVIX_MD"
+        self.JUVIXCODE_CACHE_DIR.mkdir(parents=True, exist_ok=True)
 
-        self.JUVIX_VERSION: Optional[str] = None
-        self.JUVIXCODE_CACHE_DIR: Path = self.CACHE_DIR / ".juvix_md"
         self.JUVIXCODE_HASH_FILE = self.CACHE_DIR / ".hash_juvix_md"
-        self.HASH_DIR: Path = self.CACHE_DIR / ".hash"
-        self.HTML_CACHE_DIR: Path = self.CACHE_DIR / ".html"
+
+        self.HTML_CACHE_DIR = self.CACHE_DIR / ".HTML"
+        self.HTML_CACHE_DIR.mkdir(parents=True, exist_ok=True)
+
         self.FIRST_RUN = True
 
+        self.HASH_DIR = self.CACHE_DIR / ".HASH"
+        self.HASH_DIR.mkdir(parents=True, exist_ok=True)
+
         self.JUVIX_AVAILABLE = shutil.which(self.JUVIX_BIN) is not None
 
         if self.JUVIX_ENABLED:
 
             if self.JUVIX_AVAILABLE:
                 cmd = [self.JUVIX_BIN, "--numeric-version"]
                 result = subprocess.run(cmd, capture_output=True)
@@ -93,51 +94,53 @@
             try:
                 subprocess.run([self.JUVIX_BIN, "--version"], capture_output=True)
             except FileNotFoundError:
                 log.warning(
                     "The Juvix binary is not available. Please install Juvix and make sure it's available in the PATH."
                 )
 
-        if self.REMOVE_CACHE:
-            shutil.rmtree(self.CACHE_DIR, ignore_errors=True)
-        self.create_cache_dirs()
-
         config = fix_site_url(config)
-
         self.mkconfig = config
+
         self.juvix_md_files: List[Dict[str, Any]] = []
+
         self.site_dir = config.get("site_dir", None)
         self.site_url = config.get("site_url", "")
 
-        if not self.site_url.endswith("/"):
-            self.site_url += "/"
-
         if not self.JUVIX_ENABLED:
             log.info("Juvix support is disabled. Set JUVIX_ENABLED to true to enable.")
+
         if not self.JUVIX_AVAILABLE:
             log.info(
                 "Juvix is not available on the system. check the JUVIX_BIN environment variable."
             )
+
         return config
 
     def on_files(self, files: Files, *, config: MkDocsConfig) -> Optional[Files]:
         for file in files:
             if ".juvix-build" in file.abs_src_path:
                 files.remove(file)
         return files
 
     def on_page_read_source(self, page: Page, config: MkDocsConfig) -> Optional[str]:
+
         filepath = Path(page.file.abs_src_path)
-        return self.generate_markdown(filepath)
 
-    def on_pre_build(self, config: MkDocsConfig) -> None:
-        self.pre_build()
+        if not filepath.as_posix().endswith(".juvix.md"):
+            return None
+
+        output = self.generate_markdown(filepath)
+        if not output:
+            log.error(f"Error generating markdown for file: {filepath}")
+
+        return output
 
     def on_post_build(self, config: MkDocsConfig) -> None:
-        self.post_build()
+        self.generate_html(generate=False, move_cache=True)
 
     def on_serve(self, server: Any, config: MkDocsConfig, builder: Any) -> None:
 
         gitignore = None
 
         with open(self.ROOT_DIR / ".gitignore") as file:
             gitignore = pathspec.PathSpec.from_lines(
@@ -172,189 +175,202 @@
             )
             .copy()
             .pop()
         )
         handler.on_any_event = callback_wrapper(handler.on_any_event)
 
     def on_page_markdown(
-        self, markdown: str, page, config, files: Files
+        self, markdown: str, page: Page, config: MkDocsConfig, files: Files
     ) -> Optional[str]:
-        juvix = ".juvix"
-        index = "index.juvix"
-        readme = "README.juvix"
-
-        def path_change(text):
-            page.file.name = page.file.name.replace(text, "")
-            page.file.url = page.file.url.replace(text, "")
-            page.file.dest_uri = page.file.dest_uri.replace(text, "")
-            page.file.abs_dest_path = page.file.abs_dest_path.replace(text, "")
-
-            if not page.title:
-                page.title = page.file.name
-
-        if page.file.name == index:
-            path_change(index)
-        elif page.file.name == readme:
-            path_change(readme)
-        elif page.file.name.endswith(juvix):
-            path_change(juvix)
+        path = page.file.abs_src_path
+
+        if not path.endswith(".juvix.md"):
+            return markdown
+
+        page.file.name = page.file.name.replace(".juvix", "")
+        page.file.url = page.file.url.replace(".juvix", "")
+        page.file.dest_uri = page.file.dest_uri.replace(".juvix", "")
+        page.file.abs_dest_path = page.file.abs_dest_path.replace(".juvix", "")
+
+        # if "vscode" in page.file.src_path:
+        # print(page.file)
+
+        # exit()
 
         return markdown
 
     def move_html_cache_to_site_dir(self, filepath: Path, site_dir: Path) -> None:
-        """
-        Move the corresponding HTML output generated by Juvix for the given Juvix
-        file to the site_dir, respecting the directory structure. It also takes into
-        account that the Juvix html generation produces .html for the .juvix.md,
-        which it is problematic, as it replaces the `juvix markdown` output, once
-        the move to site takes place.
-        """
 
-        filepath = Path(filepath)
-        if not filepath.name.endswith(".juvix.md"):
-            return
-
-        rel_path = filepath.relative_to(self.DOCS_DIR)
+        rel_to_docs = filepath.relative_to(self.DOCS_DIR)
+        if filepath.is_dir():
+            dest_folder = site_dir / rel_to_docs
+        else:
+            dest_folder = site_dir / rel_to_docs.parent
 
-        dest_folder = site_dir.joinpath(rel_path.parent)
         dest_folder.mkdir(parents=True, exist_ok=True)
 
+        # Patch: remove all the .html files in the destination folder of the
+        # Juvix Markdown file to not lose the generated HTML files in the site
+        # directory.
+
         for _file in self.JUVIXCODE_CACHE_DIR.rglob("*.juvix.md"):
             file = _file.absolute()
-            path_rel_raw = file.relative_to(self.JUVIXCODE_CACHE_DIR)
 
-            log.debug(f"move_html: file: {file}")
-            if file.suffixes == [".juvix", ".md"]:
-                filename = file.name
-
-                log.debug(f"move_html: filename: {filename}")
-                just_name = filename.replace(".juvix.md", "")
-                html_file = just_name + ".html"
-                html_file_path = self.HTML_CACHE_DIR / path_rel_raw.parent / html_file
-
-                log.debug(f"move_html: html_file: {html_file_path}")
-                if html_file_path.exists():
-                    log.debug(f"move_html: removing file {html_file_path}")
-                    html_file_path.unlink()
+            html_file_path = (
+                self.HTML_CACHE_DIR
+                / file.relative_to(self.JUVIXCODE_CACHE_DIR).parent
+                / file.name.replace(".juvix.md", ".html")
+            )
 
-        index_file = self.HTML_CACHE_DIR.joinpath("index.html")
+            if html_file_path.exists():
+                log.info(f"Removing file: {html_file_path}")
+                html_file_path.unlink()
 
+        index_file = self.HTML_CACHE_DIR / "index.html"
         if index_file.exists():
             index_file.unlink()
 
-        log.debug(f"Copying folder: {self.HTML_CACHE_DIR} to {dest_folder}")
+        # move the generated HTML files to the site directory
         shutil.copytree(self.HTML_CACHE_DIR, dest_folder, dirs_exist_ok=True)
         return
 
     def new_or_changed_or_no_exist(self, filepath: Path) -> bool:
         content_hash = hash_file(filepath)
         path_hash = compute_hash_filepath(filepath, hash_dir=self.HASH_DIR)
         if not path_hash.exists():
             log.debug(f"File: {filepath} does not have a hash file.")
             return True
         fresh_content_hash = path_hash.read_text()
         return content_hash != fresh_content_hash
 
-    # ------------------ Juvix Preprocessor ------------------
+    def on_pre_build(self, config: MkDocsConfig) -> None:
 
-    def pre_build(self) -> None:
         if self.FIRST_RUN:
             try:
                 log.info("Updating Juvix dependencies...")
                 subprocess.run(
                     [self.JUVIX_BIN, "dependencies", "update"], capture_output=True
                 )
+
             except Exception as e:
                 log.error(f"A problem occurred while updating Juvix dependencies: {e}")
                 return
 
-        log.info("Generating Markdown for all .juvix.md files.")
         for _file in self.DOCS_DIR.rglob("*.juvix.md"):
-            file: Path = _file.absolute()
 
+            file: Path = _file.absolute()
             relative_to: Path = file.relative_to(self.DOCS_DIR)
-
             url = urljoin(
                 self.site_url, relative_to.as_posix().replace(".juvix.md", ".html")
             )
-
             self.juvix_md_files.append(
                 {
                     "module_name": self.unqualified_module_name(file),
                     "qualified_module_name": self.qualified_module_name(file),
                     "url": url,
                     "file": file.absolute().as_posix(),
                 }
             )
             self.generate_markdown(file)
 
-        log.info("Computing SHA over Juvix content.")
-        current_sha: str = compute_sha_over_folder(self.JUVIXCODE_CACHE_DIR)
-
-        with open(self.JUVIXCODE_HASH_FILE, "w") as f:
-            f.write(current_sha)
-
-        if not self.FIRST_RUN:
-            return
-
-        log.info(
-            "Generating auxiliary HTML for Juvix files. This may take a while... It's only generated once per session."
-        )
-        self.generate_html(generate=True, move_cache=True)
-
         self.juvix_md_files.sort(key=lambda x: x["qualified_module_name"])
-
         juvix_modules = self.CACHE_DIR.joinpath("juvix_modules.json")
+
         if juvix_modules.exists():
             juvix_modules.unlink()
 
         with open(juvix_modules, "w") as f:
             json.dump(self.juvix_md_files, f, indent=4)
 
-        FIRST_RUN = False
+        sha_filecontent = (
+            self.JUVIXCODE_HASH_FILE.read_text()
+            if self.JUVIXCODE_HASH_FILE.exists()
+            else None
+        )
+
+        current_sha: str = compute_sha_over_folder(self.JUVIXCODE_CACHE_DIR)
+        equal_hashes = current_sha == sha_filecontent
+
+        log.info("Computed Juvix content hash: %s", current_sha)
+        if not equal_hashes:
+            log.info("Cache Juvix content hash: %s", sha_filecontent)
+        else:
+            log.info("The Juvix Markdown content has not changed.")
+
+        generate: bool = (
+            self.JUVIX_ENABLED
+            and self.JUVIX_AVAILABLE
+            and (
+                not equal_hashes
+                or (
+                    self.HTML_CACHE_DIR.exists()
+                    and (len(list(self.HTML_CACHE_DIR.glob("*"))) == 0)
+                    #     )
+                )
+            )
+        )
+
+        if not generate:
+            log.info("Skipping Juvix HTML generation for Juvix files.")
+        else:
+            log.info(
+                "Generating auxiliary HTML for Juvix files. This may take a while... It's only generated once per session."
+            )
+
+        with open(self.JUVIXCODE_HASH_FILE, "w") as f:
+            f.write(current_sha)
+
+        self.generate_html(generate=generate, move_cache=True)
+        self.FIRST_RUN = False
+        return
 
     def generate_html(self, generate: bool = True, move_cache: bool = True) -> None:
+
         everythingJuvix = self.DOCS_DIR.joinpath("everything.juvix.md")
 
         if not everythingJuvix.exists():
             log.warning(
-                "The file 'docs/everything.juvix.md' does not exist. It is recommended to create this file to avoid excessive builds."
+                f"Consider creating a file named 'everything.juvix.md' or 'index.juvix.md' in the docs directory to generate the HTML for all Juvix Markdown file. Otherwise, the HTML will be generated for each Juvix Markdown file."
             )
 
         files_to_process = (
             self.juvix_md_files
             if not everythingJuvix.exists()
             else [
                 {
                     "file": everythingJuvix,
                     "module_name": self.unqualified_module_name(everythingJuvix),
                     "qualified_module_name": self.qualified_module_name(
                         everythingJuvix
                     ),
-                    "url": urljoin(self.site_url, "everything.juvix.md").replace(
+                    "url": urljoin(self.site_url, everythingJuvix.name).replace(
                         ".juvix.md", ".html"
                     ),
                 }
             ]
         )
 
         for filepath_info in files_to_process:
             filepath = Path(filepath_info["file"])
+
             if generate:
                 self.generate_html_per_file(filepath)
             if self.site_dir and move_cache:
                 self.move_html_cache_to_site_dir(filepath, Path(self.site_dir))
+        return
 
     def generate_html_per_file(
         self, _filepath: Path, remove_cache: bool = False
     ) -> None:
 
-        if remove_cache and self.HTML_CACHE_DIR.exists():
-            log.debug(f"Removing folder: {self.HTML_CACHE_DIR}")
-            shutil.rmtree(self.HTML_CACHE_DIR)
+        if remove_cache:
+            try:
+                shutil.rmtree(self.HTML_CACHE_DIR)
+            except Exception as e:
+                log.error(f"Error removing folder: {e}")
 
         self.HTML_CACHE_DIR.mkdir(parents=True, exist_ok=True)
 
         filepath = _filepath.absolute()
 
         cmd = (
             [self.JUVIX_BIN, "html"]
@@ -373,51 +389,21 @@
             log.error(cd.stderr.decode("utf-8") + "\n\n" + "Fix the error first.")
             return
 
         # The following is necessary as this project may
         # contain assets with changes that are not reflected
         # in the generated HTML by Juvix.
 
-        good_assets = self.DOCS_DIR.joinpath("assets")
-        assets_in_html = self.HTML_CACHE_DIR.joinpath("assets")
+        good_assets = self.DOCS_DIR / "assets"
+        assets_in_html = self.HTML_CACHE_DIR / "assets"
+
         if assets_in_html.exists():
             shutil.rmtree(assets_in_html, ignore_errors=True)
 
-        shutil.copytree(
-            good_assets, self.HTML_CACHE_DIR.joinpath("assets"), dirs_exist_ok=True
-        )
-
-    def post_build(self) -> None:
-
-        log.debug("Running Juvix post_build hook.")
-
-        if not self.JUVIXCODE_CACHE_DIR.exists() or not list(
-            self.JUVIXCODE_CACHE_DIR.glob("*")
-        ):
-            return
-
-        sha_filecontent = (
-            self.JUVIXCODE_HASH_FILE.read_text()
-            if self.JUVIXCODE_HASH_FILE.exists()
-            else None
-        )
-
-        current_sha: str = compute_sha_over_folder(self.JUVIXCODE_CACHE_DIR)
-        log.debug(f"Current sha over Juvix content: {current_sha}")
-
-        equal_hashes = current_sha == sha_filecontent
-        if not equal_hashes:
-            log.info(
-                "The Juvix files have changed. You may need to rebuild the site if you include need libraries."
-            )
-
-            with open(self.JUVIXCODE_HASH_FILE, "w") as file:
-                file.write(current_sha)
-
-        self.generate_html(generate=False, move_cache=True)
+        shutil.copytree(good_assets, self.HTML_CACHE_DIR / "assets", dirs_exist_ok=True)
 
     @lru_cache(maxsize=128)
     def path_juvix_md_cache(self, _filepath: Path) -> Optional[Path]:
         filepath = _filepath.absolute()
         md_filename = filepath.name.replace(".juvix.md", ".md")
         rel_to_docs = filepath.relative_to(self.DOCS_DIR)
         cache_filepath = self.MARKDOWN_JUVIX_OUTPUT / rel_to_docs.parent / md_filename
@@ -426,16 +412,26 @@
     @lru_cache(maxsize=128)
     def read_cache(self, filepath: Path) -> Optional[str]:
         if cache_path := self.path_juvix_md_cache(filepath):
             return cache_path.read_text()
         return None
 
     def generate_markdown(self, filepath: Path) -> Optional[str]:
+        if (
+            not self.JUVIX_ENABLED
+            or not self.JUVIX_AVAILABLE
+            or not filepath.as_posix().endswith(".juvix.md")
+        ):
+            return None
+
         if self.new_or_changed_or_no_exist(filepath):
+            log.info(f"Running Juvix Markdown on file: {filepath}")
             return self.run_juvix(filepath)
+
+        log.debug(f"Reading cache for file: {filepath}")
         return self.read_cache(filepath)
 
     def unqualified_module_name(self, filepath: Path) -> Optional[str]:
         fposix: str = filepath.as_posix()
         if not fposix.endswith(".juvix.md"):
             return None
         return os.path.basename(fposix).replace(".juvix.md", "")
@@ -452,22 +448,21 @@
             return None
 
         if not root:
             return None
 
         relative_to_root = filepath.relative_to(Path(root))
 
-        # fixme use juvix dev root
-
         qualified_name = (
             relative_to_root.as_posix()
             .replace(".juvix.md", "")
             .replace("./", "")
             .replace("/", ".")
         )
+
         return qualified_name if qualified_name else None
 
     def md_filename(self, filepath: Path) -> Optional[str]:
         module_name = self.unqualified_module_name(filepath)
         return module_name + ".md" if module_name else None
 
     def run_juvix(self, _filepath: Path) -> Optional[str]:
```

### Comparing `mkdocs-juvix-plugin-0.2/mkdocs_juvix/standalone.py` & `mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/standalone.py`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2/mkdocs_juvix/utils.py` & `mkdocs-juvix-plugin-0.2.3/mkdocs_juvix/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2/setup.py` & `mkdocs-juvix-plugin-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="mkdocs-juvix-plugin",
-    version="0.2",
+    version="0.2.3",
     description="A plugin to render Juvix code blocks in MkDocs.",
     long_description="",
     keywords="mkdocs",
     author="Jonathan Prieto-Cubides, and GitHub contributors",
     author_email="jonathan@heliax.dev",
     license="MIT",
     python_requires=">=3.11",
```

