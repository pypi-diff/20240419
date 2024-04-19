# Comparing `tmp/loggingpython-1.4.1.tar.gz` & `tmp/loggingpython-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.4.1.tar", last modified: Mon Apr 15 19:39:43 2024, max compression
+gzip compressed data, was "loggingpython-1.4.2.tar", last modified: Fri Apr 19 13:26:27 2024, max compression
```

## Comparing `loggingpython-1.4.1.tar` & `loggingpython-1.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.247328 loggingpython-1.4.1/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     3264 2024-04-15 19:39:43.246828 loggingpython-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 19:39:43.247829 loggingpython-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1257 2024-04-15 19:39:35.000000 loggingpython-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.199828 loggingpython-1.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.208829 loggingpython-1.4.1/src/loggingpython/
--rw-rw-rw-   0        0        0     3763 2024-04-15 19:39:30.000000 loggingpython-1.4.1/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.236828 loggingpython-1.4.1/src/loggingpython/error/
--rw-rw-rw-   0        0        0      905 2024-04-05 12:51:00.000000 loggingpython-1.4.1/src/loggingpython/error/__init__.py
--rw-rw-rw-   0        0        0      439 2024-04-05 12:59:23.000000 loggingpython-1.4.1/src/loggingpython/error/client_method_call_error.py
--rw-rw-rw-   0        0        0      382 2024-04-05 12:57:01.000000 loggingpython-1.4.1/src/loggingpython/error/handler_not_found_error.py
--rw-rw-rw-   0        0        0      516 2024-04-07 13:27:03.000000 loggingpython-1.4.1/src/loggingpython/error/invalid_handler_method_error.py
--rw-rw-rw-   0        0        0      369 2024-04-07 13:41:59.000000 loggingpython-1.4.1/src/loggingpython/error/invalid_log_level_error.py
--rw-rw-rw-   0        0        0      439 2024-04-05 13:01:02.000000 loggingpython-1.4.1/src/loggingpython/error/server_method_call_error.py
--rw-rw-rw-   0        0        0      460 2024-04-07 13:28:09.000000 loggingpython-1.4.1/src/loggingpython/error/server_unreachable_error.py
-drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.243329 loggingpython-1.4.1/src/loggingpython/handler/
--rw-rw-rw-   0        0        0      777 2024-04-03 19:28:43.000000 loggingpython-1.4.1/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     3422 2024-04-14 13:49:48.000000 loggingpython-1.4.1/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     3901 2024-04-14 16:01:40.000000 loggingpython-1.4.1/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     3777 2024-04-14 13:49:55.000000 loggingpython-1.4.1/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     1653 2024-04-14 13:50:01.000000 loggingpython-1.4.1/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     5518 2024-04-14 16:01:45.000000 loggingpython-1.4.1/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     4707 2024-04-14 16:03:19.000000 loggingpython-1.4.1/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0    12186 2024-04-15 19:20:42.000000 loggingpython-1.4.1/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.4.1/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0    16486 2024-04-14 14:44:12.000000 loggingpython-1.4.1/src/loggingpython/logger.py
--rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.4.1/src/loggingpython/sys_procolls.py
-drwxrwxrwx   0        0        0        0 2024-04-15 19:39:43.244828 loggingpython-1.4.1/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3264 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 19:39:43.000000 loggingpython-1.4.1/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.424312 loggingpython-1.4.2/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     3264 2024-04-19 13:26:27.423313 loggingpython-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 13:26:27.424812 loggingpython-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1257 2024-04-19 13:25:54.000000 loggingpython-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.357312 loggingpython-1.4.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.375314 loggingpython-1.4.2/src/loggingpython/
+-rw-rw-rw-   0        0        0     3763 2024-04-15 19:39:30.000000 loggingpython-1.4.2/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.409313 loggingpython-1.4.2/src/loggingpython/error/
+-rw-rw-rw-   0        0        0      905 2024-04-05 12:51:00.000000 loggingpython-1.4.2/src/loggingpython/error/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-04-05 12:59:23.000000 loggingpython-1.4.2/src/loggingpython/error/client_method_call_error.py
+-rw-rw-rw-   0        0        0      382 2024-04-05 12:57:01.000000 loggingpython-1.4.2/src/loggingpython/error/handler_not_found_error.py
+-rw-rw-rw-   0        0        0      516 2024-04-07 13:27:03.000000 loggingpython-1.4.2/src/loggingpython/error/invalid_handler_method_error.py
+-rw-rw-rw-   0        0        0      369 2024-04-07 13:41:59.000000 loggingpython-1.4.2/src/loggingpython/error/invalid_log_level_error.py
+-rw-rw-rw-   0        0        0      439 2024-04-05 13:01:02.000000 loggingpython-1.4.2/src/loggingpython/error/server_method_call_error.py
+-rw-rw-rw-   0        0        0      460 2024-04-07 13:28:09.000000 loggingpython-1.4.2/src/loggingpython/error/server_unreachable_error.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.418312 loggingpython-1.4.2/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0      777 2024-04-03 19:28:43.000000 loggingpython-1.4.2/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     3440 2024-04-17 14:05:56.000000 loggingpython-1.4.2/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     3937 2024-04-17 14:05:58.000000 loggingpython-1.4.2/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     4441 2024-04-19 13:11:20.000000 loggingpython-1.4.2/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     1653 2024-04-14 13:50:01.000000 loggingpython-1.4.2/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     5554 2024-04-17 14:06:10.000000 loggingpython-1.4.2/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     4743 2024-04-17 14:06:26.000000 loggingpython-1.4.2/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0    12186 2024-04-15 19:20:42.000000 loggingpython-1.4.2/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.4.2/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0    16486 2024-04-14 14:44:12.000000 loggingpython-1.4.2/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.4.2/src/loggingpython/sys_procolls.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.419813 loggingpython-1.4.2/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3264 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/top_level.txt
```

### Comparing `loggingpython-1.4.1/LICENSE` & `loggingpython-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/PKG-INFO` & `loggingpython-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.1
+Version: 1.4.2
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.1/README.md` & `loggingpython-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/setup.py` & `loggingpython-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.4.1',
+    version='1.4.2',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
```

### Comparing `loggingpython-1.4.1/src/loggingpython/__init__.py` & `loggingpython-1.4.2/src/loggingpython/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/src/loggingpython/error/__init__.py` & `loggingpython-1.4.2/src/loggingpython/error/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/src/loggingpython/error/invalid_handler_method_error.py` & `loggingpython-1.4.2/src/loggingpython/error/invalid_handler_method_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/__init__.py` & `loggingpython-1.4.2/src/loggingpython/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/consolehandler.py` & `loggingpython-1.4.2/src/loggingpython/handler/consolehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
     This class inherits from the Handler class and implements specific
     methods for formatting and outputting log messages in the console.
     It supports the coloring of log messages based on their
     severity and allows customization of the formatting string.
     """
 
-    def __init__(self, stream: TextIO = sys.stdout,
+    def __init__(self,
+                 stream: TextIO = sys.stdout,
                  logformat_string: str = "%(asctime)s: [%(loggername)s]: \
 [%(loglevel)s]: %(message)s") -> None:
         """
         Initializes the ConsoleHandler with an optional stream and an optional
         optional formatting string for log messages.
 
         Args:
```

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/csvhandler.py` & `loggingpython-1.4.2/src/loggingpython/handler/csvhandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     This class inherits from the Handler class and implements specific
     methods for formatting and outputting log messages in CSV files. It
     supports the creation of new log files based on the current date and
     allows customization of the log format string. The CSVHandler ensures
     that log messages are stored in a structured and easily accessible format,
     making it suitable for further analysis or review.
     """
-    def __init__(self, name: str, path: str = "logs",
+    def __init__(self,
+                 name: str,
+                 path: str = "logs",
                  logformat_string: str = "%(asctime)s: [%(loggername)s]: \
 [%(loglevel)s]: %(message)s") -> None:
         """
         Initializes the CSVHandler with the given name, log path, and log
             format string.
 
         Args:
```

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/filehandler.py` & `loggingpython-1.4.2/src/loggingpython/handler/filehandler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import os
+from datetime import timedelta
 from datetime import datetime
 
+
 from .handler import Handler
 
 
 class FileHandler(Handler):
     """
     A class for handling log messages in files.
 
     This class inherits from the Handler class and implements specific
     methods for formatting and outputting log messages to files. It supports
     the creation of log files in a specified directory, automatic file rotation
     based on the current date, and allows customization of the formatting
     string. The FileHandler ensures that log messages are stored persistently
     and can be reviewed later for debugging or auditing purposes.
     """
