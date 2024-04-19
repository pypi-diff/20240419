# Comparing `tmp/testit-importer-allure-1.6.0.tar.gz` & `tmp/testit_importer_allure-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-importer-allure-1.6.0.tar", last modified: Wed Mar 13 05:40:00 2024, max compression
+gzip compressed data, was "testit_importer_allure-1.6.2.tar", last modified: Fri Apr 19 11:03:00 2024, max compression
```

## Comparing `testit-importer-allure-1.6.0.tar` & `testit_importer_allure-1.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:40:00.585372 testit-importer-allure-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-13 05:40:00.585372 testit-importer-allure-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/connection_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 05:40:00.585372 testit-importer-allure-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:40:00.581372 testit-importer-allure-1.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/filedto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/filereader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/minioreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-13 05:39:56.000000 testit-importer-allure-1.6.0/src/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 05:40:00.585372 testit-importer-allure-1.6.0/testit_importer_allure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-13 05:40:00.000000 testit-importer-allure-1.6.0/testit_importer_allure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-13 05:40:00.000000 testit-importer-allure-1.6.0/testit_importer_allure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 05:40:00.000000 testit-importer-allure-1.6.0/testit_importer_allure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-13 05:40:00.000000 testit-importer-allure-1.6.0/testit_importer_allure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-13 05:40:00.000000 testit-importer-allure-1.6.0/testit_importer_allure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-13 05:40:00.000000 testit-importer-allure-1.6.0/testit_importer_allure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:03:00.706045 testit_importer_allure-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-19 11:03:00.702045 testit_importer_allure-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/connection_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:03:00.706045 testit_importer_allure-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:03:00.702045 testit_importer_allure-1.6.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/filedto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/minioreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:03:00.702045 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/top_level.txt
```

### Comparing `testit-importer-allure-1.6.0/PKG-INFO` & `testit_importer_allure-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.6.0
+Version: 1.6.2
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-importer-allure-1.6.0/README.md` & `testit_importer_allure-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/setup.py` & `testit_importer_allure-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='testit-importer-allure',
-    version='1.6.0',
+    version='1.6.2',
     description='Allure report importer for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit-importer-allure/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit-importer-allure-1.6.0/src/__main__.py` & `testit_importer_allure-1.6.2/src/__main__.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/src/apiclient.py` & `testit_importer_allure-1.6.2/src/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/src/configurator.py` & `testit_importer_allure-1.6.2/src/configurator.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/src/converter.py` & `testit_importer_allure-1.6.2/src/converter.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/src/filereader.py` & `testit_importer_allure-1.6.2/src/filereader.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/src/importer.py` & `testit_importer_allure-1.6.2/src/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,24 @@
 
             test = data_tests[history_id]
             prefix = '' if 'uuid' in test else '@'
 
             if 'name' not in test and 'fullName' in test:
                 test['name'] = test['fullName']
 
+            if 'labels' in test:
+                test['labels'], test['namespace'], test['classname'], work_items_id = \
+                    self.__get_data_from_labels(test['labels'])
+            else:
+                test['labels'] = []
+                test['namespace'] = None
+                test['classname'] = None
+                work_items_id = []
+
             test['external_id'] = history_id
-            test['labels'], test['namespace'], test['classname'], work_items_id = \
-                self.__get_data_from_labels(test['labels'])
             test['attachments'] = self.__send_attachments(test['attachments']) if 'attachments' in test else []
             test['setup'], test['setup_results'], test['teardown'], test['teardown_results'] = \
                 self.__form_setup_teardown(data_fixtures, test.get('uuid', None))
             test['steps'], test['step_results'] = self.__form_steps(test.get('steps', None))
             test['links'] = self.__form_links(test['links']) if 'links' in test else []
             test['traces'] = test['statusDetails'].get('trace') if \
                 'statusDetails' in test and test['statusDetails'] else None
@@ -161,19 +168,19 @@
                     packages = label[f'{prefix}value'].split('.')
 
                     while packages and not packages[-1]:
                         del packages[-1]
 
                     if packages:
                         namespace = packages[-1]
