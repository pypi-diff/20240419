# Comparing `tmp/redditharbor-0.2.2.tar.gz` & `tmp/redditharbor-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redditharbor-0.2.2.tar", last modified: Thu Mar 14 21:01:01 2024, max compression
+gzip compressed data, was "redditharbor-0.2.3.tar", last modified: Fri Apr 19 05:56:02 2024, max compression
```

## Comparing `redditharbor-0.2.2.tar` & `redditharbor-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 21:01:01.951659 redditharbor-0.2.2/
--rw-rw-rw-   0        0        0     1084 2023-12-06 15:35:46.000000 redditharbor-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      153 2024-01-09 02:55:52.000000 redditharbor-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      798 2024-03-14 21:01:01.951659 redditharbor-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    13926 2024-03-04 03:27:18.000000 redditharbor-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 21:01:01.912145 redditharbor-0.2.2/redditharbor/
--rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.2/redditharbor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:01:01.938660 redditharbor-0.2.2/redditharbor/dock/
--rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.2/redditharbor/dock/__init__.py
--rw-rw-rw-   0        0        0    42487 2024-03-14 20:50:02.000000 redditharbor-0.2.2/redditharbor/dock/pipeline.py
--rw-rw-rw-   0        0        0     7044 2023-12-22 18:42:34.000000 redditharbor-0.2.2/redditharbor/login.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:01:01.948661 redditharbor-0.2.2/redditharbor/utils/
--rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.2/redditharbor/utils/__init__.py
--rw-rw-rw-   0        0        0    43125 2024-03-14 20:52:05.000000 redditharbor-0.2.2/redditharbor/utils/download.py
--rw-rw-rw-   0        0        0     6026 2024-02-16 11:32:00.000000 redditharbor-0.2.2/redditharbor/utils/fetch.py
--rw-rw-rw-   0        0        0     1683 2023-12-18 14:33:43.000000 redditharbor-0.2.2/redditharbor/utils/metrics.py
--rw-rw-rw-   0        0        0     6025 2023-12-21 19:53:08.000000 redditharbor-0.2.2/redditharbor/utils/subreddit_collections.py
-drwxrwxrwx   0        0        0        0 2024-03-14 21:01:01.950659 redditharbor-0.2.2/redditharbor.egg-info/
--rw-rw-rw-   0        0        0      798 2024-03-14 21:01:01.000000 redditharbor-0.2.2/redditharbor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-03-14 21:01:01.000000 redditharbor-0.2.2/redditharbor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 21:01:01.000000 redditharbor-0.2.2/redditharbor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2024-03-14 21:01:01.000000 redditharbor-0.2.2/redditharbor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-14 21:01:01.000000 redditharbor-0.2.2/redditharbor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-14 21:01:01.962659 redditharbor-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      997 2024-03-14 21:00:28.000000 redditharbor-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.721027 redditharbor-0.2.3/
+-rw-rw-rw-   0        0        0     1084 2023-12-06 15:35:46.000000 redditharbor-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      153 2024-01-09 02:55:52.000000 redditharbor-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      798 2024-04-19 05:56:02.720028 redditharbor-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10060 2024-04-18 14:29:48.000000 redditharbor-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.617356 redditharbor-0.2.3/redditharbor/
+-rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.704586 redditharbor-0.2.3/redditharbor/dock/
+-rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/dock/__init__.py
+-rw-rw-rw-   0        0        0    52389 2024-04-11 00:15:31.000000 redditharbor-0.2.3/redditharbor/dock/pipeline.py
+-rw-rw-rw-   0        0        0     7044 2023-12-22 18:42:34.000000 redditharbor-0.2.3/redditharbor/login.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.714068 redditharbor-0.2.3/redditharbor/utils/
+-rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/utils/__init__.py
+-rw-rw-rw-   0        0        0    43299 2024-03-18 14:45:00.000000 redditharbor-0.2.3/redditharbor/utils/download.py
+-rw-rw-rw-   0        0        0     6026 2024-02-16 11:32:00.000000 redditharbor-0.2.3/redditharbor/utils/fetch.py
+-rw-rw-rw-   0        0        0     1683 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/utils/metrics.py
+-rw-rw-rw-   0        0        0     6025 2023-12-21 19:53:08.000000 redditharbor-0.2.3/redditharbor/utils/subreddit_collections.py
+drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.717660 redditharbor-0.2.3/redditharbor.egg-info/
+-rw-rw-rw-   0        0        0      798 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-19 05:56:02.723318 redditharbor-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      997 2024-04-19 05:55:46.000000 redditharbor-0.2.3/setup.py
```

### Comparing `redditharbor-0.2.2/LICENSE` & `redditharbor-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.2/PKG-INFO` & `redditharbor-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: redditharbor
-Version: 0.2.2
+Version: 0.2.3
 Summary: Effortlessly collect and store Reddit data in your database.
 Home-page: https://github.com/socius-org/RedditHarbor/
-Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.3.tar.gz
 Author: Nick S.H Oh
 Author-email: research@socius.org
 License: MIT
 Keywords: Reddit,Supabase,reddit-api,database,reddit-crawler,reddit-scraper
 License-File: LICENSE
 Requires-Dist: praw==7.7.1
 Requires-Dist: supabase==1.0.3
 Requires-Dist: rich==13.4.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: presidio-analyzer==2.2.351
 Requires-Dist: presidio-anonymizer==2.2.351
