# Comparing `tmp/valphi-0.5.1.tar.gz` & `tmp/valphi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valphi-0.5.1.tar", max compression
+gzip compressed data, was "valphi-0.6.0.tar", max compression
```

## Comparing `valphi-0.5.1.tar` & `valphi-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.5.1/LICENSE
--rw-r--r--   0        0        0      425 2024-01-28 19:40:16.657587 valphi-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.5.1/valphi/__init__.py
--rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.5.1/valphi/__main__.py
--rw-r--r--   0        0        0    11109 2023-11-11 17:16:04.022107 valphi-0.5.1/valphi/cli.py
--rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.5.1/valphi/contexts.py
--rw-r--r--   0        0        0    17358 2023-11-11 15:24:19.677155 valphi-0.5.1/valphi/controllers.py
--rw-r--r--   0        0        0     1906 2023-11-11 14:25:21.765707 valphi-0.5.1/valphi/models.py
--rw-r--r--   0        0        0    17594 2024-01-25 17:09:34.655202 valphi-0.5.1/valphi/networks.py
--rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.5.1/valphi/propagators.py
--rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.5.1/valphi/utils.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 valphi-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.6.0/LICENSE
+-rw-r--r--   0        0        0      425 2024-04-19 21:55:41.442445 valphi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.6.0/valphi/__init__.py
+-rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.6.0/valphi/__main__.py
+-rw-r--r--   0        0        0    11179 2024-04-19 21:56:18.154759 valphi-0.6.0/valphi/cli.py
+-rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.6.0/valphi/contexts.py
+-rw-r--r--   0        0        0    17358 2023-11-11 15:24:19.677155 valphi-0.6.0/valphi/controllers.py
+-rw-r--r--   0        0        0     1906 2023-11-11 14:25:21.765707 valphi-0.6.0/valphi/models.py
+-rw-r--r--   0        0        0    17594 2024-01-25 17:09:34.655202 valphi-0.6.0/valphi/networks.py
+-rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.6.0/valphi/propagators.py
+-rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.6.0/valphi/utils.py
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 valphi-0.6.0/PKG-INFO
```

### Comparing `valphi-0.5.1/LICENSE` & `valphi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valphi-0.5.1/valphi/cli.py` & `valphi-0.6.0/valphi/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import dataclasses
 import webbrowser
 from enum import Enum
 from pathlib import Path
 from typing import List, Optional, Dict
 
 import typer
+from dumbo_asp.queries import pack_asp_chef_url
 from dumbo_utils.console import console
-from dumbo_utils.url import compress_object_for_url
 from dumbo_utils.validation import validate
 from rich.table import Table
 
 from valphi.controllers import Controller
 from valphi.networks import NetworkTopology, ArgumentationGraph, MaxSAT, NetworkInterface
 
 
@@ -182,24 +182,29 @@
     with console.status("Running..."):
         res = app_options.controller.find_solutions(number_of_solutions)
     if not res:
         console.print('NO SOLUTIONS')
     for index, values in enumerate(res, start=1):
         console.print(network_values_to_table(values, title=f"Solution {index}"))
     if show_in_asp_chef:
-        url = "https://asp-chef.alviano.net/open#"
-        # url = "http://localhost:5188/open#"
+        url = "https://asp-chef.alviano.net/"
+        # url = "http://localhost:5188/"
+        url += "#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%21"
         graph = app_options.controller.network.as_attack_graph().as_facts
         models = []
         for values in res:
+            models.append(f"max_value({app_options.controller.max_value}).")
             models.append(graph)
-            models.append('\n'.join(f"eval({node if type(node) is str else 'l' + '_'.join(str(x) for x in node)},{','.join(value.split('/'))})." for node, value in values.items()))
+            models.append('\n'.join(
+                f"eval({node if type(node) is str else 'l' + '_'.join(str(x) for x in node)},"
+                f"anonymous,{value.split('/')[0]})."
+                for node, value in values.items()
+            ))
             models.append('§')
-        url += compress_object_for_url({"input": '\n'.join(models[:-1])}, suffix="")
-        url += ";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%21"
+        url = pack_asp_chef_url(url, the_input='\n'.join(models[:-1]))
         webbrowser.open(url, new=0, autoraise=True)
 
 
 @app.command(name="query")
 def command_query(
         query: Optional[str] = typer.Argument(
             None,
```

### Comparing `valphi-0.5.1/valphi/contexts.py` & `valphi-0.6.0/valphi/contexts.py`

 * *Files identical despite different names*

### Comparing `valphi-0.5.1/valphi/controllers.py` & `valphi-0.6.0/valphi/controllers.py`

 * *Files identical despite different names*

### Comparing `valphi-0.5.1/valphi/models.py` & `valphi-0.6.0/valphi/models.py`

 * *Files identical despite different names*

### Comparing `valphi-0.5.1/valphi/networks.py` & `valphi-0.6.0/valphi/networks.py`

 * *Files identical despite different names*

### Comparing `valphi-0.5.1/valphi/propagators.py` & `valphi-0.6.0/valphi/propagators.py`

 * *Files identical despite different names*

