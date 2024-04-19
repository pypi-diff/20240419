# Comparing `tmp/xpath_writer-1.0.tar.gz` & `tmp/xpath_writer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpath_writer-1.0.tar", last modified: Thu Apr 18 05:20:59 2024, max compression
+gzip compressed data, was "xpath_writer-1.0.1.tar", last modified: Fri Apr 19 10:24:58 2024, max compression
```

## Comparing `xpath_writer-1.0.tar` & `xpath_writer-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:20:59.687331 xpath_writer-1.0/
--rw-rw-rw-   0        0        0      880 2024-04-18 05:20:59.685264 xpath_writer-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-18 05:20:59.687331 xpath_writer-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-04-18 05:20:48.000000 xpath_writer-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:20:59.593987 xpath_writer-1.0/xpath_writer/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:32:58.000000 xpath_writer-1.0/xpath_writer/__init__.py
--rw-rw-rw-   0        0        0     5189 2024-04-18 05:18:27.000000 xpath_writer-1.0/xpath_writer/xpath_writer.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:20:59.683202 xpath_writer-1.0/xpath_writer.egg-info/
--rw-rw-rw-   0        0        0      880 2024-04-18 05:20:59.000000 xpath_writer-1.0/xpath_writer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-04-18 05:20:59.000000 xpath_writer-1.0/xpath_writer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:20:59.000000 xpath_writer-1.0/xpath_writer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-18 05:20:59.000000 xpath_writer-1.0/xpath_writer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 05:20:59.000000 xpath_writer-1.0/xpath_writer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:58.121892 xpath_writer-1.0.1/
+-rw-rw-rw-   0        0        0      882 2024-04-19 10:24:58.119852 xpath_writer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2024-04-19 10:21:47.000000 xpath_writer-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:24:58.122933 xpath_writer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-04-19 10:24:06.000000 xpath_writer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:58.085030 xpath_writer-1.0.1/xpath_writer/
+-rw-rw-rw-   0        0        0       45 2024-04-19 10:02:08.000000 xpath_writer-1.0.1/xpath_writer/__init__.py
+-rw-rw-rw-   0        0        0     5358 2024-04-18 11:24:51.000000 xpath_writer-1.0.1/xpath_writer/xpath_writer.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:24:58.118853 xpath_writer-1.0.1/xpath_writer.egg-info/
+-rw-rw-rw-   0        0        0      882 2024-04-19 10:24:57.000000 xpath_writer-1.0.1/xpath_writer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-19 10:24:57.000000 xpath_writer-1.0.1/xpath_writer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:24:57.000000 xpath_writer-1.0.1/xpath_writer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-19 10:24:57.000000 xpath_writer-1.0.1/xpath_writer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 10:24:57.000000 xpath_writer-1.0.1/xpath_writer.egg-info/top_level.txt
```

### Comparing `xpath_writer-1.0/PKG-INFO` & `xpath_writer-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpath_writer
-Version: 1.0
+Version: 1.0.1
 Summary: A Python package for writing relative XPath expressions and make XPath Excel file.
 Home-page: https://github.com/pagidireddy/
 Author: Pagidireddy Prasanth Reddy
 Author-email: tradetrontest@gmail.com
 License: MIT
 Keywords: xpath,xpath generator,xpath writer,xpath parser
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xpath_writer-1.0/setup.py` & `xpath_writer-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="xpath_writer",
     packages=["xpath_writer"],
-    version="1.0",
+    version="1.0.1",
     author="Pagidireddy Prasanth Reddy",
     author_email="tradetrontest@gmail.com",
     description="A Python package for writing relative XPath expressions and make XPath Excel file.",
     long_description="The Xpath package provides functionality to extract XPath expressions of elements on a webpage. It utilizes BeautifulSoup for parsing HTML content for interacting with web elements in a browser environment. It utilizes pandas for writing data to Excel file.",
     url="https://github.com/pagidireddy/",
     keywords=['xpath', 'xpath generator', 'xpath writer', 'xpath parser'],
     install_requires=['requests', 'beautifulsoup4', 'pandas', 'openpyxl'],
