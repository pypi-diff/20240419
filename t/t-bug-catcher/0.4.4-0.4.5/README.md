# Comparing `tmp/t_bug_catcher-0.4.4.tar.gz` & `tmp/t_bug_catcher-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-rt3__0l8/t_bug_catcher-0.4.4.tar", last modified: Wed Apr 17 08:22:43 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-iwxaa_jb/t_bug_catcher-0.4.5.tar", last modified: Fri Apr 19 07:47:15 2024, max compression
```

## Comparing `t_bug_catcher-0.4.4.tar` & `t_bug_catcher-0.4.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.297112 t_bug_catcher-0.4.4/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11049 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    45412 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.297112 t_bug_catcher-0.4.4/t_bug_catcher/resources/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/resources/whispers_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     5578 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-17 08:22:43.000000 t_bug_catcher-0.4.4/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 08:22:43.301112 t_bug_catcher-0.4.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-17 08:22:15.000000 t_bug_catcher-0.4.4/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12221 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49938 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-19 07:47:15.000000 t_bug_catcher-0.4.5/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-19 07:47:15.000000 t_bug_catcher-0.4.5/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-19 07:47:15.000000 t_bug_catcher-0.4.5/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-19 07:47:15.000000 t_bug_catcher-0.4.5/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-19 07:47:15.000000 t_bug_catcher-0.4.5/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-19 07:47:15.000000 t_bug_catcher-0.4.5/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 07:47:15.434864 t_bug_catcher-0.4.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-19 07:46:47.000000 t_bug_catcher-0.4.5/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.4/PKG-INFO` & `t_bug_catcher-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.4
+Version: 0.4.5
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.4/README.rst` & `t_bug_catcher-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/setup.py` & `t_bug_catcher-0.4.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.4.4",
+    version="0.4.5",
     zip_safe=False,
     install_requires=install_requirements,
     include_package_data=True,
     package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.5/t_bug_catcher/bug_catcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """JiraPoster class for interacting with the Jira API."""
 
+import inspect
 import os
 import sys
 from types import TracebackType
 from typing import List, Optional
 
 from .bug_snag import BugSnag
 from .config import CONFIG
@@ -125,19 +126,41 @@
             logger.warning("Jira and BugSnag are not configured. Please configure them before reporting an error.")
             return
 
         if not exception:
             _, exception, _ = sys.exc_info()
 
         if not isinstance(exception, Exception):
-            logger.warning("Exception must be an instance of Exception.")
+            logger.warning("Implementation error. Incorrect exception type.")
+            inspected_frame = inspect.currentframe().f_back
+            if self.__configurator.is_jira_configured:
+                self.__jira.warning_message(
+                    summary="bug_catcher implementation warning ⚠️",
+                    inspected_frame=inspected_frame,
+                    message=(
+                        "Incorrect exception type. Check the variable that holds the exception "
+                        "and make sure that report_error() in the try/except block is called."
+                    ),
+                    assignee=assignee,
+                )
             return
 
         if not getattr(exception, "__traceback__", None):
-            logger.warning("No traceback available. Please provide a traceback.")
+            logger.warning("Implementation error. No traceback available.")
+            inspected_frame = inspect.currentframe().f_back
+            if self.__configurator.is_jira_configured:
+                self.__jira.warning_message(
+                    summary="bug_catcher implementation warning ⚠️",
+                    inspected_frame=inspected_frame,
+                    message=(
+                        "No traceback is available. Please, use an exception with a traceback in the try/except block. "
+                        "Not just called exceptions."
+                    ),
+                    assignee=assignee,
+                )
             return
 
         handled_error = getattr(exception, "handled_error", None)
         if handled_error:
             logger.warning(f"Exception {handled_error} already reported.")
             return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.5/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/config.py` & `t_bug_catcher-0.4.5/t_bug_catcher/config.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.5/t_bug_catcher/jira.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """JiraPoster class for interacting with the Jira API."""
 
 import hashlib
 import json
+import linecache
 import os
 import re
 import sys
 import traceback
 from datetime import datetime
 from importlib.metadata import version
 from pathlib import Path
@@ -372,14 +373,50 @@
                         ],
                     },
                 ],
             }
         ]
 
     @staticmethod
+    def __warning_markup(warning_message: str, message: str) -> List[dict]:
+        """Create the error string markup.
+
+        Args:
+            warning_message (str): The warning message.
+
+        Returns:
+            dict: The error string markup.
+        """
+        return [
+            {
+                "type": "panel",
+                "attrs": {"panelType": "warning"},
+                "content": [
+                    {
+                        "type": "paragraph",
+                        "content": [
+                            {
+                                "type": "text",
+                                "text": warning_message,
+                                "marks": [{"type": "code"}],
+                            },
+                        ],
+                    },
+                    {
+                        "type": "paragraph",
+                        "content": [
+                            {"type": "text", "text": "Message: ", "marks": [{"type": "strong"}]},
+                            {"type": "text", "text": message},
+                        ],
+                    },
+                ],
+            }
+        ]
+
+    @staticmethod
     def __date_markup() -> List[dict]:
         """Create the date markup.
 
         Returns:
             dict: The date markup.
         """
         return [
@@ -667,14 +704,41 @@
             + self.__environment_markup()
             + (self.__description_markup(additional_info) if additional_info else [])
             + self.__traceback_markup(exc_traceback_info)
             + (self.__metadata_markup(metadata) if metadata else [])
             + self.__error_markup(error_id),
         }
 
