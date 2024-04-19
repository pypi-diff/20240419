# Comparing `tmp/termii_python_client-1.1.0.tar.gz` & `tmp/termii_python_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termii_python_client-1.1.0.tar", last modified: Thu Apr 18 19:00:11 2024, max compression
+gzip compressed data, was "termii_python_client-1.2.0.tar", last modified: Fri Apr 19 07:37:27 2024, max compression
```

## Comparing `termii_python_client-1.1.0.tar` & `termii_python_client-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:00:11.207912 termii_python_client-1.1.0/
--rw-rw-rw-   0        0        0     1093 2024-04-18 09:23:17.000000 termii_python_client-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     5024 2024-04-18 19:00:11.175997 termii_python_client-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4410 2024-04-18 18:56:21.000000 termii_python_client-1.1.0/README.md
--rw-rw-rw-   0        0        0      725 2024-04-18 18:59:46.000000 termii_python_client-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 19:00:11.207912 termii_python_client-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 19:00:11.173005 termii_python_client-1.1.0/termii_python_client.egg-info/
--rw-rw-rw-   0        0        0     5024 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 19:00:11.160044 termii_python_client-1.1.0/tests/
--rw-rw-rw-   0        0        0      921 2024-04-18 00:09:57.000000 termii_python_client-1.1.0/tests/test_contact.py
--rw-rw-rw-   0        0        0     1379 2024-04-18 09:03:34.000000 termii_python_client-1.1.0/tests/test_insights.py
--rw-rw-rw-   0        0        0     1687 2024-04-17 23:13:06.000000 termii_python_client-1.1.0/tests/test_messaging.py
--rw-rw-rw-   0        0        0     1192 2024-04-17 19:04:09.000000 termii_python_client-1.1.0/tests/test_number_api.py
--rw-rw-rw-   0        0        0     2222 2024-04-17 23:12:53.000000 termii_python_client-1.1.0/tests/test_phonebooks.py
--rw-rw-rw-   0        0        0      642 2024-04-17 06:41:14.000000 termii_python_client-1.1.0/tests/test_sender_id.py
--rw-rw-rw-   0        0        0     2185 2024-04-18 18:56:32.000000 termii_python_client-1.1.0/tests/test_token.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:27.067633 termii_python_client-1.2.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-18 09:23:17.000000 termii_python_client-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5166 2024-04-19 07:37:26.992856 termii_python_client-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4552 2024-04-18 19:26:30.000000 termii_python_client-1.2.0/README.md
+-rw-rw-rw-   0        0        0      725 2024-04-19 07:32:28.000000 termii_python_client-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:37:27.071622 termii_python_client-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:26.542042 termii_python_client-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:26.599882 termii_python_client-1.2.0/src/termii/
+-rw-rw-rw-   0        0        0        0 2024-04-16 19:13:19.000000 termii_python_client-1.2.0/src/termii/__init__.py
+-rw-rw-rw-   0        0        0    21787 2024-04-19 07:04:55.000000 termii_python_client-1.2.0/src/termii/termii.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:26.973882 termii_python_client-1.2.0/src/termii_python_client.egg-info/
+-rw-rw-rw-   0        0        0     5166 2024-04-19 07:37:26.000000 termii_python_client-1.2.0/src/termii_python_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-19 07:37:26.000000 termii_python_client-1.2.0/src/termii_python_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:37:26.000000 termii_python_client-1.2.0/src/termii_python_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 07:37:26.000000 termii_python_client-1.2.0/src/termii_python_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:26.963908 termii_python_client-1.2.0/tests/
+-rw-rw-rw-   0        0        0      932 2024-04-19 07:35:12.000000 termii_python_client-1.2.0/tests/test_contact.py
+-rw-rw-rw-   0        0        0     1390 2024-04-19 07:35:19.000000 termii_python_client-1.2.0/tests/test_insights.py
+-rw-rw-rw-   0        0        0     1698 2024-04-19 07:35:25.000000 termii_python_client-1.2.0/tests/test_messaging.py
+-rw-rw-rw-   0        0        0     1203 2024-04-19 07:35:30.000000 termii_python_client-1.2.0/tests/test_number_api.py
+-rw-rw-rw-   0        0        0     2233 2024-04-19 07:35:37.000000 termii_python_client-1.2.0/tests/test_phonebooks.py
+-rw-rw-rw-   0        0        0      653 2024-04-19 07:35:43.000000 termii_python_client-1.2.0/tests/test_sender_id.py
+-rw-rw-rw-   0        0        0     2196 2024-04-19 07:34:50.000000 termii_python_client-1.2.0/tests/test_token.py
```

### Comparing `termii_python_client-1.1.0/LICENSE` & `termii_python_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.1.0/PKG-INFO` & `termii_python_client-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: termii-python-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Termii python package
 Author-email: "Gabriel Michael Ojomakpene [codewitgabi]" <codewitgabi222@gmail.com>, Joshua Joseph <joshuajosephizzyjosh@gmail.com>
 Project-URL: Homepage, https://github.com/codewitgabi/python-termii
 Project-URL: Issues, https://github.com/codewitgabi/python-termii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align="center">Termii Python Client</h1>