-Requires-Dist: pillow==10.2.0
+Requires-Dist: pillow>=10.2.0
 Requires-Dist: requests==2.31.0
 Provides-Extra: pii
 Requires-Dist: spacy[en_core_web_lg]; extra == "pii"
```

### Comparing `redditharbor-0.2.2/redditharbor/dock/pipeline.py` & `redditharbor-0.2.3/redditharbor/dock/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,32 +2,37 @@
 import logging.config
 from typing import List, Tuple, Optional
 import datetime
 import praw
 import supabase
 from rich.console import Console
 from rich.traceback import install
+from rich.progress import track
 from presidio_analyzer import AnalyzerEngine
 from presidio_anonymizer import AnonymizerEngine
+import threading
+from threading import Event
+import time
 
 console = Console(record=True)
 install()
 
-logging.config.dictConfig({
-    "version": 1, 
-    "disable_existing_loggers": True
-})
+logging.config.dictConfig({"version": 1, "disable_existing_loggers": True})
 
-# Could potentially relocate this within collect.__init__ to improve speed of loading, when not masking pii.  
+# Could potentially relocate this within collect.__init__ to improve speed of loading, when not masking pii.
 pii_analyzer = AnalyzerEngine()
 pii_anonymizer = AnonymizerEngine()
 
+
 class collect:
     def __init__(
-        self, reddit_client: praw.Reddit, supabase_client: supabase.Client, db_config: dict = None
+        self,
+        reddit_client: praw.Reddit,
+        supabase_client: supabase.Client,
+        db_config: dict = None,
     ):
         """
         Initialize the Collect instance for collecting data from Reddit and storing it in Supabase.
 
         Args:
             reddit_client (praw.Reddit): The Reddit client used for interacting with Reddit's API.
             supabase_client (supabase.Client): The Supabase client used for database interaction.
@@ -50,34 +55,34 @@
 
             self.redditor_db = self.supabase.table(self.redditor_db_config)
             self.submission_db = self.supabase.table(self.submission_db_config)
             self.comment_db = self.supabase.table(self.comment_db_config)
 
         else:
             raise ValueError("Invalid input: db_config must be provided.")
-        
-        #Check and create "error_log" folder 
+
+        # Check and create "error_log" folder
         self.error_log_path = os.path.join(os.getcwd(), "error_log")
         os.makedirs(self.error_log_path, exist_ok=True)
-    
+
     def redditor_data(self, praw_models: praw.models, insert: bool) -> Tuple[str, bool]:
         """
         Collects and stores data related to a specific Redditor.
 
         Args:
             praw_models (praw.models): An object containing praw models.
             insert (bool): Insert redditor data to DB. 
 
         Returns:
             Tuple[str, bool]: A tuple containing the unique identifier of the Redditor collected and a boolean indicating whether the Redditor was inserted in the database.
         """
         redditor_inserted = False
         redditor = praw_models.author
-        
-        if insert is True: 
+
+        if insert is True:
             if hasattr(redditor, "id"):
                 redditor_id = redditor.id
                 """IF redditor_id in REDDITOR_DB, pass. ELSE, UPDATE REDDITOR_DB with new redditor"""
                 id_filter = (
                     self.redditor_db.select("redditor_id")
                     .eq("redditor_id", redditor_id)
                     .execute()
@@ -124,15 +129,15 @@
                         is_moderator = None
 
                     num_trophies = len(redditor.trophies())
                     if num_trophies != 0:
                         trophy = []
                         for t in range(num_trophies):
                             trophy.append(redditor.trophies()[t].name)
-                        trophy = {"list": trophy}
+                        trophy = {"list": trophy, "count": num_trophies}
                     elif num_trophies == 0:
                         trophy = None
                     removed = "active"
 
             else:  # Suspended or Deleted
                 if hasattr(redditor, "name") and redditor.is_suspended is True:
                     name = redditor.name
@@ -176,58 +181,61 @@
                         is_gold = None
                         is_moderator = None
                         trophy = None
                         removed = "suspended"
                 elif redditor is None:  # Deleted
                     redditor_id = "deleted"
                     return redditor_id, redditor_inserted
-            
+
             row = {
                 "redditor_id": redditor_id,
                 "name": name,
                 "created_at": created_at,
                 "karma": karma,
                 "is_gold": is_gold,
                 "is_mod": is_moderator,
                 "trophy": trophy,
                 "removed": removed,
             }
 
             self.redditor_db.insert(row).execute()
             redditor_inserted = True
             return redditor_id, redditor_inserted
-        
-        else: 
+
+        else:
             if hasattr(redditor, "id"):
                 redditor_id = redditor.id
-            else: 
+            else:
                 if hasattr(redditor, "name") and redditor.is_suspended is True:
                     redditor_id = "suspended" + ":" + redditor.name
-                elif redditor is None: 
+                elif redditor is None:
                     redditor_id = "deleted"
-                    
+
             return redditor_id, redditor_inserted
 
     def submission_data(
-        self, submission: praw.models.reddit.submission.Submission, mask_pii: bool, insert_redditor: bool = True 
+        self,
+        submission: praw.models.reddit.submission.Submission,
+        mask_pii: bool,
+        insert_redditor: bool = True,
     ) -> Tuple[str, int, int]:
         """
         Collects and stores submissions and associated users in a specified subreddit.
 
         Args:
             submission (praw.models.reddit.submission.Submission): The praw Submission object representing the submission.
 
         Returns:
             Tuple[str, int, int]: A tuple containing the submission id, the count of inserted submissions and the count of inserted Redditors.
         """
         accessed_at = datetime.datetime.utcnow()
         submission_id = submission.id
         submission_inserted = False
         redditor_inserted = False
-        
+
         id_filter = (
             self.submission_db.select("submission_id")
             .eq("submission_id", submission_id)
             .execute()
             .dict()["data"]
         )
         if len(id_filter) == 1:
@@ -240,29 +248,35 @@
         else:
             console.log(
                 "Submission [bold red]{}[/] not in DB. Adding to DB-{}".format(
                     submission_id, self.submission_db_config
                 )
             )
 
-            redditor_id, redditor_inserted = self.redditor_data(submission, insert=insert_redditor) #consider not saving if redditor_id is "deleted"
+            redditor_id, redditor_inserted = self.redditor_data(
+                submission, insert=insert_redditor
+            )  # consider not saving if redditor_id is "deleted"
             created_at = datetime.datetime.fromtimestamp(submission.created_utc)
             title = submission.title
-            
+
             selftext = submission.selftext
-            if mask_pii is True: 
-                #presidio assumes you know what language you are sending to it. 
-                #consider using a language detection mechanism, or user to set language
-                pii_results = pii_analyzer.analyze(text=selftext, language="en", return_decision_process=False)
-                selftext = pii_anonymizer.anonymize(text=selftext, analyzer_results=pii_results).text
-            
+            if mask_pii is True:
+                # presidio assumes you know what language you are sending to it.
+                # consider using a language detection mechanism, or user to set language
+                pii_results = pii_analyzer.analyze(
+                    text=selftext, language="en", return_decision_process=False
+                )
+                selftext = pii_anonymizer.anonymize(
+                    text=selftext, analyzer_results=pii_results
+                ).text
+
             subreddit = submission.subreddit.display_name
             permalink = "https://www.reddit.com" + submission.permalink
             attachment = None
-            
+
             if submission.is_reddit_media_domain:
                 if submission.is_video:
                     attachment = {"video": submission.url}
                 else:
                     if ".jpg" in submission.url:
                         attachment = {"jpg": submission.url}
                     elif ".png" in submission.url:
@@ -373,15 +387,18 @@
 
             self.submission_db.insert(row).execute()
             submission_inserted = True
 
         return submission_id, submission_inserted, redditor_inserted
 
     def comment_data(
-        self, comments: List[praw.models.reddit.comment.Comment], mask_pii: bool, insert_redditor: bool = True 
+        self,
+        comments: List[praw.models.reddit.comment.Comment],
+        mask_pii: bool,
+        insert_redditor: bool = True,
     ) -> Tuple[int, int]:
         """
         Collects and stores comment data associated with a list of comments.
 
         Args:
             comments (List[praw.models.reddit.comment.Comment]): A list of praw Comment objects to collect and store.
 
