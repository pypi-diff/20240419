# Comparing `tmp/anemoi-utils-0.1.2.tar.gz` & `tmp/anemoi-utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi-utils-0.1.2.tar", last modified: Mon Apr 15 14:07:56 2024, max compression
+gzip compressed data, was "anemoi-utils-0.1.3.tar", last modified: Fri Apr 19 08:36:07 2024, max compression
```

## Comparing `anemoi-utils-0.1.2.tar` & `anemoi-utils-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:07:56.857730 anemoi-utils-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-15 14:07:56.853730 anemoi-utils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:07:56.853730 anemoi-utils-0.1.2/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:07:56.853730 anemoi-utils-0.1.2/anemoi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/anemoi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/anemoi/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/anemoi/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/anemoi/utils/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/anemoi/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:07:56.853730 anemoi-utils-0.1.2/anemoi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-15 14:07:56.000000 anemoi-utils-0.1.2/anemoi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-15 14:07:56.000000 anemoi-utils-0.1.2/anemoi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:07:56.000000 anemoi-utils-0.1.2/anemoi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 14:07:56.000000 anemoi-utils-0.1.2/anemoi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 14:07:56.000000 anemoi-utils-0.1.2/anemoi_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:07:56.000000 anemoi-utils-0.1.2/anemoi_utils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:07:56.857730 anemoi-utils-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-15 14:07:47.000000 anemoi-utils-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.721926 anemoi-utils-0.1.3/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/anemoi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/anemoi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/setup.py
```

### Comparing `anemoi-utils-0.1.2/LICENSE` & `anemoi-utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi-utils-0.1.2/PKG-INFO` & `anemoi-utils-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Home-page: https://github.com/ecmwf/anemoi-utils
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `anemoi-utils-0.1.2/README.md` & `anemoi-utils-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `anemoi-utils-0.1.2/anemoi/utils/humanize.py` & `anemoi-utils-0.1.3/anemoi/utils/humanize.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,47 +3,64 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
+"""
+Generate human readable strings
+"""
+
 import datetime
 import re
 from collections import defaultdict
 
 
-def bytes(n):
-    """
+def bytes(n: float) -> str:
+    """Convert a number of bytes to a human readable string
+
     >>> bytes(4096)
     '4 KiB'
+
     >>> bytes(4000)
     '3.9 KiB'
+
+    Parameters
+    ----------
+    n : float
+        the number of bytes
+
+    Returns
+    -------
+    str
+        a human readable string
+    """
+
+    """
+
+
+
     """
+
     if n < 0:
         sign = "-"
         n -= 0
     else:
         sign = ""
 
     u = ["", " KiB", " MiB", " GiB", " TiB", " PiB", " EiB", " ZiB", " YiB"]
     i = 0
     while n >= 1024:
         n /= 1024.0
         i += 1
     return "%s%g%s" % (sign, int(n * 10 + 0.5) / 10.0, u[i])
 
 
-def base2(n):
-    """
-    >>> base2(4096)
-    '4K'
-    >>> base2(4000)
-    '3.9K'
-    """
+def base2(n) -> str:
 
     u = ["", "K", "M", "G", "T", " P", "E", "Z", "Y"]
     i = 0
     while n >= 1024:
         n /= 1024.0
         i += 1
     return "%g%s" % (int(n * 10 + 0.5) / 10.0, u[i])
@@ -61,15 +78,32 @@
 def _plural(count):
     if count > 1:
         return "s"
     else:
         return ""
 
 
-def seconds(seconds):
+def seconds(seconds: float) -> str:
+    """Convert a number of seconds to a human readable string
+
+    >>> seconds(4000)
+    '1 hour 6 minutes 40 seconds'
+
+
+    Parameters
+    ----------
+    seconds : float
+        The number of seconds
+
+    Returns
+    -------
+    str
+        A human readable string
+
+    """
     if isinstance(seconds, datetime.timedelta):
         seconds = seconds.total_seconds()
 
     if seconds == 0:
         return "instantaneous"
 
     if seconds < 0.1:
@@ -109,14 +143,28 @@
 
 
 def number(value):
     return f"{value:,}"
 
 
 def plural(value, what):
+    """_summary_
+
+    Parameters
+    ----------
+    value : _type_
+        _description_
+    what : _type_
+        _description_
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
     return f"{number(value)} {what}{_plural(value)}"
 
 
 DOW = [
     "Monday",
     "Tuesday",
     "Wednesday",
@@ -155,14 +203,47 @@
     if n % 10 == 3:
         return "rd"
 
     return "th"
 
 
 def when(then, now=None, short=True):
+    """Generate a human readable string for a date, relative to now
+
+
+    >>> when(datetime.datetime.now() - datetime.timedelta(hours=2))
+    '2 hours ago'
+
+    >>> when(datetime.datetime.now() - datetime.timedelta(days=1))
+    'yesterday at 08:46'
+
+    >>> when(datetime.datetime.now() - datetime.timedelta(days=5))
+    'last Sunday'
+
+    >>> when(datetime.datetime.now() - datetime.timedelta(days=365))
+    'last year'
+
+    >>> when(datetime.datetime.now() + datetime.timedelta(days=365))
+    'next year'
+
+    Parameters
+    ----------
+    then : datetime.datetime
+        A datetime
+    now : datetime.datetime, optional
+        The reference date, by default NOW
+    short : bool, optional
+        Genererate shorter strings, by default True
+
+    Returns
+    -------
+    str
+        A human readable string
+
+    """
     last = "last"
 
     if now is None:
         now = datetime.datetime.now()
 
     diff = (now - then).total_seconds()
```

### Comparing `anemoi-utils-0.1.2/anemoi_utils.egg-info/PKG-INFO` & `anemoi-utils-0.1.3/anemoi_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to hold various functions to support training of ML models on ECMWF data.
 Home-page: https://github.com/ecmwf/anemoi-utils
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `anemoi-utils-0.1.2/setup.py` & `anemoi-utils-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "GitPython",
     "nvsmi",
 ]
 
 text_requires = [
     "termcolor",
 ]
+
 doc_requires = ["sphinx", "sphinx_rtd_theme", "nbsphinx", "pandoc"]
 
 all_requires = install_requires + provenance_requires + text_requires
 dev_requires = doc_requires + all_requires
 
 setuptools.setup(
     name="anemoi-utils",
```

