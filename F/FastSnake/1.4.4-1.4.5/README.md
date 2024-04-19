# Comparing `tmp/fastsnake-1.4.4.tar.gz` & `tmp/fastsnake-1.4.5.tar.gz`

## Comparing `fastsnake-1.4.4.tar` & `fastsnake-1.4.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.4/requirements.txt
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/__init__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/entries.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/algorithms/binary_search.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/algorithms/knapsack.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/algorithms/lower_bound.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/algorithms/mex.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/algorithms/min_coins.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/algorithms/upper_bound.py
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/application/application.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/application/arg_parser.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/application/config.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/application/contest.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/application/runner.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/structures/b_tree.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/util/codeforces.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastsnake-1.4.4/fastsnake/util/compiler.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/conftest.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_algorithms/test_binary_search.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_algorithms/test_knapsack.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_algorithms/test_lower_bound.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_algorithms/test_mex.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_algorithms/test_min_coins.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_algorithms/test_upper_bound.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_codeforces_tools/test_problem_loader.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_codeforces_tools/sample_1949_J/0.in
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_codeforces_tools/sample_1949_J/0.out
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_codeforces_tools/sample_1949_J/1.in
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_codeforces_tools/sample_1949_J/1.out
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_compiler/sample.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_compiler/test_compiler.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.4/tests/test_structures/test_b_tree.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.4/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.4/LICENSE
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 fastsnake-1.4.4/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastsnake-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 fastsnake-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fastsnake-1.4.5/requirements.txt
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 fastsnake-1.4.5/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/entries.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/algorithms/binary_search.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/algorithms/knapsack.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/algorithms/lower_bound.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/algorithms/mex.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/algorithms/min_coins.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/algorithms/upper_bound.py
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/application/application.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/application/arg_parser.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/application/config.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/application/contest.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/application/runner.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/structures/b_tree.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/util/codeforces.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastsnake-1.4.5/fastsnake/util/compiler.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/conftest.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_algorithms/test_binary_search.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_algorithms/test_knapsack.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_algorithms/test_lower_bound.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_algorithms/test_mex.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_algorithms/test_min_coins.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_algorithms/test_upper_bound.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_codeforces_tools/test_problem_loader.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_codeforces_tools/sample_1949_J/0.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_codeforces_tools/sample_1949_J/0.out
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_codeforces_tools/sample_1949_J/1.in
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_codeforces_tools/sample_1949_J/1.out
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_compiler/sample.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_compiler/test_compiler.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 fastsnake-1.4.5/tests/test_structures/test_b_tree.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 fastsnake-1.4.5/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fastsnake-1.4.5/LICENSE
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 fastsnake-1.4.5/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fastsnake-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 fastsnake-1.4.5/PKG-INFO
```

### Comparing `fastsnake-1.4.4/.github/workflows/python-package.yml` & `fastsnake-1.4.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/entries.py` & `fastsnake-1.4.5/fastsnake/entries.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return [float(x) for x in input().split()]
  
  
 def input_float_matrix(n_rows: int, separator: Optional[str] = None) -> List[List[float]]:
     """
     Return an float matrix from input.
     """
-    return [float(x) for x in input().split(separator) for _ in range(n_rows)]
+    return [[float(x) for x in input().split(separator)] for _ in range(n_rows)]
 
 
 def input_int() -> int:
     """
     Return an int from input.
     """
     return int(input())
```

### Comparing `fastsnake-1.4.4/fastsnake/algorithms/knapsack.py` & `fastsnake-1.4.5/fastsnake/algorithms/knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/algorithms/min_coins.py` & `fastsnake-1.4.5/fastsnake/algorithms/min_coins.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/application/application.py` & `fastsnake-1.4.5/fastsnake/application/application.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/application/arg_parser.py` & `fastsnake-1.4.5/fastsnake/application/arg_parser.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/application/contest.py` & `fastsnake-1.4.5/fastsnake/application/contest.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/application/runner.py` & `fastsnake-1.4.5/fastsnake/application/runner.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/structures/b_tree.py` & `fastsnake-1.4.5/fastsnake/structures/b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/util/codeforces.py` & `fastsnake-1.4.5/fastsnake/util/codeforces.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/fastsnake/util/compiler.py` & `fastsnake-1.4.5/fastsnake/util/compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_algorithms/test_binary_search.py` & `fastsnake-1.4.5/tests/test_algorithms/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_algorithms/test_knapsack.py` & `fastsnake-1.4.5/tests/test_algorithms/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_algorithms/test_lower_bound.py` & `fastsnake-1.4.5/tests/test_algorithms/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_algorithms/test_mex.py` & `fastsnake-1.4.5/tests/test_algorithms/test_mex.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_algorithms/test_upper_bound.py` & `fastsnake-1.4.5/tests/test_algorithms/test_upper_bound.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_codeforces_tools/test_problem_loader.py` & `fastsnake-1.4.5/tests/test_codeforces_tools/test_problem_loader.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_compiler/test_compiler.py` & `fastsnake-1.4.5/tests/test_compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/tests/test_structures/test_b_tree.py` & `fastsnake-1.4.5/tests/test_structures/test_b_tree.py`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/.gitignore` & `fastsnake-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/LICENSE` & `fastsnake-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/README.md` & `fastsnake-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/pyproject.toml` & `fastsnake-1.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastsnake-1.4.4/PKG-INFO` & `fastsnake-1.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastSnake
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Python Helper CLI for Competitive Programming
 Project-URL: Homepage, https://github.com/JeanExtreme002/FastSnake
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: algorithms,cli,codeforces,competition,competitive programming,contest,helper,marathon,structures
 Classifier: Intended Audience :: Developers
```