@@ -413,24 +430,30 @@
                         "Adding comment [bold red]{}[/] to DB-{}".format(
                             comment_id, self.comment_db_config,
                         )
                     )
                     link_id = comment.link_id.replace("t3_", "")
                     subreddit = str(comment.subreddit)
                     parent_id = comment.parent_id
-                    redditor_id, redditor_inserted = self.redditor_data(comment, insert=insert_redditor) #consider not saving if redditor_id is "deleted"
+                    redditor_id, redditor_inserted = self.redditor_data(
+                        comment, insert=insert_redditor
+                    )  # consider not saving if redditor_id is "deleted"
                     if redditor_inserted is True:
                         redditor_inserted_count += 1
 
                     created_at = datetime.datetime.fromtimestamp(comment.created_utc)
 
                     selfbody = comment.body
-                    if mask_pii is True: 
-                        pii_results = pii_analyzer.analyze(text=selfbody, language="en", return_decision_process=False)
-                        selfbody = pii_anonymizer.anonymize(text=selfbody, analyzer_results=pii_results).text
+                    if mask_pii is True:
+                        pii_results = pii_analyzer.analyze(
+                            text=selfbody, language="en", return_decision_process=False
+                        )
+                        selfbody = pii_anonymizer.anonymize(
+                            text=selfbody, analyzer_results=pii_results
+                        ).text
                     removed = None
 
                     if comment.edited is False:
                         edited = False
                     else:
                         edited = True
 
@@ -458,21 +481,27 @@
 
                     self.comment_db.insert(row).execute()
                     comment_inserted_count += 1
 
             except Exception as error:
                 console.log(f"t1_{comment.id}: [bold red]{error}[/]")
                 console.print_exception()
