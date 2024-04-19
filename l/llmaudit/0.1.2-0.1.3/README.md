# Comparing `tmp/llmaudit-0.1.2.tar.gz` & `tmp/llmaudit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmaudit-0.1.2.tar", last modified: Wed Apr 17 06:38:42 2024, max compression
+gzip compressed data, was "llmaudit-0.1.3.tar", last modified: Fri Apr 19 16:19:04 2024, max compression
```

## Comparing `llmaudit-0.1.2.tar` & `llmaudit-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 06:38:42.394041 llmaudit-0.1.2/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.1.2/LICENSE
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 06:38:42.393343 llmaudit-0.1.2/PKG-INFO
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 01:52:44.000000 llmaudit-0.1.2/README.md
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 06:38:42.388675 llmaudit-0.1.2/llmaudit/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.1.2/llmaudit/__init__.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.1.2/llmaudit/cli.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     5537 2024-04-17 06:38:22.000000 llmaudit-0.1.2/llmaudit/report_template.html
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.1.2/llmaudit/scan_github_repos.py
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15615 2024-04-17 01:00:12.000000 llmaudit-0.1.2/llmaudit/sprawl.py
-drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-17 06:38:42.392675 llmaudit-0.1.2/llmaudit.egg-info/
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      681 2024-04-17 06:38:42.000000 llmaudit-0.1.2/llmaudit.egg-info/PKG-INFO
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      342 2024-04-17 06:38:42.000000 llmaudit-0.1.2/llmaudit.egg-info/SOURCES.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-17 06:38:42.000000 llmaudit-0.1.2/llmaudit.egg-info/dependency_links.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-17 06:38:42.000000 llmaudit-0.1.2/llmaudit.egg-info/entry_points.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-17 06:38:42.000000 llmaudit-0.1.2/llmaudit.egg-info/requires.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-17 06:38:42.000000 llmaudit-0.1.2/llmaudit.egg-info/top_level.txt
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)      777 2024-04-17 06:38:37.000000 llmaudit-0.1.2/pyproject.toml
--rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-17 06:38:42.394202 llmaudit-0.1.2/setup.cfg
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-19 16:19:04.514328 llmaudit-0.1.3/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    11356 2024-04-16 23:43:48.000000 llmaudit-0.1.3/LICENSE
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     3409 2024-04-19 16:19:04.513575 llmaudit-0.1.3/PKG-INFO
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2723 2024-04-18 23:57:25.000000 llmaudit-0.1.3/README.md
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-19 16:19:04.506290 llmaudit-0.1.3/llmaudit/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        0 2024-04-16 23:48:32.000000 llmaudit-0.1.3/llmaudit/__init__.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     1662 2024-04-17 00:29:07.000000 llmaudit-0.1.3/llmaudit/cli.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     5539 2024-04-19 16:17:22.000000 llmaudit-0.1.3/llmaudit/report_template.html
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     2823 2024-04-17 00:29:22.000000 llmaudit-0.1.3/llmaudit/scan_github_repos.py
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)    15615 2024-04-17 01:00:12.000000 llmaudit-0.1.3/llmaudit/sprawl.py
+drwxr-xr-x   0 vikramjayanthi   (501) staff       (20)        0 2024-04-19 16:19:04.512623 llmaudit-0.1.3/llmaudit.egg-info/
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)     3409 2024-04-19 16:19:04.000000 llmaudit-0.1.3/llmaudit.egg-info/PKG-INFO
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      342 2024-04-19 16:19:04.000000 llmaudit-0.1.3/llmaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        1 2024-04-19 16:19:04.000000 llmaudit-0.1.3/llmaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       51 2024-04-19 16:19:04.000000 llmaudit-0.1.3/llmaudit.egg-info/entry_points.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       37 2024-04-19 16:19:04.000000 llmaudit-0.1.3/llmaudit.egg-info/requires.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)        9 2024-04-19 16:19:04.000000 llmaudit-0.1.3/llmaudit.egg-info/top_level.txt
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)      781 2024-04-19 16:18:54.000000 llmaudit-0.1.3/pyproject.toml
+-rw-r--r--   0 vikramjayanthi   (501) staff       (20)       38 2024-04-19 16:19:04.514461 llmaudit-0.1.3/setup.cfg
```

### Comparing `llmaudit-0.1.2/LICENSE` & `llmaudit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.2/llmaudit/cli.py` & `llmaudit-0.1.3/llmaudit/cli.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.2/llmaudit/report_template.html` & `llmaudit-0.1.3/llmaudit/report_template.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>PromptArmor Gen AI Usage Report</title>
     <link href="https://fonts.googleapis.com/css?family=Roboto:400,700&display=swap" rel="stylesheet">
-    <link rel="icon" type="image/png" href="http://branding.promptarmor.com/static/logo.png">
+    <link rel="icon" type="image/png" href="https://branding.promptarmor.com/static/logo.png">
     <style>
         body { 
             font-family: 'Roboto', sans-serif; 
             color: #333; 
             background-color: #f4f4f4; 
             margin: 0; 
             padding: 20px;
@@ -86,15 +86,15 @@
             margin-bottom: 5px;
         }
     </style>
 </head>
 <body>
     <div class="header">
         <div style="display: flex; align-items: center; justify-content: center;">
-            <img src="http://branding.promptarmor.com/static/logo.png" alt="PromptArmor Logo" style="float:left; margin-right:10px; height:3em;">
+            <img src="https://branding.promptarmor.com/static/logo.png" alt="PromptArmor Logo" style="float:left; margin-right:10px; height:3em;">
             <h1>PromptArmor Gen AI Usage Report</h1>
         </div>
         <p class="date" id="reportDate"></p>
     </div>
 <div class="statistics">
     <div class="section">
         <h2>Total # Entrypoints</h2>
```

### Comparing `llmaudit-0.1.2/llmaudit/scan_github_repos.py` & `llmaudit-0.1.3/llmaudit/scan_github_repos.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.2/llmaudit/sprawl.py` & `llmaudit-0.1.3/llmaudit/sprawl.py`

 * *Files identical despite different names*

### Comparing `llmaudit-0.1.2/pyproject.toml` & `llmaudit-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmaudit"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="PromptArmor", email="founders@promptarmor.com" },
 ]
 description = "A CLI tool to find LLM usage accross your repos"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -27,9 +27,9 @@
 
 [tool.setuptools.package-data]
 llmaudit = ["*.html", "*.png"]
 
 
 [project.urls]
 "Company Page" = "https://promptarmor.com/"
-Homepage = "https://github.com/pypa/sampleproject"
-Issues = "https://github.com/pypa/sampleproject/issues"
+Homepage = "https://github.com/promptarmor/llmaudit"
+Issues = "https://github.com/promptarmor/llmaudit/issues"
```

