# Comparing `tmp/slpkg-5.0.5.tar.gz` & `tmp/slpkg-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slpkg-5.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "slpkg-5.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `slpkg-5.0.5.tar` & `slpkg-5.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1945 2024-04-12 18:29:54.000000 slpkg-5.0.5/README.md
--rw-r--r--   0        0        0     1694 2024-04-12 18:29:54.000000 slpkg-5.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/binaries/__init__.py
--rw-r--r--   0        0        0     8384 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/binaries/install.py
--rw-r--r--   0        0        0     2252 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/binaries/required.py
--rw-r--r--   0        0        0      985 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/blacklist.py
--rw-r--r--   0        0        0     6418 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/check_updates.py
--rw-r--r--   0        0        0     1273 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/checks.py
--rw-r--r--   0        0        0     1404 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/checksum.py
--rw-r--r--   0        0        0     4184 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/choose_packages.py
--rw-r--r--   0        0        0      845 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/cleanings.py
--rw-r--r--   0        0        0     5550 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/configs.py
--rw-r--r--   0        0        0     3725 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/dependees.py
--rw-r--r--   0        0        0     1944 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/dialog_box.py
--rw-r--r--   0        0        0     5059 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/dialog_configs.py
--rw-r--r--   0        0        0     4144 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/download_only.py
--rw-r--r--   0        0        0     3992 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/downloader.py
--rw-r--r--   0        0        0      430 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/error_messages.py
--rw-r--r--   0        0        0     1738 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/find_installed.py
--rw-r--r--   0        0        0     1328 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/gpg_verify.py
--rw-r--r--   0        0        0    75013 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/install_data.py
--rw-r--r--   0        0        0     3719 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/load_data.py
--rw-r--r--   0        0        0    27384 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/main.py
--rw-r--r--   0        0        0     6253 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/multi_process.py
--rw-r--r--   0        0        0    11270 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/new_configs.py
--rw-r--r--   0        0        0     2661 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/progress_bar.py
--rw-r--r--   0        0        0     5679 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/remove_packages.py
--rw-r--r--   0        0        0     4552 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/repo_info.py
--rw-r--r--   0        0        0    27277 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/repositories.py
--rw-r--r--   0        0        0        0 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/sbos/__init__.py
--rw-r--r--   0        0        0     1075 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/sbos/dependencies.py
--rw-r--r--   0        0        0     4561 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/sbos/sbo_generate.py
--rw-r--r--   0        0        0    11449 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/sbos/slackbuild.py
--rw-r--r--   0        0        0     3119 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/search.py
--rw-r--r--   0        0        0      587 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/toml_errors.py
--rw-r--r--   0        0        0     4391 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/tracking.py
--rw-r--r--   0        0        0     6297 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/update_repositories.py
--rw-r--r--   0        0        0    10344 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/upgrade.py
--rw-r--r--   0        0        0     7760 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/utilities.py
--rw-r--r--   0        0        0        0 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/views/__init__.py
--rw-r--r--   0        0        0     5768 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/views/asciibox.py
--rw-r--r--   0        0        0     6265 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/views/cli_menu.py
--rw-r--r--   0        0        0      740 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/views/version.py
--rw-r--r--   0        0        0     6932 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/views/view_package.py
--rw-r--r--   0        0        0     9950 2024-04-12 18:29:54.000000 slpkg-5.0.5/slpkg/views/views.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1945 2024-04-19 17:35:54.000000 slpkg-5.0.6/README.md
+-rw-r--r--   0        0        0     1694 2024-04-19 17:35:54.000000 slpkg-5.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/binaries/__init__.py
+-rw-r--r--   0        0        0     9302 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/binaries/install.py
+-rw-r--r--   0        0        0     2084 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/binaries/required.py
+-rw-r--r--   0        0        0     1074 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/blacklist.py
+-rw-r--r--   0        0        0     6492 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/check_updates.py
+-rw-r--r--   0        0        0     1273 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/checks.py
+-rw-r--r--   0        0        0     1404 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/checksum.py
+-rw-r--r--   0        0        0     4184 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/choose_packages.py
+-rw-r--r--   0        0        0      845 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/cleanings.py
+-rw-r--r--   0        0        0     5679 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/configs.py
+-rw-r--r--   0        0        0     3725 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/dependees.py
+-rw-r--r--   0        0        0     1944 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/dialog_box.py
+-rw-r--r--   0        0        0     5138 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/dialog_configs.py
+-rw-r--r--   0        0        0     4144 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/download_only.py
+-rw-r--r--   0        0        0     3992 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/downloader.py
+-rw-r--r--   0        0        0      430 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/error_messages.py
+-rw-r--r--   0        0        0     1738 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/find_installed.py
+-rw-r--r--   0        0        0     1328 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/gpg_verify.py
+-rw-r--r--   0        0        0    10735 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/install_data.py
+-rw-r--r--   0        0        0     4723 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/load_data.py
+-rw-r--r--   0        0        0    27957 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/main.py
+-rw-r--r--   0        0        0     6253 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/multi_process.py
+-rw-r--r--   0        0        0    11270 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/new_configs.py
+-rw-r--r--   0        0        0     2661 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/progress_bar.py
+-rw-r--r--   0        0        0     5685 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/remove_packages.py
+-rw-r--r--   0        0        0     4816 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/repo_info.py
+-rw-r--r--   0        0        0    17927 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/repositories.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/dependencies.py
+-rw-r--r--   0        0        0     4561 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0        0        0    12368 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/sbos/slackbuild.py
+-rw-r--r--   0        0        0     3119 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/search.py
+-rw-r--r--   0        0        0      587 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/toml_errors.py
+-rw-r--r--   0        0        0     4391 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/tracking.py
+-rw-r--r--   0        0        0     4557 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/update_repositories.py
+-rw-r--r--   0        0        0    10748 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/upgrade.py
+-rw-r--r--   0        0        0     8049 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/__init__.py
+-rw-r--r--   0        0        0     5768 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/asciibox.py
+-rw-r--r--   0        0        0     6265 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/cli_menu.py
+-rw-r--r--   0        0        0      740 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/version.py
+-rw-r--r--   0        0        0     6932 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/view_package.py
+-rw-r--r--   0        0        0     9950 2024-04-19 17:35:54.000000 slpkg-5.0.6/slpkg/views/views.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.6/PKG-INFO
```

### Comparing `slpkg-5.0.5/README.md` & `slpkg-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/pyproject.toml` & `slpkg-5.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "slpkg"
-version = "5.0.5"
+version = "5.0.6"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 maintainers = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Package manager utility for Slackware Linux"
```

### Comparing `slpkg-5.0.5/slpkg/binaries/install.py` & `slpkg-5.0.6/slpkg/binaries/install.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 # -*- coding: utf-8 -*-
 
 import os
 import time
 import json
 from pathlib import Path
 from collections import OrderedDict
