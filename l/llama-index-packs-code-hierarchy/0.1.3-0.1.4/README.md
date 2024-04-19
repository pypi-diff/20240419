# Comparing `tmp/llama_index_packs_code_hierarchy-0.1.3.tar.gz` & `tmp/llama_index_packs_code_hierarchy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_code_hierarchy-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_packs_code_hierarchy-0.1.4.tar", max compression
```

## Comparing `llama_index_packs_code_hierarchy-0.1.3.tar` & `llama_index_packs_code_hierarchy-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4966 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/README.md
--rw-r--r--   0        0        0       17 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/BUILD
--rw-r--r--   0        0        0      371 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/base.py
--rw-r--r--   0        0        0    33488 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/code_hierarchy.py
--rw-r--r--   0        0        0     6099 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/query_engine.py
--rw-r--r--   0        0        0     1438 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 llama_index_packs_code_hierarchy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4966 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/README.md
+-rw-r--r--   0        0        0       17 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/BUILD
+-rw-r--r--   0        0        0      371 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/base.py
+-rw-r--r--   0        0        0    33737 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/code_hierarchy.py
+-rw-r--r--   0        0        0     6099 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/query_engine.py
+-rw-r--r--   0        0        0     1438 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 llama_index_packs_code_hierarchy-0.1.4/PKG-INFO
```

### Comparing `llama_index_packs_code_hierarchy-0.1.3/README.md` & `llama_index_packs_code_hierarchy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/base.py` & `llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/code_hierarchy.py` & `llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/code_hierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -825,15 +825,23 @@
         if child_node.text not in parent_node.text:
             raise ValueError("The child text is not contained inside the parent text.")
         if child_node.node_id not in (c.node_id for c in parent_node.child_nodes or []):
             raise ValueError("The child node is not a child of the parent node.")
 
         # Now do the replacement
         replacement_text = cls._get_replacement_text(child_node=child_node)
-        parent_node.text = parent_node.text.replace(child_node.text, replacement_text)
+
+        index = parent_node.text.find(child_node.text)
+        # If the text is found, replace only the first occurrence
+        if index != -1:
+            parent_node.text = (
+                parent_node.text[:index]
+                + replacement_text
+                + parent_node.text[index + len(child_node.text) :]
+            )
 
     @classmethod
     def _skeletonize_list(cls, nodes: List[TextNode]) -> None:
         # Create a convenient map for mapping node id's to nodes
         node_id_map = {n.node_id: n for n in nodes}
 
         def recur(node: TextNode) -> None:
```

### Comparing `llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/query_engine.py` & `llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.3/pyproject.toml` & `llama_index_packs_code_hierarchy-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Ryan Peach <rgpeach10@gmail.com>"]
 description = "A node parser which can create a hierarchy of all code scopes in a directory."
 keywords = ["c", "code", "cpp", "hierarchy", "html", "javascript", "python", "repo", "typescript"]
 license = "MIT"
 maintainers = ["ryanpeach"]
 name = "llama-index-packs-code-hierarchy"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 llama-index-core = "^0.10.1"
 tree-sitter-languages = "^1.8.0"
 tree-sitter = "^0.20.2"
 llama-index-agent-openai = ">=0.1.5"
```

### Comparing `llama_index_packs_code_hierarchy-0.1.3/PKG-INFO` & `llama_index_packs_code_hierarchy-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-code-hierarchy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A node parser which can create a hierarchy of all code scopes in a directory.
 License: MIT
 Keywords: c,code,cpp,hierarchy,html,javascript,python,repo,typescript
 Author: Ryan Peach
 Author-email: rgpeach10@gmail.com
 Maintainer: ryanpeach
 Requires-Python: >=3.8.1,<3.12
```

