# Comparing `tmp/open_parser-0.0.5.tar.gz` & `tmp/open_parser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_parser-0.0.5.tar", max compression
+gzip compressed data, was "open_parser-0.0.6.tar", max compression
```

## Comparing `open_parser-0.0.5.tar` & `open_parser-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1419 2024-04-06 00:51:24.943032 open_parser-0.0.5/README.md
--rw-r--r--   0        0        0       89 2024-04-11 07:19:40.277002 open_parser-0.0.5/open_parser/__init__.py
--rw-r--r--   0        0        0     3498 2024-04-11 07:19:40.277427 open_parser-0.0.5/open_parser/base.py
--rw-r--r--   0        0        0      394 2024-04-11 07:19:40.277903 open_parser-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 open_parser-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1886 2024-04-19 08:19:17.616734 open_parser-0.0.6/README.md
+-rw-r--r--   0        0        0       89 2024-04-19 08:21:13.633818 open_parser-0.0.6/open_parser/__init__.py
+-rw-r--r--   0        0        0     3494 2024-04-19 08:19:17.625678 open_parser-0.0.6/open_parser/base.py
+-rw-r--r--   0        0        0      394 2024-04-19 08:21:13.634455 open_parser-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2548 1970-01-01 00:00:00.000000 open_parser-0.0.6/PKG-INFO
```

### Comparing `open_parser-0.0.5/README.md` & `open_parser-0.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,25 @@
 
 ```
 conda create -n openparse python=3.10 -y
 conda activate openparse
 pip3 install open_parser
 ```
 
+## :bashfile usage
+To use OpenParse via `curl` requests, you can run the following bash command from the root folder of this repository:
+```
+bash parse.sh <your apiKey> <file path> <prompt for parse (optional, default="")>
+```
+
+For example, to extract a table from a PDF file, you can run the following command:
+```
+bash parse.sh gl**************************************  /path/to/your/file.pdf "Return the table in a JSON format with each box's key and value."
+```
+
 ## :scroll:  Examples
 
 OpenParse can extract text, numbers and symbols from PDF, images, etc. Check out each notebook below to run OpenParse within 10 lines of code!
 
 ### [Prompt to Extract Key-values into JSON from W2 (PDF)](https://github.com/CambioML/open-parser/blob/main/examples/prompt_to_extract_table_from_pdf_to_json.ipynb)
 Do you want to extract key-values from a W2 PDF into JSON format? Check out this notebook (3-min read)!
```

### Comparing `open_parser-0.0.5/open_parser/base.py` & `open_parser-0.0.6/open_parser/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
     def setAPIKey(self, apiKey):
         self._request_header = {"x-api-key": apiKey}
 
     def extract(self, file_path):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path)
         result = self._request_file_extraction(user_id, job_id, s3_key)
-        return result["file_content"]
+        return json.loads(result)["result"]["file_content"]
 
     def parse(self, file_path, prompt, mode="advanced"):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path)
         result = self._request_info_extraction(user_id, job_id, s3_key, mode, prompt)
-        return result
+        return json.loads(result)["result"]
 
     def _error_handler(self, response):
         if response.status_code == 403:
             raise Exception("Invalid API Key")
         elif response.status_code == 429:
             raise Exception("API Key limit exceeded")
         else:
@@ -69,15 +69,15 @@
         }
         response = requests.post(
             self._extracturl, headers=self._request_header, json=payload
         )
 
         if response.status_code == 200:
             print("Extraction success.")
-            return json.loads(response.json()["result"])
+            return response.text
 
         self._error_handler(response)
 
     def _request_info_extraction(self, user_id, job_id, s3_key, mode, prompt=""):
         if mode not in ["advanced", "basic"]:
             raise ValueError("Invalid mode. Choose either 'advanced' or 'basic'.")
         payload = {
@@ -89,10 +89,10 @@
         }
         response = requests.post(
             self._parseurl, headers=self._request_header, json=payload
         )
 
         if response.status_code == 200:
             print("Extraction success.")
-            return json.loads(response.json()["result"])
+            return response.text
 
         self._error_handler(response)
```

### Comparing `open_parser-0.0.5/PKG-INFO` & `open_parser-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-parser
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open parser for all.
 Author: CambioML
 Author-email: wanwanaiai45@gmail.com
 Maintainer: Rachel Hu
 Maintainer-email: goldpiggy@berkeley.edu
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
@@ -38,14 +38,25 @@
 
 ```
 conda create -n openparse python=3.10 -y
 conda activate openparse
 pip3 install open_parser
 ```
 
+## :bashfile usage
+To use OpenParse via `curl` requests, you can run the following bash command from the root folder of this repository:
+```
+bash parse.sh <your apiKey> <file path> <prompt for parse (optional, default="")>
+```
+
+For example, to extract a table from a PDF file, you can run the following command:
+```
+bash parse.sh gl**************************************  /path/to/your/file.pdf "Return the table in a JSON format with each box's key and value."
+```
+
 ## :scroll:  Examples
 
 OpenParse can extract text, numbers and symbols from PDF, images, etc. Check out each notebook below to run OpenParse within 10 lines of code!
 
 ### [Prompt to Extract Key-values into JSON from W2 (PDF)](https://github.com/CambioML/open-parser/blob/main/examples/prompt_to_extract_table_from_pdf_to_json.ipynb)
 Do you want to extract key-values from a W2 PDF into JSON format? Check out this notebook (3-min read)!
```

