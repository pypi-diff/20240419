# Comparing `tmp/my-moodle-0.4.4.tar.gz` & `tmp/my_moodle-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-moodle-0.4.4.tar", last modified: Fri Apr 12 12:52:51 2024, max compression
+gzip compressed data, was "my_moodle-0.4.5.tar", last modified: Fri Apr 19 07:05:44 2024, max compression
```

## Comparing `my-moodle-0.4.4.tar` & `my_moodle-0.4.5.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.195171 my-moodle-0.4.4/
--rw-rw-rw-   0        0        0       36 2024-03-01 17:54:38.000000 my-moodle-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1842 2024-04-12 12:52:51.193046 my-moodle-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-03-01 02:03:47.000000 my-moodle-0.4.4/license
-drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.151948 my-moodle-0.4.4/my_moodle/
--rw-rw-rw-   0        0        0     1306 2024-03-31 18:49:59.000000 my-moodle-0.4.4/my_moodle/__init__.py
--rw-rw-rw-   0        0        0      322 2024-03-01 22:18:35.000000 my-moodle-0.4.4/my_moodle/__main__.py
--rw-rw-rw-   0        0        0     5053 2024-04-09 00:23:45.000000 my-moodle-0.4.4/my_moodle/api.py
--rw-rw-rw-   0        0        0      555 2024-04-01 03:19:50.000000 my-moodle-0.4.4/my_moodle/api_functions.py
--rw-rw-rw-   0        0        0     2825 2024-03-31 01:09:50.000000 my-moodle-0.4.4/my_moodle/config_utility.py
--rw-rw-rw-   0        0        0    12286 2024-04-03 02:33:59.000000 my-moodle-0.4.4/my_moodle/course_markdown_builder.py
--rw-rw-rw-   0        0        0      340 2024-03-31 18:28:26.000000 my-moodle-0.4.4/my_moodle/course_status.py
--rw-rw-rw-   0        0        0     1572 2024-03-31 20:29:52.000000 my-moodle-0.4.4/my_moodle/csv_utility.py
--rw-rw-rw-   0        0        0    10814 2024-04-08 19:04:03.000000 my-moodle-0.4.4/my_moodle/data_utility.py
--rw-rw-rw-   0        0        0     1393 2024-03-31 10:33:22.000000 my-moodle-0.4.4/my_moodle/enrolled_users_fields.py
--rw-rw-rw-   0        0        0     1254 2024-03-31 21:14:09.000000 my-moodle-0.4.4/my_moodle/json_utility.py
--rw-rw-rw-   0        0        0     6848 2024-03-31 11:21:10.000000 my-moodle-0.4.4/my_moodle/markdown_document.py
--rw-rw-rw-   0        0        0     3596 2024-03-31 17:05:15.000000 my-moodle-0.4.4/my_moodle/markdown_methods.py
--rw-rw-rw-   0        0        0     8545 2024-04-04 17:26:47.000000 my-moodle-0.4.4/my_moodle/moodle_data_downloader.py
--rw-rw-rw-   0        0        0     5969 2024-04-09 00:22:43.000000 my-moodle-0.4.4/my_moodle/moodle_json_downloader.py
--rw-rw-rw-   0        0        0     4896 2024-04-04 23:02:57.000000 my-moodle-0.4.4/my_moodle/program_markdown_builder.py
--rw-rw-rw-   0        0        0     4470 2024-04-09 01:00:41.000000 my-moodle-0.4.4/my_moodle/project_structure.py
--rw-rw-rw-   0        0        0      311 2024-04-01 01:42:45.000000 my-moodle-0.4.4/my_moodle/resource.json
--rw-rw-rw-   0        0        0      157 2024-04-12 12:48:56.000000 my-moodle-0.4.4/my_moodle/version.py
--rw-rw-rw-   0        0        0     8987 2024-03-31 20:15:05.000000 my-moodle-0.4.4/my_moodle/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.192038 my-moodle-0.4.4/my_moodle.egg-info/
--rw-rw-rw-   0        0        0     1842 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1066 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1243 2024-03-31 22:19:42.000000 my-moodle-0.4.4/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-12 12:52:51.195171 my-moodle-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      996 2024-04-12 12:48:56.000000 my-moodle-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.190160 my-moodle-0.4.4/tests/
--rw-rw-rw-   0        0        0     1531 2024-04-12 12:51:27.000000 my-moodle-0.4.4/tests/_.py
--rw-rw-rw-   0        0        0        0 2024-03-01 02:03:47.000000 my-moodle-0.4.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2876 2024-04-12 12:51:34.000000 my-moodle-0.4.4/tests/api_test.py
--rw-rw-rw-   0        0        0     1015 2024-03-28 07:15:10.000000 my-moodle-0.4.4/tests/config_parser_test.py
--rw-rw-rw-   0        0        0     2104 2024-04-04 16:34:12.000000 my-moodle-0.4.4/tests/course_markdown_builder_test.py
--rw-rw-rw-   0        0        0     1630 2024-03-31 21:38:20.000000 my-moodle-0.4.4/tests/moodle_data_downloader_test.py
--rw-rw-rw-   0        0        0     1243 2024-03-31 20:27:00.000000 my-moodle-0.4.4/tests/moodle_data_utility_test.py
--rw-rw-rw-   0        0        0     1408 2024-03-30 17:59:07.000000 my-moodle-0.4.4/tests/moodle_json_downloader_test.py
--rw-rw-rw-   0        0        0     1476 2024-03-31 15:44:24.000000 my-moodle-0.4.4/tests/package_test.py
--rw-rw-rw-   0        0        0     1013 2024-03-30 20:11:27.000000 my-moodle-0.4.4/tests/program_markdown_builder_test.py
--rw-rw-rw-   0        0        0      659 2024-04-12 12:48:56.000000 my-moodle-0.4.4/tests/version_test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.988799 my_moodle-0.4.5/
+-rw-rw-rw-   0        0        0       36 2024-03-01 17:54:38.000000 my_moodle-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1842 2024-04-19 07:05:44.987793 my_moodle-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2024-03-01 02:03:47.000000 my_moodle-0.4.5/license
+drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.966308 my_moodle-0.4.5/my_moodle/
+-rw-rw-rw-   0        0        0     1470 2024-04-19 06:58:15.000000 my_moodle-0.4.5/my_moodle/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-03-01 22:18:35.000000 my_moodle-0.4.5/my_moodle/__main__.py
+-rw-rw-rw-   0        0        0     5053 2024-04-09 00:23:45.000000 my_moodle-0.4.5/my_moodle/api.py
+-rw-rw-rw-   0        0        0      555 2024-04-01 03:19:50.000000 my_moodle-0.4.5/my_moodle/api_functions.py
+-rw-rw-rw-   0        0        0     2825 2024-03-31 01:09:50.000000 my_moodle-0.4.5/my_moodle/config_utility.py
+-rw-rw-rw-   0        0        0    12286 2024-04-03 02:33:59.000000 my_moodle-0.4.5/my_moodle/course_markdown_builder.py
+-rw-rw-rw-   0        0        0      340 2024-03-31 18:28:26.000000 my_moodle-0.4.5/my_moodle/course_status.py
+-rw-rw-rw-   0        0        0     1629 2024-04-19 00:15:14.000000 my_moodle-0.4.5/my_moodle/csv_utility.py
+-rw-rw-rw-   0        0        0    10814 2024-04-08 19:04:03.000000 my_moodle-0.4.5/my_moodle/data_utility.py
+-rw-rw-rw-   0        0        0     1393 2024-03-31 10:33:22.000000 my_moodle-0.4.5/my_moodle/enrolled_users_fields.py
+-rw-rw-rw-   0        0        0     1254 2024-03-31 21:14:09.000000 my_moodle-0.4.5/my_moodle/json_utility.py
+-rw-rw-rw-   0        0        0     6848 2024-03-31 11:21:10.000000 my_moodle-0.4.5/my_moodle/markdown_document.py
+-rw-rw-rw-   0        0        0     3596 2024-03-31 17:05:15.000000 my_moodle-0.4.5/my_moodle/markdown_methods.py
+-rw-rw-rw-   0        0        0     8694 2024-04-19 01:10:59.000000 my_moodle-0.4.5/my_moodle/moodle_data_downloader.py
+-rw-rw-rw-   0        0        0     6500 2024-04-19 00:36:16.000000 my_moodle-0.4.5/my_moodle/moodle_json_downloader.py
+-rw-rw-rw-   0        0        0     2552 2024-04-19 02:49:07.000000 my_moodle-0.4.5/my_moodle/notebook_utility.py
+-rw-rw-rw-   0        0        0     4469 2024-04-19 01:34:39.000000 my_moodle-0.4.5/my_moodle/program_markdown_builder.py
+-rw-rw-rw-   0        0        0     4470 2024-04-09 01:00:41.000000 my_moodle-0.4.5/my_moodle/project_structure.py
+-rw-rw-rw-   0        0        0     1169 2024-04-19 01:43:28.000000 my_moodle-0.4.5/my_moodle/resource.json
+-rw-rw-rw-   0        0        0     2221 2024-04-19 02:49:40.000000 my_moodle-0.4.5/my_moodle/resource_utility.py
+-rw-rw-rw-   0        0        0     5517 2024-04-19 06:59:54.000000 my_moodle-0.4.5/my_moodle/update_utility.py
+-rw-rw-rw-   0        0        0      157 2024-04-19 00:13:16.000000 my_moodle-0.4.5/my_moodle/version.py
+-rw-rw-rw-   0        0        0     8987 2024-03-31 20:15:05.000000 my_moodle-0.4.5/my_moodle/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.986550 my_moodle-0.4.5/my_moodle.egg-info/
+-rw-rw-rw-   0        0        0     1842 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1185 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 07:05:44.000000 my_moodle-0.4.5/my_moodle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1243 2024-03-31 22:19:42.000000 my_moodle-0.4.5/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:05:44.988799 my_moodle-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      996 2024-04-19 00:13:16.000000 my_moodle-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:05:44.985773 my_moodle-0.4.5/tests/
+-rw-rw-rw-   0        0        0     1531 2024-04-12 12:51:27.000000 my_moodle-0.4.5/tests/_.py
+-rw-rw-rw-   0        0        0        0 2024-03-01 02:03:47.000000 my_moodle-0.4.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     2876 2024-04-12 12:51:34.000000 my_moodle-0.4.5/tests/api_test.py
+-rw-rw-rw-   0        0        0     1015 2024-03-28 07:15:10.000000 my_moodle-0.4.5/tests/config_parser_test.py
+-rw-rw-rw-   0        0        0     2104 2024-04-04 16:34:12.000000 my_moodle-0.4.5/tests/course_markdown_builder_test.py
+-rw-rw-rw-   0        0        0     1636 2024-04-19 00:39:24.000000 my_moodle-0.4.5/tests/moodle_data_downloader_test.py
+-rw-rw-rw-   0        0        0     1243 2024-03-31 20:27:00.000000 my_moodle-0.4.5/tests/moodle_data_utility_test.py
+-rw-rw-rw-   0        0        0     1414 2024-04-19 00:35:51.000000 my_moodle-0.4.5/tests/moodle_json_downloader_test.py
+-rw-rw-rw-   0        0        0     1768 2024-04-19 01:52:39.000000 my_moodle-0.4.5/tests/notebook_utility_test.py
+-rw-rw-rw-   0        0        0     1476 2024-03-31 15:44:24.000000 my_moodle-0.4.5/tests/package_test.py
+-rw-rw-rw-   0        0        0     1013 2024-03-30 20:11:27.000000 my_moodle-0.4.5/tests/program_markdown_builder_test.py
+-rw-rw-rw-   0        0        0      659 2024-04-19 00:13:16.000000 my_moodle-0.4.5/tests/version_test.py
```

### Comparing `my-moodle-0.4.4/PKG-INFO` & `my_moodle-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-moodle
-Version: 0.4.4
+Version: 0.4.5
 Summary: Download Moodle Course content.
 Home-page: https://github.com/marcocrowe/my-moodle-py-pi/
 Author: Mark Crowe
 Author-email: 66536097+marcocrowe@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/marcocrowe/my-moodle-py-pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `my-moodle-0.4.4/my_moodle/__init__.py` & `my_moodle-0.4.5/my_moodle/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 
 from . import api_functions as ApiFunctions
 from . import config_utility as ConfigUtility
 from . import csv_utility as CsvUtility
 from . import data_utility as DataUtility
 from . import json_utility as JsonUtility
 from . import markdown_methods
+from . import notebook_utility as NotebookUtility
 from .api import Api
 from .course_markdown_builder import CourseMarkdownBuilder
 from .course_status import CourseStatus
 from .enrolled_users_fields import EnrolledUsersFields
 from .markdown_document import MarkdownDocument
 from .moodle_data_downloader import MoodleDataDownloader
 from .moodle_json_downloader import MoodleJsonDownloader
 from .program_markdown_builder import ProgramMarkdownBuilder
+from .update_utility import update_my_moodle_template
 from .version import __version__
 from .wrapper import Course, MoodleFile
 from .__main__ import main
 
 __all__ = [
     "Api",
     "ApiFunctions",
     "ConfigUtility",
     "Course",
     "CourseMarkdownBuilder",
     "CourseStatus",
     "CsvUtility",
+    "DataUtility",
     "EnrolledUsersFields",
     "JsonUtility",
     "main",
     "markdown_methods",
     "MarkdownDocument",
     "MoodleDataDownloader",
     "MoodleFile",
-    "DataUtility",
     "MoodleJsonDownloader",
+    "NotebookUtility",
     "ProgramMarkdownBuilder",
+    "update_my_moodle_template",
     "__version__",
 ]
```

