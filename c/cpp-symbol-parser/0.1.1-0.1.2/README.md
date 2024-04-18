# Comparing `tmp/cpp_symbol_parser-0.1.1.tar.gz` & `tmp/cpp_symbol_parser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpp_symbol_parser-0.1.1.tar", last modified: Sun Mar 31 01:02:51 2024, max compression
+gzip compressed data, was "cpp_symbol_parser-0.1.2.tar", last modified: Thu Apr 18 23:21:41 2024, max compression
```

## Comparing `cpp_symbol_parser-0.1.1.tar` & `cpp_symbol_parser-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      204 2024-03-27 23:04:37.517530 cpp_symbol_parser-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-26 21:48:25.255337 cpp_symbol_parser-0.1.1/cpp_symbol_parser/__init__.py
--rw-r--r--   0        0        0     1894 2024-03-31 00:33:06.233168 cpp_symbol_parser-0.1.1/cpp_symbol_parser/ast.py
--rw-r--r--   0        0        0     2533 2024-03-27 00:49:58.554476 cpp_symbol_parser-0.1.1/cpp_symbol_parser/grammar.lark
--rw-r--r--   0        0        0      562 2024-03-27 23:10:26.672363 cpp_symbol_parser-0.1.1/cpp_symbol_parser/parser.py
--rw-r--r--   0        0        0     3805 2024-03-31 00:37:02.894559 cpp_symbol_parser-0.1.1/cpp_symbol_parser/transform.py
--rw-r--r--   0        0        0      460 2024-03-31 01:02:51.462888 cpp_symbol_parser-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 cpp_symbol_parser-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      204 2024-03-27 23:04:37.517530 cpp_symbol_parser-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 21:48:25.255337 cpp_symbol_parser-0.1.2/cpp_symbol_parser/__init__.py
+-rw-r--r--   0        0        0     1894 2024-03-31 00:33:06.233168 cpp_symbol_parser-0.1.2/cpp_symbol_parser/ast.py
+-rw-r--r--   0        0        0     2533 2024-03-27 00:49:58.554476 cpp_symbol_parser-0.1.2/cpp_symbol_parser/grammar.lark
+-rw-r--r--   0        0        0      562 2024-04-17 22:46:46.800906 cpp_symbol_parser-0.1.2/cpp_symbol_parser/parser.py
+-rw-r--r--   0        0        0     4146 2024-04-18 23:19:40.854393 cpp_symbol_parser-0.1.2/cpp_symbol_parser/transform.py
+-rw-r--r--   0        0        0      460 2024-04-18 23:21:41.787100 cpp_symbol_parser-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 cpp_symbol_parser-0.1.2/PKG-INFO
```

### Comparing `cpp_symbol_parser-0.1.1/cpp_symbol_parser/ast.py` & `cpp_symbol_parser-0.1.2/cpp_symbol_parser/ast.py`

 * *Files identical despite different names*

### Comparing `cpp_symbol_parser-0.1.1/cpp_symbol_parser/grammar.lark` & `cpp_symbol_parser-0.1.2/cpp_symbol_parser/grammar.lark`

 * *Files identical despite different names*

### Comparing `cpp_symbol_parser-0.1.1/cpp_symbol_parser/parser.py` & `cpp_symbol_parser-0.1.2/cpp_symbol_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cpp_symbol_parser-0.1.1/cpp_symbol_parser/transform.py` & `cpp_symbol_parser-0.1.2/cpp_symbol_parser/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,32 @@
             case None:
                 return self._substitutions[0]
             case Token(type='SEQ_ID'):
                 return self._substitutions[1 + int(id, 36)]
             case _:
                 assert False # TODO
 
+    def _is_template(self, tree):
+        if not isinstance(tree, Tree):
+            return False
+        if tree.data == 'template':
+            return True
+        return any(self._is_template(child) for child in tree.children)
+
     def _substitutable(self, tree):
         match tree.children[0].data:
             case 'builtin_type':
                 pass
 
             case 'substitution':
                 tree.children = self._get_substitution(tree.children[0].children[0])
 
+            case 'class_enum_type' if not self._is_template(tree):
+                self.visit_children(tree)
+
             case _:
                 self.visit_children(tree)
                 self._substitutions.append(tree.children)
 
     template_prefix = _substitutable
     prefix = _substitutable
     unscoped_template_name = _substitutable
```

