# Comparing `tmp/ietfdata-0.6.8.tar.gz` & `tmp/ietfdata-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietfdata-0.6.8.tar", last modified: Fri Aug 18 08:12:07 2023, max compression
+gzip compressed data, was "ietfdata-0.7.0.tar", last modified: Fri Apr 19 10:53:13 2024, max compression
```

## Comparing `ietfdata-0.6.8.tar` & `ietfdata-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-08-18 08:12:07.695757 ietfdata-0.6.8/
--rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.6.8/LICENSE
--rw-rw----   0 csp        (502) staff       (20)     2970 2023-08-18 08:12:07.695113 ietfdata-0.6.8/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)     2529 2023-06-21 08:17:16.000000 ietfdata-0.6.8/README.md
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-08-18 08:12:07.657067 ietfdata-0.6.8/examples/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.6.8/examples/__init__.py
--rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.6.8/examples/bluesheets.py
--rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.6.8/examples/draft-authors.py
--rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.6.8/examples/draft-references.py
--rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.6.8/examples/draft-submissions-by-date.py
--rw-rw----   0 csp        (502) staff       (20)     1695 2022-11-03 14:42:34.000000 ietfdata-0.6.8/examples/draft-submissions.py
--rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.6.8/examples/drafts-for-person.py
--rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.6.8/examples/drafts-for-rfc.py
--rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.6.8/examples/drafts-for-wg.py
--rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.6.8/examples/emails-per-person.py
--rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.6.8/examples/ietf-leadership.py
--rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.6.8/examples/non-wg-standards-track-rfcs.py
--rw-r--r--   0 csp        (502) staff       (20)     2084 2021-04-14 11:17:29.000000 ietfdata-0.6.8/examples/org-chart.py
--rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.6.8/examples/person-attendance.py
--rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.6.8/examples/person-emails.py
--rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.6.8/examples/person.py
--rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.6.8/examples/recent-pubreq.py
--rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.6.8/examples/rfc-data.py
--rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.6.8/examples/rfc-streams.py
--rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.6.8/examples/role-names.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-08-18 08:12:07.675200 ietfdata-0.6.8/ietfdata/
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.8/ietfdata/__init__.py
--rw-rw----   0 csp        (502) staff       (20)   161537 2023-08-17 23:01:24.000000 ietfdata-0.6.8/ietfdata/datatracker.py
--rw-rw----   0 csp        (502) staff       (20)    16240 2022-04-28 14:40:41.000000 ietfdata-0.6.8/ietfdata/datatracker_ext.py
--rw-rw----   0 csp        (502) staff       (20)    26016 2023-08-17 21:28:16.000000 ietfdata-0.6.8/ietfdata/mailarchive.py
--rw-rw----   0 csp        (502) staff       (20)    24630 2023-08-17 21:41:48.000000 ietfdata-0.6.8/ietfdata/mailarchive2.py
--rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.6.8/ietfdata/py.typed
--rw-rw----   0 csp        (502) staff       (20)    24747 2022-02-13 18:30:57.000000 ietfdata-0.6.8/ietfdata/rfcindex.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-08-18 08:12:07.682613 ietfdata-0.6.8/ietfdata.egg-info/
--rw-rw----   0 csp        (502) staff       (20)     2970 2023-08-18 08:12:07.000000 ietfdata-0.6.8/ietfdata.egg-info/PKG-INFO
--rw-rw----   0 csp        (502) staff       (20)     1010 2023-08-18 08:12:07.000000 ietfdata-0.6.8/ietfdata.egg-info/SOURCES.txt
--rw-rw----   0 csp        (502) staff       (20)        1 2023-08-18 08:12:07.000000 ietfdata-0.6.8/ietfdata.egg-info/dependency_links.txt
--rw-rw----   0 csp        (502) staff       (20)      131 2023-08-18 08:12:07.000000 ietfdata-0.6.8/ietfdata.egg-info/requires.txt
--rw-rw----   0 csp        (502) staff       (20)       18 2023-08-18 08:12:07.000000 ietfdata-0.6.8/ietfdata.egg-info/top_level.txt
--rw-rw----   0 csp        (502) staff       (20)      100 2021-05-19 10:27:44.000000 ietfdata-0.6.8/pyproject.toml
--rw-rw----   0 csp        (502) staff       (20)       38 2023-08-18 08:12:07.696017 ietfdata-0.6.8/setup.cfg
--rw-rw----   0 csp        (502) staff       (20)      783 2023-08-17 17:35:20.000000 ietfdata-0.6.8/setup.py
-drwxrwx---   0 csp        (502) staff       (20)        0 2023-08-18 08:12:07.692906 ietfdata-0.6.8/tests/
--rw-rw----   0 csp        (502) staff       (20)   225785 2023-08-17 16:45:02.000000 ietfdata-0.6.8/tests/test_datatracker.py
--rw-rw----   0 csp        (502) staff       (20)     5941 2023-08-17 21:56:57.000000 ietfdata-0.6.8/tests/test_datatracker_coverage.py
--rw-rw----   0 csp        (502) staff       (20)     3476 2022-10-28 12:28:48.000000 ietfdata-0.6.8/tests/test_mailarchive.py
--rw-rw----   0 csp        (502) staff       (20)     7034 2022-07-04 08:34:17.000000 ietfdata-0.6.8/tests/test_rfcindex.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.809322 ietfdata-0.7.0/
+-rw-r--r--   0 csp        (502) staff       (20)     1294 2021-04-14 11:17:29.000000 ietfdata-0.7.0/LICENSE
+-rw-r--r--   0 csp        (502) staff       (20)     3478 2024-04-19 10:53:13.809139 ietfdata-0.7.0/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)     2529 2023-06-21 08:17:16.000000 ietfdata-0.7.0/README.md
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.804970 ietfdata-0.7.0/examples/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-08-04 12:44:47.000000 ietfdata-0.7.0/examples/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)     2037 2022-10-28 12:45:40.000000 ietfdata-0.7.0/examples/bluesheets.py
+-rw-r--r--   0 csp        (502) staff       (20)     2223 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/draft-authors.py
+-rw-rw----   0 csp        (502) staff       (20)     2163 2022-10-28 12:50:08.000000 ietfdata-0.7.0/examples/draft-references.py
+-rw-rw----   0 csp        (502) staff       (20)     2748 2021-12-02 17:45:56.000000 ietfdata-0.7.0/examples/draft-submissions-by-date.py
+-rw-rw----   0 csp        (502) staff       (20)     1756 2023-11-24 13:32:11.000000 ietfdata-0.7.0/examples/draft-submissions.py
+-rw-rw----   0 csp        (502) staff       (20)     1814 2022-06-27 14:31:39.000000 ietfdata-0.7.0/examples/drafts-for-person.py
+-rw-r--r--   0 csp        (502) staff       (20)     1799 2022-10-28 13:00:03.000000 ietfdata-0.7.0/examples/drafts-for-rfc.py
+-rw-r--r--   0 csp        (502) staff       (20)     1981 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/drafts-for-wg.py
+-rw-rw----   0 csp        (502) staff       (20)     2910 2022-10-28 13:08:25.000000 ietfdata-0.7.0/examples/emails-per-person.py
+-rw-rw----   0 csp        (502) staff       (20)     4006 2024-01-20 17:43:00.000000 ietfdata-0.7.0/examples/iesg-processing-time.py
+-rw-r--r--   0 csp        (502) staff       (20)     2773 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/ietf-leadership.py
+-rw-rw----   0 csp        (502) staff       (20)     1842 2022-10-28 12:36:22.000000 ietfdata-0.7.0/examples/non-wg-standards-track-rfcs.py
+-rw-r--r--   0 csp        (502) staff       (20)     2214 2023-11-19 18:26:39.000000 ietfdata-0.7.0/examples/org-chart.py
+-rw-rw----   0 csp        (502) staff       (20)     1995 2022-12-10 15:03:43.000000 ietfdata-0.7.0/examples/person-attendance.py
+-rw-rw----   0 csp        (502) staff       (20)     1776 2022-10-28 15:37:24.000000 ietfdata-0.7.0/examples/person-emails.py
+-rw-rw----   0 csp        (502) staff       (20)     7955 2022-10-28 15:48:45.000000 ietfdata-0.7.0/examples/person.py
+-rw-r-----   0 csp        (502) staff       (20)     2203 2023-04-19 18:40:26.000000 ietfdata-0.7.0/examples/recent-pubreq.py
+-rw-r--r--   0 csp        (502) staff       (20)     5567 2022-10-28 15:51:05.000000 ietfdata-0.7.0/examples/rfc-data.py
+-rw-rw----   0 csp        (502) staff       (20)     1911 2023-11-26 14:57:50.000000 ietfdata-0.7.0/examples/rfc-per-year.py
+-rw-rw----   0 csp        (502) staff       (20)     2155 2021-08-27 12:26:02.000000 ietfdata-0.7.0/examples/rfc-streams.py
+-rw-r--r--   0 csp        (502) staff       (20)     2055 2021-04-14 11:17:29.000000 ietfdata-0.7.0/examples/role-names.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.806656 ietfdata-0.7.0/ietfdata/
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.7.0/ietfdata/__init__.py
+-rw-rw----   0 csp        (502) staff       (20)   158330 2024-03-17 21:44:16.000000 ietfdata-0.7.0/ietfdata/datatracker.py
+-rw-rw----   0 csp        (502) staff       (20)    16790 2023-12-27 18:19:57.000000 ietfdata-0.7.0/ietfdata/datatracker_ext.py
+-rw-rw----   0 csp        (502) staff       (20)    38885 2024-04-02 14:53:19.000000 ietfdata-0.7.0/ietfdata/mailarchive2.py
+-rw-rw----   0 csp        (502) staff       (20)        0 2020-04-11 11:24:32.000000 ietfdata-0.7.0/ietfdata/py.typed
+-rw-rw----   0 csp        (502) staff       (20)    25180 2023-11-23 08:45:26.000000 ietfdata-0.7.0/ietfdata/rfcindex.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.808942 ietfdata-0.7.0/ietfdata.egg-info/
+-rw-r--r--   0 csp        (502) staff       (20)     3478 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/PKG-INFO
+-rw-rw----   0 csp        (502) staff       (20)     1045 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/SOURCES.txt
+-rw-rw----   0 csp        (502) staff       (20)        1 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/dependency_links.txt
+-rw-rw----   0 csp        (502) staff       (20)      206 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/requires.txt
+-rw-rw----   0 csp        (502) staff       (20)       18 2024-04-19 10:53:13.000000 ietfdata-0.7.0/ietfdata.egg-info/top_level.txt
+-rw-rw----   0 csp        (502) staff       (20)      779 2023-12-27 19:59:03.000000 ietfdata-0.7.0/pyproject.toml
+-rw-rw----   0 csp        (502) staff       (20)       38 2024-04-19 10:53:13.809357 ietfdata-0.7.0/setup.cfg
+-rw-rw----   0 csp        (502) staff       (20)      806 2023-12-27 19:39:54.000000 ietfdata-0.7.0/setup.py
+drwxrwx---   0 csp        (502) staff       (20)        0 2024-04-19 10:53:13.808754 ietfdata-0.7.0/tests/
+-rw-rw----   0 csp        (502) staff       (20)   232033 2024-03-24 20:51:25.000000 ietfdata-0.7.0/tests/test_datatracker.py
+-rw-rw----   0 csp        (502) staff       (20)     5952 2023-12-20 17:52:07.000000 ietfdata-0.7.0/tests/test_datatracker_coverage.py
+-rw-rw----   0 csp        (502) staff       (20)     2908 2023-11-10 13:10:13.000000 ietfdata-0.7.0/tests/test_mailarchive2.py
+-rw-rw----   0 csp        (502) staff       (20)     7034 2022-07-04 08:34:17.000000 ietfdata-0.7.0/tests/test_rfcindex.py
```

### Comparing `ietfdata-0.6.8/LICENSE` & `ietfdata-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/PKG-INFO` & `ietfdata-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ietfdata
-Version: 0.6.8
-Summary: Access the IETF Data Tracker and RFC Index
-Home-page: https://github.com/glasgow-ipl/ietfdata
-Author: Colin Perkins
-Author-email: csp@csperkins.org
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [ietfdata](https://github.com/glasgow-ipl/ietfdata) - Access the IETF Datatracker and related resources
 =============================================================
 
 This project contains Python 3 libraries to interact with, and
 access, the [IETF datatracker](https://datatracker.ietf.org), 
 [RFC index](https://www.rfc-editor.org), and related resources.
```

### Comparing `ietfdata-0.6.8/README.md` & `ietfdata-0.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: ietfdata
+Version: 0.7.0
+Summary: Access the IETF Data Tracker and RFC Index
+Home-page: https://github.com/glasgow-ipl/ietfdata
+Author: Colin Perkins
+Author-email: Colin Perkins <csp@csperkins.org>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: bs4
+Requires-Dist: email_reply_parser
+Requires-Dist: imapclient
+Requires-Dist: pandas
+Requires-Dist: pandas-stubs
+Requires-Dist: python-dateutil
+Requires-Dist: pydantic
+Requires-Dist: pymongo
+Requires-Dist: requests
+Requires-Dist: requests-cache
+Requires-Dist: mypy
+Requires-Dist: wheel
+Requires-Dist: twine
+Requires-Dist: keyring
+Requires-Dist: coverage
+Requires-Dist: pymongo-stubs
+Requires-Dist: types-six
+Requires-Dist: types-requests
+Requires-Dist: types-python-dateutil
+
 [ietfdata](https://github.com/glasgow-ipl/ietfdata) - Access the IETF Datatracker and related resources
 =============================================================
 
 This project contains Python 3 libraries to interact with, and
 access, the [IETF datatracker](https://datatracker.ietf.org), 
 [RFC index](https://www.rfc-editor.org), and related resources.
```

### Comparing `ietfdata-0.6.8/examples/bluesheets.py` & `ietfdata-0.7.0/examples/bluesheets.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/draft-authors.py` & `ietfdata-0.7.0/examples/draft-authors.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/draft-references.py` & `ietfdata-0.7.0/examples/draft-references.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/draft-submissions-by-date.py` & `ietfdata-0.7.0/examples/draft-submissions-by-date.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/draft-submissions.py` & `ietfdata-0.7.0/examples/draft-submissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,9 +31,11 @@
 from ietfdata.datatracker import *
 
 dt  = DataTracker()
 doc = dt.document_from_draft("draft-ietf-eppext-keyrelay")
 for submit_url in doc.submissions:
     submit = dt.submission(submit_url)
     print(f"{submit.name}-{submit.rev} {submit.submission_date}")
+    for a in submit.parse_authors():
+        print(f"  {a}")
```

### Comparing `ietfdata-0.6.8/examples/drafts-for-person.py` & `ietfdata-0.7.0/examples/drafts-for-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/drafts-for-rfc.py` & `ietfdata-0.7.0/examples/drafts-for-rfc.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/drafts-for-wg.py` & `ietfdata-0.7.0/examples/drafts-for-wg.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/emails-per-person.py` & `ietfdata-0.7.0/examples/emails-per-person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/ietf-leadership.py` & `ietfdata-0.7.0/examples/ietf-leadership.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/non-wg-standards-track-rfcs.py` & `ietfdata-0.7.0/examples/non-wg-standards-track-rfcs.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/org-chart.py` & `ietfdata-0.7.0/examples/org-chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,19 @@
 # Example: print an organisational chart for the IETF
 
 dt = DataTracker()
 
 def print_group(group : Group, level : int):
     for i in range(0, level):
         print("  ", end="")
-    print(group.name)
+    group_type = (dt.group_type_name(group.type).name)
+    if group_type == "SDO":
+        pass
+    else:
+        print(f"{group.name} ({group_type})")
     for g in dt.groups(parent = group, state = dt.group_state_from_slug("active")):
         print_group(g, level + 1)
 
 print_group(dt.group_from_acronym("ietf"), 0)
 print_group(dt.group_from_acronym("irtf"), 0)
 
 # =============================================================================
```

### Comparing `ietfdata-0.6.8/examples/person-attendance.py` & `ietfdata-0.7.0/examples/person-attendance.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/person-emails.py` & `ietfdata-0.7.0/examples/person-emails.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/person.py` & `ietfdata-0.7.0/examples/person.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/recent-pubreq.py` & `ietfdata-0.7.0/examples/recent-pubreq.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/rfc-data.py` & `ietfdata-0.7.0/examples/rfc-data.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/rfc-streams.py` & `ietfdata-0.7.0/examples/rfc-streams.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/examples/role-names.py` & `ietfdata-0.7.0/examples/role-names.py`

 * *Files identical despite different names*

### Comparing `ietfdata-0.6.8/ietfdata/datatracker.py` & `ietfdata-0.7.0/ietfdata/datatracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2017-2022 University of Glasgow
+# Copyright (C) 2017-2023 University of Glasgow
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -49,192 +49,215 @@
 import dateutil.tz
 import glob
 import json
 import logging
 import os
 import re
 import requests
+import requests_cache
 import sys
 import time
 import urllib.parse
 
-from datetime         import datetime, timedelta, timezone
+from datetime         import date, datetime, timedelta, timezone
 from enum             import Enum
 from inspect          import signature
 from typing           import List, Optional, Tuple, Dict, Iterator, Type, TypeVar, Any, Union, Generic, get_origin
+from typing_extensions import Self
 from dataclasses      import dataclass, field
 from pathlib          import Path
-from pavlova          import Pavlova
-from pavlova.parsers  import GenericParser
+from pydantic         import BaseModel, ValidationError, model_validator
 from pymongo          import MongoClient, ASCENDING, TEXT, ReplaceOne
 from pymongo.database import Database
-from requests_cache   import CacheMixin, MongoCache, DO_NOT_CACHE
-from requests_ratelimiter import LimiterMixin
-
-class CachedLimiterSession(CacheMixin, LimiterMixin, requests.Session):
-    """
-    Session class with caching and rate-limiting behavior. Accepts arguments for both
-    LimiterSession and CachedSession.
-    """
 
 # =================================================================================================================================
 # Classes to represent the JSON-serialised objects returned by the Datatracker API:
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # URI types:
 
-@dataclass(frozen=True)
-class URI:
+class URI(BaseModel):
     uri    : Optional[str]
     root   : str = ""
     params : Dict[str, Any] = field(default_factory=dict)
 
     def __str__(self) -> str:
         if len(self.params) > 0:
             return F"{self.uri}?{urllib.parse.urlencode(self.params)}"
         else:
             return str(self.uri)
 
-    def __post_init__(self) -> None:
-        assert self.uri is None or self.uri.startswith(self.root)
+    # https://stackoverflow.com/a/77647989
+    @model_validator(mode="before")
+    @classmethod
+    def from_literal(cls, data: Any) -> Any:
+        if isinstance(data, str):
+            return {"uri" : data}
+        else:
+            return data
 
 
-@dataclass(frozen=True)
 class DocumentURI(URI):
     root : str = "/api/v1/doc/document/"
 
 
-@dataclass(frozen=True)
 class GroupURI(URI):
     root : str = "/api/v1/group/group/"
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Resource type
 
-@dataclass(frozen=True)
-class Resource:
+class Resource(BaseModel):
     resource_uri : URI
 
 T = TypeVar('T', bound=Resource)
 R = TypeVar('R', bound=Type[Resource])
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to people:
 
-@dataclass(frozen=True)
 class PersonURI(URI):
     root : str = "/api/v1/person/person/"
 
 
-@dataclass(frozen=True)
 class HistoricalPersonURI(URI):
     root : str = "/api/v1/person/historicalperson/"
 
 
-@dataclass(frozen=True)
 class Person(Resource):
     resource_uri    : PersonURI
     id              : int
     name            : str            # Full name in Unicode
-    name_from_draft : str
+    name_from_draft : Optional[str]
     ascii           : str            # Name as rendered in ASCII
     # ascii_short: Fill in this with initials and surname only if taking the initials
     # and surname of the ASCII name above produces an incorrect initials-only form.
     ascii_short     : Optional[str]
-    user            : str
+    user            : Optional[str]
     time            : datetime
-    photo           : str
-    photo_thumb     : str
+    photo           : Optional[str]
+    photo_thumb     : Optional[str]
     biography       : str
-    # Plain name correction: Use this if you have a Spanish double surname.
-    # Don't use this for nicknames, and don't use it unless you've actually
-    # observed that the datatracker shows your name incorrectly."
+    # Plain name correction: Use this if you have a Spanish double surname.
+    # Don't use this for nicknames, and don't use it unless you've actually
+    # observed that the datatracker shows your name incorrectly."
     plain           : str
-    pronouns_freetext     : str
+    pronouns_freetext     : Optional[str]
     pronouns_selectable   : str
 
 
-@dataclass(frozen=True)
 class HistoricalPerson(Resource):
     resource_uri          : HistoricalPersonURI
     id                    : int
     name                  : str
-    name_from_draft       : str
+    name_from_draft       : Optional[str]
     ascii                 : str
     ascii_short           : Optional[str]
-    user                  : str
+    user                  : Optional[str]
     time                  : datetime
-    photo                 : str
-    photo_thumb           : str
+    photo                 : Optional[str]
+    photo_thumb           : Optional[str]
     biography             : str
     history_change_reason : Optional[str]
     history_user          : Optional[str]
     history_id            : int
     history_type          : str
     history_date          : datetime
     plain                 : str
-    pronouns_freetext     : str
+    pronouns_freetext     : Optional[str]
     pronouns_selectable   : str
 
 
-@dataclass(frozen=True)
 class PersonAliasURI(URI):
     root : str = "/api/v1/person/alias/"
 
 
-@dataclass(frozen=True)
 class PersonAlias(Resource):
     id                 : int
     resource_uri       : PersonAliasURI
     person             : PersonURI
     name               : str
 
 
-@dataclass(frozen=True)
 class PersonEventURI(URI):
     root : str = "/api/v1/person/personevent/"
 
 
-@dataclass(frozen=True)
 class PersonEvent(Resource):
     desc            : str
     id              : int
     person          : PersonURI
     resource_uri    : PersonEventURI
     time            : datetime
     type            : str
 
 
+class ExtResourceTypeNameURI(URI):
+    root : str = "/api/v1/name/extresourcetypename/"
+
+
+class ExtResourceTypeName(Resource):
+    resource_uri : ExtResourceTypeNameURI
+    desc         : str
+    name         : str
+    order        : int
+    slug         : str
+    used         : bool
+
+
+class ExtResourceNameURI(URI):
+    root : str = "/api/v1/name/extresourcename/"
+
+
+class ExtResourceName(Resource):
+    resource_uri  : ExtResourceNameURI
+    type          : ExtResourceTypeNameURI
+    desc          : str
+    name          : str
+    order         : int
+    slug          : str
+    used          : bool
+
+
+class PersonExtResourceURI(URI):
+    root : str = "/api/v1/person/personextresource/"
+
+
+class PersonExtResource(Resource):
+    id           : int
+    resource_uri : PersonExtResourceURI
+    display_name : str
+    person       : PersonURI
+    name         : ExtResourceNameURI
+    value        : str
+
+
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to email addresses:
 
-@dataclass(frozen=True)
 class EmailURI(URI):
     root : str = "/api/v1/person/email/"
 
 
-@dataclass(frozen=True)
 class HistoricalEmailURI(URI):
     root : str = "/api/v1/person/historicalemail/"
 
 
-@dataclass(frozen=True)
 class Email(Resource):
     resource_uri : EmailURI
     person       : Optional[PersonURI]
     address      : str # The email address
     time         : datetime
     origin       : str
     primary      : bool
     active       : bool
 
 
-@dataclass(frozen=True)
 class HistoricalEmail(Resource):
     resource_uri          : HistoricalEmailURI
     person                : Optional[PersonURI]
     address               : str # The email address
     time                  : datetime
     origin                : str
     primary               : bool
@@ -245,108 +268,97 @@
     history_type          : str
     history_date          : datetime
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to documents:
 
-@dataclass(frozen=True)
 class DocumentTypeURI(URI):
     root : str = "/api/v1/name/doctypename/"
 
 
-@dataclass(frozen=True)
 class DocumentType(Resource):
     resource_uri : DocumentTypeURI
     name         : str
     used         : bool
     prefix       : str
     slug         : str
     desc         : str
     order        : int
 
 
-@dataclass(frozen=True)
 class DocumentStateTypeURI(URI):
     root : str = "/api/v1/doc/statetype/"
 
 
-@dataclass(frozen=True)
 class DocumentStateType(Resource):
     resource_uri : DocumentStateTypeURI
     label        : str
     slug         : str
 
 
-@dataclass(frozen=True)
 class DocumentStateURI(URI):
     root : str = "/api/v1/doc/state/"
 
 
-@dataclass(frozen=True)
 class DocumentState(Resource):
     id           : int
     resource_uri : DocumentStateURI
     desc         : str
     name         : str
     next_states  : List[DocumentStateURI]
     order        : int
     slug         : str  # FIXME: should we introduce a StateSlug type (and similar for the other slug fields)?
     type         : DocumentStateTypeURI
     used         : bool
 
 
-@dataclass(frozen=True)
 class StreamURI(URI):
     root : str = "/api/v1/name/streamname/"
 
 
-@dataclass(frozen=True)
 class Stream(Resource):
     resource_uri : StreamURI
     name         : str
     desc         : str
     used         : bool
     slug         : str
     order        : int
 
 
-@dataclass(frozen=True)
 class SubmissionURI(URI):
     root : str = "/api/v1/submit/submission/"
 
 
-@dataclass(frozen=True)
 class SubmissionCheckURI(URI):
     root : str = "/api/v1/submit/submissioncheck/"
 
 
-@dataclass(frozen=True)
 class Submission(Resource):
     abstract        : str
     access_key      : str
     auth_key        : str
     authors         : str   # See the parse_authors() method
     checks          : List[SubmissionCheckURI]
-    document_date   : Optional[datetime]
+    document_date   : Optional[date]
     draft           : DocumentURI
     file_size       : Optional[int]
-    file_types      : str   # e.g., ".txt,.xml"
+    file_types      : str   # e.g., ".txt,.xml"
     group           : Optional[GroupURI]
     id              : int
     name            : str
     note            : str
     pages           : Optional[int]
     remote_ip       : str
     replaces        : str   # This is a comma separated list of draft names (e.g., "draft-dkg-hrpc-glossary,draft-varon-hrpc-methodology")
                             # although in most cases there is only one entry, and hence no comma.
     resource_uri    : SubmissionURI
     rev             : str
     state           : str   # FIXME: this should be a URI subtype
-    submission_date : datetime
+    submission_date : date
     submitter       : str
     title           : str
     words           : Optional[int]
     xml_version     : Optional[str]
 
     """
     URLs from which this submission can be downloaded.
@@ -356,60 +368,73 @@
             yield (file_type, "https://www.ietf.org/archive/id/"  + self.name + "-" + self.rev + file_type)
 
     def parse_authors(self) -> List[Dict[str,str]]:
         authors = ast.literal_eval(self.authors) # type: List[Dict[str, str]]
         return authors
 
 
-@dataclass(frozen=True)
 class SubmissionEventURI(URI):
     root : str = "/api/v1/submit/submissionevent/"
 
 
-@dataclass(frozen=True)
 class SubmissionEvent(Resource):
     by              : Optional[PersonURI]
     desc            : str
     id              : int
     resource_uri    : SubmissionEventURI
     submission      : SubmissionURI
     time            : datetime
 
 
-@dataclass(frozen=True)
+class DocumentUrlTagURI(URI):
+    root : str = "/api/v1/name/docurltagname/"
+
+
+class DocumentUrlURI(URI):
+    root : str = "/api/v1/doc/documenturl/"
+    
+    
+class DocumentUrl(Resource):
+    desc         : str
+    doc          : DocumentURI
+    id           : int
+    resource_uri : DocumentUrlURI
+    tag          : DocumentUrlTagURI
+    url          : str
+
+
 class DocumentTagURI(URI):
     root : str = "/api/v1/name/doctagname/"
 
 
-@dataclass(frozen=True)
 class DocumentTag(Resource):
     resource_uri  : DocumentTagURI
     slug          : str
     order         : int
     name          : str
     used          : bool
     desc          : str
 
 
 # DocumentURI is defined earlier, to avoid circular dependencies
 
-@dataclass(frozen=True)
 class Document(Resource):
     id                 : int
     resource_uri       : DocumentURI
     name               : str
     title              : str
     pages              : Optional[int]
     words              : Optional[int]
     time               : datetime
     notify             : str
     expires            : Optional[str]
     type               : DocumentTypeURI
-    rfc                : Optional[int]
-    rev                : str           # If `rfc` is not None, `rev` will point to the RFC publication notice
+    rfc                : Optional[str]
+    rfc_number         : Optional[int]
+    rev                : str
     abstract           : str
     internal_comments  : str
     note               : str
     ad                 : Optional[PersonURI]
     shepherd           : Optional[EmailURI]
     group              : Optional[GroupURI]
     stream             : Optional[StreamURI]
@@ -423,180 +448,153 @@
 
     def __post_init__(self) -> None:
         assert self.intended_std_level is None or self.intended_std_level.startswith("/api/v1/name/intendedstdlevelname/")
         assert self.std_level          is None or self.std_level.startswith("/api/v1/name/stdlevelname/")
 
     def url(self) -> str:
         # See https://trac.tools.ietf.org/tools/ietfdb/browser/trunk/ietf/settings.py and search for DOC_HREFS
-        if self.type == DocumentTypeURI("/api/v1/name/doctypename/agenda/"):
+        if self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/agenda/"):
             # FIXME: should be "/meeting/{meeting.number}/materials/{doc.name}-{doc.rev}" ???
             # FIXME: This doesn't work for interim meetings
             # FIXME: This doesn't work for PDF agenda files
             # FIXME: Older items are under, e.g., https://www.ietf.org/proceedings/90/agenda/agenda-90-precis.txt
             mtg = self.name.split("-")[1]
             # Recent documents are in the datatracker, older ones on the proceedings site
             url = "https://datatracker.ietf.org/meeting/" + mtg + "/materials/" + self.uploaded_filename
             url = "https://www.ietf.org/proceedings/" + mtg + "/agenda/" + self.uploaded_filename
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/bluesheets/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/bluesheets/"):
             mtg = self.name.split("-")[1]
             if mtg == "interim":
                 mtg = "-".join(self.name.split("-")[1:-1])
             url = "https://www.ietf.org/proceedings/" + mtg + "/bluesheets/" + self.uploaded_filename
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/charter/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/charter/"):
             url = "https://www.ietf.org/charter/"     + self.name + "-" + self.rev + ".txt"
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/conflrev/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/conflrev/"):
             url = "https://www.ietf.org/cr/"          + self.name + "-" + self.rev + ".txt"
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/draft/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/draft/"):
             url = "https://www.ietf.org/archive/id/"  + self.name + "-" + self.rev + ".txt"
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/liaison/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/liaison/"):
             url = "https://www.ietf.org/lib/dt/documents/LIAISON/" + self.uploaded_filename
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/liai-att/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/liai-att/"):
             url = "https://www.ietf.org/lib/dt/documents/LIAISON/" + self.uploaded_filename
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/minutes/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/minutes/"):
             mtg = self.name.split("-")[1]
             # Recent documents are in the datatracker, older ones on the proceedings site
             url = "https://datatracker.ietf.org/meeting/" + mtg + "/materials/" + self.uploaded_filename
             url = "https://www.ietf.org/proceedings/" + mtg + "/minutes/" + self.uploaded_filename
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/recording/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/recording/"):
             url = self.external_url
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/review/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/review/"):
             # FIXME: This points to the formatted HTML page containing the message, but we really want the raw message
             url = "https://datatracker.ietf.org/doc/" + self.name
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/shepwrit/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/shepwrit/"):
             url = self.external_url
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/slides/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/slides/"):
             # FIXME: should be https://www.ietf.org/slides/{doc.name}-{doc.rev} ???
             mtg = self.name.split("-")[1]
             url = "https://www.ietf.org/proceedings/" + mtg + "/slides/" + self.uploaded_filename
-        elif self.type == DocumentTypeURI("/api/v1/name/doctypename/statchg/"):
+        elif self.type == DocumentTypeURI(uri="/api/v1/name/doctypename/statchg/"):
             url = "https://www.ietf.org/sc/"          + self.name + "-" + self.rev + ".txt"
         else:
             raise NotImplementedError
         return url
 
 
-@dataclass(frozen=True)
-class DocumentAliasURI(URI):
-    root : str = "/api/v1/doc/docalias/"
-
-
-@dataclass(frozen=True)
-class DocumentAlias(Resource):
-    id           : int
-    resource_uri : DocumentAliasURI
-    document     : DocumentURI
-    name         : str
-
-
-@dataclass(frozen=True)
 class DocumentEventURI(URI):
     root : str = "/api/v1/doc/docevent/"
 
 
-@dataclass(frozen=True)
 class DocumentEvent(Resource):
     by              : PersonURI
     desc            : str
     doc             : DocumentURI
     id              : int
     resource_uri    : DocumentEventURI
     rev             : str
     time            : datetime
     type            : str
 
 
-@dataclass(frozen=True)
 class BallotPositionNameURI(URI):
     root : str = "/api/v1/name/ballotpositionname/"
 
 
-@dataclass(frozen=True)
 class BallotPositionName(Resource):
     blocking     : bool
     desc         : Optional[str]
     name         : str
     order        : int
     resource_uri : BallotPositionNameURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class BallotTypeURI(URI):
     root : str = "/api/v1/doc/ballottype/"
 
 
-@dataclass(frozen=True)
 class BallotType(Resource):
     doc_type     : DocumentTypeURI
     id           : int
     name         : str
     order        : int
     positions    : List[BallotPositionNameURI]
     question     : str
     resource_uri : BallotTypeURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class BallotDocumentEventURI(URI):
     root : str = "/api/v1/doc/ballotdocevent/"
 
 
-@dataclass(frozen=True)
 class BallotDocumentEvent(Resource):
     ballot_type     : BallotTypeURI
     by              : PersonURI
     desc            : str
     doc             : DocumentURI
     docevent_ptr    : DocumentEventURI
     id              : int
     resource_uri    : BallotDocumentEventURI
     rev             : str
     time            : datetime
     type            : str
 
 
-@dataclass(frozen=True)
 class RelationshipTypeURI(URI):
     root : str = "/api/v1/name/docrelationshipname/"
 
 
-@dataclass(frozen=True)
 class RelationshipType(Resource):
     resource_uri   : RelationshipTypeURI
     slug           : str
     desc           : str
     name           : str
     used           : bool
     order          : int
     revname        : str
 
 
-@dataclass(frozen=True)
 class RelatedDocumentURI(URI):
     root : str = "/api/v1/doc/relateddocument/"
 
 
-@dataclass(frozen=True)
 class RelatedDocument(Resource):
     id              : int
     relationship    : RelationshipTypeURI
     resource_uri    : RelatedDocumentURI
     source          : DocumentURI
-    target          : DocumentAliasURI
+    target          : DocumentURI
 
 
-@dataclass(frozen=True)
 class DocumentAuthorURI(URI):
     root : str = "/api/v1/doc/documentauthor/"
 
 
-@dataclass(frozen=True)
 class DocumentAuthor(Resource):
     id           : int
     order        : int
     resource_uri : DocumentAuthorURI
     country      : str
     affiliation  : str
     document     : DocumentURI
@@ -605,49 +603,44 @@
 
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to groups:
 
 
-@dataclass(frozen=True)
 class GroupStateURI(URI):
     root : str = "/api/v1/name/groupstatename/"
 
 
-@dataclass(frozen=True)
 class GroupState(Resource):
     resource_uri   : GroupStateURI
     slug           : str
     desc           : str
     name           : str
     used           : bool
     order          : int
 
 
-@dataclass(frozen=True)
 class GroupTypeNameURI(URI):
     root : str = "/api/v1/name/grouptypename/"
 
 
-@dataclass(frozen=True)
 class GroupTypeName(Resource):
     desc          : str
     name          : str
     order         : int
     resource_uri  : GroupTypeNameURI
     slug          : str
     used          : bool
     verbose_name  : str
 
 
 # GroupURI is defined earlier, to avoid circular dependencies
 
 
-@dataclass(frozen=True)
 class Group(Resource):
     acronym        : str
     ad             : Optional[PersonURI]
     charter        : Optional[DocumentURI]
     comments       : str
     description    : str
     id             : int
@@ -663,20 +656,18 @@
     unused_states  : List[DocumentStateURI]
     unused_tags    : List[str]
     meeting_seen_as_area : bool
     used_roles           : str
     uses_milestone_dates : bool
 
 
-@dataclass(frozen=True)
 class GroupHistoryURI(URI):
     root : str = "/api/v1/group/grouphistory/"
 
 
-@dataclass(frozen=True)
 class GroupHistory(Resource):
     acronym              : str
     ad                   : Optional[PersonURI]
     comments             : str
     description          : str
     group                : GroupURI
     id                   : int
@@ -692,166 +683,146 @@
     unused_states        : List[DocumentStateURI]
     unused_tags          : List[str]
     uses_milestone_dates : bool
     meeting_seen_as_area : bool
     used_roles           : str
 
 
-@dataclass(frozen=True)
 class GroupEventURI(URI):
     root : str = "/api/v1/group/groupevent/"
 
 
-@dataclass(frozen=True)
 class GroupEvent(Resource):
     by           : PersonURI
     desc         : str
     group        : GroupURI
     id           : int
     resource_uri : GroupEventURI
     time         : datetime
     type         : str
 
 
-@dataclass(frozen=True)
 class GroupUrlURI(URI):
     root : str = "/api/v1/group/groupurl/"
 
 
-@dataclass(frozen=True)
 class GroupUrl(Resource):
     group        : GroupURI
     id           : int
     name         : str
     resource_uri : GroupUrlURI
     url          : str
 
 
-@dataclass(frozen=True)
 class GroupMilestoneStateNameURI(URI):
     root : str = "/api/v1/name/groupmilestonestatename/"
 
 
-@dataclass(frozen=True)
 class GroupMilestoneStateName(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : GroupMilestoneStateNameURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class GroupMilestoneURI(URI):
     root : str = "/api/v1/group/groupmilestone/"
 
 
-@dataclass(frozen=True)
 class GroupMilestone(Resource):
     desc         : str
     docs         : List[DocumentURI]
     due          : str
     group        : GroupURI
     id           : int
     order        : Optional[int]
     resolved     : str
     resource_uri : GroupMilestoneURI
     state        : GroupMilestoneStateNameURI
     time         : datetime
 
 
-@dataclass(frozen=True)
 class RoleNameURI(URI):
     root : str = "/api/v1/name/rolename/"
 
 
-@dataclass(frozen=True)
 class RoleName(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : RoleNameURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class GroupRoleURI(URI):
     root : str = "/api/v1/group/role/"
 
 
-@dataclass(frozen=True)
 class GroupRole(Resource):
     email        : EmailURI
     group        : GroupURI
     id           : int
     name         : RoleNameURI
     person       : PersonURI
     resource_uri : GroupRoleURI
 
-@dataclass(frozen=True)
 class GroupMilestoneHistoryURI(URI):
     root : str = "/api/v1/group/groupmilestonehistory/"
 
 
-@dataclass(frozen=True)
 class GroupMilestoneHistory(Resource):
     desc         : str
     docs         : List[DocumentURI]
     due          : str
     group        : GroupURI
     id           : int
     milestone    : GroupMilestoneURI
     order        : Optional[int]
     resolved     : str
     resource_uri : GroupMilestoneHistoryURI
     state        : GroupMilestoneStateNameURI
     time         : datetime
 
 
-@dataclass(frozen=True)
 class GroupMilestoneEventURI(URI):
     root : str = "/api/v1/group/milestonegroupevent/"
 
 
-@dataclass(frozen=True)
 class GroupMilestoneEvent(Resource):
     by             : PersonURI
     desc           : str
     group          : GroupURI
     groupevent_ptr : GroupEventURI
     id             : int
     milestone      : GroupMilestoneURI
     resource_uri   : GroupMilestoneEventURI
     time           : datetime
     type           : str
 
 
-@dataclass(frozen=True)
 class GroupRoleHistoryURI(URI):
     root : str = "/api/v1/group/rolehistory/"
 
 
-@dataclass(frozen=True)
 class GroupRoleHistory(Resource):
     email        : EmailURI
     group        : GroupHistoryURI
     id           : int
     name         : RoleNameURI
     person       : PersonURI
     resource_uri : GroupRoleHistoryURI
 
 
-@dataclass(frozen=True)
 class GroupStateChangeEventURI(URI):
     root : str = "/api/v1/group/changestategroupevent/"
 
 
-@dataclass(frozen=True)
 class GroupStateChangeEvent(Resource):
     by             : PersonURI
     desc           : str
     group          : GroupURI
     groupevent_ptr : GroupEventURI
     id             : int
     resource_uri   : GroupStateChangeEventURI
@@ -865,40 +836,35 @@
 
 class MeetingStatus(Enum):
     FUTURE    = 1
     ONGOING   = 2
     COMPLETED = 3
 
 
-@dataclass(frozen=True)
 class MeetingURI(URI):
     root : str = "/api/v1/meeting/meeting/"
 
 
-@dataclass(frozen=True)
 class MeetingTypeURI(URI):
     root : str = "/api/v1/name/meetingtypename/"
 
 
-@dataclass(frozen=True)
 class MeetingType(Resource):
     name         : str
     order        : int
     resource_uri : MeetingTypeURI
     slug         : str
     desc         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class ScheduleURI(URI):
     root : str = "/api/v1/meeting/schedule/"
 
 
-@dataclass(frozen=True)
 class Schedule(Resource):
     """
     A particular version of the meeting schedule (i.e., the meeting agenda)
 
     Use `meeting_session_assignments()` to find the assignment of sessions
     to timeslots within this schedule.
     """
@@ -909,24 +875,23 @@
     meeting      : MeetingURI
     visible      : bool
     public       : bool
     badness      : Optional[str]
     notes        : str
 
 
-@dataclass(frozen=True)
 class Meeting(Resource):
     id                               : int
     resource_uri                     : MeetingURI
     type                             : MeetingTypeURI
     country                          : str
     city                             : str
     venue_name                       : str
     venue_addr                       : str
-    date                             : datetime
+    date                             : date
     days                             : int  # FIXME: this should be a timedelta object
     time_zone                        : str
     acknowledgements                 : str
     agenda_info_note                 : str
     agenda_warning_note              : str
     session_request_lock_message     : str
     idsubmit_cutoff_warning_days     : str
@@ -954,45 +919,40 @@
             return MeetingStatus.FUTURE
         elif meeting_end < now:
             return MeetingStatus.COMPLETED
         else:
             return MeetingStatus.ONGOING
 
 
-@dataclass(frozen=True)
 class SessionURI(URI):
     root : str = "/api/v1/meeting/session/"
 
 
-@dataclass(frozen=True)
 class TimeslotURI(URI):
     root : str = "/api/v1/meeting/timeslot/"
 
 
-@dataclass(frozen=True)
 class Timeslot(Resource):
     id            : int
     resource_uri  : TimeslotURI
     type          : str               # FIXME: this is a URI "/api/v1/name/timeslottypename/regular/"
     meeting       : MeetingURI
     sessions      : List[SessionURI]  # Sessions assigned to this slot in various versions of the agenda; current assignment is last
     name          : str
     time          : datetime
-    duration      : str               # FIXME: this should be a timedelta object
-    location      : Optional[str]     # FIXME: this is a URI "/api/v1/meeting/room/668"
+    duration      : str               # FIXME: this should be a timedelta object
+    location      : Optional[str]     # FIXME: this is a URI "/api/v1/meeting/room/668"
     show_location : bool
     modified      : datetime
 
 
-@dataclass(frozen=True)
 class SessionAssignmentURI(URI):
     root : str = "/api/v1/meeting/schedtimesessassignment/"
 
 
-@dataclass(frozen=True)
 class SessionAssignment(Resource):
     """
     The assignment of a `session` to a `timeslot` within a meeting `schedule`
     """
     id           : int
     resource_uri : SessionAssignmentURI
     session      : SessionURI
@@ -1002,32 +962,29 @@
     modified     : datetime
     notes        : str
     pinned       : bool
     extendedfrom : Optional[str]
     badness      : int
 
 
-@dataclass(frozen=True)
 class SessionPurposeURI(URI):
     root : str = "/api/v1/name/sessionpurposename/"
 
 
-@dataclass(frozen=True)
 class SessionPurpose(Resource):
     resource_uri   : SessionPurposeURI
     used           : bool
     timeslot_types : str
     order          : int
     on_agenda      : bool
     name           : str
     desc           : str
     slug           : str
 
 
-@dataclass(frozen=True)
 class Session(Resource):
     """
     A session within a meeting.
 
     Note that a Session object is created, and will be assigned to a
     Timeslot, when a Meeting is requested, not when it is scheduled.
     Use the `meeting_session_status()` method to check if the session
@@ -1052,91 +1009,81 @@
     comments            : str
     on_agenda           : bool
     purpose             : SessionPurposeURI
     has_onsite_tool     : bool
     chat_room           : str
 
 
-@dataclass(frozen=True)
 class SessionStatusNameURI(URI):
     root : str = "/api/v1/name/sessionstatusname/"
 
 
-@dataclass(frozen=True)
 class SessionStatusName(Resource):
     order        : int
     slug         : str
     resource_uri : SessionStatusNameURI
     used         : bool
     desc         : str
     name         : str
 
 
-@dataclass(frozen=True)
 class SchedulingEventURI(URI):
     root : str = "/api/v1/meeting/schedulingevent/"
 
 
-@dataclass(frozen=True)
 class SchedulingEvent(Resource):
     id           : int
     session      : SessionURI
     status       : SessionStatusNameURI
     by           : PersonURI
     resource_uri : SchedulingEventURI
     time         : datetime
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to IPR disclosures:
 
-@dataclass(frozen=True)
 class IPRDisclosureStateURI(URI):
     root : str = "/api/v1/name/iprdisclosurestatename/"
 
 
-@dataclass(frozen=True)
 class IPRDisclosureState(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : IPRDisclosureStateURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class IPRDisclosureBaseURI(URI):
     root : str = "/api/v1/ipr/iprdisclosurebase/"
 
 
-@dataclass(frozen=True)
 class IPRDisclosureBase(Resource):
     by                 : PersonURI
     compliant          : bool
-    docs               : List[DocumentAliasURI]
+    docs               : List[DocumentURI]
     holder_legal_name  : str
     id                 : int
     notes              : str
     other_designations : str
     rel                : List[IPRDisclosureBaseURI]
     resource_uri       : IPRDisclosureBaseURI
     state              : IPRDisclosureStateURI
     submitter_email    : str
     submitter_name     : str
     time               : datetime
     title              : str
 
 
-@dataclass(frozen=True)
 class GenericIPRDisclosureURI(URI):
     root : str = "/api/v1/ipr/genericiprdisclosure/"
 
 
-@dataclass(frozen=True)
 class GenericIPRDisclosure(Resource):
     by                    : PersonURI
     compliant             : bool
     docs                  : List[DocumentURI]
     holder_contact_email  : str
     holder_contact_info   : str
     holder_contact_name   : str
@@ -1151,39 +1098,35 @@
     statement             : str
     submitter_email       : str
     submitter_name        : str
     time                  : datetime
     title                 : str
 
 
-@dataclass(frozen=True)
 class IPRLicenseTypeURI(URI):
     root : str = "/api/v1/name/iprlicensetypename/"
 
 
-@dataclass(frozen=True)
 class IPRLicenseType(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : IPRLicenseTypeURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class HolderIPRDisclosureURI(URI):
     root : str = "/api/v1/ipr/holderiprdisclosure/"
 
 
-@dataclass(frozen=True)
 class HolderIPRDisclosure(Resource):
     by                                   : PersonURI
     compliant                            : bool
-    docs                                 : List[DocumentAliasURI]
+    docs                                 : List[DocumentURI]
     has_patent_pending                   : bool
     holder_contact_email                 : str
     holder_contact_info                  : str
     holder_contact_name                  : str
     holder_legal_name                    : str
     id                                   : int
     ietfer_contact_email                 : str
@@ -1201,24 +1144,22 @@
     submitter_claims_all_terms_disclosed : bool
     submitter_email                      : str
     submitter_name                       : str
     time                                 : datetime
     title                                : str
 
 
-@dataclass(frozen=True)
 class ThirdPartyIPRDisclosureURI(URI):
     root : str = "/api/v1/ipr/thirdpartyiprdisclosure/"
 
 
-@dataclass(frozen=True)
 class ThirdPartyIPRDisclosure(Resource):
     by                     : PersonURI
     compliant              : bool
-    docs                   : List[DocumentAliasURI]
+    docs                   : List[DocumentURI]
     has_patent_pending     : bool
     holder_legal_name      : str
     id                     : int
     ietfer_contact_email   : str
     ietfer_contact_info    : str
     ietfer_name            : str
     iprdisclosurebase_ptr  : IPRDisclosureBaseURI
@@ -1233,135 +1174,119 @@
     time                   : datetime
     title                  : str
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to reviews:
 
-@dataclass(frozen=True)
 class ReviewAssignmentStateURI(URI):
     root : str = "/api/v1/name/reviewassignmentstatename/"
 
 
-@dataclass(frozen=True)
 class ReviewAssignmentState(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : ReviewAssignmentStateURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class ReviewResultTypeURI(URI):
     root : str = "/api/v1/name/reviewresultname/"
 
 
-@dataclass(frozen=True)
 class ReviewResultType(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : ReviewResultTypeURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class ReviewTypeURI(URI):
     root : str = "/api/v1/name/reviewtypename/"
 
 
-@dataclass(frozen=True)
 class ReviewType(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : ReviewTypeURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class ReviewRequestStateURI(URI):
     root : str = "/api/v1/name/reviewrequeststatename/"
 
 
-@dataclass(frozen=True)
 class ReviewRequestState(Resource):
     desc         : str
     name         : str
     order        : int
     resource_uri : ReviewRequestStateURI
     slug         : str
     used         : bool
 
 
-@dataclass(frozen=True)
 class ReviewRequestURI(URI):
     root : str = "/api/v1/review/reviewrequest/"
 
 
-@dataclass(frozen=True)
 class ReviewRequest(Resource):
     comment       : str
     deadline      : str
     doc           : DocumentURI
     id            : int
     requested_by  : PersonURI
     requested_rev : str
     resource_uri  : ReviewRequestURI
     state         : ReviewRequestStateURI
     team          : GroupURI
     time          : datetime
     type          : ReviewTypeURI
 
 
-@dataclass(frozen=True)
 class ReviewAssignmentURI(URI):
     root : str = "/api/v1/review/reviewassignment/"
 
 
-@dataclass(frozen=True)
 class ReviewAssignment(Resource):
     assigned_on    : datetime
     completed_on   : Optional[datetime]
     id             : int
     mailarch_url   : Optional[str] # can type?
     resource_uri   : ReviewAssignmentURI
     result         : Optional[ReviewResultTypeURI]
     review         : Optional[DocumentURI]
     review_request : ReviewRequestURI
     reviewed_rev   : str
     reviewer       : EmailURI
     state          : ReviewAssignmentStateURI
 
 
-@dataclass(frozen=True)
 class ReviewWishURI(URI):
     root : str = "/api/v1/review/reviewwish/"
 
 
-@dataclass(frozen=True)
 class ReviewWish(Resource):
     doc          : DocumentURI
     id           : int
     person       : PersonURI
     resource_uri : ReviewWishURI
     team         : GroupURI
     time         : datetime
 
 
-@dataclass(frozen=True)
 class HistoricalUnavailablePeriodURI(URI):
     root : str = "/api/v1/review/historicalunavailableperiod/"
 
 
-@dataclass(frozen=True)
 class HistoricalUnavailablePeriod(Resource):
     availability          : str
     end_date              : str
     history_change_reason : str
     history_date          : datetime
     history_id            : int
     history_type          : str
@@ -1369,20 +1294,18 @@
     person                : PersonURI
     reason                : str
     resource_uri          : HistoricalUnavailablePeriodURI
     start_date            : str
     team                  : GroupURI
 
 
-@dataclass(frozen=True)
 class HistoricalReviewRequestURI(URI):
     root : str = "/api/v1/review/historicalreviewrequest/"
 
 
-@dataclass(frozen=True)
 class HistoricalReviewRequest(Resource):
     comment               : str
     deadline              : str
     doc                   : DocumentURI
     history_change_reason : str
     history_date          : datetime
     history_id            : int
@@ -1393,88 +1316,79 @@
     resource_uri          : HistoricalReviewRequestURI
     state                 : ReviewRequestStateURI
     team                  : GroupURI
     time                  : datetime
     type                  : ReviewTypeURI
 
 
-@dataclass(frozen=True)
 class NextReviewerInTeamURI(URI):
     root : str = "/api/v1/review/nextreviewerinteam/"
 
 
-@dataclass(frozen=True)
 class NextReviewerInTeam(Resource):
     id            : int
     next_reviewer : PersonURI
     resource_uri  : NextReviewerInTeamURI
     team          : GroupURI
 
 
-@dataclass(frozen=True)
 class ReviewTeamSettingsURI(URI):
     root : str = "/api/v1/review/reviewteamsettings/"
 
 
-@dataclass(frozen=True)
 class ReviewTeamSettings(Resource):
-    autosuggest                         : bool
-    group                               : GroupURI
-    id                                  : int
-    notify_ad_when                      : List[ReviewResultTypeURI]
-    remind_days_unconfirmed_assignments : Optional[int]
-    resource_uri                        : ReviewTeamSettingsURI
-    review_results                      : List[ReviewResultTypeURI]
-    review_types                        : List[ReviewTypeURI]
-    secr_mail_alias                     : str
+    autosuggest                             : bool
+    group                                   : GroupURI
+    id                                      : int
+    notify_ad_when                          : List[ReviewResultTypeURI]
+    remind_days_unconfirmed_assignments     : Optional[int]
+    resource_uri                            : ReviewTeamSettingsURI
+    review_results                          : List[ReviewResultTypeURI]
+    review_types                            : List[ReviewTypeURI]
+    secr_mail_alias                         : str
+    allow_reviewer_to_reject_after_deadline : bool
 
 
-@dataclass(frozen=True)
 class ReviewerSettingsURI(URI):
     root : str = "/api/v1/review/reviewersettings/"
 
 
-@dataclass(frozen=True)
 class ReviewerSettings(Resource):
     expertise                   : str
     filter_re                   : str
     id                          : int
     min_interval                : Optional[int]
     person                      : PersonURI
     remind_days_before_deadline : Optional[int]
     remind_days_open_reviews    : Optional[int]
     request_assignment_next     : bool
     resource_uri                : ReviewerSettingsURI
     skip_next                   : int
     team                        : GroupURI
 
 
-@dataclass(frozen=True)
 class UnavailablePeriodURI(URI):
     root : str = "/api/v1/review/unavailableperiod/"
 
 
-@dataclass(frozen=True)
 class UnavailablePeriod(Resource):
     availability : str
     end_date     : str
     id           : int
     person       : PersonURI
     reason       : str
     resource_uri : UnavailablePeriodURI
     start_date   : Optional[str]
     team         : GroupURI
 
 
-@dataclass(frozen=True)
 class HistoricalReviewerSettingsURI(URI):
     root : str = "/api/v1/review/historicalreviewersettings/"
 
 
-@dataclass(frozen=True)
 class HistoricalReviewerSettings(Resource):
     expertise                   : str
     filter_re                   : str
     history_change_reason       : Optional[str]
     history_date                : datetime
     history_id                  : int
     history_type                : str
@@ -1486,20 +1400,18 @@
     remind_days_open_reviews    : Optional[int]
     request_assignment_next     : bool
     resource_uri                : HistoricalReviewerSettingsURI
     skip_next                   : int
     team                        : GroupURI
 
 
-@dataclass(frozen=True)
 class HistoricalReviewAssignmentURI(URI):
     root : str = "/api/v1/review/historicalreviewassignment/"
 
 
-@dataclass(frozen=True)
 class HistoricalReviewAssignment(Resource):
     assigned_on           : datetime
     completed_on          : datetime
     history_change_reason : str
     history_date          : datetime
     history_id            : int
     history_type          : str
@@ -1510,118 +1422,104 @@
     review                : DocumentURI
     review_request        : ReviewRequestURI
     reviewed_rev          : str
     reviewer              : EmailURI
     state                 : ReviewAssignmentStateURI
 
 
-@dataclass(frozen=True)
 class ReviewSecretarySettingsURI(URI):
     root : str = "/api/v1/review/reviewsecretarysettings/"
 
 
-@dataclass(frozen=True)
 class ReviewSecretarySettings(Resource):
     days_to_show_in_reviewer_list      : Optional[int]
     id                                 : int
     max_items_to_show_in_reviewer_list : Optional[int]
     person                             : PersonURI
     remind_days_before_deadline        : int
     resource_uri                       : ReviewSecretarySettingsURI
     team                               : GroupURI
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to mailing lists:
 
-@dataclass(frozen=True)
 class EmailListURI(URI):
     root : str = "/api/v1/mailinglists/list/"
 
 
-@dataclass(frozen=True)
 class EmailList(Resource):
     id           : int
     resource_uri : EmailListURI
     name         : str
     description  : str
     advertised   : bool
 
 
-@dataclass(frozen=True)
 class EmailListSubscriptionsURI(URI):
     root : str = "/api/v1/mailinglists/subscribed/"
 
 
-@dataclass(frozen=True)
 class EmailListSubscriptions(Resource):
     id           : int
     resource_uri : EmailListSubscriptionsURI
     email        : str
     lists        : List[EmailListURI]
     time         : datetime
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to places:
 
-@dataclass(frozen=True)
 class ContinentURI(URI):
     root : str = "/api/v1/name/continentname/"
 
 
-@dataclass(frozen=True)
 class Continent(Resource):
     resource_uri : ContinentURI
     desc         : str
     order        : int
     name         : str
     used         : bool
     slug         : str
 
 
-@dataclass(frozen=True)
 class CountryURI(URI):
     root : str = "/api/v1/name/countryname/"
 
 
-@dataclass(frozen=True)
 class Country(Resource):
     resource_uri : CountryURI
     desc         : str
     slug         : str
     in_eu        : bool
     order        : int
     used         : bool
     name         : str
     continent    : ContinentURI
 
 
-@dataclass(frozen=True)
 class CountryAliasURI(URI):
     root : str = "/api/v1/stats/countryalias/"
 
 
-@dataclass(frozen=True)
 class CountryAlias(Resource):
     id           : int
     resource_uri : CountryAliasURI
     country      : CountryURI
     alias        : str
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to statistics:
 
-@dataclass(frozen=True)
 class MeetingRegistrationURI(URI):
     root : str = "/api/v1/stats/meetingregistration/"
 
 
-@dataclass(frozen=True)
 class MeetingRegistration(Resource):
     affiliation  : str
     attended     : bool
     country_code : str
     email        : str
     first_name   : str
     id           : int
@@ -1634,34 +1532,30 @@
     checkedin    : bool
 
 
 # ---------------------------------------------------------------------------------------------------------------------------------
 # Types relating to messages:
 
 
-@dataclass(frozen=True)
 class AnnouncementFromURI(URI):
     root : str = "/api/v1/message/announcementfrom/"
 
 
-@dataclass(frozen=True)
 class AnnouncementFrom(Resource):
     address      : str
     group        : GroupURI
     id           : int
     name         : RoleNameURI
     resource_uri : AnnouncementFromURI
 
 
-@dataclass(frozen=True)
 class DTMessageURI(URI):
     root : str = "/api/v1/message/message/"
 
 
-@dataclass(frozen=True)
 class DTMessage(Resource):
     bcc            : str
     body           : str
     by             : PersonURI
     cc             : str
     content_type   : str
     frm            : str
@@ -1673,20 +1567,18 @@
     resource_uri   : DTMessageURI
     sent           : datetime
     subject        : str
     time           : datetime
     to             : str
 
 
-@dataclass(frozen=True)
 class SendQueueURI(URI):
     root : str = "/api/v1/message/sendqueue/"
 
 
-@dataclass(frozen=True)
 class SendQueueEntry(Resource):
     by             : PersonURI
     id             : int
     message        : DTMessageURI
     note           : str
     resource_uri   : SendQueueURI
     send_at        : Optional[datetime]
@@ -1706,86 +1598,69 @@
 
 class DataTracker:
     """
     A class for interacting with the IETF DataTracker.
     """
     db_conn : Optional[MongoClient]
     db      : Optional[Database]
-    backend : Optional[MongoCache]
+    backend : Optional[requests_cache.MongoCache]
 
     def __init__(self,
-            use_cache: bool = False,
-            mongodb_host: str = "localhost",
-            mongodb_port: int = 27017,
-            mongodb_user: Optional[str] = None,
-            mongodb_pass: Optional[str] = None,
-            cache_timeout: Optional[timedelta] = None):
-        if os.environ.get('IETFDATA_CACHE_HOST') is not None:
-            use_cache = True
-            cache_host = os.environ.get('IETFDATA_CACHE_HOST')
-            cache_port = os.environ.get('IETFDATA_CACHE_PORT', 27017)
-            cache_user = os.environ.get('IETFDATA_CACHE_USER')
-            cache_pass = os.environ.get('IETFDATA_CACHE_PASSWORD')
-            if cache_host is not None:
-                mongodb_host = cache_host
-            if cache_port is not None:
-                mongodb_port = int(cache_port)
-            if cache_user is not None:
-                mongodb_user = cache_user
-            if cache_pass is not None:
-                mongodb_pass = cache_pass
+                 use_cache     : bool = False,
+                 mongodb_host  : str  = os.getenv("IETFDATA_CACHE_HOST", "localhost"),
+                 mongodb_port  : str  = os.getenv("IETFDATA_CACHE_PORT", "27017"),
+                 mongodb_user  : Optional[str] = os.getenv("IETFDATA_CACHE_USER"),
+                 mongodb_pass  : Optional[str] = os.getenv("IETFDATA_CACHE_PASSWORD"),
+                 cache_timeout : Optional[timedelta] = None):
 
-        cache_limit = float(os.environ.get('IETFDATA_CACHE_RATELIMIT', "10000"))
+        if os.getenv("IETFDATA_CACHE_HOST") is not None:
+            use_cache = True
 
-        logging.getLogger('requests_cache').setLevel('WARN')
+        logging.getLogger('requests').setLevel('ERROR')
+        logging.getLogger('requests_cache').setLevel('ERROR')
+        logging.getLogger("urllib3").setLevel('ERROR')
 
         logging.basicConfig(level=os.environ.get("IETFDATA_LOGLEVEL", "INFO"))
         self.log = logging.getLogger("ietfdata")
 
-        self.ua        = "glasgow-ietfdata/0.6.8"          # Update when making a new relaase
+        self.ua        = "glasgow-ietfdata/0.7.0"          # Update when making a new relaase
         self.base_url  = os.environ.get("IETFDATA_DT_URL", "https://datatracker.ietf.org")
-        self.http_req  = 0
         self.get_count = 0
 
         if use_cache:
-            self.log.info(f"mongodb host = {mongodb_host}")
-            self.log.info(f"mongodb port = {mongodb_port}")
-            self.log.info(f"mongodb user = {mongodb_user}")
-            self.log.info(f"mongodb pass = {mongodb_pass}")
-            self.log.info(f"mongodb limit = {cache_limit}")
-            self.db_conn = MongoClient(host=mongodb_host, port=mongodb_port, username=mongodb_user, password=mongodb_pass)
+            self.log.warning(f"mongodb host = {mongodb_host}")
+            self.log.warning(f"mongodb port = {mongodb_port}")
+            self.log.warning(f"mongodb user = {mongodb_user}")
+            self.log.warning(f"mongodb pass = {mongodb_pass}")
+            self.db_conn = MongoClient(host  =mongodb_host,
+                                       port = int(mongodb_port),
+                                       username = mongodb_user,
+                                       password = mongodb_pass)
             self.db      = self.db_conn.ietfdata
-            self.backend = MongoCache(db_name="ietfdata_requests", connection=self.db_conn)
+            self.backend = requests_cache.MongoCache(db_name="ietfdata_requests", connection=self.db_conn)
             if cache_timeout is not None:
-                self.log.info(f"Cache enabled; timeout = {cache_timeout}")
-                self.session = CachedLimiterSession(backend=self.backend, expire_after=cache_timeout, per_second=cache_limit)
+                self.log.warning(f"Cache enabled; timeout = {cache_timeout}")
+                self.session = requests_cache.CachedSession(backend=self.backend, expire_after=cache_timeout)
             else:
-                self.log.info(f"Cache enabled; timeout = (auto)")
-                self.session = CachedLimiterSession(backend=self.backend, cache_control=True, per_second=cache_limit)
-            # check Datatracker and cache versions
-            self.cache_ver = "4" # Increment when changing cache architecture
-            self._cache_check_versions()
+                self.log.warning(f"Cache enabled; timeout = (auto)")
+                self.session = requests_cache.CachedSession(backend=self.backend, cache_control=True)
         else:
             self.log.warning("CACHE DISABLED")
             self.db_conn = None
             self.db      = None
             self.backend = None
-            self.session = CachedLimiterSession(expire_after=DO_NOT_CACHE, per_second=cache_limit)
-
-        self.pavlova = Pavlova()
-        for uri_type in URI.__subclasses__():
-            self.pavlova.register_parser(uri_type, GenericParser(self.pavlova, uri_type))
+            self.session = requests_cache.CachedSession(expire_after = requests_cache.DO_NOT_CACHE)
 
         self._hints = {} # type: Dict[str, Hints]
         self._hints["/api/v1/doc/ballotdocevent/"]                 = Hints(BallotDocumentEvent,         "id")
         self._hints["/api/v1/doc/ballottype/"]                     = Hints(BallotType,                  "slug")
-        self._hints["/api/v1/doc/docalias/"]                       = Hints(DocumentAlias,               "id")
         self._hints["/api/v1/doc/docevent/"]                       = Hints(DocumentEvent,               "id")
         self._hints["/api/v1/doc/document/"]                       = Hints(Document,                    "id")
         self._hints["/api/v1/doc/documentauthor/"]                 = Hints(DocumentAuthor,              "id")
+        self._hints["/api/v1/doc/documenturl/"]                    = Hints(DocumentUrl,                 "id")
         self._hints["/api/v1/doc/relateddocument/"]                = Hints(RelatedDocument,             "id")
         self._hints["/api/v1/doc/state/"]                          = Hints(DocumentState,               "id")
         self._hints["/api/v1/doc/statetype/"]                      = Hints(DocumentStateType,           "slug")
         self._hints["/api/v1/group/changestategroupevent/"]        = Hints(GroupStateChangeEvent,       "id")
         self._hints["/api/v1/group/group/"]                        = Hints(Group,                       "id")
         self._hints["/api/v1/group/groupevent/"]                   = Hints(GroupEvent,                  "id")
         self._hints["/api/v1/group/grouphistory/"]                 = Hints(GroupHistory,                "id")
@@ -1804,20 +1679,22 @@
         self._hints["/api/v1/meeting/meeting/"]                    = Hints(Meeting,                     "id")
         self._hints["/api/v1/meeting/schedtimesessassignment/"]    = Hints(SessionAssignment,           "id")
         self._hints["/api/v1/meeting/schedule/"]                   = Hints(Schedule,                    "id")
         self._hints["/api/v1/meeting/schedulingevent/"]            = Hints(SchedulingEvent,             "id")
         self._hints["/api/v1/meeting/session/"]                    = Hints(Session,                     "id")
         self._hints["/api/v1/meeting/timeslot/"]                   = Hints(Timeslot,                    "id")
         self._hints["/api/v1/message/announcementfrom/"]           = Hints(AnnouncementFrom,            "id")
-        self._hints["/api/v1/message/message/"]                    = Hints(DTMessage,                     "id")
+        self._hints["/api/v1/message/message/"]                    = Hints(DTMessage,                   "id")
         self._hints["/api/v1/message/sendqueue/"]                  = Hints(SendQueueEntry,              "id")
         self._hints["/api/v1/name/ballotpositionname/"]            = Hints(BallotPositionName,          "slug")
         self._hints["/api/v1/name/docrelationshipname/"]           = Hints(RelationshipType,            "slug")
         self._hints["/api/v1/name/doctagname/"]                    = Hints(DocumentTag,                 "slug")
         self._hints["/api/v1/name/doctypename/"]                   = Hints(DocumentType,                "slug")
+        self._hints["/api/v1/name/extresourcename/"]               = Hints(ExtResourceName,             "slug")
+        self._hints["/api/v1/name/extresourcetypename/"]           = Hints(ExtResourceTypeName,         "slug")
         self._hints["/api/v1/name/groupmilestonestatename/"]       = Hints(GroupMilestoneStateName,     "slug")
         self._hints["/api/v1/name/groupstatename/"]                = Hints(GroupState,                  "slug")
         self._hints["/api/v1/name/grouptypename/"]                 = Hints(GroupTypeName,               "slug")
         self._hints["/api/v1/name/meetingtypename/"]               = Hints(MeetingType,                 "slug")
         self._hints["/api/v1/name/iprdisclosurestatename/"]        = Hints(IPRDisclosureState,          "slug")
         self._hints["/api/v1/name/iprlicensetypename/"]            = Hints(IPRLicenseType,              "slug")
         self._hints["/api/v1/name/reviewassignmentstatename/"]     = Hints(ReviewAssignmentState,       "slug")
@@ -1830,14 +1707,15 @@
         self._hints["/api/v1/name/streamname/"]                    = Hints(Stream,                      "slug")
         self._hints["/api/v1/person/alias/"]                       = Hints(PersonAlias,                 "id")
         self._hints["/api/v1/person/email/"]                       = Hints(Email,                       "address")
         self._hints["/api/v1/person/historicalemail/"]             = Hints(HistoricalEmail,             "address")
         self._hints["/api/v1/person/historicalperson/"]            = Hints(HistoricalPerson,            "id")
         self._hints["/api/v1/person/person/"]                      = Hints(Person,                      "id")
         self._hints["/api/v1/person/personevent/"]                 = Hints(PersonEvent,                 "id")
+        self._hints["/api/v1/person/personextresource/"]           = Hints(PersonExtResource,           "id")
         self._hints["/api/v1/review/historicalreviewassignment/"]  = Hints(HistoricalReviewAssignment,  "id")
         self._hints["/api/v1/review/historicalreviewersettings/"]  = Hints(HistoricalReviewerSettings,  "id")
         self._hints["/api/v1/review/historicalreviewrequest/"]     = Hints(HistoricalReviewRequest,     "id")
         self._hints["/api/v1/review/historicalunavailableperiod/"] = Hints(HistoricalUnavailablePeriod, "id")
         self._hints["/api/v1/review/nextreviewerinteam/"]          = Hints(NextReviewerInTeam,          "id")
         self._hints["/api/v1/review/reviewassignment/"]            = Hints(ReviewAssignment,            "id")
         self._hints["/api/v1/review/reviewersettings/"]            = Hints(ReviewerSettings,            "id")
@@ -1929,15 +1807,15 @@
                     self.get_count += 1
                     r = self.session.get(url = req_url, params = req_params, headers = req_headers, verify = True, stream = False)
                     self.log.debug(f"_datatracker_get_multi  in_cache={r.from_cache} cached={r.created_at} expires={r.expires} {obj_uri}")
                     if r.status_code == 200:
                         self.log.debug(F"_datatracker_get_multi ({r.status_code}) {obj_uri}")
                         meta = r.json()['meta']
                         objs = r.json()['objects']
-                        obj_uri  = URI(meta['next'])
+                        obj_uri  = URI(uri=meta['next'])
                         for obj in objs:
                             # API requests returning lists should never return duplicate
                             # objects, but due to datatracker bugs this sometimes happens.
                             # Check for and log such problems, but pass the duplicates up
                             # to the higher layers for reconcilition.
                             if obj["resource_uri"] in fetched_objs:
                                 self.log.warning(F"_datatracker_get_multi duplicate object {obj['resource_uri']}")
@@ -2003,144 +1881,95 @@
                     self.log.error(F"_datatracker_get_multi_count: error - retry limit exceeded")
                     sys.exit(1)
                 time.sleep(retry_time)
                 retry_time *= 2
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
-    # Private methods to control the cache:
-
-    def _cache_check_versions(self) -> None:
-        if self.db is None:
-            return
-
-        # Check for and remove obsolete v0.1.0 cache format:
-        cache_version_metadata = self.db.cache_info.find_one({"meta_key": "_cache_versions"})
-        if cache_version_metadata is not None:
-            self.log.warning("_cache_check_versions: old cache detected")
-            if cache_version_metadata["cache_version"] == "0.1.0":
-                self.log.warning(f"_cache_check_versions: cache version changed 0.1.0 -> {self.cache_ver}")
-                for collection in self.db.list_collection_names():
-                    if collection.startswith("api_v1"):
-                        self.log.info(f"_cache_check_versions: remove obsolete cache {collection}")
-                        self.db[collection].drop_indexes()
-                        self.db[collection].drop()
-                self.db.cache_info.delete_one({"meta_key": "_cache_versions"})
-
-        # Find cache and datatracker versions:
-        cache_version_metadata = self.db.cache_info.find_one({"collection": "_cache_versions"})
-        if cache_version_metadata is None:
-            dt_version    = None
-            cache_version = self.cache_ver
-        else:
-            dt_version    = cache_version_metadata["dt_version"]
-            cache_version = cache_version_metadata["cache_version"]
-
-        # Check cache version
-        if cache_version == '1' or cache_version == "2" or cache_version == "3":
-            self.log.info(f"_cache_check_versions: cache version changed {cache_version} -> {self.cache_ver}")
-            for collection in self.db.list_collection_names():
-                if collection.startswith("api_v1"):
-                    self.log.info(f"_cache_check_versions: remove obsolete cache {collection}")
-                    self.db[collection].drop_indexes()
-                    self.db[collection].drop()
-            self.db.cache_info.delete_many({"collection": {"$regex": "^api_v1"}})
-        elif self.cache_ver != cache_version:
-            # Exit if the cache version doesn't match that we're expecting. Need to add code above
-            # to update the cache if the format changes, as was done with the v0.1.1 to v1 change.
-            self.log.error(f"_cache_check_versions: cache version changed {cache_version} -> {self.cache_ver}")
-            sys.exit()
-        else:
-            self.log.info(f"_cache_check_versions: cache version {self.cache_ver}")
-
-        # check Datatracker version
-        version_info = self._datatracker_get_single(URI("/api/version/"))
-        if version_info is not None:
-            if dt_version != version_info["version"]:
-                self.log.info(f"_cache_check_versions: datatracker version changed {dt_version} -> {version_info['version']}")
-                self.log.info(f"_cache_check_versions: cache cleared")
-                self.session.cache.clear()
-                dt_version = version_info["version"]
-            else:
-                self.log.info(f"_cache_check_versions: datatracker version {dt_version}")
-        else:
-            self.log.warning("_cache_check_versions: could not check datatracker version")
-
-        self.db.cache_info.replace_one(
-                {"collection": "_cache_versions"},
-                {"collection": "_cache_versions", "dt_version": dt_version, "cache_version": self.cache_ver},
-                upsert=True)
-
-    # ----------------------------------------------------------------------------------------------------------------------------
     # Private methods to retrieve objects from the datatracker:
 
     def _retrieve(self, obj_uri: URI, obj_type: Type[T]) -> Optional[T]:
         self.log.debug(F"_retrieve {obj_uri}")
         obj_json = self._datatracker_get_single(obj_uri)
         if obj_json is not None:
-            return self.pavlova.from_mapping(obj_json, obj_type)
+            #print(obj_json)
+            #print(obj_type)
+            res = None
+            try:
+                res = obj_type(**obj_json)
+            except ValidationError as e:
+                self.log.error(f"Cannot parse response {obj_json}: {e.errors()}")
+            #try:
+            #    res = self.pavlova.from_mapping(obj_json, obj_type)
+            #except PavlovaParsingError:
+            #    self.log.error(f"Cannot parse response {obj_json}")
+            return res
         else:
             return None
 
 
     def _retrieve_multi(self, obj_uri: URI, obj_type: Type[T]) -> Iterator[T]:
         self.log.debug(F"_retrieve_multi: obj_uri {obj_uri}")
-        obj_type_uri = type(obj_uri)(obj_uri.uri)
+        obj_type_uri = type(obj_uri)(uri=obj_uri.uri)
         assert obj_uri.uri      is not None
         assert obj_type_uri.uri is not None
         obj_jsons = [] # type: List[Dict[str, Any]]
         for obj_json in self._datatracker_get_multi(obj_uri):
             obj_jsons.append(obj_json)
         sort_by = self._hints[obj_type_uri.uri].sort_by
         for obj_json in sorted(obj_jsons, key=lambda k: k[sort_by]):
-            fetch_obj = self.pavlova.from_mapping(obj_json, obj_type) # type: T
-            yield fetch_obj
+            #fetch_obj = self.pavlova.from_mapping(obj_json, obj_type) # type: T
+            try:
+                fetch_obj = obj_type(**obj_json)
+                yield fetch_obj
+            except ValidationError as e:
+                self.log.error(f"Cannot parse response {obj_json}: {e.errors()}")
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about people:
     # * https://datatracker.ietf.org/api/v1/person/person/
     # * https://datatracker.ietf.org/api/v1/person/person/20209/
     # * https://datatracker.ietf.org/api/v1/person/historicalperson/
     # * https://datatracker.ietf.org/api/v1/person/alias/
 
     def person(self, person_uri: PersonURI) -> Optional[Person]:
         return self._retrieve(person_uri, Person)
 
 
     def person_from_email(self, email_addr: str) -> Optional[Person]:
-        email = self.email(EmailURI(F"/api/v1/person/email/{email_addr}/"))
+        email = self.email(EmailURI(uri=f"/api/v1/person/email/{email_addr}/"))
         if email is not None and email.person is not None:
             return self.person(email.person)
         else:
             return None
 
 
     def person_aliases(self,
             person        : Optional[Person] = None,
             name          : Optional[str] = None,
             name_contains : Optional[str] = None) -> Iterator[PersonAlias]:
-        url = PersonAliasURI("/api/v1/person/alias/")
+        url = PersonAliasURI(uri="/api/v1/person/alias/")
         if person is not None:
             url.params["person"] = person.id
         if name is not None:
             url.params["name"] = name
         if name_contains is not None:
             url.params["name__contains"] = name_contains
         yield from self._retrieve_multi(url, PersonAlias)
 
 
     def person_history(self, person: Person) -> Iterator[HistoricalPerson]:
-        url = HistoricalPersonURI("/api/v1/person/historicalperson/")
+        url = HistoricalPersonURI(uri="/api/v1/person/historicalperson/")
         url.params["id"] = person.id
         yield from self._retrieve_multi(url, HistoricalPerson)
 
 
     def person_events(self, person: Person) -> Iterator[PersonEvent]:
-        url = PersonEventURI("/api/v1/person/personevent/")
+        url = PersonEventURI(uri="/api/v1/person/personevent/")
         url.params["person"] = person.id
         yield from self._retrieve_multi(url, PersonEvent)
 
 
     def people(self,
             since : str ="1970-01-01T00:00:00",
             until : str ="2038-01-19T03:14:07",
@@ -2158,15 +1987,15 @@
             since         -- Only return people with timestamp after this
             until         -- Only return people with timestamp before this
             name_contains -- Only return peopls whose name containing this string
 
         Returns:
             An iterator, where each element is as returned by the person() method
         """
-        url = PersonURI("/api/v1/person/person/")
+        url = PersonURI(uri="/api/v1/person/person/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if name is not None:
             url.params["name"] = name
         if name_contains is not None:
             url.params["name__contains"] = name_contains
         if name_ascii is not None:
@@ -2176,42 +2005,91 @@
         if name_plain is not None:
             url.params["plain"] = name_plain
         if name_plain_contains is not None:
             url.params["plain__contains"] = name_plain_contains
         yield from self._retrieve_multi(url, Person)
 
 
+    def person_ext_resource(self, person_ext_resource_uri: PersonExtResourceURI) -> Optional[PersonExtResource]:
+        """
+        Retrieve information about an external resource associated with a
+        person.
+
+        External resources include GitHub usernames and personal webpages,
+        amongst other things.
+        """
+        return self._retrieve(person_ext_resource_uri, PersonExtResource)
+
+
+    def person_ext_resources(self,
+                             person        : Optional[Person] = None,
+                             resource_name : Optional[ExtResourceName] = None,
+                             resource_slug : Optional[str] = None) -> Iterator[PersonExtResource]:
+        url = PersonExtResourceURI(uri="/api/v1/person/personextresource/")
+        if person is not None:
+            url.params["person"] = person.id
+        if resource_name is not None:
+            url.params["name"] = resource_name.slug
+        if resource_slug is not None:
+            url.params["name"] = resource_slug
+        yield from self._retrieve_multi(url, PersonExtResource)
+
+
+    def ext_resource_name(self, ext_resource_name_uri: ExtResourceNameURI) -> Optional[ExtResourceName]:
+        return self._retrieve(ext_resource_name_uri, ExtResourceName)
+
+
+    def ext_resource_name_from_slug(self, slug: str) -> Optional[ExtResourceName]:
+        return self._retrieve(ExtResourceNameURI(uri=f"/api/v1/name/extresourcename/{slug}/"), ExtResourceName)
+
+
+    def ext_resource_names(self) -> Iterator[ExtResourceName]:
+        yield from self._retrieve_multi(ExtResourceNameURI(uri="/api/v1/name/extresourcename/"), ExtResourceName)
+
+
+    def ext_resource_type_name(self, ext_resource_type_name_uri: ExtResourceTypeNameURI) -> Optional[ExtResourceTypeName]:
+        return self._retrieve(ext_resource_type_name_uri, ExtResourceTypeName)
+
+
+    def ext_resource_type_name_from_slug(self, slug: str) -> Optional[ExtResourceTypeName]:
+        return self._retrieve(ExtResourceTypeNameURI(uri=f"/api/v1/name/extresourcetypename/{slug}/"), ExtResourceTypeName)
+
+
+    def ext_resource_type_names(self) -> Iterator[ExtResourceTypeName]:
+        yield from self._retrieve_multi(ExtResourceTypeNameURI(uri="/api/v1/name/extresourcetypename/"), ExtResourceTypeName)
+
+
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about email addresses:
     # * https://datatracker.ietf.org/api/v1/person/email/csp@csperkins.org/
     # * https://datatracker.ietf.org/api/v1/person/historicalemail/
 
     def email(self, email_uri: EmailURI) -> Optional[Email]:
         return self._retrieve(email_uri, Email)
 
 
     def email_for_address(self, email_addr: str) -> Optional[Email]:
-        uri = EmailURI(F"/api/v1/person/email/{email_addr}/")
+        uri = EmailURI(uri=f"/api/v1/person/email/{email_addr}/")
         return self.email(uri)
 
 
     def email_for_person(self, person: Person) -> Iterator[Email]:
-        uri = EmailURI("/api/v1/person/email/")
+        uri = EmailURI(uri="/api/v1/person/email/")
         uri.params["person"] = person.id
         yield from self._retrieve_multi(uri, Email)
 
 
     def email_history_for_address(self, email_addr: str) -> Iterator[HistoricalEmail]:
-        uri = HistoricalEmailURI("/api/v1/person/historicalemail/")
+        uri = HistoricalEmailURI(uri="/api/v1/person/historicalemail/")
         uri.params["address"] = email_addr
         yield from self._retrieve_multi(uri, HistoricalEmail)
 
 
     def email_history_for_person(self, person: Person) -> Iterator[HistoricalEmail]:
-        uri = HistoricalEmailURI("/api/v1/person/historicalemail/")
+        uri = HistoricalEmailURI(uri="/api/v1/person/historicalemail/")
         uri.params["person"] = person.id
         yield from self._retrieve_multi(uri, HistoricalEmail)
 
 
     def emails(self,
                since : str ="1970-01-01T00:00:00",
                until : str ="2038-01-19T03:14:07",
@@ -2223,15 +2101,15 @@
             since         -- Only return email addresses with timestamp after this
             until         -- Only return email addresses with timestamp before this
             addr_contains -- Only return email addresses containing this substring
 
         Returns:
             An iterator, where each element is an Email object
         """
-        url = EmailURI("/api/v1/person/email/")
+        url = EmailURI(uri="/api/v1/person/email/")
         url.params["time__gte"] = since
         url.params["time__lt"]   = until
         if addr_contains is not None:
             url.params["address__contains"] = addr_contains
         yield from self._retrieve_multi(url, Email)
 
 
@@ -2250,131 +2128,108 @@
     def documents(self,
             since   : str = "1970-01-01T00:00:00",
             until   : str = "2038-01-19T03:14:07",
             doctype : Optional[DocumentType] = None,
             state   : Optional[DocumentState] = None,
             stream  : Optional[Stream]       = None,
             group   : Optional[Group]        = None) -> Iterator[Document]:
-        url = DocumentURI("/api/v1/doc/document/")
+        url = DocumentURI(uri="/api/v1/doc/document/")
         url.params["time__gte"] = since
         url.params["time__lt"] = until
         if doctype is not None:
             url.params["type"] = doctype.slug
         if state is not None:
             url.params["states"] = state.id
         if stream is not None:
             url.params["stream"] = stream.slug
         if group is not None:
             url.params["group"] = group.id
         yield from self._retrieve_multi(url, Document)
 
 
     # Datatracker API endpoints returning information about document aliases:
-    # * https://datatracker.ietf.org/api/v1/doc/docalias/?name=/                 - draft that became the given RFC
-
-    def document_alias(self, document_alias_uri: DocumentAliasURI) -> Optional[DocumentAlias]:
-        return self._retrieve(document_alias_uri, DocumentAlias)
-
-
-    def document_aliases(self, name: Optional[str] = None) -> Iterator[DocumentAlias]:
-        """
-        Returns a list of DocumentAlias objects that correspond to the specified name.
-
-        Parameters:
-            name -- The name to lookup, for example "rfc3550", "std68", "bcp25", "draft-ietf-quic-transport"
-
-        Returns:
-            A list of DocumentAlias objects
-        """
-        url = DocumentAliasURI("/api/v1/doc/docalias/")
-        if name is not None:
-            url.params["name"] = name
-        yield from self._retrieve_multi(url, DocumentAlias)
-
 
     def document_from_draft(self, draft: str) -> Optional[Document]:
         """
         Returns the document with the specified name.
 
         Parameters:
             name -- The name of the document to lookup (e.g, "draft-ietf-avt-rtp-new")
 
         Returns:
             A Document object
         """
         assert draft.startswith("draft-")
         assert not "," in draft
-        return self.document(DocumentURI("/api/v1/doc/document/" + draft + "/"))
+        return self.document(DocumentURI(uri="/api/v1/doc/document/" + draft + "/"))
 
 
     def document_from_rfc(self, rfc: str) -> Optional[Document]:
         """
         Returns the document that became the specified RFC.
 
         Parameters:
             rfc -- The RFC to lookup (e.g., "rfc3550" or "RFC3550")
 
         Returns:
             A Document object
         """
         assert rfc.lower().startswith("rfc")
-        alias = self.document_alias(DocumentAliasURI(F"/api/v1/doc/docalias/{rfc.lower()}/"))
-        if alias is None:
-            return None
-        else:
-            return self.document(alias.document)
+        return self.document(DocumentURI(uri="/api/v1/doc/document/" + rfc.lower() + "/"))
 
 
     def documents_from_bcp(self, bcp: str) -> Iterator[Document]:
         """
         Returns the document that became the specified BCP.
 
         Parameters:
             bcp -- The BCP to lookup (e.g., "bcp205" or "BCP205")
 
         Returns:
             A list of Document objects
         """
         assert bcp.lower().startswith("bcp")
-        for alias in self.document_aliases(name=bcp.lower()):
-            doc = self.document(alias.document)
-            if doc is not None:
-                yield doc
+        bcp_doc = self.document(DocumentURI(uri="/api/v1/doc/document/" + bcp + "/"))
+        for rel_doc in self.related_documents(source = bcp_doc, relationship_type_slug = "contains"):
+            rfc = self.document(rel_doc.target)
+            assert rfc is not None
+            yield rfc
 
 
     def documents_from_std(self, std: str) -> Iterator[Document]:
         """
         Returns the document that became the specified STD.
 
         Parameters:
             std -- The STD to lookup (e.g., "std68" or "STD68")
 
         Returns:
             A list of Document objects
         """
         assert std.lower().startswith("std")
-        for alias in self.document_aliases(name=std.lower()):
-            doc = self.document(alias.document)
-            if doc is not None:
-                yield doc
+        std_doc = self.document(DocumentURI(uri="/api/v1/doc/document/" + std + "/"))
+        for rel_doc in self.related_documents(source = std_doc, relationship_type_slug = "contains"):
+            rfc = self.document(rel_doc.target)
+            assert rfc is not None
+            yield rfc
 
 
     # Datatracker API endpoints returning information about document types:
     # * https://datatracker.ietf.org/api/v1/name/doctypename/
 
     def document_type(self, doc_type_uri: DocumentTypeURI) -> Optional[DocumentType]:
         return self._retrieve(doc_type_uri, DocumentType)
 
 
     def document_type_from_slug(self, slug: str) -> Optional[DocumentType]:
-        return self._retrieve(DocumentTypeURI(F"/api/v1/name/doctypename/{slug}/"), DocumentType)
+        return self._retrieve(DocumentTypeURI(uri=f"/api/v1/name/doctypename/{slug}/"), DocumentType)
 
 
     def document_types(self) -> Iterator[DocumentType]:
-        yield from self._retrieve_multi(DocumentTypeURI("/api/v1/name/doctypename/"), DocumentType)
+        yield from self._retrieve_multi(DocumentTypeURI(uri="/api/v1/name/doctypename/"), DocumentType)
 
 
     # Datatracker API endpoints returning information about document states:
     # * https://datatracker.ietf.org/api/v1/doc/state/                           - Types of state a document can be in
     # * https://datatracker.ietf.org/api/v1/doc/statetype/                       - Possible types of state for a document
 
     def document_state(self, state_uri: DocumentStateURI) -> Optional[DocumentState]:
@@ -2384,32 +2239,32 @@
         states = list(self.document_states(state_type, slug))
         assert len(states) == 1
         return states[0]
 
     def document_states(self,
             state_type : Optional[DocumentStateType] = None,
             slug       : Optional[str]               = None) -> Iterator[DocumentState]:
-        url = DocumentStateURI("/api/v1/doc/state/")
+        url = DocumentStateURI(uri="/api/v1/doc/state/")
         if state_type is not None:
             url.params["type"] = state_type.slug
         if slug is not None:
             url.params["slug"] = slug
         yield from self._retrieve_multi(url, DocumentState)
 
 
     def document_state_type(self, state_type_uri : DocumentStateTypeURI) -> Optional[DocumentStateType]:
         return self._retrieve(state_type_uri, DocumentStateType)
 
 
     def document_state_type_from_slug(self, slug: str) -> Optional[DocumentStateType]:
-        return self._retrieve(DocumentStateTypeURI(F"/api/v1/doc/statetype/{slug}/"), DocumentStateType)
+        return self._retrieve(DocumentStateTypeURI(uri=f"/api/v1/doc/statetype/{slug}/"), DocumentStateType)
 
 
     def document_state_types(self) -> Iterator[DocumentStateType]:
-        url = DocumentStateTypeURI("/api/v1/doc/statetype/")
+        url = DocumentStateTypeURI(uri="/api/v1/doc/statetype/")
         yield from self._retrieve_multi(url, DocumentStateType)
 
 
     # Datatracker API endpoints returning information about document events:
     # * https://datatracker.ietf.org/api/v1/doc/docevent/                        - list of document events
     # * https://datatracker.ietf.org/api/v1/doc/docevent/?doc=...                - events for a document
     # * https://datatracker.ietf.org/api/v1/doc/docevent/?by=...                 - events by a person (as /api/v1/person/person)
@@ -2444,15 +2299,15 @@
             doc        -- Only return document events for this document
             by         -- Only return document events by this person
             event_type -- Only return document events with this type
 
         Returns:
            A sequence of DocumentEvent objects
         """
-        url = DocumentEventURI("/api/v1/doc/docevent/")
+        url = DocumentEventURI(uri="/api/v1/doc/docevent/")
         url.params["time__gte"] = since
         url.params["time__lt"] = until
         if doc is not None:
             url.params["doc"]  = doc.id
         if by is not None:
             url.params["by"]   = by.id
         if event_type is not None:
@@ -2462,48 +2317,51 @@
 
     # Datatracker API endpoints returning information about document authorship:
     # * https://datatracker.ietf.org/api/v1/doc/documentauthor/?document=...     - authors of a document
     # * https://datatracker.ietf.org/api/v1/doc/documentauthor/?person=...       - documents by person
     # * https://datatracker.ietf.org/api/v1/doc/documentauthor/?email=...        - documents by person
 
     def document_authors(self, document : Document) -> Iterator[DocumentAuthor]:
-        url = DocumentAuthorURI("/api/v1/doc/documentauthor/")
+        url = DocumentAuthorURI(uri="/api/v1/doc/documentauthor/")
         url.params["document"] = document.id
         yield from self._retrieve_multi(url, DocumentAuthor)
 
 
     def documents_authored_by_person(self, person : Person) -> Iterator[DocumentAuthor]:
-        url = DocumentAuthorURI("/api/v1/doc/documentauthor/")
+        url = DocumentAuthorURI(uri="/api/v1/doc/documentauthor/")
         url.params["person"] = person.id
         yield from self._retrieve_multi(url, DocumentAuthor)
 
 
     def documents_authored_by_email(self, email : Email) -> Iterator[DocumentAuthor]:
-        url = DocumentAuthorURI("/api/v1/doc/documentauthor/")
+        url = DocumentAuthorURI(uri="/api/v1/doc/documentauthor/")
         url.params["email"] = email.address
         yield from self._retrieve_multi(url, DocumentAuthor)
 
 
     # Datatracker API endpoints returning information about related documents:
     #   https://datatracker.ietf.org/api/v1/doc/relateddocument/?source=...      - documents that source draft relates to
     #   https://datatracker.ietf.org/api/v1/doc/relateddocument/?target=...      - documents that relate to target draft
     #   https://datatracker.ietf.org/api/v1/doc/relateddochistory/
 
     def related_documents(self,
-        source               : Optional[Document]         = None,
-        target               : Optional[DocumentAlias]    = None,
-        relationship_type    : Optional[RelationshipType] = None) -> Iterator[RelatedDocument]:
+                          source                 : Optional[Document]         = None,
+                          target                 : Optional[Document]         = None,
+                          relationship_type      : Optional[RelationshipType] = None,
+                          relationship_type_slug : Optional[str] = None) -> Iterator[RelatedDocument]:
 
-        url = RelatedDocumentURI("/api/v1/doc/relateddocument/")
+        url = RelatedDocumentURI(uri="/api/v1/doc/relateddocument/")
         if source is not None:
             url.params["source"] = source.id
         if target is not None:
             url.params["target"] = target.id
         if relationship_type is not None:
             url.params["relationship"] = relationship_type.slug
+        if relationship_type_slug is not None:
+            url.params["relationship"] = relationship_type_slug
         yield from self._retrieve_multi(url, RelatedDocument)
 
 
     def relationship_type(self, relationship_type_uri: RelationshipTypeURI) -> Optional[RelationshipType]:
         """
         Retrieve a relationship type
 
@@ -2514,28 +2372,28 @@
         Returns:
             A RelationshipType object
         """
         return self._retrieve(relationship_type_uri, RelationshipType)
 
 
     def relationship_type_from_slug(self, slug: str) -> Optional[RelationshipType]:
-        return self._retrieve(RelationshipTypeURI(F"/api/v1/name/docrelationshipname/{slug}/"), RelationshipType)
+        return self._retrieve(RelationshipTypeURI(uri=f"/api/v1/name/docrelationshipname/{slug}/"), RelationshipType)
 
 
     def relationship_types(self) -> Iterator[RelationshipType]:
         """
         A generator returning the possible relationship types
 
         Parameters:
            None
 
         Returns:
             An iterator of RelationshipType objects
         """
-        url = RelationshipTypeURI("/api/v1/name/docrelationshipname/")
+        url = RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/")
         yield from self._retrieve_multi(url, RelationshipType)
 
 
     # Datatracker API endpoints returning information about document history:
     #   https://datatracker.ietf.org/api/v1/doc/dochistory/
     #   https://datatracker.ietf.org/api/v1/doc/dochistoryauthor/
 
@@ -2550,27 +2408,27 @@
     # * https://datatracker.ietf.org/api/v1/doc/ballotdocevent/
 
     def ballot_position_name(self, ballot_position_name_uri : BallotPositionNameURI) -> Optional[BallotPositionName]:
         return self._retrieve(ballot_position_name_uri, BallotPositionName)
 
 
     def ballot_position_name_from_slug(self, slug: str) -> Optional[BallotPositionName]:
-        return self._retrieve(BallotPositionNameURI(F"/api/v1/name/ballotpositionname/{slug}/"), BallotPositionName)
+        return self._retrieve(BallotPositionNameURI(uri=f"/api/v1/name/ballotpositionname/{slug}/"), BallotPositionName)
 
 
     def ballot_position_names(self) -> Iterator[BallotPositionName]:
         """
         A generator returning information about ballot position names. These describe
         the names of the responses that a person can give to a ballot (e.g., "Discuss",
         "Abstain", "No Objection", ...).
 
         Returns:
            A sequence of BallotPositionName objects
         """
-        url = BallotPositionNameURI("/api/v1/name/ballotpositionname/")
+        url = BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/")
         yield from self._retrieve_multi(url, BallotPositionName)
 
 
     def ballot_type(self, ballot_type_uri : BallotTypeURI) -> Optional[BallotType]:
         return self._retrieve(ballot_type_uri, BallotType)
 
 
@@ -2580,15 +2438,15 @@
 
         Parameters:
             doc_type     -- Only return ballot types relating to this document type
 
         Returns:
            A sequence of BallotType objects
         """
-        url = BallotTypeURI("/api/v1/doc/ballottype/")
+        url = BallotTypeURI(uri="/api/v1/doc/ballottype/")
         if doc_type is not None:
             url.params["doc_type"] = doc_type.slug
         yield from self._retrieve_multi(url, BallotType)
 
 
 
     def ballot_document_event(self, ballot_event_uri : BallotDocumentEventURI) -> Optional[BallotDocumentEvent]:
@@ -2612,15 +2470,15 @@
             event_type   -- Only return ballot document events with this type
             by           -- Only return ballot document events by this person
             doc          -- Only return ballot document events that relate to this document
 
         Returns:
            A sequence of BallotDocumentEvent objects
         """
-        url = BallotDocumentEventURI("/api/v1/doc/ballotdocevent/")
+        url = BallotDocumentEventURI(uri="/api/v1/doc/ballotdocevent/")
         url.params["time__gte"] = since
         url.params["time__lt"] = until
         if ballot_type is not None:
             url.params["ballot_type"] = ballot_type.id
         if by is not None:
             url.params["by"] = by.id
         if doc is not None:
@@ -2640,15 +2498,15 @@
     def submission(self, submission_uri: SubmissionURI) -> Optional[Submission]:
         return self._retrieve(submission_uri, Submission)
 
 
     def submissions(self,
             date_since           : str = "1970-01-01",
             date_until           : str = "2038-01-19") -> Iterator[Submission]:
-        url = SubmissionURI("/api/v1/submit/submission/")
+        url = SubmissionURI(uri="/api/v1/submit/submission/")
         url.params["submission_date__gte"] = date_since
         url.params["submission_date__lt"] = date_until
         yield from self._retrieve_multi(url, Submission)
 
 
     def submission_event(self, event_uri: SubmissionEventURI) -> Optional[SubmissionEvent]:
         return self._retrieve(event_uri, SubmissionEvent)
@@ -2667,50 +2525,61 @@
             until      -- Only return submission events with timestamp after this
             by         -- Only return submission events by this person
             submission -- Only return submission events about this submission
 
         Returns:
            A sequence of SubmissionEvent objects
         """
-        url = SubmissionEventURI("/api/v1/submit/submissionevent/")
+        url = SubmissionEventURI(uri="/api/v1/submit/submissionevent/")
         url.params["time__gte"] = since
         url.params["time__lt"] = until
         if by is not None:
             url.params["by"] = by.id
         if submission is not None:
             url.params["submission"] = submission.id
         yield from self._retrieve_multi(url, SubmissionEvent)
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning miscellaneous information about documents:
     #   https://datatracker.ietf.org/api/v1/doc/docreminder/
-    #   https://datatracker.ietf.org/api/v1/doc/documenturl/
     #   https://datatracker.ietf.org/api/v1/doc/deletedevent/
 
     # FIXME: implement these
 
+    #   https://datatracker.ietf.org/api/v1/doc/documenturl/
+    def document_url(self, document_url_uri: DocumentUrlURI) -> Optional[DocumentUrl]:
+        return self._retrieve(document_url_uri, DocumentUrl)
+    
+    
+    def document_urls(self, doc: Optional[Document] = None) -> Iterator[DocumentUrl]:
+        url = DocumentUrlURI(uri="/api/v1/doc/documenturl/")
+        if doc is not None:
+            url.params["doc"] = doc.id
+        yield from self._retrieve_multi(url, DocumentUrl)
+
+
     #   https://datatracker.ietf.org/api/v1/name/doctagname/
     def document_tag(self, tag_uri: DocumentTagURI) -> Optional[DocumentTag]:
         return self._retrieve(tag_uri, DocumentTag)
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about RFC publication streams:
     # * https://datatracker.ietf.org/api/v1/name/streamname/
 
     def stream(self, stream_uri: StreamURI) -> Optional[Stream]:
         return self._retrieve(stream_uri, Stream)
 
 
     def stream_from_slug(self, slug: str) -> Optional[Stream]:
-        return self._retrieve(StreamURI(F"/api/v1/name/streamname/{slug}/"), Stream)
+        return self._retrieve(StreamURI(uri=f"/api/v1/name/streamname/{slug}/"), Stream)
 
 
     def streams(self) -> Iterator[Stream]:
-        yield from self._retrieve_multi(StreamURI("/api/v1/name/streamname/"), Stream)
+        yield from self._retrieve_multi(StreamURI(uri="/api/v1/name/streamname/"), Stream)
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about working groups:
     # * https://datatracker.ietf.org/api/v1/group/group/                               - list of groups
     # * https://datatracker.ietf.org/api/v1/group/group/2161/                          - info about group 2161
     # * https://datatracker.ietf.org/api/v1/group/grouphistory/?group=2161             - history
@@ -2731,15 +2600,15 @@
     # * https://datatracker.ietf.org/api/v1/name/grouptypename/
 
     def group(self, group_uri: GroupURI) -> Optional[Group]:
         return self._retrieve(group_uri, Group)
 
 
     def group_from_acronym(self, acronym: str) -> Optional[Group]:
-        url = GroupURI("/api/v1/group/group/")
+        url = GroupURI(uri="/api/v1/group/group/")
         url.params["acronym"] = acronym
         groups = list(self._retrieve_multi(url, Group))
         if len(groups) == 0:
             return None
         elif len(groups) == 1:
             return groups[0]
         else:
@@ -2748,15 +2617,15 @@
 
     def groups(self,
             since         : str                  = "1970-01-01T00:00:00",
             until         : str                  = "2038-01-19T03:14:07",
             name_contains : Optional[str]        = None,
             state         : Optional[GroupState] = None,
             parent        : Optional[Group]      = None) -> Iterator[Group]:
-        url = GroupURI("/api/v1/group/group/")
+        url = GroupURI(uri="/api/v1/group/group/")
         url.params["time__gte"]       = since
         url.params["time__lt"]       = until
         if name_contains is not None:
             url.params["name__contains"] = name_contains
         if state is not None:
             url.params["state"] = state.slug
         if parent is not None:
@@ -2765,26 +2634,26 @@
 
 
     def group_history(self, group_history_uri: GroupHistoryURI) -> Optional[GroupHistory]:
         return self._retrieve(group_history_uri, GroupHistory)
 
 
     def group_histories_from_acronym(self, acronym: str) -> Iterator[GroupHistory]:
-        url = GroupHistoryURI("/api/v1/group/grouphistory/")
+        url = GroupHistoryURI(uri="/api/v1/group/grouphistory/")
         url.params["acronym"] = acronym
         yield from self._retrieve_multi(url, GroupHistory)
 
 
     def group_histories(self,
             since         : str                  = "1970-01-01T00:00:00",
             until         : str                  = "2038-01-19T03:14:07",
             group         : Optional[Group]      = None,
             state         : Optional[GroupState] = None,
             parent        : Optional[Group]      = None) -> Iterator[GroupHistory]:
-        url = GroupHistoryURI("/api/v1/group/grouphistory/")
+        url = GroupHistoryURI(uri="/api/v1/group/grouphistory/")
         url.params["time__gte"]  = since
         url.params["time__lt"]  = until
         if group is not None:
             url.params["group"] = group.id
         if state is not None:
             url.params["state"] = state.slug
         if parent is not None:
@@ -2798,85 +2667,86 @@
 
     def group_events(self,
             since         : str                  = "1970-01-01T00:00:00",
             until         : str                  = "2038-01-19T03:14:07",
             by            : Optional[Person]     = None,
             group         : Optional[Group]      = None,
             type          : Optional[str]        = None) -> Iterator[GroupEvent]:
-        url = GroupEventURI("/api/v1/group/groupevent/")
+        url = GroupEventURI(uri="/api/v1/group/groupevent/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if by is not None:
             url.params["by"] = by.id
         if group is not None:
             url.params["group"] = group.id
         if type is not None:
             url.params["type"]  = type
         yield from self._retrieve_multi(url, GroupEvent)
 
+
     def group_url(self, group_url_uri: GroupUrlURI) -> Optional[GroupUrl]:
         return self._retrieve(group_url_uri, GroupUrl)
 
 
     def group_urls(self, group: Optional[Group] = None) -> Iterator[GroupUrl]:
-        url = GroupUrlURI("/api/v1/group/groupurl/")
+        url = GroupUrlURI(uri="/api/v1/group/groupurl/")
         if group is not None:
             url.params["group"] = group.id
         yield from self._retrieve_multi(url, GroupUrl)
 
 
     def group_milestone_statename(self, group_milestone_statename_uri: GroupMilestoneStateNameURI) -> Optional[GroupMilestoneStateName]:
         return self._retrieve(group_milestone_statename_uri, GroupMilestoneStateName)
 
 
     def group_milestone_statenames(self) -> Iterator[GroupMilestoneStateName]:
-        yield from self._retrieve_multi(GroupMilestoneStateNameURI("/api/v1/name/groupmilestonestatename/"), GroupMilestoneStateName)
+        yield from self._retrieve_multi(GroupMilestoneStateNameURI(uri="/api/v1/name/groupmilestonestatename/"), GroupMilestoneStateName)
 
 
     def group_milestone(self, group_milestone_uri : GroupMilestoneURI) -> Optional[GroupMilestone]:
         return self._retrieve(group_milestone_uri, GroupMilestone)
 
 
     def group_milestones(self,
             since         : str                               = "1970-01-01T00:00:00",
             until         : str                               = "2038-01-19T03:14:07",
             group         : Optional[Group]                   = None,
             state         : Optional[GroupMilestoneStateName] = None) -> Iterator[GroupMilestone]:
-        url = GroupMilestoneURI("/api/v1/group/groupmilestone/")
+        url = GroupMilestoneURI(uri="/api/v1/group/groupmilestone/")
         url.params["time__gte"]       = since
         url.params["time__lt"]       = until
         if group is not None:
             url.params["group"] = group.id
         if state is not None:
             url.params["state"] = state.slug
         yield from self._retrieve_multi(url, GroupMilestone)
 
 
     def role_name(self, role_name_uri: RoleNameURI) -> Optional[RoleName]:
         return self._retrieve(role_name_uri, RoleName)
 
 
     def role_name_from_slug(self, slug: str) -> Optional[RoleName]:
-        return self._retrieve(RoleNameURI(F"/api/v1/name/rolename/{slug}/"), RoleName)
+        return self._retrieve(RoleNameURI(uri=f"/api/v1/name/rolename/{slug}/"), RoleName)
 
 
     def role_names(self) -> Iterator[RoleName]:
-        yield from self._retrieve_multi(RoleNameURI("/api/v1/name/rolename/"), RoleName)
+        yield from self._retrieve_multi(RoleNameURI(uri="/api/v1/name/rolename/"), RoleName)
 
 
     def group_role(self, group_role_uri : GroupRoleURI) -> Optional[GroupRole]:
         return self._retrieve(group_role_uri, GroupRole)
 
 
     def group_roles(self,
             email         : Optional[str]           = None,
             group         : Optional[Group]         = None,
             name          : Optional[RoleName]      = None,
             person        : Optional[Person]        = None) -> Iterator[GroupRole]:
-        url = GroupRoleURI("/api/v1/group/role/")
+        url = GroupRoleURI(uri="/api/v1/group/role/")
         if email is not None:
             url.params["email"] = email
         if group is not None:
             url.params["group"] = group.id
         if name is not None:
             url.params["name"] = name.slug
         if person is not None:
@@ -2889,15 +2759,15 @@
 
 
     def group_role_histories(self,
             email         : Optional[str]           = None,
             group         : Optional[GroupHistory]  = None,
             name          : Optional[RoleName]      = None,
             person        : Optional[Person]        = None) -> Iterator[GroupRoleHistory]:
-        url = GroupRoleHistoryURI("/api/v1/group/rolehistory/")
+        url = GroupRoleHistoryURI(uri="/api/v1/group/rolehistory/")
         if email is not None:
             url.params["email"] = email
         if group is not None:
             url.params["group"] = group.id
         if name is not None:
             url.params["name"] = name.slug
         if person is not None:
@@ -2911,15 +2781,15 @@
 
     def group_milestone_histories(self,
             since         : str                               = "1970-01-01T00:00:00",
             until         : str                               = "2038-01-19T03:14:07",
             group         : Optional[Group]                   = None,
             milestone     : Optional[GroupMilestone]          = None,
             state         : Optional[GroupMilestoneStateName] = None) -> Iterator[GroupMilestoneHistory]:
-        url = GroupMilestoneHistoryURI("/api/v1/group/groupmilestonehistory/")
+        url = GroupMilestoneHistoryURI(uri="/api/v1/group/groupmilestonehistory/")
         url.params["time__gte"]       = since
         url.params["time__lt"]       = until
         if group is not None:
             url.params["group"] = group.id
         if milestone is not None:
             url.params["milestone"] = milestone.id
         if state is not None:
@@ -2934,15 +2804,15 @@
     def group_milestone_events(self,
             since         : str                        = "1970-01-01T00:00:00",
             until         : str                        = "2038-01-19T03:14:07",
             by            : Optional[Person]           = None,
             group         : Optional[Group]            = None,
             milestone     : Optional[GroupMilestone]   = None,
             type          : Optional[str]              = None) -> Iterator[GroupMilestoneEvent]:
-        url = GroupMilestoneEventURI("/api/v1/group/milestonegroupevent/")
+        url = GroupMilestoneEventURI(uri="/api/v1/group/milestonegroupevent/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if by is not None:
             url.params["by"] = by.id
         if group is not None:
             url.params["group"] = group.id
         if milestone is not None:
@@ -2958,15 +2828,15 @@
 
     def group_state_change_events(self,
             since         : str                        = "1970-01-01T00:00:00",
             until         : str                        = "2038-01-19T03:14:07",
             by            : Optional[Person]           = None,
             group         : Optional[Group]            = None,
             state         : Optional[GroupState]       = None) -> Iterator[GroupStateChangeEvent]:
-        url = GroupStateChangeEventURI("/api/v1/group/changestategroupevent/")
+        url = GroupStateChangeEventURI(uri="/api/v1/group/changestategroupevent/")
         url.params["time__gte"]       = since
         url.params["time__lt"]       = until
         if by is not None:
             url.params["by"] = by.id
         if group is not None:
             url.params["group"] = group.id
         if state is not None:
@@ -2975,32 +2845,32 @@
 
 
     def group_state(self, group_state_uri : GroupStateURI) -> Optional[GroupState]:
         return self._retrieve(group_state_uri, GroupState)
 
 
     def group_state_from_slug(self, slug : str) -> Optional[GroupState]:
-        return self._retrieve(GroupStateURI(F"/api/v1/name/groupstatename/{slug}/"), GroupState)
+        return self._retrieve(GroupStateURI(uri=f"/api/v1/name/groupstatename/{slug}/"), GroupState)
 
 
     def group_states(self) -> Iterator[GroupState]:
-        url = GroupStateURI("/api/v1/name/groupstatename/")
+        url = GroupStateURI(uri="/api/v1/name/groupstatename/")
         yield from self._retrieve_multi(url, GroupState)
 
 
     def group_type_name(self, group_type_name_uri : GroupTypeNameURI) -> Optional[GroupTypeName]:
         return self._retrieve(group_type_name_uri, GroupTypeName)
 
 
     def group_type_name_from_slug(self, slug : str) -> Optional[GroupTypeName]:
-        return self._retrieve(GroupTypeNameURI(F"/api/v1/name/grouptypename/{slug}/"), GroupTypeName)
+        return self._retrieve(GroupTypeNameURI(uri=f"/api/v1/name/grouptypename/{slug}/"), GroupTypeName)
 
 
     def group_type_names(self) -> Iterator[GroupTypeName]:
-        yield from self._retrieve_multi(GroupTypeNameURI("/api/v1/name/grouptypename/"), GroupTypeName)
+        yield from self._retrieve_multi(GroupTypeNameURI(uri="/api/v1/name/grouptypename/"), GroupTypeName)
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about meetings:
     # * https://datatracker.ietf.org/api/v1/meeting/meeting/                        - list of meetings
     # * https://datatracker.ietf.org/api/v1/meeting/meeting/747/                    - information about meeting number 747
     # * https://datatracker.ietf.org/api/v1/meeting/schedule/791/                   - a version of the meeting agenda
@@ -3029,15 +2899,15 @@
         return self._retrieve(assignment_uri, SessionAssignment)
 
 
     def meeting_session_assignments(self, schedule : Schedule) -> Iterator[SessionAssignment]:
         """
         The assignment of sessions to timeslots in a meeting schedule.
         """
-        url = SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/")
+        url = SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/")
         url.params["schedule"] = schedule.id
         yield from self._retrieve_multi(url, SessionAssignment)
 
 
     def meeting_session_status(self, session: Session) -> Optional[SessionStatusName]:
         sched_events = list(self.meeting_scheduling_events(session=session))
         if len(sched_events) > 0:
@@ -3047,37 +2917,37 @@
 
 
     def meeting_session_status_name(self, ssn_uri: SessionStatusNameURI) -> Optional[SessionStatusName]:
         return self._retrieve(ssn_uri, SessionStatusName)
 
 
     def meeting_session_status_name_from_slug(self, slug: str) -> Optional[SessionStatusName]:
-        return self._retrieve(SessionStatusNameURI(F"/api/v1/name/sessionstatusname/{slug}/"), SessionStatusName)
+        return self._retrieve(SessionStatusNameURI(uri=f"/api/v1/name/sessionstatusname/{slug}/"), SessionStatusName)
 
 
     def meeting_session_status_names(self) -> Iterator[SessionStatusName]:
-        yield from self._retrieve_multi(SessionStatusNameURI("/api/v1/name/sessionstatusname/"), SessionStatusName)
+        yield from self._retrieve_multi(SessionStatusNameURI(uri="/api/v1/name/sessionstatusname/"), SessionStatusName)
 
 
     def meeting_session_purpose(self, purpose_uri: SessionPurposeURI) -> Optional[SessionPurpose]:
         return self._retrieve(purpose_uri, SessionPurpose)
 
 
     def meeting_session_purposes(self) -> Iterator[SessionPurpose]:
-        yield from self._retrieve_multi(SessionPurposeURI("/api/v1/name/sessionpurposename/"), SessionPurpose)
+        yield from self._retrieve_multi(SessionPurposeURI(uri="/api/v1/name/sessionpurposename/"), SessionPurpose)
 
 
     def meeting_session(self, session_uri : SessionURI) -> Optional[Session]:
         return self._retrieve(session_uri, Session)
 
 
     def meeting_sessions(self,
             meeting : Meeting,
             group   : Optional[Group] = None) -> Iterator[Session]:
-        url = SessionURI("/api/v1/meeting/session/")
+        url = SessionURI(uri="/api/v1/meeting/session/")
         url.params["meeting"]  = meeting.id
         if group is not None:
             url.params["group"] = group.id
         yield from self._retrieve_multi(url, Session)
 
 
     def meeting_timeslot(self, timeslot_uri: TimeslotURI) -> Optional[Timeslot]:
@@ -3087,15 +2957,15 @@
     def meeting_scheduling_event(self, scheduling_event_uri: SchedulingEventURI) -> Optional[SchedulingEvent]:
         return self._retrieve(scheduling_event_uri, SchedulingEvent)
 
 
     def meeting_scheduling_events(self,
             by      : Optional[Person]  = None,
             session : Optional[Session] = None) -> Iterator[SchedulingEvent]:
-        url = SchedulingEventURI("/api/v1/meeting/schedulingevent/")
+        url = SchedulingEventURI(uri="/api/v1/meeting/schedulingevent/")
         if session is not None:
             url.params["session"] = session.id
         if by is not None:
             url.params["by"] = by.id
         yield from self._retrieve_multi(url, SchedulingEvent)
 
 
@@ -3124,42 +2994,42 @@
     def meetings(self,
             start_date   : str = "1970-01-01",
             end_date     : str = "2038-01-19",
             meeting_type : Optional[MeetingType] = None) -> Iterator[Meeting]:
         """
         Return information about meetings taking place within a particular date range.
         """
-        url = MeetingURI("/api/v1/meeting/meeting/")
+        url = MeetingURI(uri="/api/v1/meeting/meeting/")
         url.params["date__gte"] = start_date
         url.params["date__lte"] = end_date
         if meeting_type is not None:
             url.params["type"] = meeting_type.slug
         yield from self._retrieve_multi(url, Meeting)
 
 
 
     def meeting_type(self, meeting_type_uri: MeetingTypeURI) -> Optional[MeetingType]:
         return self._retrieve(meeting_type_uri, MeetingType)
 
 
     def meeting_type_from_slug(self, slug: str) -> Optional[MeetingType]:
-        return self._retrieve(MeetingTypeURI(F"/api/v1/name/meetingtypename/{slug}/"), MeetingType)
+        return self._retrieve(MeetingTypeURI(uri=f"/api/v1/name/meetingtypename/{slug}/"), MeetingType)
 
 
     def meeting_types(self) -> Iterator[MeetingType]:
         """
         A generator returning the possible meeting types
 
         Parameters:
            None
 
         Returns:
             An iterator of MeetingType objects
         """
-        yield from self._retrieve_multi(MeetingTypeURI("/api/v1/name/meetingtypename/"), MeetingType)
+        yield from self._retrieve_multi(MeetingTypeURI(uri="/api/v1/name/meetingtypename/"), MeetingType)
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about IPR disclosures:
     #
     #   https://datatracker.ietf.org/api/v1/ipr/iprdocrel/
     # * https://datatracker.ietf.org/api/v1/ipr/iprdisclosurebase/
@@ -3179,30 +3049,30 @@
     # * https://datatracker.ietf.org/api/v1/name/iprlicensetypename/
 
     def ipr_disclosure_state(self, ipr_disclosure_state_uri: IPRDisclosureStateURI) -> Optional[IPRDisclosureState]:
         return self._retrieve(ipr_disclosure_state_uri, IPRDisclosureState)
 
 
     def ipr_disclosure_states(self) -> Iterator[IPRDisclosureState]:
-        yield from self._retrieve_multi(IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/"), IPRDisclosureState)
+        yield from self._retrieve_multi(IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/"), IPRDisclosureState)
 
 
     def ipr_disclosure_base(self, ipr_disclosure_base_uri: IPRDisclosureBaseURI) -> Optional[IPRDisclosureBase]:
         return self._retrieve(ipr_disclosure_base_uri, IPRDisclosureBase)
 
 
     def ipr_disclosure_bases(self,
             since              : str                             = "1970-01-01T00:00:00",
             until              : str                             = "2038-01-19T03:14:07",
             by                 : Optional[Person]                = None,
             holder_legal_name  : Optional[str]                   = None,
             state              : Optional[IPRDisclosureState]    = None,
             submitter_email    : Optional[str]                   = None,
             submitter_name     : Optional[str]                   = None) -> Iterator[IPRDisclosureBase]:
-        url = IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/")
+        url = IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if by is not None:
             url.params["by"] = by.id
         if holder_legal_name is not None:
             url.params["holder_legal_name"] = holder_legal_name
         if state is not None:
@@ -3223,15 +3093,15 @@
             until               : str                             = "2038-01-19T03:14:07",
             by                  : Optional[Person]                = None,
             holder_legal_name   : Optional[str]                   = None,
             holder_contact_name : Optional[str]                   = None,
             state               : Optional[IPRDisclosureState]    = None,
             submitter_email     : Optional[str]                   = None,
             submitter_name      : Optional[str]                   = None) -> Iterator[GenericIPRDisclosure]:
-        url = GenericIPRDisclosureURI("/api/v1/ipr/genericiprdisclosure/")
+        url = GenericIPRDisclosureURI(uri="/api/v1/ipr/genericiprdisclosure/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if by is not None:
             url.params["by"] = by.id
         if holder_legal_name is not None:
             url.params["holder_legal_name"] = holder_legal_name
         if holder_contact_name is not None:
@@ -3246,15 +3116,15 @@
 
 
     def ipr_license_type(self, ipr_license_type_uri: IPRLicenseTypeURI) -> Optional[IPRLicenseType]:
         return self._retrieve(ipr_license_type_uri, IPRLicenseType)
 
 
     def ipr_license_types(self) -> Iterator[IPRLicenseType]:
-        yield from self._retrieve_multi(IPRLicenseTypeURI("/api/v1/name/iprlicensetypename/"), IPRLicenseType)
+        yield from self._retrieve_multi(IPRLicenseTypeURI(uri="/api/v1/name/iprlicensetypename/"), IPRLicenseType)
 
 
     def holder_ipr_disclosure(self, holder_ipr_disclosure_uri: HolderIPRDisclosureURI) -> Optional[HolderIPRDisclosure]:
         return self._retrieve(holder_ipr_disclosure_uri, HolderIPRDisclosure)
 
 
     def holder_ipr_disclosures(self,
@@ -3265,15 +3135,15 @@
             holder_contact_name  : Optional[str]                   = None,
             ietfer_contact_email : Optional[str]                   = None,
             ietfer_name          : Optional[str]                   = None,
             licensing            : Optional[IPRLicenseType]        = None,
             state                : Optional[IPRDisclosureState]    = None,
             submitter_email      : Optional[str]                   = None,
             submitter_name       : Optional[str]                   = None) -> Iterator[HolderIPRDisclosure]:
-        url = HolderIPRDisclosureURI("/api/v1/ipr/holderiprdisclosure/")
+        url = HolderIPRDisclosureURI(uri="/api/v1/ipr/holderiprdisclosure/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if by is not None:
             url.params["by"] = by.id
         if holder_legal_name is not None:
             url.params["holder_legal_name"] = holder_legal_name
         if holder_contact_name is not None:
@@ -3303,15 +3173,15 @@
             by                   : Optional[Person]                = None,
             holder_legal_name    : Optional[str]                   = None,
             ietfer_contact_email : Optional[str]                   = None,
             ietfer_name          : Optional[str]                   = None,
             state                : Optional[IPRDisclosureState]    = None,
             submitter_email      : Optional[str]                   = None,
             submitter_name       : Optional[str]                   = None) -> Iterator[HolderIPRDisclosure]:
-        url = ThirdPartyIPRDisclosureURI("/api/v1/ipr/thirdpartyiprdisclosure/")
+        url = ThirdPartyIPRDisclosureURI(uri="/api/v1/ipr/thirdpartyiprdisclosure/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if by is not None:
             url.params["by"] = by.id
         if holder_legal_name is not None:
             url.params["holder_legal_name"] = holder_legal_name
         if ietfer_contact_email is not None:
@@ -3366,70 +3236,70 @@
     # * https://datatracker.ietf.org/api/v1/name/reviewtypename/
 
     def review_assignment_state(self, review_assignment_state_uri: ReviewAssignmentStateURI) -> Optional[ReviewAssignmentState]:
         return self._retrieve(review_assignment_state_uri, ReviewAssignmentState)
 
 
     def review_assignment_state_from_slug(self, slug: str) -> Optional[ReviewAssignmentState]:
-        return self._retrieve(ReviewAssignmentStateURI(F"/api/v1/name/reviewassignmentstatename/{slug}/"), ReviewAssignmentState)
+        return self._retrieve(ReviewAssignmentStateURI(uri=f"/api/v1/name/reviewassignmentstatename/{slug}/"), ReviewAssignmentState)
 
 
     def review_assignment_states(self) -> Iterator[ReviewAssignmentState]:
-        yield from self._retrieve_multi(ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/"), ReviewAssignmentState)
+        yield from self._retrieve_multi(ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/"), ReviewAssignmentState)
 
 
     def review_result_type(self, review_result_uri: ReviewResultTypeURI) -> Optional[ReviewResultType]:
         return self._retrieve(review_result_uri, ReviewResultType)
 
 
     def review_result_type_from_slug(self, slug: str) -> Optional[ReviewResultType]:
-        return self._retrieve(ReviewResultTypeURI(F"/api/v1/name/reviewresultname/{slug}/"), ReviewResultType)
+        return self._retrieve(ReviewResultTypeURI(uri=f"/api/v1/name/reviewresultname/{slug}/"), ReviewResultType)
 
 
     def review_result_types(self) -> Iterator[ReviewResultType]:
-        yield from self._retrieve_multi(ReviewResultTypeURI("/api/v1/name/reviewresultname/"), ReviewResultType)
+        yield from self._retrieve_multi(ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/"), ReviewResultType)
 
 
     def review_type(self, review_type_uri: ReviewTypeURI) -> Optional[ReviewType]:
         return self._retrieve(review_type_uri, ReviewType)
 
 
     def review_type_from_slug(self, slug: str) -> Optional[ReviewType]:
-        return self._retrieve(ReviewTypeURI(F"/api/v1/name/reviewtypename/{slug}/"), ReviewType)
+        return self._retrieve(ReviewTypeURI(uri=f"/api/v1/name/reviewtypename/{slug}/"), ReviewType)
 
 
     def review_types(self) -> Iterator[ReviewType]:
-        yield from self._retrieve_multi(ReviewTypeURI("/api/v1/name/reviewtypename/"), ReviewType)
+        yield from self._retrieve_multi(ReviewTypeURI(uri="/api/v1/name/reviewtypename/"), ReviewType)
 
 
     def review_request_state(self, review_request_state_uri: ReviewRequestStateURI) -> Optional[ReviewRequestState]:
         return self._retrieve(review_request_state_uri, ReviewRequestState)
 
 
     def review_request_state_from_slug(self, slug: str) -> Optional[ReviewRequestState]:
-        return self._retrieve(ReviewRequestStateURI(F"/api/v1/name/reviewrequeststatename/{slug}/"), ReviewRequestState)
+        return self._retrieve(ReviewRequestStateURI(uri=f"/api/v1/name/reviewrequeststatename/{slug}/"), ReviewRequestState)
 
 
     def review_request_states(self) -> Iterator[ReviewRequestState]:
-        yield from self._retrieve_multi(ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/"), ReviewRequestState)
+        yield from self._retrieve_multi(ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/"), ReviewRequestState)
 
 
     def review_request(self, review_request_uri: ReviewRequestURI) -> Optional[ReviewRequest]:
         return self._retrieve(review_request_uri, ReviewRequest)
 
 
     def review_requests(self,
             since         : str                          = "1970-01-01T00:00:00",
             until         : str                          = "2038-01-19T03:14:07",
             doc           : Optional[Document]           = None,
             requested_by  : Optional[Person]             = None,
             state         : Optional[ReviewRequestState] = None,
             team          : Optional[Group]              = None,
             type          : Optional[ReviewType]         = None) -> Iterator[ReviewRequest]:
-        url = ReviewRequestURI("/api/v1/review/reviewrequest/")
+        url = ReviewRequestURI(uri="/api/v1/review/reviewrequest/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if doc is not None:
             url.params["doc"] = doc.id
         if requested_by is not None:
             url.params["requested_by"] = requested_by.id
         if state is not None:
@@ -3450,15 +3320,15 @@
             assigned_until         : str                             = "2038-01-19T03:14:07",
             completed_since        : str                             = "1970-01-01T00:00:00",
             completed_until        : str                             = "2038-01-19T03:14:07",
             result                 : Optional[ReviewResultType]      = None,
             review_request         : Optional[ReviewRequest]         = None,
             reviewer               : Optional[Email]                 = None,
             state                  : Optional[ReviewAssignmentState] = None) -> Iterator[ReviewAssignment]:
-        url = ReviewAssignmentURI("/api/v1/review/reviewassignment/")
+        url = ReviewAssignmentURI(uri="/api/v1/review/reviewassignment/")
         url.params["assigned_on__gt"]       = assigned_since
         url.params["assigned_on__lt"]       = assigned_until
         url.params["completed_on__gt"]      = completed_since
         url.params["completed_on__lt"]      = completed_until
         if result is not None:
             url.params["result"] = result.slug
         if review_request is not None:
@@ -3476,15 +3346,15 @@
 
     def review_wishes(self,
             since         : str                          = "1970-01-01T00:00:00",
             until         : str                          = "2038-01-19T03:14:07",
             doc           : Optional[Document]           = None,
             person        : Optional[Person]             = None,
             team          : Optional[Group]              = None) -> Iterator[ReviewWish]:
-        url = ReviewWishURI("/api/v1/review/reviewwish/")
+        url = ReviewWishURI(uri="/api/v1/review/reviewwish/")
         url.params["time__gte"]       = since
         url.params["time__lt"]       = until
         if doc is not None:
             url.params["doc"] = doc.id
         if person is not None:
             url.params["person"] = person.id
         if team is not None:
@@ -3497,15 +3367,15 @@
 
 
     def historical_unavailable_periods(self,
             history_type  : Optional[str]                = None,
             id            : Optional[int]                = None,
             person        : Optional[Person]             = None,
             team          : Optional[Group]              = None) -> Iterator[HistoricalUnavailablePeriod]:
-        url = HistoricalUnavailablePeriodURI("/api/v1/review/historicalunavailableperiod/")
+        url = HistoricalUnavailablePeriodURI(uri="/api/v1/review/historicalunavailableperiod/")
         if history_type is not None:
             url.params["history_type"] = history_type
         if id is not None:
             url.params["id"] = id
         if person is not None:
             url.params["person"] = person.id
         if team is not None:
@@ -3525,15 +3395,15 @@
             history_type  : Optional[str]                = None,
             id            : Optional[int]                = None,
             doc           : Optional[Document]           = None,
             requested_by  : Optional[Person]             = None,
             state         : Optional[ReviewRequestState] = None,
             team          : Optional[Group]              = None,
             type          : Optional[ReviewType]         = None) -> Iterator[HistoricalReviewRequest]:
-        url = HistoricalReviewRequestURI("/api/v1/review/historicalreviewrequest/")
+        url = HistoricalReviewRequestURI(uri="/api/v1/review/historicalreviewrequest/")
         url.params["time__gte"]         = since
         url.params["time__lt"]         = until
         url.params["history_date__gt"] = history_since
         url.params["history_date__lt"] = history_until
         if doc is not None:
             url.params["doc"] = doc.id
         if requested_by is not None:
@@ -3549,55 +3419,55 @@
 
     def next_reviewer_in_team(self, next_reviewer_in_team_uri: NextReviewerInTeamURI) -> Optional[NextReviewerInTeam]:
         return self._retrieve(next_reviewer_in_team_uri, NextReviewerInTeam)
 
 
     def next_reviewers_in_teams(self,
             team          : Optional[Group] = None) -> Iterator[NextReviewerInTeam]:
-        url = NextReviewerInTeamURI("/api/v1/review/nextreviewerinteam/")
+        url = NextReviewerInTeamURI(uri="/api/v1/review/nextreviewerinteam/")
         if team is not None:
             url.params["team"] = team.id
         yield from self._retrieve_multi(url, NextReviewerInTeam)
 
 
     def review_team_settings(self, review_team_settings_uri: ReviewTeamSettingsURI) -> Optional[ReviewTeamSettings]:
         return self._retrieve(review_team_settings_uri, ReviewTeamSettings)
 
 
     def review_team_settings_all(self,
             group                    : Optional[Group] = None) -> Iterator[ReviewTeamSettings]:
-        url = ReviewTeamSettingsURI("/api/v1/review/reviewteamsettings/")
+        url = ReviewTeamSettingsURI(uri="/api/v1/review/reviewteamsettings/")
         if group is not None:
             url.params["group"] = group.id
         yield from self._retrieve_multi(url, ReviewTeamSettings)
 
 
     def reviewer_settings(self, reviewer_settings_uri: ReviewerSettingsURI) -> Optional[ReviewerSettings]:
         return self._retrieve(reviewer_settings_uri, ReviewerSettings)
 
 
     def reviewer_settings_all(self,
             person        : Optional[Person]             = None,
             team          : Optional[Group]              = None) -> Iterator[ReviewerSettings]:
-        url = ReviewerSettingsURI("/api/v1/review/reviewersettings/")
+        url = ReviewerSettingsURI(uri="/api/v1/review/reviewersettings/")
         if person is not None:
             url.params["person"] = person.id
         if team is not None:
             url.params["team"] = team.id
         yield from self._retrieve_multi(url, ReviewerSettings)
 
 
     def unavailable_period(self, unavailable_period_uri: UnavailablePeriodURI) -> Optional[UnavailablePeriod]:
         return self._retrieve(unavailable_period_uri, UnavailablePeriod)
 
 
     def unavailable_periods(self,
             person        : Optional[Person]             = None,
             team          : Optional[Group]              = None) -> Iterator[UnavailablePeriod]:
-        url = UnavailablePeriodURI("/api/v1/review/unavailableperiod/")
+        url = UnavailablePeriodURI(uri="/api/v1/review/unavailableperiod/")
         if person is not None:
             url.params["person"] = person.id
         if team is not None:
             url.params["team"] = team.id
         yield from self._retrieve_multi(url, UnavailablePeriod)
 
 
@@ -3607,15 +3477,15 @@
 
     def historical_reviewer_settings_all(self,
             history_since : str                          = "1970-01-01T00:00:00",
             history_until : str                          = "2038-01-19T03:14:07",
             id            : Optional[int]                = None,
             person        : Optional[Person]             = None,
             team          : Optional[Group]              = None) -> Iterator[HistoricalReviewerSettings]:
-        url = HistoricalReviewerSettingsURI("/api/v1/review/historicalreviewersettings/")
+        url = HistoricalReviewerSettingsURI(uri="/api/v1/review/historicalreviewersettings/")
         url.params["history_date__gt"]       = history_since
         url.params["history_date__lt"]       = history_until
         if id is not None:
             url.params["id"] = id
         if person is not None:
             url.params["person"] = person.id
         if team is not None:
@@ -3633,15 +3503,15 @@
             completed_since        : str                             = "1970-01-01T00:00:00",
             completed_until        : str                             = "2038-01-19T03:14:07",
             id                     : Optional[int]                   = None,
             result                 : Optional[ReviewResultType]      = None,
             review_request         : Optional[ReviewRequest]         = None,
             reviewer               : Optional[Email]                 = None,
             state                  : Optional[ReviewAssignmentState] = None) -> Iterator[HistoricalReviewAssignment]:
-        url = HistoricalReviewAssignmentURI("/api/v1/review/historicalreviewassignment/")
+        url = HistoricalReviewAssignmentURI(uri="/api/v1/review/historicalreviewassignment/")
         url.params["assigned_on__gt"]       = assigned_since
         url.params["assigned_on__lt"]       = assigned_until
         url.params["completed_on__gt"]      = completed_since
         url.params["completed_on__lt"]      = completed_until
         if id is not None:
             url.params["id"] = id
         if result is not None:
@@ -3658,48 +3528,50 @@
     def review_secretary_settings(self, review_secretary_settings_uri: ReviewSecretarySettingsURI) -> Optional[ReviewSecretarySettings]:
         return self._retrieve(review_secretary_settings_uri, ReviewSecretarySettings)
 
 
     def review_secretary_settings_all(self,
             person        : Optional[Person]             = None,
             team          : Optional[Group]              = None) -> Iterator[ReviewSecretarySettings]:
-        url = ReviewSecretarySettingsURI("/api/v1/review/reviewsecretarysettings/")
+        url = ReviewSecretarySettingsURI(uri="/api/v1/review/reviewsecretarysettings/")
         if person is not None:
             url.params["person"] = person.id
         if team is not None:
             url.params["team"] = team.id
         yield from self._retrieve_multi(url, ReviewSecretarySettings)
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about mailing lists:
     #
     #   https://datatracker.ietf.org/api/v1/mailinglists/list/
     #   https://datatracker.ietf.org/api/v1/mailinglists/subscribed/
 
-    def email_list(self, email_list_uri: EmailListURI) -> Optional[EmailList]:
-        return self._retrieve(email_list_uri, EmailList)
+    # These appear to have been removed in datatracker 12.5.0
 
-
-    def email_lists(self, name : Optional[str] = None) -> Iterator[EmailList]:
-        url = EmailListURI("/api/v1/mailinglists/list/")
-        if name is not None:
-            url.params["name"] = name
-        yield from self._retrieve_multi(url, EmailList)
+    # def email_list(self, email_list_uri: EmailListURI) -> Optional[EmailList]:
+    #     return self._retrieve(email_list_uri, EmailList)
 
 
-    def email_list_subscriptions(self,
-            email_addr : Optional[str] = None,
-            email_list : Optional[EmailList] = None) -> Iterator[EmailListSubscriptions]:
-        url = EmailListSubscriptionsURI("/api/v1/mailinglists/subscribed/")
-        if email_addr is not None:
-            url.params["email"] = email_addr
-        if email_list is not None:
-            url.params["lists"] = email_list.id
-        yield from self._retrieve_multi(url, EmailListSubscriptions)
+    # def email_lists(self, name : Optional[str] = None) -> Iterator[EmailList]:
+    #     url = EmailListURI(uri="/api/v1/mailinglists/list/")
+    #     if name is not None:
+    #         url.params["name"] = name
+    #     yield from self._retrieve_multi(url, EmailList)
+
+
+    # def email_list_subscriptions(self,
+    #         email_addr : Optional[str] = None,
+    #         email_list : Optional[EmailList] = None) -> Iterator[EmailListSubscriptions]:
+    #     url = EmailListSubscriptionsURI(uri="/api/v1/mailinglists/subscribed/")
+    #     if email_addr is not None:
+    #         url.params["email"] = email_addr
+    #     if email_list is not None:
+    #         url.params["lists"] = email_list.id
+    #     yield from self._retrieve_multi(url, EmailListSubscriptions)
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about names:
     #
     # FIXME: move these into the appropriate place
     #
@@ -3725,36 +3597,36 @@
     # * https://datatracker.ietf.org/api/v1/name/continentname/
 
     def continent(self, continent_uri : ContinentURI) -> Optional[Continent]:
         return self._retrieve(continent_uri, Continent)
 
 
     def continent_from_slug(self, slug : str) -> Optional[Continent]:
-        return self._retrieve(ContinentURI(F"/api/v1/name/continentname/{slug}/"), Continent)
+        return self._retrieve(ContinentURI(uri=f"/api/v1/name/continentname/{slug}/"), Continent)
 
 
     def continents(self) -> Iterator[Continent]:
-        url = ContinentURI("/api/v1/name/continentname/")
+        url = ContinentURI(uri="/api/v1/name/continentname/")
         yield from self._retrieve_multi(url, Continent)
 
 
     def country(self, country_uri: CountryURI) -> Optional[Country]:
         return self._retrieve(country_uri, Country)
 
 
     def country_from_slug(self, slug : str) -> Optional[Country]:
-        return self._retrieve(CountryURI(F"/api/v1/name/countryname/{slug}/"), Country)
+        return self._retrieve(CountryURI(uri=f"/api/v1/name/countryname/{slug}/"), Country)
 
 
     def countries(self,
                   continent_slug : Optional[str]  = None,
                   in_eu          : Optional[bool] = None,
                   slug           : Optional[str]  = None,
                   name           : Optional[str]  = None) -> Iterator[Country]:
-        url = CountryURI("/api/v1/name/countryname/")
+        url = CountryURI(uri="/api/v1/name/countryname/")
         if continent_slug is not None:
             url.params["continent"] = continent_slug
         if in_eu is not None:
             url.params["in_eu"] = in_eu
         if slug is not None:
             url.params["slug"] = slug
         if name is not None:
@@ -3763,15 +3635,15 @@
 
 
     def country_alias(self, country_alias_uri : CountryAliasURI) -> Optional[CountryAlias]:
         return self._retrieve(country_alias_uri, CountryAlias)
 
 
     def country_aliases(self, alias : str) -> Iterator[CountryAlias]:
-        url = CountryAliasURI("/api/v1/stats/countryalias/")
+        url = CountryAliasURI(uri="/api/v1/stats/countryalias/")
         url.params["alias"] = alias
         yield from self._retrieve_multi(url, CountryAlias)
 
 
     # ----------------------------------------------------------------------------------------------------------------------------
     # Datatracker API endpoints returning information about statistics:
     #
@@ -3790,15 +3662,15 @@
                 email         : Optional[str]             = None,
                 first_name    : Optional[str]             = None,
                 last_name     : Optional[str]             = None,
                 meeting       : Optional[Meeting]         = None,
                 person        : Optional[Person]          = None,
                 reg_type      : Optional[str]             = None,
                 ticket_type   : Optional[str]             = None) -> Iterator[MeetingRegistration]:
-        url = MeetingRegistrationURI("/api/v1/stats/meetingregistration/")
+        url = MeetingRegistrationURI(uri="/api/v1/stats/meetingregistration/")
         if affiliation is not None:
             url.params["affiliation"] = affiliation
         if attended is not None:
             url.params["attended"] = attended
         if country_code is not None:
             url.params["country_code"] = country_code
         if email is not None:
@@ -3830,15 +3702,15 @@
         return self._retrieve(announcement_from_uri, AnnouncementFrom)
 
 
     def announcements_from(self,
                 address : Optional[str]          = None,
                 group   : Optional[Group]        = None,
                 name    : Optional[RoleName]     = None) -> Iterator[AnnouncementFrom]:
-        url = AnnouncementFromURI("/api/v1/message/announcementfrom/")
+        url = AnnouncementFromURI(uri="/api/v1/message/announcementfrom/")
         if address is not None:
             url.params["address"] = address
         if group is not None:
             url.params["group"] = group.id
         if name is not None:
             url.params["name"] = name.slug
         yield from self._retrieve_multi(url, AnnouncementFrom)
@@ -3852,15 +3724,15 @@
     #            since : str                           = "1970-01-01T00:00:00",
     #            until : str                           = "2038-01-19T03:14:07",
     #            by               : Optional[Person]   = None,
     #            frm              : Optional[str]      = None,
     #            related_doc      : Optional[Document] = None,
     #            subject_contains : Optional[str]      = None,
     #            body_contains    : Optional[str]      = None) -> Iterator[DTMessage]:
-    #    url = DTMessageURI("/api/v1/message/message/")
+    #    url = DTMessageURI(uri="/api/v1/message/message/")
     #    url.params["time__gte"]       = since
     #    url.params["time__lt"]       = until
     #    if by is not None:
     #        url.params["by"] = by.id
     #    if frm is not None:
     #        url.params["frm"] = frm
     #    if related_doc is not None:
@@ -3877,15 +3749,15 @@
 
 
     def send_queue(self,
                 since   : str                = "1970-01-01T00:00:00",
                 until   : str                = "2038-01-19T03:14:07",
                 by      : Optional[Person]   = None,
                 message : Optional[DTMessage]  = None) -> Iterator[SendQueueEntry]:
-        url = SendQueueURI("/api/v1/message/sendqueue/")
+        url = SendQueueURI(uri="/api/v1/message/sendqueue/")
         url.params["time__gte"] = since
         url.params["time__lt"]  = until
         if by is not None:
             url.params["by"] = by.id
         if message is not None:
             url.params["message"] = message.id
         yield from self._retrieve_multi(url, SendQueueEntry)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ietfdata-0.6.8/ietfdata/datatracker_ext.py` & `ietfdata-0.7.0/ietfdata/datatracker_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         # If given, e.g. "Colin Perkins (csperkins)" also try "Colin Perkins":
         if len(split) == 3 and len(split[2]) >= 2 and split[2][0] == "(" and split[2][-1] == ")":
             alias = split[0] + " " + split[1]
             names.append(alias)
 
     # Derive names from the email address:
     if "@" in email:
-        local, remote = email.split("@")
+        local, remote = email.rsplit("@", 1)
 
         if local.endswith(".ietf") or local.endswith("-ietf") or local.endswith("+ietf"):
             local = local[:-5]
         split = local.split(".")
 
         # If given, e.g., "colin.perkins@glasgow.ac.uk" also try "Colin Perkins":
         if len(split) == 2 and len(split[0]) > 1 and len(split[1]) > 1:
@@ -69,47 +69,55 @@
         # If given, e.g., "mary.h.barnes@gmail.com" also try "Mary H. Barnes" and "Mary Barnes":
         if len(split) == 3 and len(split[0]) > 1 and len(split[1]) == 1 and len(split[2]) > 1:
             alias = split[0][0].upper() + split[0][1:] + " " + split[1].upper() + ". " + split[2][0].upper() + split[2][1:]
             names.append(alias)
             alias = split[0][0].upper() + split[0][1:] + " " + split[2][0].upper() + split[2][1:]
             names.append(alias)
 
-    return names
+    utf8_safe_names = []
+    for n in names:
+        try:
+            n.encode("utf-8")
+            utf8_safe_names.append(n)
+        except UnicodeEncodeError:
+            pass
+
+    return utf8_safe_names
 
 # =================================================================================================================================
 
 @dataclass
 class DraftHistory:
     draft      : Document
     rev        : str
-    date       : datetime
+    date       : date
     submission : Optional[Submission]
 
 
 class DataTrackerExt(DataTracker):
     """
     The `DataTrackerExt` class extends the `DataTracker` with methods that
     perform complex queries across multiple API endpoints.
     """
 
     def __init__(self,
-            use_cache: bool = False,
-            mongodb_hostname: str = "localhost",
-            mongodb_port: int = 27017,
-            mongodb_username: Optional[str] = None,
-            mongodb_password: Optional[str] = None):
-        super().__init__(use_cache, mongodb_hostname, mongodb_port, mongodb_username, mongodb_password)
-
+                 use_cache     : bool = False,
+                 mongodb_host  : str  = os.getenv("IETFDATA_CACHE_HOST", "localhost"),
+                 mongodb_port  : str  = os.getenv("IETFDATA_CACHE_PORT", "27017"),
+                 mongodb_user  : Optional[str] = os.getenv("IETFDATA_CACHE_USER"),
+                 mongodb_pass  : Optional[str] = os.getenv("IETFDATA_CACHE_PASSWORD"),
+                 cache_timeout : Optional[timedelta] = None):
+        super().__init__(use_cache, mongodb_host, mongodb_port, mongodb_user, mongodb_pass, cache_timeout)
 
 
     def draft_history(self, draft: Document, drafts_seen: List[Document] = []) -> List[DraftHistory]:
         """
         Find the previous versions of an Internet-Draft
         """
-        assert draft.type == DocumentTypeURI("/api/v1/name/doctypename/draft/")
+        assert draft.type == DocumentTypeURI(uri="/api/v1/name/doctypename/draft/")
 
         drafts : List[DraftHistory] = []
 
         if draft in drafts_seen:
             return []
         else:
             drafts_seen.append(draft)
@@ -149,25 +157,23 @@
                     found = True
                     break
             if not found:
                 drafts.append(DraftHistory(draft, submission.rev, submission.submission_date, submission))
 
         # Step 3: Use related_documents() to find additional drafts this replaces:
         for related in self.related_documents(source=draft, relationship_type=self.relationship_type_from_slug("replaces")):
-            alias  = self.document_alias(related.target)
-            if alias is not None:
-                reldoc = self.document(alias.document)
-                if reldoc is not None:
-                    found = False
-                    for r in replaces:
-                        if r.name == reldoc.name:
-                            found = True
-                            break
-                    if not found:
-                        replaces.append(reldoc)
+            reldoc = self.document(related.target)
+            if reldoc is not None:
+                found = False
+                for r in replaces:
+                    if r.name == reldoc.name:
+                        found = True
+                        break
+                if not found:
+                    replaces.append(reldoc)
 
         # Step 4: Process the drafts this replaces, to find earlier versions:
         for r in replaces:
             if r.name != draft.name:
                 drafts.extend(self.draft_history(r, drafts_seen=drafts_seen))
 
         return list(reversed(sorted(drafts, key=lambda d: d.date)))
@@ -323,25 +329,31 @@
 
     def person_from_name_email(self, name: str, email_addr: str) -> Optional[Person]:
         """
         Given a name and an email address, for example as might be extracted from an
         email "From:" header, try to find a person in the datatracker. This uses a
         number of heuristics if there is no exact match.
         """
+        assert len(email_addr) > 0
+
+        # Decode DMARC (e.g., arnaud.taddei=40broadcom.com@dmarc.ietf.org -> arnaud.taddei@broadcom.com)
+        if email_addr.endswith("@dmarc.ietf.org"):
+            email_addr = email_addr[:-15].replace("=40", "@")
+
         # Try to match on the email address:
         email = self.email_for_address(email_addr)
         if email is not None and email.person is not None:
             self.log.debug(f"person_from_name_email: {name} <{email_addr}> -> {email.person} (email match)")
             return self.person(email.person)
 
         # Try to match on the base email address:
         if "@" in email_addr:
-            local, remote = email_addr.split("@")
+            local, remote = email_addr.rsplit("@", 1)
             if local.count("+") == 1:
-                base, suffix = local.split("+")
+                base, suffix = local.rsplit("+", 1)
                 email_base = F"{base}@{remote}"
                 email = self.email_for_address(email_base)
                 if email is not None and email.person is not None:
                     self.log.debug(f"person_from_name_email: {name} <{email_addr}> -> {email.person} (email match as {email_base})")
                     return self.person(email.person)
 
         # Try to match on the name:
```

### Comparing `ietfdata-0.6.8/ietfdata/mailarchive2.py` & `ietfdata-0.7.0/ietfdata/mailarchive2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2022 University of Glasgow
+# Copyright (C) 2020-2023 University of Glasgow
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -30,20 +30,20 @@
 import pandas as pd
 import os
 import logging
 import time
 
 from datetime           import datetime, timedelta
 from graphlib           import TopologicalSorter
-from typing             import Dict, Iterator, List, Optional, Tuple, Union
+from typing             import Dict, Iterator, List, Optional, Tuple, Union, Any
 from gridfs             import GridFS
 from pymongo            import MongoClient, ASCENDING, ReplaceOne, UpdateOne
 from pymongo.database   import Database
 from email              import policy, utils
-from email.message      import Message as EmailMessage
+from email.message      import Message
 from email_reply_parser import EmailReplyParser
 from imapclient         import IMAPClient
 from dataclasses        import field
 
 # =================================================================================================
 # Database design for the mail archive:
 #
@@ -53,14 +53,23 @@
 # The `lists` collection contains documents of the form:
 #
 #   {
 #     list: "100attendees"
 #     uidvalidity: 1505323361
 #   }
 #
+# The `lists_metadata` collections contains documents of the form:
+#
+#   {
+#     "list": "100attendees",
+#     "project": "sodestream",
+#     "key": "is_spam",
+#     "value": False,
+#   }
+#
 # The uidvalidity value is provided by the IMAP server when selecting a mailbox,
 # and should never change. If it does, messages with the old uidvalidity MUST be
 # deleted and the mailbox MUST be re-downloaded.
 #
 # The `messages` collections contains documents of the form:
 #
 #   {
@@ -87,211 +96,262 @@
 # where the timestamp is the IMAP INTERNALDATE [RFC 3501, Section 2.3.3] represented
 # as a `datetime`, and the size is the IMAP RFC822.SIZE  [RFC 3501, Section 2.3.4].
 # The headers is a dictionary containing the headers parsed from the messages, with
 # each element containing a list of header values, one for each time that header appears
 # in the message. The gridfs_id points to a file containing the raw message content (the
 # IMAP RFC822 fetch result).
 #
+# The `parsed_headers` collections contains documents of the form:
+#
+#   { # FIXME: implement this
+#     "list": "100attendees",
+#     "uidvalidity": 1505323361m
+#     "uid":  1,
+#     "message_id": "<CAAiTEH9EVrZzF08F4T3z6QzhAnwBmKk9jhHEf=xMy-=3W4r9+Q@mail.gmail.com>",
+#     "date": 2017-09-13T10:11:47.000+00:00,
+#     "from": ["matt@conundrum.com"],        # DMARC rewriting undone, email address extracted
+#     "to":   ["100attendees@ietf.org"],     # Email addresses extracted
+#     "cc":   [],                            # Email addresses extracted
+#   }
+#
+# The `metadata` collections contains documents of the form:
+#
+#   {
+#     "list": "100attendees",
+#     "uidvalidity": 1505323361
+#     "uid":  1,
+#     "message_id": "<CAAiTEH9EVrZzF08F4T3z6QzhAnwBmKk9jhHEf=xMy-=3W4r9+Q@mail.gmail.com>",
+#     "project": "sodestream",
+#     "key": "is_spam",
+#     "value": False,
+#   }
+#
 # =================================================================================================
 
-class Message:
-    _mailing_list : MailingList
-    _uidvalidity  : int
-    _uid          : int
-    _gridfs_id    : int
-    _timestamp    : datetime
-    _size         : int
-    _headers      : Dict[str, List[str]]
-    _parent       : Optional[Message] = None
-    _children     : List[Message] = field(default_factory=list)
+class Envelope:
+    _mailing_list  : MailingList
+    _uidvalidity   : int
+    _uid           : int
+    _gridfs_id     : int
+    _dste_received : datetime
+    _size          : int
+    _headers       : Dict[str, List[str]]
 
     def __init__(self,
-                 ml: MailingList,
-                 uidvalidity: int,
-                 uid: int,
-                 gridfs_id: int,
-                 timestamp: datetime,
-                 size:int,
-                 headers: Dict[str, List[str]]) -> None:
-        self._mailing_list = ml
-        self._uidvalidity  = uidvalidity
-        self._uid          = uid
-        self._gridfs_id    = gridfs_id
-        self._timestamp    = timestamp
-        self._size         = size
-        self._headers      = headers
-        self._children     = []
-
-
-    # Accessors for messages properties. Messages in IMAP are assigned
-    # a unique identifier `uid()` within a folder representing a mailing
-    # list. That identifier is not supposed to change, but the IMAP
-    # standard recognises that mailboxes occasionally get rebuilt. If
-    # this happens, the `uidvalidity()` will change. The combination of
-    # mailing_list(), uid(), and uidvalidity() uniquely identifies a 
-    # message on the server.
+                 ml            : MailingList,
+                 uidvalidity   : int,
+                 uid           : int,
+                 gridfs_id     : int,
+                 date_received : datetime,
+                 size          : int,
+                 headers       : Dict[str, List[str]]) -> None:
+        self._mailing_list  = ml
+        self._uidvalidity   = uidvalidity
+        self._uid           = uid
+        self._gridfs_id     = gridfs_id
+        self._dste_received = date_received
+        self._size          = size
+        self._headers       = headers
+
+
+    # Accessors for properties of the message in this Envelope.
+    #
+    # Messages in IMAP are assigned a unique identifier `uid()` within a folder
+    # representing a mailing list. That identifier is not supposed to change,
+    # but the IMAP standard recognises that mailboxes occasionally get rebuilt.
+    # If this happens, the `uidvalidity()` will change. The combination of
+    # mailing_list(), uid(), and uidvalidity() uniquely identifies a message on
+    # the server.
+
     def mailing_list(self) -> MailingList:
         return self._mailing_list
 
 
     def uidvalidity(self) -> int:
         return self._uidvalidity
 
 
     def uid(self) -> int:
         return self._uid
 
 
-    # Timestamp is the time the messages was received by the IMAP server
-    def timestamp(self) -> datetime:
-        return self._timestamp
+    def date_received(self) -> datetime:
+        return self._dste_received
 
 
     def size(self) -> int:
         return self._size
 
 
-    # Accessors for commonly-used headers:
-    def header_from(self) -> Optional[str]:
-        return self._headers["from"][0] if "from" in self._headers else None
-
-
-    def header_to(self) -> Optional[str]:
-        return self._headers["to"][0] if "to" in self._headers else None
-
-
-    def header_cc(self) -> Optional[str]:
-        return self._headers["cc"][0] if "cc" in self._headers else None
-
-
-    def header_subject(self) -> Optional[str]:
-        return self._headers["subject"][0] if "subject" in self._headers else None
-
-
-    def header_date(self) -> Optional[datetime]:
+    def date(self) -> Optional[datetime]:
+        """
+        The "Date:" header from the Message within this Envelope, parsed into a
+        `DateTime` object.
+
+        This will return `None` if the "Date:" header is not present or cannot
+        be parsed.
+
+        The `header("date")` method can be used to return the unparsed "Date:"
+        header as a `str`.
+        """
         msg_date = None # type: Optional[datetime]
         try:
-            parsed_date = email.utils.parsedate(self._headers["date"][0]) 
+            parsed_date = email.utils.parsedate(self._headers["date"][0])
             if parsed_date is not None:
                 msg_date = datetime.fromtimestamp(time.mktime(parsed_date))
             else:
                 msg_date = None
         except:
             msg_date = None
         return msg_date
 
 
-    def header_message_id(self) -> Optional[str]:
-        return self._headers["message-id"][0] if "message-id" in self._headers else None
-
-
-    def header_in_reply_to(self) -> Optional[str]:
-        return self._headers["in-reply-to"][0] if "in-reply-to" in self._headers else None
-
-
-    def header_references(self) -> Optional[str]:
-        return self._headers["references"][0] if "references" in self._headers else None
+    def header(self, header_name:str) -> List[str]:
+        """
+        Accessor for the headers of the message in this Envelope.
 
+        Some headers, e.g., "Received:" are expected to occur multiple times
+        within a message and will return a list containing multiple items.
 
-    # Accessor for other headers:
-    def header(self, header_name:str) -> List[str]:
-        return self._headers[header_name]
+        Other headers, e.g., "From:", are only supposed to occur once in each
+        message. In these cases, this method should return a list containing a
+        single value. Note, however, that the IETF mail archive contains some
+        malformed messages with unexpected duplicate headers. For example,
+        there are some messages with two addresses in the "From:" line.
+        """
+        if not header_name in self._headers:
+            return []
+        else:
+            return self._headers[header_name]
 
 
-    # Accessor for message body:
-    def body(self) -> EmailMessage:
+    def contents(self) -> Message:
+        """
+        Return the Message contained within this Envelope.
+        """
         msg = self._mailing_list._mail_archive._fs.get(self._gridfs_id)
         return email.message_from_bytes(msg.read(), policy=policy.default)
 
 
-    # Find the messages that this is in reply to. Each message can only be
-    # in reply to a single other message, but there may be multiple copies
-    # of that message in the archive if it was sent to multiple lists, each
-    # of which may have different replies.  This method returns all the copies.
-    # If this is the first message in a thread, then an empty list is returned.
-    def in_reply_to(self) -> List[Message]:
-        in_reply_to = self.header_in_reply_to()
-        references  = self.header_references()
-        if in_reply_to is not None:
-            parent = in_reply_to
-        elif references is not None:
-            parent = references.split(" ")[-1]
+    def in_reply_to(self) -> List[Envelope]:
+        """
+        Return the envelopes containing the messages that this is in reply to.
+
+        Each message can only be in reply to a single other message, but there
+        may be multiple copies of that message in the archive if it was sent to
+        multiple lists, each of which may itself have different replies. This
+        method returns all such copies.
+
+        If this is the first message in a thread, then an empty list is returned.
+        """
+        in_reply_to = self.header("in-reply-to")
+        references  = self.header("references")
+        if len(in_reply_to) == 1:
+            parent = in_reply_to[0]
+        elif references is not None and len(references) > 0:
+            parent = references[0].split(" ")[-1]
         else:
             return []
         parents = []
         for message in self._mailing_list._mail_archive._db.messages.find({"message_id": parent}):
-            mailing_list = self._mailing_list._mail_archive.mailing_list(message["list"])
-            uidvalidity  = message["uidvalidity"]
-            uid          = message["uid"]
-            gridfs_id    = message["gridfs_id"]
-            timestamp    = message["timestamp"]
-            size         = message["size"]
-            headers      = message["headers"]
-            parents.append(Message(mailing_list, uidvalidity, uid, gridfs_id, timestamp, size, headers))
+            mailing_list  = self._mailing_list._mail_archive.mailing_list(message["list"])
+            uidvalidity   = message["uidvalidity"]
+            uid           = message["uid"]
+            gridfs_id     = message["gridfs_id"]
+            date_received = message["timestamp"]
+            size          = message["size"]
+            headers       = message["headers"]
+            parents.append(Envelope(mailing_list, uidvalidity, uid, gridfs_id, date_received, size, headers))
         return parents
 
 
-    def replies(self) -> List[Message]:
+    def replies(self) -> List[Envelope]:
+        """
+        Return the envelopes containing the messages sent in reply to this.
+        """
         replies = []
-        for message in self._mailing_list._mail_archive._db.messages.find({"in_reply_to": self.header_message_id()}):
-            mailing_list = self._mailing_list._mail_archive.mailing_list(message["list"])
-            uidvalidity  = message["uidvalidity"]
-            uid          = message["uid"]
-            gridfs_id    = message["gridfs_id"]
-            timestamp    = message["timestamp"]
-            size         = message["size"]
-            headers      = message["headers"]
-            replies.append(Message(mailing_list, uidvalidity, uid, gridfs_id, timestamp, size, headers))
+        for message in self._mailing_list._mail_archive._db.messages.find({"in_reply_to": self.header("message-id")[0]}):
+            mailing_list  = self._mailing_list._mail_archive.mailing_list(message["list"])
+            uidvalidity   = message["uidvalidity"]
+            uid           = message["uid"]
+            gridfs_id     = message["gridfs_id"]
+            date_received = message["timestamp"]
+            size          = message["size"]
+            headers       = message["headers"]
+            replies.append(Envelope(mailing_list, uidvalidity, uid, gridfs_id, date_received, size, headers))
         return replies
 
 
-    def add_child_message(self, child: Message):
-        self._children.append(child)
-
-
-    def get_child_count(self) -> int:
-        return len(self._children) + sum([child.get_child_count() for child in self._children])
-
-
-    def get_child_from_addrs(self, child_from_addrs: List[str]) -> List[str]:
-        header_from = self.header_from()
-        if header_from is not None:
-            child_from_addrs.append(header_from)
-        for child in self._children:
-            child.get_child_from_addrs(child_from_addrs)
-        return child_from_addrs
-
-
-    def get_child_dates(self, child_dates: List[datetime]):
-        child_dates.append(self.timestamp())
-        for child in self._children:
-            child.get_child_dates(child_dates)
-        return child_dates
-
-
-# =================================================================================================
-
-class MessageThread:
-    def __init__(self, root: Message):
-        self.root = root
-
-
-    def get_message_count(self):
-        return 1 + self.root.get_child_count()
-
-
-    def get_unique_from_count(self):
-        from_addrs = self.root.get_child_from_addrs([])
-        return len(list(set(from_addrs)))
+    def add_metadata(self, project:str, key:str, value):
+        """
+        Add metadata relating to the message in this envelope.
+
+        Parameters:
+        - `project` -- the project or user to which this metadata relates
+        - `key`     -- the key under which the metadata should be scored
+        - `value`   -- the value of the metadata to store
+
+        The `project` is intended to allow different users to store metadata
+        in a shared mail archive database. For example, a group project that
+        works with the mail archive might tag message envelopes with agreed-
+        upon metadata using the project's name in the `project` field, while
+        exploratory work from individual members of the project might use
+        their username as the basis for the `project` (e.g., "alice_test4").
+        """
+        entry = {"list"        : self.mailing_list().name(),
+                 "uidvalidity" : self.uidvalidity(),
+                 "uid"         : self.uid(),
+                 "message_id"  : self._headers["message-id"][0] if "message-id" in self._headers else None,
+                 "project"     : project,
+                 "key"         : key,
+                 "value"       : value,
+        }
+        self._mailing_list._mail_archive._db.metadata.insert_one(entry)
+
+
+    def get_metadata(self, project:str, key:str):
+        """
+        Get metadata relating to the message in this envelope.
+
+        Parameters:
+        - `project` -- the project or user to which this metadata relates
+        - `key`     -- the key under which the metadata was scored
+        """
+        query = {"list"        : self.mailing_list().name(),
+                 "uidvalidity" : self.uidvalidity(),
+                 "uid"         : self.uid(),
+                 "project"     : project,
+                 "key"         : key}
+        result = self._mailing_list._mail_archive._db.metadata.find_one(query) # type: Optional[Dict[str, Any]]
+        if result is not None:
+            return result["value"]
+        else:
+            return None
 
 
-    def get_duration(self):
-        earliest_date = self.root.timestamp()
-        latest_date = sorted(self.root.get_child_dates([]), reverse=True)[0]
-        return latest_date - earliest_date
+    def clear_metadata(self, project:str, key:Optional[str] = None):
+        """
+        Remove metadata relating to the message in this envelope.
+
+        Parameters:
+        - `project` -- the project or user to which this metadata relates
+        - `key`     -- the key under which the metadata was scored
+
+        If the `key` is specified then only the single metadata value
+        identified by the `project` and `key` is removed. If the `key`
+        is not specified, then all metadata relating to `project` is
+        removed from this envelope.
+        """
+        query = {"list"        : self.mailing_list().name(),
+                 "uidvalidity" : self.uidvalidity(),
+                 "uid"         : self.uid(),
+                 "project"     : project}
+        if key is not None:
+            query["key"] = key
+        self._mailing_list._mail_archive._db.metadata.delete_many(query)
 
 
 # =================================================================================================
 
 class MailingList:
     _log          : logging.Logger
     _mail_archive : MailArchive
@@ -301,25 +361,30 @@
     def __init__(self, mail_archive: MailArchive, list_name: str):
         logging.basicConfig(level=os.environ.get("IETFDATA_LOGLEVEL", "INFO"))
         self._log          = logging.getLogger("ietfdata")
         self._mail_archive = mail_archive
         self._list_name    = list_name
         ml = self._mail_archive._db.lists.find_one({"list": list_name})
         if ml is None:
-            imap = IMAPClient(host='imap.ietf.org', ssl=True, use_uid=True)
+            imap = IMAPClient(host=self._mail_archive._imap_server, ssl=True, use_uid=True)
             imap.login("anonymous", "anonymous")
-            status_imap = imap.folder_status("Shared Folders/" + self._list_name)
+
+            _, _, imap_ns_shared = imap.namespace()
+            imap_prefix    = imap_ns_shared[0][0]
+            imap_separator = imap_ns_shared[0][1]
+
+            status_imap = imap.folder_status(f"{imap_prefix}{self._list_name}")
             status_json = {
                 "list"         : self._list_name,
                 "uidvalidity"  : status_imap[b'UIDVALIDITY'],
             }
             self._mail_archive._db.lists.insert_one(status_json)
             imap.logout()
-            self._log.info(f"Created cache for list {self._list_name}")
             self._uidvalidity = status_imap[b'UIDVALIDITY']
+            self._log.info(f"Created cache for list {self._list_name}")
         else:
             self._uidvalidity = ml["uidvalidity"] #type: int
 
 
     def name(self) -> str:
         return self._list_name
 
@@ -333,118 +398,151 @@
 
 
     def message_uids(self) -> Iterator[int]:
         for msg in self._mail_archive._db.messages.find({"list" : self._list_name, "uidvalidity": self._uidvalidity}):
             yield msg["uid"]
 
 
-    def message(self, uid: int) -> Optional[Message]:
+    def message(self, uid: int) -> Optional[Envelope]:
+        """
+        Return the Envelope containing the Message identified by the
+        specified uid within this mailing list.
+        """
         message = self._mail_archive._db.messages.find_one({"list" : self._list_name, "uidvalidity": self._uidvalidity, "uid": uid})
         if message is not None:
             uidvalidity = message["uidvalidity"]
             uid         = message["uid"]
             gridfs_id   = message["gridfs_id"]
             timestamp   = message["timestamp"]
             size        = message["size"]
             headers     = message["headers"]
-            return Message(self, uidvalidity, uid, gridfs_id, timestamp, size, headers)
+            return Envelope(self, uidvalidity, uid, gridfs_id, timestamp, size, headers)
         else:
             return None
 
 
-    def messages(self, since: str = "1970-01-01T00:00:00", until: str = "2038-01-19T03:14:07") -> Iterator[Message]:
+    def messages(self,
+                 received_after: str = "1970-01-01T00:00:00",
+                 received_before: str = "2038-01-19T03:14:07") -> Iterator[Envelope]:
+        """
+        Return the envelopes containing the specified messages from this mailing list.
+        """
         query = {"list"        : self._list_name,
                  "uidvalidity" : self._uidvalidity,
                  "timestamp"   : {
-                     "$gt": datetime.strptime(since, "%Y-%m-%dT%H:%M:%S"),
-                     "$lt": datetime.strptime(until, "%Y-%m-%dT%H:%M:%S")
+                     "$gt": datetime.strptime(received_after,  "%Y-%m-%dT%H:%M:%S"),
+                     "$lt": datetime.strptime(received_before, "%Y-%m-%dT%H:%M:%S")
                  }
                 }
-        messages = self._mail_archive._db.messages.find(query, no_cursor_timeout=True)
+        messages = self._mail_archive._db.messages.find(query, sort=[("uid", ASCENDING)], batch_size=100)
         for message in messages:
             uidvalidity = message["uidvalidity"]
             uid         = message["uid"]
             gridfs_id   = message["gridfs_id"]
             timestamp   = message["timestamp"]
             size        = message["size"]
             headers     = message["headers"]
-            yield Message(self, uidvalidity, uid, gridfs_id, timestamp, size, headers)
-        messages.close()
+            yield Envelope(self, uidvalidity, uid, gridfs_id, timestamp, size, headers)
 
 
     def messages_as_dataframe(self,
-                 since : str = "1970-01-01T00:00:00",
-                 until : str = "2038-01-19T03:14:07") -> pd.DataFrame:
+                              received_after  : str = "1970-01-01T00:00:00",
+                              received_before : str = "2038-01-19T03:14:07") -> pd.DataFrame:
+        """
+        Return a dataframe containing information about the specified messages from
+        this mailing list.
+        """
         messages_as_dict = []
-        for message in self.messages(since = since, until = until):
-            mdict = {"Message-ID"  : message.header_message_id(),
-                     "From"        : message.header_from(),
-                     "To"          : message.header_to(),
-                     "Cc"          : message.header_cc(),
-                     "Subject"     : message.header_subject(),
-                     "Date"        : message.header_date(),
-                     "In-Reply-To" : message.header_in_reply_to(),
-                     "References"  : message.header_references()}
+        for message in self.messages(received_after = received_after, received_before = received_before):
+            mdict = {"Message-ID"  : message.header("message-id")[0] if message.header("message-id") != [] else None,
+                     "From"        : message.header("from")[0],
+                     "To"          : message.header("to"),
+                     "Cc"          : message.header("cc"),
+                     "Subject"     : message.header("subject")[0],
+                     "Date"        : message.date(),
+                     "In-Reply-To" : message.header("in-reply-to") if message.header("in-reply-to") != [] else None,
+                     "References"  : message.header("references"),
+                    }
             messages_as_dict.append(mdict)
         df = pd.DataFrame(data=messages_as_dict)
         df.set_index("Message-ID", inplace=True)
         return df
 
 
-    def update(self) -> List[int]:
+    # FIXME: this should update the parsed_headers database collection
+    def update(self, verbose=True) -> List[int]:
+        """
+        Update the local copy of this mailing list from the IMAP server.
+
+        This MUST be called at least once for each mailing list, else no
+        messages will be retrieved from the server. That initial update
+        may well be slow, since it downloads the entire set of messages
+        from the list. Subsequent calls to `update()` only fetch the new
+        messages and so are much faster.
+        """
+        if verbose:
+            print(f"[mailarchive] Check {self._list_name}")
+
+        # Login to the IMAP server:
         self._log.info(f"Updating list {self.name()}")
-        imap = IMAPClient(host='imap.ietf.org', ssl=True, use_uid=True)
+        imap = IMAPClient(host=self._mail_archive._imap_server, ssl=True, use_uid=True)
         imap.login("anonymous", "anonymous")
-
-        folder_status = imap.folder_status("Shared Folders/" + self._list_name)
+        _, _, imap_ns_shared = imap.namespace()
+        imap_prefix    = imap_ns_shared[0][0]
+        imap_separator = imap_ns_shared[0][1]
+        folder_status  = imap.folder_status(f"{imap_prefix}{self._list_name}")
+
+        # If UIDVALIDITY has changed, the cache will be invalid and we must re-download
+        # the entire folder. IMAP servers are supposed to ensure the UIDVALIDITY doesn't
+        # change, but sometimes a re-index occurs on the server so we have to handle it.
         if folder_status[b'UIDVALIDITY'] != self._uidvalidity:
-            # if UIDVALIDITY has changed, the cache will be invalid and we must re-download
-            # the entire folder. IMAP servers are supposed to ensure the UIDVALIDITY doesn't
-            # change, but sometimes a re-index occurs on the server so we have to handle it.
             self._log.warn(f"UIDVALIDITY changed for mailing list {self._list_name}")
             # Remove messages with old uidvalidity:
             for msg in self._mail_archive._db.messages.find({"list": self._list_name, "uidvalidity": self._uidvalidity}):
                 self._mail_archive._fs.delete(msg["gridfs_id"])
                 self._mail_archive._db.messages.delete_one({"list" : self._list_name, "uidvalidity": self._uidvalidity, "uid" : msg['uid']})
+                if verbose:
+                    print(f"[mailarchive] Remove {self._list_name}/{msg['uid']} due to UIDVALIDITY change")
             # Write the new uidvalidity to the database:
             list_status = {
                 "list"        : self._list_name,
                 "uidvalidity" : folder_status[b'UIDVALIDITY'],
             }
             self._mail_archive._db.lists.replace_one({"list" : self._list_name}, list_status)
             self._uidvalidity = folder_status[b'UIDVALIDITY']
 
-        imap.select_folder("Shared Folders/" + self._list_name, readonly=True)
+        # Find the messages to fetch:
+        imap.select_folder(f"{imap_prefix}{self._list_name}", readonly=True)
         server_messages = imap.search()
         cached_messages = list(self.message_uids())
         msgs_to_fetch   = []
-
-        # Find the messages to fetch:
         for uid in server_messages:
             if uid not in cached_messages:
                 msgs_to_fetch.append(uid)
 
-        # Fetch the messages
+        # Fetch the messages:
         for i in range(0, len(msgs_to_fetch), 16):
             uid_slice = msgs_to_fetch[slice(i, i+16, 1)]
             for uid, msg in imap.fetch(uid_slice, "INTERNALDATE RFC822.SIZE RFC822").items():
+                if verbose:
+                    print(f"[mailarchive] Fetch {self._list_name}/{uid}")
                 e = email.message_from_bytes(msg[b"RFC822"], policy=policy.default)
                 # Extract the headers:
                 headers = {}
                 try:
                     for header in e.keys():
                         if header not in headers:
                             try:
                                 header_values = e.get_all(header)
                                 if header_values is not None:
                                     headers[header.lower().replace(".", "-")] = header_values
                             except Exception as ex:
-                                self._log.info(f"cannot extract header {header} for {self._list_name}/{uid}")
+                                self._log.warn(f"Cannot extract header {header} for {self._list_name}/{uid}")
                 except:
-                    self._log.info(f"cannot extract headers for {self._list_name}/{uid}")
+                    self._log.warn(f"Cannot extract headers for {self._list_name}/{uid}")
                 # Find the parent message:
                 if "in-reply-to" in headers:
                     in_reply_to = headers["in-reply-to"][0]
                 elif "references" in headers:
                     in_reply_to = headers["references"][0].split(" ")[-1]
                 else:
                     in_reply_to = None
@@ -464,115 +562,326 @@
                 self._log.info(f"saved message {self._list_name}/{uid}")
 
         imap.unselect_folder()
         imap.logout()
         return msgs_to_fetch
 
 
-    def threads(self) -> Iterator[MessageThread]:
-        threads = []
-        message_by_message_id = {message.header_message_id() : message for message in self.messages()}
-
-        for message_id in message_by_message_id:
-            message = message_by_message_id[message_id]
-            if message.header_in_reply_to() is None:
-                threads.append(message)
-            if message.header_in_reply_to() is not None and message.header_in_reply_to() in message_by_message_id:
-                message._parent = message_by_message_id[message.header_in_reply_to()]
-                message_by_message_id[message.header_in_reply_to()].add_child_message(message)
-
-        return iter([MessageThread(message) for message in threads])
-
-    #def threads(self) -> Iterator[MessageThread]:
-    #    ts = TopologicalSorter()
-    #    for msg in self.messages():
-    #        if msg.header_references() is not None:
-    #            ts.add(msg.header_message_id(), msg.header_references().split(" ").reverse())
-    #        elif msg.header_in_reply_to() is not None:
-    #            ts.add(msg.header_message_id(), msg.header_in_reply_to())
-    #        else:
-    #            ts.add(msg.header_message_id())
-    #    for msg_id in ts.static_order():
-    #        print(msg_id)
-
+    def threads(self, this_list_only=False) -> Dict[str, List[Envelope]]:
+        """
+        Returns a dictionary of threads in this mailing list.
+
+        The dictionary returned maps message-id values of the first messages in
+        each thread to lists of the Envelope objects containing that message.
+
+        Threads frequently start on one mailing list and have later messages
+        sent to a different mailing list. If you have a complete copy of the
+        mail archive (i.e., if you previously called `MailArchive::update()`),
+        then this function will track threads across lists to find the first
+        message in each (unless `this_list_only` is set to True).
+
+        The first message in a thread can be copied to several mailing lists.
+        If this happens, the message-id for the thread will map to a list of
+        Envelope objects, each representing a copy of the message sent to a
+        different mailing list.
+        If the first message in the thread was only sent to a single mailing
+        list, then the message-id for the thread will map onto a list with a
+        single Envelope.
+        """
+        threads = {}
+        seen    = {} # type: Dict[str,Envelope]
+        for msg in self.messages():
+            msg_id  = msg.header("message-id")[0]
+            seen[msg_id] = msg
+
+            self._log.debug(f"{msg.uid():5} {msg.header('message-id')} {msg.header('subject')}")
+
+            parents = msg.in_reply_to()
+            if len(parents) == 0:
+                # This is the first message in the thread
+                if msg.header("message-id")[0] not in threads:
+                    threads[msg.header("message-id")[0]] = [msg]
+                self._log.debug("      First in thread")
+            elif parents[0].header("message-id")[0] in seen:
+                # This is part of a thread we've already seen
+                self._log.debug(f"      {parents[0].header('message-id')} {parents[0].header('subject')}")
+                self._log.debug(f"      Continues known thread")
+            else:
+                # This is either a new thread that has been copied to this list
+                # where the earlier messages in the thread are on another list,
+                # or this message is part of an existing thread but has arrived
+                # before its parent.
+                curr = []
+                curr.append(msg)
+                while True:
+                    parents = curr[0].in_reply_to()
+
+                    parent_in_this_list = False
+                    for p in parents:
+                        if p.mailing_list() == self.name():
+                            parent_in_this_list = True
+                    if not parent_in_this_list and this_list_only:
+                        self._log.debug(f"      {parents[0].header('message-id')} {parents[0].header('subject')}")
+                        self._log.debug(f"      Not in this list")
+                        if curr[0].header("message-id")[0] not in threads:
+                            threads[curr[0].header("message-id")[0]] = curr
+                        break
+
+                    if len(parents) == 0:
+                        self._log.debug("      First in thread")
+                        if curr[0].header("message-id")[0] not in threads:
+                            threads[curr[0].header("message-id")[0]] = curr
+                        break
+                    curr = parents
+                    self._log.debug(f"      {curr[0].header('message-id')} {curr[0].header('subject')}")
+        return threads
+
+
+    def add_metadata(self, project:str, key:str, value):
+        """
+        Add metadata relating to the list.
+
+        Parameters:
+        - `project` -- the project or user to which this metadata relates
+        - `key`     -- the key under which the metadata should be scored
+        - `value`   -- the value of the metadata to store
+
+        The `project` is intended to allow different users to store metadata
+        in a shared mail archive database. For example, a group project that
+        works with the mail archive might tag message envelopes with agreed-
+        upon metadata using the project's name in the `project` field, while
+        exploratory work from individual members of the project might use
+        their username as the basis for the `project` (e.g., "alice_test4").
+        """
+        entry = {"list"    : self._list_name,
+                 "project" : project,
+                 "key"     : key,
+                 "value"   : value,
+        }
+        self._mail_archive._db.lists_metadata.insert_one(entry)
+
+
+    def get_metadata(self, project:str, key:str):
+        """
+        Get metadata relating to the list.
+
+        Parameters:
+        - `project` -- the project or user to which this metadata relates
+        - `key`     -- the key under which the metadata was scored
+        """
+        query = {"list"    : self._list_name,
+                 "project" : project,
+                 "key"     : key}
+        result = self._mail_archive._db.lists_metadata.find_one(query) # type: Optional[Dict[str, Any]]
+        if result is not None:
+            return result["value"]
+        else:
+            return None
 
-# =================================================================================================
 
-# Private helper for MailArchive::update()
-def _update_list(ml: MailingList) -> None:
-    ml.update()
+    def clear_metadata(self, project:str, key:Optional[str] = None):
+        """
+        Remove metadata relating to the list.
+
+        Parameters:
+        - `project` -- the project or user to which this metadata relates
+        - `key`     -- the key under which the metadata was scored
+
+        If the `key` is specified then only the single metadata value
+        identified by the `project` and `key` is removed. If the `key`
+        is not specified, then all metadata relating to `project` is
+        removed from this envelope.
+        """
+        query = {"list"    : self._list_name,
+                 "project" : project}
+        if key is not None:
+            query["key"] = key
+        self._mail_archive._db.lists_metadata.delete_many(query)
 
+# =================================================================================================
 
 class MailArchive:
+    """
+    A class representing the IETF email archive.
+    """
+
+    _log           : logging.Logger
+    _imap_server   : str
     _mongoclient   : MongoClient
     _db            : Database
     _fs            : GridFS
-    _log           : logging.Logger
     _mailing_lists : Dict[str, MailingList]
 
-
     def __init__(self,
-            mongodb_hostname : str = "localhost",
-            mongodb_port     : int = 27017,
-            mongodb_username : Optional[str] = None,
-            mongodb_password : Optional[str] = None):
-        # Enable logging
+                 imap_server      : str = "imap.ietf.org",
+                 mongodb_hostname : str = "localhost",
+                 mongodb_port     : str = "27017",
+                 mongodb_username : Optional[str] = None,
+                 mongodb_password : Optional[str] = None):
+        """
+        Initialise the MailArchive.
+        """
         logging.basicConfig(level=os.environ.get("IETFDATA_LOGLEVEL", "INFO"))
-        self._log           = logging.getLogger("ietfdata")
+        self._log         = logging.getLogger("ietfdata")
+        self._imap_server = imap_server
         # Connect to MongoDB:
         cache_host     = os.environ.get('IETFDATA_CACHE_HOST',     mongodb_hostname)
         cache_port     = os.environ.get('IETFDATA_CACHE_PORT',     mongodb_port)
         cache_username = os.environ.get('IETFDATA_CACHE_USER',     mongodb_username)
         cache_password = os.environ.get('IETFDATA_CACHE_PASSWORD', mongodb_password)
         if cache_username is not None:
             self._mongoclient = MongoClient(host=cache_host, port=int(cache_port), username=cache_username, password=cache_password)
         else:
             self._mongoclient = MongoClient(host=cache_host, port=int(cache_port))
         self._db = self._mongoclient.ietfdata_mailarchive_v2
-        self._db.messages.create_index([('list', ASCENDING), ('uidvalidity', ASCENDING), (       'uid', ASCENDING)], unique=True)
-        self._db.messages.create_index([('list', ASCENDING), ('uidvalidity', ASCENDING), ( 'timestamp', ASCENDING)], unique=False)
-        self._db.messages.create_index([('list', ASCENDING), ('uidvalidity', ASCENDING), ('message_id', ASCENDING)], unique=False)
-        self._db.messages.create_index([('message_id', ASCENDING)], unique=False)
-        self._db.lists.create_index([('list', ASCENDING)], unique=True)
+        self._db.lists.create_index([('list', ASCENDING),
+                                    ], unique=True)
+        self._db.lists_metadata.create_index([('list', ASCENDING),
+                                              ('project', ASCENDING),
+                                              ('key', ASCENDING),
+                                             ], unique=True)
+
+        self._db.messages.create_index([('list', ASCENDING),
+                                        ('uidvalidity', ASCENDING),
+                                        ('uid', ASCENDING),
+                                       ], unique=True)
+        self._db.messages.create_index([('list', ASCENDING),
+                                        ('uidvalidity', ASCENDING),
+                                        ('message_id', ASCENDING),
+                                       ], unique=False)
+        self._db.messages.create_index([('message_id', ASCENDING),
+                                       ], unique=False)
+
+        self._db.metadata.create_index([('list', ASCENDING), 
+                                        ('uidvalidity', ASCENDING), 
+                                        ('uid', ASCENDING),
+                                        ('project', ASCENDING),
+                                        ('key', ASCENDING),
+                                       ], unique=False)
+        self._db.metadata.create_index([('message_id', ASCENDING)
+                                       ], unique=False)
         self._fs = GridFS(self._db)
         # Create other state:
         self._mailing_lists = {}
 
 
     def mailing_list_names(self) -> Iterator[str]:
-        imap = IMAPClient(host='imap.ietf.org', ssl=True, use_uid=True)
+        """
+        Yield the names of the mailing lists that exist in the mail archive.
+        """
+        imap = IMAPClient(host=self._imap_server, ssl=True, use_uid=True)
         imap.login("anonymous", "anonymous")
         folders = imap.list_folders()
         imap.logout()
         for (flags, delimiter, name) in folders:
             if b'\Noselect' not in flags:
                 yield name.split(delimiter.decode("utf-8"))[-1]
 
 
     def mailing_list(self, mailing_list_name: str) -> MailingList:
+        """
+        Return an object representing the given mailing list.
+        """
         if not mailing_list_name in self._mailing_lists:
             self._mailing_lists[mailing_list_name] = MailingList(self, mailing_list_name)
         return self._mailing_lists[mailing_list_name]
 
 
+    def message(self, message_id:str) -> List[Envelope]:
+        """
+        Return the envelopes for all messages with the specified `message_id`.
+
+        There can be multiple copies of a message with a particular ID in the
+        archive if it was sent to multiple lists. This method returns all the
+        copies, since each copy might have a different set of replies.  For
+        example, message "<396c8d37-f979-73fe-34fa-475a038b94f8@alum.mit.edu>"
+        appears in the archives of the "art", "last-call", and "tsvwg" lists.
+        """
+        messages = []
+        for message in self._db.messages.find({"message_id": message_id}):
+            mailing_list  = self.mailing_list(message["list"])
+            uidvalidity   = message["uidvalidity"]
+            uid           = message["uid"]
+            gridfs_id     = message["gridfs_id"]
+            date_received = message["timestamp"]
+            size          = message["size"]
+            headers       = message["headers"]
+            messages.append(Envelope(mailing_list, uidvalidity, uid, gridfs_id, date_received, size, headers))
+        return messages
+
+
+    # FIXME: add `addr_from`, `addr_to`, `addr_cc`, `sent_after`, `sent_before`
+    # parameters, operating on the parsed_headers database collection
     def messages(self,
-                 since : str = "1970-01-01T00:00:00",
-                 until : str = "2038-01-19T03:14:07") -> Iterator[Message]:
-        for ml_name in self.mailing_list_names():
-            ml = self.mailing_list(ml_name)
-            yield from ml.messages(since, until)
+                 received_after    : str = "1970-01-01T00:00:00",
+                 received_before   : str = "2038-01-19T03:14:07",
+                 header_from       : Optional[str] = None,
+                 header_to         : Optional[str] = None,
+                 header_subject    : Optional[str] = None,
+                 mailing_list_name : Optional[str] = None,
+                ) -> Iterator[Envelope]:
+        """
+        Return the envelopes of all specified messages in the archive.
+        """
+        query = {"timestamp"   : {
+                     "$gt": datetime.strptime(received_after,  "%Y-%m-%dT%H:%M:%S"),
+                     "$lt": datetime.strptime(received_before, "%Y-%m-%dT%H:%M:%S")
+                 }
+                } # type: Dict[str, Union[str, Dict[str, Any]]]
+        if header_from is not None:
+            query["headers.from"] = { "$regex": f"{header_from}"}
+        if header_to is not None:
+            query["headers.to"] = { "$regex": f"{header_to}"}
+        if header_subject is not None:
+            query["headers.subject"] = { "$regex": f"{header_subject}"}
+        if mailing_list_name is not None:
+            query["list"] = mailing_list_name
+        messages = self._db.messages.find(query, no_cursor_timeout=True)
+        for message in messages:
+            mailing_list = self.mailing_list(message["list"])
+            uidvalidity  = message["uidvalidity"]
+            uid          = message["uid"]
+            gridfs_id    = message["gridfs_id"]
+            timestamp    = message["timestamp"]
+            size         = message["size"]
+            headers      = message["headers"]
+            yield Envelope(mailing_list, uidvalidity, uid, gridfs_id, timestamp, size, headers)
+        messages.close()
 
 
-    def update(self) -> None:
-        # WARNING: The first time this method is called, it will download the
-        # entire mail archive. This will take several hours and download tens
-        # of gigabytes of data. Subsequent calls will just fetch new data, so
-        # will be much faster. Set the environment variable IETFDATA_LOGLEVEL
-        # to INFO before running this to be informed of progress.
+    def update(self, verbose = True) -> None:
+        """
+        Update the local cache of the messages from all the mailing lists.
+
+        This method should be called when working with a complete copy of
+        the mail archive to synchronise the local copy with the IETF IMAP
+        server.
+
+        To only download a subset of the messages, use the `mailing_list()`
+        method to get a MailingList object for the lists of interest, then
+        call the `update()` method on those objects.
+
+        WARNING: The first time this method is called, it will download the
+        entire mail archive. This will take several hours and download tens
+        of gigabytes of data. Subsequent calls will just fetch new data and
+        so will be much faster.
+        """
         with concurrent.futures.ThreadPoolExecutor(max_workers = 8) as executor:
             for ml_name in self.mailing_list_names():
                 ml = self.mailing_list(ml_name)
-                executor.submit(_update_list, ml)
+                executor.submit(lambda mailing_list : mailing_list.update(verbose), ml)
+
+
+    def clear_metadata(self, project: str):
+        """
+        Remove metadata relating to the project from all mailing lists
+        and message envelopes.
+
+        WARNING: This is a destructive operation that should not normally
+        be needed. Use with care.
+        """
+        self._db.lists_metadata.delete_many({"project": project})
+        self._db.metadata.delete_many({"project": project})
 
 
 # =================================================================================================
 # vim: set tw=0 ai:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ietfdata-0.6.8/ietfdata/rfcindex.py` & `ietfdata-0.7.0/ietfdata/rfcindex.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,22 +258,29 @@
              (self.doc_id == "RFC0317") or (self.doc_id == "RFC0323") or \
              (self.doc_id == "RFC0327") or (self.doc_id == "RFC0367") or \
              (self.doc_id == "RFC0369") or (self.doc_id == "RFC0441") or \
              (self.doc_id == "RFC1305"):
             return "iso8859_1"
         elif self.doc_id == "RFC2166":
             return "windows-1252"
-        elif (self.doc_id == "RFC2497") or (self.doc_id == "RFC2497") or \
-             (self.doc_id == "RFC2557"):
+        elif (self.doc_id == "RFC2497") or (self.doc_id == "RFC2557"):
             return "iso8859_1"
         elif self.doc_id == "RFC2708":
             # This RFC is corrupt: line 521 has a byte with value 0xC6 that
             # is clearly intended to be a ' character, but that code point
             # doesn't correspond to ' in any character set I can find. Use
             # ISO 8859-1 which gets all characters right apart from this.
+            #
+            # According to Greg Skinner: "regarding the test in line 268
+            # for RFC2708, as far as I can tell, U+0092 was introduced in
+            # draft-ietf-printmib-job-protomap-01 in multiple places. In -02,
+            # it was replaced with U+0027 everywhere except section 5.0.
+            # Somehow, that stray character became the corrupt text you
+            # identified."
+            # (https://github.com/glasgow-ipl/ietfdata/issues/137)
             return "iso8859_1"
         elif self.doc_id == "RFC2875":
             # Both the text and PDF versions of this document have corrupt
             # characters (lines 754 and 926 of the text version). Using 
             # ISO 8859-1 is no more corrupt than the original.
             return "iso8859_1"
         else:
```

### Comparing `ietfdata-0.6.8/ietfdata.egg-info/SOURCES.txt` & `ietfdata-0.7.0/ietfdata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 examples/draft-references.py
 examples/draft-submissions-by-date.py
 examples/draft-submissions.py
 examples/drafts-for-person.py
 examples/drafts-for-rfc.py
 examples/drafts-for-wg.py
 examples/emails-per-person.py
+examples/iesg-processing-time.py
 examples/ietf-leadership.py
 examples/non-wg-standards-track-rfcs.py
 examples/org-chart.py
 examples/person-attendance.py
 examples/person-emails.py
 examples/person.py
 examples/recent-pubreq.py
 examples/rfc-data.py
+examples/rfc-per-year.py
 examples/rfc-streams.py
 examples/role-names.py
 ietfdata/__init__.py
 ietfdata/datatracker.py
 ietfdata/datatracker_ext.py
-ietfdata/mailarchive.py
 ietfdata/mailarchive2.py
 ietfdata/py.typed
 ietfdata/rfcindex.py
 ietfdata.egg-info/PKG-INFO
 ietfdata.egg-info/SOURCES.txt
 ietfdata.egg-info/dependency_links.txt
 ietfdata.egg-info/requires.txt
 ietfdata.egg-info/top_level.txt
 tests/test_datatracker.py
 tests/test_datatracker_coverage.py
-tests/test_mailarchive.py
+tests/test_mailarchive2.py
 tests/test_rfcindex.py
```

### Comparing `ietfdata-0.6.8/setup.py` & `ietfdata-0.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ietfdata",
-    version="0.6.8",
+    version="0.7.0",
     author="Colin Perkins",
     author_email="csp@csperkins.org",
     description="Access the IETF Data Tracker and RFC Index",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/glasgow-ipl/ietfdata",
     packages=setuptools.find_packages(),
@@ -17,11 +17,12 @@
         'ietfdata': ['py.typed'],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.11',
     setup_requires=["setuptools-pipfile"],
+    tests_require=[],
     use_pipfile=True
 )
```

### Comparing `ietfdata-0.6.8/tests/test_datatracker.py` & `ietfdata-0.7.0/tests/test_datatracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import unittest
 import os
 import sys
 
+from datetime      import date, datetime, timedelta, timezone
 from pathlib       import Path
 from unittest.mock import patch, Mock
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 import ietfdata
 from ietfdata.datatracker import *
@@ -40,79 +41,79 @@
 # Unit tests:
 
 class TestDatatracker(unittest.TestCase):
     dt : DataTracker
 
     @classmethod
     def setUpClass(self) -> None:
-        self.dt = DataTracker()
+        self.dt = DataTracker(cache_timeout = timedelta(minutes = 15))
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to the datatracker access layer:
 
     def test__datatracker_get_single(self) -> None:
-        json = self.dt._datatracker_get_single(URI("/api/v1/person/email/csp@csperkins.org/"))
+        json = self.dt._datatracker_get_single(URI(uri="/api/v1/person/email/csp@csperkins.org/"))
         if json is not None:
             self.assertEqual(json["resource_uri"], "/api/v1/person/email/csp@csperkins.org/")
             self.assertEqual(json["address"],      "csp@csperkins.org")
             self.assertEqual(json["person"],       "/api/v1/person/person/20209/")
             self.assertEqual(json["time"],         "1970-01-02T07:59:59Z")
             self.assertEqual(json["primary"],      True)
             self.assertEqual(json["active"],       True)
         else:
             self.fail("Cannot retrieve single JSON item")
 
 
     def test__datatracker_get_multi_small(self) -> None:
-        url = URI("/api/v1/doc/document/")
+        url = URI(uri="/api/v1/doc/document/")
         url.params["group"] = 1963
         url.params["type"]  = "draft"
         json = list(self.dt._datatracker_get_multi(url, "id"))
         self.assertEqual(len(json), 2)
         self.assertEqual(json[0][  "id"], 63980)
         self.assertEqual(json[0]["name"], "draft-ietf-netvc-requirements")
         self.assertEqual(json[1][  "id"], 64020)
         self.assertEqual(json[1]["name"], "draft-ietf-netvc-testing")
 
 
     def test__datatracker_get_multi_large(self) -> None:
-        url = URI("/api/v1/meeting/meeting/")
+        url = URI(uri="/api/v1/meeting/meeting/")
         url.params["type"]  = "ietf"
         json = list(self.dt._datatracker_get_multi(url, "id"))
         self.assertGreaterEqual(len(json), 111)
 
 
     def test__datatracker_get_multi_count(self) -> None:
-        count = self.dt._datatracker_get_multi_count(URI("/api/v1/name/stdlevelname/"))
+        count = self.dt._datatracker_get_multi_count(URI(uri="/api/v1/name/stdlevelname/"))
         self.assertEqual(count, 8)
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to email addresses:
 
     def test_email(self) -> None:
-        e  = self.dt.email(EmailURI("/api/v1/person/email/csp@csperkins.org/"))
+        e  = self.dt.email(EmailURI(uri="/api/v1/person/email/csp@csperkins.org/"))
         if e is not None:
-            self.assertEqual(e.resource_uri, EmailURI("/api/v1/person/email/csp@csperkins.org/"))
+            self.assertEqual(e.resource_uri, EmailURI(uri="/api/v1/person/email/csp@csperkins.org/"))
             self.assertEqual(e.address,      "csp@csperkins.org")
-            self.assertEqual(e.person,       PersonURI("/api/v1/person/person/20209/"))
+            self.assertEqual(e.person,       PersonURI(uri="/api/v1/person/person/20209/"))
             self.assertEqual(e.time,         datetime.fromisoformat("1970-01-01T23:59:59-08:00"))
             # self.assertEqual(e.origin,     "author: draft-ietf-mmusic-rfc4566bis")
             self.assertEqual(e.primary,      True)
             self.assertEqual(e.active,       True)
         else:
             self.fail("Cannot find email address")
 
 
     def test_email_for_address(self) -> None:
         e  = self.dt.email_for_address("csp@csperkins.org")
         if e is not None:
-            self.assertEqual(e.resource_uri, EmailURI("/api/v1/person/email/csp@csperkins.org/"))
+            self.assertEqual(e.resource_uri, EmailURI(uri="/api/v1/person/email/csp@csperkins.org/"))
             self.assertEqual(e.address,      "csp@csperkins.org")
-            self.assertEqual(e.person,       PersonURI("/api/v1/person/person/20209/"))
+            self.assertEqual(e.person,       PersonURI(uri="/api/v1/person/person/20209/"))
             self.assertEqual(e.time,         datetime.fromisoformat("1970-01-01T23:59:59-08:00"))
             # self.assertEqual(e.origin,     "author: draft-ietf-mmusic-rfc4566bis")
             self.assertEqual(e.primary,      True)
             self.assertEqual(e.active,       True)
         else:
             self.fail("Cannot find email address")
 
@@ -137,76 +138,76 @@
         
         self.assertEqual(h[0].history_id, 167444)
         self.assertEqual(h[0].history_type, "~")
         self.assertEqual(h[0].history_change_reason, None)
         self.assertEqual(h[0].origin, "author: draft-ietf-avt-rtptest")
         self.assertEqual(h[0].address, "csp@isi.edu")
         self.assertEqual(h[0].active, False)
-        self.assertEqual(h[0].person, PersonURI("/api/v1/person/person/20209/"))
+        self.assertEqual(h[0].person, PersonURI(uri="/api/v1/person/person/20209/"))
         self.assertEqual(h[0].time, datetime.fromisoformat("2012-02-26T00:46:44-08:00"))
-        self.assertEqual(h[0].resource_uri, HistoricalEmailURI("/api/v1/person/historicalemail/167444/"))
+        self.assertEqual(h[0].resource_uri, HistoricalEmailURI(uri="/api/v1/person/historicalemail/167444/"))
         self.assertEqual(h[0].primary, False)
         self.assertEqual(h[0].history_date, datetime.fromisoformat("2022-06-27T12:36:15-07:00"))
         self.assertEqual(h[0].history_user, "")
         
         self.assertEqual(h[1].history_id, 161025)
         self.assertEqual(h[1].history_type, "~")
         self.assertEqual(h[1].history_change_reason, None)
         self.assertEqual(h[1].origin, "author: draft-ietf-avt-rtptest")
         self.assertEqual(h[1].address, "csp@isi.edu")
         self.assertEqual(h[1].active, False)
-        self.assertEqual(h[1].person, PersonURI("/api/v1/person/person/20209/"))
+        self.assertEqual(h[1].person, PersonURI(uri="/api/v1/person/person/20209/"))
         self.assertEqual(h[1].time, datetime.fromisoformat("2012-02-26T00:46:44-08:00"))
-        self.assertEqual(h[1].resource_uri, HistoricalEmailURI("/api/v1/person/historicalemail/161025/"))
+        self.assertEqual(h[1].resource_uri, HistoricalEmailURI(uri="/api/v1/person/historicalemail/161025/"))
         self.assertEqual(h[1].primary, False)
         self.assertEqual(h[1].history_date, datetime.fromisoformat("2022-04-19T14:40:37-07:00"))
         self.assertEqual(h[1].history_user, "")
         
         self.assertEqual(h[2].history_id, 128355)
         self.assertEqual(h[2].history_type, "~")
         self.assertEqual(h[2].history_change_reason, None)
         self.assertEqual(h[2].origin, "author: draft-ietf-avt-rtptest")
         self.assertEqual(h[2].address, "csp@isi.edu")
         self.assertEqual(h[2].active, False)
-        self.assertEqual(h[2].person, PersonURI("/api/v1/person/person/20209/"))
+        self.assertEqual(h[2].person, PersonURI(uri="/api/v1/person/person/20209/"))
         self.assertEqual(h[2].time, datetime.fromisoformat("2012-02-26T00:46:44-08:00"))
-        self.assertEqual(h[2].resource_uri, HistoricalEmailURI("/api/v1/person/historicalemail/128355/"))
+        self.assertEqual(h[2].resource_uri, HistoricalEmailURI(uri="/api/v1/person/historicalemail/128355/"))
         self.assertEqual(h[2].primary, False)
         self.assertEqual(h[2].history_date, datetime.fromisoformat("2021-05-18T16:32:20-07:00"))
         self.assertEqual(h[2].history_user, "")
         
         self.assertEqual(h[3].history_id, 128350)
         self.assertEqual(h[3].history_change_reason, None)
         self.assertEqual(h[3].history_type, "~")
         self.assertEqual(h[3].origin, "author: draft-ietf-avt-rtptest")
         self.assertEqual(h[3].address, "csp@isi.edu")
         self.assertEqual(h[3].active, False)
-        self.assertEqual(h[3].person, PersonURI("/api/v1/person/person/20209/"))
+        self.assertEqual(h[3].person, PersonURI(uri="/api/v1/person/person/20209/"))
         self.assertEqual(h[3].time, datetime.fromisoformat("2012-02-26T00:46:44-08:00"))
-        self.assertEqual(h[3].resource_uri, HistoricalEmailURI("/api/v1/person/historicalemail/128350/"))
+        self.assertEqual(h[3].resource_uri, HistoricalEmailURI(uri="/api/v1/person/historicalemail/128350/"))
         self.assertEqual(h[3].primary, False)
         self.assertEqual(h[3].history_user, "")
         self.assertEqual(h[3].history_date, datetime.fromisoformat("2021-05-18T16:30:53-07:00"))
         
-        self.assertEqual(h[4].resource_uri, HistoricalEmailURI("/api/v1/person/historicalemail/71987/"))
+        self.assertEqual(h[4].resource_uri, HistoricalEmailURI(uri="/api/v1/person/historicalemail/71987/"))
         self.assertEqual(h[4].address,      "csp@isi.edu")
-        self.assertEqual(h[4].person,       PersonURI("/api/v1/person/person/20209/"))
+        self.assertEqual(h[4].person,       PersonURI(uri="/api/v1/person/person/20209/"))
         self.assertEqual(h[4].origin,       "author: draft-ietf-avt-rtptest")
         self.assertEqual(h[4].time,         datetime.fromisoformat("2012-02-26T00:46:44-08:00"))
         self.assertEqual(h[4].active,       False)
         self.assertEqual(h[4].primary,      False)
         self.assertEqual(h[4].history_id,   71987)
         self.assertEqual(h[4].history_date, datetime.fromisoformat("2019-09-29T14:39:48-07:00"))
         self.assertEqual(h[4].history_type, "~")
         self.assertEqual(h[4].history_user, "")
         self.assertEqual(h[4].history_change_reason, None)
         
-        self.assertEqual(h[5].resource_uri, HistoricalEmailURI("/api/v1/person/historicalemail/2090/"))
+        self.assertEqual(h[5].resource_uri, HistoricalEmailURI(uri="/api/v1/person/historicalemail/2090/"))
         self.assertEqual(h[5].address,      "csp@isi.edu")
-        self.assertEqual(h[5].person,       PersonURI("/api/v1/person/person/20209/"))
+        self.assertEqual(h[5].person,       PersonURI(uri="/api/v1/person/person/20209/"))
         self.assertEqual(h[5].origin,       "author: draft-ietf-avt-rtptest")
         self.assertEqual(h[5].time,         datetime.fromisoformat("2012-02-26T00:46:44-08:00"))
         self.assertEqual(h[5].active,       False)
         self.assertEqual(h[5].primary,      False)
         self.assertEqual(h[5].history_id,   2090)
         self.assertEqual(h[5].history_date, datetime.fromisoformat("2018-06-19T15:39:40-07:00"))
         self.assertEqual(h[5].history_type, "~")
@@ -226,43 +227,43 @@
         else:
             self.fail("Cannot find person")
 
 
     def test_emails(self) -> None:
         e = list(self.dt.emails(addr_contains="csperkins.org"))
         self.assertEqual(len(e), 1)
-        self.assertEqual(e[0].resource_uri, EmailURI('/api/v1/person/email/csp@csperkins.org/'))
+        self.assertEqual(e[0].resource_uri, EmailURI(uri="/api/v1/person/email/csp@csperkins.org/"))
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to people:
 
     def test_person_from_email(self) -> None:
         p  = self.dt.person_from_email("csp@csperkins.org")
         if p is not None:
             self.assertEqual(p.id,              20209)
-            self.assertEqual(p.resource_uri,    PersonURI("/api/v1/person/person/20209/"))
+            self.assertEqual(p.resource_uri,    PersonURI(uri="/api/v1/person/person/20209/"))
             self.assertEqual(p.name,            "Colin Perkins")
             self.assertEqual(p.name_from_draft, "Colin Perkins")
             self.assertEqual(p.ascii,           "Colin Perkins")
             self.assertEqual(p.ascii_short,     "")
             self.assertEqual(p.plain,           "")
             self.assertEqual(p.user,            "")
             self.assertEqual(p.time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
             self.assertEqual(p.photo,           "https://www.ietf.org/lib/dt/media/photo/csp-square.jpg")
             self.assertEqual(p.photo_thumb,     "https://www.ietf.org/lib/dt/media/photo/csp-square_GDMMZmn.jpg")
             # self.assertEqual(p.biography,     "Colin Perkins is a ...")
         else:
             self.fail("Cannot find person")
 
     def test_person(self) -> None:
-        p  = self.dt.person(PersonURI("/api/v1/person/person/20209/"))
+        p  = self.dt.person(PersonURI(uri="/api/v1/person/person/20209/"))
         if p is not None:
             self.assertEqual(p.id,              20209)
-            self.assertEqual(p.resource_uri,    PersonURI("/api/v1/person/person/20209/"))
+            self.assertEqual(p.resource_uri,    PersonURI(uri="/api/v1/person/person/20209/"))
             self.assertEqual(p.name,            "Colin Perkins")
             self.assertEqual(p.name_from_draft, "Colin Perkins")
             self.assertEqual(p.ascii,           "Colin Perkins")
             self.assertEqual(p.ascii_short,     "")
             self.assertEqual(p.plain,           "")
             self.assertEqual(p.user,            "")
             self.assertEqual(p.time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -270,21 +271,21 @@
             self.assertEqual(p.photo_thumb,     "https://www.ietf.org/lib/dt/media/photo/csp-square_GDMMZmn.jpg")
             # self.assertEqual(p.biography,     "Colin Perkins is a ...")
         else:
             self.fail("Cannot find person")
 
 
     def test_person_history(self) -> None:
-        p  = self.dt.person(PersonURI("/api/v1/person/person/20209/"))
+        p  = self.dt.person(PersonURI(uri="/api/v1/person/person/20209/"))
         if p is not None:
             h  = list(self.dt.person_history(p))
             self.assertEqual(len(h), 8)
             
             self.assertEqual(h[0].id,              20209)
-            self.assertEqual(h[0].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/27668/"))
+            self.assertEqual(h[0].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/27668/"))
             self.assertEqual(h[0].name,            "Colin Perkins")
             self.assertEqual(h[0].name_from_draft, "Colin Perkins")
             self.assertEqual(h[0].ascii,           "Colin Perkins")
             self.assertEqual(h[0].ascii_short,     "")
             self.assertEqual(h[0].plain,           "")
             self.assertEqual(h[0].user,            "")
             self.assertEqual(h[0].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -294,15 +295,15 @@
             self.assertEqual(h[0].history_change_reason, None)
             self.assertEqual(h[0].history_user,    "")
             self.assertEqual(h[0].history_id,      27668)
             self.assertEqual(h[0].history_type,    "~")
             self.assertEqual(h[0].history_date,    datetime.fromisoformat("2022-06-27T12:36:15-07:00"))
             
             self.assertEqual(h[1].id,              20209)
-            self.assertEqual(h[1].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/24980/"))
+            self.assertEqual(h[1].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/24980/"))
             self.assertEqual(h[1].name,            "Colin Perkins")
             self.assertEqual(h[1].name_from_draft, "Colin Perkins")
             self.assertEqual(h[1].ascii,           "Colin Perkins")
             self.assertEqual(h[1].ascii_short,     None)
             self.assertEqual(h[1].plain,           "")
             self.assertEqual(h[1].user,            "")
             self.assertEqual(h[1].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -311,15 +312,15 @@
             self.assertEqual(h[1].history_change_reason, None)
             self.assertEqual(h[1].history_user,    "")
             self.assertEqual(h[1].history_id,      24980)
             self.assertEqual(h[1].history_type,    "~")
             self.assertEqual(h[1].history_date,    datetime.fromisoformat("2022-04-19T14:47:28-07:00"))
             
             self.assertEqual(h[2].id,              20209)
-            self.assertEqual(h[2].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/24978/"))
+            self.assertEqual(h[2].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/24978/"))
             self.assertEqual(h[2].name,            "Colin Perkins")
             self.assertEqual(h[2].name_from_draft, "Colin Perkins")
             self.assertEqual(h[2].ascii,           "Colin Perkins")
             self.assertEqual(h[2].ascii_short,     "")
             self.assertEqual(h[2].plain,           "")
             self.assertEqual(h[2].user,            "")
             self.assertEqual(h[2].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -328,15 +329,15 @@
             self.assertEqual(h[2].history_change_reason, None)
             self.assertEqual(h[2].history_user,    "")
             self.assertEqual(h[2].history_id,      24978)
             self.assertEqual(h[2].history_type,    "~")
             self.assertEqual(h[2].history_date,    datetime.fromisoformat("2022-04-19T14:40:37-07:00"))
             
             self.assertEqual(h[3].id,              20209)
-            self.assertEqual(h[3].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/17735/"))
+            self.assertEqual(h[3].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/17735/"))
             self.assertEqual(h[3].name,            "Colin Perkins")
             self.assertEqual(h[3].name_from_draft, "Colin Perkins")
             self.assertEqual(h[3].ascii,           "Colin Perkins")
             self.assertEqual(h[3].ascii_short,     "")
             self.assertEqual(h[3].plain,           "")
             self.assertEqual(h[3].user,            "")
             self.assertEqual(h[3].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -345,15 +346,15 @@
             self.assertEqual(h[3].history_change_reason, None)
             self.assertEqual(h[3].history_user,    "")
             self.assertEqual(h[3].history_id,      17735)
             self.assertEqual(h[3].history_type,    "~")
             self.assertEqual(h[3].history_date,    datetime.fromisoformat("2021-05-18T16:32:20-07:00"))
             
             self.assertEqual(h[4].id,              20209)
-            self.assertEqual(h[4].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/17734/"))
+            self.assertEqual(h[4].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/17734/"))
             self.assertEqual(h[4].name,            "Colin Perkins")
             self.assertEqual(h[4].name_from_draft, "Colin Perkins")
             self.assertEqual(h[4].ascii,           "Colin Perkins")
             self.assertEqual(h[4].ascii_short,     "")
             self.assertEqual(h[4].plain,           "")
             self.assertEqual(h[4].user,            "")
             self.assertEqual(h[4].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -362,15 +363,15 @@
             self.assertEqual(h[4].history_change_reason, None)
             self.assertEqual(h[4].history_user,    "")
             self.assertEqual(h[4].history_id,      17734)
             self.assertEqual(h[4].history_type,    "~")
             self.assertEqual(h[4].history_date,    datetime.fromisoformat("2021-05-18T16:30:53-07:00"))
             
             self.assertEqual(h[5].id,              20209)
-            self.assertEqual(h[5].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/11731/"))
+            self.assertEqual(h[5].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/11731/"))
             self.assertEqual(h[5].name,            "Colin Perkins")
             self.assertEqual(h[5].name_from_draft, "Colin Perkins")
             self.assertEqual(h[5].ascii,           "Colin Perkins")
             self.assertEqual(h[5].ascii_short,     "")
             self.assertEqual(h[5].plain,           "")
             self.assertEqual(h[5].user,            "")
             self.assertEqual(h[5].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -379,15 +380,15 @@
             self.assertEqual(h[5].history_change_reason, None)
             self.assertEqual(h[5].history_user,    "")
             self.assertEqual(h[5].history_id,      11731)
             self.assertEqual(h[5].history_type,    "~")
             self.assertEqual(h[5].history_date,    datetime.fromisoformat("2019-09-29T14:39:48-07:00"))
             
             self.assertEqual(h[6].id,              20209)
-            self.assertEqual(h[6].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/10878/"))
+            self.assertEqual(h[6].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/10878/"))
             self.assertEqual(h[6].name,            "Colin Perkins")
             self.assertEqual(h[6].name_from_draft, "Colin Perkins")
             self.assertEqual(h[6].ascii,           "Colin Perkins")
             self.assertEqual(h[6].ascii_short,     None)
             self.assertEqual(h[6].plain,           "")
             self.assertEqual(h[6].user,            "")
             self.assertEqual(h[6].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -396,15 +397,15 @@
             self.assertEqual(h[6].history_change_reason, None)
             self.assertEqual(h[6].history_user,    "")
             self.assertEqual(h[6].history_id,      10878)
             self.assertEqual(h[6].history_type,    "~")
             self.assertEqual(h[6].history_date,    datetime.fromisoformat("2019-03-29T02:44:28-07:00"))
             
             self.assertEqual(h[7].id,              20209)
-            self.assertEqual(h[7].resource_uri,    HistoricalPersonURI("/api/v1/person/historicalperson/127/"))
+            self.assertEqual(h[7].resource_uri,    HistoricalPersonURI(uri="/api/v1/person/historicalperson/127/"))
             self.assertEqual(h[7].name,            "Colin Perkins")
             self.assertEqual(h[7].name_from_draft, "Colin Perkins")
             self.assertEqual(h[7].ascii,           "Colin Perkins")
             self.assertEqual(h[7].ascii_short,     "")
             self.assertEqual(h[7].plain,           "")
             self.assertEqual(h[7].user,            "")
             self.assertEqual(h[7].time,            datetime.fromisoformat("2012-02-26T00:03:54-08:00"))
@@ -418,106 +419,141 @@
             self.assertEqual(h[7].history_date,    datetime.fromisoformat("2018-06-19T15:39:39-07:00"))
 
         else:
             self.fail("Cannot find person")
 
 
     def test_person_aliases(self) -> None:
-        p  = self.dt.person(PersonURI("/api/v1/person/person/20209/"))
+        p  = self.dt.person(PersonURI(uri="/api/v1/person/person/20209/"))
         if p is not None:
             aliases  = list(self.dt.person_aliases(person = p))
             self.assertEqual(len(aliases), 2)
             self.assertEqual(aliases[0].id,           62)
-            self.assertEqual(aliases[0].resource_uri, PersonAliasURI("/api/v1/person/alias/62/"))
-            self.assertEqual(aliases[0].person,       PersonURI("/api/v1/person/person/20209/"))
+            self.assertEqual(aliases[0].resource_uri, PersonAliasURI(uri="/api/v1/person/alias/62/"))
+            self.assertEqual(aliases[0].person,       PersonURI(uri="/api/v1/person/person/20209/"))
             self.assertEqual(aliases[0].name,         "Dr. Colin Perkins")
             self.assertEqual(aliases[1].id,           22620)
-            self.assertEqual(aliases[1].resource_uri, PersonAliasURI("/api/v1/person/alias/22620/"))
-            self.assertEqual(aliases[1].person,       PersonURI("/api/v1/person/person/20209/"))
+            self.assertEqual(aliases[1].resource_uri, PersonAliasURI(uri="/api/v1/person/alias/22620/"))
+            self.assertEqual(aliases[1].person,       PersonURI(uri="/api/v1/person/person/20209/"))
             self.assertEqual(aliases[1].name,         "Colin Perkins")
         else:
             self.fail("Cannot find person")
 
 
     #def test_person_events(self) -> None:
-    #    p = self.dt.person(PersonURI("/api/v1/person/person/3/"))
+    #    p = self.dt.person(PersonURI(uri="/api/v1/person/person/3/"))
     #    if p is not None:
     #        events = list(self.dt.person_events(p))
     #        self.assertEqual(len(events), 1)
     #        self.assertEqual(events[0].desc,         "Sent GDPR notice email to [u'vint@google.com', u'vcerf@mci.net', u'vcerf@nri.reston.va.us', u'vinton.g.cerf@wcom.com'] with confirmation deadline 2018-10-22")
     #        self.assertEqual(events[0].id,           478)
-    #        self.assertEqual(events[0].person,       PersonURI("/api/v1/person/person/3/"))
-    #        self.assertEqual(events[0].resource_uri, PersonEventURI("/api/v1/person/personevent/478/"))
+    #        self.assertEqual(events[0].person,       PersonURI(uri="/api/v1/person/person/3/"))
+    #        self.assertEqual(events[0].resource_uri, PersonEventURI(uri="/api/v1/person/personevent/478/"))
     #        self.assertEqual(events[0].time,         datetime.fromisoformat("2018-09-24T09:28:32.502465"))
     #        self.assertEqual(events[0].type,         "gdpr_notice_email")
     #    else:
     #        self.fail("Cannot find person")
 
 
     def test_people(self) -> None:
         p  = list(self.dt.people(name_contains="Colin Perkins"))
         self.assertEqual(len(p), 1)
-        self.assertEqual(p[ 0].resource_uri, PersonURI("/api/v1/person/person/20209/"))
+        self.assertEqual(p[ 0].resource_uri, PersonURI(uri="/api/v1/person/person/20209/"))
 
 
+    def test_person_ext_resource(self) -> None:
+        r = self.dt.person_ext_resource(PersonExtResourceURI(uri="/api/v1/person/personextresource/177/"))
+        if r is not None:
+            self.assertEqual(r.resource_uri, PersonExtResourceURI(uri="/api/v1/person/personextresource/177/"))
+            self.assertEqual(r.id,           177)
+            self.assertEqual(r.display_name, "")
+            self.assertEqual(r.person,       PersonURI(uri="/api/v1/person/person/20209/"))
+            self.assertEqual(r.name,         ExtResourceNameURI(uri="/api/v1/name/extresourcename/github_username/"))
+            self.assertEqual(r.value,        "csperkins")
+        else:
+            self.fail("Cannot find PersonExternalResource")
+
+
+    def test_person_ext_resources(self) -> None:
+        p = self.dt.person_from_email("csp@csperkins.org")
+        r = list(self.dt.person_ext_resources(p))
+        self.assertEqual(len(r), 3)
+        self.assertEqual(r[0].value, "csperkins")
+        self.assertEqual(r[1].value, "https://csperkins.org/")
+        self.assertEqual(r[2].value, "https://www.gla.ac.uk/schools/computing/staff/colinperkins/")
+
+
+    def test_ext_resource_name(self) -> None:
+        r = self.dt.ext_resource_name(ExtResourceNameURI(uri="/api/v1/name/extresourcename/github_username/"))
+        if r is not None:
+            self.assertEqual(r.resource_uri, ExtResourceNameURI(uri="/api/v1/name/extresourcename/github_username/"))
+            self.assertEqual(r.desc,  "GitHub Username")
+            self.assertEqual(r.name,  "GitHub Username")
+            self.assertEqual(r.order, 0)
+            self.assertEqual(r.slug,  "github_username")
+            self.assertEqual(r.type,  ExtResourceTypeNameURI(uri="/api/v1/name/extresourcetypename/string/"))
+            self.assertEqual(r.used,  True)
+        else:
+            self.fail("Cannot find ExtResourceName")
+
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to documents:
 
-    # There is one test_document_*() method for each document type
+    # There is one test_document_*() method for each document type
 
     def test_document_agenda(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/agenda-90-precis/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/agenda-90-precis/"))
         if d is not None:
             self.assertEqual(d.expires,            None)
             self.assertEqual(d.intended_std_level, None)
             self.assertEqual(d.uploaded_filename,  "agenda-90-precis.txt")
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/81/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/81/")])
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.notify,             "")
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/agenda/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/agenda/"))
             self.assertEqual(d.rev,                "2")
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 218)
             self.assertEqual(d.std_level,          None)
             self.assertEqual(d.ad,                 None)
             self.assertEqual(d.time,               datetime.fromisoformat("2014-07-21T18:14:17+00:00"))
             self.assertEqual(d.title,              "Agenda for PRECIS at IETF-90")
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.pages,              None)
             self.assertEqual(d.tags,               [])
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/agenda-90-precis/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/agenda-90-precis/"))
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.words,              None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.name,               "agenda-90-precis")
             self.assertEqual(d.stream,             None)
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/1798/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/1798/"))
             self.assertEqual(d.note,               "")
             self.assertEqual(d.external_url,       "")
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/proceedings/90/agenda/agenda-90-precis.txt")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_bluesheets(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/bluesheets-95-xrblock-01/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/bluesheets-95-xrblock-01/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 68163)
             self.assertEqual(d.name,               "bluesheets-95-xrblock-01")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "00")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/bluesheets/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/1815/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/bluesheets-95-xrblock-01/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/bluesheets/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/1815/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/bluesheets-95-xrblock-01/"))
             self.assertEqual(d.title,              "Bluesheets IETF95 : xrblock : Wed 16:20")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "bluesheets-95-xrblock-01.pdf")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -525,36 +561,36 @@
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("2016-08-22T05:39:08-07:00"))
             self.assertEqual(d.pages,              None)
             self.assertEqual(d.stream,             None)
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/139/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/139/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/proceedings/95/bluesheets/bluesheets-95-xrblock-01.pdf")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_charter(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/charter-ietf-vgmib/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/charter-ietf-vgmib/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 1)
             self.assertEqual(d.name,               "charter-ietf-vgmib")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "01")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/charter/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/925/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/charter-ietf-vgmib/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/charter/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/925/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/charter-ietf-vgmib/"))
             self.assertEqual(d.title,              "100VG-AnyLAN MIB")
             self.assertEqual(d.abstract,           "100VG-AnyLAN MIB")
             self.assertEqual(d.uploaded_filename,  "")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -562,110 +598,110 @@
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("1998-01-26T12:00:00-08:00"))
             self.assertEqual(d.pages,              None)
             self.assertEqual(d.stream,             None)
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/88/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/88/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/charter/charter-ietf-vgmib-01.txt")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_conflrev(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/conflict-review-kiyomoto-kcipher2/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/conflict-review-kiyomoto-kcipher2/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 17898)
             self.assertEqual(d.name,               "conflict-review-kiyomoto-kcipher2")
             self.assertEqual(d.notify,             "\"Nevil Brownlee\" <rfc-ise@rfc-editor.org>, draft-kiyomoto-kcipher2@tools.ietf.org")
             self.assertEqual(d.rev,                "00")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/conflrev/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/2/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/conflict-review-kiyomoto-kcipher2/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/conflrev/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/2/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/conflict-review-kiyomoto-kcipher2/"))
             self.assertEqual(d.title,              "IETF conflict review for draft-kiyomoto-kcipher2")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
-            self.assertEqual(d.ad,                 PersonURI("/api/v1/person/person/19177/"))
+            self.assertEqual(d.ad,                 PersonURI(uri="/api/v1/person/person/19177/"))
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("2013-07-15T14:47:31-07:00"))
             self.assertEqual(d.pages,              None)
-            self.assertEqual(d.stream,             StreamURI("/api/v1/name/streamname/ietf/"))
+            self.assertEqual(d.stream,             StreamURI(uri="/api/v1/name/streamname/ietf/"))
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/97/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/97/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/cr/conflict-review-kiyomoto-kcipher2-00.txt")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_draft(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/draft-ietf-avt-rtp-new/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-ietf-avt-rtp-new/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 19971)
             self.assertEqual(d.name,               "draft-ietf-avt-rtp-new")
             self.assertEqual(d.notify,             "magnus.westerlund@ericsson.com, csp@csperkins.org")
             self.assertEqual(d.rev,                "12")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            "2003-09-08T07:00:12Z")
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/draft/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/941/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/draft-ietf-avt-rtp-new/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/draft/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/941/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/draft-ietf-avt-rtp-new/"))
             self.assertEqual(d.title,              "RTP: A Transport Protocol for Real-Time Applications")
             # self.assertEqual(d.abstract,         "This memorandum describes RTP, the real-time transport protocol...")
             self.assertEqual(d.uploaded_filename,  "")
-            self.assertEqual(d.rfc,                3550)
+            self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, "/api/v1/name/intendedstdlevelname/std/")
-            self.assertEqual(d.ad,                 PersonURI("/api/v1/person/person/2515/"))
+            self.assertEqual(d.ad,                 PersonURI(uri="/api/v1/person/person/2515/"))
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              34861)
-            self.assertEqual(d.tags,               [DocumentTagURI("/api/v1/name/doctagname/app-min/"), DocumentTagURI("/api/v1/name/doctagname/errata/")])
+            self.assertEqual(d.tags,               [DocumentTagURI(uri="/api/v1/name/doctagname/app-min/")])
             self.assertEqual(d.time,               datetime.fromisoformat("2015-10-14T20:49:52+00:00"))
             self.assertEqual(d.pages,              104)
-            self.assertEqual(d.stream,             StreamURI("/api/v1/name/streamname/ietf/"))
+            self.assertEqual(d.stream,             StreamURI(uri="/api/v1/name/streamname/ietf/"))
             self.assertEqual(d.std_level,          "/api/v1/name/stdlevelname/std/")
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/3/"), DocumentStateURI("/api/v1/doc/state/7/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/3/"), DocumentStateURI(uri="/api/v1/doc/state/7/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/archive/id/draft-ietf-avt-rtp-new-12.txt")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_liaison(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/liaison-2012-05-31-3gpp-mmusic-on-rtcp-bandwidth-negotiation-attachment-1/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/liaison-2012-05-31-3gpp-mmusic-on-rtcp-bandwidth-negotiation-attachment-1/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 46457)
             self.assertEqual(d.name,               "liaison-2012-05-31-3gpp-mmusic-on-rtcp-bandwidth-negotiation-attachment-1")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/liaison/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/liaison/"))
             self.assertEqual(d.group,              None)
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/liaison-2012-05-31-3gpp-mmusic-on-rtcp-bandwidth-negotiation-attachment-1/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/liaison-2012-05-31-3gpp-mmusic-on-rtcp-bandwidth-negotiation-attachment-1/"))
             self.assertEqual(d.title,              "S4-120810 DRAFT LS to IETF MMUSIC WG on RTCP Bandwidth Negotiation")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "liaison-2012-05-31-3gpp-mmusic-on-rtcp-bandwidth-negotiation-attachment-1.doc")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -683,26 +719,26 @@
             self.assertEqual(url, "https://www.ietf.org/lib/dt/documents/LIAISON/liaison-2012-05-31-3gpp-mmusic-on-rtcp-bandwidth-negotiation-attachment-1.doc")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_liai_att(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/liaison-2004-08-23-itu-t-ietf-liaison-statement-to-ietf-and-itu-t-study-groups-countering-spam-pdf-version-attachment-1/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/liaison-2004-08-23-itu-t-ietf-liaison-statement-to-ietf-and-itu-t-study-groups-countering-spam-pdf-version-attachment-1/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 43519)
             self.assertEqual(d.name,               "liaison-2004-08-23-itu-t-ietf-liaison-statement-to-ietf-and-itu-t-study-groups-countering-spam-pdf-version-attachment-1")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/liai-att/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/liai-att/"))
             self.assertEqual(d.group,              None)
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/liaison-2004-08-23-itu-t-ietf-liaison-statement-to-ietf-and-itu-t-study-groups-countering-spam-pdf-version-attachment-1/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/liaison-2004-08-23-itu-t-ietf-liaison-statement-to-ietf-and-itu-t-study-groups-countering-spam-pdf-version-attachment-1/"))
             self.assertEqual(d.title,              "Liaison Statement to IETF and ITU-T Study Groups: Countering SPAM (PDF version)")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "file39.pdf")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -720,26 +756,26 @@
             self.assertEqual(url, "https://www.ietf.org/lib/dt/documents/LIAISON/file39.pdf")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_minutes(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/minutes-89-cfrg/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/minutes-89-cfrg/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 272)
             self.assertEqual(d.name,               "minutes-89-cfrg")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "1")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/minutes/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/31/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/minutes-89-cfrg/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/minutes/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/31/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/minutes-89-cfrg/"))
             self.assertEqual(d.title,              "Minutes for CFRG at IETF-89")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "minutes-89-cfrg.txt")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -747,36 +783,36 @@
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("2014-04-09T08:09:14-07:00"))
             self.assertEqual(d.pages,              None)
             self.assertEqual(d.stream,             None)
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/79/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/79/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/proceedings/89/minutes/minutes-89-cfrg.txt")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_recording(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/recording-94-taps-1/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/recording-94-taps-1/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 49624)
             self.assertEqual(d.name,               "recording-94-taps-1")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "00")
             self.assertEqual(d.external_url,       "https://www.ietf.org/audio/ietf94/ietf94-room304-20151103-1520.mp3")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/recording/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/1924/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/recording-94-taps-1/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/recording/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/1924/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/recording-94-taps-1/"))
             self.assertEqual(d.title,              "Audio recording for 2015-11-03 15:20")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -784,37 +820,37 @@
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("2015-11-24T08:23:42-08:00"))
             self.assertEqual(d.pages,              None)
             self.assertEqual(d.stream,             None)
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/135/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/135/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/audio/ietf94/ietf94-room304-20151103-1520.mp3")
             # Downloading the MP3 is expensive, so check a HEAD request instead:
             # self.assertEqual(self.dt.session.head(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_review(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/review-bchv-rfc6890bis-04-genart-lc-kyzivat-2017-02-28/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/review-bchv-rfc6890bis-04-genart-lc-kyzivat-2017-02-28/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 69082)
             self.assertEqual(d.name,               "review-bchv-rfc6890bis-04-genart-lc-kyzivat-2017-02-28")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "00")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/review/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/1972/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/review-bchv-rfc6890bis-04-genart-lc-kyzivat-2017-02-28/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/review/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/1972/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/review-bchv-rfc6890bis-04-genart-lc-kyzivat-2017-02-28/"))
             self.assertEqual(d.title,              "Last Call Review of draft-bchv-rfc6890bis-04")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -822,41 +858,41 @@
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("2017-02-28T12:52:33-08:00"))
             self.assertEqual(d.pages,              None)
             self.assertEqual(d.stream,             None)
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/143/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/143/")])
 
             url = d.url()
             self.assertEqual(url, "https://datatracker.ietf.org/doc/review-bchv-rfc6890bis-04-genart-lc-kyzivat-2017-02-28")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_shepwrit(self) -> None:
-        for d in self.dt.documents(doctype=self.dt.document_type(DocumentTypeURI("/api/v1/name/doctypename/shepwrit/"))):
+        for d in self.dt.documents(doctype=self.dt.document_type(DocumentTypeURI(uri="/api/v1/name/doctypename/shepwrit/"))):
             self.fail("shepwrit is not used, so this should return no documents")
 
 
     def test_document_slides(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/slides-65-l2vpn-4/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/slides-65-l2vpn-4/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 736)
             self.assertEqual(d.name,               "slides-65-l2vpn-4")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "00")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/slides/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/1593/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/slides-65-l2vpn-4/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/slides/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/1593/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/slides-65-l2vpn-4/"))
             self.assertEqual(d.title,              "Congruency for VPLS Mcast & Unicast Paths")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "l2vpn-4.pdf")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
@@ -864,62 +900,62 @@
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("2006-04-07T17:30:22-07:00"))
             self.assertEqual(d.pages,              None)
             self.assertEqual(d.stream,             None)
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/141/"), DocumentStateURI("/api/v1/doc/state/138/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/141/"), DocumentStateURI(uri="/api/v1/doc/state/138/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/proceedings/65/slides/l2vpn-4.pdf")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_document_statchg(self) -> None:
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/status-change-rfc3044-rfc3187-orig-urn-regs-to-historic/"))
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/status-change-rfc3044-rfc3187-orig-urn-regs-to-historic/"))
         if d is not None:
             self.assertEqual(d.internal_comments,  "")
             self.assertEqual(d.id,                 78306)
             self.assertEqual(d.name,               "status-change-rfc3044-rfc3187-orig-urn-regs-to-historic")
             self.assertEqual(d.notify,             "")
             self.assertEqual(d.rev,                "00")
             self.assertEqual(d.external_url,       "")
             self.assertEqual(d.expires,            None)
-            self.assertEqual(d.type,               DocumentTypeURI("/api/v1/name/doctypename/statchg/"))
-            self.assertEqual(d.group,              GroupURI("/api/v1/group/group/2/"))
-            self.assertEqual(d.resource_uri,       DocumentURI("/api/v1/doc/document/status-change-rfc3044-rfc3187-orig-urn-regs-to-historic/"))
+            self.assertEqual(d.type,               DocumentTypeURI(uri="/api/v1/name/doctypename/statchg/"))
+            self.assertEqual(d.group,              GroupURI(uri="/api/v1/group/group/2/"))
+            self.assertEqual(d.resource_uri,       DocumentURI(uri="/api/v1/doc/document/status-change-rfc3044-rfc3187-orig-urn-regs-to-historic/"))
             self.assertEqual(d.title,              "Change status of RFC 3044 and RFC 3187 (original ISSN and ISBN URN Namespace registrationS) to Historic")
             self.assertEqual(d.abstract,           "")
             self.assertEqual(d.uploaded_filename,  "")
             self.assertEqual(d.rfc,                None)
             self.assertEqual(d.shepherd,           None)
             self.assertEqual(d.submissions,        [])
             self.assertEqual(d.intended_std_level, None)
-            self.assertEqual(d.ad,                 PersonURI("/api/v1/person/person/102154/"))
+            self.assertEqual(d.ad,                 PersonURI(uri="/api/v1/person/person/102154/"))
             self.assertEqual(d.note,               "")
             self.assertEqual(d.words,              None)
             self.assertEqual(d.tags,               [])
             self.assertEqual(d.time,               datetime.fromisoformat("2017-08-21T09:32:46-07:00"))
             self.assertEqual(d.pages,              None)
-            self.assertEqual(d.stream,             StreamURI("/api/v1/name/streamname/ietf/"))
+            self.assertEqual(d.stream,             StreamURI(uri="/api/v1/name/streamname/ietf/"))
             self.assertEqual(d.std_level,          None)
-            self.assertEqual(d.states,             [DocumentStateURI("/api/v1/doc/state/127/")])
+            self.assertEqual(d.states,             [DocumentStateURI(uri="/api/v1/doc/state/127/")])
 
             url = d.url()
             self.assertEqual(url, "https://www.ietf.org/sc/status-change-rfc3044-rfc3187-orig-urn-regs-to-historic-00.txt")
             self.assertEqual(self.dt.session.get(url).status_code, 200)
         else:
             self.fail("Cannot find document")
 
 
     def test_documents(self):
-        doctype = self.dt.document_type(DocumentTypeURI("/api/v1/name/doctypename/draft/"))
+        doctype = self.dt.document_type(DocumentTypeURI(uri="/api/v1/name/doctypename/draft/"))
         group   = self.dt.group_from_acronym("xrblock")
         documents = list(self.dt.documents(doctype = doctype, group = group))
         self.assertEqual(len(documents), 21)
         self.assertEqual(documents[ 0].name, "draft-ietf-xrblock-rtcp-xr-discard-rle-metrics")
         self.assertEqual(documents[ 1].name, "draft-ietf-xrblock-rtcp-xr-pdv")
         self.assertEqual(documents[ 2].name, "draft-ietf-xrblock-rtcp-xr-meas-identity")
         self.assertEqual(documents[ 3].name, "draft-ietf-xrblock-rtcp-xr-delay")
@@ -942,60 +978,57 @@
         self.assertEqual(documents[20].name, "draft-ietf-xrblock-independent-burst-gap-discard")
 
 
     # FIXME: this needs to be updated
     def test_document_from_draft(self) -> None:
         d  = self.dt.document_from_draft("draft-ietf-avt-rtp-new")
         if d is not None:
-            self.assertEqual(d.resource_uri, DocumentURI("/api/v1/doc/document/draft-ietf-avt-rtp-new/"))
+            self.assertEqual(d.resource_uri, DocumentURI(uri="/api/v1/doc/document/draft-ietf-avt-rtp-new/"))
         else:
             self.fail("Cannot find document")
 
-    # FIXME: this needs to be updated
     def test_document_from_rfc(self) -> None:
         d  = self.dt.document_from_rfc("rfc3550")
         if d is not None:
-            self.assertEqual(d.resource_uri, DocumentURI("/api/v1/doc/document/draft-ietf-avt-rtp-new/"))
+            self.assertEqual(d.resource_uri, DocumentURI(uri="/api/v1/doc/document/rfc3550/"))
         else:
             self.fail("Cannot find document")
 
-    # FIXME: this needs to be updated
     def test_documents_from_bcp(self) -> None:
         d  = list(self.dt.documents_from_bcp("bcp205"))
         if d is not None:
             self.assertEqual(len(d), 1)
-            self.assertEqual(d[0].resource_uri, DocumentURI("/api/v1/doc/document/draft-sheffer-rfc6982bis/"))
+            self.assertEqual(d[0].resource_uri, DocumentURI(uri="/api/v1/doc/document/rfc7942/"))
         else:
             self.fail("Cannot find document")
 
-    # FIXME: this needs to be updated
     def test_documents_from_std(self) -> None:
         d  = list(self.dt.documents_from_std("std68"))
         self.assertEqual(len(d), 1)
-        self.assertEqual(d[0].resource_uri, DocumentURI("/api/v1/doc/document/draft-crocker-rfc4234bis/"))
+        self.assertEqual(d[0].resource_uri, DocumentURI(uri="/api/v1/doc/document/rfc5234/"))
 
 
     def test_document_state(self) -> None:
-        s = self.dt.document_state(DocumentStateURI('/api/v1/doc/state/7/'))
+        s = self.dt.document_state(DocumentStateURI(uri="/api/v1/doc/state/7/"))
         if s is not None:
             self.assertEqual(s.id,           7)
-            self.assertEqual(s.resource_uri, DocumentStateURI("/api/v1/doc/state/7/"))
+            self.assertEqual(s.resource_uri, DocumentStateURI(uri="/api/v1/doc/state/7/"))
             self.assertEqual(s.name,         "RFC Published")
             self.assertEqual(s.desc,         "The ID has been published as an RFC.")
-            self.assertEqual(s.type,         DocumentStateTypeURI("/api/v1/doc/statetype/draft-iesg/"))
-            self.assertEqual(s.next_states,  [DocumentStateURI("/api/v1/doc/state/8/")])
+            self.assertEqual(s.type,         DocumentStateTypeURI(uri="/api/v1/doc/statetype/draft-iesg/"))
+            self.assertEqual(s.next_states,  [DocumentStateURI(uri="/api/v1/doc/state/8/")])
             self.assertEqual(s.order,        32)
             self.assertEqual(s.slug,         "pub")
             self.assertEqual(s.used,         True)
         else:
             self.fail("Cannot find state")
 
 
     def test_document_states(self) -> None:
-        st = self.dt.document_state_type(DocumentStateTypeURI("/api/v1/doc/statetype/draft-rfceditor/"))
+        st = self.dt.document_state_type(DocumentStateTypeURI(uri="/api/v1/doc/statetype/draft-rfceditor/"))
         states = list(self.dt.document_states(state_type = st))
         self.assertEqual(len(states), 19)
         self.assertEqual(states[ 0].name, 'AUTH')
         self.assertEqual(states[ 1].name, 'AUTH48')
         self.assertEqual(states[ 2].name, 'EDIT')
         self.assertEqual(states[ 3].name, 'IANA')
         self.assertEqual(states[ 4].name, 'IESG')
@@ -1012,65 +1045,69 @@
         self.assertEqual(states[15].name, 'IESG')
         self.assertEqual(states[16].name, 'ISR-AUTH')
         self.assertEqual(states[17].name, 'Pending')
         self.assertEqual(states[18].name, 'TI')
 
 
     def test_document_state_type(self) -> None:
-        st = self.dt.document_state_type(DocumentStateTypeURI("/api/v1/doc/statetype/draft-rfceditor/"))
+        st = self.dt.document_state_type(DocumentStateTypeURI(uri="/api/v1/doc/statetype/draft-rfceditor/"))
         if st is not None:
-            self.assertEqual(st.resource_uri, DocumentStateTypeURI("/api/v1/doc/statetype/draft-rfceditor/"))
+            self.assertEqual(st.resource_uri, DocumentStateTypeURI(uri="/api/v1/doc/statetype/draft-rfceditor/"))
             self.assertEqual(st.slug,         "draft-rfceditor")
             self.assertEqual(st.label,        "RFC Editor state")
         else:
             self.fail("Cannot find state type")
 
 
     def test_document_state_types(self) -> None:
         st = list(self.dt.document_state_types())
-        self.assertEqual(len(st), 30)
+        self.assertEqual(len(st), 34)
         self.assertEqual(st[ 0].slug, 'agenda')
-        self.assertEqual(st[ 1].slug, 'bluesheets')
-        self.assertEqual(st[ 2].slug, 'bofreq')
-        self.assertEqual(st[ 3].slug, 'charter')
-        self.assertEqual(st[ 4].slug, 'chatlog')
-        self.assertEqual(st[ 5].slug, 'conflrev')
-        self.assertEqual(st[ 6].slug, 'draft')
-        self.assertEqual(st[ 7].slug, 'draft-iana')
+        self.assertEqual(st[ 1].slug, 'bcp')
+        self.assertEqual(st[ 2].slug, 'bluesheets')
+        self.assertEqual(st[ 3].slug, 'bofreq')
+        self.assertEqual(st[ 4].slug, 'charter')
+        self.assertEqual(st[ 5].slug, 'chatlog')
+        self.assertEqual(st[ 6].slug, 'conflrev')
+        self.assertEqual(st[ 7].slug, 'draft')
         self.assertEqual(st[ 8].slug, 'draft-iana-action')
         self.assertEqual(st[ 9].slug, 'draft-iana-experts')
         self.assertEqual(st[10].slug, 'draft-iana-review')
         self.assertEqual(st[11].slug, 'draft-iesg')
         self.assertEqual(st[12].slug, 'draft-rfceditor')
         self.assertEqual(st[13].slug, 'draft-stream-editorial')
         self.assertEqual(st[14].slug, 'draft-stream-iab')
         self.assertEqual(st[15].slug, 'draft-stream-ietf')
         self.assertEqual(st[16].slug, 'draft-stream-irtf')
         self.assertEqual(st[17].slug, 'draft-stream-ise')
-        self.assertEqual(st[18].slug, 'liai-att')
-        self.assertEqual(st[19].slug, 'liaison')
-        self.assertEqual(st[20].slug, 'minutes')
-        self.assertEqual(st[21].slug, 'polls')
-        self.assertEqual(st[22].slug, 'procmaterials')
-        self.assertEqual(st[23].slug, 'recording')
-        self.assertEqual(st[24].slug, 'reuse_policy')
-        self.assertEqual(st[25].slug, 'review')
-        self.assertEqual(st[26].slug, 'shepwrit')
-        self.assertEqual(st[27].slug, 'slides')
-        self.assertEqual(st[28].slug, 'statchg')
-        self.assertEqual(st[29].slug, 'statement')
+        self.assertEqual(st[18].slug, 'fyi')
+        self.assertEqual(st[19].slug, 'liai-att')
+        self.assertEqual(st[20].slug, 'liaison')
+        self.assertEqual(st[21].slug, 'minutes')
+        self.assertEqual(st[22].slug, 'narrativeminutes')
+        self.assertEqual(st[23].slug, 'polls')
+        self.assertEqual(st[24].slug, 'procmaterials')
+        self.assertEqual(st[25].slug, 'recording')
+        self.assertEqual(st[26].slug, 'reuse_policy')
+        self.assertEqual(st[27].slug, 'review')
+        self.assertEqual(st[28].slug, 'rfc')
+        self.assertEqual(st[29].slug, 'shepwrit')
+        self.assertEqual(st[30].slug, 'slides')
+        self.assertEqual(st[31].slug, 'statchg')
+        self.assertEqual(st[32].slug, 'statement')
+        self.assertEqual(st[33].slug, 'std')
 
 
     def test_document_event(self) -> None:
-        e = self.dt.document_event(DocumentEventURI("/api/v1/doc/docevent/729040/"))
+        e = self.dt.document_event(DocumentEventURI(uri="/api/v1/doc/docevent/729040/"))
         if e is not None:
             self.assertEqual(e.id,              729040)
-            self.assertEqual(e.resource_uri,    DocumentEventURI("/api/v1/doc/docevent/729040/"))
-            self.assertEqual(e.by,              PersonURI("/api/v1/person/person/121595/"))
-            self.assertEqual(e.doc,             DocumentURI("/api/v1/doc/document/draft-irtf-cfrg-randomness-improvements/"))
+            self.assertEqual(e.resource_uri,    DocumentEventURI(uri="/api/v1/doc/docevent/729040/"))
+            self.assertEqual(e.by,              PersonURI(uri="/api/v1/person/person/121595/"))
+            self.assertEqual(e.doc,             DocumentURI(uri="/api/v1/doc/document/draft-irtf-cfrg-randomness-improvements/"))
             self.assertEqual(e.type,            "new_revision")
             self.assertEqual(e.desc,            "New version available: <b>draft-irtf-cfrg-randomness-improvements-09.txt</b>")
             self.assertEqual(e.rev,             "09")
             self.assertEqual(e.time,            datetime.fromisoformat("2020-01-27T06:41:36-08:00"))
         else:
             self.fail("Cannot find event")
 
@@ -1105,31 +1142,31 @@
         p  = self.dt.person_from_email("csp@csperkins.org")
         d  = self.dt.document_from_draft("draft-ietf-avtcore-rtp-circuit-breakers")
         de = list(self.dt.document_events(doc=d, by=p))
         self.assertEqual(len(de), 22)
 
 
     def test_ballot_position_name(self) -> None:
-        bp = self.dt.ballot_position_name(BallotPositionNameURI("/api/v1/name/ballotpositionname/moretime/"))
+        bp = self.dt.ballot_position_name(BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/moretime/"))
         if bp is not None:
             self.assertEqual(bp.blocking,     False)
             self.assertEqual(bp.desc,         "")
             self.assertEqual(bp.order,        0)
-            self.assertEqual(bp.resource_uri, BallotPositionNameURI("/api/v1/name/ballotpositionname/moretime/"))
+            self.assertEqual(bp.resource_uri, BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/moretime/"))
             self.assertEqual(bp.slug,         "moretime")
             self.assertEqual(bp.used,         True)
 
 
     def test_ballot_position_name_from_slug(self) -> None:
         bp = self.dt.ballot_position_name_from_slug("moretime")
         if bp is not None:
             self.assertEqual(bp.blocking,     False)
             self.assertEqual(bp.desc,         "")
             self.assertEqual(bp.order,        0)
-            self.assertEqual(bp.resource_uri, BallotPositionNameURI("/api/v1/name/ballotpositionname/moretime/"))
+            self.assertEqual(bp.resource_uri, BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/moretime/"))
             self.assertEqual(bp.slug,         "moretime")
             self.assertEqual(bp.used,         True)
 
 
     def test_ballot_position_names(self) -> None:
         bps = list(self.dt.ballot_position_names())
         self.assertEqual(len(bps), 10)
@@ -1142,227 +1179,255 @@
         self.assertEqual(bps[6].slug, "norecord")
         self.assertEqual(bps[7].slug, "notready")
         self.assertEqual(bps[8].slug, "recuse")
         self.assertEqual(bps[9].slug, "yes")
 
 
     def test_ballot_type(self) -> None:
-        bt = self.dt.ballot_type(BallotTypeURI("/api/v1/doc/ballottype/5/"))
+        bt = self.dt.ballot_type(BallotTypeURI(uri="/api/v1/doc/ballottype/5/"))
         if bt is not None:
-            self.assertEqual(bt.doc_type,       DocumentTypeURI("/api/v1/name/doctypename/conflrev/"))
+            self.assertEqual(bt.doc_type,       DocumentTypeURI(uri="/api/v1/name/doctypename/conflrev/"))
             self.assertEqual(bt.id,             5)
             self.assertEqual(bt.name,           "Approve")
             self.assertEqual(bt.order,          0)
             self.assertEqual(len(bt.positions), 6)
-            self.assertEqual(bt.positions[0],   BallotPositionNameURI("/api/v1/name/ballotpositionname/yes/"))
-            self.assertEqual(bt.positions[1],   BallotPositionNameURI("/api/v1/name/ballotpositionname/noobj/"))
-            self.assertEqual(bt.positions[2],   BallotPositionNameURI("/api/v1/name/ballotpositionname/discuss/"))
-            self.assertEqual(bt.positions[3],   BallotPositionNameURI("/api/v1/name/ballotpositionname/abstain/"))
-            self.assertEqual(bt.positions[4],   BallotPositionNameURI("/api/v1/name/ballotpositionname/recuse/"))
-            self.assertEqual(bt.positions[5],   BallotPositionNameURI("/api/v1/name/ballotpositionname/norecord/"))
+            self.assertEqual(bt.positions[0],   BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/yes/"))
+            self.assertEqual(bt.positions[1],   BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/noobj/"))
+            self.assertEqual(bt.positions[2],   BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/discuss/"))
+            self.assertEqual(bt.positions[3],   BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/abstain/"))
+            self.assertEqual(bt.positions[4],   BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/recuse/"))
+            self.assertEqual(bt.positions[5],   BallotPositionNameURI(uri="/api/v1/name/ballotpositionname/norecord/"))
             self.assertEqual(bt.question,       "Is this the correct conflict review response?")
-            self.assertEqual(bt.resource_uri,   BallotTypeURI("/api/v1/doc/ballottype/5/"))
+            self.assertEqual(bt.resource_uri,   BallotTypeURI(uri="/api/v1/doc/ballottype/5/"))
             self.assertEqual(bt.slug,           "conflrev")
             self.assertEqual(bt.used,           True)
         else:
             self.fail("Could not find ballot type")
 
 
     def test_ballot_types_doctype(self) -> None:
-        bts = list(self.dt.ballot_types(self.dt.document_type(DocumentTypeURI("/api/v1/name/doctypename/draft/"))))
+        bts = list(self.dt.ballot_types(self.dt.document_type(DocumentTypeURI(uri="/api/v1/name/doctypename/draft/"))))
         self.assertEqual(len(bts), 3)
         self.assertEqual(bts[0].slug, "approve")
         self.assertEqual(bts[1].slug, "irsg-approve")
 
 
     def test_ballot_document_event(self) -> None:
-        e = self.dt.ballot_document_event(BallotDocumentEventURI("/api/v1/doc/ballotdocevent/744784/"))
+        e = self.dt.ballot_document_event(BallotDocumentEventURI(uri="/api/v1/doc/ballotdocevent/744784/"))
         if e is not None:
-            self.assertEqual(e.ballot_type,  BallotTypeURI("/api/v1/doc/ballottype/5/"))
-            self.assertEqual(e.by,           PersonURI("/api/v1/person/person/21684/"))
+            self.assertEqual(e.ballot_type,  BallotTypeURI(uri="/api/v1/doc/ballottype/5/"))
+            self.assertEqual(e.by,           PersonURI(uri="/api/v1/person/person/21684/"))
             self.assertEqual(e.desc,         'Created "Approve" ballot')
-            self.assertEqual(e.doc,          DocumentURI("/api/v1/doc/document/conflict-review-dold-payto/"))
-            self.assertEqual(e.docevent_ptr, DocumentEventURI("/api/v1/doc/docevent/744784/"))
+            self.assertEqual(e.doc,          DocumentURI(uri="/api/v1/doc/document/conflict-review-dold-payto/"))
+            self.assertEqual(e.docevent_ptr, DocumentEventURI(uri="/api/v1/doc/docevent/744784/"))
             self.assertEqual(e.id,           744784)
-            self.assertEqual(e.resource_uri, BallotDocumentEventURI("/api/v1/doc/ballotdocevent/744784/"))
+            self.assertEqual(e.resource_uri, BallotDocumentEventURI(uri="/api/v1/doc/ballotdocevent/744784/"))
             self.assertEqual(e.rev,          "00")
             self.assertEqual(e.time,         datetime.fromisoformat("2020-04-04T10:57:29-07:00"))
             self.assertEqual(e.type,         "created_ballot")
         else:
             self.fail("Cannot find ballot event")
 
 
     def test_ballot_document_events(self) -> None:
         d  = self.dt.document_from_draft("draft-ietf-avtcore-rtp-circuit-breakers")
         de = list(self.dt.ballot_document_events(doc=d))
         self.assertEqual(len(de), 2)
         self.assertEqual(de[0].id, 461800)
         self.assertEqual(de[1].id, 478676)
 
-        bt = self.dt.ballot_type(BallotTypeURI("/api/v1/doc/ballottype/3/")) # Charter approval
-        p  = self.dt.person(PersonURI("/api/v1/person/person/108756/"))      # Cindy Morgan
-        d  = self.dt.document(DocumentURI("/api/v1/doc/document/charter-ietf-rmcat/"))
+        bt = self.dt.ballot_type(BallotTypeURI(uri="/api/v1/doc/ballottype/3/")) # Charter approval
+        p  = self.dt.person(PersonURI(uri="/api/v1/person/person/108756/"))      # Cindy Morgan
+        d  = self.dt.document(DocumentURI(uri="/api/v1/doc/document/charter-ietf-rmcat/"))
         de = list(self.dt.ballot_document_events(doc = d, ballot_type = bt, by = p, event_type = "closed_ballot"))
         self.assertEqual(len(de), 1)
         self.assertEqual(de[0].id, 304166)
 
 
     def test_documents_authored_by_person(self) -> None:
         p = self.dt.person_from_email("ladan@isi.edu")
         if p is not None:
             a = list(self.dt.documents_authored_by_person(p))
-            self.assertEqual(len(a), 7)
+            self.assertEqual(len(a), 9)
             self.assertEqual(a[0].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-ac3/'))
             self.assertEqual(a[1].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-hdtv-video/'))
             self.assertEqual(a[2].document, DocumentURI(uri='/api/v1/doc/document/draft-ietf-avt-smpte292-video/'))
             self.assertEqual(a[3].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-avt-uncomp-video/'))
             self.assertEqual(a[4].document, DocumentURI(uri='/api/v1/doc/document/draft-ietf-avt-uncomp-video/'))
             self.assertEqual(a[5].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-avt-tfrc-profile/'))
             self.assertEqual(a[6].document, DocumentURI(uri='/api/v1/doc/document/draft-ietf-avt-tfrc-profile/'))
+            self.assertEqual(a[7].document, DocumentURI(uri='/api/v1/doc/document/rfc3497/'))
+            self.assertEqual(a[8].document, DocumentURI(uri='/api/v1/doc/document/rfc4175/'))
         else:
             self.fail("Cannot find person");
 
 
     def test_documents_authored_by_email(self) -> None:
-        e = self.dt.email(EmailURI("/api/v1/person/email/ladan@isi.edu/"))
+        e = self.dt.email(EmailURI(uri="/api/v1/person/email/ladan@isi.edu/"))
         if e is not None:
             a = list(self.dt.documents_authored_by_email(e))
-            self.assertEqual(len(a), 7)
+            self.assertEqual(len(a), 9)
             self.assertEqual(a[0].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-ac3/'))
             self.assertEqual(a[1].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-hdtv-video/'))
             self.assertEqual(a[2].document, DocumentURI(uri='/api/v1/doc/document/draft-ietf-avt-smpte292-video/'))
             self.assertEqual(a[3].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-avt-uncomp-video/'))
             self.assertEqual(a[4].document, DocumentURI(uri='/api/v1/doc/document/draft-ietf-avt-uncomp-video/'))
             self.assertEqual(a[5].document, DocumentURI(uri='/api/v1/doc/document/draft-gharai-avt-tfrc-profile/'))
             self.assertEqual(a[6].document, DocumentURI(uri='/api/v1/doc/document/draft-ietf-avt-tfrc-profile/'))
+            self.assertEqual(a[7].document, DocumentURI(uri='/api/v1/doc/document/rfc3497/'))
+            self.assertEqual(a[8].document, DocumentURI(uri='/api/v1/doc/document/rfc4175/'))
         else:
             self.fail("Cannot find person");
 
 
 
 
     # FIXME: this needs to be updated
     def test_submission(self) -> None:
-        s  = self.dt.submission(SubmissionURI("/api/v1/submit/submission/2402/"))
+        s  = self.dt.submission(SubmissionURI(uri="/api/v1/submit/submission/2402/"))
         if s is not None:
             #self.assertEqual(s.abstract,        "Internet technical specifications often need to...")
             self.assertEqual(s.access_key,      "f77d08da6da54f3cbecca13d31646be8")
             self.assertEqual(s.auth_key,        "fMm6hur5dJ7gV58x5SE0vkHUoDOrSuSF")
             self.assertEqual(s.authors,         "[{'email': 'dcrocker@bbiw.net', 'name': 'Dave Crocker'}, {'email': 'paul.overell@thus.net', 'name': 'Paul Overell'}]")
-            self.assertEqual(s.checks,          [SubmissionCheckURI("/api/v1/submit/submissioncheck/386/")])
-            self.assertEqual(s.document_date,   datetime.fromisoformat("2007-10-09T00:00:00"))
-            self.assertEqual(s.draft,           DocumentURI("/api/v1/doc/document/draft-crocker-rfc4234bis/"))
+            self.assertEqual(s.checks,          [SubmissionCheckURI(uri="/api/v1/submit/submissioncheck/386/")])
+            self.assertEqual(s.document_date,   date.fromisoformat("2007-10-09"))
+            self.assertEqual(s.draft,           DocumentURI(uri="/api/v1/doc/document/draft-crocker-rfc4234bis/"))
             self.assertEqual(s.file_size,       27651)
             self.assertEqual(s.file_types,      ".txt,.xml,.pdf")
             #self.assertEqual(s.first_two_pages, "\n\n\nNetwork Working Group...")
-            self.assertEqual(s.group,           GroupURI("/api/v1/group/group/1027/"))
+            self.assertEqual(s.group,           GroupURI(uri="/api/v1/group/group/1027/"))
             self.assertEqual(s.id,              2402)
             self.assertEqual(s.name,            "draft-crocker-rfc4234bis")
             self.assertEqual(s.note,            "")
             self.assertEqual(s.pages,           13)
             self.assertEqual(s.remote_ip,       "72.255.3.179")
             self.assertEqual(s.replaces,        "")
-            self.assertEqual(s.resource_uri,    SubmissionURI("/api/v1/submit/submission/2402/"))
+            self.assertEqual(s.resource_uri,    SubmissionURI(uri="/api/v1/submit/submission/2402/"))
             self.assertEqual(s.rev,             "01")
             self.assertEqual(s.state,           "/api/v1/name/draftsubmissionstatename/posted/")
-            self.assertEqual(s.submission_date, datetime.fromisoformat("2007-10-09T00:00:00"))
+            self.assertEqual(s.submission_date, date.fromisoformat("2007-10-09"))
             self.assertEqual(s.submitter,       "Dave Crocker")
             self.assertEqual(s.title,           "Augmented BNF for Syntax Specifications: ABNF")
             self.assertEqual(s.words,           None)
             self.assertEqual(s.xml_version,     None)
         else:
             self.fail("Cannot find submission")
 
 
     def test_submission_event(self) -> None:
-        e  = self.dt.submission_event(SubmissionEventURI("/api/v1/submit/submissionevent/188542/"))
+        e  = self.dt.submission_event(SubmissionEventURI(uri="/api/v1/submit/submissionevent/188542/"))
         if e is not None:
-            self.assertEqual(e.by,           PersonURI("/api/v1/person/person/115824/"))
+            self.assertEqual(e.by,           PersonURI(uri="/api/v1/person/person/115824/"))
             self.assertEqual(e.desc,         "Uploaded submission")
             self.assertEqual(e.id,           188542)
-            self.assertEqual(e.resource_uri, SubmissionEventURI("/api/v1/submit/submissionevent/188542/"))
-            self.assertEqual(e.submission,   SubmissionURI("/api/v1/submit/submission/111128/"))
+            self.assertEqual(e.resource_uri, SubmissionEventURI(uri="/api/v1/submit/submissionevent/188542/"))
+            self.assertEqual(e.submission,   SubmissionURI(uri="/api/v1/submit/submission/111128/"))
             self.assertEqual(e.time,         datetime.fromisoformat("2020-03-23T04:18:27-07:00"))
         else:
             self.fail("Cannot find submission event")
 
 
+    def test_document_url(self) -> None:
+        doc_url = self.dt.document_url(DocumentUrlURI(uri="/api/v1/doc/documenturl/4594/"))
+        if doc_url is not None:
+            self.assertEqual(doc_url.desc,         "")
+            self.assertEqual(doc_url.doc,          DocumentURI(uri="/api/v1/doc/document/draft-mcquistin-augmented-ascii-diagrams/"))
+            self.assertEqual(doc_url.id,           4594)
+            self.assertEqual(doc_url.resource_uri, DocumentUrlURI(uri="/api/v1/doc/documenturl/4594/"))
+            self.assertEqual(doc_url.tag,          DocumentUrlTagURI(uri="/api/v1/name/docurltagname/repository/"))
+            self.assertEqual(doc_url.url,          "https://github.com/glasgow-ipl/draft-mcquistin-augmented-ascii-diagrams")
+        else:
+            self.fail("Cannot find document URL")
+            
+            
+    def test_document_urls(self) -> None:
+        doc_urls = list(self.dt.document_urls(self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-mcquistin-augmented-ascii-diagrams/"))))
+        self.assertEqual(len(doc_urls),  1)
+        self.assertEqual(doc_urls[0].id, 4594)
+
+
     def test_document_type(self) -> None:
-        doctype = self.dt.document_type(DocumentTypeURI("/api/v1/name/doctypename/draft/"))
+        doctype = self.dt.document_type(DocumentTypeURI(uri="/api/v1/name/doctypename/draft/"))
         if doctype is not None:
-            self.assertEqual(doctype.resource_uri, DocumentTypeURI("/api/v1/name/doctypename/draft/"))
+            self.assertEqual(doctype.resource_uri, DocumentTypeURI(uri="/api/v1/name/doctypename/draft/"))
             self.assertEqual(doctype.name,         "Draft")
             self.assertEqual(doctype.used,         True)
             self.assertEqual(doctype.prefix,       "draft")
             self.assertEqual(doctype.slug,         "draft")
             self.assertEqual(doctype.desc,         "")
             self.assertEqual(doctype.order,        0)
         else:
             self.fail("Cannot find doctype")
 
 
     def test_document_type_from_slug(self) -> None:
         doctype = self.dt.document_type_from_slug("draft")
         if doctype is not None:
-            self.assertEqual(doctype.resource_uri, DocumentTypeURI("/api/v1/name/doctypename/draft/"))
+            self.assertEqual(doctype.resource_uri, DocumentTypeURI(uri="/api/v1/name/doctypename/draft/"))
             self.assertEqual(doctype.name,         "Draft")
             self.assertEqual(doctype.used,         True)
             self.assertEqual(doctype.prefix,       "draft")
             self.assertEqual(doctype.slug,         "draft")
             self.assertEqual(doctype.desc,         "")
             self.assertEqual(doctype.order,        0)
         else:
             self.fail("Cannot find doctype")
 
 
     def test_document_types(self) -> None:
         types = list(self.dt.document_types())
-        self.assertEqual(len(types), 18)
+        self.assertEqual(len(types), 23)
         self.assertEqual(types[ 0].slug, "agenda")
-        self.assertEqual(types[ 1].slug, "bluesheets")
-        self.assertEqual(types[ 2].slug, "bofreq")
-        self.assertEqual(types[ 3].slug, "charter")
-        self.assertEqual(types[ 4].slug, "chatlog")
-        self.assertEqual(types[ 5].slug, "conflrev")
-        self.assertEqual(types[ 6].slug, "draft")
-        self.assertEqual(types[ 7].slug, "liai-att")
-        self.assertEqual(types[ 8].slug, "liaison")
-        self.assertEqual(types[ 9].slug, "minutes")
-        self.assertEqual(types[10].slug, "polls")
-        self.assertEqual(types[11].slug, "procmaterials")
-        self.assertEqual(types[12].slug, "recording")
-        self.assertEqual(types[13].slug, "review")
-        self.assertEqual(types[14].slug, "shepwrit")
-        self.assertEqual(types[15].slug, "slides")
-        self.assertEqual(types[16].slug, "statchg")
-        self.assertEqual(types[17].slug, "statement")
+        self.assertEqual(types[ 1].slug, "bcp")
+        self.assertEqual(types[ 2].slug, "bluesheets")
+        self.assertEqual(types[ 3].slug, "bofreq")
+        self.assertEqual(types[ 4].slug, "charter")
+        self.assertEqual(types[ 5].slug, "chatlog")
+        self.assertEqual(types[ 6].slug, "conflrev")
+        self.assertEqual(types[ 7].slug, "draft")
+        self.assertEqual(types[ 8].slug, "fyi")
+        self.assertEqual(types[ 9].slug, "liai-att")
+        self.assertEqual(types[10].slug, "liaison")
+        self.assertEqual(types[11].slug, "minutes")
+        self.assertEqual(types[12].slug, "narrativeminutes")
+        self.assertEqual(types[13].slug, "polls")
+        self.assertEqual(types[14].slug, "procmaterials")
+        self.assertEqual(types[15].slug, "recording")
+        self.assertEqual(types[16].slug, "review")
+        self.assertEqual(types[17].slug, "rfc")
+        self.assertEqual(types[18].slug, "shepwrit")
+        self.assertEqual(types[19].slug, "slides")
+        self.assertEqual(types[20].slug, "statchg")
+        self.assertEqual(types[21].slug, "statement")
+        self.assertEqual(types[22].slug, "std")
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to streams:
 
     def test_stream(self) -> None:
-        stream = self.dt.stream(StreamURI("/api/v1/name/streamname/irtf/"))
+        stream = self.dt.stream(StreamURI(uri="/api/v1/name/streamname/irtf/"))
         if stream is not None:
             self.assertEqual(stream.desc,         "Internet Research Task Force (IRTF)")
             self.assertEqual(stream.name,         "IRTF")
             self.assertEqual(stream.order,        3)
-            self.assertEqual(stream.resource_uri, StreamURI("/api/v1/name/streamname/irtf/"))
+            self.assertEqual(stream.resource_uri, StreamURI(uri="/api/v1/name/streamname/irtf/"))
             self.assertEqual(stream.slug,         "irtf")
             self.assertEqual(stream.used,         True)
         else:
             self.fail("Cannot find stream")
 
 
     def test_stream_from_slug(self) -> None:
         stream = self.dt.stream_from_slug("irtf")
         if stream is not None:
             self.assertEqual(stream.desc,         "Internet Research Task Force (IRTF)")
             self.assertEqual(stream.name,         "IRTF")
             self.assertEqual(stream.order,        3)
-            self.assertEqual(stream.resource_uri, StreamURI("/api/v1/name/streamname/irtf/"))
+            self.assertEqual(stream.resource_uri, StreamURI(uri="/api/v1/name/streamname/irtf/"))
             self.assertEqual(stream.slug,         "irtf")
             self.assertEqual(stream.used,         True)
         else:
             self.fail("Cannot find stream")
 
 
     def test_streams(self) -> None:
@@ -1376,31 +1441,31 @@
         self.assertEqual(streams[ 5].slug, "legacy")
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to groups:
 
     # FIXME: this needs to be updated
     def test_group(self) -> None:
-        group = self.dt.group(GroupURI("/api/v1/group/group/941/"))
+        group = self.dt.group(GroupURI(uri="/api/v1/group/group/941/"))
         if group is not None:
             self.assertEqual(group.acronym,        "avt")
             self.assertEqual(group.ad,             None)
-            self.assertEqual(group.charter,        DocumentURI("/api/v1/doc/document/charter-ietf-avt/"))
+            self.assertEqual(group.charter,        DocumentURI(uri="/api/v1/doc/document/charter-ietf-avt/"))
             self.assertEqual(group.comments,       "")
             self.assertEqual(group.description,    "\n  The Audio/Video Transport Working Group was formed to specify a protocol \n  for real-time transmission of audio and video over unicast and multicast \n  UDP/IP. This is the Real-time Transport Protocol, RTP, along with its \n  associated profiles and payload formats.")
             self.assertEqual(group.id,             941)
-            self.assertEqual(group.list_archive,   "https://mailarchive.ietf.org/arch/search/?email_list=avt")
+            self.assertEqual(group.list_archive,   "https://mailarchive.ietf.org/arch/browse/avt")
             self.assertEqual(group.list_email,     "avt@ietf.org")
             self.assertEqual(group.list_subscribe, "https://www.ietf.org/mailman/listinfo/avt")
             self.assertEqual(group.name,           "Audio/Video Transport")
-            self.assertEqual(group.parent,         GroupURI("/api/v1/group/group/1683/"))
-            self.assertEqual(group.resource_uri,   GroupURI("/api/v1/group/group/941/"))
-            self.assertEqual(group.state,          GroupStateURI("/api/v1/name/groupstatename/conclude/"))
+            self.assertEqual(group.parent,         GroupURI(uri="/api/v1/group/group/1683/"))
+            self.assertEqual(group.resource_uri,   GroupURI(uri="/api/v1/group/group/941/"))
+            self.assertEqual(group.state,          GroupStateURI(uri="/api/v1/name/groupstatename/conclude/"))
             self.assertEqual(group.time,           datetime.fromisoformat("2011-12-09T12:00:00-08:00"))
-            self.assertEqual(group.type,           GroupTypeNameURI("/api/v1/name/grouptypename/wg/"))
+            self.assertEqual(group.type,           GroupTypeNameURI(uri="/api/v1/name/grouptypename/wg/"))
             self.assertEqual(group.unused_states,  [])
             self.assertEqual(group.unused_tags,    [])
             self.assertEqual(group.meeting_seen_as_area, False)
             self.assertEqual(group.used_roles,           "[]")
             self.assertEqual(group.uses_milestone_dates, True)
         else:
             self.fail("Cannot find group")
@@ -1430,31 +1495,31 @@
         self.assertEqual(groups[0].id,    3)  # IRTF
         self.assertEqual(groups[1].id, 1853)  # IRTF Open Meeting
         self.assertEqual(groups[2].id, 2282)  # ACM/IRTF Applied Networking Research Workshop
         self.assertEqual(groups[3].id, 2372)  # IAB/IRTF Workshop on Congestion Control for Interactive Real-Time Communication
 
 
     def test_group_history(self) -> None:
-        group_history = self.dt.group_history(GroupHistoryURI("/api/v1/group/grouphistory/4042/"))
+        group_history = self.dt.group_history(GroupHistoryURI(uri="/api/v1/group/grouphistory/4042/"))
         if group_history is not None:
             self.assertEqual(group_history.acronym,              "git")
             self.assertEqual(group_history.ad,                   None)
             self.assertEqual(group_history.comments,             "")
             self.assertEqual(group_history.description,          "")
-            self.assertEqual(group_history.group,                GroupURI("/api/v1/group/group/2233/"))
+            self.assertEqual(group_history.group,                GroupURI(uri="/api/v1/group/group/2233/"))
             self.assertEqual(group_history.id,                   4042)
             self.assertEqual(group_history.list_archive,         "https://mailarchive.ietf.org/arch/browse/ietf-and-github/")
             self.assertEqual(group_history.list_email,           "ietf-and-github@ietf.org")
             self.assertEqual(group_history.list_subscribe,       "https://www.ietf.org/mailman/listinfo/ietf-and-github")
             self.assertEqual(group_history.name,                 "GitHub Integration and Tooling")
-            self.assertEqual(group_history.parent,               GroupURI("/api/v1/group/group/1008/"))
-            self.assertEqual(group_history.resource_uri,         GroupHistoryURI("/api/v1/group/grouphistory/4042/"))
-            self.assertEqual(group_history.state,                GroupStateURI("/api/v1/name/groupstatename/active/"))
+            self.assertEqual(group_history.parent,               GroupURI(uri="/api/v1/group/group/1008/"))
+            self.assertEqual(group_history.resource_uri,         GroupHistoryURI(uri="/api/v1/group/grouphistory/4042/"))
+            self.assertEqual(group_history.state,                GroupStateURI(uri="/api/v1/name/groupstatename/active/"))
             self.assertEqual(group_history.time,                 datetime.fromisoformat("2019-02-08T14:07:27-08:00"))
-            self.assertEqual(group_history.type,                 GroupTypeNameURI("/api/v1/name/grouptypename/wg/"))
+            self.assertEqual(group_history.type,                 GroupTypeNameURI(uri="/api/v1/name/grouptypename/wg/"))
             self.assertEqual(group_history.unused_states,        [])
             self.assertEqual(group_history.unused_tags,          [])
             self.assertEqual(group_history.meeting_seen_as_area, False)
             self.assertEqual(group_history.used_roles,           "[]")
             self.assertEqual(group_history.uses_milestone_dates, True)
         else:
             self.fail("Cannot find group history")
@@ -1472,66 +1537,66 @@
         group_histories = list(self.dt.group_histories(group=avt))
         self.assertEqual(len(group_histories), 2)
         self.assertEqual(group_histories[0].id, 2179)
         self.assertEqual(group_histories[1].id, 2257)
 
 
     def test_group_event(self) -> None:
-        group_event = self.dt.group_event(GroupEventURI("/api/v1/group/groupevent/16849/"))
+        group_event = self.dt.group_event(GroupEventURI(uri="/api/v1/group/groupevent/16849/"))
         if group_event is not None:
-            self.assertEqual(group_event.by,           PersonURI("/api/v1/person/person/108756/"))
+            self.assertEqual(group_event.by,           PersonURI(uri="/api/v1/person/person/108756/"))
             self.assertEqual(group_event.desc,         "Added milestone \"Submit data flow information model (informational)\", due 2020-04-30, from approved charter")
-            self.assertEqual(group_event.group,        GroupURI("/api/v1/group/group/1962/"))
+            self.assertEqual(group_event.group,        GroupURI(uri="/api/v1/group/group/1962/"))
             self.assertEqual(group_event.id,           16849)
-            self.assertEqual(group_event.resource_uri, GroupEventURI("/api/v1/group/groupevent/16849/"))
+            self.assertEqual(group_event.resource_uri, GroupEventURI(uri="/api/v1/group/groupevent/16849/"))
             self.assertEqual(group_event.time,         datetime.fromisoformat("2020-04-20T13:31:48-07:00"))
             self.assertEqual(group_event.type,         "changed_milestone")
         else:
             self.fail("Cannot find group event")
 
 
     def test_group_events_by(self) -> None:
-        group_events_by = self.dt.group_events(by=self.dt.person(PersonURI("/api/v1/person/person/108756/")))
+        group_events_by = self.dt.group_events(by=self.dt.person(PersonURI(uri="/api/v1/person/person/108756/")))
         self.assertIsNot(group_events_by, None)
 
 
     def test_group_events_group(self) -> None:
-        group_events_group = list(self.dt.group_events(group=self.dt.group(GroupURI("/api/v1/group/group/1997/"))))
+        group_events_group = list(self.dt.group_events(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1997/"))))
         self.assertEqual(len(group_events_group),  4)
         self.assertEqual(group_events_group[0].id, 8975)
         self.assertEqual(group_events_group[1].id, 9151)
         self.assertEqual(group_events_group[2].id, 9585)
         self.assertEqual(group_events_group[3].id, 9652)
 
 
     def test_group_events_type(self) -> None:
         group_events_type = self.dt.group_events(type="changed_state")
         self.assertIsNot(group_events_type, None)
 
 
     def test_group_url(self) -> None:
-        group_url = self.dt.group_url(GroupUrlURI("/api/v1/group/groupurl/1/"))
+        group_url = self.dt.group_url(GroupUrlURI(uri="/api/v1/group/groupurl/1/"))
         if group_url is not None:
-            self.assertEqual(group_url.group,        GroupURI("/api/v1/group/group/934/"))
+            self.assertEqual(group_url.group,        GroupURI(uri="/api/v1/group/group/934/"))
             self.assertEqual(group_url.id,           1)
             self.assertEqual(group_url.name,         "Applications Area Web Page")
-            self.assertEqual(group_url.resource_uri, GroupUrlURI("/api/v1/group/groupurl/1/"))
+            self.assertEqual(group_url.resource_uri, GroupUrlURI(uri="/api/v1/group/groupurl/1/"))
             self.assertEqual(group_url.url,          "http://www.apps.ietf.org/")
         else:
             self.fail("Cannot find group URL")
 
 
     def test_group_urls(self) -> None:
-        group_urls = list(self.dt.group_urls(self.dt.group(GroupURI("/api/v1/group/group/1062/"))))
+        group_urls = list(self.dt.group_urls(self.dt.group(GroupURI(uri="/api/v1/group/group/1062/"))))
         self.assertEqual(len(group_urls),  1)
         self.assertEqual(group_urls[0].id, 20)
 
 
     def test_group_milestone_statename(self) -> None:
-        group_milestone_statename = self.dt.group_milestone_statename(GroupMilestoneStateNameURI("/api/v1/name/groupmilestonestatename/active/"))
+        group_milestone_statename = self.dt.group_milestone_statename(GroupMilestoneStateNameURI(uri="/api/v1/name/groupmilestonestatename/active/"))
         if group_milestone_statename is not None:
             self.assertEqual(group_milestone_statename.desc,  "")
             self.assertEqual(group_milestone_statename.order, 1)
             self.assertEqual(group_milestone_statename.slug,  "active")
             self.assertEqual(group_milestone_statename.used,  True)
         else:
             self.fail("Cannot find group milestone state name")
@@ -1543,76 +1608,76 @@
         self.assertEqual(group_milestone_statenames[0].slug, "active")
         self.assertEqual(group_milestone_statenames[1].slug, "charter")
         self.assertEqual(group_milestone_statenames[2].slug, "deleted")
         self.assertEqual(group_milestone_statenames[3].slug, "review")
 
 
     def test_group_milestone(self) -> None:
-        group_milestone = self.dt.group_milestone(GroupMilestoneURI("/api/v1/group/groupmilestone/1520/"))
+        group_milestone = self.dt.group_milestone(GroupMilestoneURI(uri="/api/v1/group/groupmilestone/1520/"))
         if group_milestone is not None:
             self.assertEqual(group_milestone.desc,         "Define a protocol for the link and IP layer.")
             self.assertEqual(group_milestone.docs,         [])
             self.assertEqual(group_milestone.due,          "1988-03-31")
-            self.assertEqual(group_milestone.group,        GroupURI("/api/v1/group/group/1209/"))
+            self.assertEqual(group_milestone.group,        GroupURI(uri="/api/v1/group/group/1209/"))
             self.assertEqual(group_milestone.id,           1520)
             self.assertEqual(group_milestone.order,        None)
             self.assertEqual(group_milestone.resolved,     "")
-            self.assertEqual(group_milestone.resource_uri, GroupMilestoneURI("/api/v1/group/groupmilestone/1520/"))
-            self.assertEqual(group_milestone.state,        GroupMilestoneStateNameURI("/api/v1/name/groupmilestonestatename/active/"))
+            self.assertEqual(group_milestone.resource_uri, GroupMilestoneURI(uri="/api/v1/group/groupmilestone/1520/"))
+            self.assertEqual(group_milestone.state,        GroupMilestoneStateNameURI(uri="/api/v1/name/groupmilestonestatename/active/"))
             self.assertEqual(group_milestone.time,         datetime.fromisoformat("2012-02-26T00:21:52-08:00"))
         else:
             self.fail("Cannot find group milestone")
 
 
     def test_group_milestones(self) -> None:
         group_milestones = self.dt.group_milestones()
         self.assertIsNot(group_milestones, None)
 
 
     def test_group_milestones_group(self) -> None:
-        group_milestones = list(self.dt.group_milestones(group=self.dt.group(GroupURI("/api/v1/group/group/1209/"))))
+        group_milestones = list(self.dt.group_milestones(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1209/"))))
         self.assertEqual(len(group_milestones),  1)
         self.assertEqual(group_milestones[0].id, 1520)
         self.assertIsNot(group_milestones, None)
 
 
     def test_group_milestones_state(self) -> None:
-        group_milestones = self.dt.group_milestones(state=self.dt.group_milestone_statename(GroupMilestoneStateNameURI("/api/v1/name/groupmilestonestatename/active/")))
+        group_milestones = self.dt.group_milestones(state=self.dt.group_milestone_statename(GroupMilestoneStateNameURI(uri="/api/v1/name/groupmilestonestatename/active/")))
         self.assertIsNot(group_milestones, None)
 
 
     def test_role_name(self) -> None:
-        role_name = self.dt.role_name(RoleNameURI("/api/v1/name/rolename/ceo/"))
+        role_name = self.dt.role_name(RoleNameURI(uri="/api/v1/name/rolename/ceo/"))
         if role_name is not None:
             self.assertEqual(role_name.desc,         "")
             self.assertEqual(role_name.name,         "CEO")
             self.assertEqual(role_name.order,        0)
-            self.assertEqual(role_name.resource_uri, RoleNameURI("/api/v1/name/rolename/ceo/"))
+            self.assertEqual(role_name.resource_uri, RoleNameURI(uri="/api/v1/name/rolename/ceo/"))
             self.assertEqual(role_name.slug,         "ceo")
             self.assertEqual(role_name.used,         True)
         else:
             self.fail("Cannot find role name")
 
 
     def test_role_name_from_slug(self) -> None:
         role_name = self.dt.role_name_from_slug("ceo")
         if role_name is not None:
             self.assertEqual(role_name.desc,         "")
             self.assertEqual(role_name.name,         "CEO")
             self.assertEqual(role_name.order,        0)
-            self.assertEqual(role_name.resource_uri, RoleNameURI("/api/v1/name/rolename/ceo/"))
+            self.assertEqual(role_name.resource_uri, RoleNameURI(uri="/api/v1/name/rolename/ceo/"))
             self.assertEqual(role_name.slug,         "ceo")
             self.assertEqual(role_name.used,         True)
         else:
             self.fail("Cannot find role name")
 
 
     def test_role_names(self) -> None:
         role_names = list(self.dt.role_names())
-        self.assertEqual(len(role_names), 34)
+        self.assertEqual(len(role_names), 35)
         self.assertEqual(role_names[ 0].slug, "ad")
         self.assertEqual(role_names[ 1].slug, "admdir")
         self.assertEqual(role_names[ 2].slug, "advisor")
         self.assertEqual(role_names[ 3].slug, "announce")
         self.assertEqual(role_names[ 4].slug, "atlarge")
         self.assertEqual(role_names[ 5].slug, "auth")
         self.assertEqual(role_names[ 6].slug, "ceo")
@@ -1621,43 +1686,44 @@
         self.assertEqual(role_names[ 9].slug, "coord")
         self.assertEqual(role_names[10].slug, "delegate")
         self.assertEqual(role_names[11].slug, "devdir")
         self.assertEqual(role_names[12].slug, "editor")
         self.assertEqual(role_names[13].slug, "execdir")
         self.assertEqual(role_names[14].slug, "exofficio")
         self.assertEqual(role_names[15].slug, "lead")
-        self.assertEqual(role_names[16].slug, "liaiman")
-        self.assertEqual(role_names[17].slug, "liaison")
-        self.assertEqual(role_names[18].slug, "liaison_cc_contact")
-        self.assertEqual(role_names[19].slug, "liaison_contact")
-        self.assertEqual(role_names[20].slug, "matman")
-        self.assertEqual(role_names[21].slug, "member")
-        self.assertEqual(role_names[22].slug, "pre-ad")
-        self.assertEqual(role_names[23].slug, "recman")
-        self.assertEqual(role_names[24].slug, "reviewer")
-        self.assertEqual(role_names[25].slug, "robot")
-        self.assertEqual(role_names[26].slug, "secr")
-        self.assertEqual(role_names[27].slug, "techadv")
-        self.assertEqual(role_names[28].slug, "trac-admin")
-        self.assertEqual(role_names[29].slug, "trac-editor")
-        self.assertEqual(role_names[30].slug, "wikiadmin")
-        self.assertEqual(role_names[31].slug, "wikiman")
-        self.assertEqual(role_names[32].slug, "yc_admin")
-        self.assertEqual(role_names[33].slug, "yc_operator")
+        self.assertEqual(role_names[16].slug, "leadmaintainer")
+        self.assertEqual(role_names[17].slug, "liaiman")
+        self.assertEqual(role_names[18].slug, "liaison")
+        self.assertEqual(role_names[19].slug, "liaison_cc_contact")
+        self.assertEqual(role_names[20].slug, "liaison_contact")
+        self.assertEqual(role_names[21].slug, "matman")
+        self.assertEqual(role_names[22].slug, "member")
+        self.assertEqual(role_names[23].slug, "pre-ad")
+        self.assertEqual(role_names[24].slug, "recman")
+        self.assertEqual(role_names[25].slug, "reviewer")
+        self.assertEqual(role_names[26].slug, "robot")
+        self.assertEqual(role_names[27].slug, "secr")
+        self.assertEqual(role_names[28].slug, "techadv")
+        self.assertEqual(role_names[29].slug, "trac-admin")
+        self.assertEqual(role_names[30].slug, "trac-editor")
+        self.assertEqual(role_names[31].slug, "wikiadmin")
+        self.assertEqual(role_names[32].slug, "wikiman")
+        self.assertEqual(role_names[33].slug, "yc_admin")
+        self.assertEqual(role_names[34].slug, "yc_operator")
 
 
 
     def test_group_role(self) -> None:
-        group_role = self.dt.group_role(GroupRoleURI("/api/v1/group/role/1076/"))
+        group_role = self.dt.group_role(GroupRoleURI(uri="/api/v1/group/role/1076/"))
         if group_role is not None:
-            self.assertEqual(group_role.email,  EmailURI("/api/v1/person/email/csp@csperkins.org/"))
-            self.assertEqual(group_role.group,  GroupURI("/api/v1/group/group/1727/"))
+            self.assertEqual(group_role.email,  EmailURI(uri="/api/v1/person/email/csp@csperkins.org/"))
+            self.assertEqual(group_role.group,  GroupURI(uri="/api/v1/group/group/1727/"))
             self.assertEqual(group_role.id,     1076)
-            self.assertEqual(group_role.name,   RoleNameURI("/api/v1/name/rolename/chair/"))
-            self.assertEqual(group_role.person, PersonURI("/api/v1/person/person/20209/"))
+            self.assertEqual(group_role.name,   RoleNameURI(uri="/api/v1/name/rolename/chair/"))
+            self.assertEqual(group_role.person, PersonURI(uri="/api/v1/person/person/20209/"))
         else:
             self.fail("Cannot find group role")
 
 
     def test_group_roles(self) -> None:
         group_roles = self.dt.group_roles()
         self.assertIsNot(group_roles, None)
@@ -1666,221 +1732,221 @@
     def test_group_roles_email(self) -> None:
         group_roles = list(self.dt.group_roles(email="csp@csperkins.org"))
         self.assertEqual(len(group_roles), 12)
         self.assertEqual(group_roles[0].id, 1076)   # SAFE BoF chair
         self.assertEqual(group_roles[1].id, 3998)   # TSV DIR reviewer
         self.assertEqual(group_roles[2].id, 8464)   # IRSG chair
         self.assertEqual(group_roles[3].id, 8465)   # IRTF Open Meeting chair
-        self.assertEqual(group_roles[4].id, 8466)   # IRTF chair
+        self.assertEqual(group_roles[4].id, 8466)   # IRTF chair
         self.assertEqual(group_roles[5].id, 9355)   # RMCAT chair
         self.assertEqual(group_roles[6].id, 10200)  # IAB EDM programme member
         self.assertEqual(group_roles[7].id, 11103)  # TSV ART reviewer
         self.assertEqual(group_roles[8].id, 11680)  # IRTF ANRW chair
         self.assertEqual(group_roles[9].id, 12875)  # RSAB member
         self.assertEqual(group_roles[10].id, 12915) # IAB-ISOC Policy Coordination
         self.assertEqual(group_roles[11].id, 13098) # IAB E-Impact workshop
 
 
     def test_group_roles_group(self) -> None:
-        group_roles = list(self.dt.group_roles(group=self.dt.group(GroupURI("/api/v1/group/group/1997/")))) # SPUD BoF
+        group_roles = list(self.dt.group_roles(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1997/")))) # SPUD BoF
         self.assertEqual(len(group_roles), 3)
         self.assertEqual(group_roles[0].id, 3036)   # AD is Spencer Dawkins
         self.assertEqual(group_roles[1].id, 3037)   # Chair is Eliot Lear
         self.assertEqual(group_roles[2].id, 3038)   # Chair is Mirja Kühlewind
 
 
     def test_group_roles_group_name(self) -> None:
         iab   = self.dt.group_from_acronym("iab")
         chair = self.dt.role_name_from_slug("chair")
         group_roles = list(self.dt.group_roles(group = iab, name = chair))
         self.assertEqual(len(group_roles), 1)
-        self.assertEqual(group_roles[0].id, 9605)   # IAB chair is Mirja Kühlewind
+        self.assertEqual(group_roles[0].id, 13626)   # IAB chair is Tommy Pauley
 
 
 
     def test_group_roles_name(self) -> None:
-        group_roles = self.dt.group_roles(name=self.dt.role_name(RoleNameURI("/api/v1/name/rolename/chair/")))
+        group_roles = self.dt.group_roles(name=self.dt.role_name(RoleNameURI(uri="/api/v1/name/rolename/chair/")))
         self.assertIsNot(group_roles, None)
 
 
     def test_group_roles_person(self) -> None:
-        group_roles = list(self.dt.group_roles(person=self.dt.person(PersonURI("/api/v1/person/person/20209/"))))
+        group_roles = list(self.dt.group_roles(person=self.dt.person(PersonURI(uri="/api/v1/person/person/20209/"))))
         self.assertEqual(len(group_roles), 12)
         self.assertEqual(group_roles[0].id, 1076)   # SAFE BoF chair
         self.assertEqual(group_roles[1].id, 3998)   # TSV DIR reviewer
         self.assertEqual(group_roles[2].id, 8464)   # IRSG chair
         self.assertEqual(group_roles[3].id, 8465)   # IRTF Open Meeting chair
-        self.assertEqual(group_roles[4].id, 8466)   # IRTF chair
+        self.assertEqual(group_roles[4].id, 8466)   # IRTF chair
         self.assertEqual(group_roles[5].id, 9355)   # RMCAT chair
         self.assertEqual(group_roles[6].id, 10200)  # IAB EDM programme member
         self.assertEqual(group_roles[7].id, 11103)  # TSV ART reviewer
         self.assertEqual(group_roles[8].id, 11680)  # IRTF ANRW chair
         self.assertEqual(group_roles[9].id, 12875) # RSAB member
         self.assertEqual(group_roles[10].id, 12915) # IAB-ISOC Policy Coordination
         self.assertEqual(group_roles[11].id, 13098) # IAB E-Impact workshop
 
 
     def test_group_milestone_history(self) -> None:
-        group_milestone_history = self.dt.group_milestone_history(GroupMilestoneHistoryURI("/api/v1/group/groupmilestonehistory/1433/"))
+        group_milestone_history = self.dt.group_milestone_history(GroupMilestoneHistoryURI(uri="/api/v1/group/groupmilestonehistory/1433/"))
         if group_milestone_history is not None:
             self.assertEqual(group_milestone_history.desc,         "Agreement on charter and issues in current draft.")
             self.assertEqual(group_milestone_history.docs,         [])
             self.assertEqual(group_milestone_history.due,          "1996-05-31")
-            self.assertEqual(group_milestone_history.group,        GroupURI("/api/v1/group/group/1326/"))
+            self.assertEqual(group_milestone_history.group,        GroupURI(uri="/api/v1/group/group/1326/"))
             self.assertEqual(group_milestone_history.id,           1433)
-            self.assertEqual(group_milestone_history.milestone,    GroupMilestoneURI("/api/v1/group/groupmilestone/2114/"))
+            self.assertEqual(group_milestone_history.milestone,    GroupMilestoneURI(uri="/api/v1/group/groupmilestone/2114/"))
             self.assertEqual(group_milestone_history.order,        None)
             self.assertEqual(group_milestone_history.resolved,     "Done")
-            self.assertEqual(group_milestone_history.resource_uri, GroupMilestoneHistoryURI("/api/v1/group/groupmilestonehistory/1433/"))
-            self.assertEqual(group_milestone_history.state,        GroupMilestoneStateNameURI("/api/v1/name/groupmilestonestatename/active/"))
+            self.assertEqual(group_milestone_history.resource_uri, GroupMilestoneHistoryURI(uri="/api/v1/group/groupmilestonehistory/1433/"))
+            self.assertEqual(group_milestone_history.state,        GroupMilestoneStateNameURI(uri="/api/v1/name/groupmilestonestatename/active/"))
             self.assertEqual(group_milestone_history.time,         datetime.fromisoformat("2013-05-20T15:42:45-07:00"))
         else:
             self.fail("Cannot find group milestone history")
 
 
     def test_group_milestone_histories(self) -> None:
         group_milestone_histories = self.dt.group_milestone_histories()
         self.assertIsNot(group_milestone_histories, None)
 
 
     def test_group_milestone_histories_group(self) -> None:
-        group_milestone_histories = list(self.dt.group_milestone_histories(group=self.dt.group(GroupURI("/api/v1/group/group/1326/"))))
+        group_milestone_histories = list(self.dt.group_milestone_histories(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1326/"))))
         self.assertEqual(len(group_milestone_histories), 40)
 
 
     def test_group_milestone_histories_milestone(self) -> None:
-        group_milestone_histories = list(self.dt.group_milestone_histories(milestone=self.dt.group_milestone(GroupMilestoneURI("/api/v1/group/groupmilestone/2114/"))))
+        group_milestone_histories = list(self.dt.group_milestone_histories(milestone=self.dt.group_milestone(GroupMilestoneURI(uri="/api/v1/group/groupmilestone/2114/"))))
         self.assertEqual(len(group_milestone_histories),  1)
         self.assertEqual(group_milestone_histories[0].id, 1433)
 
 
     def test_group_milestone_histories_state(self) -> None:
-        group_milestone_histories = self.dt.group_milestone_histories(state=self.dt.group_milestone_statename(GroupMilestoneStateNameURI("/api/v1/name/groupmilestonestatename/active/")))
+        group_milestone_histories = self.dt.group_milestone_histories(state=self.dt.group_milestone_statename(GroupMilestoneStateNameURI(uri="/api/v1/name/groupmilestonestatename/active/")))
         self.assertIsNot(group_milestone_histories, None)
 
 
     def test_group_milestone_event(self) -> None:
-        group_milestone_event = self.dt.group_milestone_event(GroupMilestoneEventURI("/api/v1/group/milestonegroupevent/16849/"))
+        group_milestone_event = self.dt.group_milestone_event(GroupMilestoneEventURI(uri="/api/v1/group/milestonegroupevent/16849/"))
         if group_milestone_event is not None:
-            self.assertEqual(group_milestone_event.by,             PersonURI("/api/v1/person/person/108756/"))
+            self.assertEqual(group_milestone_event.by,             PersonURI(uri="/api/v1/person/person/108756/"))
             self.assertEqual(group_milestone_event.desc,           "Added milestone \"Submit data flow information model (informational)\", due 2020-04-30, from approved charter")
-            self.assertEqual(group_milestone_event.group,          GroupURI("/api/v1/group/group/1962/"))
-            self.assertEqual(group_milestone_event.groupevent_ptr, GroupEventURI("/api/v1/group/groupevent/16849/"))
+            self.assertEqual(group_milestone_event.group,          GroupURI(uri="/api/v1/group/group/1962/"))
+            self.assertEqual(group_milestone_event.groupevent_ptr, GroupEventURI(uri="/api/v1/group/groupevent/16849/"))
             self.assertEqual(group_milestone_event.id,             16849)
-            self.assertEqual(group_milestone_event.milestone,      GroupMilestoneURI("/api/v1/group/groupmilestone/8539/"))
-            self.assertEqual(group_milestone_event.resource_uri,   GroupMilestoneEventURI("/api/v1/group/milestonegroupevent/16849/"))
+            self.assertEqual(group_milestone_event.milestone,      GroupMilestoneURI(uri="/api/v1/group/groupmilestone/8539/"))
+            self.assertEqual(group_milestone_event.resource_uri,   GroupMilestoneEventURI(uri="/api/v1/group/milestonegroupevent/16849/"))
             self.assertEqual(group_milestone_event.time,           datetime.fromisoformat("2020-04-20T13:31:48-07:00"))
             self.assertEqual(group_milestone_event.type,           "changed_milestone")
         else:
             self.fail("Cannot find group milestone event")
 
 
     def test_group_milestone_events(self) -> None:
         group_milestone_events = self.dt.group_milestone_events()
         self.assertIsNot(group_milestone_events, None)
 
 
     def test_group_milestone_events_by(self) -> None:
-        group_milestone_events = self.dt.group_milestone_events(by=self.dt.person(PersonURI("/api/v1/person/person/108756/")))
+        group_milestone_events = self.dt.group_milestone_events(by=self.dt.person(PersonURI(uri="/api/v1/person/person/108756/")))
         self.assertIsNot(group_milestone_events, None)
 
 
     def test_group_milestone_events_group(self) -> None:
-        group_milestone_events = list(self.dt.group_milestone_events(group=self.dt.group(GroupURI("/api/v1/group/group/1326/"))))
+        group_milestone_events = list(self.dt.group_milestone_events(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1326/"))))
         self.assertEqual(len(group_milestone_events), 51)
 
 
     def test_group_milestone_events_milestone(self) -> None:
-        group_milestone_events = list(self.dt.group_milestone_events(milestone=self.dt.group_milestone(GroupMilestoneURI("/api/v1/group/groupmilestone/6489/"))))
+        group_milestone_events = list(self.dt.group_milestone_events(milestone=self.dt.group_milestone(GroupMilestoneURI(uri="/api/v1/group/groupmilestone/6489/"))))
         self.assertEqual(len(group_milestone_events),  3)
         self.assertEqual(group_milestone_events[0].id, 7224)
         self.assertEqual(group_milestone_events[1].id, 11947)
         self.assertEqual(group_milestone_events[2].id, 16331)
 
 
     def test_group_milestone_events_type(self) -> None:
         group_milestone_events = self.dt.group_milestone_events(type="changed_milestone")
         self.assertIsNot(group_milestone_events, None)
 
 
     def test_group_role_history(self) -> None:
-        group_role_history = self.dt.group_role_history(GroupRoleHistoryURI("/api/v1/group/rolehistory/519/"))
+        group_role_history = self.dt.group_role_history(GroupRoleHistoryURI(uri="/api/v1/group/rolehistory/519/"))
         if group_role_history is not None:
-            self.assertEqual(group_role_history.email,        EmailURI("/api/v1/person/email/csp@csperkins.org/"))
-            self.assertEqual(group_role_history.group,        GroupHistoryURI("/api/v1/group/grouphistory/256/"))
+            self.assertEqual(group_role_history.email,        EmailURI(uri="/api/v1/person/email/csp@csperkins.org/"))
+            self.assertEqual(group_role_history.group,        GroupHistoryURI(uri="/api/v1/group/grouphistory/256/"))
             self.assertEqual(group_role_history.id,           519)
-            self.assertEqual(group_role_history.name,         RoleNameURI("/api/v1/name/rolename/chair/"))
-            self.assertEqual(group_role_history.person,       PersonURI("/api/v1/person/person/20209/"))
-            self.assertEqual(group_role_history.resource_uri, GroupRoleHistoryURI("/api/v1/group/rolehistory/519/"))
+            self.assertEqual(group_role_history.name,         RoleNameURI(uri="/api/v1/name/rolename/chair/"))
+            self.assertEqual(group_role_history.person,       PersonURI(uri="/api/v1/person/person/20209/"))
+            self.assertEqual(group_role_history.resource_uri, GroupRoleHistoryURI(uri="/api/v1/group/rolehistory/519/"))
         else:
             self.fail("Cannot find group role history")
 
 
     def test_group_role_histories(self) -> None:
         group_role_histories = self.dt.group_role_histories()
         self.assertIsNot(group_role_histories, None)
 
 
     def test_group_role_histories_email(self) -> None:
         group_role_histories = list(self.dt.group_role_histories(email="csp@csperkins.org"))
-        self.assertEqual(len(group_role_histories), 71)
+        self.assertEqual(len(group_role_histories), 84)
 
 
     def test_group_role_histories_group(self) -> None:
-        group_role_histories = list(self.dt.group_role_histories(group=self.dt.group_history(GroupHistoryURI("/api/v1/group/grouphistory/256/"))))
+        group_role_histories = list(self.dt.group_role_histories(group=self.dt.group_history(GroupHistoryURI(uri="/api/v1/group/grouphistory/256/"))))
         self.assertEqual(len(group_role_histories), 1)
         self.assertEqual(group_role_histories[0].id, 519)
 
 
     def test_group_role_histories_name(self) -> None:
-        group_role_histories = self.dt.group_role_histories(name=self.dt.role_name(RoleNameURI("/api/v1/name/rolename/chair/")))
+        group_role_histories = self.dt.group_role_histories(name=self.dt.role_name(RoleNameURI(uri="/api/v1/name/rolename/chair/")))
         self.assertIsNot(group_role_histories, None)
 
 
     def test_group_role_histories_person(self) -> None:
-        group_role_histories = list(self.dt.group_role_histories(person=self.dt.person(PersonURI("/api/v1/person/person/20209/"))))
-        self.assertEqual(len(group_role_histories), 71)
+        group_role_histories = list(self.dt.group_role_histories(person=self.dt.person(PersonURI(uri="/api/v1/person/person/20209/"))))
+        self.assertEqual(len(group_role_histories), 84)
 
 
     def test_group_state_change_event(self) -> None:
-        group_state_change_event = self.dt.group_state_change_event(GroupStateChangeEventURI("/api/v1/group/changestategroupevent/16833/"))
+        group_state_change_event = self.dt.group_state_change_event(GroupStateChangeEventURI(uri="/api/v1/group/changestategroupevent/16833/"))
         if group_state_change_event is not None:
-            self.assertEqual(group_state_change_event.by,             PersonURI("/api/v1/person/person/106842/"))
+            self.assertEqual(group_state_change_event.by,             PersonURI(uri="/api/v1/person/person/106842/"))
             self.assertEqual(group_state_change_event.desc,           "State changed to <b>Proposed</b> from Unknown")
-            self.assertEqual(group_state_change_event.group,          GroupURI("/api/v1/group/group/2273/"))
-            self.assertEqual(group_state_change_event.groupevent_ptr, GroupEventURI("/api/v1/group/groupevent/16833/"))
+            self.assertEqual(group_state_change_event.group,          GroupURI(uri="/api/v1/group/group/2273/"))
+            self.assertEqual(group_state_change_event.groupevent_ptr, GroupEventURI(uri="/api/v1/group/groupevent/16833/"))
             self.assertEqual(group_state_change_event.id,             16833)
-            self.assertEqual(group_state_change_event.resource_uri,   GroupStateChangeEventURI("/api/v1/group/changestategroupevent/16833/"))
-            self.assertEqual(group_state_change_event.state,          GroupStateURI("/api/v1/name/groupstatename/proposed/"))
+            self.assertEqual(group_state_change_event.resource_uri,   GroupStateChangeEventURI(uri="/api/v1/group/changestategroupevent/16833/"))
+            self.assertEqual(group_state_change_event.state,          GroupStateURI(uri="/api/v1/name/groupstatename/proposed/"))
             self.assertEqual(group_state_change_event.time,           datetime.fromisoformat("2020-04-14T14:52:24-07:00"))
             self.assertEqual(group_state_change_event.type,           "changed_state")
         else:
             self.fail("Cannot find group state change event")
 
     def test_group_state_change_events(self) -> None:
         group_state_change_events = self.dt.group_state_change_events()
 
 
     def test_group_state_change_events_by(self) -> None:
-        group_state_change_events = self.dt.group_state_change_events(by=self.dt.person(PersonURI("/api/v1/person/person/108756/")))
+        group_state_change_events = self.dt.group_state_change_events(by=self.dt.person(PersonURI(uri="/api/v1/person/person/108756/")))
         self.assertIsNot(group_state_change_events, None)
 
 
     def test_group_state_change_events_group(self) -> None:
-        group_state_change_events = self.dt.group_state_change_events(group=self.dt.group(GroupURI("/api/v1/group/group/1326/")))
+        group_state_change_events = self.dt.group_state_change_events(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1326/")))
         self.assertIsNot(group_state_change_events, None)
 
 
     def test_group_state_change_events_state(self) -> None:
-        group_state_change_events = self.dt.group_state_change_events(state=self.dt.group_state(GroupStateURI("/api/v1/name/groupstatename/proposed/")))
+        group_state_change_events = self.dt.group_state_change_events(state=self.dt.group_state(GroupStateURI(uri="/api/v1/name/groupstatename/proposed/")))
         self.assertIsNot(group_state_change_events, None)
 
 
     def test_groups_state(self) -> None:
-        groups = list(self.dt.groups(state=self.dt.group_state(GroupStateURI("/api/v1/name/groupstatename/abandon/"))))
+        groups = list(self.dt.groups(state=self.dt.group_state(GroupStateURI(uri="/api/v1/name/groupstatename/abandon/"))))
         self.assertEqual(len(groups), 14)
         self.assertEqual(groups[ 0].id, 1949)
         self.assertEqual(groups[ 1].id, 2009)
         self.assertEqual(groups[ 2].id, 2018)
         self.assertEqual(groups[ 3].id, 2155)
         self.assertEqual(groups[ 4].id, 2190)
         self.assertEqual(groups[ 5].id, 2200)
@@ -1891,41 +1957,41 @@
         self.assertEqual(groups[10].id, 2334)    # JSON Web Proofs
         self.assertEqual(groups[11].id, 2348)    # RADEXTRA
         self.assertEqual(groups[12].id, 2387)    # CONGRESS was renamed to CCWG while chartering
         self.assertEqual(groups[13].id, 2389)    # NIMBY was renamed to IVY while chartering
 
 
     def test_groups_parent(self) -> None:
-        groups = list(self.dt.groups(parent=self.dt.group(GroupURI("/api/v1/group/group/1/"))))
+        groups = list(self.dt.groups(parent=self.dt.group(GroupURI(uri="/api/v1/group/group/1/"))))
         self.assertEqual(len(groups), 3)
         self.assertEqual(groups[0].id, 2)       # IESG
         self.assertEqual(groups[1].id, 7)       # IAB
         self.assertEqual(groups[2].id, 2173)    # IANA Community Coordination Group
 
 
     def test_group_state(self) -> None:
-        state = self.dt.group_state(GroupStateURI("/api/v1/name/groupstatename/abandon/"))
+        state = self.dt.group_state(GroupStateURI(uri="/api/v1/name/groupstatename/abandon/"))
         if state is not None:
             self.assertEqual(state.desc,         "Formation of the group (most likely a BoF or Proposed WG) was abandoned")
             self.assertEqual(state.name,         "Abandoned")
             self.assertEqual(state.order,        0)
-            self.assertEqual(state.resource_uri, GroupStateURI("/api/v1/name/groupstatename/abandon/"))
+            self.assertEqual(state.resource_uri, GroupStateURI(uri="/api/v1/name/groupstatename/abandon/"))
             self.assertEqual(state.slug,         "abandon")
             self.assertEqual(state.used,         True)
         else:
             self.fail("Cannot find group state")
 
 
     def test_group_state_from_slug(self) -> None:
         state = self.dt.group_state_from_slug("abandon")
         if state is not None:
             self.assertEqual(state.desc,         "Formation of the group (most likely a BoF or Proposed WG) was abandoned")
             self.assertEqual(state.name,         "Abandoned")
             self.assertEqual(state.order,        0)
-            self.assertEqual(state.resource_uri, GroupStateURI("/api/v1/name/groupstatename/abandon/"))
+            self.assertEqual(state.resource_uri, GroupStateURI(uri="/api/v1/name/groupstatename/abandon/"))
             self.assertEqual(state.slug,         "abandon")
             self.assertEqual(state.used,         True)
         else:
             self.fail("Cannot find group state")
 
 
     # FIXME: this needs to be updated
@@ -1940,146 +2006,147 @@
         self.assertEqual(states[5].slug, "dormant")
         self.assertEqual(states[6].slug, "proposed")
         self.assertEqual(states[7].slug, "replaced")
         self.assertEqual(states[8].slug, "unknown")
 
 
     def test_group_type_name(self) -> None:
-        group_type_name = self.dt.group_type_name(GroupTypeNameURI("/api/v1/name/grouptypename/adhoc/"))
+        group_type_name = self.dt.group_type_name(GroupTypeNameURI(uri="/api/v1/name/grouptypename/adhoc/"))
         if group_type_name is not None:
             self.assertEqual(group_type_name.desc,         "Ad Hoc schedulable Group Type, for instance HotRfc")
             self.assertEqual(group_type_name.name,         "Ad Hoc")
             self.assertEqual(group_type_name.order,        0)
-            self.assertEqual(group_type_name.resource_uri, GroupTypeNameURI("/api/v1/name/grouptypename/adhoc/"))
+            self.assertEqual(group_type_name.resource_uri, GroupTypeNameURI(uri="/api/v1/name/grouptypename/adhoc/"))
             self.assertEqual(group_type_name.slug,         "adhoc")
             self.assertEqual(group_type_name.used,         True)
             self.assertEqual(group_type_name.verbose_name, "Ad Hoc Group Type")
 
 
     def test_group_type_name_from_slug(self) -> None:
         group_type_name = self.dt.group_type_name_from_slug("adhoc")
         if group_type_name is not None:
             self.assertEqual(group_type_name.desc,         "Ad Hoc schedulable Group Type, for instance HotRfc")
             self.assertEqual(group_type_name.name,         "Ad Hoc")
             self.assertEqual(group_type_name.order,        0)
-            self.assertEqual(group_type_name.resource_uri, GroupTypeNameURI("/api/v1/name/grouptypename/adhoc/"))
+            self.assertEqual(group_type_name.resource_uri, GroupTypeNameURI(uri="/api/v1/name/grouptypename/adhoc/"))
             self.assertEqual(group_type_name.slug,         "adhoc")
             self.assertEqual(group_type_name.used,         True)
             self.assertEqual(group_type_name.verbose_name, "Ad Hoc Group Type")
 
 
     def test_group_type_names(self) -> None:
         group_type_names = list(self.dt.group_type_names())
-        self.assertEqual(len(group_type_names), 25)
+        self.assertEqual(len(group_type_names), 26)
         self.assertEqual(group_type_names[ 0].slug, "adhoc")
         self.assertEqual(group_type_names[ 1].slug, "adm")
         self.assertEqual(group_type_names[ 2].slug, "ag")
         self.assertEqual(group_type_names[ 3].slug, "area")
         self.assertEqual(group_type_names[ 4].slug, "dir")
         self.assertEqual(group_type_names[ 5].slug, "edappr")
         self.assertEqual(group_type_names[ 6].slug, "edwg")
         self.assertEqual(group_type_names[ 7].slug, "iab")
         self.assertEqual(group_type_names[ 8].slug, "iabasg")
-        self.assertEqual(group_type_names[ 9].slug, "iana")
-        self.assertEqual(group_type_names[10].slug, "iesg")
-        self.assertEqual(group_type_names[11].slug, "ietf")
-        self.assertEqual(group_type_names[12].slug, "individ")
-        self.assertEqual(group_type_names[13].slug, "irtf")
-        self.assertEqual(group_type_names[14].slug, "ise")
-        self.assertEqual(group_type_names[15].slug, "isoc")
-        self.assertEqual(group_type_names[16].slug, "nomcom")
-        self.assertEqual(group_type_names[17].slug, "program")
-        self.assertEqual(group_type_names[18].slug, "rag")
-        self.assertEqual(group_type_names[19].slug, "review")
-        self.assertEqual(group_type_names[20].slug, "rfcedtyp")
-        self.assertEqual(group_type_names[21].slug, "rg")
-        self.assertEqual(group_type_names[22].slug, "sdo")
-        self.assertEqual(group_type_names[23].slug, "team")
-        self.assertEqual(group_type_names[24].slug, "wg")
+        self.assertEqual(group_type_names[ 9].slug, "iabworkshop")
+        self.assertEqual(group_type_names[10].slug, "iana")
+        self.assertEqual(group_type_names[11].slug, "iesg")
+        self.assertEqual(group_type_names[12].slug, "ietf")
+        self.assertEqual(group_type_names[13].slug, "individ")
+        self.assertEqual(group_type_names[14].slug, "irtf")
+        self.assertEqual(group_type_names[15].slug, "ise")
+        self.assertEqual(group_type_names[16].slug, "isoc")
+        self.assertEqual(group_type_names[17].slug, "nomcom")
+        self.assertEqual(group_type_names[18].slug, "program")
+        self.assertEqual(group_type_names[19].slug, "rag")
+        self.assertEqual(group_type_names[20].slug, "review")
+        self.assertEqual(group_type_names[21].slug, "rfcedtyp")
+        self.assertEqual(group_type_names[22].slug, "rg")
+        self.assertEqual(group_type_names[23].slug, "sdo")
+        self.assertEqual(group_type_names[24].slug, "team")
+        self.assertEqual(group_type_names[25].slug, "wg")
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to meetings:
 
     def test_meeting_session_assignment(self) -> None:
-        assignment = self.dt.meeting_session_assignment(SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61212/"))
+        assignment = self.dt.meeting_session_assignment(SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61212/"))
         if assignment is not None:
             self.assertEqual(assignment.id,           61212)
             self.assertEqual(assignment.modified,     datetime.fromisoformat("2017-10-17T12:14:33-07:00"))
             self.assertEqual(assignment.extendedfrom, None)
-            self.assertEqual(assignment.timeslot,     TimeslotURI("/api/v1/meeting/timeslot/9132/"))
-            self.assertEqual(assignment.session,      SessionURI("/api/v1/meeting/session/25907/"))
-            self.assertEqual(assignment.agenda,       ScheduleURI("/api/v1/meeting/schedule/787/"))
-            self.assertEqual(assignment.schedule,     ScheduleURI("/api/v1/meeting/schedule/787/"))
+            self.assertEqual(assignment.timeslot,     TimeslotURI(uri="/api/v1/meeting/timeslot/9132/"))
+            self.assertEqual(assignment.session,      SessionURI(uri="/api/v1/meeting/session/25907/"))
+            self.assertEqual(assignment.agenda,       ScheduleURI(uri="/api/v1/meeting/schedule/787/"))
+            self.assertEqual(assignment.schedule,     ScheduleURI(uri="/api/v1/meeting/schedule/787/"))
             self.assertEqual(assignment.pinned,       False)
-            self.assertEqual(assignment.resource_uri, SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61212/"))
+            self.assertEqual(assignment.resource_uri, SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61212/"))
             self.assertEqual(assignment.badness,      0)
             self.assertEqual(assignment.notes, "")
         else:
             self.fail("cannot find meeting session assignment")
 
 
     def test_meeting_session_assignments(self) -> None:
-        meeting  = self.dt.meeting(MeetingURI("/api/v1/meeting/meeting/365/")) # IETF 90 in Toronto
+        meeting  = self.dt.meeting(MeetingURI(uri="/api/v1/meeting/meeting/365/")) # IETF 90 in Toronto
         if meeting is not None and meeting.schedule is not None:
             schedule = self.dt.meeting_schedule(meeting.schedule)
             if schedule is not None:
                 assignments = list(self.dt.meeting_session_assignments(schedule))
                 self.assertEqual(len(assignments), 161)
             else:
                 self.fail("Cannot find schedule")
         else:
             self.fail("Cannot find meeting")
 
 
     def test_meeting_session_status(self) -> None:
-        session = self.dt.meeting_session(SessionURI("/api/v1/meeting/session/25907/"))
+        session = self.dt.meeting_session(SessionURI(uri="/api/v1/meeting/session/25907/"))
         if session is not None:
             status  = self.dt.meeting_session_status(session)
             if status is None:
                 self.fail("Cannot find session status")
             self.assertEqual(status.slug, "sched")
         else:
             self.fail("Cannot find session")
 
 
     def test_meeting_session_status_name(self) -> None:
-        ssn = self.dt.meeting_session_status_name(SessionStatusNameURI("/api/v1/name/sessionstatusname/sched/"))
+        ssn = self.dt.meeting_session_status_name(SessionStatusNameURI(uri="/api/v1/name/sessionstatusname/sched/"))
         if ssn is not None:
             self.assertEqual(ssn.order,        0)
             self.assertEqual(ssn.slug,         "sched")
-            self.assertEqual(ssn.resource_uri, SessionStatusNameURI("/api/v1/name/sessionstatusname/sched/"))
+            self.assertEqual(ssn.resource_uri, SessionStatusNameURI(uri="/api/v1/name/sessionstatusname/sched/"))
             self.assertEqual(ssn.used,         True)
             self.assertEqual(ssn.desc,         "")
             self.assertEqual(ssn.name,         "Scheduled")
         else:
             self.fail("Cannot find meeting session status name")
 
 
     def test_meeting_session_purpose(self) -> None:
-        sp = self.dt.meeting_session_purpose(SessionPurposeURI("/api/v1/name/sessionpurposename/closed_meeting/"))
+        sp = self.dt.meeting_session_purpose(SessionPurposeURI(uri="/api/v1/name/sessionpurposename/closed_meeting/"))
         if sp is not None:
             self.assertEqual(sp.used, True)
             self.assertEqual(sp.timeslot_types, "['other', 'regular']")
             self.assertEqual(sp.order, 10)
             self.assertEqual(sp.on_agenda, False)
-            self.assertEqual(sp.resource_uri, SessionPurposeURI("/api/v1/name/sessionpurposename/closed_meeting/"))
+            self.assertEqual(sp.resource_uri, SessionPurposeURI(uri="/api/v1/name/sessionpurposename/closed_meeting/"))
             self.assertEqual(sp.name, "Closed meeting")
             self.assertEqual(sp.desc, "Closed meeting")
             self.assertEqual(sp.slug, "closed_meeting")
         else:
             self.fail("Cannot find meeting session purpose")
 
 
     def test_meeting_session_status_name_from_slug(self) -> None:
         ssn = self.dt.meeting_session_status_name_from_slug("sched")
         if ssn is not None:
             self.assertEqual(ssn.order,        0)
             self.assertEqual(ssn.slug,         "sched")
-            self.assertEqual(ssn.resource_uri, SessionStatusNameURI("/api/v1/name/sessionstatusname/sched/"))
+            self.assertEqual(ssn.resource_uri, SessionStatusNameURI(uri="/api/v1/name/sessionstatusname/sched/"))
             self.assertEqual(ssn.used,         True)
             self.assertEqual(ssn.desc,         "")
             self.assertEqual(ssn.name,         "Scheduled")
         else:
             self.fail("Cannot find meeting session status name")
 
 
@@ -2096,146 +2163,146 @@
         self.assertEqual(status_names[ 7].slug, "resched")    # Rescheduled
         self.assertEqual(status_names[ 8].slug, "sched")      # Scheduled
         self.assertEqual(status_names[ 9].slug, "scheda")     # Scheduled - Announcement to be sent
         self.assertEqual(status_names[10].slug, "schedw")     # Waiting for Scheduling
 
 
     def test_meeting_session(self) -> None:
-        session = self.dt.meeting_session(SessionURI("/api/v1/meeting/session/25907/"))
+        session = self.dt.meeting_session(SessionURI(uri="/api/v1/meeting/session/25907/"))
         if session is not None:
-            self.assertEqual(session.resource_uri,        SessionURI("/api/v1/meeting/session/25907/"))
+            self.assertEqual(session.resource_uri,        SessionURI(uri="/api/v1/meeting/session/25907/"))
             self.assertEqual(session.id,                  25907)
             self.assertEqual(session.type,                "/api/v1/name/timeslottypename/regular/")
             self.assertEqual(session.name,                "")
-            self.assertEqual(session.meeting,             MeetingURI("/api/v1/meeting/meeting/747/"))
-            self.assertEqual(session.group,               GroupURI("/api/v1/group/group/1803/"))
-            self.assertEqual(session.materials,           [DocumentURI("/api/v1/doc/document/agenda-100-homenet/"),
-                                                           DocumentURI("/api/v1/doc/document/slides-100-homenet-chair-slides/"),
-                                                           DocumentURI("/api/v1/doc/document/slides-100-homenet-support-for-hncp-in-ipv6-ce-routers/"),
-                                                           DocumentURI("/api/v1/doc/document/slides-100-homenet-homenet-security/"),
-                                                           DocumentURI("/api/v1/doc/document/slides-100-homenet-naming/"),
-                                                           DocumentURI("/api/v1/doc/document/recording-100-homenet-1/"),
-                                                           DocumentURI("/api/v1/doc/document/minutes-100-homenet/"),
-                                                           DocumentURI("/api/v1/doc/document/bluesheets-100-homenet-201711131550/"),
-                                                           DocumentURI("/api/v1/doc/document/recording-100-homenet-2/")])
+            self.assertEqual(session.meeting,             MeetingURI(uri="/api/v1/meeting/meeting/747/"))
+            self.assertEqual(session.group,               GroupURI(uri="/api/v1/group/group/1803/"))
+            self.assertEqual(session.materials,           [DocumentURI(uri="/api/v1/doc/document/agenda-100-homenet/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/slides-100-homenet-chair-slides/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/slides-100-homenet-support-for-hncp-in-ipv6-ce-routers/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/slides-100-homenet-homenet-security/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/slides-100-homenet-naming/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/recording-100-homenet-1/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/minutes-100-homenet/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/bluesheets-100-homenet-201711131550/"),
+                                                           DocumentURI(uri="/api/v1/doc/document/recording-100-homenet-2/")])
             self.assertEqual(session.scheduled,           datetime.fromisoformat("2017-10-20T17:24:10-07:00"))
             self.assertEqual(session.requested_duration,  "1:30:00")
             self.assertEqual(session.resources,           [])
             self.assertEqual(session.agenda_note,         "")
-            self.assertEqual(session.assignments,         [SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/57892/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/58170/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/59755/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/58279/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/58458/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/58623/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/58832/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/59092/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/59259/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/59424/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/59585/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/59937/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/60151/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/60325/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/60509/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/60692/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/60867/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61041/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61212/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61405/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61595/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61765/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/61939/"),
-                                                           SessionAssignmentURI("/api/v1/meeting/schedtimesessassignment/67156/")])
+            self.assertEqual(session.assignments,         [SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/57892/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/58170/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/59755/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/58279/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/58458/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/58623/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/58832/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/59092/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/59259/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/59424/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/59585/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/59937/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/60151/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/60325/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/60509/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/60692/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/60867/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61041/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61212/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61405/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61595/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61765/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/61939/"),
+                                                           SessionAssignmentURI(uri="/api/v1/meeting/schedtimesessassignment/67156/")])
             self.assertEqual(session.remote_instructions, "")
             self.assertEqual(session.short,               "")
             self.assertEqual(session.attendees,           120)
             self.assertEqual(session.modified,            datetime.fromisoformat("2017-10-20T17:24:10-07:00"))
             self.assertEqual(session.comments,            "")
         else:
             self.fail("cannot find meeting session")
 
 
     def test_meeting_sessions(self) -> None:
-        ietf90  = self.dt.meeting(MeetingURI("/api/v1/meeting/meeting/365/")) # IETF 90 in Toronto
+        ietf90  = self.dt.meeting(MeetingURI(uri="/api/v1/meeting/meeting/365/")) # IETF 90 in Toronto
         tsvwg   = self.dt.group_from_acronym("tsvwg")
         if ietf90 is not None and tsvwg is not None:
             sessions = list(self.dt.meeting_sessions(meeting=ietf90, group=tsvwg))
             self.assertEqual(len(sessions), 2)
             self.assertEqual(sessions[0].id, 23197)
             self.assertEqual(sessions[1].id, 23198)
         else:
             self.fail("cannot find ietf90 or tsvwg")
 
 
     def test_meeting_timeslot(self) -> None:
-        ts = self.dt.meeting_timeslot(TimeslotURI("/api/v1/meeting/timeslot/12857/"))
+        ts = self.dt.meeting_timeslot(TimeslotURI(uri="/api/v1/meeting/timeslot/12857/"))
         if ts is not None:
-            self.assertEqual(ts.resource_uri,   TimeslotURI("/api/v1/meeting/timeslot/12857/"))
+            self.assertEqual(ts.resource_uri,   TimeslotURI(uri="/api/v1/meeting/timeslot/12857/"))
             self.assertEqual(ts.id,             12857)
             self.assertEqual(ts.type,           "/api/v1/name/timeslottypename/regular/")
-            self.assertEqual(ts.meeting,       MeetingURI("/api/v1/meeting/meeting/1211/"))
-            self.assertEqual(ts.sessions,      [SessionURI("/api/v1/meeting/session/28208/")])
+            self.assertEqual(ts.meeting,       MeetingURI(uri="/api/v1/meeting/meeting/1211/"))
+            self.assertEqual(ts.sessions,      [SessionURI(uri="/api/v1/meeting/session/28208/")])
             self.assertEqual(ts.name,          "")
             self.assertEqual(ts.time,          datetime.fromisoformat("2020-08-05T06:00:00-07:00"))
             self.assertEqual(ts.duration,      "2:30:00")
             self.assertEqual(ts.location,      None)
             self.assertEqual(ts.show_location, True)
             self.assertEqual(ts.modified,      datetime.fromisoformat("2020-07-30T01:28:28-07:00"))
         else:
             self.fail("cannot find timeslot")
 
 
     def test_meeting_scheduling_event(self) -> None:
-        se = self.dt.meeting_scheduling_event(SchedulingEventURI("/api/v1/meeting/schedulingevent/16203/"))
+        se = self.dt.meeting_scheduling_event(SchedulingEventURI(uri="/api/v1/meeting/schedulingevent/16203/"))
         if se is not None:
-            self.assertEqual(se.resource_uri, SchedulingEventURI("/api/v1/meeting/schedulingevent/16203/"))
+            self.assertEqual(se.resource_uri, SchedulingEventURI(uri="/api/v1/meeting/schedulingevent/16203/"))
             self.assertEqual(se.id,           16203)
-            self.assertEqual(se.session,      SessionURI("/api/v1/meeting/session/28208/"))
-            self.assertEqual(se.status,       SessionStatusNameURI("/api/v1/name/sessionstatusname/sched/"))
-            self.assertEqual(se.by,           PersonURI("/api/v1/person/person/106460/"))
+            self.assertEqual(se.session,      SessionURI(uri="/api/v1/meeting/session/28208/"))
+            self.assertEqual(se.status,       SessionStatusNameURI(uri="/api/v1/name/sessionstatusname/sched/"))
+            self.assertEqual(se.by,           PersonURI(uri="/api/v1/person/person/106460/"))
             self.assertEqual(se.time,         datetime.fromisoformat("2020-06-12T13:01:38-07:00"))
         else:
             self.fail("Cannot find scheduling event")
 
 
     def test_meeting_scheduling_events(self) -> None:
-        session = self.dt.meeting_session(SessionURI("/api/v1/meeting/session/28208/"))
+        session = self.dt.meeting_session(SessionURI(uri="/api/v1/meeting/session/28208/"))
         events  = list(self.dt.meeting_scheduling_events(session=session))
         self.assertEqual(len(events),  2)
         self.assertEqual(events[0].id, 16192)
         self.assertEqual(events[1].id, 16203)
 
 
     def test_meeting_schedule(self) -> None:
-        schedule = self.dt.meeting_schedule(ScheduleURI("/api/v1/meeting/schedule/209/"))
+        schedule = self.dt.meeting_schedule(ScheduleURI(uri="/api/v1/meeting/schedule/209/"))
         if schedule is not None:
             self.assertEqual(schedule.id,           209)
-            self.assertEqual(schedule.resource_uri, ScheduleURI("/api/v1/meeting/schedule/209/"))
-            self.assertEqual(schedule.meeting,      MeetingURI("/api/v1/meeting/meeting/365/"))
-            self.assertEqual(schedule.owner,        PersonURI("/api/v1/person/person/109129/"))
+            self.assertEqual(schedule.resource_uri, ScheduleURI(uri="/api/v1/meeting/schedule/209/"))
+            self.assertEqual(schedule.meeting,      MeetingURI(uri="/api/v1/meeting/meeting/365/"))
+            self.assertEqual(schedule.owner,        PersonURI(uri="/api/v1/person/person/109129/"))
             self.assertEqual(schedule.name,         "prelim-fix")
             self.assertEqual(schedule.visible,      True)
             self.assertEqual(schedule.public,       True)
             self.assertEqual(schedule.badness,      None)
             self.assertEqual(schedule.notes,        "")
         else:
             self.fail("cannot find meeting schedule")
 
 
     def test_meeting(self) -> None:
-        meeting = self.dt.meeting(MeetingURI("/api/v1/meeting/meeting/365/"))
+        meeting = self.dt.meeting(MeetingURI(uri="/api/v1/meeting/meeting/365/"))
         if meeting is not None:
             self.assertEqual(meeting.id,                               365)
-            self.assertEqual(meeting.resource_uri,                     MeetingURI("/api/v1/meeting/meeting/365/"))
-            self.assertEqual(meeting.type,                             MeetingTypeURI("/api/v1/name/meetingtypename/ietf/"))
+            self.assertEqual(meeting.resource_uri,                     MeetingURI(uri="/api/v1/meeting/meeting/365/"))
+            self.assertEqual(meeting.type,                             MeetingTypeURI(uri="/api/v1/name/meetingtypename/ietf/"))
             self.assertEqual(meeting.city,                             "Toronto")
             self.assertEqual(meeting.country,                          "CA")
             self.assertEqual(meeting.venue_name,                       "Fairmont Royal York Hotel")
             self.assertEqual(meeting.venue_addr,                       "100 Front Street W\r\nToronto, Ontario, Canada M5J 1E3")
-            self.assertEqual(meeting.date,                             datetime.fromisoformat("2014-07-20T00:00:00"))
+            self.assertEqual(meeting.date,                             date.fromisoformat("2014-07-20"))
             self.assertEqual(meeting.days,                             6)
             self.assertEqual(meeting.time_zone,                        "America/Toronto")
             self.assertEqual(meeting.idsubmit_cutoff_day_offset_00,    20)
             self.assertEqual(meeting.idsubmit_cutoff_day_offset_01,    13)
             self.assertEqual(meeting.idsubmit_cutoff_warning_days,     "21 days, 0:00:00")
             self.assertEqual(meeting.idsubmit_cutoff_time_utc,         "23:59:59")
             self.assertEqual(meeting.submission_cutoff_day_offset,     26)
@@ -2244,18 +2311,17 @@
             self.assertEqual(meeting.attendees,                        1237)
             self.assertEqual(meeting.session_request_lock_message,     "")
             self.assertEqual(meeting.reg_area,                         "Ballroom Foyer ")
             self.assertEqual(meeting.break_area,                       "Convention and Main Mezzanine Level Foyers")
             self.assertEqual(meeting.agenda_info_note,                 "")
             self.assertEqual(meeting.agenda_warning_note,              "")
             self.assertEqual(meeting.show_important_dates,             True)
-            print(meeting.updated)
             self.assertEqual(meeting.updated,                          datetime.fromisoformat("2023-02-10T10:42:38-08:00"))
-            self.assertEqual(meeting.agenda,                           ScheduleURI("/api/v1/meeting/schedule/209/"))
-            self.assertEqual(meeting.schedule,                         ScheduleURI("/api/v1/meeting/schedule/209/"))
+            self.assertEqual(meeting.agenda,                           ScheduleURI(uri="/api/v1/meeting/schedule/209/"))
+            self.assertEqual(meeting.schedule,                         ScheduleURI(uri="/api/v1/meeting/schedule/209/"))
             self.assertEqual(meeting.number,                           "90")
             self.assertEqual(meeting.proceedings_final,                False)
             self.assertEqual(meeting.acknowledgements,                 "")
         else:
             self.fail("Cannot find meeting")
 
 
@@ -2265,30 +2331,30 @@
         self.assertEqual(len(meetings),  3)
         self.assertEqual(meetings[0].city, "Prague")
         self.assertEqual(meetings[1].city, "Montreal")
         self.assertEqual(meetings[2].city, "Singapore")
 
 
     def test_meeting_type(self) -> None:
-        meeting_type = self.dt.meeting_type(MeetingTypeURI("/api/v1/name/meetingtypename/ietf/"))
+        meeting_type = self.dt.meeting_type(MeetingTypeURI(uri="/api/v1/name/meetingtypename/ietf/"))
         if meeting_type is not None:
-            self.assertEqual(meeting_type.resource_uri, MeetingTypeURI("/api/v1/name/meetingtypename/ietf/"))
+            self.assertEqual(meeting_type.resource_uri, MeetingTypeURI(uri="/api/v1/name/meetingtypename/ietf/"))
             self.assertEqual(meeting_type.name,         "IETF")
             self.assertEqual(meeting_type.order,        0)
             self.assertEqual(meeting_type.slug,         "ietf")
             self.assertEqual(meeting_type.desc,         "")
             self.assertEqual(meeting_type.used,         True)
         else:
             self.fail("Cannot find meeting_type")
 
 
     def test_meeting_type_from_slug(self) -> None:
         meeting_type = self.dt.meeting_type_from_slug("ietf")
         if meeting_type is not None:
-            self.assertEqual(meeting_type.resource_uri, MeetingTypeURI("/api/v1/name/meetingtypename/ietf/"))
+            self.assertEqual(meeting_type.resource_uri, MeetingTypeURI(uri="/api/v1/name/meetingtypename/ietf/"))
             self.assertEqual(meeting_type.name,         "IETF")
             self.assertEqual(meeting_type.order,        0)
             self.assertEqual(meeting_type.slug,         "ietf")
             self.assertEqual(meeting_type.desc,         "")
             self.assertEqual(meeting_type.used,         True)
         else:
             self.fail("Cannot find meeting_type")
@@ -2299,262 +2365,263 @@
         self.assertEqual(len(types),  2)
         self.assertEqual(types[0].slug, "ietf")
         self.assertEqual(types[1].slug, "interim")
 
 
     @patch.object(ietfdata.datatracker, 'datetime', Mock(wraps=datetime))
     def test_meeting_status_future(self) -> None:
-        meeting = self.dt.meeting(MeetingURI("/api/v1/meeting/meeting/365/"))
+        meeting = self.dt.meeting(MeetingURI(uri="/api/v1/meeting/meeting/365/"))
         if meeting is not None:
-            ietfdata.datatracker.datetime.now.return_value = datetime(2014, 1, 1) # type: ignore
+            ietfdata.datatracker.datetime.now.return_value = date(2014, 1, 1) # type: ignore
             self.assertEqual(meeting.status(), MeetingStatus.FUTURE)
         else:
             self.fail("Cannot find meeting")
 
 
     @patch.object(ietfdata.datatracker, 'datetime', Mock(wraps=datetime))
     def test_meeting_status_completed(self) -> None:
-        meeting = self.dt.meeting(MeetingURI("/api/v1/meeting/meeting/365/"))
+        meeting = self.dt.meeting(MeetingURI(uri="/api/v1/meeting/meeting/365/"))
         if meeting is not None:
-            ietfdata.datatracker.datetime.now.return_value = datetime(2014, 12, 1) # type: ignore
+            ietfdata.datatracker.datetime.now.return_value = date(2014, 12, 1) # type: ignore
             self.assertEqual(meeting.status(), MeetingStatus.COMPLETED)
         else:
             self.fail("Cannot find meeting")
 
 
     @patch.object(ietfdata.datatracker, 'datetime', Mock(wraps=datetime))
     def test_meeting_status_ongoing(self) -> None:
-        meeting = self.dt.meeting(MeetingURI("/api/v1/meeting/meeting/365/"))
+        meeting = self.dt.meeting(MeetingURI(uri="/api/v1/meeting/meeting/365/"))
         if meeting is not None:
-            ietfdata.datatracker.datetime.now.return_value = datetime(2014, 7, 20) # type: ignore
+            ietfdata.datatracker.datetime.now.return_value = date(2014, 7, 20) # type: ignore
             self.assertEqual(meeting.status(), MeetingStatus.ONGOING)
         else:
             self.fail("Cannot find meeting")
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to related documents:
 
     def test_related_documents_all(self) -> None:
-        source = self.dt.document(DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        target = list(self.dt.document_aliases(name="draft-gwinn-paging-protocol-v3"))[0]
+        source = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        target = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3"))
         rel    = self.dt.relationship_type_from_slug("replaces")
         rdocs  = list(self.dt.related_documents(source=source, target=target, relationship_type=rel))
         self.assertEqual(len(rdocs), 1)
         self.assertEqual(rdocs[0].id, 3)
-        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/replaces/"))
-        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/3/"))
-        self.assertEqual(rdocs[0].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[0].target,       DocumentAliasURI("/api/v1/doc/docalias/draft-gwinn-paging-protocol-v3/"))
+        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/replaces/"))
+        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/3/"))
+        self.assertEqual(rdocs[0].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[0].target,       DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3/"))
 
 
     def test_related_documents_source_target(self) -> None:
-        source = self.dt.document(DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        target = list(self.dt.document_aliases(name="draft-gwinn-paging-protocol-v3"))[0]
+        source = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        target = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3"))
         rdocs  = list(self.dt.related_documents(source=source, target=target))
         self.assertEqual(len(rdocs), 1)
         self.assertEqual(rdocs[0].id, 3)
-        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/replaces/"))
-        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/3/"))
-        self.assertEqual(rdocs[0].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[0].target,       DocumentAliasURI("/api/v1/doc/docalias/draft-gwinn-paging-protocol-v3/"))
+        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/replaces/"))
+        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/3/"))
+        self.assertEqual(rdocs[0].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[0].target,       DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3/"))
 
 
     def test_related_documents_source_relationship(self) -> None:
-        source = self.dt.document(DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        rel    = self.dt.relationship_type_from_slug("replaces")
-        rdocs  = list(self.dt.related_documents(source=source, relationship_type=rel))
+        source = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        rdocs  = list(self.dt.related_documents(source=source, relationship_type_slug = "replaces"))
         self.assertEqual(len(rdocs), 1)
         self.assertEqual(rdocs[0].id, 3)
-        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/replaces/"))
-        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/3/"))
-        self.assertEqual(rdocs[0].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[0].target,       DocumentAliasURI("/api/v1/doc/docalias/draft-gwinn-paging-protocol-v3/"))
+        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/replaces/"))
+        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/3/"))
+        self.assertEqual(rdocs[0].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[0].target,       DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3/"))
 
 
     def test_related_documents_target_relationship(self) -> None:
-        target = list(self.dt.document_aliases(name="draft-gwinn-paging-protocol-v3"))[0]
-        rel    = self.dt.relationship_type_from_slug("replaces")
-        rdocs  = list(self.dt.related_documents(target=target, relationship_type=rel))
+        target = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3"))
+        rdocs  = list(self.dt.related_documents(target=target, relationship_type_slug = "replaces"))
         self.assertEqual(len(rdocs), 1)
         self.assertEqual(rdocs[0].id, 3)
-        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/replaces/"))
-        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/3/"))
-        self.assertEqual(rdocs[0].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[0].target,       DocumentAliasURI("/api/v1/doc/docalias/draft-gwinn-paging-protocol-v3/"))
+        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/replaces/"))
+        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/3/"))
+        self.assertEqual(rdocs[0].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[0].target,       DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3/"))
 
 
     def test_related_documents_target(self) -> None:
-        target = list(self.dt.document_aliases(name="draft-gwinn-paging-protocol-v3"))[0]
+        target = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3"))
         rdocs  = list(self.dt.related_documents(target=target))
         self.assertEqual(len(rdocs), 1)
         self.assertEqual(rdocs[0].id, 3)
-        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/replaces/"))
-        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/3/"))
-        self.assertEqual(rdocs[0].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[0].target,       DocumentAliasURI("/api/v1/doc/docalias/draft-gwinn-paging-protocol-v3/"))
+        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/replaces/"))
+        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/3/"))
+        self.assertEqual(rdocs[0].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[0].target,       DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3/"))
 
 
     def test_related_documents_source(self) -> None:
-        source = self.dt.document(DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        rdocs  = list(self.dt.related_documents(source=source))
+        src_doc = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        rdocs  = list(self.dt.related_documents(source = src_doc))
         self.assertEqual(len(rdocs), 6)
         self.assertEqual(rdocs[0].id, 3)
-        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/replaces/"))
-        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/3/"))
-        self.assertEqual(rdocs[0].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[0].target,       DocumentAliasURI("/api/v1/doc/docalias/draft-gwinn-paging-protocol-v3/"))
-        self.assertEqual(rdocs[1].id, 2059)
-        self.assertEqual(rdocs[1].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/obs/"))
-        self.assertEqual(rdocs[1].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/2059/"))
-        self.assertEqual(rdocs[1].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[1].target,       DocumentAliasURI("/api/v1/doc/docalias/rfc1645/"))
-        self.assertEqual(rdocs[2].id, 10230)
-        self.assertEqual(rdocs[2].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/refold/"))
-        self.assertEqual(rdocs[2].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/10230/"))
-        self.assertEqual(rdocs[2].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[2].target,       DocumentAliasURI("/api/v1/doc/docalias/rfc1425/"))
-        self.assertEqual(rdocs[3].id, 10231)
-        self.assertEqual(rdocs[3].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/refold/"))
-        self.assertEqual(rdocs[3].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/10231/"))
-        self.assertEqual(rdocs[3].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[3].target,       DocumentAliasURI("/api/v1/doc/docalias/rfc1521/"))
-        self.assertEqual(rdocs[4].id, 10233)
-        self.assertEqual(rdocs[4].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/refold/"))
-        self.assertEqual(rdocs[4].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/10233/"))
-        self.assertEqual(rdocs[4].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[4].target,       DocumentAliasURI("/api/v1/doc/docalias/std10/"))
-        self.assertEqual(rdocs[5].id, 10234)
-        self.assertEqual(rdocs[5].relationship, RelationshipTypeURI("/api/v1/name/docrelationshipname/refold/"))
-        self.assertEqual(rdocs[5].resource_uri, RelatedDocumentURI("/api/v1/doc/relateddocument/10234/"))
-        self.assertEqual(rdocs[5].source,       DocumentURI("/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
-        self.assertEqual(rdocs[5].target,       DocumentAliasURI("/api/v1/doc/docalias/rfc1486/"))
+        self.assertEqual(rdocs[0].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/replaces/"))
+        self.assertEqual(rdocs[0].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/3/"))
+        self.assertEqual(rdocs[0].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[0].target,       DocumentURI(uri="/api/v1/doc/document/draft-gwinn-paging-protocol-v3/"))
+        self.assertEqual(rdocs[1].id, 10230)
+        self.assertEqual(rdocs[1].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/refold/"))
+        self.assertEqual(rdocs[1].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/10230/"))
+        self.assertEqual(rdocs[1].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[1].target,       DocumentURI(uri="/api/v1/doc/document/rfc1425/"))
+        self.assertEqual(rdocs[2].id, 10231)
+        self.assertEqual(rdocs[2].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/refold/"))
+        self.assertEqual(rdocs[2].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/10231/"))
+        self.assertEqual(rdocs[2].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[2].target,       DocumentURI(uri="/api/v1/doc/document/rfc1521/"))
+        self.assertEqual(rdocs[3].id, 10233)
+        self.assertEqual(rdocs[3].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/refold/"))
+        self.assertEqual(rdocs[3].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/10233/"))
+        self.assertEqual(rdocs[3].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[3].target,       DocumentURI(uri="/api/v1/doc/document/std10/"))
+        self.assertEqual(rdocs[4].id, 10234)
+        self.assertEqual(rdocs[4].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/refold/"))
+        self.assertEqual(rdocs[4].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/10234/"))
+        self.assertEqual(rdocs[4].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[4].target,       DocumentURI(uri="/api/v1/doc/document/rfc1486/"))
+        self.assertEqual(rdocs[5].id, 1289508)
+        self.assertEqual(rdocs[5].relationship, RelationshipTypeURI(uri="/api/v1/name/docrelationshipname/became_rfc/"))
+        self.assertEqual(rdocs[5].resource_uri, RelatedDocumentURI(uri="/api/v1/doc/relateddocument/1289508/"))
+        self.assertEqual(rdocs[5].source,       DocumentURI(uri="/api/v1/doc/document/draft-rfced-info-snpp-v3/"))
+        self.assertEqual(rdocs[5].target,       DocumentURI(uri="/api/v1/doc/document/rfc1861/"))
 
 
     def test_related_documents_relationship(self) -> None:
         rel    = self.dt.relationship_type_from_slug("replaces")
         rdocs  = self.dt.related_documents(relationship_type=rel)
         self.assertIsNot(rdocs, None)
 
 
     def test_relationship_types(self) -> None:
         types = list(self.dt.relationship_types())
-        self.assertEqual(len(types), 16)
-        self.assertEqual(types[ 0].slug, "conflrev")
-        self.assertEqual(types[ 1].slug, "downref-approval")
-        self.assertEqual(types[ 2].slug, "obs")
-        self.assertEqual(types[ 3].slug, "possibly-replaces")
-        self.assertEqual(types[ 4].slug, "refinfo")
-        self.assertEqual(types[ 5].slug, "refnorm")
-        self.assertEqual(types[ 6].slug, "refold")
-        self.assertEqual(types[ 7].slug, "refunk")
-        self.assertEqual(types[ 8].slug, "replaces")
-        self.assertEqual(types[ 9].slug, "tobcp")
-        self.assertEqual(types[10].slug, "toexp")
-        self.assertEqual(types[11].slug, "tohist")
-        self.assertEqual(types[12].slug, "toinf")
-        self.assertEqual(types[13].slug, "tois")
-        self.assertEqual(types[14].slug, "tops")
-        self.assertEqual(types[15].slug, "updates")
+        self.assertEqual(len(types), 18)
+        self.assertEqual(types[ 0].slug, "became_rfc")
+        self.assertEqual(types[ 1].slug, "conflrev")
+        self.assertEqual(types[ 2].slug, "contains")
+        self.assertEqual(types[ 3].slug, "downref-approval")
+        self.assertEqual(types[ 4].slug, "obs")
+        self.assertEqual(types[ 5].slug, "possibly-replaces")
+        self.assertEqual(types[ 6].slug, "refinfo")
+        self.assertEqual(types[ 7].slug, "refnorm")
+        self.assertEqual(types[ 8].slug, "refold")
+        self.assertEqual(types[ 9].slug, "refunk")
+        self.assertEqual(types[10].slug, "replaces")
+        self.assertEqual(types[11].slug, "tobcp")
+        self.assertEqual(types[12].slug, "toexp")
+        self.assertEqual(types[13].slug, "tohist")
+        self.assertEqual(types[14].slug, "toinf")
+        self.assertEqual(types[15].slug, "tois")
+        self.assertEqual(types[16].slug, "tops")
+        self.assertEqual(types[17].slug, "updates")
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to IPR disclosures:
 
     def test_ipr_disclosure_state(self) -> None:
-        ipr_disclosure_state = self.dt.ipr_disclosure_state(IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/pending/"))
+        ipr_disclosure_state = self.dt.ipr_disclosure_state(IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/pending/"))
         if ipr_disclosure_state is not None:
-            self.assertEqual(ipr_disclosure_state.resource_uri, IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/pending/"))
+            self.assertEqual(ipr_disclosure_state.resource_uri, IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/pending/"))
             self.assertEqual(ipr_disclosure_state.name,         "Pending")
             self.assertEqual(ipr_disclosure_state.used,         True)
             self.assertEqual(ipr_disclosure_state.slug,         "pending")
             self.assertEqual(ipr_disclosure_state.desc,         "")
             self.assertEqual(ipr_disclosure_state.order,        0)
         else:
             self.fail("Cannot find IPR disclosure state")
 
 
     def test_ipr_disclosure_states(self) -> None:
         states = list(self.dt.ipr_disclosure_states())
-        self.assertEqual(len(states), 5)
+        self.assertEqual(len(states), 6)
         self.assertEqual(states[0].slug,  "parked")
         self.assertEqual(states[1].slug,  "pending")
         self.assertEqual(states[2].slug,  "posted")
         self.assertEqual(states[3].slug,  "rejected")
         self.assertEqual(states[4].slug,  "removed")
+        self.assertEqual(states[5].slug,  "removed_objfalse")
 
 
     def test_ipr_disclosure_base(self) -> None:
-        ipr_disclosure_base = self.dt.ipr_disclosure_base(IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/4169/"))
+        ipr_disclosure_base = self.dt.ipr_disclosure_base(IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/4169/"))
         if ipr_disclosure_base is not None:
-            self.assertEqual(ipr_disclosure_base.by,                 PersonURI("/api/v1/person/person/1/"))
+            self.assertEqual(ipr_disclosure_base.by,                 PersonURI(uri="/api/v1/person/person/1/"))
             self.assertEqual(ipr_disclosure_base.compliant,          True)
             self.assertEqual(ipr_disclosure_base.docs,               [])
             self.assertEqual(ipr_disclosure_base.holder_legal_name,  "Patent and IP Recoveries llc as use licensee for US6370629 & US6393126")
             self.assertEqual(ipr_disclosure_base.id,                 4169)
             self.assertEqual(ipr_disclosure_base.notes,              "See update #4099 for specifics")
             self.assertEqual(ipr_disclosure_base.other_designations, "")
-            self.assertEqual(ipr_disclosure_base.rel,                [IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/4102/")])
-            self.assertEqual(ipr_disclosure_base.resource_uri,       IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/4169/"))
-            self.assertEqual(ipr_disclosure_base.state,              IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/parked/"))
+            self.assertEqual(ipr_disclosure_base.rel,                [IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/4102/")])
+            self.assertEqual(ipr_disclosure_base.resource_uri,       IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/4169/"))
+            self.assertEqual(ipr_disclosure_base.state,              IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/parked/"))
             self.assertEqual(ipr_disclosure_base.submitter_email,    "tglassey1@protonmail.com")
             self.assertEqual(ipr_disclosure_base.submitter_name,     "Todd Glassey")
             self.assertEqual(ipr_disclosure_base.time,               datetime.fromisoformat("2020-05-30T16:11:44-07:00"))
             self.assertEqual(ipr_disclosure_base.title,              "Patent and IP Recoveries llc as use licensee for US6370629 & US6393126's General License Statement")
         else:
             self.fail("Cannot find IPR disclosure base")
 
 
     def test_ipr_disclosure_bases(self) -> None:
         ipr_disclosure_bases = self.dt.ipr_disclosure_bases()
         self.assertIsNot(ipr_disclosure_bases, None)
 
 
     def test_ipr_disclosure_bases_by(self) -> None:
-        ipr_disclosure_bases = self.dt.ipr_disclosure_bases(by=self.dt.person(PersonURI("/api/v1/person/person/1/")))
+        ipr_disclosure_bases = self.dt.ipr_disclosure_bases(by=self.dt.person(PersonURI(uri="/api/v1/person/person/1/")))
         self.assertIsNot(ipr_disclosure_bases, None)
 
 
     def test_ipr_disclosure_bases_holder_legal_name(self) -> None:
         ipr_disclosure_bases = self.dt.ipr_disclosure_bases(holder_legal_name="Patent and IP Recoveries llc as use licensee for US6370629 & US6393126")
         self.assertIsNot(ipr_disclosure_bases, None)
 
 
     def test_ipr_disclosure_bases_state(self) -> None:
-        ipr_disclosure_bases = self.dt.ipr_disclosure_bases(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/pending/")))
+        ipr_disclosure_bases = self.dt.ipr_disclosure_bases(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/pending/")))
         self.assertIsNot(ipr_disclosure_bases, None)
 
 
     def test_ipr_disclosure_bases_submitter_email(self) -> None:
         ipr_disclosure_bases = self.dt.ipr_disclosure_bases(submitter_email="tglassey1@protonmail.com")
         self.assertIsNot(ipr_disclosure_bases, None)
 
 
     def test_ipr_disclosure_bases_submitter_name(self) -> None:
         ipr_disclosure_bases = self.dt.ipr_disclosure_bases(submitter_name="Todd Glassey")
         self.assertIsNot(ipr_disclosure_bases, None)
 
 
     def test_generic_ipr_disclosure(self) -> None:
-        generic_ipr_disclosure = self.dt.generic_ipr_disclosure(GenericIPRDisclosureURI("/api/v1/ipr/genericiprdisclosure/4061/"))
+        generic_ipr_disclosure = self.dt.generic_ipr_disclosure(GenericIPRDisclosureURI(uri="/api/v1/ipr/genericiprdisclosure/4061/"))
         if generic_ipr_disclosure is not None:
-            self.assertEqual(generic_ipr_disclosure.by,                    PersonURI("/api/v1/person/person/1/"))
+            self.assertEqual(generic_ipr_disclosure.by,                    PersonURI(uri="/api/v1/person/person/1/"))
             self.assertEqual(generic_ipr_disclosure.compliant,             True)
             self.assertEqual(generic_ipr_disclosure.docs,                  [])
             self.assertEqual(generic_ipr_disclosure.holder_contact_email,  "kayew@i-dns.net")
             self.assertEqual(generic_ipr_disclosure.holder_contact_info,   "Legal Counsel\r\ni-DNS.net International, Inc.\r\n#24-02 Suntec Tower Three\r\nSingapore 038988\r\nT: (65) 2486-163\r\nF: (65) 2486-199\r\n")
             self.assertEqual(generic_ipr_disclosure.holder_contact_name,   "Ka Yew Leong")
             self.assertEqual(generic_ipr_disclosure.holder_legal_name,     "i-DNS.net International,")
             self.assertEqual(generic_ipr_disclosure.id,                    4061)
-            self.assertEqual(generic_ipr_disclosure.iprdisclosurebase_ptr, IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/4061/"))
+            self.assertEqual(generic_ipr_disclosure.iprdisclosurebase_ptr, IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/4061/"))
             self.assertEqual(generic_ipr_disclosure.notes,                 "More information can be found in i-DNS.net International Technology Position\r\nPaper at http://www.i-DNS.net/tech/techposition.html")
             self.assertEqual(generic_ipr_disclosure.other_designations,    "")
-            self.assertEqual(generic_ipr_disclosure.rel,                   [IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/3150/")])
-            self.assertEqual(generic_ipr_disclosure.resource_uri,          GenericIPRDisclosureURI("/api/v1/ipr/genericiprdisclosure/4061/"))
-            self.assertEqual(generic_ipr_disclosure.state,                 IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/parked/"))
+            self.assertEqual(generic_ipr_disclosure.rel,                   [IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/3150/")])
+            self.assertEqual(generic_ipr_disclosure.resource_uri,          GenericIPRDisclosureURI(uri="/api/v1/ipr/genericiprdisclosure/4061/"))
+            self.assertEqual(generic_ipr_disclosure.state,                 IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/parked/"))
             self.assertEqual(generic_ipr_disclosure.statement,             "\r\nThe Patent Holder states that its position with respect to licensing any patent claims\r\ncontained in the patent(s) or patent application(s) disclosed above that would necessarily\r\nbe infringed by implementation of the technology required by the relevant IETF\r\nspecification (\"Necessary Patent Claims\"), for the purpose of implementing such\r\nspecification, is as follows(select one licensing declaration option only):\r\n\r\n\r\n    See text box below for licensing declaration.\r\n\r\n\r\nLicensing information, comments, notes or URL for further information:\r\n\r\nIn accordance with Section 10 of RFC 2026, i-DNS.net International, Inc.\r\n  (i-DNS.net) hereby states that if i-DNS.net&#39;s contribution is incorporated\r\n  into an IETF standard and i-DNS.net has patents or patent applications over\r\n  such contribution, i-DNS.net is willing to grant a license to such patent\r\n  rights to the extent it is necessary to the implementation of the standard\r\n  and on fair, reasonable and non-discriminatory terms based on reciprocity.\r\n")
             self.assertEqual(generic_ipr_disclosure.submitter_email,       "kayew@i-dns.net")
             self.assertEqual(generic_ipr_disclosure.submitter_name,        "Ka Yew Leong")
             self.assertEqual(generic_ipr_disclosure.time,                  datetime.fromisoformat("2020-03-21T04:35:16-07:00"))
             self.assertEqual(generic_ipr_disclosure.title,                 "i-DNS.net International,'s General License Statement")
         else:
             self.fail("Cannot find generic IPR disclosure")
@@ -2562,47 +2629,47 @@
 
     def test_generic_ipr_disclosures(self) -> None:
         generic_ipr_disclosures = self.dt.generic_ipr_disclosures()
         self.assertIsNot(generic_ipr_disclosures, None)
 
 
     def test_generic_ipr_disclosures_by(self) -> None:
-        generic_ipr_disclosures = self.dt.generic_ipr_disclosures(by=self.dt.person(PersonURI("/api/v1/person/person/1/")))
+        generic_ipr_disclosures = self.dt.generic_ipr_disclosures(by=self.dt.person(PersonURI(uri="/api/v1/person/person/1/")))
         self.assertIsNot(generic_ipr_disclosures, None)
 
 
     def test_generic_ipr_disclosures_holder_legal_name(self) -> None:
         generic_ipr_disclosures = self.dt.generic_ipr_disclosures(holder_legal_name="i-DNS.net International,")
         self.assertIsNot(generic_ipr_disclosures, None)
 
 
     def test_generic_ipr_disclosures_holder_contact_name(self) -> None:
         generic_ipr_disclosures = self.dt.generic_ipr_disclosures(holder_contact_name="Ka Yew Leong")
         self.assertIsNot(generic_ipr_disclosures, None)
 
 
     def test_generic_ipr_disclosures_state(self) -> None:
-        generic_ipr_disclosures = self.dt.generic_ipr_disclosures(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/parked/")))
+        generic_ipr_disclosures = self.dt.generic_ipr_disclosures(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/parked/")))
         self.assertIsNot(generic_ipr_disclosures, None)
 
 
     def test_generic_ipr_disclosures_submitter_email(self) -> None:
         generic_ipr_disclosures = self.dt.generic_ipr_disclosures(submitter_email="kayew@i-dns.net")
         self.assertIsNot(generic_ipr_disclosures, None)
 
 
     def test_generic_ipr_disclosures_submitter_name(self) -> None:
         generic_ipr_disclosures = self.dt.generic_ipr_disclosures(submitter_name="Ka Yew Leong")
         self.assertIsNot(generic_ipr_disclosures, None)
 
 
     def test_ipr_license_type(self) -> None:
-        ipr_license_type = self.dt.ipr_license_type(IPRLicenseTypeURI("/api/v1/name/iprlicensetypename/no-license/"))
+        ipr_license_type = self.dt.ipr_license_type(IPRLicenseTypeURI(uri="/api/v1/name/iprlicensetypename/no-license/"))
         if ipr_license_type is not None:
-            self.assertEqual(ipr_license_type.resource_uri, IPRLicenseTypeURI("/api/v1/name/iprlicensetypename/no-license/"))
+            self.assertEqual(ipr_license_type.resource_uri, IPRLicenseTypeURI(uri="/api/v1/name/iprlicensetypename/no-license/"))
             self.assertEqual(ipr_license_type.name,         "No License")
             self.assertEqual(ipr_license_type.used,         True)
             self.assertEqual(ipr_license_type.slug,         "no-license")
             self.assertEqual(ipr_license_type.desc,         "a) No License Required for Implementers")
             self.assertEqual(ipr_license_type.order,        1)
         else:
             self.fail("Cannot find IPR license type")
@@ -2617,37 +2684,37 @@
         self.assertEqual(types[3].slug,  "reasonable")
         self.assertEqual(types[4].slug,  "royalty-free")
         self.assertEqual(types[5].slug,  "see-below")
         self.assertEqual(types[6].slug,  "unwilling-to-commit")
 
 
     def test_holder_ipr_disclosure(self) -> None:
-        holder_ipr_disclosure = self.dt.holder_ipr_disclosure(HolderIPRDisclosureURI("/api/v1/ipr/holderiprdisclosure/4176/"))
+        holder_ipr_disclosure = self.dt.holder_ipr_disclosure(HolderIPRDisclosureURI(uri="/api/v1/ipr/holderiprdisclosure/4176/"))
         if holder_ipr_disclosure is not None:
-            self.assertEqual(holder_ipr_disclosure.by,                                   PersonURI("/api/v1/person/person/1/"))
+            self.assertEqual(holder_ipr_disclosure.by,                                   PersonURI(uri="/api/v1/person/person/1/"))
             self.assertEqual(holder_ipr_disclosure.compliant,                            True)
-            self.assertEqual(holder_ipr_disclosure.docs,                                 [DocumentAliasURI("/api/v1/doc/docalias/draft-gandhi-spring-twamp-srpm/")])
+            self.assertEqual(holder_ipr_disclosure.docs,                                 [DocumentURI(uri="/api/v1/doc/document/draft-gandhi-spring-twamp-srpm/")])
             self.assertEqual(holder_ipr_disclosure.has_patent_pending,                   False)
             self.assertEqual(holder_ipr_disclosure.holder_contact_email,                 "francesco.battipede@telecomitalia.it")
             self.assertEqual(holder_ipr_disclosure.holder_contact_info,                  "Technology Innovation-Patents\r\nVia G. Reiss Romoli 274\r\n10148 Torino - Italy\r\nT: +39 011 228 5580")
             self.assertEqual(holder_ipr_disclosure.holder_contact_name,                  "Francesco Battipede")
             self.assertEqual(holder_ipr_disclosure.holder_legal_name,                    "Telecom Italia SpA")
             self.assertEqual(holder_ipr_disclosure.id,                                   4176)
             self.assertEqual(holder_ipr_disclosure.ietfer_contact_email,                 "mauro.cociglio@telecomitalia.it")
             self.assertEqual(holder_ipr_disclosure.ietfer_contact_info,                  "Technology Innovation\r\nVia G. Reiss Romoli 274\r\n10148 Torino - Italy\r\nT: +39 011 228 5028")
             self.assertEqual(holder_ipr_disclosure.ietfer_name,                          "Mauro Cociglio")
-            self.assertEqual(holder_ipr_disclosure.iprdisclosurebase_ptr,                IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/4176/"))
-            self.assertEqual(holder_ipr_disclosure.licensing,                            IPRLicenseTypeURI("/api/v1/name/iprlicensetypename/reasonable/"))
+            self.assertEqual(holder_ipr_disclosure.iprdisclosurebase_ptr,                IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/4176/"))
+            self.assertEqual(holder_ipr_disclosure.licensing,                            IPRLicenseTypeURI(uri="/api/v1/name/iprlicensetypename/reasonable/"))
             self.assertEqual(holder_ipr_disclosure.licensing_comments,                   "This undertaking is made subject to the condition that those who seek licences agree to reciprocate.")
             self.assertEqual(holder_ipr_disclosure.notes,                                "")
             self.assertEqual(holder_ipr_disclosure.other_designations,                   "")
             self.assertEqual(holder_ipr_disclosure.patent_info,                          "Number: AR074847B1, CN2008801327719, EP2374241B, KR101475347, US8451734\nInventor: Mauro Cociglio, Luca Maria Castaldelli, Domenico Laforgia\nTitle: Measurement of data loss in a communication network\nDate: 2008-12-22\nNotes: EP2374241B: validated in DE, FI, FR, GB, IT, NL, SE")
             self.assertEqual(holder_ipr_disclosure.rel,                                  [])
-            self.assertEqual(holder_ipr_disclosure.resource_uri,                         HolderIPRDisclosureURI("/api/v1/ipr/holderiprdisclosure/4176/"))
-            self.assertEqual(holder_ipr_disclosure.state,                                IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/posted/"))
+            self.assertEqual(holder_ipr_disclosure.resource_uri,                         HolderIPRDisclosureURI(uri="/api/v1/ipr/holderiprdisclosure/4176/"))
+            self.assertEqual(holder_ipr_disclosure.state,                                IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/posted/"))
             self.assertEqual(holder_ipr_disclosure.submitter_claims_all_terms_disclosed, False)
             self.assertEqual(holder_ipr_disclosure.submitter_email,                      "francesco.battipede@telecomitalia.it")
             self.assertEqual(holder_ipr_disclosure.submitter_name,                       "Francesco Battipede")
             self.assertEqual(holder_ipr_disclosure.time,                                 datetime.fromisoformat("2020-06-08T02:44:12-07:00"))
             self.assertEqual(holder_ipr_disclosure.title,                                "Telecom Italia SpA's Statement about IPR related to draft-gandhi-spring-twamp-srpm")
         else:
             self.fail("Cannot find holder IPR disclosure")
@@ -2655,15 +2722,15 @@
 
     def test_holder_ipr_disclosures(self) -> None:
         holder_ipr_disclosures = self.dt.holder_ipr_disclosures()
         self.assertIsNot(holder_ipr_disclosures, None)
 
 
     def test_holder_ipr_disclosures_by(self) -> None:
-        holder_ipr_disclosures = self.dt.holder_ipr_disclosures(by=self.dt.person(PersonURI("/api/v1/person/person/1/")))
+        holder_ipr_disclosures = self.dt.holder_ipr_disclosures(by=self.dt.person(PersonURI(uri="/api/v1/person/person/1/")))
         self.assertIsNot(holder_ipr_disclosures, None)
 
 
     def test_holder_ipr_disclosures_holder_legal_name(self) -> None:
         holder_ipr_disclosures = self.dt.holder_ipr_disclosures(holder_legal_name="Telecom Italia SpA")
         self.assertIsNot(holder_ipr_disclosures, None)
 
@@ -2680,67 +2747,67 @@
 
     def test_holder_ipr_disclosures_ietfer_name(self) -> None:
         holder_ipr_disclosures = self.dt.holder_ipr_disclosures(ietfer_name="Mauro Cociglio")
         self.assertIsNot(holder_ipr_disclosures, None)
 
 
     def test_holder_ipr_disclosures_licensing(self) -> None:
-        holder_ipr_disclosures = self.dt.holder_ipr_disclosures(licensing=self.dt.ipr_license_type(IPRLicenseTypeURI("/api/v1/name/iprlicensetypename/reasonable/")))
+        holder_ipr_disclosures = self.dt.holder_ipr_disclosures(licensing=self.dt.ipr_license_type(IPRLicenseTypeURI(uri="/api/v1/name/iprlicensetypename/reasonable/")))
         self.assertIsNot(holder_ipr_disclosures, None)
 
 
     def test_holder_ipr_disclosures_state(self) -> None:
-        holder_ipr_disclosures = self.dt.holder_ipr_disclosures(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/posted/")))
+        holder_ipr_disclosures = self.dt.holder_ipr_disclosures(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/posted/")))
         self.assertIsNot(holder_ipr_disclosures, None)
 
 
     def test_holder_ipr_disclosures_submitter_email(self) -> None:
         holder_ipr_disclosures = self.dt.holder_ipr_disclosures(submitter_email="francesco.battipede@telecomitalia.it")
         self.assertIsNot(holder_ipr_disclosures, None)
 
 
     def test_holder_ipr_disclosures_submitter_name(self) -> None:
         holder_ipr_disclosures = self.dt.holder_ipr_disclosures(submitter_name="Francesco Battipede")
         self.assertIsNot(holder_ipr_disclosures, None)
 
 
     def test_thirdparty_ipr_disclosure(self) -> None:
-        thirdparty_ipr_disclosure = self.dt.thirdparty_ipr_disclosure(ThirdPartyIPRDisclosureURI("/api/v1/ipr/thirdpartyiprdisclosure/4153/"))
+        thirdparty_ipr_disclosure = self.dt.thirdparty_ipr_disclosure(ThirdPartyIPRDisclosureURI(uri="/api/v1/ipr/thirdpartyiprdisclosure/4153/"))
         if thirdparty_ipr_disclosure is not None:
-            self.assertEqual(thirdparty_ipr_disclosure.by,                                   PersonURI("/api/v1/person/person/1/"))
+            self.assertEqual(thirdparty_ipr_disclosure.by,                                   PersonURI(uri="/api/v1/person/person/1/"))
             self.assertEqual(thirdparty_ipr_disclosure.compliant,                            True)
-            self.assertEqual(thirdparty_ipr_disclosure.docs,                                 [DocumentAliasURI("/api/v1/doc/docalias/draft-mattsson-cfrg-det-sigs-with-noise/")])
+            self.assertEqual(thirdparty_ipr_disclosure.docs,                                 [DocumentURI(uri="/api/v1/doc/document/draft-mattsson-cfrg-det-sigs-with-noise/")])
             self.assertEqual(thirdparty_ipr_disclosure.has_patent_pending,                   False)
             self.assertEqual(thirdparty_ipr_disclosure.holder_legal_name,                    "QUALCOMM Incorporated")
             self.assertEqual(thirdparty_ipr_disclosure.id,                                   4153)
             self.assertEqual(thirdparty_ipr_disclosure.ietfer_contact_email,                 "bbrumley@gmail.com")
             self.assertEqual(thirdparty_ipr_disclosure.ietfer_contact_info,                  "")
             self.assertEqual(thirdparty_ipr_disclosure.ietfer_name,                          "Billy Brumley")
-            self.assertEqual(thirdparty_ipr_disclosure.iprdisclosurebase_ptr,                IPRDisclosureBaseURI("/api/v1/ipr/iprdisclosurebase/4153/"))
+            self.assertEqual(thirdparty_ipr_disclosure.iprdisclosurebase_ptr,                IPRDisclosureBaseURI(uri="/api/v1/ipr/iprdisclosurebase/4153/"))
             self.assertEqual(thirdparty_ipr_disclosure.notes,                                "")
             self.assertEqual(thirdparty_ipr_disclosure.other_designations,                   "")
             self.assertEqual(thirdparty_ipr_disclosure.patent_info,                          "Number: US9621525B2\nInventor: Billy Bob Brumley\nTitle: Semi-deterministic digital signature generation\nDate: 2014-06-02")
             self.assertEqual(thirdparty_ipr_disclosure.rel,                                  [])
-            self.assertEqual(thirdparty_ipr_disclosure.resource_uri,                         ThirdPartyIPRDisclosureURI("/api/v1/ipr/thirdpartyiprdisclosure/4153/"))
-            self.assertEqual(thirdparty_ipr_disclosure.state,                                IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/parked/"))
+            self.assertEqual(thirdparty_ipr_disclosure.resource_uri,                         ThirdPartyIPRDisclosureURI(uri="/api/v1/ipr/thirdpartyiprdisclosure/4153/"))
+            self.assertEqual(thirdparty_ipr_disclosure.state,                                IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/parked/"))
             self.assertEqual(thirdparty_ipr_disclosure.submitter_email,                      "bbrumley@gmail.com")
             self.assertEqual(thirdparty_ipr_disclosure.submitter_name,                       "Billy Brumley")
             self.assertEqual(thirdparty_ipr_disclosure.time,                                 datetime.fromisoformat("2020-05-14T20:32:24-07:00"))
             self.assertEqual(thirdparty_ipr_disclosure.title,                                "Billy Brumley's Statement about IPR related to draft-mattsson-cfrg-det-sigs-with-noise belonging to QUALCOMM Incorporated")
         else:
             self.fail("Cannot find third party IPR disclosure")
 
 
     def test_thirdparty_ipr_disclosures(self) -> None:
         thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures()
         self.assertIsNot(thirdparty_ipr_disclosures, None)
 
 
     def test_thirdparty_ipr_disclosures_by(self) -> None:
-        thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures(by=self.dt.person(PersonURI("/api/v1/person/person/1/")))
+        thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures(by=self.dt.person(PersonURI(uri="/api/v1/person/person/1/")))
         self.assertIsNot(thirdparty_ipr_disclosures, None)
 
 
     def test_thirdparty_ipr_disclosures_holder_legal_name(self) -> None:
         thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures(holder_legal_name="QUALCOMM Incorporated")
         self.assertIsNot(thirdparty_ipr_disclosures, None)
 
@@ -2752,15 +2819,15 @@
 
     def test_thirdparty_ipr_disclosures_ietfer_name(self) -> None:
         thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures(ietfer_name="Billy Brumley")
         self.assertIsNot(thirdparty_ipr_disclosures, None)
 
 
     def test_thirdparty_ipr_disclosures_state(self) -> None:
-        thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI("/api/v1/name/iprdisclosurestatename/pending/")))
+        thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures(state=self.dt.ipr_disclosure_state(IPRDisclosureStateURI(uri="/api/v1/name/iprdisclosurestatename/pending/")))
         self.assertIsNot(thirdparty_ipr_disclosures, None)
 
 
     def test_thirdparty_ipr_disclosures_submitter_email(self) -> None:
         thirdparty_ipr_disclosures = self.dt.thirdparty_ipr_disclosures(submitter_email="bbrumley@gmail.com")
         self.assertIsNot(thirdparty_ipr_disclosures, None)
 
@@ -2770,30 +2837,30 @@
         self.assertIsNot(thirdparty_ipr_disclosures, None)
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to reviews:
 
     def test_review_assignment_state(self) -> None:
-        rev_assign_state = self.dt.review_assignment_state(ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/accepted/"))
+        rev_assign_state = self.dt.review_assignment_state(ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/accepted/"))
         if rev_assign_state is not None:
-            self.assertEqual(rev_assign_state.resource_uri, ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/accepted/"))
+            self.assertEqual(rev_assign_state.resource_uri, ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/accepted/"))
             self.assertEqual(rev_assign_state.name,         "Accepted")
             self.assertEqual(rev_assign_state.used,         True)
             self.assertEqual(rev_assign_state.slug,         "accepted")
             self.assertEqual(rev_assign_state.desc,         "The reviewer has accepted the assignment")
             self.assertEqual(rev_assign_state.order,        0)
         else:
             self.fail("Cannot find review assignment state")
 
 
     def test_review_assignment_state_from_slug(self) -> None:
         rev_assign_state = self.dt.review_assignment_state_from_slug("accepted")
         if rev_assign_state is not None:
-            self.assertEqual(rev_assign_state.resource_uri, ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/accepted/"))
+            self.assertEqual(rev_assign_state.resource_uri, ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/accepted/"))
             self.assertEqual(rev_assign_state.name,         "Accepted")
             self.assertEqual(rev_assign_state.used,         True)
             self.assertEqual(rev_assign_state.slug,         "accepted")
             self.assertEqual(rev_assign_state.desc,         "The reviewer has accepted the assignment")
             self.assertEqual(rev_assign_state.order,        0)
         else:
             self.fail("Cannot find review assignment state")
@@ -2810,30 +2877,30 @@
         self.assertEqual(states[5].slug, "part-completed")
         self.assertEqual(states[6].slug, "rejected")
         self.assertEqual(states[7].slug, "unknown")
         self.assertEqual(states[8].slug, "withdrawn")
 
 
     def test_review_result_type(self) -> None:
-        review_result_type = self.dt.review_result_type(ReviewResultTypeURI("/api/v1/name/reviewresultname/serious-issues/"))
+        review_result_type = self.dt.review_result_type(ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/serious-issues/"))
         if review_result_type is not None:
-            self.assertEqual(review_result_type.resource_uri, ReviewResultTypeURI("/api/v1/name/reviewresultname/serious-issues/"))
+            self.assertEqual(review_result_type.resource_uri, ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/serious-issues/"))
             self.assertEqual(review_result_type.name,         "Serious Issues")
             self.assertEqual(review_result_type.used,         True)
             self.assertEqual(review_result_type.slug,         "serious-issues")
             self.assertEqual(review_result_type.desc,         "")
             self.assertEqual(review_result_type.order,        1)
         else:
             self.fail("Cannot find review result type")
 
 
     def test_review_result_type_from_slug(self) -> None:
         review_result_type = self.dt.review_result_type_from_slug("serious-issues")
         if review_result_type is not None:
-            self.assertEqual(review_result_type.resource_uri, ReviewResultTypeURI("/api/v1/name/reviewresultname/serious-issues/"))
+            self.assertEqual(review_result_type.resource_uri, ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/serious-issues/"))
             self.assertEqual(review_result_type.name,         "Serious Issues")
             self.assertEqual(review_result_type.used,         True)
             self.assertEqual(review_result_type.slug,         "serious-issues")
             self.assertEqual(review_result_type.desc,         "")
             self.assertEqual(review_result_type.order,        1)
         else:
             self.fail("Cannot find review result type")
@@ -2850,30 +2917,30 @@
         self.assertEqual(types[5].slug, "ready-issues")
         self.assertEqual(types[6].slug, "ready-nits")
         self.assertEqual(types[7].slug, "right-track")
         self.assertEqual(types[8].slug, "serious-issues")
 
 
     def test_review_type(self) -> None:
-        review_type = self.dt.review_type(ReviewTypeURI("/api/v1/name/reviewtypename/early/"))
+        review_type = self.dt.review_type(ReviewTypeURI(uri="/api/v1/name/reviewtypename/early/"))
         if review_type is not None:
-            self.assertEqual(review_type.resource_uri, ReviewTypeURI("/api/v1/name/reviewtypename/early/"))
+            self.assertEqual(review_type.resource_uri, ReviewTypeURI(uri="/api/v1/name/reviewtypename/early/"))
             self.assertEqual(review_type.name,         "Early")
             self.assertEqual(review_type.used,         True)
             self.assertEqual(review_type.slug,         "early")
             self.assertEqual(review_type.desc,         "")
             self.assertEqual(review_type.order,        1)
         else:
             self.fail("Cannot find review type")
 
 
     def test_review_type_from_slug(self) -> None:
         review_type = self.dt.review_type_from_slug("early")
         if review_type is not None:
-            self.assertEqual(review_type.resource_uri, ReviewTypeURI("/api/v1/name/reviewtypename/early/"))
+            self.assertEqual(review_type.resource_uri, ReviewTypeURI(uri="/api/v1/name/reviewtypename/early/"))
             self.assertEqual(review_type.name,         "Early")
             self.assertEqual(review_type.used,         True)
             self.assertEqual(review_type.slug,         "early")
             self.assertEqual(review_type.desc,         "")
             self.assertEqual(review_type.order,        1)
         else:
             self.fail("Cannot find review type")
@@ -2884,30 +2951,30 @@
         self.assertEqual(len(types), 3)
         self.assertEqual(types[0].slug, "early")
         self.assertEqual(types[1].slug, "lc")
         self.assertEqual(types[2].slug, "telechat")
 
 
     def test_review_request_state(self) -> None:
-        review_request_state = self.dt.review_request_state(ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/assigned/"))
+        review_request_state = self.dt.review_request_state(ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/assigned/"))
         if review_request_state is not None:
-            self.assertEqual(review_request_state.resource_uri, ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/assigned/"))
+            self.assertEqual(review_request_state.resource_uri, ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/assigned/"))
             self.assertEqual(review_request_state.name,         "Assigned")
             self.assertEqual(review_request_state.used,         True)
             self.assertEqual(review_request_state.slug,         "assigned")
             self.assertEqual(review_request_state.desc,         "The ReviewRequest has been assigned to at least one reviewer")
             self.assertEqual(review_request_state.order,        0)
         else:
             self.fail("Cannot find review request state")
 
 
     def test_review_request_state_from_slug(self) -> None:
         review_request_state = self.dt.review_request_state_from_slug("assigned")
         if review_request_state is not None:
-            self.assertEqual(review_request_state.resource_uri, ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/assigned/"))
+            self.assertEqual(review_request_state.resource_uri, ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/assigned/"))
             self.assertEqual(review_request_state.name,         "Assigned")
             self.assertEqual(review_request_state.used,         True)
             self.assertEqual(review_request_state.slug,         "assigned")
             self.assertEqual(review_request_state.desc,         "The ReviewRequest has been assigned to at least one reviewer")
             self.assertEqual(review_request_state.order,        0)
         else:
             self.fail("Cannot find review request state")
@@ -2927,196 +2994,198 @@
         self.assertEqual(states[ 8].slug, "rejected")
         self.assertEqual(states[ 9].slug, "requested")
         self.assertEqual(states[10].slug, "unknown")
         self.assertEqual(states[11].slug, "withdrawn")
 
 
     def test_review_request(self) -> None:
-        review_request = self.dt.review_request(ReviewRequestURI("/api/v1/review/reviewrequest/12006/"))
+        review_request = self.dt.review_request(ReviewRequestURI(uri="/api/v1/review/reviewrequest/12006/"))
         if review_request is not None:
             self.assertEqual(review_request.comment,       "")
             self.assertEqual(review_request.deadline,      "2019-05-30")
-            self.assertEqual(review_request.doc,           DocumentURI("/api/v1/doc/document/draft-ietf-pce-inter-area-as-applicability/"))
+            self.assertEqual(review_request.doc,           DocumentURI(uri="/api/v1/doc/document/draft-ietf-pce-inter-area-as-applicability/"))
             self.assertEqual(review_request.id,            12006)
-            self.assertEqual(review_request.requested_by,  PersonURI("/api/v1/person/person/1/"))
+            self.assertEqual(review_request.requested_by,  PersonURI(uri="/api/v1/person/person/1/"))
             self.assertEqual(review_request.requested_rev, "")
-            self.assertEqual(review_request.resource_uri,  ReviewRequestURI("/api/v1/review/reviewrequest/12006/"))
-            self.assertEqual(review_request.state,         ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/assigned/"))
-            self.assertEqual(review_request.team,          GroupURI("/api/v1/group/group/1976/"))
+            self.assertEqual(review_request.resource_uri,  ReviewRequestURI(uri="/api/v1/review/reviewrequest/12006/"))
+            self.assertEqual(review_request.state,         ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/assigned/"))
+            self.assertEqual(review_request.team,          GroupURI(uri="/api/v1/group/group/1976/"))
             self.assertEqual(review_request.time,          datetime.fromisoformat("2019-05-16T13:57:00-07:00"))
-            self.assertEqual(review_request.type,          ReviewTypeURI("/api/v1/name/reviewtypename/lc/"))
+            self.assertEqual(review_request.type,          ReviewTypeURI(uri="/api/v1/name/reviewtypename/lc/"))
         else:
             self.fail("Cannot find review request")
 
 
     def test_review_requests(self) -> None:
         review_requests = self.dt.review_requests()
         self.assertIsNot(review_requests, None)
 
 
     def test_review_requests_doc(self) -> None:
-        review_requests = list(self.dt.review_requests(doc=self.dt.document(DocumentURI("/api/v1/doc/document/draft-davis-t-langtag-ext/"))))
+        review_requests = list(self.dt.review_requests(doc=self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-davis-t-langtag-ext/"))))
         self.assertEqual(len(review_requests), 2)
         self.assertEqual(review_requests[0].id, 1)
         self.assertEqual(review_requests[1].id, 4457)
 
 
     def test_review_requests_requested_by(self) -> None:
-        review_requests = self.dt.review_requests(requested_by=self.dt.person(PersonURI("/api/v1/person/person/1/")))
+        review_requests = self.dt.review_requests(requested_by=self.dt.person(PersonURI(uri="/api/v1/person/person/1/")))
         self.assertIsNot(review_requests, None)
 
 
     def test_review_requests_state(self) -> None:
-        review_requests = self.dt.review_requests(state=self.dt.review_request_state(ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/assigned/")))
+        review_requests = self.dt.review_requests(state=self.dt.review_request_state(ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/assigned/")))
         self.assertIsNot(review_requests, None)
 
 
     def test_review_requests_team(self) -> None:
-        review_requests = self.dt.review_requests(team=self.dt.group(GroupURI("/api/v1/group/group/1261/")))
+        review_requests = self.dt.review_requests(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1261/")))
         self.assertIsNot(review_requests, None)
 
 
     def test_review_requests_type(self) -> None:
-        review_requests = self.dt.review_requests(type=self.dt.review_type(ReviewTypeURI("/api/v1/name/reviewtypename/telechat/")))
+        review_requests = self.dt.review_requests(type=self.dt.review_type(ReviewTypeURI(uri="/api/v1/name/reviewtypename/telechat/")))
         self.assertIsNot(review_requests, None)
 
 
     def test_review_assignment(self) -> None:
-        review_assignment = self.dt.review_assignment(ReviewAssignmentURI("/api/v1/review/reviewassignment/10000/"))
+        review_assignment = self.dt.review_assignment(ReviewAssignmentURI(uri="/api/v1/review/reviewassignment/10000/"))
         if review_assignment is not None:
             self.assertEqual(review_assignment.assigned_on,    datetime.fromisoformat("2011-01-18T22:58:05-07:00"))
             self.assertEqual(review_assignment.completed_on,   datetime.fromisoformat("2011-02-26T12:33:30-07:00"))
             self.assertEqual(review_assignment.id,             10000)
             self.assertEqual(review_assignment.mailarch_url,   "http://www.ietf.org/mail-archive/web/secdir/current/msg02466.html")
-            self.assertEqual(review_assignment.resource_uri,   ReviewAssignmentURI("/api/v1/review/reviewassignment/10000/"))
+            self.assertEqual(review_assignment.resource_uri,   ReviewAssignmentURI(uri="/api/v1/review/reviewassignment/10000/"))
             self.assertEqual(review_assignment.result,         None)
-            self.assertEqual(review_assignment.review,         DocumentURI("/api/v1/doc/document/review-holsten-about-uri-scheme-secdir-lc-laganier-2011-02-26/"))
-            self.assertEqual(review_assignment.review_request, ReviewRequestURI("/api/v1/review/reviewrequest/4229/"))
+            self.assertEqual(review_assignment.review,         DocumentURI(uri="/api/v1/doc/document/review-holsten-about-uri-scheme-secdir-lc-laganier-2011-02-26/"))
+            self.assertEqual(review_assignment.review_request, ReviewRequestURI(uri="/api/v1/review/reviewrequest/4229/"))
             self.assertEqual(review_assignment.reviewed_rev,   "")
-            self.assertEqual(review_assignment.reviewer,       EmailURI("/api/v1/person/email/julien.ietf@gmail.com/"))
-            self.assertEqual(review_assignment.state,          ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/completed/"))
+            self.assertEqual(review_assignment.reviewer,       EmailURI(uri="/api/v1/person/email/julien.ietf@gmail.com/"))
+            self.assertEqual(review_assignment.state,          ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/completed/"))
         else:
             self.fail("Cannot find review assignment")
 
 
     def test_review_assignments(self) -> None:
         review_assignments = self.dt.review_assignments()
         self.assertIsNot(review_assignments, None)
 
 
     def test_review_assignments_result(self) -> None:
-        review_assignments = self.dt.review_assignments(result=self.dt.review_result_type(ReviewResultTypeURI("/api/v1/name/reviewresultname/nits/")))
+        review_assignments = self.dt.review_assignments(result=self.dt.review_result_type(ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/nits/")))
         self.assertIsNot(review_assignments, None)
 
 
     def test_review_assignments_review_request(self) -> None:
-        review_assignments = list(self.dt.review_assignments(review_request=self.dt.review_request(ReviewRequestURI("/api/v1/review/reviewrequest/8354/"))))
+        review_assignments = list(self.dt.review_assignments(review_request=self.dt.review_request(ReviewRequestURI(uri="/api/v1/review/reviewrequest/8354/"))))
         self.assertEqual(len(review_assignments),  1)
         self.assertEqual(review_assignments[0].id, 1458)
 
 
     def test_review_assignments_reviewer(self) -> None:
-        review_assignments = self.dt.review_assignments(reviewer=self.dt.email(EmailURI("/api/v1/person/email/csp@csperkins.org/")))
+        review_assignments = self.dt.review_assignments(reviewer=self.dt.email(EmailURI(uri="/api/v1/person/email/csp@csperkins.org/")))
         self.assertIsNot(review_assignments, None)
 
 
     def test_review_assignments_state(self) -> None:
-        review_assignments = self.dt.review_assignments(state=self.dt.review_assignment_state(ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/completed/")))
+        review_assignments = self.dt.review_assignments(state=self.dt.review_assignment_state(ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/completed/")))
         self.assertIsNot(review_assignments, None)
 
 
     def test_review_wish(self) -> None:
-        review_wish = self.dt.review_wish(ReviewWishURI("/api/v1/review/reviewwish/7/"))
+        review_wish = self.dt.review_wish(ReviewWishURI(uri="/api/v1/review/reviewwish/63/"))
         if review_wish is not None:
-            self.assertEqual(review_wish.doc,          DocumentURI("/api/v1/doc/document/draft-ietf-perc-double/"))
-            self.assertEqual(review_wish.id,           7)
-            self.assertEqual(review_wish.person,       PersonURI("/api/v1/person/person/5376/"))
-            self.assertEqual(review_wish.resource_uri, ReviewWishURI("/api/v1/review/reviewwish/7/"))
-            self.assertEqual(review_wish.team,         GroupURI("/api/v1/group/group/1972/"))
-            self.assertEqual(review_wish.time,         datetime.fromisoformat("2018-05-10T08:41:39-07:00"))
+            self.assertEqual(review_wish.doc,          DocumentURI(uri="/api/v1/doc/document/draft-arkko-ipv6-transition-guidelines/"))
+            self.assertEqual(review_wish.id,           63)
+            self.assertEqual(review_wish.person,       PersonURI(uri="/api/v1/person/person/113626/"))
+            self.assertEqual(review_wish.resource_uri, ReviewWishURI(uri="/api/v1/review/reviewwish/63/"))
+            self.assertEqual(review_wish.team,         GroupURI(uri="/api/v1/group/group/1976/"))
+            self.assertEqual(review_wish.time,         datetime.fromisoformat("2022-09-15T11:35:19+00:00"))
         else:
             self.fail("Cannot find review wish")
 
 
     def test_review_wishes(self) -> None:
         review_wishes = self.dt.review_wishes()
         self.assertIsNot(review_wishes, None)
 
 
     def test_review_wishes_doc(self) -> None:
-        review_wishes = list(self.dt.review_wishes(doc=self.dt.document(DocumentURI("/api/v1/doc/document/draft-ietf-perc-double/"))))
+        review_wishes = list(self.dt.review_wishes(doc=self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-arkko-ipv6-transition-guidelines/"))))
         self.assertEqual(len(review_wishes),  1)
-        self.assertEqual(review_wishes[0].id, 7)
+        self.assertEqual(review_wishes[0].id, 63)
 
 
     def test_review_wishes_person(self) -> None:
-        review_wishes = list(self.dt.review_wishes(person=self.dt.person(PersonURI("/api/v1/person/person/5376/"))))
-        self.assertEqual(len(review_wishes),  2)
-        self.assertEqual(review_wishes[0].id, 7)
-        self.assertEqual(review_wishes[1].id, 43)
+        review_wishes = list(self.dt.review_wishes(person=self.dt.person(PersonURI(uri="/api/v1/person/person/113626/"))))
+        self.assertEqual(len(review_wishes),  7)
+        self.assertEqual(review_wishes[0].id, 60)
+        self.assertEqual(review_wishes[1].id, 61)
+        self.assertEqual(review_wishes[2].id, 62)
+        self.assertEqual(review_wishes[3].id, 63)
+        self.assertEqual(review_wishes[4].id, 64)
+        self.assertEqual(review_wishes[5].id, 65)
+        self.assertEqual(review_wishes[6].id, 66)
 
 
     def test_review_wishes_team(self) -> None:
-        review_wishes = list(self.dt.review_wishes(team=self.dt.group(GroupURI("/api/v1/group/group/1972/")))) # GenART
-        self.assertEqual(len(review_wishes),  4)
-        self.assertEqual(review_wishes[0].id, 7)
-        self.assertEqual(review_wishes[1].id, 24)
-        self.assertEqual(review_wishes[2].id, 43)
-        self.assertEqual(review_wishes[3].id, 53)
+        review_wishes = list(self.dt.review_wishes(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1972/")))) # GenART
+        self.assertEqual(len(review_wishes),  1)
+        self.assertEqual(review_wishes[0].id, 24)
 
 
     def test_reviewer_settings(self) -> None:
-        reviewer_settings = self.dt.reviewer_settings(ReviewerSettingsURI("/api/v1/review/reviewersettings/1/"))
+        reviewer_settings = self.dt.reviewer_settings(ReviewerSettingsURI(uri="/api/v1/review/reviewersettings/1/"))
         if reviewer_settings is not None:
             self.assertEqual(reviewer_settings.expertise,                   "")
             self.assertEqual(reviewer_settings.filter_re,                   "^draft-carpenter-.*$")
             self.assertEqual(reviewer_settings.id,                          1)
             self.assertEqual(reviewer_settings.min_interval,                14)
-            self.assertEqual(reviewer_settings.person,                      PersonURI("/api/v1/person/person/1958/"))
+            self.assertEqual(reviewer_settings.person,                      PersonURI(uri="/api/v1/person/person/1958/"))
             self.assertEqual(reviewer_settings.remind_days_before_deadline, 3)
             self.assertEqual(reviewer_settings.remind_days_open_reviews,    None)
             self.assertEqual(reviewer_settings.request_assignment_next,     False)
-            self.assertEqual(reviewer_settings.resource_uri,                ReviewerSettingsURI("/api/v1/review/reviewersettings/1/"))
+            self.assertEqual(reviewer_settings.resource_uri,                ReviewerSettingsURI(uri="/api/v1/review/reviewersettings/1/"))
             self.assertEqual(reviewer_settings.skip_next,                   0)
-            self.assertEqual(reviewer_settings.team,                        GroupURI("/api/v1/group/group/1972/"))
+            self.assertEqual(reviewer_settings.team,                        GroupURI(uri="/api/v1/group/group/1972/"))
         else:
             self.fail("Cannot find reviewer settings")
 
 
     def test_reviewer_settings_all(self) -> None:
         reviewer_settings = self.dt.reviewer_settings_all()
         self.assertIsNot(reviewer_settings, None)
 
 
     def test_reviewer_settings_all_person(self) -> None:
-        reviewer_settings = list(self.dt.reviewer_settings_all(person=self.dt.person(PersonURI("/api/v1/person/person/1958/"))))
+        reviewer_settings = list(self.dt.reviewer_settings_all(person=self.dt.person(PersonURI(uri="/api/v1/person/person/1958/"))))
         self.assertEqual(len(reviewer_settings),  1)
         self.assertEqual(reviewer_settings[0].id, 1)
 
 
     def test_reviewer_settings_all_team(self) -> None:
-        reviewer_settings = self.dt.reviewer_settings_all(team=self.dt.group(GroupURI("/api/v1/group/group/1972/")))
+        reviewer_settings = self.dt.reviewer_settings_all(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1972/")))
         self.assertIsNot(reviewer_settings, None)
 
 
     def test_historical_unavailable_period(self) -> None:
-        historical_unavailable_period = self.dt.historical_unavailable_period(HistoricalUnavailablePeriodURI("/api/v1/review/historicalunavailableperiod/29/"))
+        historical_unavailable_period = self.dt.historical_unavailable_period(HistoricalUnavailablePeriodURI(uri="/api/v1/review/historicalunavailableperiod/29/"))
         if historical_unavailable_period is not None:
             self.assertEqual(historical_unavailable_period.availability,          "unavailable")
             self.assertEqual(historical_unavailable_period.end_date,              "2020-05-15")
             self.assertEqual(historical_unavailable_period.history_change_reason, "Set end date of unavailability period: Francis Dupont is unavailable in genart 2020-03-16 - 2020-05-15")
             self.assertEqual(historical_unavailable_period.history_date,          datetime.fromisoformat("2020-05-11T03:40:02-07:00"))
             self.assertEqual(historical_unavailable_period.history_id,            29)
             self.assertEqual(historical_unavailable_period.history_type,          "~")
             self.assertEqual(historical_unavailable_period.id,                    334)
-            self.assertEqual(historical_unavailable_period.person,                PersonURI("/api/v1/person/person/106670/"))
+            self.assertEqual(historical_unavailable_period.person,                PersonURI(uri="/api/v1/person/person/106670/"))
             self.assertEqual(historical_unavailable_period.reason,                "")
-            self.assertEqual(historical_unavailable_period.resource_uri,          HistoricalUnavailablePeriodURI("/api/v1/review/historicalunavailableperiod/29/"))
+            self.assertEqual(historical_unavailable_period.resource_uri,          HistoricalUnavailablePeriodURI(uri="/api/v1/review/historicalunavailableperiod/29/"))
             self.assertEqual(historical_unavailable_period.start_date,            "2020-03-16")
-            self.assertEqual(historical_unavailable_period.team,                  GroupURI("/api/v1/group/group/1972/"))
+            self.assertEqual(historical_unavailable_period.team,                  GroupURI(uri="/api/v1/group/group/1972/"))
         else:
             self.fail("Cannot find historical unavailable period")
 
 
     def test_historical_unavailable_periods(self) -> None:
         historical_unavailable_periods = self.dt.historical_unavailable_periods()
         self.assertIsNot(historical_unavailable_periods, None)
@@ -3130,51 +3199,51 @@
     def test_historical_unavailable_periods_id(self) -> None:
         historical_unavailable_periods = list(self.dt.historical_unavailable_periods(id=328))
         self.assertEqual(len(historical_unavailable_periods),          1)
         self.assertEqual(historical_unavailable_periods[0].history_id, 14)
 
 
     def test_historical_unavailable_periods_person(self) -> None:
-        historical_unavailable_periods = self.dt.historical_unavailable_periods(person=self.dt.person(PersonURI("/api/v1/person/person/119822/")))
+        historical_unavailable_periods = self.dt.historical_unavailable_periods(person=self.dt.person(PersonURI(uri="/api/v1/person/person/119822/")))
         self.assertIsNot(historical_unavailable_periods, None)
 
 
     def test_historical_unavailable_periods_team(self) -> None:
-        historical_unavailable_periods = self.dt.historical_unavailable_periods(team=self.dt.group(GroupURI("/api/v1/group/group/1261/")))
+        historical_unavailable_periods = self.dt.historical_unavailable_periods(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1261/")))
         self.assertIsNot(historical_unavailable_periods, None)
 
     def test_next_reviewer_in_team(self) -> None:
-        next_reviewer_in_team = self.dt.next_reviewer_in_team(NextReviewerInTeamURI("/api/v1/review/nextreviewerinteam/1/"))
+        next_reviewer_in_team = self.dt.next_reviewer_in_team(NextReviewerInTeamURI(uri="/api/v1/review/nextreviewerinteam/1/"))
         if next_reviewer_in_team is not None:
             self.assertEqual(next_reviewer_in_team.id,            1)
-            self.assertEqual(next_reviewer_in_team.next_reviewer, PersonURI("/api/v1/person/person/106670/"))
-            self.assertEqual(next_reviewer_in_team.resource_uri,  NextReviewerInTeamURI("/api/v1/review/nextreviewerinteam/1/"))
-            self.assertEqual(next_reviewer_in_team.team,          GroupURI("/api/v1/group/group/1972/"))
+            self.assertEqual(next_reviewer_in_team.next_reviewer, PersonURI(uri="/api/v1/person/person/106670/"))
+            self.assertEqual(next_reviewer_in_team.resource_uri,  NextReviewerInTeamURI(uri="/api/v1/review/nextreviewerinteam/1/"))
+            self.assertEqual(next_reviewer_in_team.team,          GroupURI(uri="/api/v1/group/group/1972/"))
         else:
             self.fail("Cannot find next reviewer in team")
 
 
     def test_historical_review_request(self) -> None:
-        historical_review_request = self.dt.historical_review_request(HistoricalReviewRequestURI("/api/v1/review/historicalreviewrequest/836/"))
+        historical_review_request = self.dt.historical_review_request(HistoricalReviewRequestURI(uri="/api/v1/review/historicalreviewrequest/836/"))
         if historical_review_request is not None:
             self.assertEqual(historical_review_request.comment,               "")
             self.assertEqual(historical_review_request.deadline,              "2020-06-09")
-            self.assertEqual(historical_review_request.doc,                   DocumentURI("/api/v1/doc/document/draft-ietf-capport-rfc7710bis/"))
+            self.assertEqual(historical_review_request.doc,                   DocumentURI(uri="/api/v1/doc/document/draft-ietf-capport-rfc7710bis/"))
             self.assertEqual(historical_review_request.history_change_reason, "Requested Telechat review by IOTDIR")
             self.assertEqual(historical_review_request.history_date,          datetime.fromisoformat("2020-05-27T07:12:46-07:00"))
             self.assertEqual(historical_review_request.history_id,            836)
             self.assertEqual(historical_review_request.history_type,          "+")
             self.assertEqual(historical_review_request.id,                    13428)
-            self.assertEqual(historical_review_request.requested_by,          PersonURI("/api/v1/person/person/105099/"))
+            self.assertEqual(historical_review_request.requested_by,          PersonURI(uri="/api/v1/person/person/105099/"))
             self.assertEqual(historical_review_request.requested_rev,         "")
-            self.assertEqual(historical_review_request.resource_uri,          HistoricalReviewRequestURI("/api/v1/review/historicalreviewrequest/836/"))
-            self.assertEqual(historical_review_request.state,                 ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/requested/"))
-            self.assertEqual(historical_review_request.team,                  GroupURI("/api/v1/group/group/1975/"))
+            self.assertEqual(historical_review_request.resource_uri,          HistoricalReviewRequestURI(uri="/api/v1/review/historicalreviewrequest/836/"))
+            self.assertEqual(historical_review_request.state,                 ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/requested/"))
+            self.assertEqual(historical_review_request.team,                  GroupURI(uri="/api/v1/group/group/1975/"))
             self.assertEqual(historical_review_request.time,                  datetime.fromisoformat("2020-05-27T07:12:37-07:00"))
-            self.assertEqual(historical_review_request.type,                  ReviewTypeURI("/api/v1/name/reviewtypename/telechat/"))
+            self.assertEqual(historical_review_request.type,                  ReviewTypeURI(uri="/api/v1/name/reviewtypename/telechat/"))
         else:
             self.fail("Cannot find historical review request")
 
 
     def test_historical_review_requests(self) -> None:
         historical_review_requests = self.dt.historical_review_requests()
         self.assertIsNot(historical_review_requests, None)
@@ -3187,135 +3256,135 @@
 
     def test_historical_review_requests_id(self) -> None:
         historical_review_requests = self.dt.historical_review_requests(id=13428)
         self.assertIsNot(historical_review_requests, None)
 
 
     def test_historical_review_requests_doc(self) -> None:
-        historical_review_requests = self.dt.historical_review_requests(doc=self.dt.document(DocumentURI("/api/v1/doc/document/draft-ietf-capport-rfc7710bis/")))
+        historical_review_requests = self.dt.historical_review_requests(doc=self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-ietf-capport-rfc7710bis/")))
         self.assertIsNot(historical_review_requests, None)
 
 
     def test_historical_review_requests_requested_by(self) -> None:
-        historical_review_requests = self.dt.historical_review_requests(requested_by=self.dt.person(PersonURI("/api/v1/person/person/105099/")))
+        historical_review_requests = self.dt.historical_review_requests(requested_by=self.dt.person(PersonURI(uri="/api/v1/person/person/105099/")))
         self.assertIsNot(historical_review_requests, None)
 
 
     def test_historical_review_requests_state(self) -> None:
-        historical_review_requests = self.dt.historical_review_requests(state=self.dt.review_request_state(ReviewRequestStateURI("/api/v1/name/reviewrequeststatename/requested/")))
+        historical_review_requests = self.dt.historical_review_requests(state=self.dt.review_request_state(ReviewRequestStateURI(uri="/api/v1/name/reviewrequeststatename/requested/")))
         self.assertIsNot(historical_review_requests, None)
 
 
     def test_historical_review_requests_team(self) -> None:
-        historical_review_requests = self.dt.historical_review_requests(team=self.dt.group(GroupURI("/api/v1/group/group/1975/")))
+        historical_review_requests = self.dt.historical_review_requests(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1975/")))
         self.assertIsNot(historical_review_requests, None)
 
 
     def test_historical_review_requests_type(self) -> None:
-        historical_review_requests = self.dt.historical_review_requests(type=self.dt.review_type(ReviewTypeURI("/api/v1/name/reviewtypename/telechat/")))
+        historical_review_requests = self.dt.historical_review_requests(type=self.dt.review_type(ReviewTypeURI(uri="/api/v1/name/reviewtypename/telechat/")))
         self.assertIsNot(historical_review_requests, None)
 
 
     def test_next_reviewers_in_teams(self) -> None:
         next_reviewers_in_teams = self.dt.next_reviewers_in_teams()
         self.assertIsNot(next_reviewers_in_teams, None)
 
 
     def test_next_reviewers_in_teams_team(self) -> None:
-        next_reviewers_in_teams = list(self.dt.next_reviewers_in_teams(team=self.dt.group(GroupURI("/api/v1/group/group/1972/"))))
+        next_reviewers_in_teams = list(self.dt.next_reviewers_in_teams(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1972/"))))
         self.assertEqual(len(next_reviewers_in_teams),  1)
         self.assertEqual(next_reviewers_in_teams[0].id, 1)
 
     def test_review_team_settings(self) -> None:
-        review_team_settings = self.dt.review_team_settings(ReviewTeamSettingsURI("/api/v1/review/reviewteamsettings/1/"))
+        review_team_settings = self.dt.review_team_settings(ReviewTeamSettingsURI(uri="/api/v1/review/reviewteamsettings/1/"))
         if review_team_settings is not None:
             self.assertEqual(review_team_settings.autosuggest,                      True)
-            self.assertEqual(review_team_settings.group,                            GroupURI("/api/v1/group/group/1261/"))
+            self.assertEqual(review_team_settings.group,                            GroupURI(uri="/api/v1/group/group/1261/"))
             self.assertEqual(review_team_settings.id,                               1)
             self.assertEqual(len(review_team_settings.notify_ad_when),              3)
-            self.assertEqual(review_team_settings.notify_ad_when[0],                ReviewResultTypeURI("/api/v1/name/reviewresultname/serious-issues/"))
-            self.assertEqual(review_team_settings.notify_ad_when[1],                ReviewResultTypeURI("/api/v1/name/reviewresultname/issues/"))
-            self.assertEqual(review_team_settings.notify_ad_when[2],                ReviewResultTypeURI("/api/v1/name/reviewresultname/not-ready/"))
+            self.assertEqual(review_team_settings.notify_ad_when[0],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/serious-issues/"))
+            self.assertEqual(review_team_settings.notify_ad_when[1],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/issues/"))
+            self.assertEqual(review_team_settings.notify_ad_when[2],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/not-ready/"))
             self.assertIs(review_team_settings.remind_days_unconfirmed_assignments, None)
-            self.assertEqual(review_team_settings.resource_uri,                     ReviewTeamSettingsURI("/api/v1/review/reviewteamsettings/1/"))
+            self.assertEqual(review_team_settings.resource_uri,                     ReviewTeamSettingsURI(uri="/api/v1/review/reviewteamsettings/1/"))
             self.assertEqual(len(review_team_settings.review_results),              5)
-            self.assertEqual(review_team_settings.review_results[0],                ReviewResultTypeURI("/api/v1/name/reviewresultname/serious-issues/"))
-            self.assertEqual(review_team_settings.review_results[1],                ReviewResultTypeURI("/api/v1/name/reviewresultname/issues/"))
-            self.assertEqual(review_team_settings.review_results[2],                ReviewResultTypeURI("/api/v1/name/reviewresultname/nits/"))
-            self.assertEqual(review_team_settings.review_results[3],                ReviewResultTypeURI("/api/v1/name/reviewresultname/not-ready/"))
-            self.assertEqual(review_team_settings.review_results[4],                ReviewResultTypeURI("/api/v1/name/reviewresultname/ready/"))
+            self.assertEqual(review_team_settings.review_results[0],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/serious-issues/"))
+            self.assertEqual(review_team_settings.review_results[1],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/issues/"))
+            self.assertEqual(review_team_settings.review_results[2],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/nits/"))
+            self.assertEqual(review_team_settings.review_results[3],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/not-ready/"))
+            self.assertEqual(review_team_settings.review_results[4],                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/ready/"))
             self.assertEqual(len(review_team_settings.review_types),                3)
-            self.assertEqual(review_team_settings.review_types[0],                  ReviewTypeURI("/api/v1/name/reviewtypename/early/"))
-            self.assertEqual(review_team_settings.review_types[1],                  ReviewTypeURI("/api/v1/name/reviewtypename/lc/"))
-            self.assertEqual(review_team_settings.review_types[2],                  ReviewTypeURI("/api/v1/name/reviewtypename/telechat/"))
+            self.assertEqual(review_team_settings.review_types[0],                  ReviewTypeURI(uri="/api/v1/name/reviewtypename/early/"))
+            self.assertEqual(review_team_settings.review_types[1],                  ReviewTypeURI(uri="/api/v1/name/reviewtypename/lc/"))
+            self.assertEqual(review_team_settings.review_types[2],                  ReviewTypeURI(uri="/api/v1/name/reviewtypename/telechat/"))
             self.assertEqual(review_team_settings.secr_mail_alias,                  "")
         else:
             self.fail("Cannot find review team settings")
 
 
     def test_review_team_settings_all(self) -> None:
         review_team_settings_all = self.dt.review_team_settings_all()
         self.assertIsNot(review_team_settings_all, None)
 
 
     def test_review_team_settings_all_group(self) -> None:
-        review_team_settings_all = list(self.dt.review_team_settings_all(group=self.dt.group(GroupURI("/api/v1/group/group/1261/"))))
+        review_team_settings_all = list(self.dt.review_team_settings_all(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1261/"))))
         self.assertEqual(len(review_team_settings_all),  1)
         self.assertEqual(review_team_settings_all[0].id, 1)
 
 
     def test_unavailable_period(self) -> None:
-        unavailable_period = self.dt.unavailable_period(UnavailablePeriodURI("/api/v1/review/unavailableperiod/1/"))
+        unavailable_period = self.dt.unavailable_period(UnavailablePeriodURI(uri="/api/v1/review/unavailableperiod/1/"))
         if unavailable_period is not None:
             self.assertEqual(unavailable_period.availability, "unavailable")
             self.assertEqual(unavailable_period.end_date,     "2016-12-01")
             self.assertEqual(unavailable_period.id,           1)
-            self.assertEqual(unavailable_period.person,       PersonURI("/api/v1/person/person/101208/"))
+            self.assertEqual(unavailable_period.person,       PersonURI(uri="/api/v1/person/person/101208/"))
             self.assertEqual(unavailable_period.reason,       "")
-            self.assertEqual(unavailable_period.resource_uri, UnavailablePeriodURI("/api/v1/review/unavailableperiod/1/"))
+            self.assertEqual(unavailable_period.resource_uri, UnavailablePeriodURI(uri="/api/v1/review/unavailableperiod/1/"))
             self.assertEqual(unavailable_period.start_date,   None)
-            self.assertEqual(unavailable_period.team,         GroupURI("/api/v1/group/group/1261/"))
+            self.assertEqual(unavailable_period.team,         GroupURI(uri="/api/v1/group/group/1261/"))
         else:
             self.fail("Cannot find unavailable period")
 
 
     def test_unavailable_periods(self) -> None:
         unavailable_periods = self.dt.unavailable_periods()
         self.assertIsNot(unavailable_periods, None)
 
 
     def test_unavailable_periods_person(self) -> None:
-        unavailable_periods = self.dt.unavailable_periods(person=self.dt.person(PersonURI("/api/v1/person/person/101208/")))
+        unavailable_periods = self.dt.unavailable_periods(person=self.dt.person(PersonURI(uri="/api/v1/person/person/101208/")))
         self.assertIsNot(unavailable_periods, None)
 
 
     def test_unavailable_periods_team(self) -> None:
-        unavailable_periods = self.dt.unavailable_periods(team=self.dt.group(GroupURI("/api/v1/group/group/1261/")))
+        unavailable_periods = self.dt.unavailable_periods(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1261/")))
         self.assertIsNot(unavailable_periods, None)
 
 
     def test_historical_reviewer_settings(self) -> None:
-        historical_reviewer_settings = self.dt.historical_reviewer_settings(HistoricalReviewerSettingsURI("/api/v1/review/historicalreviewersettings/733/"))
+        historical_reviewer_settings = self.dt.historical_reviewer_settings(HistoricalReviewerSettingsURI(uri="/api/v1/review/historicalreviewersettings/733/"))
         if historical_reviewer_settings is not None:
             self.assertEqual(historical_reviewer_settings.expertise,                   "")
             self.assertEqual(historical_reviewer_settings.filter_re,                   "^draft-(weber).*$")
             self.assertEqual(historical_reviewer_settings.history_change_reason,       None)
             self.assertEqual(historical_reviewer_settings.history_date,                datetime.fromisoformat("2020-05-27T08:15:54-07:00"))
             self.assertEqual(historical_reviewer_settings.history_id,                  733)
             self.assertEqual(historical_reviewer_settings.history_type,                "~")
             self.assertEqual(historical_reviewer_settings.history_user,                "")
             self.assertEqual(historical_reviewer_settings.id,                          97)
             self.assertEqual(historical_reviewer_settings.min_interval,                None)
-            self.assertEqual(historical_reviewer_settings.person,                      PersonURI("/api/v1/person/person/110404/"))
+            self.assertEqual(historical_reviewer_settings.person,                      PersonURI(uri="/api/v1/person/person/110404/"))
             self.assertEqual(historical_reviewer_settings.remind_days_before_deadline, None)
             self.assertEqual(historical_reviewer_settings.remind_days_open_reviews,    None)
             self.assertEqual(historical_reviewer_settings.request_assignment_next,     False)
-            self.assertEqual(historical_reviewer_settings.resource_uri,                HistoricalReviewerSettingsURI("/api/v1/review/historicalreviewersettings/733/"))
+            self.assertEqual(historical_reviewer_settings.resource_uri,                HistoricalReviewerSettingsURI(uri="/api/v1/review/historicalreviewersettings/733/"))
             self.assertEqual(historical_reviewer_settings.skip_next,                   0)
-            self.assertEqual(historical_reviewer_settings.team,                        GroupURI("/api/v1/group/group/1974/"))
+            self.assertEqual(historical_reviewer_settings.team,                        GroupURI(uri="/api/v1/group/group/1974/"))
         else:
             self.fail("Cannot find historical reviewer settings")
 
 
     def test_historical_reviewer_settings_all(self) -> None:
         historical_reviewer_settings = self.dt.historical_reviewer_settings_all()
         self.assertIsNot(historical_reviewer_settings, None)
@@ -3323,41 +3392,41 @@
 
     def test_historical_reviewer_settings_all_id(self) -> None:
         historical_reviewer_settings = self.dt.historical_reviewer_settings_all(id=97)
         self.assertIsNot(historical_reviewer_settings, None)
 
 
     def test_historical_reviewer_settings_all_person(self) -> None:
-        historical_reviewer_settings = self.dt.historical_reviewer_settings_all(person=self.dt.person(PersonURI("/api/v1/person/person/110404/")))
+        historical_reviewer_settings = self.dt.historical_reviewer_settings_all(person=self.dt.person(PersonURI(uri="/api/v1/person/person/110404/")))
         self.assertIsNot(historical_reviewer_settings, None)
 
 
     def test_historical_reviewer_settings_all_team(self) -> None:
-        historical_reviewer_settings = self.dt.historical_reviewer_settings_all(team=self.dt.group(GroupURI("/api/v1/group/group/1974/")))
+        historical_reviewer_settings = self.dt.historical_reviewer_settings_all(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1974/")))
         self.assertIsNot(historical_reviewer_settings, None)
 
 
     def test_historical_review_assignment(self) -> None:
-        historical_review_assignment = self.dt.historical_review_assignment(HistoricalReviewAssignmentURI("/api/v1/review/historicalreviewassignment/1130/"))
+        historical_review_assignment = self.dt.historical_review_assignment(HistoricalReviewAssignmentURI(uri="/api/v1/review/historicalreviewassignment/1130/"))
         if historical_review_assignment is not None:
             self.assertEqual(historical_review_assignment.assigned_on,           datetime.fromisoformat("2020-05-19T08:35:44-07:00"))
             self.assertEqual(historical_review_assignment.completed_on,          datetime.fromisoformat("2020-05-27T08:17:03-07:00"))
             self.assertEqual(historical_review_assignment.history_change_reason, "Request for Last Call review by OPSDIR Completed: Not Ready. Reviewer: Scott Bradner.")
             self.assertEqual(historical_review_assignment.history_date,          datetime.fromisoformat("2020-05-27T08:17:03-07:00"))
             self.assertEqual(historical_review_assignment.history_id,            1130)
             self.assertEqual(historical_review_assignment.history_type,          "~")
             self.assertEqual(historical_review_assignment.id,                    11544)
             self.assertEqual(historical_review_assignment.mailarch_url,          None)
-            self.assertEqual(historical_review_assignment.resource_uri,          HistoricalReviewAssignmentURI("/api/v1/review/historicalreviewassignment/1130/"))
-            self.assertEqual(historical_review_assignment.result,                ReviewResultTypeURI("/api/v1/name/reviewresultname/not-ready/"))
-            self.assertEqual(historical_review_assignment.review,                DocumentURI("/api/v1/doc/document/review-ietf-ospf-te-link-attr-reuse-12-opsdir-lc-bradner-2020-05-27/"))
-            self.assertEqual(historical_review_assignment.review_request,        ReviewRequestURI("/api/v1/review/reviewrequest/13398/"))
+            self.assertEqual(historical_review_assignment.resource_uri,          HistoricalReviewAssignmentURI(uri="/api/v1/review/historicalreviewassignment/1130/"))
+            self.assertEqual(historical_review_assignment.result,                ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/not-ready/"))
+            self.assertEqual(historical_review_assignment.review,                DocumentURI(uri="/api/v1/doc/document/review-ietf-ospf-te-link-attr-reuse-12-opsdir-lc-bradner-2020-05-27/"))
+            self.assertEqual(historical_review_assignment.review_request,        ReviewRequestURI(uri="/api/v1/review/reviewrequest/13398/"))
             self.assertEqual(historical_review_assignment.reviewed_rev,          "12")
-            self.assertEqual(historical_review_assignment.reviewer,              EmailURI("/api/v1/person/email/sob@sobco.com/"))
-            self.assertEqual(historical_review_assignment.state,                 ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/completed/"))
+            self.assertEqual(historical_review_assignment.reviewer,              EmailURI(uri="/api/v1/person/email/sob@sobco.com/"))
+            self.assertEqual(historical_review_assignment.state,                 ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/completed/"))
         else:
             self.fail("Cannot find historical review assignment")
 
 
     def test_historical_review_assignments(self) -> None:
         historical_review_assignments = self.dt.historical_review_assignments()
         self.assertIsNot(historical_review_assignments, None)
@@ -3365,157 +3434,157 @@
 
     def test_historical_review_assignments_id(self) -> None:
         historical_review_assignments = self.dt.historical_review_assignments(id=11544)
         self.assertIsNot(historical_review_assignments, None)
 
 
     def test_historical_review_assignments_result(self) -> None:
-        historical_review_assignments = self.dt.historical_review_assignments(result=self.dt.review_result_type(ReviewResultTypeURI("/api/v1/name/reviewresultname/nits/")))
+        historical_review_assignments = self.dt.historical_review_assignments(result=self.dt.review_result_type(ReviewResultTypeURI(uri="/api/v1/name/reviewresultname/nits/")))
         self.assertIsNot(historical_review_assignments, None)
 
 
     def test_historical_review_assignments_review_request(self) -> None:
-        historical_review_assignments = list(self.dt.historical_review_assignments(review_request=self.dt.review_request(ReviewRequestURI("/api/v1/review/reviewrequest/13398/"))))
+        historical_review_assignments = list(self.dt.historical_review_assignments(review_request=self.dt.review_request(ReviewRequestURI(uri="/api/v1/review/reviewrequest/13398/"))))
         self.assertIsNot(historical_review_assignments, None)
 
 
     def test_historical_review_assignments_reviewer(self) -> None:
-        historical_review_assignments = self.dt.historical_review_assignments(reviewer=self.dt.email(EmailURI("/api/v1/person/email/csp@csperkins.org/")))
+        historical_review_assignments = self.dt.historical_review_assignments(reviewer=self.dt.email(EmailURI(uri="/api/v1/person/email/csp@csperkins.org/")))
         self.assertIsNot(historical_review_assignments, None)
 
 
     def test_historical_review_assignments_state(self) -> None:
-        historical_review_assignments = self.dt.historical_review_assignments(state=self.dt.review_assignment_state(ReviewAssignmentStateURI("/api/v1/name/reviewassignmentstatename/completed/")))
+        historical_review_assignments = self.dt.historical_review_assignments(state=self.dt.review_assignment_state(ReviewAssignmentStateURI(uri="/api/v1/name/reviewassignmentstatename/completed/")))
         self.assertIsNot(historical_review_assignments, None)
 
 
     def test_review_secretary_settings(self) -> None:
-        review_secretary_settings = self.dt.review_secretary_settings(ReviewSecretarySettingsURI("/api/v1/review/reviewsecretarysettings/1/"))
+        review_secretary_settings = self.dt.review_secretary_settings(ReviewSecretarySettingsURI(uri="/api/v1/review/reviewsecretarysettings/1/"))
         if review_secretary_settings is not None:
             self.assertEqual(review_secretary_settings.days_to_show_in_reviewer_list,      None)
             self.assertEqual(review_secretary_settings.id,                                 1)
             self.assertEqual(review_secretary_settings.max_items_to_show_in_reviewer_list, None)
-            self.assertEqual(review_secretary_settings.person,                             PersonURI("/api/v1/person/person/105519/"))
+            self.assertEqual(review_secretary_settings.person,                             PersonURI(uri="/api/v1/person/person/105519/"))
             self.assertEqual(review_secretary_settings.remind_days_before_deadline,        2)
-            self.assertEqual(review_secretary_settings.resource_uri,                       ReviewSecretarySettingsURI("/api/v1/review/reviewsecretarysettings/1/"))
-            self.assertEqual(review_secretary_settings.team,                               GroupURI("/api/v1/group/group/2174/"))
+            self.assertEqual(review_secretary_settings.resource_uri,                       ReviewSecretarySettingsURI(uri="/api/v1/review/reviewsecretarysettings/1/"))
+            self.assertEqual(review_secretary_settings.team,                               GroupURI(uri="/api/v1/group/group/2174/"))
         else:
             self.fail("Cannot find review secretary settings")
 
 
     def test_review_secretary_settings_all(self) -> None:
         review_secretary_settings = self.dt.review_secretary_settings_all()
         self.assertIsNot(review_secretary_settings, None)
 
 
     def test_review_secretary_settings_all_person(self) -> None:
-        review_secretary_settings = self.dt.review_secretary_settings_all(person=self.dt.person(PersonURI("/api/v1/person/person/115026/")))
+        review_secretary_settings = self.dt.review_secretary_settings_all(person=self.dt.person(PersonURI(uri="/api/v1/person/person/115026/")))
         self.assertIsNot(review_secretary_settings, None)
 
 
     def test_review_secretary_settings_all_team(self) -> None:
-        review_secretary_settings = self.dt.review_secretary_settings_all(team=self.dt.group(GroupURI("/api/v1/group/group/1982/")))
+        review_secretary_settings = self.dt.review_secretary_settings_all(team=self.dt.group(GroupURI(uri="/api/v1/group/group/1982/")))
         self.assertIsNot(review_secretary_settings, None)
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to mailing lists:
 
 
-    def test_email_list(self) -> None:
-        ml = self.dt.email_list(EmailListURI("/api/v1/mailinglists/list/461/"))
-        if ml is not None:
-            self.assertEqual(ml.id,           461)
-            self.assertEqual(ml.resource_uri, EmailListURI("/api/v1/mailinglists/list/461/"))
-            self.assertEqual(ml.name,         "hackathon")
-            self.assertEqual(ml.description,  "Discussion regarding past, present, and future IETF hackathons.")
-            self.assertEqual(ml.advertised,   True)
-        else:
-            self.fail("Cannot find email list")
-
-
-    def test_email_lists(self) -> None:
-        ml = list(self.dt.email_lists(name="ietf"))
-        if ml is not None:
-            self.assertEqual(len(ml), 1)
-            self.assertEqual(ml[0].id,            262)
-            self.assertEqual(ml[0].description,  "IETF-Discussion. This is the most general IETF mailing list, intended for discussion of technical, procedural, operational, and other topics for which no dedicated mailing lists exist.")
-            self.assertEqual(ml[0].resource_uri, EmailListURI("/api/v1/mailinglists/list/262/"))
-            self.assertEqual(ml[0].advertised,   True)
-            self.assertEqual(ml[0].name,         "ietf")
-        else:
-            self.fail("Cannot find email list")
-
-
-    def test_email_list_subscriptions(self) -> None:
-        subs = list(self.dt.email_list_subscriptions(email_addr="colin.perkins@glasgow.ac.uk"))
-        self.assertEqual(len(subs), 1)
-        self.assertEqual(subs[0].id,           66700)
-        self.assertEqual(subs[0].resource_uri, EmailListSubscriptionsURI(uri="/api/v1/mailinglists/subscribed/66700/"))
-        self.assertEqual(subs[0].email,        "colin.perkins@glasgow.ac.uk")
-        self.assertEqual(subs[0].lists[0],     EmailListURI("/api/v1/mailinglists/list/461/"))
-
-    def test_email_list_subscriptions_by_list(self) -> None:
-        subs = list(self.dt.email_list_subscriptions(email_list=self.dt.email_list(EmailListURI("/api/v1/mailinglists/list/1/"))))
-        self.assertIsNot(subs, None)
+    #def test_email_list(self) -> None:
+    #    ml = self.dt.email_list(EmailListURI(uri="/api/v1/mailinglists/list/461/"))
+    #    if ml is not None:
+    #        self.assertEqual(ml.id,           461)
+    #        self.assertEqual(ml.resource_uri, EmailListURI(uri="/api/v1/mailinglists/list/461/"))
+    #        self.assertEqual(ml.name,         "hackathon")
+    #        self.assertEqual(ml.description,  "Discussion regarding past, present, and future IETF hackathons.")
+    #        self.assertEqual(ml.advertised,   True)
+    #    else:
+    #        self.fail("Cannot find email list")
+
+
+    #def test_email_lists(self) -> None:
+    #    ml = list(self.dt.email_lists(name="ietf"))
+    #    if ml is not None:
+    #        self.assertEqual(len(ml), 1)
+    #        self.assertEqual(ml[0].id,            262)
+    #        self.assertEqual(ml[0].description,  "IETF-Discussion. This is the most general IETF mailing list, intended for discussion of technical, procedural, operational, and other topics for which no dedicated mailing lists exist.")
+    #        self.assertEqual(ml[0].resource_uri, EmailListURI(uri="/api/v1/mailinglists/list/262/"))
+    #        self.assertEqual(ml[0].advertised,   True)
+    #        self.assertEqual(ml[0].name,         "ietf")
+    #    else:
+    #        self.fail("Cannot find email list")
+
+
+    #def test_email_list_subscriptions(self) -> None:
+    #    subs = list(self.dt.email_list_subscriptions(email_addr="colin.perkins@glasgow.ac.uk"))
+    #    self.assertEqual(len(subs), 1)
+    #    self.assertEqual(subs[0].id,           66700)
+    #    self.assertEqual(subs[0].resource_uri, EmailListSubscriptionsURI(uri="/api/v1/mailinglists/subscribed/66700/"))
+    #    self.assertEqual(subs[0].email,        "colin.perkins@glasgow.ac.uk")
+    #    self.assertEqual(subs[0].lists[0],     EmailListURI(uri="/api/v1/mailinglists/list/461/"))
+
+    #def test_email_list_subscriptions_by_list(self) -> None:
+    #    subs = list(self.dt.email_list_subscriptions(email_list=self.dt.email_list(EmailListURI(uri="/api/v1/mailinglists/list/1/"))))
+    #    self.assertIsNot(subs, None)
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to countries and continents:
 
     def test_continent(self) -> None:
-        continent = self.dt.continent(ContinentURI("/api/v1/name/continentname/europe/"))
+        continent = self.dt.continent(ContinentURI(uri="/api/v1/name/continentname/europe/"))
         if continent is not None:
             self.assertEqual(continent.used, True)
             self.assertEqual(continent.order, 0)
             self.assertEqual(continent.desc, "")
             self.assertEqual(continent.name, "Europe")
-            self.assertEqual(continent.resource_uri, ContinentURI("/api/v1/name/continentname/europe/"))
+            self.assertEqual(continent.resource_uri, ContinentURI(uri="/api/v1/name/continentname/europe/"))
             self.assertEqual(continent.slug, "europe")
         else:
             self.fail("Cannot find continent")
 
 
     def test_continent_from_slug(self) -> None:
         continent = self.dt.continent_from_slug("europe")
         if continent is not None:
             self.assertEqual(continent.used, True)
             self.assertEqual(continent.order, 0)
             self.assertEqual(continent.desc, "")
             self.assertEqual(continent.name, "Europe")
-            self.assertEqual(continent.resource_uri, ContinentURI("/api/v1/name/continentname/europe/"))
+            self.assertEqual(continent.resource_uri, ContinentURI(uri="/api/v1/name/continentname/europe/"))
             self.assertEqual(continent.slug, "europe")
         else:
             self.fail("Cannot find continent")
 
 
     def test_continents(self) -> None:
         continents = list(self.dt.continents())
         self.assertEqual(len(continents), 7)
 
 
     def test_country(self) -> None:
-        country = self.dt.country(CountryURI("/api/v1/name/countryname/DE/"))
+        country = self.dt.country(CountryURI(uri="/api/v1/name/countryname/DE/"))
         if country is not None:
             self.assertEqual(country.order,        0)
-            self.assertEqual(country.continent,    ContinentURI("/api/v1/name/continentname/europe/"))
-            self.assertEqual(country.resource_uri, CountryURI("/api/v1/name/countryname/DE/"))
+            self.assertEqual(country.continent,    ContinentURI(uri="/api/v1/name/continentname/europe/"))
+            self.assertEqual(country.resource_uri, CountryURI(uri="/api/v1/name/countryname/DE/"))
             self.assertEqual(country.used,         True)
             self.assertEqual(country.desc,         "")
             self.assertEqual(country.name,         "Germany")
             self.assertEqual(country.in_eu,        True)
             self.assertEqual(country.slug,         "DE")
         else:
             self.fail("Cannot find country")
 
 
     def test_country_from_slug(self) -> None:
         country = self.dt.country_from_slug("DE")
         if country is not None:
             self.assertEqual(country.order,        0)
-            self.assertEqual(country.continent,    ContinentURI("/api/v1/name/continentname/europe/"))
-            self.assertEqual(country.resource_uri, CountryURI("/api/v1/name/countryname/DE/"))
+            self.assertEqual(country.continent,    ContinentURI(uri="/api/v1/name/continentname/europe/"))
+            self.assertEqual(country.resource_uri, CountryURI(uri="/api/v1/name/countryname/DE/"))
             self.assertEqual(country.used,         True)
             self.assertEqual(country.desc,         "")
             self.assertEqual(country.name,         "Germany")
             self.assertEqual(country.in_eu,        True)
             self.assertEqual(country.slug,         "DE")
         else:
             self.fail("Cannot find country")
@@ -3538,50 +3607,50 @@
 
     def test_countries_name(self) -> None:
         countries = list(self.dt.countries(name = "Germany"))
         self.assertEqual(len(countries), 1)
 
 
     def test_country_alias(self) -> None:
-        country = self.dt.country_alias(CountryAliasURI("/api/v1/stats/countryalias/292/"))
+        country = self.dt.country_alias(CountryAliasURI(uri="/api/v1/stats/countryalias/292/"))
         if country is not None:
-            self.assertEqual(country.country,      CountryURI("/api/v1/name/countryname/BE/"))
-            self.assertEqual(country.resource_uri, CountryAliasURI("/api/v1/stats/countryalias/292/"))
+            self.assertEqual(country.country,      CountryURI(uri="/api/v1/name/countryname/BE/"))
+            self.assertEqual(country.resource_uri, CountryAliasURI(uri="/api/v1/stats/countryalias/292/"))
             self.assertEqual(country.alias,        "belgique")
             self.assertEqual(country.id,           292)
         else:
             self.fail("Cannot find country alias")
 
 
     def test_country_aliases(self) -> None:
         aliases = list(self.dt.country_aliases("belgique"))
         self.assertEqual(len(aliases), 1)
-        self.assertEqual(aliases[0].resource_uri, CountryAliasURI("/api/v1/stats/countryalias/292/"))
-        self.assertEqual(aliases[0].country,      CountryURI("/api/v1/name/countryname/BE/"))
+        self.assertEqual(aliases[0].resource_uri, CountryAliasURI(uri="/api/v1/stats/countryalias/292/"))
+        self.assertEqual(aliases[0].country,      CountryURI(uri="/api/v1/name/countryname/BE/"))
         self.assertEqual(aliases[0].alias,        "belgique")
         self.assertEqual(aliases[0].id,           292)
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to statistics:
 
     def test_meeting_registration(self) -> None:
-        reg = self.dt.meeting_registration(MeetingRegistrationURI("/api/v1/stats/meetingregistration/42206/"))
+        reg = self.dt.meeting_registration(MeetingRegistrationURI(uri="/api/v1/stats/meetingregistration/42206/"))
         if reg is not None:
             self.assertEqual(reg.affiliation,  "University of Glasgow")
             self.assertEqual(reg.attended,     True)
             self.assertEqual(reg.country_code, "GB")
             self.assertEqual(reg.email,        "sm@smcquistin.uk")
             self.assertEqual(reg.first_name,   "Stephen")
             self.assertEqual(reg.id,           42206)
             self.assertEqual(reg.last_name,    "McQuistin")
-            self.assertEqual(reg.meeting,      MeetingURI("/api/v1/meeting/meeting/1003/"))
+            self.assertEqual(reg.meeting,      MeetingURI(uri="/api/v1/meeting/meeting/1003/"))
             self.assertEqual(reg.person,       PersonURI(uri="/api/v1/person/person/117769/"))
             self.assertEqual(reg.reg_type,     "remote")
-            self.assertEqual(reg.resource_uri, MeetingRegistrationURI("/api/v1/stats/meetingregistration/42206/"))
+            self.assertEqual(reg.resource_uri, MeetingRegistrationURI(uri="/api/v1/stats/meetingregistration/42206/"))
             self.assertEqual(reg.ticket_type,  "full_week_pass")
         else:
             self.fail("Cannot find meeting registration")
 
 
     def test_meeting_registrations(self) -> None:
         regs = self.dt.meeting_registrations()
@@ -3615,20 +3684,20 @@
 
     def test_meeting_registrations_last_name(self) -> None:
         regs = self.dt.meeting_registrations(last_name="McQuistin")
         self.assertIsNot(regs, None)
 
 
     def test_meeting_registrations_meeting(self) -> None:
-        regs = self.dt.meeting_registrations(meeting=self.dt.meeting(MeetingURI("/api/v1/meeting/meeting/1003/")))
+        regs = self.dt.meeting_registrations(meeting=self.dt.meeting(MeetingURI(uri="/api/v1/meeting/meeting/1003/")))
         self.assertIsNot(regs, None)
 
 
     def test_meeting_registrations_person(self) -> None:
-        regs = self.dt.meeting_registrations(person=self.dt.person(PersonURI("/api/v1/person/person/117769/")))
+        regs = self.dt.meeting_registrations(person=self.dt.person(PersonURI(uri="/api/v1/person/person/117769/")))
         self.assertIsNot(regs, None)
 
 
     def test_meeting_registrations_reg_type(self) -> None:
         regs = self.dt.meeting_registrations(reg_type="remote")
         self.assertIsNot(regs, None)
 
@@ -3638,21 +3707,21 @@
         self.assertIsNot(regs, None)
 
 
     # -----------------------------------------------------------------------------------------------------------------------------
     # Tests relating to messages:
 
     def test_announcement_from(self) -> None:
-        announcement_from = self.dt.announcement_from(AnnouncementFromURI("/api/v1/message/announcementfrom/1/"))
+        announcement_from = self.dt.announcement_from(AnnouncementFromURI(uri="/api/v1/message/announcementfrom/1/"))
         if announcement_from is not None:
             self.assertEqual(announcement_from.address,      "IETF Chair <chair@ietf.org>")
-            self.assertEqual(announcement_from.group,        GroupURI("/api/v1/group/group/1/"))
+            self.assertEqual(announcement_from.group,        GroupURI(uri="/api/v1/group/group/1/"))
             self.assertEqual(announcement_from.id,           1)
-            self.assertEqual(announcement_from.name,         RoleNameURI("/api/v1/name/rolename/chair/"))
-            self.assertEqual(announcement_from.resource_uri, AnnouncementFromURI("/api/v1/message/announcementfrom/1/"))
+            self.assertEqual(announcement_from.name,         RoleNameURI(uri="/api/v1/name/rolename/chair/"))
+            self.assertEqual(announcement_from.resource_uri, AnnouncementFromURI(uri="/api/v1/message/announcementfrom/1/"))
         else:
             self.fail("Cannot find announcement from metadata")
 
 
     def test_announcements_from(self) -> None:
         announcements_from = self.dt.announcements_from()
         self.assertIsNot(announcements_from, None)
@@ -3661,83 +3730,83 @@
     def test_announcements_from_address(self) -> None:
         announcements_from = list(self.dt.announcements_from(address="IETF Chair <chair@ietf.org>"))
         self.assertEqual(len(announcements_from),  1)
         self.assertEqual(announcements_from[0].id, 1)
 
 
     def test_announcements_from_group(self) -> None:
-        announcements_from = list(self.dt.announcements_from(group=self.dt.group(GroupURI("/api/v1/group/group/1/"))))
+        announcements_from = list(self.dt.announcements_from(group=self.dt.group(GroupURI(uri="/api/v1/group/group/1/"))))
         self.assertEqual(len(announcements_from),  6)
         self.assertEqual(announcements_from[0].id, 1)
         self.assertEqual(announcements_from[1].id, 2)
         self.assertEqual(announcements_from[2].id, 7)
         self.assertEqual(announcements_from[3].id, 8)
         self.assertEqual(announcements_from[4].id, 27)
         self.assertEqual(announcements_from[5].id, 28)
 
 
     def test_announcements_from_name(self) -> None:
-        announcements_from = list(self.dt.announcements_from(name=self.dt.role_name(RoleNameURI("/api/v1/name/rolename/chair/"))))
+        announcements_from = list(self.dt.announcements_from(name=self.dt.role_name(RoleNameURI(uri="/api/v1/name/rolename/chair/"))))
         self.assertEqual(len(announcements_from),  10)
         self.assertEqual(announcements_from[0].id, 1)
         self.assertEqual(announcements_from[1].id, 2)
         self.assertEqual(announcements_from[2].id, 3)
         self.assertEqual(announcements_from[3].id, 10)
         self.assertEqual(announcements_from[4].id, 12)
         self.assertEqual(announcements_from[5].id, 13)
         self.assertEqual(announcements_from[6].id, 15)
         self.assertEqual(announcements_from[7].id, 16)
         self.assertEqual(announcements_from[8].id, 24)
         self.assertEqual(announcements_from[9].id, 26)
 
 
     #def test_message(self) -> None:
-    #    message = self.dt.message(DTMessageURI("/api/v1/message/message/158636/"))
+    #    message = self.dt.message(DTMessageURI(uri="/api/v1/message/message/158636/"))
     #    if message is not None:
     #        self.assertEqual(message.bcc,            "")
     #        self.assertEqual(message.body,           "\nA New Internet-Draft is available from the on-line Internet-Drafts directories.\n\n\n        Title           : Describing Protocol Data Units with Augmented Packet Header Diagrams\n        Authors         : Stephen McQuistin\n                          Vivian Band\n                          Dejice Jacob\n                          Colin Perkins\n\tFilename        : draft-mcquistin-augmented-ascii-diagrams-05.txt\n\tPages           : 26\n\tDate            : 2020-06-17\n\nAbstract:\n   This document describes a machine-readable format for specifying the\n   syntax of protocol data units within a protocol specification.  This\n   format is comprised of a consistently formatted packet header\n   diagram, followed by structured explanatory text.  It is designed to\n   maintain human readability while enabling support for automated\n   parser generation from the specification document.  This document is\n   itself an example of how the format can be used.\n\n\nThe IETF datatracker status page for this draft is:\nhttps://datatracker.ietf.org/doc/draft-mcquistin-augmented-ascii-diagrams/\n\nThere are also htmlized versions available at:\nhttps://tools.ietf.org/html/draft-mcquistin-augmented-ascii-diagrams-05\nhttps://datatracker.ietf.org/doc/html/draft-mcquistin-augmented-ascii-diagrams-05\n\nA diff from the previous version is available at:\nhttps://www.ietf.org/rfcdiff?url2=draft-mcquistin-augmented-ascii-diagrams-05\n\n\nPlease note that it may take a couple of minutes from the time of submission\nuntil the htmlized version and diff are available at tools.ietf.org.\n\nInternet-Drafts are also available by anonymous FTP at:\nftp://ftp.ietf.org/internet-drafts/\n\n")
-    #        self.assertEqual(message.by,             PersonURI("/api/v1/person/person/1/"))
+    #        self.assertEqual(message.by,             PersonURI(uri="/api/v1/person/person/1/"))
     #        self.assertEqual(message.cc,             "")
     #        self.assertEqual(message.content_type,   "text/plain")
     #        self.assertEqual(message.frm,            "internet-drafts@ietf.org")
     #        self.assertEqual(message.id,             158636)
     #        self.assertEqual(message.msgid,          "<159239631351.30959.7146324646157253269@ietfa.amsl.com>")
-    #        self.assertEqual(message.related_docs,   [DocumentURI("/api/v1/doc/document/draft-mcquistin-augmented-ascii-diagrams/")])
+    #        self.assertEqual(message.related_docs,   [DocumentURI(uri="/api/v1/doc/document/draft-mcquistin-augmented-ascii-diagrams/")])
     #        self.assertEqual(message.related_groups, [])
     #        self.assertEqual(message.reply_to, "")
-    #        self.assertEqual(message.resource_uri,   DTMessageURI("/api/v1/message/message/158636/"))
+    #        self.assertEqual(message.resource_uri,   DTMessageURI(uri="/api/v1/message/message/158636/"))
     #        self.assertEqual(message.sent,           datetime.fromisoformat("2020-06-17T05:18:33.607859"))
     #        self.assertEqual(message.subject,        "I-D Action: draft-mcquistin-augmented-ascii-diagrams-05.txt")
     #        self.assertEqual(message.time,           datetime.fromisoformat("2020-06-17T05:18:33"))
     #        self.assertEqual(message.to,             "i-d-announce@ietf.org")
     #    else:
     #        self.fail("Cannot find message")
 
 
     #def test_messages(self) -> None:
     #    messages = self.dt.messages()
     #    self.assertIsNot(messages, None)
 
 
     #def test_messages_by(self) -> None:
-    #    person = self.dt.person(PersonURI("/api/v1/person/person/1/"))
+    #    person = self.dt.person(PersonURI(uri="/api/v1/person/person/1/"))
     #    if person is not None:
     #        messages = list(self.dt.messages(by=person))
     #        self.assertNotEqual(len(messages), 0)
     #    else:
     #        self.fail("Cannot find person")
 
 
     #def test_messages_frm(self) -> None:
     #    messages = list(self.dt.messages(frm="internet-drafts@ietf.org"))
     #    self.assertNotEqual(len(messages), 0)
 
 
     #def test_messages_related_doc(self) -> None:
-    #    doc = self.dt.document(DocumentURI("/api/v1/doc/document/draft-mcquistin-augmented-ascii-diagrams/"))
+    #    doc = self.dt.document(DocumentURI(uri="/api/v1/doc/document/draft-mcquistin-augmented-ascii-diagrams/"))
     #    if doc is not None:
     #        messages = list(self.dt.messages(related_doc=doc))
     #        self.assertNotEqual(len(messages), 0)
     #    else:
     #        self.fail("Cannot find document")
 
 
@@ -3749,40 +3818,40 @@
 
     #def test_messages_body_contains(self) -> None:
     #    messages = list(self.dt.messages(body_contains="draft-mcquistin-augmented-ascii-diagrams-05"))
     #    self.assertNotEqual(len(messages), 0)
 
 
     def test_send_queue_entry(self) -> None:
-        send_queue_entry = self.dt.send_queue_entry(SendQueueURI("/api/v1/message/sendqueue/1/"))
+        send_queue_entry = self.dt.send_queue_entry(SendQueueURI(uri="/api/v1/message/sendqueue/1/"))
         if send_queue_entry is not None:
-            self.assertEqual(send_queue_entry.by,           PersonURI("/api/v1/person/person/105651/"))
+            self.assertEqual(send_queue_entry.by,           PersonURI(uri="/api/v1/person/person/105651/"))
             self.assertEqual(send_queue_entry.id,           1)
-            self.assertEqual(send_queue_entry.message,      DTMessageURI("/api/v1/message/message/4001/"))
+            self.assertEqual(send_queue_entry.message,      DTMessageURI(uri="/api/v1/message/message/4001/"))
             self.assertEqual(send_queue_entry.note,         "")
-            self.assertEqual(send_queue_entry.resource_uri, SendQueueURI("/api/v1/message/sendqueue/1/"))
+            self.assertEqual(send_queue_entry.resource_uri, SendQueueURI(uri="/api/v1/message/sendqueue/1/"))
             self.assertEqual(send_queue_entry.send_at,      None)
             self.assertEqual(send_queue_entry.sent_at,      datetime.fromisoformat("2005-04-27T22:21:09-07:00"))
             self.assertEqual(send_queue_entry.time,         datetime.fromisoformat("2005-04-26T22:21:09-07:00"))
         else:
             self.fail("Cannot find send queue entry")
 
 
     def test_send_queue(self) -> None:
         send_queue = self.dt.send_queue()
         self.assertIsNot(send_queue, None)
 
 
     def test_send_queue_by(self) -> None:
-        send_queue = self.dt.send_queue(by=self.dt.person(PersonURI("/api/v1/person/person/105651/")))
+        send_queue = self.dt.send_queue(by=self.dt.person(PersonURI(uri="/api/v1/person/person/105651/")))
         self.assertIsNot(send_queue, None)
 
 
     #def test_send_queue_message(self) -> None:
-    #    message = self.dt.message(DTMessageURI("/api/v1/message/message/4001/"))
+    #    message = self.dt.message(DTMessageURI(uri="/api/v1/message/message/4001/"))
     #    if message is not None:
     #        send_queue = list(self.dt.send_queue(message = message))
     #        self.assertEqual(len(send_queue),  1)
     #        self.assertEqual(send_queue[0].id, 1)
     #    else:
     #        self.fail("Cannot find message")
```

### Comparing `ietfdata-0.6.8/tests/test_datatracker_coverage.py` & `ietfdata-0.7.0/tests/test_datatracker_coverage.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,19 +107,19 @@
         for endpoint_uri in self.endpoint_uris:
             if endpoint_uri not in ignored_endpoints:
                 with self.subTest(msg=endpoint_uri):
                     if endpoint_uri not in covered_uris:
                         self.fail(f"No API methods for datatracker endpoint {endpoint_uri}")
 
 
-    def test_endpoint_fields(self) -> None:
-        for uri in self.dt._hints:
-            if uri in self.endpoint_uris:
-                with self.subTest(msg=f"{uri}, {self.dt._hints[uri].obj_type.__name__}"):
-                    fields_in_object = list(self.dt._hints[uri].obj_type.__dict__["__dataclass_fields__"].keys())
-                    fields_in_schema = self.endpoint_uris[uri]
-                    for object_field in fields_in_object:
-                        self.assertIn(object_field, fields_in_schema, msg="object has field not in schema")
-                    for schema_field in fields_in_schema:
-                        self.assertIn(schema_field, fields_in_object, msg="schema has field not in object")
-                    self.assertCountEqual(fields_in_object, fields_in_schema)
+    #def test_endpoint_fields(self) -> None:
+    #    for uri in self.dt._hints:
+    #        if uri in self.endpoint_uris:
+    #            with self.subTest(msg=f"{uri}, {self.dt._hints[uri].obj_type.__name__}"):
+    #                fields_in_object = list(self.dt._hints[uri].obj_type.__dict__["__dataclass_fields__"].keys())
+    #                fields_in_schema = self.endpoint_uris[uri]
+    #                for object_field in fields_in_object:
+    #                    self.assertIn(object_field, fields_in_schema, msg="object has field not in schema")
+    #                for schema_field in fields_in_schema:
+    #                    self.assertIn(schema_field, fields_in_object, msg="schema has field not in object")
+    #                self.assertCountEqual(fields_in_object, fields_in_schema)
```

### Comparing `ietfdata-0.6.8/tests/test_mailarchive.py` & `ietfdata-0.7.0/tests/test_mailarchive2.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 import pymongo 
 
 from pathlib       import Path
 from unittest.mock import patch, Mock
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
-from ietfdata.datatracker import *
-from ietfdata.mailarchive import *
+from ietfdata.datatracker  import *
+from ietfdata.mailarchive2 import *
 
 
 # =================================================================================================================================
 # Unit tests:
 
 class TestMailArchive(unittest.TestCase):
     dt : DataTracker
@@ -66,21 +66,12 @@
     def test_mailarchive_mailing_list(self) -> None:
         mlist = self.ma.mailing_list("100attendees")
         mlist.update()
         self.assertEqual(mlist.name(), "100attendees")
         self.assertEqual(mlist.num_messages(), 434)
 
 
-    def test_mailarchive_message_from_archive_url(self) -> None:
-        msg = self.ma.message_from_archive_url("https://mailarchive.ietf.org/arch/msg/100attendees/w-zDVgSif2qjO4zhl3TUokb-ZNM")
-        if msg is not None:
-            self.assertEqual(msg.list_name,  "100attendees")
-            self.assertEqual(msg.message_id, "<75EBC4EB-32D0-4D65-AC17-BEFDAB13AC00@gmail.com>")
-            self.assertEqual(msg._imap_uid,  333)
-        else:
-            self.fail("Cannot find message: https://mailarchive.ietf.org/arch/msg/100attendees/w-zDVgSif2qjO4zhl3TUokb-ZNM")
-
 if __name__ == '__main__':
     unittest.main()
 
 # =================================================================================================================================
 # vim: set tw=0 ai:
```

### Comparing `ietfdata-0.6.8/tests/test_rfcindex.py` & `ietfdata-0.7.0/tests/test_rfcindex.py`

 * *Files identical despite different names*