### Comparing `my-moodle-0.4.4/my_moodle/api.py` & `my_moodle-0.4.5/my_moodle/api.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/api_functions.py` & `my_moodle-0.4.5/my_moodle/api_functions.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/config_utility.py` & `my_moodle-0.4.5/my_moodle/config_utility.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/course_markdown_builder.py` & `my_moodle-0.4.5/my_moodle/course_markdown_builder.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/csv_utility.py` & `my_moodle-0.4.5/my_moodle/csv_utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 def save_json_fields_list_to_csv(
     json_list: list[dict], fieldnames: list, filename: str
 ) -> None:
     """Save data to a CSV file.
 
     Args:
         data (list): List of JSON dictionaries containing data to be saved.
+        fieldnames (list): List of field names to save.
         filename (str): Name of the CSV file to save.
     """
     if not json_list:
         logging.warning("No data to save.")
         return
 
     with open(filename, mode="w", newline="", encoding="utf-8") as file:
```

### Comparing `my-moodle-0.4.4/my_moodle/data_utility.py` & `my_moodle-0.4.5/my_moodle/data_utility.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/enrolled_users_fields.py` & `my_moodle-0.4.5/my_moodle/enrolled_users_fields.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/json_utility.py` & `my_moodle-0.4.5/my_moodle/json_utility.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/markdown_document.py` & `my_moodle-0.4.5/my_moodle/markdown_document.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/markdown_methods.py` & `my_moodle-0.4.5/my_moodle/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/moodle_data_downloader.py` & `my_moodle-0.4.5/my_moodle/moodle_data_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,28 @@
 
     def __init__(
         self,
         program_name: str,
         server: str,
         token: str,
         data_dir: str = "",
+        enable_enrollment_download: bool = False,
         timeout: float = 300.0,
         rest_format: str = "json",
     ):
         self.program_name = program_name
         """College program name"""
         self._api = Api(server, token, rest_format, timeout)
         """API for Moodle"""
         dir_p = f"{data_dir}/_data" if not data_dir else "_data"
