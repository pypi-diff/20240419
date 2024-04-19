# Comparing `tmp/flake8_pyi-24.4.0.tar.gz` & `tmp/flake8_pyi-24.4.1.tar.gz`

## Comparing `flake8_pyi-24.4.0.tar` & `flake8_pyi-24.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.editorconfig
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.flake8
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20399 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/ERRORCODES.md
--rw-r--r--   0        0        0    92123 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/pyi.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/scripts/typeshed_primer_download_errors.js
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/scripts/typeshed_primer_post_comment.js
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/check.yml
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/typeshed_primer.yml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.github/workflows/typeshed_primer_comment.yml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/F822.pyi
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/aliases.pyi
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/attribute_annotations.pyi
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/calls.pyi
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/classdefs.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/comparisons.pyi
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/defaults.pyi
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/del.pyi
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/disabled_by_default.pyi
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/emptyclasses.pyi
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/emptyfunctions.pyi
--rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/exit_methods.pyi
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/forward_refs.pyi
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/forward_refs_annassign.pyi
--rw-r--r--   0        0        0    15235 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/imports.pyi
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/incomplete.pyi
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/literals.pyi
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/names_requiring_values.pyi
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/never_vs_noreturn.pyi
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep570.pyi
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep604_union_types.pyi
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep646_py311.pyi
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/pep695_py312.pyi
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/quotes.pyi
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/single_element_tuples.pyi
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/sysplatform.pyi
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/sysversioninfo.pyi
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/test_pyi_files.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/type_comments.pyi
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/typevar.pyi
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/union_duplicates.pyi
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/unused_things.pyi
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/tests/vanilla_flake8_not_clean_forward_refs.pyi
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/LICENSE
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/README.md
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/pyproject.toml
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 flake8_pyi-24.4.0/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.editorconfig
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.flake8
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20526 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/ERRORCODES.md
+-rw-r--r--   0        0        0    93305 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/pyi.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/scripts/typeshed_primer_download_errors.js
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/scripts/typeshed_primer_post_comment.js
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/workflows/typeshed_primer.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.github/workflows/typeshed_primer_comment.yml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/F822.pyi
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/aliases.pyi
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/attribute_annotations.pyi
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/calls.pyi
+-rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/classdefs.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/comparisons.pyi
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/defaults.pyi
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/del.pyi
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/disabled_by_default.pyi
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/emptyclasses.pyi
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/emptyfunctions.pyi
+-rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/exit_methods.pyi
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/forward_refs.pyi
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/forward_refs_annassign.pyi
+-rw-r--r--   0        0        0    15235 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/imports.pyi
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/incomplete.pyi
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/literals.pyi
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/names_requiring_values.pyi
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/never_vs_noreturn.pyi
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/pep570.pyi
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/pep604_union_types.pyi
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/pep646_py311.pyi
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/pep695_py312.pyi
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/quotes.pyi
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/single_element_tuples.pyi
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/sysplatform.pyi
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/sysversioninfo.pyi
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/test_pyi_files.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/type_comments.pyi
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/typevar.pyi
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/union_duplicates.pyi
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/unused_things.pyi
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/tests/vanilla_flake8_not_clean_forward_refs.pyi
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/LICENSE
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/README.md
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 flake8_pyi-24.4.1/PKG-INFO
```

### Comparing `flake8_pyi-24.4.0/.flake8` & `flake8_pyi-24.4.1/.flake8`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/.pre-commit-config.yaml` & `flake8_pyi-24.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/CHANGELOG.md` & `flake8_pyi-24.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## 24.4.1
+
+New error codes:
+* Y066: When using if/else with `sys.version_info`,
+  put the code for new Python versions first.
+
 ## 24.4.0
 
 Bugfixes:
 * Fix Y026 false positive: allow simple assignment to `None` in class scopes
   if the class is known to be an enum class.
 
 ## 24.3.1
```

