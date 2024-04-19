# Comparing `tmp/drumpler_mammoth-2.1.3.tar.gz` & `tmp/drumpler_mammoth-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler_mammoth-2.1.3.tar", last modified: Wed Apr 17 19:48:17 2024, max compression
+gzip compressed data, was "drumpler_mammoth-2.1.4.tar", last modified: Fri Apr 19 15:28:28 2024, max compression
```

## Comparing `drumpler_mammoth-2.1.3.tar` & `drumpler_mammoth-2.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:48:17.045491 drumpler_mammoth-2.1.3/
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.1.3/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 19:48:17.044554 drumpler_mammoth-2.1.3/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.1.3/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:48:17.040599 drumpler_mammoth-2.1.3/drumpler_mammoth/
--rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.1.3/drumpler_mammoth/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)     1959 2024-04-17 19:48:08.000000 drumpler_mammoth-2.1.3/drumpler_mammoth/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     5973 2024-04-17 19:46:23.000000 drumpler_mammoth-2.1.3/drumpler_mammoth/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)      938 2024-04-17 16:38:09.000000 drumpler_mammoth-2.1.3/drumpler_mammoth/mylogger.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:48:17.043784 drumpler_mammoth-2.1.3/drumpler_mammoth.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 19:48:17.000000 drumpler_mammoth-2.1.3/drumpler_mammoth.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      344 2024-04-17 19:48:17.000000 drumpler_mammoth-2.1.3/drumpler_mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 19:48:17.000000 drumpler_mammoth-2.1.3/drumpler_mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       23 2024-04-17 19:48:17.000000 drumpler_mammoth-2.1.3/drumpler_mammoth.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-17 19:48:17.000000 drumpler_mammoth-2.1.3/drumpler_mammoth.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 19:48:17.045670 drumpler_mammoth-2.1.3/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      725 2024-04-17 19:48:12.000000 drumpler_mammoth-2.1.3/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-19 15:28:28.365171 drumpler_mammoth-2.1.4/
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-18 20:05:31.000000 drumpler_mammoth-2.1.4/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     5716 2024-04-19 15:28:28.364522 drumpler_mammoth-2.1.4/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     5171 2024-04-18 20:13:32.000000 drumpler_mammoth-2.1.4/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-19 15:28:28.361153 drumpler_mammoth-2.1.4/drumpler_mammoth/
+-rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-18 20:05:31.000000 drumpler_mammoth-2.1.4/drumpler_mammoth/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)     1943 2024-04-19 15:25:52.000000 drumpler_mammoth-2.1.4/drumpler_mammoth/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6043 2024-04-19 15:25:52.000000 drumpler_mammoth-2.1.4/drumpler_mammoth/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)      938 2024-04-19 15:25:52.000000 drumpler_mammoth-2.1.4/drumpler_mammoth/mylogger.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-19 15:28:28.363842 drumpler_mammoth-2.1.4/drumpler_mammoth.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     5716 2024-04-19 15:28:28.000000 drumpler_mammoth-2.1.4/drumpler_mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      344 2024-04-19 15:28:28.000000 drumpler_mammoth-2.1.4/drumpler_mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-19 15:28:28.000000 drumpler_mammoth-2.1.4/drumpler_mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       23 2024-04-19 15:28:28.000000 drumpler_mammoth-2.1.4/drumpler_mammoth.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-19 15:28:28.000000 drumpler_mammoth-2.1.4/drumpler_mammoth.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-19 15:28:28.365332 drumpler_mammoth-2.1.4/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      725 2024-04-19 15:26:16.000000 drumpler_mammoth-2.1.4/setup.py
```

### Comparing `drumpler_mammoth-2.1.3/LICENSE` & `drumpler_mammoth-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.3/drumpler_mammoth/http_request.py` & `drumpler_mammoth-2.1.4/drumpler_mammoth/http_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-import requests
 import json
 
 class HttpRequest:
     def __init__(self, id, job_id, source_ip, user_agent, method, request_url, request_raw, custom_value):
         self.id = id
         self.job_id = job_id
         self.source_ip = source_ip
         self.user_agent = user_agent
         self.method = method
         self.request_url = request_url
         self.custom_value = custom_value
 
         # Ensure request_raw is correctly handled
         if isinstance(request_raw, str):
