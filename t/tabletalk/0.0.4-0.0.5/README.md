# Comparing `tmp/tabletalk-0.0.4.tar.gz` & `tmp/tabletalk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabletalk-0.0.4.tar", last modified: Fri Apr 19 18:05:16 2024, max compression
+gzip compressed data, was "tabletalk-0.0.5.tar", last modified: Fri Apr 19 18:19:38 2024, max compression
```

## Comparing `tabletalk-0.0.4.tar` & `tabletalk-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:05:16.713113 tabletalk-0.0.4/
--rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.4/LICENSE
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 18:05:16.712898 tabletalk-0.0.4/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.4/README.md
--rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 18:05:16.713166 tabletalk-0.0.4/setup.cfg
--rw-r--r--   0 vinceberry   (501) staff       (20)     1154 2024-04-19 18:04:45.000000 tabletalk-0.0.4/setup.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:05:16.711880 tabletalk-0.0.4/tabletalk/
--rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.4/tabletalk/__init__.py
--rw-r--r--   0 vinceberry   (501) staff       (20)     2914 2024-04-19 17:59:24.000000 tabletalk-0.0.4/tabletalk/talk.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:05:16.712696 tabletalk-0.0.4/tabletalk.egg-info/
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 18:05:16.000000 tabletalk-0.0.4/tabletalk.egg-info/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 18:05:16.000000 tabletalk-0.0.4/tabletalk.egg-info/SOURCES.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 18:05:16.000000 tabletalk-0.0.4/tabletalk.egg-info/dependency_links.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 18:05:16.000000 tabletalk-0.0.4/tabletalk.egg-info/requires.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 18:05:16.000000 tabletalk-0.0.4/tabletalk.egg-info/top_level.txt
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:19:38.981783 tabletalk-0.0.5/
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.5/LICENSE
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 18:19:38.981542 tabletalk-0.0.5/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.5/README.md
+-rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 18:19:38.981827 tabletalk-0.0.5/setup.cfg
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1154 2024-04-19 18:19:29.000000 tabletalk-0.0.5/setup.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:19:38.980506 tabletalk-0.0.5/tabletalk/
+-rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.5/tabletalk/__init__.py
+-rw-r--r--   0 vinceberry   (501) staff       (20)     2914 2024-04-19 18:19:11.000000 tabletalk-0.0.5/tabletalk/talk.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 18:19:38.981316 tabletalk-0.0.5/tabletalk.egg-info/
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/requires.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 18:19:38.000000 tabletalk-0.0.5/tabletalk.egg-info/top_level.txt
```

### Comparing `tabletalk-0.0.4/LICENSE` & `tabletalk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tabletalk-0.0.4/PKG-INFO` & `tabletalk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.4
+Version: 0.0.5
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tabletalk-0.0.4/setup.py` & `tabletalk-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'NL2SQL2RAG'
 LONG_DESCRIPTION = 'TableTalk allows you ask query your tabular data with natural language, then produces a generated response.'
 
 setup(
     name="tabletalk",
     version=VERSION,
     author="Vince Berry",
```

### Comparing `tabletalk-0.0.4/tabletalk/talk.py` & `tabletalk-0.0.5/tabletalk/talk.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         query = str(query).strip()
         table_name = str(table_name).strip()
         engine = create_engine("sqlite:///:memory:")
         df = pd.read_csv(self.csv_path)
         columns = df.columns
         df.to_sql(table_name, engine, if_exists='replace', index=False)
         client = OpenAI(api_key=self.openai_api_key)
-        print('Generating response...')
         response = client.chat.completions.create(
             model="gpt-4-turbo-preview",
             # model="gpt-3.5-turbo",
             messages=[
                 {"role": "system", "content": "You are a helpful assistant."},
                 {"role": "user", "content": f"Using only these columns: {columns}, return the SQL query that will answer this question: {query}. This is a SQLite Database, so it's important to consider what it's limitations are. The table is called {table_name}. Err on the side of returning more information by using lowercase comparisons that are similar but not exact. The response should look like this: SELECT * FROM table_name WHERE column_name LIKE '%company name%'. Don't return the exact answer, but rather the SQL query that will return the answer. Don't return anything but the SQL query. Don't include '```sql' or '```' in the response."},
             ],
@@ -42,14 +41,15 @@
         sql_parse = response.choices[0].message.content.replace("'''sql",'').replace("'''",'').strip()
         new_df = pd.read_sql(sql_parse, engine)
         result = []
         for _, row in new_df.iterrows():
             row_str = ','.join([f'{col}:{row[col]}' for col in new_df.columns])
             result.append(row_str)
 
+        print('Generating response...')
         response2 = client.chat.completions.create(
             model="gpt-4-turbo-preview",
             # model="gpt-3.5-turbo",
             messages=[
                 {"role": "system", "content": "You are a helpful assistant."},
                 {"role": "user", "content": f"Using only this list of strings: {result}, return the answer to this question: {query}. Don't reference yourself."},
             ],
```

### Comparing `tabletalk-0.0.4/tabletalk.egg-info/PKG-INFO` & `tabletalk-0.0.5/tabletalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.4
+Version: 0.0.5
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