-        self._json_downloader = MoodleJsonDownloader(program_name, self._api, dir_p)
-        """Moodle JSON downloader"""
+        """Data directory path"""
+        self._json_downloader = MoodleJsonDownloader(
+            program_name, self._api, enable_enrollment_download, dir_p
+        )
+        """Enable enrollment download flag"""
         self.data_dir = data_dir
         """Data directory"""
 
     @property
     def api(self) -> Api:
         """API for Moodle
 
@@ -53,14 +57,15 @@
         """Moodle JSON downloader
 
         Returns:
             MoodleJsonDownloader: The Moodle JSON downloader
         """
         return self._json_downloader
 
+
     def create_directory(self, directory: str) -> str:
         """Create a directory
 
         Args:
             directory (str): The directory to create
 
         Returns:
```

### Comparing `my-moodle-0.4.4/my_moodle/moodle_json_downloader.py` & `my_moodle-0.4.5/my_moodle/moodle_json_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,40 +18,57 @@
     make_slug,
 )
 
 
 class MoodleJsonDownloader:
     """Moodle data downloader"""
 
-    def __init__(self, program_name: str, api: Api, data_dir: str = "_data"):
+    def __init__(
+        self,
+        program_name: str,
+        api: Api,
+        enable_enrollment_download: bool = False,
+        data_dir: str = "_data",
+    ):
         """Constructor
 
         Args:
             program_name (str): The program name
             api (Api): The API for Moodle
             data_dir (str, optional): The data directory. Defaults to "_data".
         """
         self._api: Api = api
         """API for Moodle"""
         self.data_dir = data_dir
         """Data directory"""
         self._program_name = program_name
         """College program name"""
