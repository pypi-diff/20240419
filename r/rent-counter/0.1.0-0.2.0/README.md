# Comparing `tmp/rent_counter-0.1.0.tar.gz` & `tmp/rent_counter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rent_counter-0.1.0.tar", last modified: Fri Apr 19 10:54:30 2024, max compression
+gzip compressed data, was "rent_counter-0.2.0.tar", last modified: Fri Apr 19 13:20:40 2024, max compression
```

## Comparing `rent_counter-0.1.0.tar` & `rent_counter-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 10:54:30.346528 rent_counter-0.1.0/
--rw-rw-rw-   0        0        0     2001 2024-04-19 10:54:30.340531 rent_counter-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 10:54:30.336535 rent_counter-0.1.0/rent_counter.egg-info/
--rw-rw-rw-   0        0        0     2001 2024-04-19 10:54:30.000000 rent_counter-0.1.0/rent_counter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-19 10:54:30.000000 rent_counter-0.1.0/rent_counter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:54:30.000000 rent_counter-0.1.0/rent_counter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:54:30.000000 rent_counter-0.1.0/rent_counter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 10:54:30.347528 rent_counter-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      795 2024-04-19 10:45:32.000000 rent_counter-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:54:30.331537 rent_counter-0.1.0/tests/
--rw-rw-rw-   0        0        0     2242 2024-04-19 07:51:08.000000 rent_counter-0.1.0/tests/test_countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:20:40.184521 rent_counter-0.2.0/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 13:20:40.177174 rent_counter-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2024-04-19 07:51:08.000000 rent_counter-0.2.0/README.md
+-rw-rw-rw-   0        0        0      451 2024-04-19 07:51:08.000000 rent_counter-0.2.0/countdown.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:20:40.174175 rent_counter-0.2.0/rent_counter.egg-info/
+-rw-rw-rw-   0        0        0     2001 2024-04-19 13:20:40.000000 rent_counter-0.2.0/rent_counter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-04-19 13:20:40.000000 rent_counter-0.2.0/rent_counter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:20:40.000000 rent_counter-0.2.0/rent_counter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 13:20:40.000000 rent_counter-0.2.0/rent_counter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 13:20:40.185530 rent_counter-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      824 2024-04-19 12:59:35.000000 rent_counter-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:20:40.158579 rent_counter-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1119 2024-04-19 12:54:47.000000 rent_counter-0.2.0/tests/test_countdown.py
```

### Comparing `rent_counter-0.1.0/PKG-INFO` & `rent_counter-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.1.0/README.md` & `rent_counter-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rent_counter-0.1.0/rent_counter.egg-info/PKG-INFO` & `rent_counter-0.2.0/rent_counter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rent_counter
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python library for managing rent expiration countdowns
 Home-page: https://github.com/Erickadikah/count
 Author: Erick Adikah
 Author-email: your.email@example.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rent_counter-0.1.0/setup.py` & `rent_counter-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rent_counter',
-    version='0.1.0',
+    version='0.2.0',
     packages=find_packages(),
     include_package_data=True,
+    py_modules=['countdown'],
     description='A Python library for managing rent expiration countdowns',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Erick Adikah',
     author_email='your.email@example.com',
     license='MIT',
     url='https://github.com/Erickadikah/count',
@@ -19,8 +20,7 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     install_requires=[
         
     ],
 )
-
```

### Comparing `rent_counter-0.1.0/tests/test_countdown.py` & `rent_counter-0.2.0/tests/test_countdown.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,33 +18,8 @@
     def test_remaining_time_present(self):
         end_date = datetime.now()  # End date is the current date
         remaining_time = calculate_remaining_time(end_date)
         self.assertIsInstance(remaining_time, timedelta)
         self.assertLessEqual(abs(remaining_time.total_seconds()), 1)
 
 if __name__ == '__main__':
-    unittest.main()
-import unittest
-from datetime import datetime, timedelta
-from countdown import calculate_remaining_time
-
-class TestCountdown(unittest.TestCase):
-    def test_remaining_time_future(self):
-        end_date = datetime.now() + timedelta(days=7)  # End date 7 days from now
-        remaining_time = calculate_remaining_time(end_date)
-        self.assertIsInstance(remaining_time, timedelta)
-        self.assertGreaterEqual(remaining_time.total_seconds(), 0)
-
-    def test_remaining_time_past(self):
-        end_date = datetime.now() - timedelta(days=7)  # End date 7 days ago
-        remaining_time = calculate_remaining_time(end_date)
-        self.assertIsInstance(remaining_time, timedelta)
-        self.assertLessEqual(remaining_time.total_seconds(), 0)
-
-    def test_remaining_time_present(self):
-        end_date = datetime.now()  # End date is the current date
-        remaining_time = calculate_remaining_time(end_date)
-        self.assertIsInstance(remaining_time, timedelta)
-        self.assertLessEqual(abs(remaining_time.total_seconds()), 1)
-
-if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

