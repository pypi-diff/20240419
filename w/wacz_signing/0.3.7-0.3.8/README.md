# Comparing `tmp/wacz_signing-0.3.7.tar.gz` & `tmp/wacz_signing-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wacz_signing-0.3.7.tar", max compression
+gzip compressed data, was "wacz_signing-0.3.8.tar", max compression
```

## Comparing `wacz_signing-0.3.7.tar` & `wacz_signing-0.3.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2022-10-01 19:18:01.340865 wacz_signing-0.3.7/COPYING
--rw-r--r--   0        0        0     3921 2023-03-15 19:24:50.140830 wacz_signing-0.3.7/README.md
--rw-r--r--   0        0        0      538 2024-02-28 18:17:09.870123 wacz_signing-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-01 14:24:50.997566 wacz_signing-0.3.7/wacz_signing/__init__.py
--rw-r--r--   0        0        0     5688 2022-10-05 19:40:58.732093 wacz_signing-0.3.7/wacz_signing/material.py
--rw-r--r--   0        0        0    11353 2024-02-28 18:10:12.685144 wacz_signing-0.3.7/wacz_signing/signer.py
--rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 wacz_signing-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-01 19:18:01.340865 wacz_signing-0.3.8/COPYING
+-rw-r--r--   0        0        0     3921 2023-03-15 19:24:50.140830 wacz_signing-0.3.8/README.md
+-rw-r--r--   0        0        0      538 2024-04-19 13:25:37.777886 wacz_signing-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-01 14:24:50.997566 wacz_signing-0.3.8/wacz_signing/__init__.py
+-rw-r--r--   0        0        0     5688 2022-10-05 19:40:58.732093 wacz_signing-0.3.8/wacz_signing/material.py
+-rw-r--r--   0        0        0    11529 2024-02-29 12:43:25.426631 wacz_signing-0.3.8/wacz_signing/signer.py
+-rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 wacz_signing-0.3.8/PKG-INFO
```

### Comparing `wacz_signing-0.3.7/COPYING` & `wacz_signing-0.3.8/COPYING`

 * *Files identical despite different names*

### Comparing `wacz_signing-0.3.7/README.md` & `wacz_signing-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `wacz_signing-0.3.7/pyproject.toml` & `wacz_signing-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wacz_signing"
-version = "0.3.7"
+version = "0.3.8"
 description = "A library for signing and timestamping file hashes"
 authors = ["Ben Steinberg <bsteinberg@law.harvard.edu>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `wacz_signing-0.3.7/wacz_signing/material.py` & `wacz_signing-0.3.8/wacz_signing/material.py`

 * *Files identical despite different names*

### Comparing `wacz_signing-0.3.7/wacz_signing/signer.py` & `wacz_signing-0.3.8/wacz_signing/signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,16 +156,18 @@
 
 
 def verify(signed_req):
     """ Verify a signed and timestamped string """
 
     # fingerprints (sha-256) of trusted domain and timestamp root certificates
     domain_cert_roots = [
-        # Lets Encrypt Root CA X3
+        # Lets Encrypt Root CA X3: https://crt.sh/?id=3958242236
         '6d99fb265eb1c5b3744765fcbc648f3cd8e1bffafdc4c2f99b9d47cf7ff1c24f',
+        # Lets Encrypt Intermediate R3: https://crt.sh/?id=3334561879
+        '67add1166b020ae61b8f5fc96813c04c2aa589960796865572a3c7e737613dfd'
     ]
 
     # add comma-separated cert roots in an env var; this is useful for testing
     additional_cert_roots = os.getenv('CERT_ROOTS')
     if additional_cert_roots:
         domain_cert_roots += additional_cert_roots.split(',')
```

### Comparing `wacz_signing-0.3.7/PKG-INFO` & `wacz_signing-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wacz_signing
-Version: 0.3.7
+Version: 0.3.8
 Summary: A library for signing and timestamping file hashes
 License: GPL-3.0-or-later
 Author: Ben Steinberg
 Author-email: bsteinberg@law.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wacz_signing Version: 0.3.7 Summary: A library for
+Metadata-Version: 2.1 Name: wacz_signing Version: 0.3.8 Summary: A library for
 signing and timestamping file hashes License: GPL-3.0-or-later Author: Ben
 Steinberg Author-email: bsteinberg@law.harvard.edu Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: cryptography
```