-                elif label[f'{prefix}name'] == 'parentSuite':
+                elif label[f'{prefix}name'] == 'parentSuite' and label[f'{prefix}value']:
                     namespace = label[f'{prefix}value']
-                elif label[f'{prefix}name'] in ('subSuite', 'suite'):
+                elif label[f'{prefix}name'] in ('subSuite', 'suite') and label[f'{prefix}value']:
                     class_name = label[f'{prefix}value']
-                elif label[f'{prefix}name'] == 'testClass':
+                elif label[f'{prefix}name'] == 'testClass' and label[f'{prefix}value'].split('.')[-1]:
                     class_name = label[f'{prefix}value'].split('.')[-1]
 
         return labels, namespace, class_name, work_items_id
 
     @staticmethod
     def __parse_xml(data, key, value):
         if key in data:
@@ -238,15 +245,16 @@
                         {
                             'title': step['name'],
                             'step_results': inner_results_steps,
                             'outcome': step[f'{prefix}status'].title() if f'{prefix}status' in step and step[f'{prefix}status'] in (
                                     'passed', 'skipped') else 'Failed',
                             'duration': (int(step[f'{prefix}stop']) - int(
                                 step[f'{prefix}start'])) if f'{prefix}stop' in step else 0,
-                            'started_on': datetime.fromtimestamp(int(step[f'{prefix}start']) / 1000.0),
+                            'started_on': datetime.fromtimestamp(
+                                int(step[f'{prefix}start']) / 1000.0) if f'{prefix}start' in step else None,
                             'completed_on': datetime.fromtimestamp(
                                 int(step[f'{prefix}stop']) / 1000.0) if f'{prefix}stop' in step else None,
                             "attachments": attachments,
                             'parameters': self.__form_parameters(step['parameters']) if 'parameters' in step else None
                         }
                     )
```

### Comparing `testit-importer-allure-1.6.0/src/minioreader.py` & `testit_importer_allure-1.6.2/src/minioreader.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/src/parser.py` & `testit_importer_allure-1.6.2/src/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,19 @@
         elif file_extension == '.xml' and file_name[-9:] == 'testsuite':
             self.__read_xml(file)
 
     def __read_json(self, file_dto: FileDto):
         result_data = json.load(file_dto.file)
 
         if 'result' in file_dto.name:
-            if result_data['historyId'] not in self.__data_tests \
-                    or result_data['start'] > self.__data_tests[result_data['historyId']]['start']:
+            if 'historyId' not in result_data:
+                result_data['historyId'] = self.__get_hash(result_data['fullName'])
+
+            if result_data['historyId'] not in self.__data_tests or \
+                    result_data['start'] > self.__data_tests[result_data['historyId']]['start']:
                 self.__data_tests[str(result_data['historyId'])] = result_data
 
         elif 'container' in file_dto.name:
             if 'children' in result_data:
                 self.__data_fixtures[result_data['uuid']] = result_data
 
     def __read_xml(self, file_dto: FileDto):
@@ -68,7 +71,12 @@
             md5 = hashlib.md5()
             md5.update(testcase['title'].encode('utf-8'))
             testcase_id = md5.hexdigest()
 
             if testcase_id not in self.__data_tests \
                     or testcase['@start'] > self.__data_tests[testcase_id]['@start']:
                 self.__data_tests[testcase_id] = testcase
+
+    @staticmethod
+    def __get_hash(value: str):
+        md = hashlib.sha256(bytes(value, encoding='utf-8'))
+        return md.hexdigest()
```

### Comparing `testit-importer-allure-1.6.0/src/rabbitmq.py` & `testit_importer_allure-1.6.2/src/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `testit-importer-allure-1.6.0/testit_importer_allure.egg-info/PKG-INFO` & `testit_importer_allure-1.6.2/testit_importer_allure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.6.0
+Version: 1.6.2
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-importer-allure-1.6.0/testit_importer_allure.egg-info/SOURCES.txt` & `testit_importer_allure-1.6.2/testit_importer_allure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

