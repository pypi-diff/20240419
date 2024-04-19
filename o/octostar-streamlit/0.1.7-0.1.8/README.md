# Comparing `tmp/octostar_streamlit-0.1.7.tar.gz` & `tmp/octostar_streamlit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octostar_streamlit-0.1.7.tar", max compression
+gzip compressed data, was "octostar_streamlit-0.1.8.tar", max compression
```

## Comparing `octostar_streamlit-0.1.7.tar` & `octostar_streamlit-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1073 2024-04-03 17:04:55.018503 octostar_streamlit-0.1.7/LICENSE
--rw-r--r--   0        0        0      324 2024-04-03 17:04:55.018503 octostar_streamlit-0.1.7/README.md
--rw-r--r--   0        0        0     1965 2024-04-03 17:04:55.018503 octostar_streamlit-0.1.7/octostar_streamlit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 17:04:55.018503 octostar_streamlit-0.1.7/octostar_streamlit/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 17:04:55.018503 octostar_streamlit-0.1.7/octostar_streamlit/core/desktop/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-03 17:04:55.018503 octostar_streamlit-0.1.7/octostar_streamlit/core/desktop/method_call.py
--rw-r--r--   0        0        0     7821 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/desktop/params.py
--rw-r--r--   0        0        0     6134 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/entities.py
--rw-r--r--   0        0        0      281 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/method_call.py
--rw-r--r--   0        0        0        0 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/ontology/__init__.py
--rw-r--r--   0        0        0      673 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/ontology/method_call.py
--rw-r--r--   0        0        0     1766 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/ontology/params.py
--rw-r--r--   0        0        0      222 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/params_base_model.py
--rw-r--r--   0        0        0      867 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/core/streamlit_executor.py
--rw-r--r--   0        0        0    10049 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/desktop.py
--rw-r--r--   0        0        0      253 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/.gitignore
--rw-r--r--   0        0        0   235160 2024-04-03 17:05:16.549931 octostar_streamlit-0.1.7/octostar_streamlit/frontend/dist/assets/index-BCMUK_M-.js
--rw-r--r--   0        0        0      383 2024-04-03 17:05:16.549931 octostar_streamlit-0.1.7/octostar_streamlit/frontend/dist/index.html
--rw-r--r--   0        0        0     1497 2024-04-03 17:05:16.381935 octostar_streamlit-0.1.7/octostar_streamlit/frontend/dist/vite.svg
--rw-r--r--   0        0        0      356 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/index.html
--rw-r--r--   0        0        0    42450 2024-04-03 17:05:12.854011 octostar_streamlit-0.1.7/octostar_streamlit/frontend/package-lock.json
--rw-r--r--   0        0        0      413 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/package.json
--rw-r--r--   0        0        0     1497 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/public/vite.svg
--rw-r--r--   0        0        0      835 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/core.ts
--rw-r--r--   0        0        0    14114 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/desktop.ts
--rw-r--r--   0        0        0     2373 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/main.ts
--rw-r--r--   0        0        0     4166 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/ontology.ts
--rw-r--r--   0        0        0       38 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      527 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/tsconfig.json
--rw-r--r--   0        0        0       86 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/frontend/vite.config.ts
--rw-r--r--   0        0        0     3984 2024-04-03 17:04:55.022503 octostar_streamlit-0.1.7/octostar_streamlit/ontology.py
--rw-r--r--   0        0        0      736 2024-04-03 17:04:55.026503 octostar_streamlit-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/LICENSE
+-rw-r--r--   0        0        0      324 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/README.md
+-rw-r--r--   0        0        0     1965 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/octostar_streamlit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/octostar_streamlit/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/octostar_streamlit/core/desktop/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/octostar_streamlit/core/desktop/method_call.py
+-rw-r--r--   0        0        0     7821 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/octostar_streamlit/core/desktop/params.py
+-rw-r--r--   0        0        0     6134 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/octostar_streamlit/core/entities.py
+-rw-r--r--   0        0        0      281 2024-04-19 07:32:01.555224 octostar_streamlit-0.1.8/octostar_streamlit/core/method_call.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/core/ontology/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/core/ontology/method_call.py
+-rw-r--r--   0        0        0     1766 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/core/ontology/params.py
+-rw-r--r--   0        0        0      222 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/core/params_base_model.py
+-rw-r--r--   0        0        0      867 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/core/streamlit_executor.py
+-rw-r--r--   0        0        0    10075 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/desktop.py
+-rw-r--r--   0        0        0      253 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/.gitignore
+-rw-r--r--   0        0        0   235160 2024-04-19 07:32:28.275616 octostar_streamlit-0.1.8/octostar_streamlit/frontend/dist/assets/index-BCMUK_M-.js
+-rw-r--r--   0        0        0      383 2024-04-19 07:32:28.279616 octostar_streamlit-0.1.8/octostar_streamlit/frontend/dist/index.html
+-rw-r--r--   0        0        0     1497 2024-04-19 07:32:28.019612 octostar_streamlit-0.1.8/octostar_streamlit/frontend/dist/vite.svg
+-rw-r--r--   0        0        0      356 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/index.html
+-rw-r--r--   0        0        0    42450 2024-04-19 07:32:24.095558 octostar_streamlit-0.1.8/octostar_streamlit/frontend/package-lock.json
+-rw-r--r--   0        0        0      413 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/package.json
+-rw-r--r--   0        0        0     1497 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/public/vite.svg
+-rw-r--r--   0        0        0      835 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/core.ts
+-rw-r--r--   0        0        0    14114 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/desktop.ts
+-rw-r--r--   0        0        0     2373 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/main.ts
+-rw-r--r--   0        0        0     4166 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/ontology.ts
+-rw-r--r--   0        0        0       38 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      527 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/tsconfig.json
+-rw-r--r--   0        0        0       86 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/frontend/vite.config.ts
+-rw-r--r--   0        0        0     3984 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/octostar_streamlit/ontology.py
+-rw-r--r--   0        0        0      736 2024-04-19 07:32:01.559224 octostar_streamlit-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 octostar_streamlit-0.1.8/PKG-INFO
```

### Comparing `octostar_streamlit-0.1.7/LICENSE` & `octostar_streamlit-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/__init__.py` & `octostar_streamlit-0.1.8/octostar_streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/core/desktop/method_call.py` & `octostar_streamlit-0.1.8/octostar_streamlit/core/desktop/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/core/desktop/params.py` & `octostar_streamlit-0.1.8/octostar_streamlit/core/desktop/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/core/entities.py` & `octostar_streamlit-0.1.8/octostar_streamlit/core/entities.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/core/ontology/method_call.py` & `octostar_streamlit-0.1.8/octostar_streamlit/core/ontology/method_call.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/core/ontology/params.py` & `octostar_streamlit-0.1.8/octostar_streamlit/core/ontology/params.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/core/streamlit_executor.py` & `octostar_streamlit-0.1.8/octostar_streamlit/core/streamlit_executor.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/desktop.py` & `octostar_streamlit-0.1.8/octostar_streamlit/desktop.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 
 def delete(params: DeleteParams, key=None) -> None:
     return call_desktop_api_method("delete", params, key)
 
 
 def searchXperience(params: SearchXperienceParams, key=None) -> List[Entity]:
     result = call_desktop_api_method("searchXperience", params, key)