+<h1 align="center">Termii Python Client <img alt="Static Badge" src="https://img.shields.io/badge/termii-python-client?style=for-the-badge&logo=github&logoColor=%23000">
+</h1>
+<br><br>
 
 <div align="center">
     <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/t/codewitgabi/python-termii">
     <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/codewitgabi/python-termii">
     <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues/codewitgabi/python-termii">
     <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-pr/codewitgabi/python-termii">
     <img alt="GitHub License" src="https://img.shields.io/github/license/codewitgabi/python-termii">
```

### Comparing `termii_python_client-1.1.0/README.md` & `termii_python_client-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-<h1 align="center">Termii Python Client</h1>
+<h1 align="center">Termii Python Client <img alt="Static Badge" src="https://img.shields.io/badge/termii-python-client?style=for-the-badge&logo=github&logoColor=%23000">
+</h1>
+<br><br>
 
 <div align="center">
     <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/t/codewitgabi/python-termii">
     <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/codewitgabi/python-termii">
     <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues/codewitgabi/python-termii">
     <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-pr/codewitgabi/python-termii">
     <img alt="GitHub License" src="https://img.shields.io/github/license/codewitgabi/python-termii">
```

### Comparing `termii_python_client-1.1.0/pyproject.toml` & `termii_python_client-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.31.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "termii-python-client"
-version = "1.1.0"
+version = "1.2.0"
 authors = [ { name="Gabriel Michael Ojomakpene [codewitgabi]", email="codewitgabi222@gmail.com" }, { name="Joshua Joseph", email="joshuajosephizzyjosh@gmail.com" },
 ]
 description = "Termii python package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `termii_python_client-1.1.0/termii_python_client.egg-info/PKG-INFO` & `termii_python_client-1.2.0/src/termii_python_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: termii-python-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: Termii python package
 Author-email: "Gabriel Michael Ojomakpene [codewitgabi]" <codewitgabi222@gmail.com>, Joshua Joseph <joshuajosephizzyjosh@gmail.com>
 Project-URL: Homepage, https://github.com/codewitgabi/python-termii
 Project-URL: Issues, https://github.com/codewitgabi/python-termii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<h1 align="center">Termii Python Client</h1>
+<h1 align="center">Termii Python Client <img alt="Static Badge" src="https://img.shields.io/badge/termii-python-client?style=for-the-badge&logo=github&logoColor=%23000">
+</h1>
+<br><br>
 
 <div align="center">
     <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/t/codewitgabi/python-termii">
     <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/codewitgabi/python-termii">
     <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues/codewitgabi/python-termii">
     <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-pr/codewitgabi/python-termii">
     <img alt="GitHub License" src="https://img.shields.io/github/license/codewitgabi/python-termii">
