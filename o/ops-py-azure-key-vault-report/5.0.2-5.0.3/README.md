# Comparing `tmp/ops_py_azure_key_vault_report-5.0.2.tar.gz` & `tmp/ops_py_azure_key_vault_report-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_report-5.0.2.tar", last modified: Tue Apr 16 14:12:19 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_report-5.0.3.tar", last modified: Fri Apr 19 13:57:41 2024, max compression
```

## Comparing `ops_py_azure_key_vault_report-5.0.2.tar` & `ops_py_azure_key_vault_report-5.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:19.164827 ops_py_azure_key_vault_report-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 14:12:16.000000 ops_py_azure_key_vault_report-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 14:12:19.164827 ops_py_azure_key_vault_report-5.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:19.164827 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/az_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19937 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/azure_key_vault_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/html_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1218 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/ms_teams_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/set_timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4149 2024-04-16 14:12:11.000000 ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/slack_payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:19.164827 ops_py_azure_key_vault_report-5.0.2/ops_py_azure_key_vault_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-16 14:12:19.000000 ops_py_azure_key_vault_report-5.0.2/ops_py_azure_key_vault_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-16 14:12:19.000000 ops_py_azure_key_vault_report-5.0.2/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:12:19.000000 ops_py_azure_key_vault_report-5.0.2/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 14:12:19.000000 ops_py_azure_key_vault_report-5.0.2/ops_py_azure_key_vault_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 14:12:16.000000 ops_py_azure_key_vault_report-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-16 14:12:16.000000 ops_py_azure_key_vault_report-5.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:12:19.164827 ops_py_azure_key_vault_report-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 14:12:16.000000 ops_py_azure_key_vault_report-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:41.855461 ops_py_azure_key_vault_report-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-19 13:57:41.855461 ops_py_azure_key_vault_report-5.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:41.851461 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/az_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25592 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/azure_key_vault_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/html_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/ms_teams_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/set_timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7390 2024-04-19 13:57:37.000000 ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/slack_payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:41.851461 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:57:41.000000 ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:57:41.855461 ops_py_azure_key_vault_report-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 13:57:39.000000 ops_py_azure_key_vault_report-5.0.3/setup.py
```

### Comparing `ops_py_azure_key_vault_report-5.0.2/LICENSE` & `ops_py_azure_key_vault_report-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/az_cmd.py` & `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/az_cmd.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/azure_key_vault_report.py` & `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/azure_key_vault_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,79 +10,116 @@
 from .slack_payloads import SlackPayloads
 
 
 ########################################################################################################################
 
 
 class AzureKeyVaultReport(object):
-    """generates a report from the results of 'az keyvault' commands
+    """Generates reports i various formats from the results of 'az keyvault' commands.
 
     The values of 'updated', 'created' and 'expires' are converted to date object
     and the age (in days) is calculated.
 
-    Then a table is generated and sorted by (from top to bottom):
-    the oldest 'Expiration' date, then by
-    the oldest 'Last Updated' date
-
-
     Attributes
     ----------
 
     results : list
         The list of results from the 'az keyvault' commands, enriched with 'vault_name' and 'record_type'
     items : list
         The list of items.
         Items are enriched with more data, e.g. age of each date element, vault_name, record_type, record_name
-    html_table :
-        The html table object which are used to provide an HTML table for the MS Teams payload.
     vaults : list
          The unique list of vaults processed
+    html_table :
+        The html table object which are used to provide an HTML table for the MS Teams payload.
     summary_values: dict
         The config for the summary report. Read from config.py
     report_values: dict
         The config for the report. Read from config.py
-    report: str
-        The report as standard Markdown
-    summary: str
-        The summary as standard Markdown
-
+    report: list
+        The list of filtered row items as dict
+    summary: dict
+        The summary of the report as dict
+    report_md : str
+        The text Markdown version of the report
+    summary_md : str
+        The text Markdown version of the summary
+    report_summary_md : str
+        The text Markdown version of the summary and report combined
+    slack_rows_md : list
+        The list of Slack messages formatted as Slack Markdown
+    report_full : dict
+        The full report, including the summary, as dict
 
     Methods
     -------
-
     parse_results()
         Parse through the provided 'results' from the azure cli keyvault cmd outputs.
         For each result in the results new item is created and added to the items list.
         Each item contains the following data:
         - Date objects, created from the 'updated', 'created' and 'expires' values and stored as values
           in new X_ts keys.
         - The age (in days) is calculated from each of the date objects and stored as values in new X_age keys.
         - 'vault_name' and 'record_type