-    return [Entity(**v) for v in result]
+    return result if not result else [Entity(**v) for v in result]
 
 
 def show_tab(params: ShowTabParams, key=None) -> None:
     return call_desktop_api_method("showTab", params, key)
 
 
 def close_tab(params: CloseTabParams, key=None) -> None:
```

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/dist/assets/index-BCMUK_M-.js` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/dist/assets/index-BCMUK_M-.js`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/dist/vite.svg` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/package-lock.json` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/public/vite.svg` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/core.ts` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/core.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/desktop.ts` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/desktop.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/main.ts` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/main.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/src/ontology.ts` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/src/ontology.ts`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/frontend/tsconfig.json` & `octostar_streamlit-0.1.8/octostar_streamlit/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit-0.1.7/octostar_streamlit/ontology.py` & `octostar_streamlit-0.1.8/octostar_streamlit/ontology.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,9 +116,9 @@
     result = call_ontology_api_method("getSysInheritance", None, key)
     return [Inheritance(**inheritance) for inheritance in result]
 
 
 # TODO: implement subscribe
 
 
-def consustent_uuid(params: ConsistentUUIDParams, key=None) -> str:
+def consistent_uuid(params: ConsistentUUIDParams, key=None) -> str:
     return call_ontology_api_method("consistentUUID", params, key)
```

### Comparing `octostar_streamlit-0.1.7/pyproject.toml` & `octostar_streamlit-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octostar-streamlit"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 license = "MIT"
 authors = ["Oleksandr Korzhov <another.fullstack.dev@gmail.com>"]
 readme = "README.md"
 include = [
     "octostar_streamlit/frontend/dist/**/*",
 ]
```

### Comparing `octostar_streamlit-0.1.7/PKG-INFO` & `octostar_streamlit-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octostar-streamlit
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 License: MIT
 Author: Oleksandr Korzhov
 Author-email: another.fullstack.dev@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