-                console.save_html(os.path.join(self.error_log_path, f"t1_{comment.id}.html"))
+                console.save_html(
+                    os.path.join(self.error_log_path, f"t1_{comment.id}.html")
+                )
                 continue
 
         return comment_inserted_count, redditor_inserted_count
 
     def subreddit_submission(
-        self, subreddits: List[str], sort_types: List[str], limit: int = 10, mask_pii: bool = False
+        self,
+        subreddits: List[str],
+        sort_types: List[str],
+        limit: int = 10,
+        mask_pii: bool = False,
     ) -> None:
         """
         Lazy collection. Collects and stores submissions and associated users in specified subreddits.
 
         Args:
             subreddits (List[str]): A list of subreddit names to collect submissions from.
             sort_types (List[str]): A list of sorting types for submissions (e.g., 'hot', 'new', 'rising', 'top', 'controversial').
@@ -496,40 +525,44 @@
                     r_ = self.reddit.subreddit(subreddit)
                     for submission in getattr(r_, sort_type)(limit=limit):
                         try:
                             (
                                 submission_id,
                                 submission_inserted,
                                 redditor_inserted,
-                            ) = self.submission_data(submission=submission, mask_pii=mask_pii)
+                            ) = self.submission_data(
+                                submission=submission, mask_pii=mask_pii
+                            )
 
                             if submission_inserted is True:
                                 total_submission_inserted_count += 1
                             if redditor_inserted is True:
                                 total_redditor_inserted_count += 1
 
                         except Exception as error:
                             console.log(f"t3_{submission_id}: [bold red]{error}[/]")
                             console.print_exception()
                             console.save_html(
-                                os.path.join(self.error_log_path, f"t3_{submission_id}.html")
+                                os.path.join(
+                                    self.error_log_path, f"t3_{submission_id}.html"
+                                )
                             )
                             continue
 
         return console.print(
             f"[bold green]{total_submission_inserted_count} submission and {total_redditor_inserted_count} user data collected from subreddit(s) {subreddits}"
         )
 
     def subreddit_comment(
         self,
         subreddits: List[str],
         sort_types: List[str],
         limit: int = 10,
         level: Optional[int] = 1,
-        mask_pii: bool = False 
+        mask_pii: bool = False,
     ) -> None:
         """
         Lazy collection. Collects and stores comments and associated users in specified subreddits.
 
         Args:
             subreddits (List[str]): A list of subreddit names to collect comments from.
             sort_types (List[str]): A list of sorting types for submissions (e.g., 'hot', 'new', 'rising', 'top', 'controversial').
@@ -554,15 +587,15 @@
                     console.print(sort_type, justify="center")
 
                     r_ = self.reddit.subreddit(subreddit)
 
                     for submission in getattr(r_, sort_type)(limit=limit):
                         try:
                             submission_id = submission.id
-                            
+
                             link_id_filter = (
                                 self.comment_db.select("link_id")
                                 .eq("link_id", submission_id)
                                 .execute()
                                 .dict()["data"]
                             )
 
@@ -576,37 +609,41 @@
                             else:
                                 submission.comments.replace_more(limit=level)
                                 # len(submission.comments.list()) would often give different values to submission.num_comments
                                 comments = submission.comments.list()
                                 (
                                     comment_inserted_count,
                                     redditor_inserted_count,
-                                ) = self.comment_data(comments=comments, mask_pii=mask_pii)
+                                ) = self.comment_data(
+                                    comments=comments, mask_pii=mask_pii
+                                )
                                 total_comment_inserted_count += comment_inserted_count
                                 total_redditor_inserted_count += redditor_inserted_count
 
                         except Exception as error:
                             console.log(f"t3_{submission.id}: [bold red]{error}[/]")
                             console.print_exception()
                             console.save_html(
-                                os.path.join(self.error_log_path, f"t3_{submission.id}.html")
+                                os.path.join(
+                                    self.error_log_path, f"t3_{submission.id}.html"
+                                )
                             )
                             continue
 
         return console.print(
             f"[bold green]{total_comment_inserted_count} comment and {total_redditor_inserted_count} user data collected from subreddit(s) {subreddits}"
         )
 
     def subreddit_submission_and_comment(
         self,
         subreddits: List[str],
         sort_types: List[str],
         limit: int = 10,
         level: int = 1,
-        mask_pii: bool = False 
+        mask_pii: bool = False,
     ) -> None:
         """
         Lazy collection. Collects and stores submissions, comments and associated users in specified subreddits.
 
         Args:
             subreddits (List[str]): A list of subreddit names to collect comments from.
             sort_types (List[str]): A list of sorting types for submissions (e.g., 'hot', 'new', 'rising', 'top', 'controversial').
@@ -618,77 +655,89 @@
             None. Prints the count of collected submissions, comments and user data to the console.
         """
 
         with console.status(
             "[bold green]Collecting submissions, comments and users from subreddit(s)...",
             spinner="aesthetic",
         ):
-            total_submission_inserted_count = 0 
+            total_submission_inserted_count = 0
             total_comment_inserted_count = 0
             total_redditor_inserted_count = 0
 
             for subreddit in subreddits:
                 console.print(f"[bold]subreddit: {subreddit}", justify="center")
                 for sort_type in sort_types:
                     console.print(sort_type, justify="center")
                     r_ = self.reddit.subreddit(subreddit)
                     for submission in getattr(r_, sort_type)(limit=limit):
                         try:
