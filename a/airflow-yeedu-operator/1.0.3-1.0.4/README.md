# Comparing `tmp/airflow-yeedu-operator-1.0.3.tar.gz` & `tmp/airflow-yeedu-operator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-yeedu-operator-1.0.3.tar", last modified: Fri Mar 15 08:12:04 2024, max compression
+gzip compressed data, was "airflow-yeedu-operator-1.0.4.tar", last modified: Fri Apr 19 08:14:34 2024, max compression
```

## Comparing `airflow-yeedu-operator-1.0.3.tar` & `airflow-yeedu-operator-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-03-15 08:12:04.613268 airflow-yeedu-operator-1.0.3/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    11357 2024-03-15 08:06:04.000000 airflow-yeedu-operator-1.0.3/LICENSE
--rw-r--r--   0 rk0601    (1001) rk0601    (1001)     2763 2024-03-15 08:12:04.613268 airflow-yeedu-operator-1.0.3/PKG-INFO
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     2338 2024-03-15 08:06:04.000000 airflow-yeedu-operator-1.0.3/README.md
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-03-15 08:12:04.613268 airflow-yeedu-operator-1.0.3/airflow_yeedu_operator.egg-info/
--rw-r--r--   0 rk0601    (1001) rk0601    (1001)     2763 2024-03-15 08:12:04.000000 airflow-yeedu-operator-1.0.3/airflow_yeedu_operator.egg-info/PKG-INFO
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      371 2024-03-15 08:12:04.000000 airflow-yeedu-operator-1.0.3/airflow_yeedu_operator.egg-info/SOURCES.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        1 2024-03-15 08:12:04.000000 airflow-yeedu-operator-1.0.3/airflow_yeedu_operator.egg-info/dependency_links.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       37 2024-03-15 08:12:04.000000 airflow-yeedu-operator-1.0.3/airflow_yeedu_operator.egg-info/requires.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        6 2024-03-15 08:12:04.000000 airflow-yeedu-operator-1.0.3/airflow_yeedu_operator.egg-info/top_level.txt
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       38 2024-03-15 08:12:04.613268 airflow-yeedu-operator-1.0.3/setup.cfg
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      777 2024-03-15 08:11:37.000000 airflow-yeedu-operator-1.0.3/setup.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-03-15 08:12:04.613268 airflow-yeedu-operator-1.0.3/yeedu/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-03-15 08:06:04.000000 airflow-yeedu-operator-1.0.3/yeedu/__init__.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-03-15 08:12:04.613268 airflow-yeedu-operator-1.0.3/yeedu/hooks/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-03-15 08:06:04.000000 airflow-yeedu-operator-1.0.3/yeedu/hooks/__init__.py
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     6488 2024-03-15 08:09:52.000000 airflow-yeedu-operator-1.0.3/yeedu/hooks/yeedu.py
-drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-03-15 08:12:04.613268 airflow-yeedu-operator-1.0.3/yeedu/operators/
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-03-15 08:06:04.000000 airflow-yeedu-operator-1.0.3/yeedu/operators/__init__.py
--rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     4137 2024-03-15 08:06:04.000000 airflow-yeedu-operator-1.0.3/yeedu/operators/yeedu.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-19 08:14:34.211357 airflow-yeedu-operator-1.0.4/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    11357 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.4/LICENSE
+-rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-19 08:14:34.211357 airflow-yeedu-operator-1.0.4/PKG-INFO
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     2647 2024-04-19 08:12:22.000000 airflow-yeedu-operator-1.0.4/README.md
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-19 08:14:34.211357 airflow-yeedu-operator-1.0.4/airflow_yeedu_operator.egg-info/
+-rw-r--r--   0 rk0601    (1001) rk0601    (1001)     3072 2024-04-19 08:14:34.000000 airflow-yeedu-operator-1.0.4/airflow_yeedu_operator.egg-info/PKG-INFO
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      371 2024-04-19 08:14:34.000000 airflow-yeedu-operator-1.0.4/airflow_yeedu_operator.egg-info/SOURCES.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        1 2024-04-19 08:14:34.000000 airflow-yeedu-operator-1.0.4/airflow_yeedu_operator.egg-info/dependency_links.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       37 2024-04-19 08:14:34.000000 airflow-yeedu-operator-1.0.4/airflow_yeedu_operator.egg-info/requires.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)        6 2024-04-19 08:14:34.000000 airflow-yeedu-operator-1.0.4/airflow_yeedu_operator.egg-info/top_level.txt
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)       38 2024-04-19 08:14:34.211357 airflow-yeedu-operator-1.0.4/setup.cfg
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      777 2024-04-17 12:43:19.000000 airflow-yeedu-operator-1.0.4/setup.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-19 08:14:34.211357 airflow-yeedu-operator-1.0.4/yeedu/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.4/yeedu/__init__.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-19 08:14:34.211357 airflow-yeedu-operator-1.0.4/yeedu/hooks/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.4/yeedu/hooks/__init__.py
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)     9499 2024-04-17 12:36:38.000000 airflow-yeedu-operator-1.0.4/yeedu/hooks/yeedu.py
+drwxrwxr-x   0 rk0601    (1001) rk0601    (1001)        0 2024-04-19 08:14:34.211357 airflow-yeedu-operator-1.0.4/yeedu/operators/
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)      787 2024-04-17 12:36:04.000000 airflow-yeedu-operator-1.0.4/yeedu/operators/__init__.py
+-rw-rw-r--   0 rk0601    (1001) rk0601    (1001)    29182 2024-04-17 12:36:38.000000 airflow-yeedu-operator-1.0.4/yeedu/operators/yeedu.py
```

### Comparing `airflow-yeedu-operator-1.0.3/LICENSE` & `airflow-yeedu-operator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.3/PKG-INFO` & `airflow-yeedu-operator-1.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: airflow-yeedu-operator
-Version: 1.0.3
-Summary: Submission and monitoring of jobs using the Yeedu API in Apache Airflow. 
-Author: Yeedu
-Author-email: yeedu@modak.com
-License: All Rights Reserved
-Project-URL: GitHub, https://github.com/yeedu-io/Apache-Airflow-Operator
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: apache-airflow>=2.5.0
-Requires-Dist: requests>=2.27
-
 # Airflow Yeedu Operator
 [![PyPI version](https://badge.fury.io/py/airflow-yeedu-operator.png)](https://badge.fury.io/py/airflow-yeedu-operator)
 
 ## Installation
 
 To use the Yeedu Operator in your Airflow environment, install it using the following command:
 
@@ -22,33 +9,42 @@
 pip3 install airflow-yeedu-operator
 ```
 
 # DAG: Yeedu Job Execution
 
 ## Overview
 
-The `YeeduJobRunOperator` in this DAG facilitates the submission and monitoring of jobs using the Yeedu API in Apache Airflow. This DAG enables users to execute Yeedu jobs and handle their completion status and logs seamlessly within their Airflow environment.
+The `YeeduOperator` in this DAG facilitates the submission and monitoring of jobs and notebooks using the Yeedu API in Apache Airflow. This DAG enables users to execute Yeedu jobs and handle their completion status and logs seamlessly within their Airflow environment.
 
 ## Prerequisites
 
 Before using this DAG, ensure you have:
 
 - Access to the Yeedu API.
 - Proper configuration of Airflow with required connections and variables (if applicable).
 
+1. Open your shell configuration file (`.bashrc` for Bash).
+2. Add the below lines
+
+   ```bash
+   export YEEDU_SCHEDULER_USER=example@test.com
+   export YEEDU_SCHEDULER_PASSWORD=password
+
+   ```
+
 ## Usage
 
 ### DAG Initialization
 
 Import the necessary modules and instantiate the DAG with required arguments and schedule interval.
 
 ```python
 from datetime import datetime, timedelta
 from airflow import DAG
-from yeedu.operators.yeedu import YeeduJobRunOperator
+from yeedu.operators.yeedu import YeeduOperator
 
 # Define DAG arguments
 default_args = {
     'owner': 'airflow',
     'depends_on_past': False,
     'start_date': datetime(2023, 1, 1),
     'retries': 1,
@@ -62,29 +58,33 @@
     description='DAG to execute jobs using Yeedu API',
     schedule_interval='@once',
     catchup=False,
 )
 ```
 ### Task Initialization
 
-Create tasks using `YeeduJobRunOperator` to perform various Yeedu API operations.
-# Define YeeduJobRunOperator tasks
+Create tasks using `YeeduOperator` to perform various Yeedu API operations.
+# Define YeeduOperator tasks
 
 ```python
-    submit_job_task = YeeduJobRunOperator(
-    task_id='submit_yeedu_job',
-    job_conf_id='your_job_config_id',  # Replace with your job config ID
-    token='your_yeedu_api_token',  # Replace with your Yeedu API token
-    hostname='yeedu.example.com',  # Replace with your Yeedu API hostname
-    workspace_id=123,  # Replace with your Yeedu workspace ID
-    dag=dag,
-)
+
+    submit_job_task = YeeduOperator(
+        task_id='demo_dag',
+        conf_id='config_id',  # Replace with your job config ID or Notebook Config ID
+        tenant_id='tenant_id',  # Replace with your Yeedu tenant_id
+        base_url='http://hostname:8080/api/v1/',  # Replace with your Yeedu API URL
+        workspace_id='your_workspace_id',  # Replace with your Yeedu workspace ID
+        dag=dag,
+    )
+
 ```
 ### Execution
 
 To execute this DAG:
 
-1. Ensure all required configurations (job config ID, API token, hostname, workspace ID) are correctly provided in the task definitions.
+1. Ensure all required configurations (config ID, API URL, tenant ID, workspace ID) are correctly provided in the task definitions,
+and YEEDU_SCHEDULER_USER, YEEDU_SCHEDULER_PASSWORD are added as Environment Variables.
 2. Place the DAG file in the appropriate Airflow DAGs folder.
 3. Trigger the DAG manually or based on the defined schedule interval.
 4. Monitor the Airflow UI for task execution and logs.
 
+
```

### Comparing `airflow-yeedu-operator-1.0.3/airflow_yeedu_operator.egg-info/PKG-INFO` & `airflow-yeedu-operator-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-yeedu-operator
-Version: 1.0.3
+Version: 1.0.4
 Summary: Submission and monitoring of jobs using the Yeedu API in Apache Airflow. 
 Author: Yeedu
 Author-email: yeedu@modak.com
 License: All Rights Reserved
 Project-URL: GitHub, https://github.com/yeedu-io/Apache-Airflow-Operator
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,33 +22,42 @@
 pip3 install airflow-yeedu-operator
 ```
 
 # DAG: Yeedu Job Execution
 
 ## Overview
 
-The `YeeduJobRunOperator` in this DAG facilitates the submission and monitoring of jobs using the Yeedu API in Apache Airflow. This DAG enables users to execute Yeedu jobs and handle their completion status and logs seamlessly within their Airflow environment.
+The `YeeduOperator` in this DAG facilitates the submission and monitoring of jobs and notebooks using the Yeedu API in Apache Airflow. This DAG enables users to execute Yeedu jobs and handle their completion status and logs seamlessly within their Airflow environment.
 
 ## Prerequisites
 
 Before using this DAG, ensure you have:
 
 - Access to the Yeedu API.
 - Proper configuration of Airflow with required connections and variables (if applicable).
 
+1. Open your shell configuration file (`.bashrc` for Bash).
+2. Add the below lines
+
+   ```bash
+   export YEEDU_SCHEDULER_USER=example@test.com
+   export YEEDU_SCHEDULER_PASSWORD=password
+
+   ```
+
 ## Usage
 
 ### DAG Initialization
 
 Import the necessary modules and instantiate the DAG with required arguments and schedule interval.
 
 ```python
 from datetime import datetime, timedelta
 from airflow import DAG
-from yeedu.operators.yeedu import YeeduJobRunOperator
+from yeedu.operators.yeedu import YeeduOperator
 
 # Define DAG arguments
 default_args = {
     'owner': 'airflow',
     'depends_on_past': False,
     'start_date': datetime(2023, 1, 1),
     'retries': 1,
@@ -62,29 +71,33 @@
     description='DAG to execute jobs using Yeedu API',
     schedule_interval='@once',
     catchup=False,
 )
 ```
 ### Task Initialization
 
-Create tasks using `YeeduJobRunOperator` to perform various Yeedu API operations.
-# Define YeeduJobRunOperator tasks
+Create tasks using `YeeduOperator` to perform various Yeedu API operations.
+# Define YeeduOperator tasks
 
 ```python
-    submit_job_task = YeeduJobRunOperator(
-    task_id='submit_yeedu_job',
-    job_conf_id='your_job_config_id',  # Replace with your job config ID
-    token='your_yeedu_api_token',  # Replace with your Yeedu API token
-    hostname='yeedu.example.com',  # Replace with your Yeedu API hostname
-    workspace_id=123,  # Replace with your Yeedu workspace ID
-    dag=dag,
-)
+
+    submit_job_task = YeeduOperator(
+        task_id='demo_dag',
+        conf_id='config_id',  # Replace with your job config ID or Notebook Config ID
+        tenant_id='tenant_id',  # Replace with your Yeedu tenant_id
+        base_url='http://hostname:8080/api/v1/',  # Replace with your Yeedu API URL
+        workspace_id='your_workspace_id',  # Replace with your Yeedu workspace ID
+        dag=dag,
+    )
+
 ```
 ### Execution
 
 To execute this DAG:
 
-1. Ensure all required configurations (job config ID, API token, hostname, workspace ID) are correctly provided in the task definitions.
+1. Ensure all required configurations (config ID, API URL, tenant ID, workspace ID) are correctly provided in the task definitions,
+and YEEDU_SCHEDULER_USER, YEEDU_SCHEDULER_PASSWORD are added as Environment Variables.
 2. Place the DAG file in the appropriate Airflow DAGs folder.
 3. Trigger the DAG manually or based on the defined schedule interval.
 4. Monitor the Airflow UI for task execution and logs.
 
+
```

### Comparing `airflow-yeedu-operator-1.0.3/setup.py` & `airflow-yeedu-operator-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def read(*parts):
     return codecs.open(os.path.join(here, *parts), 'r').read()
 
 
 setup(
     name='airflow-yeedu-operator',
-    version='1.0.3',
+    version='1.0.4',
     description='Submission and monitoring of jobs using the Yeedu API in Apache Airflow. ',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='Yeedu',
     author_email='yeedu@modak.com',
     packages=find_packages(),
     install_requires=[
```

### Comparing `airflow-yeedu-operator-1.0.3/yeedu/__init__.py` & `airflow-yeedu-operator-1.0.4/yeedu/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.3/yeedu/hooks/__init__.py` & `airflow-yeedu-operator-1.0.4/yeedu/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-yeedu-operator-1.0.3/yeedu/hooks/yeedu.py` & `airflow-yeedu-operator-1.0.4/yeedu/hooks/yeedu.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,14 +24,27 @@
 
 import requests
 import time
 import logging
 from typing import Tuple
 from airflow.hooks.base import BaseHook
 from airflow.exceptions import AirflowException
+from typing import Optional, Dict
+import json
+import os
+
+
+
+YEEDU_SCHEDULER_USER = os.getenv("YEEDU_SCHEDULER_USER")
+YEEDU_SCHEDULER_PASSWORD = os.getenv("YEEDU_SCHEDULER_PASSWORD")
+
+headers: dict = {
+            'accept': 'application/json',
+            'Content-Type': 'application/json'
+        }
 
 class YeeduHook(BaseHook):
     """
     YeeduHook provides an interface to interact with the Yeedu API.
 
     :param token: Yeedu API token.
     :type token: str
@@ -39,61 +52,117 @@
     :type hostname: str
     :param workspace_id: The ID of the Yeedu workspace.
     :type workspace_id: int
     :param args: Additional positional arguments.
     :param kwargs: Additional keyword arguments.
     """
 
-    def __init__(self, token: str, hostname: str, workspace_id: int, *args, **kwargs) -> None:
+    def __init__(self, conf_id: int, tenant_id: str, base_url: str, workspace_id: int, *args, **kwargs) -> None:
         """
         Initializes YeeduHook with the necessary configurations to communicate with the Yeedu API.
 
-        :param token: Yeedu API token.
-        :param hostname: Yeedu API hostname.
+        :param tenant_id: Yeedu API tenant_id.
+        :param base_url: Yeedu API base_url.
         :param workspace_id: The ID of the Yeedu workspace.
         """
 
         super().__init__(*args, **kwargs)
-        self.token: str = token
-        self.headers: dict = {
-            'accept': 'application/json',
-            'Authorization': f"Bearer {token}",
-            'Content-Type': 'application/json'
-        }
-        self.base_url: str = f'http://{hostname}/api/v1/workspace/{workspace_id}/'
+        self.tenant_id: str = tenant_id
+        self.conf_id = conf_id
+        self.workspace_id = workspace_id
+        self.base_url: str = base_url
 
-    def _api_request(self, method: str, url: str, data=None) -> requests.Response:
+    def _api_request(self, method: str, url: str, data=None, params: Optional[Dict] = None) -> requests.Response:
         """
         Makes an HTTP request to the Yeedu API.
 
         :param method: The HTTP method (GET, POST, etc.).
         :param url: The URL of the API endpoint.
         :param data: The JSON data for the request.
         :return: The API response.
         """
 
         try:
-            response: requests.Response = requests.request(method, url, headers=self.headers, json=data)
+            response: requests.Response = requests.request(method, url, headers=headers, json=data, params=params)
             return response
                         
         except Exception as e:
             raise AirflowException(e)
             
 
+    def yeedu_login(self):
+        try:
+            login_url = self.base_url+'login'
+            data = {
+                    "username": f"{YEEDU_SCHEDULER_USER}",
+                    "password": f"{YEEDU_SCHEDULER_PASSWORD}"
+                }
+            # self.log.info(f"{data},{YEEDU_SCHEDULER_USER},{YEEDU_SCHEDULER_PASSWORD}")
+            login_response = self._api_request('POST',login_url,data)
+
+            if login_response.status_code == 200:
+                self.log.info(
+                    f'Login successful. Token: {login_response.json().get("token")}')
+                headers['Authorization'] = f"Bearer {login_response.json().get('token')}"
+                self.associate_tenant()
+                return login_response.json().get('token')
+            else:
+                raise AirflowException(login_response.text)
+        except Exception as e:
+            self.log.info(f"An error occurred during yeedu_login: {e}")
+            raise AirflowException(e)
+
+    def associate_tenant(self):
+        try:
+            # Construct the tenant URL
+            tenant_url = self.base_url+f'user/select/{self.tenant_id}'
+
+            # Make the POST request to associate the tenant
+            tenant_associate_response = self._api_request('POST',tenant_url)
 
+            if tenant_associate_response.status_code == 201:
+                self.log.info(
+                    f'Tenant associated successfully. Status Code: {tenant_associate_response.status_code}')
+                self.log.info(
+                    f'Tenant Association Response: {tenant_associate_response.json()}')
+                return 0
+            else:
+                raise AirflowException(tenant_associate_response.text)
+        except Exception as e:
+            self.log.info(f"An error occurred during associate_tenant: {e}")
+            raise AirflowException(e)  
+        
+    def get_job_type(self):
+
+        # URL for notebook configuration API
+        notebook_url = self.base_url + f'workspace/{self.workspace_id}/notebook/conf?notebook_conf_id={self.conf_id}'
+        response_notebook = self._api_request('GET',notebook_url)
+        # self.log.info("notebookresponse",response_notebook.json())
+        # URL for job configuration API
+        job_url = self.base_url + f'workspace/{self.workspace_id}/spark/job/conf?job_conf_id={self.conf_id}'
+        response_job = self._api_request('GET',job_url)
+        # self.log.info(response_job.json())
+        # Check status codes and return job type
+        if response_notebook.status_code == 200:
+            return 'notebook'
+        elif response_job.status_code == 200:
+            return 'job'
+        else:
+            return None
+        
     def submit_job(self, job_conf_id: str) -> int:
         """
         Submits a job to Yeedu.
 
         :param job_conf_id: The job configuration ID.
         :return: The ID of the submitted job.
         """
 
         try:
-            job_url: str = self.base_url + 'spark/job'
+            job_url: str = self.base_url + f'workspace/{self.workspace_id}/spark/job'
             data: dict = {'job_conf_id': job_conf_id}
             response = self._api_request('POST', job_url, data)
             api_status_code = response.status_code
             response_json = response.json()
             if api_status_code == 200:
                 job_id = response.json().get('job_id')
                 if job_id:
@@ -113,15 +182,15 @@
         Retrieves the status of a Yeedu job.
 
         :param job_id: The ID of the job.
         :return: The API response containing job status.
         """
 
         try:
-            job_status_url: str = self.base_url + f'spark/job/{job_id}'
+            job_status_url: str = self.base_url + f'workspace/{self.workspace_id}/spark/job/{job_id}'
             return self._api_request('GET', job_status_url)
                         
         except Exception as e:
             raise AirflowException(e)
 
             
 
@@ -131,15 +200,15 @@
 
         :param job_id: The ID of the job.
         :param log_type: The type of logs to retrieve ('stdout' or 'stderr').
         :return: The logs for the specified job and log type.
         """
 
         try:
-            logs_url: str = self.base_url + f'spark/job/{job_id}/log/{log_type}'
+            logs_url: str = self.base_url + f'workspace/{self.workspace_id}/spark/job/{job_id}/log/{log_type}'
             time.sleep(30)
             return self._api_request('GET', logs_url).text
         
         except Exception as e:
             raise AirflowException(e)
             
 
@@ -177,8 +246,9 @@
                 # If continuous failures reach the threshold, throw an error
                 if attempts_failure == max_attempts:
                     raise AirflowException("Continuous API failure reached the threshold")
 
             return job_status
         
         except Exception as e:
-            raise AirflowException(e)
+            raise AirflowException(e)
+
```

### Comparing `airflow-yeedu-operator-1.0.3/yeedu/operators/__init__.py` & `airflow-yeedu-operator-1.0.4/yeedu/operators/__init__.py`

 * *Files identical despite different names*

