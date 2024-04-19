# Comparing `tmp/nccommons-0.1.5.tar.gz` & `tmp/nccommons-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nccommons-0.1.5.tar", last modified: Tue Mar 26 07:47:46 2024, max compression
+gzip compressed data, was "nccommons-0.1.6.tar", last modified: Fri Apr 19 18:40:56 2024, max compression
```

## Comparing `nccommons-0.1.5.tar` & `nccommons-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-03-26 07:47:46.960926 nccommons-0.1.5/
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-02-08 09:46:36.000000 nccommons-0.1.5/LICENSE
--rw-r--r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      636 2024-03-26 07:47:46.960926 nccommons-0.1.5/PKG-INFO
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      131 2024-03-07 07:30:50.000000 nccommons-0.1.5/README.md
-drwxrwxr-x   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-03-26 07:47:46.948926 nccommons-0.1.5/nccommons/
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      141 2024-03-07 07:53:03.000000 nccommons-0.1.5/nccommons/__init__.py
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      171 2024-02-10 17:05:37.000000 nccommons-0.1.5/nccommons/decode.py
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)     4304 2024-03-26 07:46:20.000000 nccommons-0.1.5/nccommons/emails.py
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)     6735 2024-03-07 08:05:00.000000 nccommons-0.1.5/nccommons/gsheetHelper.py
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)     3439 2024-02-10 14:48:59.000000 nccommons-0.1.5/nccommons/jsons.py
-drwxrwxr-x   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-03-26 07:47:46.960926 nccommons-0.1.5/nccommons.egg-info/
--rw-r--r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      636 2024-03-26 07:47:46.000000 nccommons-0.1.5/nccommons.egg-info/PKG-INFO
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      265 2024-03-26 07:47:46.000000 nccommons-0.1.5/nccommons.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        1 2024-03-26 07:47:46.000000 nccommons-0.1.5/nccommons.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)       10 2024-03-26 07:47:46.000000 nccommons-0.1.5/nccommons.egg-info/top_level.txt
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)       38 2024-03-26 07:47:46.964926 nccommons-0.1.5/setup.cfg
--rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      663 2024-03-26 07:47:04.000000 nccommons-0.1.5/setup.py
+drwxrwxr-x   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-04-19 18:40:56.009580 nccommons-0.1.6/
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-02-08 09:46:36.000000 nccommons-0.1.6/LICENSE
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      550 2024-04-19 18:40:56.009580 nccommons-0.1.6/PKG-INFO
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-02-08 09:46:51.000000 nccommons-0.1.6/README.md
+drwxrwxr-x   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-04-19 18:40:55.997580 nccommons-0.1.6/nccommons/
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      191 2024-04-19 18:37:14.000000 nccommons-0.1.6/nccommons/__init__.py
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      171 2024-02-10 17:05:37.000000 nccommons-0.1.6/nccommons/decode.py
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)     4372 2024-04-19 18:38:45.000000 nccommons-0.1.6/nccommons/emails.py
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)     3439 2024-02-10 14:48:59.000000 nccommons-0.1.6/nccommons/jsons.py
+drwxrwxr-x   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        0 2024-04-19 18:40:56.005580 nccommons-0.1.6/nccommons.egg-info/
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      550 2024-04-19 18:40:55.000000 nccommons-0.1.6/nccommons.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      239 2024-04-19 18:40:55.000000 nccommons-0.1.6/nccommons.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)        1 2024-04-19 18:40:55.000000 nccommons-0.1.6/nccommons.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)       10 2024-04-19 18:40:55.000000 nccommons-0.1.6/nccommons.egg-info/top_level.txt
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)       38 2024-04-19 18:40:56.009580 nccommons-0.1.6/setup.cfg
+-rw-rw-r--   0 abhishekmaurya  (1001) abhishekmaurya  (1001)      665 2024-04-19 18:39:30.000000 nccommons-0.1.6/setup.py
```

### Comparing `nccommons-0.1.5/PKG-INFO` & `nccommons-0.1.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: nccommons
-Version: 0.1.5
-Summary: This package provide comon functions that can be used in API or UI Automation
+Version: 0.1.6
+Summary: This package provides common functions that can be used in API or UI Automation
 Home-page: https://github.com/abhishek.maurya/Abhishekkapackage
 Author: Abhishek Maurya
 Author-email: testmartech1@netcorecloud.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-pip install wheel