-            self.request_json = json.loads(request_raw)
+            self.request_dict = json.loads(request_raw)
         elif isinstance(request_raw, dict):
-            self.request_json = request_raw
+            self.request_dict = request_raw
         else:
             raise ValueError("request_raw must be either a JSON string or a dictionary")
 
     @property
     def id(self):
         return self._id
```

### Comparing `drumpler_mammoth-2.1.3/drumpler_mammoth/mammoth.py` & `drumpler_mammoth-2.1.4/drumpler_mammoth/mammoth.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,20 @@
                     source_ip=data['source_ip'],
                     user_agent=data['user_agent'],
                     method=data['method'],
                     request_url=data['request_url'],
                     request_raw=json.loads(data['request_raw']),
                     custom_value=data['custom_value']
                 )
+            elif response.status_code == 404:
+                self.logger.info("No pending jobs found.")
+                return None
             else:
-                self.logger.error(f"Failed to fetch next pending job: {response.status_code} - {response.text}")
+                print(response.status_code, response.text)
+                self.logger.error(f"Error occured: {response.status_code} - {response.text}")
                 return None
         except requests.ConnectionError as e:
             self.logger.error(f"Network problem occurred: {str(e)}")
             return None
         except requests.Timeout as e:
             self.logger.error(f"Request timed out: {str(e)}")
             return None
@@ -64,29 +68,25 @@
         
     def insert_event(self, job_id, message):
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         event_data = {
             "job_id": job_id,
             "message": message
         }
-        response = requests.post(f"{self.drumpler_url}/events", json=event_data, headers=headers)
-        if response.status_code == 201:
-            print(f"Event logged successfully for job {job_id}")
-        else:
+        response = requests.post(f"{self.drumpler_url}/jobs/{job_id}/insert-event", json=event_data, headers=headers)
+        if response.status_code != 200:
             print(f"Failed to log event for job {job_id}: {response.status_code}")
 
     def mark_request_as_handled(self, job_id):
         """
         Mark the request as handled when the job is completed.
         """
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         response = requests.put(f"{self.drumpler_url}/jobs/{job_id}/mark-handled", headers=headers)
-        if response.status_code == 200:
-            print(f"Request marked as handled for job {job_id}")
-        else:
+        if response.status_code != 200:
             print(f"Failed to mark request as handled for job {job_id}: {response.status_code}")
         
     def update_status(self, job_id, new_status):
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         data = {"status": new_status}
         try:
             response = requests.put(f"{self.drumpler_url}/jobs/{job_id}/update-status", json=data, headers=headers)
@@ -99,15 +99,15 @@
         except requests.RequestException as e:
             self.logger.error(f"Failed to update status due to HTTP error: {str(e)}")
 
     def worker_task(self):
         while not self.stop_signal.is_set():
             request = self.fetch_next_pending_job()
             if request:
-                if self.user_process_request_data(request):
+                if self.user_process_request_data(self, request.job_id, request.request_dict):
                     self.insert_event(request.job_id, "Request processed successfully")
                     self.update_status(request.job_id, "Completed")
                     self.logger.info(f"Request processed successfully for job {request.job_id}")
                 else:
                     self.insert_event(request.job_id, "Failed to process request")
                     self.update_status(request.job_id, "Error")
                     self.logger.error(f"Failed to process request for job {request.job_id}")
```

### Comparing `drumpler_mammoth-2.1.3/drumpler_mammoth/mylogger.py` & `drumpler_mammoth-2.1.4/drumpler_mammoth/mylogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from logging.handlers import RotatingFileHandler
 
 class MyLogger:
     _logger = None
 
     @classmethod
-    def get_logger(cls, name='MammothLogger', file_name='mammoth.log', level=logging.DEBUG):
+    def get_logger(cls, name='MammothLogger', file_name='mammoth.log', level=logging.ERROR):
         if cls._logger is None:
             # Create logger
             cls._logger = logging.getLogger(name)
             cls._logger.setLevel(level)
 
             # Create handlers
             c_handler = logging.StreamHandler()
```

### Comparing `drumpler_mammoth-2.1.3/setup.py` & `drumpler_mammoth-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='drumpler_mammoth',
-    version='2.1.3',
+    version='2.1.4',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler-Mammoth',
     packages=find_packages(),
```