+    def __create_warning_description_markup(
+        self,
+        warning_message: str,
+        message: str,
+        warning_id: str,
+    ) -> dict:
+        """Create a warning description.
+
+        Args:
+            warning_message (str): The warning message.
+            warning_id (str): The warning ID.
+
+        Returns:
+            dict: A dictionary containing the version, type, and content.
+        """
+        return {
+            "version": 1,
+            "type": "doc",
+            "content": []
+            + self.__warning_markup(warning_message, message)
+            + self.__bot_name_markup()
+            + self.__date_markup()
+            + self.__runlink_markup()
+            + self.__environment_markup()
+            + self.__error_markup(warning_id),
+        }
+
     def __create_transtion_markup(self, issue_status: str) -> dict:
         """Create a transition markup.
 
         Args:
             issue_status (str): The status of the Jira issue.
 
         Returns:
@@ -958,14 +1022,63 @@
             for attachment in attachments:
                 if os.path.exists(str(attachment)):
                     self.add_attachment(attachment, ticket_id)
         if self._webhook_url and self._project_key != CONFIG.SUPPORT_BOARD:
             self.move_ticket_to_board(ticket_id)
         return response
 
+    def warning_message(self, summary: str, inspected_frame, message: str, assignee: Optional[str] = None) -> None:
+        """Create a new ticket with warning message.
+
+        Args:
+            summary (str): The summary of the ticket.
+            inspected_frame (frame): The frame of the warning.
+            assignee (str, optional): The assignee of the ticket. Defaults to None.
+
+        Returns:
+            The response from creating the ticket.
+        """
+        if self._project_key == CONFIG.SUPPORT_BOARD and CONFIG.ADMIN_CODE:
+            summary = CONFIG.ADMIN_CODE + " - " + summary
+
+        warning_id, warning_message = self.__generate_warning_id(inspected_frame)
+
+        existing_ticket = self.filter_tickets(
+            all_tickets=self.get_issues()["issues"],
+            error_id=warning_id,
+        )
+        if existing_ticket:
+            self.__update_existing_ticket(
+                existing_ticket=existing_ticket,
+                summary=summary,
+            )
+            return existing_ticket
+
+        assignee_id = None
+        assignee = assignee if assignee else self._default_assignee
+        if assignee:
+            try:
+                assignee_id = self.__get_assignee(assignee)
+            except Exception as ex:
+                logger.info(f"Failed to get assignee {assignee} due to: {ex}")
+
+        description = self.__create_warning_description_markup(
+            warning_message=warning_message,
+            message=message,
+            warning_id=warning_id,
+        )
+        response = self.__create_new_ticket(
+            summary=summary,
+            description=description,
+            assignee_id=assignee_id,
+            labels=["bug_catcher_warning"],
+        )
+
+        return response
+
     def report_error(
         self,
         exception: Optional[Exception] = None,
         assignee: Optional[str] = None,
         attachments: Union[List, str, Path, None] = None,
         stack_trace: Optional[str] = None,
         metadata: Optional[dict] = None,
@@ -1267,14 +1380,34 @@
         frames = get_frames(exc_traceback)
         exception_chain = "-".join([f"{frame.name}" for frame in frames])
         rel_path = os.path.relpath(frames[-1].filename, os.getcwd())
         path = Path(os.path.splitext(rel_path)[0]).as_posix()
         error_id = f"{path}-{exception_chain}-{frames[-1].line}-" f"{exc_type.__module__}-{exc_type.__name__}"
         return hashlib.md5(error_id.encode()).hexdigest()
 
+    @staticmethod
+    def __generate_warning_id(inspected_frame) -> tuple:
+        """Generates an error string ID using the exception, function name, and error string.
+
+        Args:
+            inspected_frame (frame): The frame of the warning.
+
+        Returns:
+            tuple: The generated error string ID and the warning message.
+        """
+        lineno = inspected_frame.f_lineno
+        filename = inspected_frame.f_code.co_filename
+        func = inspected_frame.f_code.co_name
+        line = linecache.getline(filename, lineno).strip()
+        rel_path = os.path.relpath(filename, os.getcwd())
+
+        warning_message = f"{line}\n{rel_path}:{func}:{lineno}"
+        warning_id = hashlib.md5(f"{filename}-{lineno}-{func}-{line}".encode()).hexdigest()
+        return warning_id, warning_message
+
     def __get_assignee(self, assignee: str) -> str:
         """Get assignee Jira user by ID.
 
         Args:
             assignee (str): The ID of the assignee.
 
         Returns:
```

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/resources/whispers_config.yml` & `t_bug_catcher-0.4.5/t_bug_catcher/resources/whispers_config.yml`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.4.5/t_bug_catcher/stack_saver.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/utils/common.py` & `t_bug_catcher-0.4.5/t_bug_catcher/utils/common.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.5/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.5/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.4
+Version: 0.4.5
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.4/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.5/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.4/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.5/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

