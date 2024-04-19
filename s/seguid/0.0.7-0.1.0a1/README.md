# Comparing `tmp/seguid-0.0.7.tar.gz` & `tmp/seguid-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seguid-0.0.7.tar", max compression
+gzip compressed data, was "seguid-0.1.0a1.tar", max compression
```

## Comparing `seguid-0.0.7.tar` & `seguid-0.1.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1092 2024-04-19 12:23:15.489563 seguid-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     1593 2024-04-19 12:23:15.489563 seguid-0.0.7/README.md
--rw-r--r--   0        0        0      907 2024-04-19 12:23:15.493563 seguid-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2564 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/__init__.py
--rw-r--r--   0        0        0     2209 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/__main__.py
--rw-r--r--   0        0        0     3370 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/_asserts.py
--rw-r--r--   0        0        0     8327 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/_chksum.py
--rw-r--r--   0        0        0      765 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/_config.py
--rw-r--r--   0        0        0     3504 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/_manip.py
--rw-r--r--   0        0        0     3001 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/_reprutils.py
--rw-r--r--   0        0        0     1398 2024-04-19 12:23:15.493563 seguid-0.0.7/src/seguid/_tables.py
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 seguid-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-17 17:32:00.313892 seguid-0.1.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     1593 2024-04-17 17:32:00.313892 seguid-0.1.0a1/README.md
+-rw-r--r--   0        0        0      952 2024-04-17 17:32:00.313892 seguid-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      697 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/__init__.py
+-rw-r--r--   0        0        0     2209 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/__main__.py
+-rw-r--r--   0        0        0     3370 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_asserts.py
+-rw-r--r--   0        0        0     9473 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_chksum.py
+-rw-r--r--   0        0        0      765 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_config.py
+-rw-r--r--   0        0        0     3504 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_manip.py
+-rw-r--r--   0        0        0     3001 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_reprutils.py
+-rw-r--r--   0        0        0     1398 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_tables.py
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 seguid-0.1.0a1/PKG-INFO
```

### Comparing `seguid-0.0.7/LICENSE.txt` & `seguid-0.1.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/README.md` & `seguid-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/pyproject.toml` & `seguid-0.1.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "seguid"
-version = "0.0.7"
+version = "0.1.0a01"
 description = "Sequence Globally Unique Identifier (SEGUID) Checksums for Linear, Circular, Single-Stranded and Double-Stranded Biological Sequences"
 authors = [
   "Bjorn Johansson <bjornjobb@gmail.com>",
   "Henrik Bengtsson",
   "Louis Abraham"
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://seguid-python.seguid.org"
-homepage = "https://www.seguid.org"
+homepage = "https://github.com/seguid/seguid-python?tab=readme-ov-file#seguid-v2-checksums-for-linear-circular-single--and-double-stranded-biological-sequences"
 repository = "https://github.com/seguid/seguid-python"
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/seguid/seguid-python/issues"
+
 [tool.poetry.dependencies]
 python = ">=3.6, <4.0"
 pydivsufsort = { version = "^0.0.14", optional = true }
 setuptools = [
   {version = "<=69.0.3", python = "<3.8"},
   {version = "<=59.6.0", python = "<3.7"},
 ]
```

### Comparing `seguid-0.0.7/src/seguid/__main__.py` & `seguid-0.1.0a1/src/seguid/__main__.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/src/seguid/_asserts.py` & `seguid-0.1.0a1/src/seguid/_asserts.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/src/seguid/_chksum.py` & `seguid-0.1.0a1/src/seguid/_chksum.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""
+seguid.
 
+The seguid module provides four functions for calculations of SEGUID checksums
+for biological sequences with varying topologies:
+
+ * lsseguid: (l)inear   (s)ingle-stranded SEGUID
+ * csseguid: (c)ircular (s)ingle-stranded SEGUID
+ * ldseguid: (l)inear   (d)ouble-stranded SEGUID
+ * cdseguid: (c)ircular (d)ouble-stranded SEGUID
+
+Some auxillary functions are also provided.
+
+The functions can be made to work without external dependencies, but
+csseguid and cdseguid are considerably faster with pydivsufsort installed.
+
+"""
 
 import hashlib
 import base64
 
 from seguid._manip import reverse
 from seguid._manip import rotate
 from seguid._manip import rotate_to_min
@@ -48,29 +64,28 @@
         shortform = csum[:short]
     return " ".join((shortform, longform)).strip()
 
 
 def seguid(seq: str, alphabet: str = "{DNA}", form: str = "long") -> str:
     """SEGUID v1 checksum for linear protein or single-stranded DNA.
 
-    .. warning::
-        ``seguid()`` (obsolete) is superseded by :func:`lsseguid()` (recommended).
+    'Warning: seguid() (obsolete) is superseded by lsseguid() (recommended).'
 
     Given a nucleotide or amino-acid sequence ``seq`` in uppercase, the function returns
-    a string containing the **SE**\ quence **G**\ lobally **U**\ nique **ID**\ entifier (**SEGUID**\ ).
-    The SEGUID is defined as the Base64 encoded SHA1 checksum calculated for the sequence
-    in uppercase with the trailing padding symbol (``=``) removed.
+    a string containing the SEquence Globally Unique IDentifier (SEGUID). The SEGUID is
+    defined as the Base64 encoded SHA1 checksum calculated for the sequence in uppercase
+    with the trailing padding symbol (``=``) removed.
 
-    The original definition of the SEGUID v1 checksum algorithm (Babnigg & Giometti, 2006)
+    The original definition of the SEGUID checksum algorithm (Babnigg & Giometti, 2006)
     included transformation to uppercase before calculating the checksum.
 
-    ``seguid()`` does *not* coerce the input sequence to upper case. If your input sequence
-    has lower-case symbols, you can use :meth:`str.upper` to emulate what the original method does.
+    `seguid()` does *not* coerce the input sequence to upper case. If your input sequence
+    has lower-case symbols, you can use `seq.upper()` to emulate what the original method does.
 
-    ``seguid()`` only accepts symbols as specified by the `alphabet` argument.
+    `seguid()` only accepts symbols as specified by the `alphabet` argument.
 
     Thus, our implementation is more conservative, which has the benefit of
     lowering the risk of passing the incorrect sequence by mistake.
 
     The resulting checksum string may contain forward slash (``/``) and plus-sign (``+``) symbols.
     These characters cannot be a part of a Uniform Resource Locator (URL) or a filename on
     some operating systems. The SEGUID v2 checksum produced by ``lsseguid()`` is similar to the
@@ -80,32 +95,46 @@
     The checksum is prefixed with ``seguid=``.
 
     Examples
     --------
     >>> seguid("AT")
     'seguid=Ax/RG6hzSrMEEWoCO1IWMGska+4'
 
+    References
+    ----------
+
+    * Babnigg, G., & Giometti, C. S. (2006). A database of unique protein
+      sequence identifiers for proteome studies. Proteomics, 6(16), 4514–4522.
+      https://doi.org/10.1002/pmic.200600032
+
+    * Pereira, Humberto, Paulo César Silva, Wayne M Davis, Louis Abraham, Gyorgy Babnigg,
+      Henrik Bengtsson, and Bjorn Johansson. 2024. “SEGUID v2: Extending SEGUID Checksums
+      for Circular, Linear, Single- and Double-Stranded Biological Sequences.” bioRxiv.
+      https://doi.org/10.1101/2024.02.28.582384.
     """
     return _form(
         seguid_prefix,
         _seguid(seq, alphabet=alphabet, encoding=base64.standard_b64encode),
         form,
     )
 
 
 def lsseguid(seq: str, alphabet: str = "{DNA}", form: str = "long") -> str:
     """SEGUID checksum for linear single-stranded DNA.
 
-    Identical to the ``seguid()`` function except for that forward slashes (``/``) and plus signs (``+``)
-    in the resulting checksum are replaced by underscores (``_``) and minus signs (``-``), respectively
+    Identical to the ``seguid()`` function except for that the forward slashes (``/``) and plus signs (``+``)
+    of the standard Base64 encoding are replaced by underscores (``_``) and minus signs (``-``), respectively
     following the Base64url standard in RFC 4648 section 5.
 
+    The ``base64.urlsafe_b64encode()`` from the Python standard library is used.
+
     This checksum is applicable to linear single-stranded DNA sequences or
     protein sequences. If protein sequences are analyzed, the alphabet
-    argument should be ``"{protein}"`` or ``"{protein-extended}"``.
+    argument should be ``"{protein}"`` or ``"{protein-extended}"``. See _tables
+    module for details.
 
     The checksum is prefixed with ``lsseguid=``.
 
     Examples
     --------
     >>> lsseguid("AT")
     'lsseguid=Ax_RG6hzSrMEEWoCO1IWMGska-4'
@@ -116,16 +145,16 @@
         form,
     )
 
 
 def csseguid(seq: str, alphabet: str = "{DNA}", form: str = "long") -> str:
     r"""SEGUID checksum for circular single-stranded DNA.
 
-    The ``csseguid()`` is the :func:`lsseguid()` checksum calculated for the lexicographically
-    smallest string rotation of ``seq``.
+    The ``csseguid()`` is the ``lsseguid()`` checksum calculated for the lexicographically
+    smallest string rotation of a sequence.
 
     Only defined for circular single-stranded sequences.
 
     The checksum is prefixed with ``csseguid=``.
 
     Examples
     --------
@@ -149,22 +178,21 @@
 
 def ldseguid(
     watson: str, crick: str, alphabet: str = "{DNA}", form: str = "long"
 ) -> str:
     r"""SEGUID checksum for linear double-stranded DNA.
 
     Calculates the ``ldseguid()`` checksum for a double-stranded DNA (dsDNA) sequence defined by two