-    add_report(self, expire_threshold=None, ignore_no_expiration=True, include_all=False, teams_json=False):
-        Creates a detailed 'column and rows' report, from which a Markdown table is generated.
-        An optional html may also be generated from this report.
-        The columns: "Record Name", "Record Type", "Vault Name", "Last Updated", "Expiration" and "Comment"
-        are defined in the 'config.py'
+
+    add_report(expire_threshold=None, critical_threshold=None,
+               ignore_no_expiration=True, include_all=False, teams_json=False):
+        Creates detailed 'column and rows' reports with comment according to the parameters passed.
+
+        The column names are defined in the 'config.py' file.
+
         The values for the "Comment" column is generated according to the age of 'updated', 'created' and 'expires'.
         If missing 'expires' then a comment concerning that is added.
+
+        When a row is completed it is added to the report(s), according to input arguments.
+        A json object of a completed row is ALWAYS created.
+
     add_summary()
-        Creates a Markdown table of the summary report. The text for this table is defined in the config.py
+        Creates a summary as a dict ('summary') and as a plain text Markdown table ('summary_md').
+
+        The heading / keys are defined in the config.py file.
+
+        The 'summary' dict is also added to the 'report_full' dict.
+
     sort_items():
         Returns a sorted list of all the records
-    get_markdown_report()
-        Returns the report(s) as Markdown table(s). The report and/or just the summary.
+
     get_teams_payload()
         Create and returns an MS Teams payload. The HTML table is added as a part of the payload, if no other
         text is provided as argument.
+
     get_html_table()
         Returns the HTML table which is used in the MS Teams payload.
-    get_markdown_report_only()
-        Returns the report as plaintext Markdown table.
-    get_markdown_summary()
-        Returns the summary as plaintext Markdown table.
+
+    get_slack_md(rows)
+        Creates a Slack Markdown of the provided list of rows.
+
+    create_kv_rows()
+        Creates key/value pairs of the items in the report rows
+
+    get_report_full()
+        Returns the dict version of the full report were all the rows are included and a dict of the summary.
+
+    get_report()
+        Returns a list of dict versions of the filtered rows.
+
+    get_summary()
+        Returns the dict version of the summary.
+
+    get_summary_markdown()
+        Returns a string with the plain text Markdown version of the summary.
+
+    get_report_markdown()
+        Returns a string with the plain text Markdown version of the report.
+
+    get_report_summary_markdown()
+        Returns a string with the plain text Markdown version of the summary and report combined.
+
+    get_slack_payloads(self, title, max_chars=3500, app=True, md=True)
+        Returns a list of Slack messages to be used in Slack posts.
     """
 
     def __init__(self, results):
         """
         Parameters
         ----------
         results : list
@@ -154,15 +191,16 @@
         sorted_list = sorted(expired, key=lambda x: (str(x.get('expires')), x.get('updated', ' ')), reverse=False)
         sorted_list += sorted(will_expire, key=lambda x: (str(x.get('expires')), x.get('updated', ' ')), reverse=False)
         sorted_list += sorted(others, key=lambda x: (str(x.get('expires')), x.get('updated', ' ')), reverse=False)
 
         return sorted_list
 
     def parse_results(self):
-        """parse through the result from the azure cli keyvault cmd output"""
+        """Parse through the result from the azure cli keyvault cmd output and build new enriched items."""
+
         if not isinstance(self.results, list):
             return
 
         for r in self.results:
             for o in r.get("out"):
                 item = {}
                 if isinstance(o, dict):
@@ -213,15 +251,16 @@
 
                             if "expires" in k and not v:
                                 self.summary_values["missing"]["value"] += 1
 
                 self.items.append(item)
 
     def add_summary(self):
-        """adds the summary as Markdown"""
+        """Creates a plain text Markdown version of the summary, and also add it to the 'report_full' dict."""
+
         self.summary = {}
         self.summary_values["vaults"]["value"] = len(self.vaults)
         self.summary_values["records"]["value"] = len(self.items)
 
         rows = []
         for k, v in self.summary_values.items():
             if "heading" in k:
@@ -234,26 +273,37 @@
                     self.summary[text] = value
 
         md = Markdown(rows)
         md.set_widths()
         self.summary_md = md.get_output(1)
         self.report_full["summary"]["rows"] = [self.summary]
 