-                            #Collect Submission
+                            # Collect Submission
                             (
                                 submission_id,
                                 submission_inserted,
                                 submission_redditor_inserted,
-                            ) = self.submission_data(submission=submission, mask_pii=mask_pii)
-                            
-                            if submission_inserted is True: 
-                                total_submission_inserted_count += 1 
-                            if submission_redditor_inserted is True: 
-                                total_redditor_inserted_count += 1 
-                            
-                            #Check if comments of submission were crawled
+                            ) = self.submission_data(
+                                submission=submission, mask_pii=mask_pii
+                            )
+
+                            if submission_inserted is True:
+                                total_submission_inserted_count += 1
+                            if submission_redditor_inserted is True:
+                                total_redditor_inserted_count += 1
+
+                            # Check if comments of submission were crawled
                             link_id_filter = (
                                 self.comment_db.select("link_id")
                                 .eq("link_id", submission_id)
                                 .execute()
                                 .dict()["data"]
                             )
-                            
+
                             if len(link_id_filter) >= 1:
                                 console.log(
                                     "Submission Link [bold red]{}[/] already in DB-{}".format(
                                         submission_id, self.comment_db_config
                                     )
                                 )
 
                             else:
                                 submission.comments.replace_more(limit=level)
                                 # len(submission.comments.list()) would often give different values to submission.num_comments
                                 comments = submission.comments.list()
                                 (
                                     comment_inserted_count,
                                     comment_redditor_inserted_count,
-                                ) = self.comment_data(comments=comments, mask_pii=mask_pii)
+                                ) = self.comment_data(
+                                    comments=comments, mask_pii=mask_pii
+                                )
                                 total_comment_inserted_count += comment_inserted_count
-                                total_redditor_inserted_count += comment_redditor_inserted_count
+                                total_redditor_inserted_count += (
+                                    comment_redditor_inserted_count
+                                )
 
                         except Exception as error:
                             console.log(f"t3_{submission.id}: [bold red]{error}[/]")
                             console.print_exception()
                             console.save_html(
-                                os.path.join(self.error_log_path, f"t3_{submission.id}.html")
+                                os.path.join(
+                                    self.error_log_path, f"t3_{submission.id}.html"
+                                )
                             )
                             continue
 
         return console.print(
             f"[bold green]{total_submission_inserted_count} submission, {total_comment_inserted_count} comment, and {total_redditor_inserted_count} user data collected from subreddit(s) {subreddits}"
         )
 
     def submission_from_user(
-        self, user_names: List[str], sort_types: List[str], limit: int = 10, mask_pii: bool = False
+        self,
+        user_names: List[str],
+        sort_types: List[str],
+        limit: int = 10,
+        mask_pii: bool = False,
     ) -> None:
         """
         Collects and stores submissions from specified user(s).
 
         Args:
             user_names (List[str]): A list of Reddit usernames from which to collect submissions.
             sort_types (List[str]): A list of sorting types for user's submissions (e.g., 'hot', 'new', 'rising', 'top', 'controversial').
@@ -716,15 +765,19 @@
                             )
                         ]
                         for submission in submissions:
                             try:
                                 (
                                     submission_id,
                                     submission_inserted,
-                                ) = self.submission_data(submission=submission, mask_pii=mask_pii)[:2]
+                                ) = self.submission_data(
+                                    submission=submission, mask_pii=mask_pii
+                                )[
+                                    :2
+                                ]
                                 if submission_inserted is True:
                                     total_submission_inserted_count += (
                                         submission_inserted
                                     )
                             except Exception as error:
                                 console.log(f"t3_{submission_id}: [bold red]{error}[/]")
                                 console.print_exception()
@@ -743,15 +796,19 @@
                         )
                         continue
         return console.print(
             f"[bold green]{total_submission_inserted_count} submission data collected from {len(user_names)} user(s)"
         )
 
     def comment_from_user(
-        self, user_names: List[str], sort_types: List[str], limit: int = 10, mask_pii: bool = False 
+        self,
+        user_names: List[str],
+        sort_types: List[str],
+        limit: int = 10,
+        mask_pii: bool = False,
     ) -> None:
         """
         Collects and stores comments from specified user(s).
 
         Args:
             user_names (List[str]): A list of Reddit usernames from which to collect comments. Must to user name, not id. 
             sort_types (List[str]): A list of sorting types for user's comments (e.g., 'hot', 'new', 'rising', 'top', 'controversial').
@@ -773,28 +830,30 @@
                     try:
                         comments = [
                             comment
                             for comment in getattr(redditor.comments, sort_type)(
                                 limit=limit
                             )
                         ]
-                        comment_inserted_count = self.comment_data(comments=comments, mask_pii=mask_pii)[0]
+                        comment_inserted_count = self.comment_data(
+                            comments=comments, mask_pii=mask_pii
+                        )[0]
                         total_comment_inserted_count += comment_inserted_count
                     except Exception as error:
                         console.log(f"user_{user_name}: [bold red]{error}[/]")
                         console.print_exception()
                         console.save_html(
                             os.path.join(self.error_log_path, f"user_{user_name}.html")
                         )
                         continue
 
         return console.print(
             f"[bold green]{total_comment_inserted_count} comment data collected from {len(user_names)} user(s)"
         )
