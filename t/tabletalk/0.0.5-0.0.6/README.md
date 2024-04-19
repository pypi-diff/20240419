# Comparing `tmp/tabletalk-0.0.5.tar.gz` & `tmp/tabletalk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabletalk-0.0.5.tar", last modified: Fri Apr 19 18:19:38 2024, max compression
+gzip compressed data, was "tabletalk-0.0.6.tar", last modified: Fri Apr 19 20:03:18 2024, max compression
```

## Comparing `tabletalk-0.0.5.tar` & `tabletalk-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:19:38.981783 tabletalk-0.0.5/
--rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.5/LICENSE
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 18:19:38.981542 tabletalk-0.0.5/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.5/README.md
--rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 18:19:38.981827 tabletalk-0.0.5/setup.cfg
--rw-r--r--   0 vinceberry   (501) staff       (20)     1154 2024-04-19 18:19:29.000000 tabletalk-0.0.5/setup.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:19:38.980506 tabletalk-0.0.5/tabletalk/
--rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.5/tabletalk/__init__.py
--rw-r--r--   0 vinceberry   (501) staff       (20)     2914 2024-04-19 18:19:11.000000 tabletalk-0.0.5/tabletalk/talk.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:19:38.981316 tabletalk-0.0.5/tabletalk.egg-info/
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/SOURCES.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/dependency_links.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/requires.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/top_level.txt
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:03:18.529873 tabletalk-0.0.6/
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.6/LICENSE
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 20:03:18.529624 tabletalk-0.0.6/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.6/README.md
+-rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 20:03:18.529925 tabletalk-0.0.6/setup.cfg
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1154 2024-04-19 20:03:04.000000 tabletalk-0.0.6/setup.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:03:18.528454 tabletalk-0.0.6/tabletalk/
+-rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.6/tabletalk/__init__.py
+-rw-r--r--   0 vinceberry   (501) staff       (20)     3400 2024-04-19 19:55:39.000000 tabletalk-0.0.6/tabletalk/talk.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:03:18.529358 tabletalk-0.0.6/tabletalk.egg-info/
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/requires.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/top_level.txt
```

### Comparing `tabletalk-0.0.5/LICENSE` & `tabletalk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tabletalk-0.0.5/PKG-INFO` & `tabletalk-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.5
+Version: 0.0.6
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tabletalk-0.0.5/setup.py` & `tabletalk-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'NL2SQL2RAG'
 LONG_DESCRIPTION = 'TableTalk allows you ask query your tabular data with natural language, then produces a generated response.'
 
 setup(
     name="tabletalk",
     version=VERSION,
     author="Vince Berry",
```

### Comparing `tabletalk-0.0.5/tabletalk/talk.py` & `tabletalk-0.0.6/tabletalk/talk.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from sqlalchemy import create_engine
 import pandas as pd
 from openai import OpenAI
+import os
 
 class TableTalk():
     def __init__(
             self,
             openai_api_key: str,
             csv_path: str,
+            generate_response: bool = True,
             ) -> None:
         self.openai_api_key = openai_api_key
         self.csv_path = csv_path
+        self.generate_response = generate_response
 
     def query_table(
             self,
             query: str,
-            table_name: str = 'data_table'
+            table_name: str = 'data_table',
+            save_source_data_as_csv: bool = False
             ) -> str:
         print('Scanning your data...')
         query = str(query).strip()
         table_name = str(table_name).strip()
         engine = create_engine("sqlite:///:memory:")
         df = pd.read_csv(self.csv_path)
         columns = df.columns
@@ -41,24 +45,30 @@
         sql_parse = response.choices[0].message.content.replace("'''sql",'').replace("'''",'').strip()
         new_df = pd.read_sql(sql_parse, engine)
         result = []
         for _, row in new_df.iterrows():
             row_str = ','.join([f'{col}:{row[col]}' for col in new_df.columns])
             result.append(row_str)
 
-        print('Generating response...')
-        response2 = client.chat.completions.create(
-            model="gpt-4-turbo-preview",
-            # model="gpt-3.5-turbo",
-            messages=[
-                {"role": "system", "content": "You are a helpful assistant."},
-                {"role": "user", "content": f"Using only this list of strings: {result}, return the answer to this question: {query}. Don't reference yourself."},
-            ],
-            temperature=1,
-            max_tokens=1024,
-            top_p=1,
-            frequency_penalty=0,
-            presence_penalty=0
-        )
-        print(f'ANSWER:\n{'-'*20}\n{response2.choices[0].message.content}\n{'-'*20}')
-        return response2.choices[0].message.content
+        if save_source_data_as_csv:
+            # make tables dir if it doesn't exist
+            if os.path.isdir('tables') == False:
+                os.mkdir('tables')
+            new_df.to_csv(f'query_results.csv', index=False)
 
+        if self.generate_response:
+            print('Generating response...')
+            response2 = client.chat.completions.create(
+                model="gpt-4-turbo-preview",
+                # model="gpt-3.5-turbo",
+                messages=[
+                    {"role": "system", "content": "You are a helpful assistant."},
+                    {"role": "user", "content": f"Using only this list of strings: {result}, return the answer to this question: {query}. Don't reference yourself."},
+                ],
+                temperature=1,
+                max_tokens=1024,
+                top_p=1,
+                frequency_penalty=0,
+                presence_penalty=0
+            )
+            print(f'ANSWER:\n{'-'*20}\n{response2.choices[0].message.content}\n{'-'*20}')
+            return response2.choices[0].message.content
```

### Comparing `tabletalk-0.0.5/tabletalk.egg-info/PKG-INFO` & `tabletalk-0.0.6/tabletalk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.5
+Version: 0.0.6
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