```

### Comparing `termii_python_client-1.1.0/tests/test_contact.py` & `termii_python_client-1.2.0/tests/test_contact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Contacts API allows you manage (i.e. edit, update, & delete) contacts in your phonebook.
 """
 
 # imports
 
 import os
-from termii import Termii
+from src.termii.termii import Termii
 from unittest import TestCase
 
 
 class TestContacts(TestCase):
     def setUp(self) -> None:
         self.termii = Termii(api_key=os.environ.get("TERMII_API_KEY"))
         self.sender_id = os.environ.get("TERMII_SENDER_ID")
```

### Comparing `termii_python_client-1.1.0/tests/test_insights.py` & `termii_python_client-1.2.0/tests/test_insights.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The Balance API returns your total balance and balance information from your wallet, such as currency.
 """
 
 # imports
 
 import os
 from unittest import TestCase
-from termii import Termii
+from src.termii.termii import Termii
 
 
 class TestInsights(TestCase):
     def setUp(self) -> None:
         self.sender_id = os.environ.get("TERMII_SENDER_ID")
         self.termii = Termii(api_key=os.environ.get(
             "TERMII_API_KEY"), sender_id=self.sender_id)
```

### Comparing `termii_python_client-1.1.0/tests/test_messaging.py` & `termii_python_client-1.2.0/tests/test_messaging.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 # imports
 
 import os
 import unittest
 from unittest import TestCase
-from termii import Termii
+from src.termii.termii import Termii
 
 
 class TestMessaging(TestCase):
     def setUp(self) -> None:
         self.termii = Termii(api_key=os.environ.get("TERMII_API_KEY"))
         self.sender_id = os.environ.get("TERMII_SENDER_ID")
```

### Comparing `termii_python_client-1.1.0/tests/test_number_api.py` & `termii_python_client-1.2.0/tests/test_number_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This API allows businesses send messages to customers using Termii's auto-generated messaging numbers that adapt to customers location.
 """
 
 # imports
 
 import os
 from unittest import TestCase
-from termii import Termii
+from src.termii.termii import Termii
 
 
 class TestNumberAPI(TestCase):
     def setUp(self) -> None:
         self.sender_id = os.environ.get("TERMII_SENDER_ID")
         self.termii = Termii(api_key=os.environ.get(
             "TERMII_API_KEY"), sender_id=self.sender_id)
```

### Comparing `termii_python_client-1.1.0/tests/test_phonebooks.py` & `termii_python_client-1.2.0/tests/test_phonebooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # imports
 
 import os
 from unittest import TestCase
 import unittest
-from termii import Termii
+from src.termii.termii import Termii
 
 
 class TestPhonebook(TestCase):
     def setUp(self) -> None:
         self.termii = Termii(api_key=os.environ.get("TERMII_API_KEY"))
         self.sender_id = os.environ.get("TERMII_SENDER_ID")
```

### Comparing `termii_python_client-1.1.0/tests/test_sender_id.py` & `termii_python_client-1.2.0/tests/test_sender_id.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from unittest import TestCase
-from termii import Termii
+from src.termii.termii import Termii
 
 
 class TestSenderID(TestCase):
     def setUp(self) -> None:
         self.termii = Termii(api_key=os.environ.get("TERMII_API_KEY"))
 
     def test_get_senderId(self):
```

### Comparing `termii_python_client-1.1.0/tests/test_token.py` & `termii_python_client-1.2.0/tests/test_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The send token API allows businesses trigger one-time-passwords (OTP) across any available messaging channel on Termii. One-time-passwords created are generated randomly and there's an option to set an expiry time.
 """
 
 # imports
 
 import os
 from unittest import TestCase
-from termii import Termii
+from src.termii.termii import Termii
 
 
 class TestToken(TestCase):
     def setUp(self) -> None:
         self.termii = Termii(api_key=os.environ.get("TERMII_API_KEY"))
         self.sender_id = os.environ.get("TERMII_SENDER_ID")
         self.email_configuration_id = os.environ.get(
```

