# Comparing `tmp/mo-testing-7.585.24095.tar.gz` & `tmp/mo_testing-7.587.24110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-testing-7.585.24095.tar", last modified: Thu Apr  4 12:52:10 2024, max compression
+gzip compressed data, was "mo_testing-7.587.24110.tar", last modified: Fri Apr 19 03:13:34 2024, max compression
```

## Comparing `mo-testing-7.585.24095.tar` & `mo_testing-7.587.24110.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:52:10.315884 mo-testing-7.585.24095/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo-testing-7.585.24095/LICENSE
--rw-rw-rw-   0        0        0     2047 2024-04-04 12:52:10.315884 mo-testing-7.585.24095/PKG-INFO
--rw-rw-rw-   0        0        0      946 2020-05-12 21:52:10.000000 mo-testing-7.585.24095/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 12:52:10.306527 mo-testing-7.585.24095/mo_testing/
--rw-rw-rw-   0        0        0      449 2024-04-04 12:52:03.000000 mo-testing-7.585.24095/mo_testing/__init__.py
--rw-rw-rw-   0        0        0    11718 2024-04-04 12:52:03.000000 mo-testing-7.585.24095/mo_testing/fuzzytestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:52:10.314832 mo-testing-7.585.24095/mo_testing.egg-info/
--rw-rw-rw-   0        0        0     2047 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 12:52:10.315884 mo-testing-7.585.24095/setup.cfg
--rw-rw-rw-   0        0        0     2092 2024-04-04 12:52:06.000000 mo-testing-7.585.24095/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:13:34.052117 mo_testing-7.587.24110/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-7.587.24110/LICENSE
+-rw-rw-rw-   0        0        0     2047 2024-04-19 03:13:34.051107 mo_testing-7.587.24110/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2020-05-12 21:52:10.000000 mo_testing-7.587.24110/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 03:13:34.040584 mo_testing-7.587.24110/mo_testing/
+-rw-rw-rw-   0        0        0      449 2024-04-04 12:52:03.000000 mo_testing-7.587.24110/mo_testing/__init__.py
+-rw-rw-rw-   0        0        0    11849 2024-04-19 03:13:23.000000 mo_testing-7.587.24110/mo_testing/fuzzytestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:13:34.050107 mo_testing-7.587.24110/mo_testing.egg-info/
+-rw-rw-rw-   0        0        0     2047 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 03:13:34.000000 mo_testing-7.587.24110/mo_testing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 03:13:34.053117 mo_testing-7.587.24110/setup.cfg
+-rw-rw-rw-   0        0        0     2092 2024-04-19 03:13:26.000000 mo_testing-7.587.24110/setup.py
```

### Comparing `mo-testing-7.585.24095/LICENSE` & `mo_testing-7.587.24110/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-testing-7.585.24095/PKG-INFO` & `mo_testing-7.587.24110/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 7.585.24095
+Version: 7.587.24110
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-testing-7.585.24095/README.md` & `mo_testing-7.587.24110/README.md`

 * *Files identical despite different names*

### Comparing `mo-testing-7.585.24095/mo_testing/fuzzytestcase.py` & `mo_testing-7.587.24110/mo_testing/fuzzytestcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,14 @@
 from mo_logs import Except, Log, suppress_exception
 from mo_logs.strings import expand_template, quote
 from mo_math import is_number, log10
 from mo_times import dates
 
 
 class FuzzyTestCase(unittest.TestCase):