+from multiprocessing import Process
 
 from slpkg.upgrade import Upgrade
 from slpkg.configs import Configs
 from slpkg.checksum import Md5sum
 from slpkg.views.views import View
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.gpg_verify import GPGVerify
 from slpkg.downloader import Downloader
 from slpkg.views.asciibox import AsciiBox
+from slpkg.progress_bar import ProgressBar
 from slpkg.multi_process import MultiProcess
 from slpkg.binaries.required import Required
 
 
 class Packages(Configs):
 
     def __init__(self, repository: str, data: dict, packages: list, flags: list, mode: str):
@@ -35,36 +37,41 @@
         self.multi_proc = MultiProcess(flags)
         self.view = View(flags, repository, data)
         self.check_md5 = Md5sum(flags)
         self.download = Downloader(flags)
         self.upgrade = Upgrade(repository, data)
         self.ascii = AsciiBox()
         self.gpg = GPGVerify()
+        self.progress = ProgressBar()
 
         self.dependencies: list = []
         self.install_order: list = []
         self.binary_packages: list = []
         self.skipped_packages: list = []
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
+        self.bar_process = None
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ('-k', '--skip-installed'), flags)
 
+        self.option_for_progress_bar: bool = self.utils.is_option(
+            ('-B', '--progress-bar'), flags)
+
         self.packages: list = self.utils.apply_package_pattern(data, packages)
 
     def execute(self) -> None:
+        self.bar_progress()
         self.creating_dependencies_list()
         self.choose_package_dependencies()
         self.add_dependencies_to_install_order()
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
-
         self.check_for_skipped()
 
         self.view.install_upgrade_packages(self.packages, self.dependencies, self.mode)
         self.view.question()
 
         start: float = time.time()
         self.view.skipping_packages(self.skipped_packages)
@@ -73,23 +80,21 @@
         self.set_progress_message()
         self.install_packages()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
-        print('\rResolving dependencies... ', end='')
         for package in self.packages:
             dependencies: tuple = Required(self.data, package, self.flags).resolve()
 
             for dependency in dependencies:
                 self.dependencies.append(dependency)
 
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
-        print(f'{self.bgreen}{self.ascii.done}{self.endc}')
 
     def add_dependencies_to_install_order(self) -> None:
         self.install_order.extend(self.dependencies)
 
     def clean_the_main_slackbuilds(self) -> None:
         for dependency in self.dependencies:
             if dependency in self.packages:
@@ -205,11 +210,32 @@
                     status: bool = True
 
                 if self.option_for_reinstall:
                     status: bool = True
 
                 choices.extend([(package, repo_ver, status, help_text)])
 
+            self.done_process()
+
             text: str = f'There are {len(choices)} dependencies:'
             code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
 
             os.system('clear')
+        else:
+            self.done_process()
+
+    def bar_progress(self) -> None:
+        if self.progress_bar or self.option_for_progress_bar:
+            message: str = 'Resolving dependencies'
+            self.bar_process = Process(target=self.progress.progress_bar, args=(message,))
+            self.bar_process.start()
+        else:
+            print('\rResolving dependencies... ', end='')
+
+    def done_process(self) -> None:
+        if self.progress_bar or self.option_for_progress_bar:
+            time.sleep(0.1)
+            self.bar_process.terminate()
+            self.bar_process.join()
+            print('\x1b[?25h')
+        else:
+            print(f'{self.bgreen}{self.ascii.done}{self.endc}')
```

### Comparing `slpkg-5.0.5/slpkg/check_updates.py` & `slpkg-5.0.6/slpkg/check_updates.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,28 +41,25 @@
             ('-c', '--check'), flags)
 
         self.option_for_progress_bar: bool = self.utils.is_option(
             ('-B', '--progress-bar'), flags)
 
     def check_the_repositories(self, queue=None) -> None:
         if self.option_for_repository:
-            self.repositories(self.repository)
+            self.save_the_compares(self.repository)
         else:
-            self.check_updates_for_repositories()
+            for repo, enable in self.repos.repositories.items():
+                if enable['enable']:
+                    self.save_the_compares(repo)
 
         if queue is not None:
             queue.put(self.compare)
             queue.put(self.error_connected)
 
-    def check_updates_for_repositories(self) -> None:
-        for repo, enable in self.repos.repositories.items():
-            if enable['enable']:
-                self.repositories(repo)
-
-    def repositories(self, repo: str) -> None:
+    def save_the_compares(self, repo: str) -> None:
         local_chg_txt: Path = Path(self.repos.repositories[repo]['path'],
                                    self.repos.repositories[repo]['changelog_txt'])
         repo_chg_txt: str = (f"{self.repos.repositories[repo]['mirror_changelog']}"
                              f"{self.repos.repositories[repo]['changelog_txt']}")
         repo_data_file: Path = Path(self.repos.repositories[repo]['path'],
                                     self.repos.data_json)
 
@@ -97,15 +94,15 @@
             self.error_connected.append(repo_chg_txt)
 
         if repo_size == 0:
             return False
 
         return local_size != repo_size
 
-    def error_connected_repositories(self) -> None:
+    def check_for_error_connected(self) -> None:
         if self.error_connected:
             print(f'\n{self.endc}Failed connected to the mirrors:\n')
             for repo in self.error_connected:
                 print(f'{self.red}>{self.endc} {repo}')
 
     def set_http_proxy_server(self) -> None:
         self.http = ProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
@@ -121,22 +118,27 @@
     def view_messages(self) -> None:
         repo_for_update: list = []
         for repo, comp in self.compare.items():
             if comp:
                 repo_for_update.append(repo)
 
         if repo_for_update:
-            last_updates: dict = self.repo_info.read_last_updated()
+            last_updates: dict = self.repo_info.repo_information()
             print(f"\n{self.bgreen}There are new updates available for the "
                   f"repositories:{self.endc}\n")
 
             for repo in repo_for_update:
                 repo_length: int = max(len(name) for name in repo_for_update)
+
+                last_updated: str = 'None'
+                if last_updates.get(repo):
+                    last_updated: str = last_updates[repo].get('last_updated', 'None')
+
                 print(f'> {self.bgreen}{repo:<{repo_length}}{self.endc} Last Updated: '
-                      f"'{last_updates.get(repo, None)}'")
+                      f"'{last_updated}'")
             if not self.option_for_check:
                 print()
         else:
             print(f'\n{self.endc}{self.yellow}No updated packages since the last check.{self.endc}')
 
         if self.option_for_check:
             print()
@@ -165,10 +167,10 @@
 
             print('\x1b[?25h')
         else:
             print(f'\r{message}... ', end='')
             self.check_the_repositories()
             print()
 
-        self.error_connected_repositories()
+        self.check_for_error_connected()
         self.view_messages()
         return self.compare
```

### Comparing `slpkg-5.0.5/slpkg/checks.py` & `slpkg-5.0.6/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/checksum.py` & `slpkg-5.0.6/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/choose_packages.py` & `slpkg-5.0.6/slpkg/choose_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/cleanings.py` & `slpkg-5.0.6/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/configs.py` & `slpkg-5.0.6/slpkg/configs.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,54 +69,55 @@
     proxy_password: str = ''
 
     try:
         # Load user configuration.
         config_path_file = Path(etc_path, f'{prog_name}.toml')
         if config_path_file.exists():
             with open(config_path_file, 'rb') as conf:
-                configs = tomli.load(conf)
+                configs = {k.lower(): v for k, v in tomli.load(conf).items()}
 
         if configs:
-            config = configs['CONFIGS']
+            config = {k.lower(): v for k, v in configs['configs'].items()}
 
-            os_arch: str = config['OS_ARCH']
-            download_only_path: Path = Path(config['DOWNLOAD_ONLY_PATH'])
-            ask_question: bool = config['ASK_QUESTION']
-            installpkg: str = config['INSTALLPKG']
-            reinstall: str = config['REINSTALL']
-            removepkg: str = config['REMOVEPKG']
-            colors: bool = config['COLORS']
-            makeflags: str = config['MAKEFLAGS']
-            gpg_verification: bool = config['GPG_VERIFICATION']
-            checksum_md5: bool = config['CHECKSUM_MD5']
-            dialog: bool = config['DIALOG']
-            new_packages: bool = config['NEW_PACKAGES']
-            removed_packages: bool = config['REMOVED_PACKAGES']
-            downloader: str = config['DOWNLOADER']
-            wget_options: str = config['WGET_OPTIONS']
-            curl_options: str = config['CURL_OPTIONS']
-            lftp_get_options: str = config['LFTP_GET_OPTIONS']
-            lftp_mirror_options: str = config['LFTP_MIRROR_OPTIONS']
-            ascii_characters: bool = config['ASCII_CHARACTERS']
-            file_list_suffix: str = config['FILE_LIST_SUFFIX']
-            parallel_downloads: bool = config['PARALLEL_DOWNLOADS']
-            maximum_parallel: int = config['MAXIMUM_PARALLEL']
-            progress_bar: bool = config['PROGRESS_BAR']
-            progress_spinner: str = config['PROGRESS_SPINNER']
-            spinner_color: str = config['SPINNER_COLOR']
-            border_color: str = config['BORDER_COLOR']
-            process_log: bool = config['PROCESS_LOG']
-
-            urllib_retries: Any = config['URLLIB_RETRIES']
-            urllib_redirect: Any = config['URLLIB_REDIRECT']
-            urllib_timeout: float = config['URLLIB_TIMEOUT']
-
-            proxy_address: str = config['PROXY_ADDRESS']
-            proxy_username: str = config['PROXY_USERNAME']
-            proxy_password: str = config['PROXY_PASSWORD']
+            os_arch: str = config['os_arch']
+            download_only_path: Path = Path(config['download_only_path'])
+            ask_question: bool = config['ask_question']
+            kernel_version: str = config['kernel_version']
+            installpkg: str = config['installpkg']
+            reinstall: str = config['reinstall']
+            removepkg: str = config['removepkg']
+            colors: bool = config['colors']
+            makeflags: str = config['makeflags']
+            gpg_verification: bool = config['gpg_verification']
+            checksum_md5: bool = config['checksum_md5']
+            dialog: bool = config['dialog']
+            new_packages: bool = config['new_packages']
+            removed_packages: bool = config['removed_packages']
+            downloader: str = config['downloader']
+            wget_options: str = config['wget_options']
+            curl_options: str = config['curl_options']
+            lftp_get_options: str = config['lftp_get_options']
+            lftp_mirror_options: str = config['lftp_mirror_options']
+            ascii_characters: bool = config['ascii_characters']
+            file_list_suffix: str = config['file_list_suffix']
+            parallel_downloads: bool = config['parallel_downloads']
+            maximum_parallel: int = config['maximum_parallel']
+            progress_bar: bool = config['progress_bar']
+            progress_spinner: str = config['progress_spinner']
+            spinner_color: str = config['spinner_color']
+            border_color: str = config['border_color']
+            process_log: bool = config['process_log']
+
+            urllib_retries: Any = config['urllib_retries']
+            urllib_redirect: Any = config['urllib_redirect']
+            urllib_timeout: float = config['urllib_timeout']
+
+            proxy_address: str = config['proxy_address']
+            proxy_username: str = config['proxy_username']
+            proxy_password: str = config['proxy_password']
 
     except (KeyError, tomli.TOMLDecodeError) as error:
         toml_errors.raise_toml_error_message(error, toml_file='/etc/slpkg/slpkg.toml')
 
     blink: str = ''
     bold: str = ''
     red: str = ''