-    def __init__(self, name: str, path: str = "logs",
+    def __init__(self,
+                 name: str,
+                 path: str = "logs",
                  logformat_string: str = "%(asctime)s: [%(loggername)s]: \
-[%(loglevel)s]: %(message)s") -> None:
+[%(loglevel)s]: %(message)s",
+                 new_file_after: timedelta = timedelta(days=1)
+                 ) -> None:
         """
         Initializes the FileHandler with the given name, log path, and log
             format string.
 
         Args:
             name (str): The name of the log file.
             path (str, optional): The path where the log files will be
@@ -61,14 +67,26 @@
         current_date = datetime.now().strftime("%Y-%m-%d")
         if current_date != self._current_date:
             self.current_date = current_date
             self._close_file()
             filename = f"{self.logpath}/{self.name}_{self._current_date}.log"
             self.file = open(filename, "a")
 
+    def _update_file(self) -> None:
+        """
+        Updates the log file if the current date has changed.
+        """
+        current_date = datetime.now().strftime("%Y-%m-%d")
+        if (datetime.now() - self.last_log_time) > self.new_file_after:
+            self._current_date = current_date
+            self._close_file()
+            filename = f"{self.path}/{self.name}_{self._current_date}.log"
+            self.file = open(filename, "a")
+            self.last_log_time = datetime.now()
+
     def _close_file(self) -> None:
         """
         Closes the current log file.
         """
         if self.file:
             self.file.close()
```

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/handler.py` & `loggingpython-1.4.2/src/loggingpython/handler/handler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/jsonhandler.py` & `loggingpython-1.4.2/src/loggingpython/handler/jsonhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     supports the creation of new log files based on the current date and
     allows customization of the log format string. The JSONHandler ensures
     that log messages are stored in a structured and easily accessible format,
     making it suitable for further analysis or review. It also includes
     features for hashing log messages for unique identification and updating
     the log file if the current date has changed.
     """
-    def __init__(self, name: str, path: str = "logs") -> None:
+    def __init__(self,
+                 name: str,
+                 path: str = "logs") -> None:
         """
         Initializes the JSONHandler with the given name, log path, and log
             format string.
 
         Args:
             name (str): The name of the log file.
             path (str, optional): The path where the log files will be
```

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.4.2/src/loggingpython/handler/sqlhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     supports the creation of new log databases based on the current date and
     allows customization of the log format string. The SQLHandler ensures
     that log messages are stored in a structured and easily accessible format,
     making it suitable for further analysis or review. It also includes
     features for updating the log database if the current date has changed and
     for creating the necessary database structure.
     """
-    def __init__(self, name: str, path: str = "logs") -> None:
+    def __init__(self,
+                 name: str,
+                 path: str = "logs") -> None:
         """
         Initializes the SQLHandler with the given name, log path, and log
             format string.
 
         Args:
             name (str): The name of the log file.
             path (str, optional): The path where the log files will be
```

### Comparing `loggingpython-1.4.1/src/loggingpython/handler/syshandler.py` & `loggingpython-1.4.2/src/loggingpython/handler/syshandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/src/loggingpython/logger.py` & `loggingpython-1.4.2/src/loggingpython/logger.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.1/src/loggingpython.egg-info/PKG-INFO` & `loggingpython-1.4.2/src/loggingpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.1
+Version: 1.4.2
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.1/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.4.2/src/loggingpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