-    """
-    COMPARE STRUCTURE AND NUMBERS!
-
-    ONLY THE ATTRIBUTES IN THE expected STRUCTURE ARE TESTED TO EXIST
-    EXTRA ATTRIBUTES ARE IGNORED.
-
-    NUMBERS ARE MATCHED BY ...
-    * places (UP TO GIVEN SIGNIFICANT DIGITS)
-    * digits (UP TO GIVEN DECIMAL PLACES, WITH NEGATIVE MEANING LEFT-OF-UNITS)
-    * delta (MAXIMUM ABSOLUTE DIFFERENCE FROM expected)
-    """
-
     def __init__(self, *args, **kwargs):
         unittest.TestCase.__init__(self, *args, **kwargs)
         self.default_places=15
 
 
     def set_default_places(self, places):
         """
@@ -94,14 +82,25 @@
                 return True
             except Exception as cause:
                 causes.append(cause)
         Log.error("problem is not raised", cause=first(causes))
 
 
 def assertAlmostEqual(test, expected, digits=None, places=None, msg=None, delta=None):
+    """
+    COMPARE STRUCTURE AND NUMBERS!
+
+    ONLY THE ATTRIBUTES IN THE expected STRUCTURE ARE TESTED TO EXIST
+    EXTRA ATTRIBUTES ARE IGNORED.
+
+    NUMBERS ARE MATCHED BY ...
+    * places (UP TO GIVEN SIGNIFICANT DIGITS)
+    * digits (UP TO GIVEN DECIMAL PLACES, WITH NEGATIVE MEANING LEFT-OF-UNITS)
+    * delta (MAXIMUM ABSOLUTE DIFFERENCE FROM expected)
+    """
     show_detail = True
     test = from_data(test)
     expected = from_data(expected)
     try:
         if test is None and (is_null_op(expected) or expected is None):
             return
         elif test is expected:
@@ -110,15 +109,18 @@
             assertAlmostEqualValue(test, expected, msg=msg, digits=digits, places=places, delta=delta)
         elif isinstance(test, UniqueIndex):
             if test ^ expected:
                 Log.error("Sets do not match")
         elif is_data(expected) and is_data(test):
             for k, e in from_data(expected).items():
                 t = test.get(k)
-                assertAlmostEqual(t, e, msg=coalesce(msg, "")+"key "+quote(k)+": ", digits=digits, places=places, delta=delta)
+                try:
+                    assertAlmostEqual(t, e, msg=coalesce(msg, "")+"key "+quote(k)+": ", digits=digits, places=places, delta=delta)
+                except Exception as cause:
+                    Log.error("key {k}={t} does not match expected {k}={e}", k=k, t=t, e=e, cause=cause)
         elif is_data(expected):
             if is_many(test):
                 test = list(test)
                 if len(test) != 1:
                     Log.error("Expecting data, not a list")
                 test = test[0]
             for k, e in expected.items():
@@ -239,33 +241,32 @@
     if delta != None:
         num_param += 1
     if num_param > 1:
         raise TypeError("specify only one of digits, places or delta")
 
     if digits is not None:
         with suppress_exception:
-            diff = log10(abs(test-expected))
-            if diff < digits:
+            diff = round(abs(test-expected)*pow(10, digits))
+            if diff == 0:
                 return
 
         standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{digits}} decimal places", locals())
     elif delta is not None:
         if abs(test - expected) <= delta:
             return
 
         standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{delta}} delta", locals())
     else:
         if places is None:
             places = 15
 
         with suppress_exception:
-            diff = mo_math.log10(abs(test-expected))
-            if diff == None:
-                return  # Exactly the same
-            if diff < mo_math.ceiling(mo_math.log10(abs(test)))-places:
+            factor = mo_math.ceiling(log10(abs(test)))
+            diff = log10(abs(test-expected))-factor + places
+            if diff < -0.3:
                 return
 
         standardMsg = expand_template("{{test|json}} != {{expected|json}} within {{places}} places", locals())
 
     raise AssertionError(coalesce(msg, "") + ": (" + standardMsg + ")")
```

### Comparing `mo-testing-7.585.24095/mo_testing.egg-info/PKG-INFO` & `mo_testing-7.587.24110/mo_testing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 7.585.24095
+Version: 7.587.24110
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-testing-7.585.24095/setup.py` & `mo_testing-7.587.24110/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     install_requires=["mo-collections==5.584.24095","mo-dots==9.584.24095","mo-future==7.584.24095","mo-logs==8.584.24095","mo-math==7.584.24095","mo-threads==6.585.24095"],
     license='MPL 2.0',
     long_description='# More Testing\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertEqual` method with the following parameters:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n\n',
     long_description_content_type='text/markdown',
     name='mo-testing',
     packages=["mo_testing"],
     url='https://github.com/klahnakoski/mo-testing',
-    version='7.585.24095'
+    version='7.587.24110'
 )
```