-sudo apt install twine
+UNKNOWN
 
-gspread
-google-api-python-client 
-google-auth-httplib2 
-google-auth-oauthlib
-oauth2client
```

### Comparing `nccommons-0.1.5/nccommons/emails.py` & `nccommons-0.1.6/nccommons/emails.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import csv
 import email
 import imaplib
 import re
 from concurrent.futures import ThreadPoolExecutor
+from datetime import datetime
 
 import requests
 
-
 def search_email(mail_server, username, password, subject=None, sender=None, recipient=None):
     with imaplib.IMAP4_SSL(host=mail_server) as imap_server:
         try:
             imap_server.login(username, password)
         except imaplib.IMAP4.error as e:
             print("IMAP login failed:", e)
             return []
 
         imap_server.select("INBOX")
 
+        today = datetime.now().strftime("%d-%b-%Y")
+
         search_criteria = []
         if subject:
             search_criteria.append(f'SUBJECT "{subject}"')
         if sender:
             search_criteria.append(f'FROM "{sender}"')
         if recipient:
             search_criteria.append(f'TO "{recipient}"')
 
+        search_criteria.append(f'SINCE "{today}"')
+
         if not search_criteria:
             return []
 
         search_string = " ".join(search_criteria)
         _, selected_mails = imap_server.search(None, search_string)
         email_list = []
 
@@ -38,19 +42,19 @@
             email_message = email.message_from_bytes(bytes_data)
 
             email_details = {
                 "from": email_message["from"],
                 "to": email_message["to"],
                 "date": email_message["date"],
                 "subject": email_message["subject"],
-                "fncId": email_message["X-Fncid"]
             }
+
             for part in email_message.walk():
                 content_type = part.get_content_type()
-                if content_type in ["text/html", "html"]:
+                if content_type in ["text/plain", "text/html", "html"]:
                     try:
                         message = part.get_payload(decode=True)
                         email_details["body"] = message.decode()
                     except UnicodeDecodeError as e:
                         print("Failed to decode email body:", e)
                     break
 
@@ -120,8 +124,8 @@
 #process_emails(subject=subject, sender=sender, recipients=recipients)
 
 
 """     email_list = ['http://smt.com//414896-cHJhcHA0X2F1dG9tYXRpb24xXzE2Nzg2NDIzNTU=.zip',
                   'http://smt.com//414897-cHJhcHA0X2F1dG9tYXRpb24xXzE2Nzg2NDI1NjU=.zip',
                   'http://smt.com/jobs//414895-cHJhcHA0X2F1dG9tYXRpb24xXzE2Nzg2NDE3MDU=.zip']
     gmail_helper.find_smtreports_zip_from_gmail(email_list, '414897') """
-#search_email("imap.gmail.com", "abhishekmauryanetcore@gmail.com", "hrjs dihb mjkl lpib", subject="Duplicate Emailabhishek", sender=None, recipient=None)
+search_email("imap.gmail.com","abhishekmauryanetcore@gmail.com","hrjs dihb mjkl lpib","Please confirm your report request")
```

### Comparing `nccommons-0.1.5/nccommons/jsons.py` & `nccommons-0.1.6/nccommons/jsons.py`

 * *Files identical despite different names*

### Comparing `nccommons-0.1.5/nccommons.egg-info/PKG-INFO` & `nccommons-0.1.6/nccommons.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: nccommons
-Version: 0.1.5
-Summary: This package provide comon functions that can be used in API or UI Automation
+Version: 0.1.6
+Summary: This package provides common functions that can be used in API or UI Automation
 Home-page: https://github.com/abhishek.maurya/Abhishekkapackage
 Author: Abhishek Maurya
 Author-email: testmartech1@netcorecloud.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-pip install wheel
-sudo apt install twine
+UNKNOWN
 
-gspread
-google-api-python-client 
-google-auth-httplib2 
-google-auth-oauthlib
-oauth2client
```

### Comparing `nccommons-0.1.5/setup.py` & `nccommons-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="nccommons",
-    version="0.1.5",
+    version="0.1.6",
     author="Abhishek Maurya",
     author_email="testmartech1@netcorecloud.com",
-    description="This package provide comon functions that can be used in API or UI Automation",
+    description="This package provides common functions that can be used in API or UI Automation",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/abhishek.maurya/Abhishekkapackage",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

