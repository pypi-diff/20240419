# Comparing `tmp/activecollab-3.tar.gz` & `tmp/activecollab-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activecollab-3.tar", last modified: Mon Apr 15 10:18:08 2024, max compression
+gzip compressed data, was "activecollab-3.1.tar", last modified: Fri Apr 19 05:52:10 2024, max compression
```

## Comparing `activecollab-3.tar` & `activecollab-3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:18:08.344722 activecollab-3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:18:08.340722 activecollab-3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:18:08.344722 activecollab-3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-15 10:17:58.000000 activecollab-3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 10:17:58.000000 activecollab-3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:18:08.344722 activecollab-3/ActiveCollab/
--rw-r--r--   0 runner    (1001) docker     (127)    13031 2024-04-15 10:17:58.000000 activecollab-3/ActiveCollab/ActiveCollab.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 10:17:58.000000 activecollab-3/ActiveCollab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:18:08.344722 activecollab-3/ActiveCollab/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-15 10:17:58.000000 activecollab-3/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:18:08.344722 activecollab-3/ActiveCollab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-15 10:18:08.000000 activecollab-3/ActiveCollab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-15 10:18:08.000000 activecollab-3/ActiveCollab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:18:08.000000 activecollab-3/ActiveCollab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 10:18:08.000000 activecollab-3/ActiveCollab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 10:18:08.000000 activecollab-3/ActiveCollab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 10:17:58.000000 activecollab-3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-15 10:18:08.344722 activecollab-3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-15 10:17:58.000000 activecollab-3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-15 10:17:58.000000 activecollab-3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:18:08.344722 activecollab-3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-15 10:17:58.000000 activecollab-3/setup.py_bck
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 05:52:05.000000 activecollab-3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 05:52:05.000000 activecollab-3.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/ActiveCollab/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-19 05:52:05.000000 activecollab-3.1/ActiveCollab/ActiveCollab.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 05:52:05.000000 activecollab-3.1/ActiveCollab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/ActiveCollab/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-19 05:52:05.000000 activecollab-3.1/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:52:10.768946 activecollab-3.1/ActiveCollab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 05:52:10.000000 activecollab-3.1/ActiveCollab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 05:52:05.000000 activecollab-3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 05:52:10.768946 activecollab-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 05:52:05.000000 activecollab-3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-19 05:52:05.000000 activecollab-3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:52:10.768946 activecollab-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 05:52:05.000000 activecollab-3.1/setup.py_bck
```

### Comparing `activecollab-3/.github/workflows/publish.yml` & `activecollab-3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `activecollab-3/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc` & `activecollab-3.1/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `activecollab-3/ActiveCollab.egg-info/PKG-INFO` & `activecollab-3.1/ActiveCollab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,71 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 3
-Summary: A Python module to interact with ActiveCollab and perform certain actions
+Version: 3.1
+Summary: A python library working with activeCollab
 Author-email: Ankushtpss <ankushkumartpss@gmail.com>
 Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
 Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
-Keywords: ActiveCollab,Active Collab,active collab
+Keywords: Active Collab,ActiveCollab,Active Collab SDK,active collab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: selenium
-Requires-Dist: webdriver_manager
+Requires-Dist: requests
+Requires-Dist: sys
 
 # ActiveCollab
 
 ## Overview
-This project aims to build a headless interaction with your active collab using Selenium WebDriver.
-
+Library for Active Collab. Perform actions such as list projects, list users, add note, add task, get project detail.
 
 ## Download stats
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab) <br>
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab/week)](https://pepy.tech/project/ActiveCollab) <br>
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab/month)](https://pepy.tech/project/ActiveCollab)
-
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab)
 
 ## Installation
-
 ```console
 pip install ActiveCollab
 ```
-ActiveCollab officially supports Python 3.8+.
+ActiveCollab supports Python 3+.
 
 ## Usage
 
 ### Default
 ```python
 import ActiveCollab
 
 host_url = 'host_url' # Active Collab hosted URL  
 
-user_name = 'your_username_or_email' # Active Collab username or email
+user_name = 'your_email' # Active Collab username or email
 
 password = 'your_password' # Active Collab Password
 
 ac = ActiveCollab.Connect(host_url,user_name,password)  # Login to Active Collab
 ```
 
-
-
 ### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
 ### List all users
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
 ### List Users in a Project
 ```python
-ac.list_users_in_project(project_id)  # List out all users in the project (project_id)
+ac.project_detail(project_id)  # List out all info like id, name, users/members of a project (project_id)
 ```
 
-### + Add User in a Project
+### + Add Note in a Project
 ```python
-ac.add_user_in_project(project_id,user_name_or_user_email)  # Add user in provided project_id
+ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
 ```
 
-
 ### + Add Task in a Project
 ```python
 ac.add_task_in_project(project_id,task_title,task_description,task_assignee)  # Add task in the provided project_id
 ```
 
