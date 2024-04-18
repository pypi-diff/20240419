# Comparing `tmp/nothion-0.3.0.tar.gz` & `tmp/nothion-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nothion-0.3.0.tar", last modified: Mon Mar 18 18:41:04 2024, max compression
+gzip compressed data, was "nothion-0.3.1.tar", last modified: Thu Apr 18 22:34:16 2024, max compression
```

## Comparing `nothion-0.3.0.tar` & `nothion-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:41:04.925857 nothion-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-18 18:40:57.000000 nothion-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-18 18:41:04.925857 nothion-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-18 18:40:57.000000 nothion-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-18 18:41:02.000000 nothion-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 18:41:04.925857 nothion-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:41:04.921857 nothion-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:41:04.921857 nothion-0.3.0/src/nothion/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/_notion_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/_notion_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/_notion_table_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15011 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/notion_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/personal_stats_model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 18:40:57.000000 nothion-0.3.0/src/nothion/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:41:04.925857 nothion-0.3.0/src/nothion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-18 18:41:04.000000 nothion-0.3.0/src/nothion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-18 18:41:04.000000 nothion-0.3.0/src/nothion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 18:41:04.000000 nothion-0.3.0/src/nothion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-18 18:41:04.000000 nothion-0.3.0/src/nothion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 18:41:04.000000 nothion-0.3.0/src/nothion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:41:04.921857 nothion-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-03-18 18:40:57.000000 nothion-0.3.0/tests/test_notion_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17013 2024-03-18 18:40:57.000000 nothion-0.3.0/tests/test_notion_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:34:16.646259 nothion-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 22:34:08.000000 nothion-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-18 22:34:16.646259 nothion-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 22:34:08.000000 nothion-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 22:34:14.000000 nothion-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 22:34:16.646259 nothion-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:34:16.642259 nothion-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:34:16.646259 nothion-0.3.1/src/nothion/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/_notion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/_notion_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/_notion_table_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15276 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/notion_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/personal_stats_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:34:08.000000 nothion-0.3.1/src/nothion/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:34:16.646259 nothion-0.3.1/src/nothion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-18 22:34:16.000000 nothion-0.3.1/src/nothion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 22:34:16.000000 nothion-0.3.1/src/nothion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:34:16.000000 nothion-0.3.1/src/nothion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 22:34:16.000000 nothion-0.3.1/src/nothion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 22:34:16.000000 nothion-0.3.1/src/nothion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:34:16.646259 nothion-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-18 22:34:08.000000 nothion-0.3.1/tests/test_notion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-04-18 22:34:08.000000 nothion-0.3.1/tests/test_notion_client.py
```

### Comparing `nothion-0.3.0/LICENSE` & `nothion-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nothion-0.3.0/PKG-INFO` & `nothion-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nothion
-Version: 0.3.0
+Version: 0.3.1
 Summary: Yet another unofficial Notion API client.
 Author-email: anggelomos <anggelomos@outlook.com>
 Project-URL: repository, https://github.com/anggelomos/nothion
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nothion-0.3.0/README.md` & `nothion-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nothion-0.3.0/pyproject.toml` & `nothion-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nothion"
-version = "0.3.0"
+version = "0.3.1"
 description = "Yet another unofficial Notion API client."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3.10",]
 dependencies = [ "tickthon", "requests", "attrs",]
 [[project.authors]]
 name = "anggelomos"
```

### Comparing `nothion-0.3.0/src/nothion/_notion_api.py` & `nothion-0.3.1/src/nothion/_notion_api.py`

 * *Files identical despite different names*

### Comparing `nothion-0.3.0/src/nothion/_notion_payloads.py` & `nothion-0.3.1/src/nothion/_notion_payloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         payload = {
             "properties": {
                 TasksHeaders.DONE.value: {"checkbox": task.status != 0},
                 "title": {"title": [{"text": {"content": task.title}}]},
                 TasksHeaders.FOCUS_TIME.value: {"number": task.focus_time},
                 TasksHeaders.TAGS.value: {"multi_select": list(map(lambda tag: {"name": tag}, task.tags))},
                 TasksHeaders.TICKTICK_ID.value: {"rich_text": [{"text": {"content": task.ticktick_id}}]},
+                TasksHeaders.COLUMN_ID.value: {"rich_text": [{"text": {"content": task.column_id}}]},
                 TasksHeaders.PROJECT_ID.value: {"rich_text": [{"text": {"content": task.project_id}}]},
                 TasksHeaders.TICKTICK_ETAG.value: {"rich_text": [{"text": {"content": task.ticktick_etag}}]},
                 TasksHeaders.CREATED_DATE.value: {"date": {"start": task.created_date}},
                 TasksHeaders.TIMEZONE.value: {"rich_text": [{"text": {"content": task.timezone}}]},
             }
         }
