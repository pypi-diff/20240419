# Comparing `tmp/airmailer-0.2.0.tar.gz` & `tmp/airmailer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airmailer-0.2.0.tar", last modified: Fri Jul  7 00:02:10 2023, max compression
+gzip compressed data, was "airmailer-0.2.2.tar", last modified: Thu Apr 18 22:55:49 2024, max compression
```

## Comparing `airmailer-0.2.0.tar` & `airmailer-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.664908 airmailer-0.2.0/
--rw-rw-r--   0 cmalek     (501) admin       (80)      161 2021-11-30 23:45:18.000000 airmailer-0.2.0/AUTHORS.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)     3542 2021-12-02 17:36:04.000000 airmailer-0.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)       89 2021-11-30 23:45:18.000000 airmailer-0.2.0/HISTORY.rst
--rw-rw-r--   0 cmalek     (501) admin       (80)      589 2021-11-30 23:45:18.000000 airmailer-0.2.0/LICENSE
--rw-rw-r--   0 cmalek     (501) admin       (80)      262 2021-11-30 23:45:18.000000 airmailer-0.2.0/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2017 2023-07-07 00:02:10.665173 airmailer-0.2.0/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      769 2023-07-06 17:48:03.000000 airmailer-0.2.0/README.rst
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.653265 airmailer-0.2.0/airmailer/
--rw-rw-r--   0 cmalek     (501) admin       (80)      132 2023-07-07 00:00:47.000000 airmailer-0.2.0/airmailer/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.662661 airmailer-0.2.0/airmailer/backend/
--rw-rw-r--   0 cmalek     (501) admin       (80)      150 2021-12-02 17:45:23.000000 airmailer-0.2.0/airmailer/backend/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8867 2023-07-06 17:35:36.000000 airmailer-0.2.0/airmailer/backend/aws.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2519 2023-07-06 23:55:46.000000 airmailer-0.2.0/airmailer/backend/base.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6573 2021-12-02 18:31:49.000000 airmailer-0.2.0/airmailer/backend/smtp.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.663940 airmailer-0.2.0/airmailer/cli/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-12-02 18:43:46.000000 airmailer-0.2.0/airmailer/cli/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      453 2021-12-02 18:45:58.000000 airmailer-0.2.0/airmailer/cli/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      405 2021-12-02 17:22:14.000000 airmailer-0.2.0/airmailer/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      103 2021-12-02 18:45:46.000000 airmailer-0.2.0/airmailer/logging.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      187 2023-06-30 22:26:03.000000 airmailer-0.2.0/airmailer/main.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    22227 2023-07-06 23:54:10.000000 airmailer-0.2.0/airmailer/message.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-07 00:02:10.659079 airmailer-0.2.0/airmailer.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2017 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      575 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       50 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/not-zip-safe
--rw-rw-r--   0 cmalek     (501) admin       (80)       23 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       10 2023-07-07 00:02:10.000000 airmailer-0.2.0/airmailer.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      734 2023-07-07 00:02:10.666366 airmailer-0.2.0/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1511 2023-07-07 00:00:47.000000 airmailer-0.2.0/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2024-04-18 22:55:49.823843 airmailer-0.2.2/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      161 2021-11-30 23:45:18.000000 airmailer-0.2.2/AUTHORS.rst
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3542 2021-12-02 17:36:04.000000 airmailer-0.2.2/CONTRIBUTING.rst
+-rw-rw-r--   0 cmalek     (501) admin       (80)      322 2023-08-21 16:45:28.000000 airmailer-0.2.2/HISTORY.rst
+-rw-rw-r--   0 cmalek     (501) admin       (80)      589 2021-11-30 23:45:18.000000 airmailer-0.2.2/LICENSE
+-rw-rw-r--   0 cmalek     (501) admin       (80)      262 2021-11-30 23:45:18.000000 airmailer-0.2.2/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1329 2024-04-18 22:55:49.823913 airmailer-0.2.2/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      769 2023-07-06 17:48:03.000000 airmailer-0.2.2/README.rst
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2024-04-18 22:55:49.821749 airmailer-0.2.2/airmailer/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      132 2024-04-18 22:55:46.000000 airmailer-0.2.2/airmailer/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2024-04-18 22:55:49.823424 airmailer-0.2.2/airmailer/backend/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      150 2021-12-02 17:45:23.000000 airmailer-0.2.2/airmailer/backend/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8867 2023-07-06 17:35:36.000000 airmailer-0.2.2/airmailer/backend/aws.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2786 2024-04-18 22:50:11.000000 airmailer-0.2.2/airmailer/backend/base.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6573 2021-12-02 18:31:49.000000 airmailer-0.2.2/airmailer/backend/smtp.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2024-04-18 22:55:49.823725 airmailer-0.2.2/airmailer/cli/
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2021-12-02 18:43:46.000000 airmailer-0.2.2/airmailer/cli/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      453 2021-12-02 18:45:58.000000 airmailer-0.2.2/airmailer/cli/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      405 2021-12-02 17:22:14.000000 airmailer-0.2.2/airmailer/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      103 2021-12-02 18:45:46.000000 airmailer-0.2.2/airmailer/logging.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      187 2023-06-30 22:26:03.000000 airmailer-0.2.2/airmailer/main.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    22227 2023-07-06 23:54:10.000000 airmailer-0.2.2/airmailer/message.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2024-04-18 22:55:49.822806 airmailer-0.2.2/airmailer.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1329 2024-04-18 22:55:49.000000 airmailer-0.2.2/airmailer.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      590 2024-04-18 22:55:49.000000 airmailer-0.2.2/airmailer.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2024-04-18 22:55:49.000000 airmailer-0.2.2/airmailer.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       49 2024-04-18 22:55:49.000000 airmailer-0.2.2/airmailer.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2024-04-18 22:55:49.000000 airmailer-0.2.2/airmailer.egg-info/not-zip-safe
+-rw-rw-r--   0 cmalek     (501) admin       (80)       25 2024-04-18 22:55:49.000000 airmailer-0.2.2/airmailer.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       10 2024-04-18 22:55:49.000000 airmailer-0.2.2/airmailer.egg-info/top_level.txt
+-rw-r--r--   0 cmalek     (501) admin       (80)      116 2023-08-21 16:43:10.000000 airmailer-0.2.2/pyproject.toml
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1911 2024-04-18 22:55:49.824374 airmailer-0.2.2/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)       69 2023-08-21 16:43:23.000000 airmailer-0.2.2/setup.py
```

### Comparing `airmailer-0.2.0/CONTRIBUTING.rst` & `airmailer-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `airmailer-0.2.0/LICENSE` & `airmailer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airmailer-0.2.0/README.rst` & `airmailer-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `airmailer-0.2.0/airmailer/backend/aws.py` & `airmailer-0.2.2/airmailer/backend/aws.py`

 * *Files identical despite different names*

### Comparing `airmailer-0.2.0/airmailer/backend/base.py` & `airmailer-0.2.2/airmailer/backend/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,21 +66,32 @@
 
     def send_mail(
         self,
         subject: str,
         message,
         from_email: str,
         recipient_list: Iterable[str],
-        html_message: str = None
+        html_message: str = None,
+        bcc: Iterable[str] = None,
+        cc: Iterable[str] = None,
+        reply_to: Iterable[str] = None,
     ):
         """
         Easy wrapper for sending a single message to a recipient list. All members
         of the recipient list will see the other recipients in the 'To' field.
         """
-        mail = EmailMultiAlternatives(subject, message, from_email, recipient_list)
+        mail = EmailMultiAlternatives(
+            subject=subject,
+            body=message,
+            from_email=from_email,
+            to=recipient_list,
+            bcc=bcc,
+            cc=cc,
+            reply_to=reply_to,
+        )
         if html_message:
             mail.attach_alternative(html_message, 'text/html')
 
         with self as conn:
             num_sent = conn.send_messages([mail])
 
         return num_sent
```

### Comparing `airmailer-0.2.0/airmailer/backend/smtp.py` & `airmailer-0.2.2/airmailer/backend/smtp.py`

 * *Files identical despite different names*

### Comparing `airmailer-0.2.0/airmailer/message.py` & `airmailer-0.2.2/airmailer/message.py`

 * *Files identical despite different names*

### Comparing `airmailer-0.2.0/airmailer.egg-info/SOURCES.txt` & `airmailer-0.2.2/airmailer.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 airmailer/__init__.py
 airmailer/cli.py
 airmailer/logging.py
 airmailer/main.py
 airmailer/message.py
```