+        self.__enable_enrollment_download = enable_enrollment_download
+        """Enable enrollment download flag"""
 
         makedirs(self.data_dir, exist_ok=True)
 
     @property
     def api(self) -> Api:
         """API for Moodle
 
         Returns:
             Api: The API for Moodle
         """
         return self._api
 
+    @property
+    def __is_enrollment_download_enabled(self) -> bool:
+        """Is enrollment download enabled
+
+        Returns:
+            bool: True if enrollment download is enabled
+        """
+        return self.__enable_enrollment_download
+
     def create_directory(self, directory: str) -> str:
         """Create a directory
 
         Args:
             directory (str): The directory to create
 
         Returns:
@@ -92,15 +109,16 @@
 
         for course_json in courses_json.get("courses", []):
             if course_json.get("coursecategory") == N_TUTORR:
                 continue
 
             self.download_course_contents(course_json)
             # self.download_json_course_private_files(course_json)
-            self.download_students_by_course(course_json)
+            if self.__is_enrollment_download_enabled:
+                self.download_students_by_course(course_json)
 
     def download_course_contents(self, course_json: dict) -> None:
         """Download course contents json
         Args:
             course_json (dict): The course json
         """
         course_id = course_json.get("id", "")
```

### Comparing `my-moodle-0.4.4/my_moodle/program_markdown_builder.py` & `my_moodle-0.4.5/my_moodle/program_markdown_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
 ProgramMarkdownBuilder Class
 """
 
 import logging
 from os import makedirs