-    def add_report(self, expire_threshold=None, ignore_no_expiration=True, include_all=False, teams_json=False,
-                   critical_threshold=None):
-        """creates a plain text report and initiates ms team report generation if specified.
-        returns the plain text report.
+    def add_report(self, expire_threshold=None, critical_threshold=None, ignore_no_expiration=True,
+                   include_all=False, teams_json=False):
+        """Creates a detailed 'column and rows' reports with comment.
+
+        The column names are defined in the 'config.py' file.
+
+        The values for the "Comment" column is generated according to the age of 'updated', 'created' and 'expires'.
+        If missing 'expires' then a comment concerning that is added.
+
+        When a row is completed it is added to the report(s), according to input arguments.
+        A json object of a completed row is ALWAYS created.
 
         Parameters
         ----------
         expire_threshold : int
             Ignore to report the record if days till the secret will expire are more than this 'expire_threshold' value
             NOTE: Secrets expiring today or already expired will always be reported.
+        critical_threshold : int
+            If specified, a Slack Markdown post of the row will be created, IF the row contains a record which days to
+            expiring/expired (+/-) are within the value of 'critical_threshold' value.
+            The markdown post will then be added to a 'slack_rows_md' list.
         ignore_no_expiration : bool
-            Report all records if set to False. If set to True only secrets with Expiration Date set will be reported.
+            Reports all records if set to False. If set to True only secrets with Expiration Date set will be reported.
         include_all : bool
             If set to True all records are included in the output.
         teams_json : bool
             If set to True then a report in json format containing a html table will also be generated.
         """
         if not isinstance(self.results, list):
             return
@@ -268,18 +318,14 @@
         rows_all = [self.report_values["heading"]]
 
         # Sort the items from top and down
         # First sort by the oldest 'Expiration' date
         # Then sort by the oldest 'Last Updated' date
         items = self.sort_items()
 
-        logging.info(f"expire_threshold: {expire_threshold} {type(expire_threshold)} - "
-                     f"ignore_no_expiration: {ignore_no_expiration} ({type(ignore_no_expiration)}) - "
-                     f"include_all: {include_all} {type(include_all)}")
-
         for item in items:
             # Get name of the record. If no name, we skip to next item in the list
             record_name = item.get("record_name")
             if not record_name:
                 continue
 
             # Get the record type
@@ -321,86 +367,140 @@
 
             if isinstance(updated_age, int):
                 comment += f"Updated {updated_age} days ago. "
 
             # A little cosmetic touch to avoid plural where it should not be used
             comment = comment.replace(" 1 days", " 1 day")
 
-            # Add to row: the value of: 'comment'
+            # Add the comment to the row
             row.append(comment)
 
+            # The row is now complete
             # Add the row to the rows_all (The ones that will be stored in db, but not necessarily will be alerted on)
             rows_all.append(row)
 
             # Only include disabled entries if set to include_all
             if not include_all and not enabled:
                 continue
 
             # Skip records with no Expiration Date set, only if 'ignore_no_expiration' and not 'include_all'
             if not expires:
                 if ignore_no_expiration and not include_all:
                     continue
 
-            # Handle those with Expiration Date
+            # If the record has Expiration Date set, check if it should be alerted and/or reported on
             if isinstance(expires_age, int):
-                # Handle those which has not expired yet
+
+                # The record has not expired yet, but it is logged.
                 if expires_age < 0:
-                    logging.info(f"'{record_name}' has not expired yet. "
+                    logging.info(f"{record_name} has not expired yet. "
                                  f"It will expire in {abs(expires_age)} days ({expires}).")
 
-                    # Handle those within valid 'expire_threshold'
+                # Check if soon expiring OR expired recently (the critical_threshold range)
+                # If so, a Slack Markdown Payload of current row will be created
+                # and added to the list of Slack Markdown payloads,
+                if isinstance(critical_threshold, int):
+                    slack_md = False
+
+                    # The record has not expired, but is within the critical_threshold range
+                    if 0 >= expires_age >= -critical_threshold:
+                        logging.info(f"{record_name} - expiring in {abs(expires_age)} days.")
+                        slack_md = True
+
+                    # The record has expired and is within the critical_threshold range
+                    if 0 < expires_age <= critical_threshold:
+                        logging.info(f"{record_name} - expired {expires_age} days ago.")
+                        slack_md = True
+
+                    if slack_md:
+                        logging.info(f"{record_name} - critical_threshold is set to '{critical_threshold}'.")
+                        logging.info(f"{record_name} - will be alerted to Slack.")
+                        slack_md_payload = self.get_slack_md(row)
+                        if slack_md_payload:
+                            logging.info(f"{record_name} - Slack Markdown payload created.")
+                            self.slack_rows_md.append(slack_md_payload)
+
+                    # Handle those within the valid 'expire_threshold' range
+                    # Those record will not be included in the standard report.
+                    # They will only be included in the full report or if 'include_all' is set to True
                     if isinstance(expire_threshold, int) and expire_threshold < abs(expires_age):
-                        logging.info(f"'{record_name}' Expiration Date is within the valid specified threshold of "
-                                     f"{expire_threshold} days. This record will start to be "
-                                     f"reported in {abs(expires_age) - expire_threshold} days.")
-
-                        # Only skipped if 'include_all' is not specified.
+                        logging.info(
+                            f"'{record_name}' - Expiration Date is within the valid specified threshold of "
+                            f"{expire_threshold} days. This record will start to be "
+                            f"reported in {abs(expires_age) - expire_threshold} days.")
+
+                        # This record is within the valid 'expire_threshold' range so the loop will
+                        # not proceed with adding the row the list of rows
+                        # unless if 'include_all' is set to True, then the row will be added.
                         if not include_all:
                             continue
 
-            # Then finally add the row to the rows (The ones that will be reported)
+            # Then finally add the row to the rows which will be reported on
             rows.append(row)
 
-            # Add Slack Markdown Payload of current row and add it is to list of Slack Markdown payloads,
-            # but only if it is within the critical range
-            if (isinstance(critical_threshold, int) and isinstance(expires_age, int)
-                    and (0 <= expires_age <= critical_threshold or 0 >= expires_age >= -critical_threshold)):
-                slack_md_payload = self.get_slack_md(row)
-                if slack_md_payload:
-                    self.slack_rows_md.append(slack_md_payload)
-
-            # If a html_table is created, then also add the row to the html table. Used in MS Teams payload
+            # If the teams_json argument was set to True, a html_table was created.
+            # If so, then the row is also added to the html table, which are used in the MS Teams payload.
             if self.html_table:
                 self.html_table.add_html_row(*row)
 
+        ################################################################################################################
+        # All the rows are now processed. Only the wanted rows are kept and will be used to create the reports
+
+        # A json object of all rows are always created.
         self.report_full["report"]["rows"] = self.create_kv_rows(rows_all)
 
+        # If 'include_all' argument is set to True, then 'all_rows' are used instead of the ones not filtered out.
         if include_all:
             rows = rows_all
 
         if not rows:
             logging.error("No report generated.")
             return
 
-        # Create markdown of the report
-        md = Markdown(rows)
-        md.set_widths()
+        # Create the reports
         if len(rows) > 1:
+            # Create a plain text Markdown of the report
+            md = Markdown(rows)
+            md.set_widths()
             self.report_md = md.get_output()
 
             # Create json of the report
             self.report = self.create_kv_rows(rows)
 
-        logging.info("report generated.")
+            logging.info("report generated.")
+
+    def create_kv_rows(self, rows):
+        """Creates key/value pairs of the items in the rows
+
+        Returns
+        -------
+        A list of row items as dicts.
+        """
+
+        kv_rows = []
+        for i, r in enumerate(rows):
+            if i > 0:
+                j = {}
+                for n, v in enumerate(self.report_values.get("heading")):
+                    j[v] = r[n]
+                kv_rows.append(j)
+        return kv_rows
 
     def get_slack_md(self, row):
+        """Creates a Slack Markdown of the row.
+
+        Returns
+        -------
+        A dict of the Slack item.
+        """
+
         if not row:
             return
 
-        payload = {
+        item = {
                 "blocks": [
                     {
                         "type": "header",
                         "text": {
                             "type": "plain_text",
                             "text": f"{row[0]}"
                         }
@@ -415,80 +515,115 @@
                     {
                         "type": "section",
                         "fields": []
                     }
                 ]
             }
 
-        blocks = payload.get("blocks")
+        blocks = item.get("blocks")
         for i in range(1, len(row)-1):
             x = {"type": "mrkdwn",
                  "text": f"*{self.report_values['heading'][i]}:*\n{row[i]}"
                  }
             blocks[-1]["fields"].append(x)
         blocks.append({"type": "divider"})
-        return payload
-
-    def create_kv_rows(self, rows):
-        kv_rows = []
-        for i, r in enumerate(rows):
-            if i > 0:
-                j = {}
-                for n, v in enumerate(self.report_values.get("heading")):
-                    j[v] = r[n]
-                kv_rows.append(j)
-        return kv_rows
+        return item
 
     def get_report_full(self):
+        """Returns the dict version of the full report were all the rows are included and a dict of the summary."""
+
         return self.report_full
 
     def get_report(self):
+        """Returns a list of dict versions of the filtered rows."""
+
         return self.report
 
     def get_summary(self):
+        """Returns the dict version of the summary."""
+
         return self.summary
 
     def get_summary_markdown(self):
-        """return the Markdown summary"""
+        """Returns a string with the plain text Markdown version of the summary."""
+
         return self.summary_md
 
     def get_report_markdown(self):
-        """return the Markdown report"""
+        """Returns a string with the plain text Markdown version of the report."""
+
         return self.report_md
 
     def get_report_summary_markdown(self):
-        """return the plain text report"""
+        """Returns a string with the plain text Markdown version of the summary and report combined."""
+
         if self.report_md:
             self.report_summary_md = f"{self.summary_md}\n\n{self.report_md}"
         else:
             self.report_summary_md = self.summary_md
 
         return self.report_summary_md
 
     def get_teams_payload(self, title, text=""):
-        """build and return the MS Teams payload"""
+        """Initiate the MSTeamsPayload class to build and return an MS Teams payload.
+
+        Parameters
+        ----------
+        title : string
+            The 'activityTitle' of the MS Teams payload
+        text : string
+            The 'text' part of the payload. If not provided, the generated 'html_table' will be used instead.
+
+        Returns
+        -------
+        A json dump (string) of the complete payload.
+        """
+
         if not isinstance(self.results, list):
             return
 
         if len(self.items) == 0:
             return
 
         if not text:
             text = self.get_html_table()
 
         ms_teams_payload = MSTeamsPayload(title, text, self.summary_values)
         ms_teams_payload.set_json_facts()
         return ms_teams_payload.get_json_output()
 
     def get_html_table(self):
-        """return the html table"""
+        """Returns the 'html_table as string'
+
+        None is returned if the 'add_report' method has not been executed with 'teams_json' argument set to True"""
+
         if self.html_table:
             return self.html_table.get_table()
 
-    def get_slack_payloads(self, title, max_chars=3500, app=True, md=True):
+    def get_slack_payloads(self, title, max_chars=3500, md=False, app=True):
+        """Returns a list of Slack messages to be used in Slack posts.
+
+        Parameters
+        ----------
+        title : string
+            Title/heading of the message.
+        max_chars : int
+            Message above this limit will be split into multiple parts
+            (default: 3500)
+        md : boolean
+            If set to True, the 'slack_rows_md' will be returned, which is a list of Slack items (dicts) to be posted to Slack.
+            This list has only been populated if the 'add_report' method has not been executed with a value for the
+            'critical_threshold' and the record in the row has met the 'critical_threshold' filter.
+        app : boolean
+            If True, a list of Slack items (dicts) to be used as payload for a Slack App is returned
+            If False, a list of Slack items in tuple pairs is returned. To be used to post to a Slack Workflow.
+
+            Note: Not relevant if 'md' is set to True
+
+        """
 
         if md:
             return self.slack_rows_md
 
         self.get_summary_markdown()
         self.get_report_summary_markdown()
         self.get_report_markdown()
```

### Comparing `ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/config.py` & `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/config.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/ms_teams_json.py` & `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/ms_teams_json.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.2/azure_key_vault_report/set_timestamp.py` & `ops_py_azure_key_vault_report-5.0.3/azure_key_vault_report/set_timestamp.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 import logging
 from datetime import datetime
 
 
 ########################################################################################################################
 
 def now():
+    """Returns current time and date: <year>-<month>-<day> <hour>:<minute>:<second>.<microsecond>
+
+    Returns
+    -------
+    datetime.datetime object
+    """
     return datetime.now()
 
 
 def set_timestamp(s, date_format=None):
     """Returns a date object of a string in format %Y-%m-%d.
 
     Parameters
@@ -19,15 +25,15 @@
         The date in string format
     date_format : str
         The expected format of the date string format.
         Please refer to https://strftime.org/
 
     Returns
     -------
-    datetime.datetime object
+    ts : datetime.datetime object
         If the provided string ('s') parameter is not in valid format, None is returned.
     """
 
     if not date_format:
         date_format = "%Y-%m-%d"
     try:
         ts = datetime.strptime(str(s), date_format)
```

### Comparing `ops_py_azure_key_vault_report-5.0.2/ops_py_azure_key_vault_report.egg-info/SOURCES.txt` & `ops_py_azure_key_vault_report-5.0.3/ops_py_azure_key_vault_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