```

### Comparing `xpath_writer-1.0/xpath_writer/xpath_writer.py` & `xpath_writer-1.0.1/xpath_writer/xpath_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 
 
 def make_excel(data, filename):
     """
@@ -65,25 +64,25 @@
         xpath_list = []
         no_duplicates = []
         for tag in tags:
             temp = {}
             if tag.text not in no_duplicates:
                 if tag.name == 'a' and tag.text:
                     xp = "//" + f'{tag.name}' + '[normalize-space()=' + f'"{tag.text}"' + ']'
-                    temp['Name'] = f'link_'+tag.text
+                    temp['Name'] = f'link_'+tag.text[:15]
                     temp['XPATH'] = xp
                     xpath_list.append(temp)
                     no_duplicates.append(tag.text)
 
                 elif tag.name == 'span' and tag.text:
                     class_value = tag.get('class')
                     if class_value:
                         class_value = ' '.join(class_value)
                         xp = f"//{tag.name}[@class='{class_value}' and contains(text(), '{tag.text}')]"
-                        temp['Name'] = 'span_'+tag.text
+                        temp['Name'] = 'span_'+tag.text[:15]
                         temp['XPATH'] = xp
                         xpath_list.append(temp)
                         no_duplicates.append(tag.text)
 
                 elif tag.name == 'input':
                     xpath = '//'
                     xpath += tag.name + "["
@@ -98,15 +97,15 @@
                         temp['Name'] = "Input" + f"{tag['name']}"
                     temp['XPATH'] = xpath
                     xpath_list.append(temp)
                     no_duplicates.append(tag.text)
 
                 elif tag.name == 'button' and len(tag.text) != 0:
                     xp = "//" + f"{tag.name}" + '[.=' + f"'{tag.text}']"
-                    temp['Name'] = 'button_'+tag.text
+                    temp['Name'] = 'button_'+tag.text[:15]
                     temp['XPATH'] = xp
                     xpath_list.append(temp)
                     no_duplicates.append(tag.text)
 
             else:
                 continue
         return xpath_list
@@ -125,26 +124,29 @@
         xpath_list = []
         no_duplicates = []
         for tag in tags:
             temp = {}
             if tag.text not in no_duplicates:
                 if tag.name == tag_name and tag.text:
                     try:
-                        xp = "//" + f'{tag.name}' + '[normalize-space()=' + f'"{tag.text}"' + ']'
-                        temp['Name'] = f'{tag.name}_'+tag.text
-                        temp['XPATH'] = xp
-                        xpath_list.append(temp)
-                        no_duplicates.append(tag.text)
-                    except:
                         xp = f'//{tag.name}'
                         if tag.attrs:
                             xp += '['
                             for attr, value in tag.attrs.items():
                                 if attr == 'class':
                                     value = ' '.join(value)
                                 xp += f"@{attr}='{value}' and "
                             xp = xp[:-5] + ']'
-                        temp['Name'] = f'{tag.name}_'+tag.text
+                        try:
+                            temp['Name'] = "Input_" + f"{tag['placeholder']}"
+                        except:
+                            temp['Name'] = "Input" + f"{tag['name']}"
+                        temp['XPATH'] = xp
+                        xpath_list.append(temp)
+                        no_duplicates.append(tag.text)
+                    except:
+                        xp = "//" + f'{tag.name}' + '[normalize-space()=' + f'"{tag.text}"' + ']'
+                        temp['Name'] = f'{tag.name}_' + tag.text[:15]
                         temp['XPATH'] = xp
                         xpath_list.append(temp)
                         no_duplicates.append(tag.text)
         return xpath_list
```

### Comparing `xpath_writer-1.0/xpath_writer.egg-info/PKG-INFO` & `xpath_writer-1.0.1/xpath_writer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpath_writer
-Version: 1.0
+Version: 1.0.1
 Summary: A Python package for writing relative XPath expressions and make XPath Excel file.
 Home-page: https://github.com/pagidireddy/
 Author: Pagidireddy Prasanth Reddy
 Author-email: tradetrontest@gmail.com
 License: MIT
 Keywords: xpath,xpath generator,xpath writer,xpath parser
 Classifier: Programming Language :: Python :: 3
```