-    
+
     def submission_by_keyword(
         self, subreddits: List[str], query: str, limit: int = 10, mask_pii: bool = False
     ) -> None:
         """
         Collects and stores submissions with specified keywords from given subreddits.
 
         You can customize the search behavior by leveraging boolean operators:
@@ -814,94 +873,323 @@
             limit (int, optional): Maximum number of submissions to collect. Defaults to 10.
             mask_pii (bool, optional): Mask (anonymise) personally identifiable information (PII). Defaults to False.
 
         Returns:
             None. Prints the count of collected submissions data to the console.
         """
 
-
         with console.status(
             "[bold green]Collecting submissions with specified keyword(s)...",
             spinner="aesthetic",
         ):
             total_submission_inserted_count = 0
             for subreddit in subreddits:
                 console.print(f"[bold]subreddit: {subreddit}", justify="center")
                 r_ = self.reddit.subreddit(subreddit)
                 for submission in r_.search(query, sort="relevance", limit=limit):
                     try:
-                        (
-                            submission_id,
-                            submission_inserted,
-                        ) = self.submission_data(submission=submission, mask_pii=mask_pii, insert_redditor=False)[:2]
+                        (submission_id, submission_inserted,) = self.submission_data(
+                            submission=submission,
+                            mask_pii=mask_pii,
+                            insert_redditor=False,
+                        )[:2]
 
                         if submission_inserted is True:
                             total_submission_inserted_count += 1
 
                     except Exception as error:
                         console.log(f"t3_{submission_id}: [bold red]{error}[/]")
                         console.print_exception()
                         console.save_html(
-                            os.path.join(self.error_log_path, f"t3_{submission_id}.html")
+                            os.path.join(
+                                self.error_log_path, f"t3_{submission_id}.html"
+                            )
                         )
                         continue
 
         return console.print(
             f"[bold green]{total_submission_inserted_count} submission data collected from subreddit(s) {subreddits} with query='{query}'"
         )
