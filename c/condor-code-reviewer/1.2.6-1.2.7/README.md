# Comparing `tmp/condor_code_reviewer-1.2.6.tar.gz` & `tmp/condor_code_reviewer-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condor_code_reviewer-1.2.6.tar", last modified: Thu Apr 18 04:14:45 2024, max compression
+gzip compressed data, was "condor_code_reviewer-1.2.7.tar", last modified: Thu Apr 18 04:18:38 2024, max compression
```

## Comparing `condor_code_reviewer-1.2.6.tar` & `condor_code_reviewer-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.052969 condor_code_reviewer-1.2.6/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:14:45.052755 condor_code_reviewer-1.2.6/PKG-INFO
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.052552 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/
--rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/entry_points.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/requires.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 04:14:45.000000 condor_code_reviewer-1.2.6/condor_code_reviewer.egg-info/top_level.txt
--rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 04:14:45.053009 condor_code_reviewer-1.2.6/setup.cfg
--rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 04:14:39.000000 condor_code_reviewer-1.2.6/setup.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.051829 condor_code_reviewer-1.2.6/src/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.6/src/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.6/src/cli.py
-drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:14:45.052291 condor_code_reviewer-1.2.6/src/lib/
--rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.6/src/lib/__init__.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-04-18 04:10:06.000000 condor_code_reviewer-1.2.6/src/lib/github_pr.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.6/src/lib/openai_assistant.py
--rw-r--r--   0 cparedesr   (501) staff       (20)     2399 2024-04-18 04:14:33.000000 condor_code_reviewer-1.2.6/src/reviewer.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:18:38.328272 condor_code_reviewer-1.2.7/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:18:38.328043 condor_code_reviewer-1.2.7/PKG-INFO
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:18:38.327811 condor_code_reviewer-1.2.7/condor_code_reviewer.egg-info/
+-rw-r--r--   0 cparedesr   (501) staff       (20)      110 2024-04-18 04:18:38.000000 condor_code_reviewer-1.2.7/condor_code_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 cparedesr   (501) staff       (20)      386 2024-04-18 04:18:38.000000 condor_code_reviewer-1.2.7/condor_code_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        1 2024-04-18 04:18:38.000000 condor_code_reviewer-1.2.7/condor_code_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       40 2024-04-18 04:18:38.000000 condor_code_reviewer-1.2.7/condor_code_reviewer.egg-info/entry_points.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       16 2024-04-18 04:18:38.000000 condor_code_reviewer-1.2.7/condor_code_reviewer.egg-info/requires.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)        4 2024-04-18 04:18:38.000000 condor_code_reviewer-1.2.7/condor_code_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 cparedesr   (501) staff       (20)       38 2024-04-18 04:18:38.328322 condor_code_reviewer-1.2.7/setup.cfg
+-rw-r--r--   0 cparedesr   (501) staff       (20)      307 2024-04-18 04:18:36.000000 condor_code_reviewer-1.2.7/setup.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:18:38.326970 condor_code_reviewer-1.2.7/src/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-26 23:26:52.000000 condor_code_reviewer-1.2.7/src/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1948 2024-03-27 00:51:27.000000 condor_code_reviewer-1.2.7/src/cli.py
+drwxr-xr-x   0 cparedesr   (501) staff       (20)        0 2024-04-18 04:18:38.327412 condor_code_reviewer-1.2.7/src/lib/
+-rw-r--r--   0 cparedesr   (501) staff       (20)        0 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.7/src/lib/__init__.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2902 2024-04-18 04:10:06.000000 condor_code_reviewer-1.2.7/src/lib/github_pr.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     1688 2024-03-19 00:32:11.000000 condor_code_reviewer-1.2.7/src/lib/openai_assistant.py
+-rw-r--r--   0 cparedesr   (501) staff       (20)     2409 2024-04-18 04:17:42.000000 condor_code_reviewer-1.2.7/src/reviewer.py
```

### Comparing `condor_code_reviewer-1.2.6/src/cli.py` & `condor_code_reviewer-1.2.7/src/cli.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.6/src/lib/github_pr.py` & `condor_code_reviewer-1.2.7/src/lib/github_pr.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.6/src/lib/openai_assistant.py` & `condor_code_reviewer-1.2.7/src/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `condor_code_reviewer-1.2.6/src/reviewer.py` & `condor_code_reviewer-1.2.7/src/reviewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
             first_change_line = self._get_first_change_line(diff)
 
             if response and response != 'APIError: No response':
                 self.gh.comment_on_file(filename, response, first_change_line)
 
     def _get_first_change_line(self, diff):
-        match = re.search(r'@@ -(\d+),', diff)
+        match = re.search(r'@@ -\d+,\d+ \+(\d+),', diff)
         if match:
             return int(match.group(1))
         else:
             return 1
 
     def summary_review(self):
         summary = self.assistant.add_and_retrieve_message("Summary Review", "user")
```