### Comparing `flake8_pyi-24.4.0/CONTRIBUTING.md` & `flake8_pyi-24.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/ERRORCODES.md` & `flake8_pyi-24.4.1/ERRORCODES.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 | Y059 | `Generic[]` should always be the last base class, if it is present in a class's bases tuple. At runtime, if `Generic[]` is not the final class in a the bases tuple, this [can cause the class creation to fail](https://github.com/python/cpython/issues/106102). In a stub file, however, this rule is enforced purely for stylistic consistency. | Style
 | Y060 | Redundant inheritance from `Generic[]`. For example, `class Foo(Iterable[_T], Generic[_T]): ...` can be written more simply as `class Foo(Iterable[_T]): ...`.<br><br>To avoid false-positive errors, and to avoid complexity in the implementation, this check is deliberately conservative: it only flags classes where all subscripted bases have identical code inside their subscript slices. | Style
 | Y061 | Do not use `None` inside a `Literal[]` slice. For example, use `Literal["foo"] \| None` instead of `Literal["foo", None]`. While both are legal according to [PEP 586](https://peps.python.org/pep-0586/), the former is preferred for stylistic consistency. Note that this warning is not emitted if Y062 is emitted for the same `Literal[]` slice. For example, `Literal[None, None, True, True]` only causes Y062 to be emitted. | Style
 | Y062 | `Literal[]` slices shouldn't contain duplicates, e.g. `Literal[True, True]` is not allowed. | Redundant code
 | Y063 | Use [PEP 570 syntax](https://peps.python.org/pep-0570/) (e.g. `def foo(x: int, /) -> None: ...`) to denote positional-only arguments, rather than [the older Python 3.7-compatible syntax described in PEP 484](https://peps.python.org/pep-0484/#positional-only-arguments) (`def foo(__x: int) -> None: ...`, etc.). | Style
 | Y064 | Use simpler syntax to define final literal types. For example, use `x: Final = 42` instead of `x: Final[Literal[42]]`. | Style
 | Y065 | Don't use bare `Incomplete` in argument and return annotations. Instead, leave them unannotated. Omitting an annotation entirely from a function will cause some type checkers to view the parameter or return type as "untyped"; this may result in stricter type-checking on code that makes use of the stubbed function. | Style
+| Y066 | When using if/else with `sys.version_info`, put the code for new Python versions first. | Style
 
 ## Warnings disabled by default
 
 The following error codes are also provided, but are disabled by default due to
 the risk of false-positive errors. To enable these error codes, use
 `--extend-select={code1,code2,...}` on the command line or in your flake8
 configuration file.
```

### Comparing `flake8_pyi-24.4.0/pyi.py` & `flake8_pyi-24.4.1/pyi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1582,14 +1582,16 @@
                         self.visit(elt)
             else:
                 self.visit(node)
         else:
             self.visit(node)
 
     def visit_If(self, node: ast.If) -> None:
+        self._check_for_Y066_violations(node)
+
         test = node.test
         # No types can appear in if conditions, so avoid confusing additional errors.
         with self.string_literals_allowed.enabled():
             self.visit(test)
         if isinstance(test, ast.BoolOp):
             for expression in test.values:
                 self._check_if_expression(expression)
@@ -1617,14 +1619,42 @@
                 else:
                     self.error(node, Y002)
             else:
                 self.error(node, Y002)
         else:
             self.error(node, Y002)
 
+    def _check_for_Y066_violations(self, node: ast.If) -> None:
+        def is_version_info(attr: ast.expr) -> bool:
+            return (
+                isinstance(attr, ast.Attribute)
+                and _is_name(attr.value, "sys")
+                and attr.attr == "version_info"
+            )
+
+        def if_chain_ends_with_else(if_chain: ast.If) -> bool:
+            orelse = if_chain.orelse
+            if len(orelse) == 1 and isinstance(orelse[0], ast.If):
+                return if_chain_ends_with_else(orelse[0])
+            return bool(orelse)
+
+        test = node.test
+        if not isinstance(test, ast.Compare):
+            return
+
+        left = test.left
+        op = test.ops[0]
+        if (
+            is_version_info(left)
+            and isinstance(op, ast.Lt)  # sys.version_info < ...
+            and if_chain_ends_with_else(node)
+        ):
+            new_syntax = "if " + unparse(test).replace("<", ">=", 1)
+            self.error(node, Y066.format(new_syntax=new_syntax))
+
     def _check_subscript_version_check(self, node: ast.Compare) -> None:
         # unless this is on, comparisons against a single integer aren't allowed
         must_be_single = False
         # if strict equality is allowed, it must be against a tuple of this length
         can_have_strict_equals: int | None = None
         version_info = node.left
         if isinstance(version_info, ast.Subscript):
@@ -2411,14 +2441,18 @@
     "class would be inferred as generic anyway"
 )
 Y061 = 'Y061 None inside "Literal[]" expression. Replace with "{suggestion}"'
 Y062 = 'Y062 Duplicate "Literal[]" member "{}"'
 Y063 = "Y063 Use PEP-570 syntax to indicate positional-only arguments"
 Y064 = 'Y064 Use "{suggestion}" instead of "{original}"'
 Y065 = 'Y065 Leave {what} unannotated rather than using "Incomplete"'
+Y066 = (
+    "Y066 When using if/else with sys.version_info, "
+    'put the code for new Python versions first, e.g. "{new_syntax}"'
+)
 Y090 = (
     'Y090 "{original}" means '
     '"a tuple of length 1, in which the sole element is of type {typ!r}". '
     'Perhaps you meant "{new}"?'
 )
 
 DISABLED_BY_DEFAULT = ["Y090"]
```

### Comparing `flake8_pyi-24.4.0/.github/scripts/typeshed_primer_download_errors.js` & `flake8_pyi-24.4.1/.github/scripts/typeshed_primer_download_errors.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/.github/scripts/typeshed_primer_post_comment.js` & `flake8_pyi-24.4.1/.github/scripts/typeshed_primer_post_comment.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/.github/workflows/check.yml` & `flake8_pyi-24.4.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/.github/workflows/publish.yml` & `flake8_pyi-24.4.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/.github/workflows/typeshed_primer.yml` & `flake8_pyi-24.4.1/.github/workflows/typeshed_primer.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/.github/workflows/typeshed_primer_comment.yml` & `flake8_pyi-24.4.1/.github/workflows/typeshed_primer_comment.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/aliases.pyi` & `flake8_pyi-24.4.1/tests/aliases.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/attribute_annotations.pyi` & `flake8_pyi-24.4.1/tests/attribute_annotations.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/calls.pyi` & `flake8_pyi-24.4.1/tests/calls.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/classdefs.pyi` & `flake8_pyi-24.4.1/tests/classdefs.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/defaults.pyi` & `flake8_pyi-24.4.1/tests/defaults.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/emptyfunctions.pyi` & `flake8_pyi-24.4.1/tests/emptyfunctions.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/exit_methods.pyi` & `flake8_pyi-24.4.1/tests/exit_methods.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/forward_refs.pyi` & `flake8_pyi-24.4.1/tests/forward_refs.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/forward_refs_annassign.pyi` & `flake8_pyi-24.4.1/tests/forward_refs_annassign.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/imports.pyi` & `flake8_pyi-24.4.1/tests/imports.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/incomplete.pyi` & `flake8_pyi-24.4.1/tests/incomplete.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/literals.pyi` & `flake8_pyi-24.4.1/tests/literals.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/names_requiring_values.pyi` & `flake8_pyi-24.4.1/tests/names_requiring_values.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/never_vs_noreturn.pyi` & `flake8_pyi-24.4.1/tests/never_vs_noreturn.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/pep570.pyi` & `flake8_pyi-24.4.1/tests/pep570.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/pep604_union_types.pyi` & `flake8_pyi-24.4.1/tests/pep604_union_types.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/pep695_py312.pyi` & `flake8_pyi-24.4.1/tests/pep695_py312.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/quotes.pyi` & `flake8_pyi-24.4.1/tests/quotes.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/single_element_tuples.pyi` & `flake8_pyi-24.4.1/tests/single_element_tuples.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/test_pyi_files.py` & `flake8_pyi-24.4.1/tests/test_pyi_files.py`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/type_comments.pyi` & `flake8_pyi-24.4.1/tests/type_comments.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/typevar.pyi` & `flake8_pyi-24.4.1/tests/typevar.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/union_duplicates.pyi` & `flake8_pyi-24.4.1/tests/union_duplicates.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/tests/unused_things.pyi` & `flake8_pyi-24.4.1/tests/unused_things.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/.gitignore` & `flake8_pyi-24.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/LICENSE` & `flake8_pyi-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/README.md` & `flake8_pyi-24.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-24.4.0/pyproject.toml` & `flake8_pyi-24.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 authors = [
   { name="Łukasz Langa", email="=lukasz@langa.pl" },
 ]
 maintainers = [
   { name="Jelle Zijlstra", email="jelle.zijlstra@gmail.com" },
   { name="Alex Waygood", email="alex.waygood@gmail.com" },
-  { name="Sebastian Rittau" },
+  { name="Sebastian Rittau", email="sebastian@rittau.biz" },
   { name="Akuli" },
   { name="Shantanu" },
 ]
 description = "A plugin for flake8 to enable linting .pyi stub files."
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.8"
@@ -26,15 +26,15 @@
     "pyflakes",
     "linter",
     "qa",
     "stubs",
     "typing",
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Flake8",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `flake8_pyi-24.4.0/PKG-INFO` & `flake8_pyi-24.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: flake8-pyi
-Version: 24.4.0
+Version: 24.4.1
 Summary: A plugin for flake8 to enable linting .pyi stub files.
 Project-URL: Homepage, https://github.com/PyCQA/flake8-pyi
 Project-URL: Source, https://github.com/PyCQA/flake8-pyi
 Project-URL: Bug Tracker, https://github.com/PyCQA/flake8-pyi/issues
 Project-URL: Changelog, https://github.com/PyCQA/flake8-pyi/blob/main/CHANGELOG.md
 Author-email: Łukasz Langa <=lukasz@langa.pl>
-Maintainer: Sebastian Rittau, Akuli, Shantanu
-Maintainer-email: Jelle Zijlstra <jelle.zijlstra@gmail.com>, Alex Waygood <alex.waygood@gmail.com>
+Maintainer: Akuli, Shantanu
+Maintainer-email: Jelle Zijlstra <jelle.zijlstra@gmail.com>, Alex Waygood <alex.waygood@gmail.com>, Sebastian Rittau <sebastian@rittau.biz>
 License: MIT
 License-File: LICENSE
 Keywords: bugs,flake8,linter,pyflakes,pyi,qa,stubs,typing
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