-    
-    def comment_from_submission( 
-        self, 
+
+    def comment_from_submission(
+        self,
         submission_ids: List[str],
-        level: Optional[int] = 1, 
-        mask_pii: bool = False 
+        level: Optional[int] = 1,
+        mask_pii: bool = False,
     ) -> None:
         """
         Collects and stores comments from specified submission id(s).
         
         Parameters:
             submission_ids (List[str]): A list of submission IDs from which to collect comments.
             level (Optional[int]): The depth of comments to collect. Defaults to 1.
             mask_pii (bool, optional): Mask (or anonymise) personally identifiable information (PII). Defaults to False.
 
         Returns:
             None
         """
         with console.status(
-            "[bold green]Collecting comments from submission id(s)...", spinner="aesthetic"
+            "[bold green]Collecting comments from submission id(s)...",
+            spinner="aesthetic",
         ):
             total_comment_inserted_count = 0
             for submission_id in submission_ids:
                 console.print(f"[bold]submission: {submission_id}", justify="center")
                 submission = self.reddit.submission(submission_id)
                 try:
-                     #Check if comments of submission were crawled
+                    # Check if comments of submission were crawled
                     link_id_filter = (
                         self.comment_db.select("link_id")
                         .eq("link_id", submission_id)
                         .execute()
                         .dict()["data"]
                     )
-                    
+
                     if len(link_id_filter) >= 1:
-                        console.log(f"Submission Link [bold red]{submission_id}[/] already in DB-{self.comment_db_config}")
+                        console.log(
+                            f"Submission Link [bold red]{submission_id}[/] already in DB-{self.comment_db_config}"
+                        )
 
                     else:
                         submission.comments.replace_more(limit=level)
                         comments = submission.comments.list()
-                        comment_inserted_count = self.comment_data(comments=comments, mask_pii=mask_pii, insert_redditor=False)[0]
+                        comment_inserted_count = self.comment_data(
+                            comments=comments, mask_pii=mask_pii, insert_redditor=False
+                        )[0]
                         total_comment_inserted_count += comment_inserted_count
                 except Exception as error:
                     console.log(f"t3_{submission.id}: [bold red]{error}[/]")
                     console.print_exception()
                     console.save_html(
                         os.path.join(self.error_log_path, f"t3_{submission.id}.html")
                     )
                     continue
         return console.print(
             f"[bold green]{total_comment_inserted_count} comment data collected from {len(submission_ids)} submission(s)"
         )
+
     # def user_from_submission(self):
     #     return
+
+    # def user_from_subreddit(self):
+    #     return
+
+
+class update:
+    """
+    Class to update data from Reddit to Supabase periodically.
     
-    # def user_from_subreddit(self): 
-    #     return 
+    Args:
+        reddit_client (praw.Reddit): Reddit client.
+        supabase_client (supabase.Client): Supabase client.
+        db_config (dict, optional): Database configuration. Defaults to None.
+    """
+
+    def __init__(
+        self,
+        reddit_client: praw.Reddit,
+        supabase_client: supabase.Client,
+        db_config: dict = None,
+    ) -> None:
+
+        if db_config is not None:
+            self.reddit = reddit_client
+            self.supabase = supabase_client
+
+            self.redditor_db_config = db_config["user"]
+            self.submission_db_config = db_config["submission"]
+            self.comment_db_config = db_config["comment"]
+
+            self.redditor_db = self.supabase.table(self.redditor_db_config)
+            self.submission_db = self.supabase.table(self.submission_db_config)
+            self.comment_db = self.supabase.table(self.comment_db_config)
+
+        else:
+            raise ValueError("Invalid input: db_config must be provided.")
+
+        # Get Row Counts for non-archived data
+        ## Submission
+        self.submission_row_count = (
+            self.submission_db.select("archived", count="exact")
+            .eq("archived", False)
+            .execute()
+            .count
+        )
+        ## Comment
+        # For comments, need to access both comment_db and submission_db
+        # First, get a list of DISTINCT link_IDs from comment_db
+        # Second, check if link_IDs are archived or not from submission_db
+        # Third, get a list of non-archived list_IDs
+        # Fourth, count number of rows with such a list
+
+        ## User
+        # TBD
+
+        # Event to signal the threads to stop
+        self.stop_event = Event()
+
+    def submission(self):
+        """
+        Update submission data from Reddit to Supabase.
+        """
+        page_size = 1000
+        page_numbers = (self.submission_row_count // page_size) + (
+            1 if self.submission_row_count % page_size != 0 else 0
+        )
+        start_row, end_row = 0, min(self.submission_row_count, page_size)
+
+        for page in range(1, page_numbers + 1):
+            if page == 1:
+                pass
+            elif page < (page_numbers - 1):
+                start_row += page_size
+                end_row += page_size
+            else:
+                start_row += page_size
+                end_row = self.submission_row_count
+
+            columns = set(["submission_id", "score", "upvote_ratio", "num_comments"])
+            # Give priority to most recent submissions in the paginated submission
+            paginated_submission = (
+                self.submission_db.select(*columns)
+                .eq("archived", False)
+                .order("created_at", desc=True)
+                .range(start_row, end_row)
+                .execute()
+                .model_dump()["data"]
+            )
+
+            for submission in track(
+                paginated_submission,
+                description=f"Updating submission in DB-{self.submission_db_config} {page}\{page_numbers}",
+            ):
+                submission_id = submission["submission_id"]
+                score, upvote_ratio, num_comments = (
+                    submission["score"],
+                    submission["upvote_ratio"],
+                    submission["num_comments"],
+                )
+
+                accessed_at = datetime.datetime.utcnow()
+                submission = self.reddit.submission(id=submission_id)
+
+                score.update(
+                    {accessed_at.isoformat(timespec="seconds"): submission.score}
+                )
+                upvote_ratio.update(
+                    {accessed_at.isoformat(timespec="seconds"): submission.upvote_ratio}
+                )
+                num_comments.update(
+                    {accessed_at.isoformat(timespec="seconds"): submission.num_comments}
+                )
+                archived = submission.archived
+                if archived is True:
+                    console.print(f"{submission_id} is archived")
+
+                self.submission_db.update(
+                    {
+                        "score": score,
+                        "upvote_ratio": upvote_ratio,
+                        "num_comments": num_comments,
+                        "archived": archived,
+                    }
+                ).eq("submission_id", submission_id).execute()
+
+    def run_task_with_interval(self, task: str, interval: int, duration: int) -> None:
+        """
+        Run the task with a specified interval and duration.
+        
+        Args:
+            task (str): Task to perform. 
+            interval (int): Time interval between tasks in seconds.
+            duration (int): Duration for which the task should run in seconds.
+        """
+        loop_start = time.time()
+        loop_end = loop_start + duration if duration else float("inf")
+        update_count = 0
+
+        while (
+            time.time() < loop_end and not self.stop_event.is_set()
+        ):  # Continue looping until the stop event is set
+            if task == "submission":
+                start = time.time()
+                self.submission()
+                update_count += 1
+                end = time.time()
+                difference = int(end - start)
+                if (
+                    difference >= interval
+                ):  # If updating the DB took more time than the update time interval
+                    pass
+                else:  # If updating the DB took less time than the update time interval
+                    console.log(
+                        f"[bold green]Updated successfully[/] ({difference} seconds). Commencing next schedule in {interval-difference} seconds"
+                    )
+                    time.sleep(interval - difference)
+
+            elif task == "comment":
+                row_count = None
+            elif task == "user":
+                row_count = None
+
+        self.stop_event.set()
+
+        return console.print(
+            f"[bold green]Processed {update_count} cycles of submission updates, each comprising {self.submission_row_count} submissions."
+        )
+
+    def schedule_task(self, task: str, duration: str) -> None:
+        """
+        Schedule the task with a specified duration and automatically determine the update time interval based on the Row Count.
+        
+        Args:
+            task (str): Task to perform. Avaliable tasks are 'submission'. 
+            duration (str): Duration for which the task should run. Options are '1hr', '6hr', '12hr', and '1d'.
+        """
+        tasks = ["submission", "comment", "user"]
+        # Get Row Count
+        if task in tasks:
+            if task == "submission":
+                row_count = self.submission_row_count
+            elif task == "comment":
+                row_count = None
+            elif task == "user":
+                row_count = None
+        else:
+            raise ValueError(
+                f"Invalid task type: {task}. Avaliable tasks are 'submission', 'comment', and 'user'."
+            )
+
+        # Automatically determine update time interval based on the Row Count
+        if row_count <= 1000:
+            interval = 10 * 60
+        elif row_count > 1000 and row_count <= 3000:
+            interval = 30 * 60
+        elif row_count > 3000 and row_count <= 6000:
+            interval = 60 * 60
+        elif row_count > 6000 and row_count <= 36000:
+            interval = 6 * 60 * 60
+        elif row_count > 36000 and row_count <= 72000:
+            interval = 12 * 60 * 60
+        elif row_count > 72000:
+            interval = 24 * 60 * 60
+
+        duration_in_seconds = {
+            "1hr": 60 * 60,
+            "6hr": 6 * 60 * 60,
+            "12hr": 12 * 60 * 60,
+            "1d": 24 * 60 * 60,
+        }
+
+        duration_seconds = duration_in_seconds.get(duration)
+        if duration_seconds:
+            threading.Thread(
+                target=self.run_task_with_interval,
+                args=(task, interval, duration_seconds,),
+                daemon=True,
+            ).start()
+            while not self.stop_event.is_set():
+                time.sleep(0.01)
+        else:
+            raise ValueError(
+                "Invalid duration interval. Avaliable durations are '1hr', '6hr', '12hr', and '1d'."
+            )
```

### Comparing `redditharbor-0.2.2/redditharbor/login.py` & `redditharbor-0.2.3/redditharbor/login.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.2/redditharbor/utils/download.py` & `redditharbor-0.2.3/redditharbor/utils/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,21 +391,23 @@
                             with open(path, 'wb') as file:
                                 file.write(response.content)
                             success += 1
                         else:
                             # console.print(f"[bold red]{response.status_code}[/]: Failed to download image (url: {img_url})") 
                             fail += 1 
                             failed_urls.append(img_url)
-
-        return console.print(
-            f"[bold green]{success} image files successfully downloaded and saved\n",
-            f"[bold red]Failed to download {fail} image files\n", 
-            f"Failed urls: {failed_urls}"
-        )
-
+        
+        if fail == 0: 
+            return console.print(f"[bold green]{success} image files successfully downloaded and saved\n")
+        else: 
+            return console.print(
+                f"[bold green]{success} image files successfully downloaded and saved\n",
+                f"[bold red]Failed to download {fail} image files\n", 
+                f"Failed urls: {failed_urls}"
+            )
 
 class comment:
     def __init__(
         self,
         supabase_client: supabase.Client,
         db_name: str,
         paginate: bool or dict = True,
```

### Comparing `redditharbor-0.2.2/redditharbor/utils/fetch.py` & `redditharbor-0.2.3/redditharbor/utils/fetch.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.2/redditharbor/utils/metrics.py` & `redditharbor-0.2.3/redditharbor/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.2/redditharbor/utils/subreddit_collections.py` & `redditharbor-0.2.3/redditharbor/utils/subreddit_collections.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.2/redditharbor.egg-info/PKG-INFO` & `redditharbor-0.2.3/redditharbor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: redditharbor
-Version: 0.2.2
+Version: 0.2.3
 Summary: Effortlessly collect and store Reddit data in your database.
 Home-page: https://github.com/socius-org/RedditHarbor/
-Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.2.tar.gz
+Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.3.tar.gz
 Author: Nick S.H Oh
 Author-email: research@socius.org
 License: MIT
 Keywords: Reddit,Supabase,reddit-api,database,reddit-crawler,reddit-scraper
 License-File: LICENSE
 Requires-Dist: praw==7.7.1
 Requires-Dist: supabase==1.0.3
 Requires-Dist: rich==13.4.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: presidio-analyzer==2.2.351
 Requires-Dist: presidio-anonymizer==2.2.351
-Requires-Dist: pillow==10.2.0
+Requires-Dist: pillow>=10.2.0
 Requires-Dist: requests==2.31.0
 Provides-Extra: pii
 Requires-Dist: spacy[en_core_web_lg]; extra == "pii"
```

### Comparing `redditharbor-0.2.2/setup.py` & `redditharbor-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup
 
 setup(
   name = 'redditharbor',
   packages = ['redditharbor'],   
-  version = '0.2.2',      
+  version = '0.2.3',      
   license='MIT',        
   description = 'Effortlessly collect and store Reddit data in your database.',   
   author = 'Nick S.H Oh',                   
   author_email = 'research@socius.org',      
   url = 'https://github.com/socius-org/RedditHarbor/',  
-  download_url = 'https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.2.tar.gz', 
+  download_url = 'https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.3.tar.gz', 
   keywords = ['Reddit', 'Supabase', 'reddit-api', 'database', 'reddit-crawler', 'reddit-scraper'],
   include_package_data=True,
   install_requires=[
           'praw == 7.7.1',
           'supabase == 1.0.3', 
           'rich == 13.4.2',
           'python-dotenv == 1.0.0',
           'presidio-analyzer == 2.2.351', 
           'presidio-anonymizer == 2.2.351',
-          'pillow == 10.2.0', 
+          'pillow >= 10.2.0', 
           'requests == 2.31.0'  
       ],
   extras_require={
     'pii': ['spacy[en_core_web_lg]'],
     }
 )
```