```

### Comparing `nothion-0.3.0/src/nothion/_notion_table_headers.py` & `nothion-0.3.1/src/nothion/_notion_table_headers.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     DONE = "Done"
     NOTE = "Note"
     FOCUS_TIME = "Focus time"
     DUE_DATE = "Due date"
     CREATED_DATE = "Created date"
     TAGS = "Tags"
     TICKTICK_ID = "Ticktick id"
+    COLUMN_ID = "Column id"
     TICKTICK_ETAG = "Ticktick etag"
     PROJECT_ID = "Project id"
     TIMEZONE = "Timezone"
 
 
 class StatsHeaders(Enum):
     COMPLETED = "completed"
```

### Comparing `nothion-0.3.0/src/nothion/notion_client.py` & `nothion-0.3.1/src/nothion/notion_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,23 @@
             if task_properties[TasksHeaders.CREATED_DATE.value]["date"]:
                 created_date = task_properties[TasksHeaders.CREATED_DATE.value]["date"]["start"]
 
             project_id = ""
             if task_properties[TasksHeaders.PROJECT_ID.value]["rich_text"]:
                 project_id = task_properties[TasksHeaders.PROJECT_ID.value]["rich_text"][0]["plain_text"]
 
+            column_id = ""
+            if task_properties[TasksHeaders.COLUMN_ID.value]["rich_text"]:
+                column_id = task_properties[TasksHeaders.COLUMN_ID.value]["rich_text"][0]["plain_text"]
+
             parsed_tasks.append(Task(title=task_properties[TasksHeaders.NOTE.value]["title"][0]["plain_text"],
                                      status=2 if task_properties[TasksHeaders.DONE.value]["checkbox"] else 0,
                                      ticktick_id=task_properties[TasksHeaders.TICKTICK_ID.value]
                                      ["rich_text"][0]["plain_text"],
+                                     column_id=column_id,
                                      ticktick_etag=task_properties[TasksHeaders.TICKTICK_ETAG.value]
                                      ["rich_text"][0]["plain_text"],
                                      created_date=created_date,
                                      focus_time=task_properties[TasksHeaders.FOCUS_TIME.value]["number"],
                                      deleted=int(raw_task["archived"]),
                                      tags=tuple([tag["name"] for tag in task_properties[TasksHeaders.TAGS.value]
                                                                                        ["multi_select"]]),
```

### Comparing `nothion-0.3.0/src/nothion.egg-info/PKG-INFO` & `nothion-0.3.1/src/nothion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nothion
-Version: 0.3.0
+Version: 0.3.1
 Summary: Yet another unofficial Notion API client.
 Author-email: anggelomos <anggelomos@outlook.com>
 Project-URL: repository, https://github.com/anggelomos/nothion
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nothion-0.3.0/tests/test_notion_api.py` & `nothion-0.3.1/tests/test_notion_api.py`

 * *Files identical despite different names*

### Comparing `nothion-0.3.0/tests/test_notion_client.py` & `nothion-0.3.1/tests/test_notion_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
     assert updated_task.title == original_task.title
     assert updated_task.focus_time != original_task.focus_time
 
 
 def test_create_task_note(notion_client):
     task_id = uuid4().hex
     expected_task = Task(ticktick_id=task_id,
+                         column_id="test-column-id",
                          ticktick_etag="created-task-note-to-delete",
                          created_date="9999-09-09",
                          status=0,
                          title="Test Task Note to Delete",
                          focus_time=0.9,
                          tags=("test", "existing", "delete", "unprocessed"),
                          project_id="a123a4b5c6d7e8f9a0b1c2d3s4h",
```