```

### Comparing `slpkg-5.0.5/slpkg/dependees.py` & `slpkg-5.0.6/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/dialog_box.py` & `slpkg-5.0.6/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/dialog_configs.py` & `slpkg-5.0.6/slpkg/dialog_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         height: int = 9
         width: int = 0
         form_height: int = 0
         text: str = f'Edit the configuration file: {self.config_file}'
         title: str = ' Configuration File '
 
         # Creating the elements for the dialog form.
-        for i, (key, value) in enumerate(self.configs['CONFIGS'].items(), start=1):
+        for i, (key, value) in enumerate(self.configs['configs'].items(), start=1):
             if value is True:
                 value: str = 'true'
             elif value is False:
                 value: str = 'false'
             elements.extend(
                 [(key, i, 1, str(value), i, 21, 47, 200, '0x0', f'Config: {key} = {value}')]
             )
@@ -72,29 +72,30 @@
         """ Check for true of false values. """
         keys: list = [
             'COLORS',
             'DIALOG',
             'SILENT_MODE',
             'ASCII_CHARACTERS',
             'ASK_QUESTION',
+            'KERNEL_VERSION',
             'PARALLEL_DOWNLOADS',
             'PROGRESS_BAR',
             'SPINNING_BAR',
             'CASE_INSENSITIVE',
             'PROCESS_LOG',
             'URLLIB_RETRIES',
             'URLLIB_REDIRECT',
             'GPG_VERIFICATION',
             'CHECKSUM_MD5',
             'NEW_PACKAGES',
             'REMOVED_PACKAGES'
         ]
         values: list = ['true', 'false']
 
-        for key, value in zip(self.configs['CONFIGS'].keys(), tags):
+        for key, value in zip(self.configs['configs'].keys(), tags):
 
             if key in keys and value not in values:
                 self.dialogbox.msgbox(f"\nError: Value for '{key}', it must be 'true' or 'false.'\n",
                                       height=7, width=60)
                 return False
 
             if key in ['DOWNLOADER'] and value not in ['wget2', 'wget', 'curl', 'lftp']:
@@ -111,26 +112,27 @@
 
     def write_file(self, tags: list) -> None:
         """ Write the new values to the config file. """
         self.read_configs()
 
         with open(self.config_file, 'w') as patch_toml:
             for line in self.orig_configs:
-                for key, value in zip(self.configs['CONFIGS'].keys(), tags):
+                for key, value in zip(self.configs['configs'].keys(), tags):
 
                     if line.lstrip().startswith(f'{key} ='):
                         line = f'  {key} = "{value}"\n'
 
                     if line.lstrip().startswith(
 
                             ('COLORS =',
                              'DIALOG =',
                              'SILENT_MODE =',
                              'ASCII_CHARACTERS =',
                              'ASK_QUESTION =',
+                             'KERNEL_VERSION =',
                              'PARALLEL_DOWNLOADS =',
                              'MAXIMUM_PARALLEL = ',
                              'PROGRESS_BAR =',
                              'SPINNING_BAR =',
                              'CASE_SENSITIVE =',
                              'PROCESS_LOG =',
                              'URLLIB_RETRIES =',
```

### Comparing `slpkg-5.0.5/slpkg/download_only.py` & `slpkg-5.0.6/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/downloader.py` & `slpkg-5.0.6/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/find_installed.py` & `slpkg-5.0.6/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/gpg_verify.py` & `slpkg-5.0.6/slpkg/gpg_verify.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/load_data.py` & `slpkg-5.0.6/slpkg/load_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import json
+import time
 from pathlib import Path
+from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.blacklist import Blacklist
 from slpkg.views.asciibox import AsciiBox
+from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 
 
 class LoadData(Configs):
 
-    def __init__(self):
+    def __init__(self, flags=None):
         self.repos = Repositories()
         self.utils = Utilities()
         self.black = Blacklist()
         self.ascii = AsciiBox()
+        self.progress = ProgressBar()
+
+        if flags is None:
+            flags = []
+
+        self.bar_process = None
+
+        self.option_for_progress_bar: bool = self.utils.is_option(
+            ('-B', '--progress-bar'), flags)
 
     def load(self, repository: str, message=True) -> dict:
         if message:
-            print('\rDatabase loading... ', end='')
+            self.bar_progress()
+
         data: dict = {}
         if repository == '*':
             for repo, item in self.repos.repositories.items():
                 if item['enable']:  # Check if the repository is enabled
                     json_data_file: Path = Path(self.repos.repositories[repo]['path'], self.repos.data_json)
                     data[repo] = self.read_data_file(json_data_file)
         else:
@@ -37,15 +50,16 @@
         if blacklist:
             if repository == '*':
                 self._remove_blacklist_from_all_repos(data)
             else:
                 self._remove_blacklist_from_a_repo(data)
 
         if message:
-            print(f'{self.bgreen}{self.ascii.done}{self.endc}')
+            self.done_process()
+            # print(f'{self.bgreen}{self.ascii.done}{self.endc}')
         return data
 
     def read_data_file(self, file: Path) -> dict:
         """
         Read JSON data from the file.
         Args:
             file: Path file for reading.
@@ -95,7 +109,24 @@
         for pkg, dep in data.items():
             deps: list = dep['requires']
             for blk in blacklist_packages:
                 if blk in deps:
                     deps.remove(blk)
                     data[pkg]['requires'] = deps
         return data
+
+    def bar_progress(self) -> None:
+        if self.progress_bar or self.option_for_progress_bar:
+            message: str = 'Database loading'
+            self.bar_process = Process(target=self.progress.progress_bar, args=(message,))
+            self.bar_process.start()
+        else:
+            print('\rDatabase loading... ', end='')
+
+    def done_process(self) -> None:
+        if self.progress_bar or self.option_for_progress_bar:
+            time.sleep(0.1)
+            self.bar_process.terminate()
+            self.bar_process.join()
+            print('\x1b[?25h')
+        else:
+            print(f'{self.bgreen}{self.ascii.done}{self.endc}')
```

### Comparing `slpkg-5.0.5/slpkg/main.py` & `slpkg-5.0.6/slpkg/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         self.args: list = args
         self.flags: list = []
         self.directory: str = str(self.tmp_slpkg)
 
         self.utils = Utilities()
         self.usage = Usage()
         self.repos = Repositories()
-        self.load_data = LoadData()
 
         self.repository: str = self.repos.default_repository
 
         self.data: dict = {}
         self.flag_yes: str = '--yes'
         self.flag_short_yes: str = '-y'
         self.flag_check: str = '-c'
@@ -135,19 +134,21 @@
                 self.flag_reinstall,
                 self.flag_short_reinstall,
                 self.flag_for_progress_bar,
                 self.flag_short_for_progress_bar,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_parallel,
-                self.flag_short_parallel
+                self.flag_short_parallel,
             ],
             'repo-info': [
                 self.flag_repository,
-                self.flag_short_repository
+                self.flag_short_repository,
+                self.flag_for_progress_bar,
+                self.flag_short_for_progress_bar
             ],
             'configs': [],
             'clean-tmp': [],
             'build': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_resolve_off,
@@ -191,25 +192,27 @@
                 self.flag_directory,
                 self.flag_short_directory,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_parallel,
                 self.flag_short_parallel,
                 self.flag_no_case,
-                self.flag_short_no_case
+                self.flag_short_no_case,
+                self.flag_for_progress_bar,
+                self.flag_short_for_progress_bar
             ],
             'remove': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_resolve_off,
                 self.flag_short_resolve_off,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_for_progress_bar,
-                self.flag_short_for_progress_bar,
+                self.flag_short_for_progress_bar
             ],
             'find': [
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_no_case,
                 self.flag_short_no_case
             ],
@@ -217,49 +220,57 @@
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version,
                 self.flag_no_case,
-                self.flag_short_no_case
+                self.flag_short_no_case,
+                self.flag_for_progress_bar,
+                self.flag_short_for_progress_bar
             ],
             'search': [
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version,
                 self.flag_no_case,
-                self.flag_short_no_case
+                self.flag_short_no_case,
+                self.flag_for_progress_bar,
+                self.flag_short_for_progress_bar
             ],
             'dependees': [
                 self.flag_full_reverse,
                 self.flag_short_full_reverse,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version,
                 self.flag_no_case,
                 self.flag_short_no_case,
+                self.flag_for_progress_bar,
+                self.flag_short_for_progress_bar
             ],
             'tracking': [
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version,
                 self.flag_repository,
                 self.flag_short_repository,
                 self.flag_no_case,
                 self.flag_short_no_case,
                 self.flag_resolve_off,
-                self.flag_short_resolve_off
+                self.flag_short_resolve_off,
+                self.flag_for_progress_bar,
+                self.flag_short_for_progress_bar
             ]
         }
 
         self.commands['-h'] = self.commands['--help']
         self.commands['-v'] = self.commands['--version']
         self.commands['-u'] = self.commands['update']
         self.commands['-U'] = self.commands['upgrade']
@@ -277,14 +288,15 @@
         self.commands['-t'] = self.commands['tracking']
 
         self.split_options()
         self.split_options_from_args()
         self.move_options()
         self.invalid_options()
         self.check_for_repositories()
+        self.load_data = LoadData(self.flags)
 
         self.check = Check(self.repository)
         self.choose = Choose(self.repository)
 
     def check_for_repositories(self) -> None:
         """ Checks a combination for binaries use repositories only and if repository exists. """
         except_options: tuple = (
```

### Comparing `slpkg-5.0.5/slpkg/multi_process.py` & `slpkg-5.0.6/slpkg/multi_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/new_configs.py` & `slpkg-5.0.6/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/progress_bar.py` & `slpkg-5.0.6/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/remove_packages.py` & `slpkg-5.0.6/slpkg/remove_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,13 +130,13 @@
 
             text: str = f'There are {len(choices)} dependencies:'
             if upgrade:
                 text: str = f'There are {len(choices)} packages:'
             code, packages = self.dialogbox.checklist(text, title, height, width, list_height, choices)
             os.system('clear')
             return packages
-        return []
+        return packages
 
     def remove_question(self) -> str:
         if not self.option_for_yes and self.ask_question:
             answer: str = input('\nDo you want to remove these packages? [y/N] ')
             return answer
```

### Comparing `slpkg-5.0.5/slpkg/repo_info.py` & `slpkg-5.0.6/slpkg/repo_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class RepoInfo(Configs):
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repository: str = repository
 
-        self.load_data = LoadData()
+        self.load_data = LoadData(flags)
         self.utils = Utilities()
         self.repos = Repositories()
         self.columns, self.rows = shutil.get_terminal_size()
         self.name_alignment: int = self.columns - 61
 
         if self.name_alignment < 1:
             self.name_alignment: int = 1
@@ -30,23 +30,24 @@
         self.total_packages: int = 0
         self.repo_data: dict = {}
         self.dates: dict = {}
 
         self.option_for_repository: bool = self.utils.is_option(
             ('-o', '--repository'), flags)
 
-    def read_last_updated(self) -> dict:
-        last_updated_json: Path = Path(f'{self.repos.repositories_path}', self.repos.last_update_json)
-        if last_updated_json.is_file():
-            return self.utils.read_json_file(last_updated_json)
+    def repo_information(self) -> dict:
+        repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
+        if repo_info_json.is_file():
+            repo_info_json: Path = Path(f'{self.repos.repositories_path}', self.repos.repos_information)
+            return self.utils.read_json_file(repo_info_json)
         return {}
 
     def info(self) -> None:
         """ Prints information about repositories. """
-        self.dates: dict = self.read_last_updated()
+        self.dates: dict = self.repo_information()
         if self.option_for_repository:
             self.repo_data: dict = self.load_data.load(self.repository)
         else:
             self.repo_data: dict = self.load_data.load('*')
         self.view_the_title()
 
         if self.option_for_repository:
@@ -68,44 +69,48 @@
             title: str = f'repository information:'.title()
         print(f'\n{title}')
         print('=' * (self.columns - 1))
         print(f"{'Name:':<{self.name_alignment}}{'Status:':<14}{'Last Updated:':<34}{'Packages:':>12}")
         print('=' * (self.columns - 1))
 
     def view_the_repository_information(self) -> None:
+        date: str = 'None'
         count: int = 0
         color: str = self.red
         status: str = 'Disabled'
-        date: str = self.dates.get(self.repository, 'None')
+        if self.dates.get(self.repository):
+            date: str = self.dates[self.repository].get('last_updated', 'None')
 
         if self.repos.repositories[self.repository]['enable']:
             status: str = 'Enabled'
             color: str = self.green
             count: int = self.count_the_packages(self.repository)
 
         self.view_the_line_information(self.repository, status, date, count, color)
         self.view_summary_of_repository()
 
     def view_the_repositories_information(self) -> None:
         for repo, item in self.repos.repositories.items():
+            date: str = 'None'
             count: int = 0
             color: str = self.red
             status: str = 'Disabled'
-            date: str = self.dates.get(repo, 'None')
+            if self.dates.get(repo):
+                date: str = self.dates[repo].get('last_updated', 'None')
     
             if item['enable']:
                 self.enabled += 1
                 status: str = 'Enabled'
                 color: str = self.green
                 count: int = self.count_the_packages(repo)
 
             self.view_the_line_information(repo, status, date, count, color)
         self.view_summary_of_all_repositories()
 
-    def view_the_line_information(self, repository: str, status: str, date: str, count: int, color: str) -> None: # type: ignore
+    def view_the_line_information(self, repository: str, status: str, date: str, count: int, color: str) -> None:
         repo_color: str = self.cyan
         if repository == self.repos.default_repository:
             repo_color: str = self.byellow
             repository: str = f'{repository} (default)'
 
         print(f"{repo_color}{repository:<{self.name_alignment}}{self.endc}{color}{status:<14}{self.endc}{date:<34}"
               f"{self.yellow}{count:>12}{self.endc}")
```

### Comparing `slpkg-5.0.5/slpkg/sbos/dependencies.py` & `slpkg-5.0.6/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/sbos/sbo_generate.py` & `slpkg-5.0.6/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/sbos/slackbuild.py` & `slpkg-5.0.6/slpkg/sbos/slackbuild.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 import os
 import time
 import json
 import shutil
 
 from pathlib import Path
 from collections import OrderedDict
+from multiprocessing import Process
 
 from slpkg.upgrade import Upgrade
 from slpkg.checksum import Md5sum
 from slpkg.configs import Configs
 from slpkg.views.views import View
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.gpg_verify import GPGVerify
 from slpkg.downloader import Downloader
 from slpkg.views.asciibox import AsciiBox
+from slpkg.progress_bar import ProgressBar
 from slpkg.repositories import Repositories
 from slpkg.multi_process import MultiProcess
 from slpkg.sbos.dependencies import Requires
 
 
 class Slackbuilds(Configs):
     """ Download build and install the SlackBuilds. """
@@ -40,34 +42,40 @@
         self.dialogbox = DialogBox()
         self.multi_proc = MultiProcess(flags)
         self.view = View(flags, repository, data)
         self.check_md5 = Md5sum(flags)
         self.download = Downloader(flags)
         self.upgrade = Upgrade(repository, data)
         self.gpg = GPGVerify()
+        self.progress = ProgressBar()
 
         self.sources: dict = {}
         self.install_order: list = []
         self.dependencies: list = []
         self.skipped_packages: list = []
         self.asc_files: list = []
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
+        self.bar_process = None
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ('-k', '--skip-installed'), flags)
 
+        self.option_for_progress_bar: bool = self.utils.is_option(
+            ('-B', '--progress-bar'), flags)
+
         self.slackbuilds: list = self.utils.apply_package_pattern(data, slackbuilds)
 
         self.repo_tag: str = self.repos.repositories[repository]['repo_tag']
         self.tar_suffix: str = self.repos.repositories[repository]['tar_suffix']
 
     def execute(self) -> None:
+        self.bar_progress()
         self.creating_dependencies_list()
         self.choose_package_dependencies()
         self.add_dependencies_to_install_order()
         self.clean_the_main_slackbuilds()
         self.add_main_packages_to_install_order()
         self.check_for_skipped()
         self.view_slackbuilds_before_build()
@@ -79,23 +87,21 @@
         self.set_progress_message()
         self.build_and_install_the_slackbuilds()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
     def creating_dependencies_list(self) -> None:
-        print('\rResolving dependencies... ', end='')
         for slackbuild in self.slackbuilds:
             dependencies: tuple = Requires(self.data, slackbuild, self.flags).resolve()
 
             for dependency in dependencies:
                 self.dependencies.append(dependency)
 
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
-        print(f'{self.bgreen}{self.ascii.done}{self.endc}')
 
     def add_dependencies_to_install_order(self) -> None:
         self.install_order.extend(self.dependencies)
 
     def clean_the_main_slackbuilds(self) -> None:
         for dep in self.dependencies:
             if dep in self.slackbuilds:
@@ -278,12 +284,33 @@
 
                 if self.option_for_reinstall:
                     status: bool = True
 
                 choices.extend(
                     [(package, repo_ver, status, help_text)]
                 )
-            text: str = f'There are {len(choices)} dependencies:'
 
+            self.done_process()
+
+            text: str = f'There are {len(choices)} dependencies:'
             code, self.dependencies = self.dialogbox.checklist(text, title, height, width, list_height, choices)
 
             os.system('clear')
+        else:
+            self.done_process()
+
+    def bar_progress(self) -> None:
+        if self.progress_bar or self.option_for_progress_bar:
+            message: str = 'Resolving dependencies'
+            self.bar_process = Process(target=self.progress.progress_bar, args=(message,))
+            self.bar_process.start()
+        else:
+            print('\rResolving dependencies... ', end='')
+
+    def done_process(self) -> None:
+        if self.progress_bar or self.option_for_progress_bar:
+            time.sleep(0.1)
+            self.bar_process.terminate()
+            self.bar_process.join()
+            print('\x1b[?25h')
+        else:
+            print(f'{self.bgreen}{self.ascii.done}{self.endc}')
```

### Comparing `slpkg-5.0.5/slpkg/search.py` & `slpkg-5.0.6/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/toml_errors.py` & `slpkg-5.0.6/slpkg/toml_errors.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/tracking.py` & `slpkg-5.0.6/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/update_repositories.py` & `slpkg-5.0.6/slpkg/update_repositories.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,116 +17,87 @@
 class UpdateRepositories(Configs):
     """ Updates the local repositories and install the data
         into the database.
     """
 
     def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
-        self.flags: list = flags
-        self.repository: str = repository
 
         self.view = View(flags)
         self.multi_process = MultiProcess(flags)
         self.repos = Repositories()
         self.utils = Utilities()
         self.data = InstallData()
         self.generate = SBoGenerate()
         self.check_updates = CheckUpdates(flags, repository)
         self.download = Downloader(flags)
 
         self.repos_for_update: dict = {}
 
-        self.option_for_repository: bool = self.utils.is_option(
-            ('-o', '--repository'), flags)
-
     def repositories(self) -> None:
         self.repos_for_update: dict = self.check_updates.updates()
-        self.update_the_repositories()
 
-    def update_the_repositories(self) -> None:
         if not any(list(self.repos_for_update.values())):
             self.view.question(message='Do you want to force update?')
             # Force update the repositories.
             for repo in self.repos_for_update:
                 self.repos_for_update[repo] = True
 
-        if self.option_for_repository:
-            self.view_downloading_message(self.repository)
-            if self.repository in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
-                self.update_slackbuild_repos(self.repository)
-            else:
-                self.update_binary_repos(self.repository)
-        else:
-            for repo, update in self.repos_for_update.items():
-                if update:
-                    self.view_downloading_message(repo)
-                    if repo in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
-                        self.update_slackbuild_repos(repo)
-                    else:
-                        self.update_binary_repos(repo)
+        self.run_update()
+
+    def run_update(self) -> None:
+        for repo, update in self.repos_for_update.items():
+            if update:
+                self.view_downloading_message(repo)
+                if repo in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
+                    self.update_slackbuild_repos(repo)
+                else:
+                    self.update_binary_repos(repo)
 
     def view_downloading_message(self, repo: str) -> None:
         print(f"Syncing with the repository '{self.green}{repo}{self.endc}', please wait...\n")
 
     def update_binary_repos(self, repo: str) -> None:
+        """ Updates the binary repositories. """
         urls: dict = {}
 
-        install: dict = {
-            self.repos.slack_repo_name: self.data.install_slack_data,
-            self.repos.slack_extra_repo_name: self.data.install_slack_extra_data,
-            self.repos.slack_patches_repo_name: self.data.install_slack_patches_data,
-            self.repos.alien_repo_name: self.data.install_alien_data,
-            self.repos.multilib_repo_name: self.data.install_multilib_data,
-            self.repos.restricted_repo_name: self.data.install_restricted_data,
-            self.repos.gnome_repo_name: self.data.install_gnome_data,
-            self.repos.msb_repo_name: self.data.install_msb_data,
-            self.repos.csb_repo_name: self.data.install_csb_data,
-            self.repos.conraid_repo_name: self.data.install_conraid_data,
-            self.repos.slackdce_repo_name: self.data.install_slackdce_data,
-            self.repos.slackonly_repo_name: self.data.install_slackonly_data,
-            self.repos.salix_repo_name: self.data.install_salix_data,
-            self.repos.salix_extra_repo_name: self.data.install_salix_extra_data,
-            self.repos.slackel_repo_name: self.data.install_slackel_data,
-            self.repos.slint_repo_name: self.data.install_slint_data,
-            self.repos.pprkut_repo_name: self.data.install_pprkut_data
-        }
-
         self.utils.create_directory(self.repos.repositories[repo]['path'])
-        self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'], self.repos.repositories[repo]['changelog_txt'])
-        self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'], self.repos.repositories[repo]['packages_txt'])
-        self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'], self.repos.repositories[repo]['checksums_txt'])
-
-        changelog: str = f"{self.repos.repositories[repo]['mirror_changelog']}{self.repos.repositories[repo]['changelog_txt']}"
-        packages: str = f"{self.repos.repositories[repo]['mirror_packages']}{self.repos.repositories[repo]['packages_txt']}"
-        checksums: str = f"{self.repos.repositories[repo]['mirror_packages']}{self.repos.repositories[repo]['checksums_txt']}"
+        self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'],
+                                         self.repos.repositories[repo]['changelog_txt'])
+        self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'],
+                                         self.repos.repositories[repo]['packages_txt'])
+        self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'],
+                                         self.repos.repositories[repo]['checksums_md5'])
+
+        changelog: str = (f"{self.repos.repositories[repo]['mirror_changelog']}"
+                          f"{self.repos.repositories[repo]['changelog_txt']}")
+        packages: str = (f"{self.repos.repositories[repo]['mirror_packages']}"
+                         f"{self.repos.repositories[repo]['packages_txt']}")
+        checksums: str = (f"{self.repos.repositories[repo]['mirror_packages']}"
+                          f"{self.repos.repositories[repo]['checksums_md5']}")
 
         urls[repo] = ((changelog, packages, checksums), self.repos.repositories[repo]['path'])
 
         self.download.download(urls)
 
-        install[repo]()
+        self.data.install_binary_data(repo)
 
     def update_slackbuild_repos(self, repo: str) -> None:
-        """ Update the slackbuild repositories. """
+        """ Updates the slackbuild repositories. """
         self.utils.create_directory(self.repos.repositories[repo]['path'])
         self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'],
                                          self.repos.repositories[repo]['slackbuilds_txt'])
         self.utils.remove_file_if_exists(self.repos.repositories[repo]['path'],
                                          self.repos.repositories[repo]['changelog_txt'])
 
         lftp_command: str = (f"lftp {self.lftp_mirror_options} {self.repos.repositories[repo]['mirror_packages']} "
                              f"{self.repos.repositories[repo]['path']}")
 
         self.multi_process.process(lftp_command)
 
-        # It checks if there is a SLACKBUILDS.TXT file, otherwise it going to create one.
+        # It checks if there is a SLACKBUILDS.TXT file, otherwise it's going to create one.
         if not Path(self.repos.repositories[repo]['path'],
                     self.repos.repositories[repo]['slackbuilds_txt']).is_file():
             self.generate.slackbuild_file(self.repos.repositories[repo]['path'],
                                           self.repos.repositories[repo]['slackbuilds_txt'])
 
-        install: dict = {
-            self.repos.sbo_repo_name: self.data.install_sbo_data,
-            self.repos.ponce_repo_name: self.data.install_ponce_data
-        }
-
-        install[repo]()
+        self.data.install_sbo_data(repo)
```

### Comparing `slpkg-5.0.5/slpkg/upgrade.py` & `slpkg-5.0.6/slpkg/upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import shutil
+import platform
+from pathlib import Path
 from typing import Generator
 from packaging.version import parse, InvalidVersion
-from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 from slpkg.load_data import LoadData
 
 
@@ -27,14 +28,15 @@
         self.id: int = 0
         self.sum_upgrade: int = 0
         self.sum_removed: int = 0
         self.sum_added: int = 0
         self.installed_names: list = []
         self.installed_packages: list = []
 
+        self.kernel_ver: str = platform.uname()[2]
         self.columns, self.rows = shutil.get_terminal_size()
 
     def load_installed_packages(self, repository: str) -> None:
         if repository == self.repos.slack_repo_name:
             extra_repo: dict = {}
 
             extra_data_file: Path = Path(self.repos.repositories[self.repos.slack_extra_repo_name]['path'],
@@ -43,15 +45,15 @@
             if self.repos.repositories[self.repos.slack_extra_repo_name]['enable'] and extra_data_file.is_file():
                 extra_repo: dict = self.load_data.load(self.repos.slack_extra_repo_name, message=False)
 
             installed: dict = self.utils.all_installed()
 
             for name, package in installed.items():
                 tag: str = self.utils.split_package(package)['tag']
-                if not tag:  # Add only slackware original packages that have not tag.
+                if not tag:  # Add only slackware original packages that have not package tag.
                     if extra_repo.get(name):  # Avoid installed packages from extra repository.
                         extra_package: str = extra_repo[name]['package']
                         if extra_package[:-4] != package:
                             self.installed_packages.append(Path(package))
                             self.installed_names.append(name)
                     else:
                         self.installed_packages.append(Path(package))
@@ -85,15 +87,20 @@
 
     def is_package_upgradeable(self, installed: str) -> bool:
         """ Returns True for upgradeable packages. """
         inst_name: str = self.utils.split_package(installed)['name']
         if self.data.get(inst_name):
             repo_version: str = self.data[inst_name]['version']
             repo_build: str = self.data[inst_name]['build']
+
             inst_version: str = self.utils.split_package(installed)['version']
+            if (self.kernel_version and self.repository in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]
+                    and inst_version.endswith(f'_{self.kernel_ver}')):
+                inst_version: str = inst_version.replace(f'_{self.kernel_ver}', '')
+
             inst_build: str = self.utils.split_package(installed)['build']
             try:
                 if parse(repo_version) > parse(inst_version):
                     return True
 
                 if parse(repo_version) == parse(inst_version) and int(repo_build) > int(inst_build):
                     return True
@@ -196,15 +203,16 @@
         if found_packages:
             print()
 
             name_alignment: int = 18
             if self.columns > 80:
                 name_alignment: int = (self.columns - 80) + 18
 
-            title: str = f"{'packages':<{name_alignment}} {'Repository':<15} {'Build':<6} {'Installed':<15} {'Build':<5} {'Repo':>15}"
+            title: str = (f"{'packages':<{name_alignment}} {'Repository':<15} {'Build':<6} {'Installed':<15} "
+                          f"{'Build':<5} {'Repo':>15}")
             print(len(title) * '=')
             print(f'{self.bgreen}{title}{self.endc}')
             print(len(title) * '=')
 
             for data in found_packages.values():
                 name: str = data['name']
                 repo_version: str = data['repo_version']
@@ -223,15 +231,16 @@
 
                 color: str = self.violet
                 if mode == 'remove':
                     color: str = self.red
                 if mode == 'add':
                     color: str = self.cyan
 
-                print(f"{color}{name:<{name_alignment}}{self.endc} {repo_version:<15} {repo_build:<6} {inst_version:<15} "
+                print(f"{color}{name:<{name_alignment}}{self.endc} {repo_version:<15} "
+                      f"{repo_build:<6} {inst_version:<15} "
                       f"{inst_build:<5} {repo:>15}")
 
             print(len(title) * '=')
             print(f'{self.grey}Total packages: {self.sum_upgrade} upgraded, '
                   f'{self.sum_removed} removed and {self.sum_added} added.{self.endc}\n')
         else:
             print('\nEverything is up-to-date!\n')
```

### Comparing `slpkg-5.0.5/slpkg/utilities.py` & `slpkg-5.0.6/slpkg/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,7 +217,16 @@
         """
         matching_packages: list = []
         blacklist: tuple = self.black.packages()
         if blacklist:
             pattern: str = '|'.join(blacklist)
             matching_packages: list = [pkg for pkg in packages if re.search(pattern, pkg)]
         return matching_packages
+
+    def convert_dict_keys_to_lower(self, d: dict) -> dict:
+        new_dict = {}
+        for key, value in d.items():
+            if isinstance(value, dict):
+                value = self.convert_dict_keys_to_lower(value)
+            new_dict[key.lower()] = value
+        return new_dict
+
```

### Comparing `slpkg-5.0.5/slpkg/views/asciibox.py` & `slpkg-5.0.6/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/views/cli_menu.py` & `slpkg-5.0.6/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/views/version.py` & `slpkg-5.0.6/slpkg/views/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (5, 0, 5)
+        self.version_info: tuple = (5, 0, 6)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'GNU General Public License v3 (GPLv3)'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
         self.email: str = 'dslackw@gmail.com'
 
     def view(self) -> None:
```

### Comparing `slpkg-5.0.5/slpkg/views/view_package.py` & `slpkg-5.0.6/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/slpkg/views/views.py` & `slpkg-5.0.6/slpkg/views/views.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.5/PKG-INFO` & `slpkg-5.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 5.0.5
+Version: 5.0.6
 Summary: Package manager utility for Slackware Linux
 Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Maintainer-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slpkg Version: 5.0.5 Summary: Package manager
+Metadata-Version: 2.1 Name: slpkg Version: 5.0.6 Summary: Package manager
 utility for Slackware Linux Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis
 gmail.com> Maintainer-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Environment :: Console
 Classifier: Operating System :: POSIX Classifier: Operating System :: POSIX ::
```