-    strings representing the upper (Watson) and the complementary (Crick) DNA strands. Watson and Crick
-    strands are always equal in length.
-
+    strings representing the upper (Watson) and the complementary (Crick) DNA strands.
     Optional single-stranded DNA regions in the ends are indicated by a dash (``-``) in either strand.
+    Watson and Crick strands are always equal in length.
 
     The algorithm first selects the lexicographically smallest of the Watson and Crick strands.
 
-    The two string are joined 5'-3', separated by a semicolon (``;``) and the :func:`lsseguid()` function
+    The two string are joined 5'-3', separated by a semicolon (``;``) and the ``lsseguid()`` function
     is used on the resulting string.
 
     ::
 
         dsDNA    SEGUID checksum
 
         -TATGCC  ldseguid=rr65d6AYuP-CdMaVmdw3L9FPt6I
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `seguid-0.0.7/src/seguid/_config.py` & `seguid-0.1.0a1/src/seguid/_config.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/src/seguid/_manip.py` & `seguid-0.1.0a1/src/seguid/_manip.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/src/seguid/_reprutils.py` & `seguid-0.1.0a1/src/seguid/_reprutils.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/src/seguid/_tables.py` & `seguid-0.1.0a1/src/seguid/_tables.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.7/PKG-INFO` & `seguid-0.1.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seguid
-Version: 0.0.7
+Version: 0.1.0a1
 Summary: Sequence Globally Unique Identifier (SEGUID) Checksums for Linear, Circular, Single-Stranded and Double-Stranded Biological Sequences
-Home-page: https://www.seguid.org
+Home-page: https://github.com/seguid/seguid-python?tab=readme-ov-file#seguid-v2-checksums-for-linear-circular-single--and-double-stranded-biological-sequences
 License: MIT
 Author: Bjorn Johansson
 Author-email: bjornjobb@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pydivsufsort
 Requires-Dist: pydivsufsort (>=0.0.14,<0.0.15) ; extra == "pydivsufsort"
 Requires-Dist: setuptools (<=59.6.0) ; python_version < "3.7"
 Requires-Dist: setuptools (<=69.0.3) ; python_version < "3.8"
-Project-URL: Bug Tracker, https://github.com/seguid/seguid-python/issues
 Project-URL: Documentation, https://seguid-python.seguid.org
 Project-URL: Repository, https://github.com/seguid/seguid-python
 Description-Content-Type: text/markdown
 
 [![Python checks](https://github.com/seguid/seguid-python/actions/workflows/check-python.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/check-python.yml)
 [![seguid-tests](https://github.com/seguid/seguid-python/actions/workflows/seguid-tests.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/seguid-tests.yml)
 [![Python Code Coverage](https://codecov.io/gh/seguid/seguid-python/graph/badge.svg)](https://codecov.io/gh/seguid/seguid-python)
```