-from os.path import dirname, join
 from pathlib import Path
 
-from my_moodle.json_utility import load_json_from_file
+from .resource_utility import PackageResources
 from .data_utility import N_TUTORR, group_courses_by_category
 from .markdown_document import MarkdownDocument
 from .markdown_methods import MarkdownLink
 from .project_structure import course_directory, clean_course_name
 
+
 class ProgramMarkdownBuilder:
     """Program Markdown Builder"""
 
     def __init__(self, program_name: str, filename: str = "readme.md"):
         """Initialise the CourseMarkdownBuilder
 
         Args:
@@ -87,39 +87,26 @@
         """
         with open(file_path, "w", encoding=encoding) as file:
             file.write(str(self))
 
     def add_template_notice(self) -> None:
         """Add the template notice"""
 
-        package_recourses = self.get_package_recourses()
-        template_message = package_recourses["template_message"]
+        package_recourses = PackageResources()
 
         link = "https://github.com/marcocrowe/my-moodle-template"
         instructions_link = "template-instructions.md"
-        filled_message = template_message.format(
+        filled_message = package_recourses.template_message.format(
             link=link, instructions_link=instructions_link
         )
 
         self._markdown_document.write_paragraph(filled_message)
         self._markdown_document.write_hr()
         self._markdown_document.write_line()
 
-    def get_package_recourses(self) -> dict:
-        """Get the package recourses
-
-        Returns:
-            dict: This package's recourses
-
-        """
-        current_dir = dirname(__file__)
-        resource_filename = "resource.json"
-
-        return load_json_from_file(join(current_dir, resource_filename))
-
     def process_courses_json(self, courses_json: list[dict]) -> None:
         """Process the courses json
 
         Args:
             courses_json (dict): The courses json.
         """
 
@@ -129,13 +116,13 @@
         for category, courses in courses_by_category.items():
             if category == N_TUTORR:
                 logging.warning("Skipping category: %s", category)
                 continue
             self.add_category(category)
             courses = sorted(courses, key=lambda x: x.get("fullname", ""))
             for course in courses:
-                name =  clean_course_name(course.get("fullname", ""))
+                name = clean_course_name(course.get("fullname", ""))
                 dir_path = course_directory(course)
 
                 self.add_course(clean_course_name(name), dir_path)
             self._markdown_document.write_line()
         self._markdown_document.write_hr()
```

### Comparing `my-moodle-0.4.4/my_moodle/project_structure.py` & `my_moodle-0.4.5/my_moodle/project_structure.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle/wrapper.py` & `my_moodle-0.4.5/my_moodle/wrapper.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/my_moodle.egg-info/PKG-INFO` & `my_moodle-0.4.5/my_moodle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-moodle
-Version: 0.4.4
+Version: 0.4.5
 Summary: Download Moodle Course content.
 Home-page: https://github.com/marcocrowe/my-moodle-py-pi/
 Author: Mark Crowe
 Author-email: 66536097+marcocrowe@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/marcocrowe/my-moodle-py-pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `my-moodle-0.4.4/my_moodle.egg-info/SOURCES.txt` & `my_moodle-0.4.5/my_moodle.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 my_moodle/data_utility.py
 my_moodle/enrolled_users_fields.py
 my_moodle/json_utility.py
 my_moodle/markdown_document.py
 my_moodle/markdown_methods.py
 my_moodle/moodle_data_downloader.py
 my_moodle/moodle_json_downloader.py
+my_moodle/notebook_utility.py
 my_moodle/program_markdown_builder.py
 my_moodle/project_structure.py
 my_moodle/resource.json
+my_moodle/resource_utility.py
+my_moodle/update_utility.py
 my_moodle/version.py
 my_moodle/wrapper.py
 my_moodle.egg-info/PKG-INFO
 my_moodle.egg-info/SOURCES.txt
 my_moodle.egg-info/dependency_links.txt
 my_moodle.egg-info/requires.txt
 my_moodle.egg-info/top_level.txt
@@ -31,10 +34,11 @@
 tests/__init__.py
 tests/api_test.py
 tests/config_parser_test.py
 tests/course_markdown_builder_test.py
 tests/moodle_data_downloader_test.py
 tests/moodle_data_utility_test.py
 tests/moodle_json_downloader_test.py
+tests/notebook_utility_test.py
 tests/package_test.py
 tests/program_markdown_builder_test.py
 tests/version_test.py
```

### Comparing `my-moodle-0.4.4/readme.md` & `my_moodle-0.4.5/readme.md`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/setup.py` & `my_moodle-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Setuptools configuration for my-moodle package.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="my-moodle",
-    version="0.4.4",
+    version="0.4.5",
     author="Mark Crowe",
     author_email="66536097+marcocrowe@users.noreply.github.com",
     description="Download Moodle Course content.",
     long_description=open("readme.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/marcocrowe/my-moodle-py-pi/",
     project_urls={
```

### Comparing `my-moodle-0.4.4/tests/_.py` & `my_moodle-0.4.5/tests/_.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/tests/api_test.py` & `my_moodle-0.4.5/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/tests/config_parser_test.py` & `my_moodle-0.4.5/tests/config_parser_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/tests/course_markdown_builder_test.py` & `my_moodle-0.4.5/tests/course_markdown_builder_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/tests/moodle_data_downloader_test.py` & `my_moodle-0.4.5/tests/moodle_data_downloader_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,12 +30,12 @@
 
         Returns:
             MoodleDataDownloader: The MoodleDataDownloader object
         """
         #data_dir: str = "data"
         test_config_file: str = "tests/config-a-s.ini"
         program_name, server, token = check_and_read_config(test_config_file)
-        return MoodleDataDownloader(program_name, server, token, getcwd())
+        return MoodleDataDownloader(program_name, server, token, getcwd(), True)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `my-moodle-0.4.4/tests/moodle_data_utility_test.py` & `my_moodle-0.4.5/tests/moodle_data_utility_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/tests/moodle_json_downloader_test.py` & `my_moodle-0.4.5/tests/moodle_json_downloader_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def __build_sut(self) -> MoodleJsonDownloader:
         """Generate a MoodleJsonDownloader object for testing.
 
         Returns:
             MoodleJsonDownloader: The MoodleJsonDownloader object
         """
         directory: str = "tests"
-        test_config_file: str = f"{directory}/config-a-s.ini"
+        test_config_file: str = f"{directory}/config-b-s.ini"
         program_name, server, token = check_and_read_config(test_config_file)
         api = Api(server, token)
-        return MoodleJsonDownloader(program_name, api)
+        return MoodleJsonDownloader(program_name, api, True)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `my-moodle-0.4.4/tests/package_test.py` & `my_moodle-0.4.5/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/tests/program_markdown_builder_test.py` & `my_moodle-0.4.5/tests/program_markdown_builder_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.4/tests/version_test.py` & `my_moodle-0.4.5/tests/version_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class TestVersion(unittest.TestCase):
     """Test case for version"""
 
     def test_version(self) -> None:
         """Test the version of the package"""
-        expected_version: str = "0.4.4"  # Update this value when the version changes
+        expected_version: str = "0.4.5"  # Update this value when the version changes
         self.assertEqual(
             __version__,
             expected_version,
             f"Expected version: {expected_version}, Actual version: {__version__}",
         )
```