-### + Add Note in a Project
-```python
-ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
-```
```

### Comparing `activecollab-3/LICENSE` & `activecollab-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `activecollab-3/PKG-INFO` & `activecollab-3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,71 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 3
-Summary: A Python module to interact with ActiveCollab and perform certain actions
+Version: 3.1
+Summary: A python library working with activeCollab
 Author-email: Ankushtpss <ankushkumartpss@gmail.com>
 Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
 Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
-Keywords: ActiveCollab,Active Collab,active collab
+Keywords: Active Collab,ActiveCollab,Active Collab SDK,active collab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: selenium
-Requires-Dist: webdriver_manager
+Requires-Dist: requests
+Requires-Dist: sys
 
 # ActiveCollab
 
 ## Overview
-This project aims to build a headless interaction with your active collab using Selenium WebDriver.
-
+Library for Active Collab. Perform actions such as list projects, list users, add note, add task, get project detail.
 
 ## Download stats
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab) <br>
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab/week)](https://pepy.tech/project/ActiveCollab) <br>
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab/month)](https://pepy.tech/project/ActiveCollab)
-
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab)
 
 ## Installation
-
 ```console
 pip install ActiveCollab
 ```
-ActiveCollab officially supports Python 3.8+.
+ActiveCollab supports Python 3+.
 
 ## Usage
 
 ### Default
 ```python
 import ActiveCollab
 
 host_url = 'host_url' # Active Collab hosted URL  
 
-user_name = 'your_username_or_email' # Active Collab username or email
+user_name = 'your_email' # Active Collab username or email
 
 password = 'your_password' # Active Collab Password
 
 ac = ActiveCollab.Connect(host_url,user_name,password)  # Login to Active Collab
 ```
 
-
-
 ### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
 ### List all users
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
 ### List Users in a Project
 ```python
-ac.list_users_in_project(project_id)  # List out all users in the project (project_id)
+ac.project_detail(project_id)  # List out all info like id, name, users/members of a project (project_id)
 ```
 
-### + Add User in a Project
+### + Add Note in a Project
 ```python
-ac.add_user_in_project(project_id,user_name_or_user_email)  # Add user in provided project_id
+ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
 ```
 
-
 ### + Add Task in a Project
 ```python
 ac.add_task_in_project(project_id,task_title,task_description,task_assignee)  # Add task in the provided project_id
 ```
 
-### + Add Note in a Project
-```python
-ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
-```
```

### Comparing `activecollab-3/README.md` & `activecollab-3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 # ActiveCollab
 
 ## Overview
-This project aims to build a headless interaction with your active collab using Selenium WebDriver.
-
+Library for Active Collab. Perform actions such as list projects, list users, add note, add task, get project detail.
 
 ## Download stats
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab) <br>
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab/week)](https://pepy.tech/project/ActiveCollab) <br>
-[![Downloads](https://static.pepy.tech/badge/ActiveCollab/month)](https://pepy.tech/project/ActiveCollab)
-
+[![Downloads](https://static.pepy.tech/badge/ActiveCollab)](https://pepy.tech/project/ActiveCollab)
 
 ## Installation
-
 ```console
 pip install ActiveCollab
 ```
-ActiveCollab officially supports Python 3.8+.
+ActiveCollab supports Python 3+.
 
 ## Usage
 
 ### Default
 ```python
 import ActiveCollab
 
 host_url = 'host_url' # Active Collab hosted URL  
 
-user_name = 'your_username_or_email' # Active Collab username or email
+user_name = 'your_email' # Active Collab username or email
 
 password = 'your_password' # Active Collab Password
 
 ac = ActiveCollab.Connect(host_url,user_name,password)  # Login to Active Collab
 ```
 
-
-
 ### List all projects
 ```python
 ac.list_projects()  # List out all project assigned to logged in user
 ```
 
 ### List all users
 ```python
 ac.list_users()  # List out all users in your organization with id, name and email
 ```
 
 ### List Users in a Project
 ```python
-ac.list_users_in_project(project_id)  # List out all users in the project (project_id)
+ac.project_detail(project_id)  # List out all info like id, name, users/members of a project (project_id)
 ```
 
-### + Add User in a Project
+### + Add Note in a Project
 ```python
-ac.add_user_in_project(project_id,user_name_or_user_email)  # Add user in provided project_id
+ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
 ```
 
-
 ### + Add Task in a Project
 ```python
 ac.add_task_in_project(project_id,task_title,task_description,task_assignee)  # Add task in the provided project_id
 ```
 
-### + Add Note in a Project
-```python
-ac.add_note_in_project(project_id,note_title,note_content)  # Add note in the provided project_id
-```
```

### Comparing `activecollab-3/pyproject.toml` & `activecollab-3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "ActiveCollab"
 authors = [
   { name="Ankushtpss", email="ankushkumartpss@gmail.com" },
 ]
-description = "A Python module to interact with ActiveCollab and perform certain actions"
-keywords = ["ActiveCollab", "Active Collab", "active collab"]
+description = "A python library working with activeCollab"
+keywords = ["Active Collab", "ActiveCollab",  "Active Collab SDK", "active collab"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "selenium",
-    "webdriver_manager",
+    "requests",
+    "sys",
 ]
 
-version = "3"
+version = "3.1"
 
 [tool.setuptools_scm]
 
 [project.urls]
 "Homepage" = "https://github.com/Ankushtpss/ActiveCollab"
 "Bug Tracker" = "https://github.com/Ankushtpss/ActiveCollab/issues"
```

### Comparing `activecollab-3/setup.py_bck` & `activecollab-3.1/setup.py_bck`

 * *Files identical despite different names*

