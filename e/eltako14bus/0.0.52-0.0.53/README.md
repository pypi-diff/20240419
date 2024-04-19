# Comparing `tmp/eltako14bus-0.0.52.tar.gz` & `tmp/eltako14bus-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eltako14bus-0.0.52.tar", last modified: Thu Apr 11 11:44:59 2024, max compression
+gzip compressed data, was "eltako14bus-0.0.53.tar", last modified: Fri Apr 19 21:50:25 2024, max compression
```

## Comparing `eltako14bus-0.0.52.tar` & `eltako14bus-0.0.53.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:44:59.367677 eltako14bus-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-11 11:44:59.367677 eltako14bus-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:44:59.367677 eltako14bus-0.0.52/eltako14bus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-11 11:44:59.000000 eltako14bus-0.0.52/eltako14bus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 11:44:59.000000 eltako14bus-0.0.52/eltako14bus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:44:59.000000 eltako14bus-0.0.52/eltako14bus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-11 11:44:59.000000 eltako14bus-0.0.52/eltako14bus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 11:44:59.000000 eltako14bus-0.0.52/eltako14bus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:44:59.367677 eltako14bus-0.0.52/eltakobus/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/coap.py
--rw-r--r--   0 runner    (1001) docker     (127)    44440 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    43255 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/eep.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/locking.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/eltakobus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:44:59.367677 eltako14bus-0.0.52/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:44:59.367677 eltako14bus-0.0.52/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-11 11:44:51.000000 eltako14bus-0.0.52/tests/generic_eep_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/eltako14bus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/eltakobus/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/coap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43255 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/eep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/tests/generic_eep_test.py
```

### Comparing `eltako14bus-0.0.52/LICENSE` & `eltako14bus-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/PKG-INFO` & `eltako14bus-0.0.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.52
+Version: 0.0.53
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.52/README.md` & `eltako14bus-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/eltako14bus.egg-info/PKG-INFO` & `eltako14bus-0.0.53/eltako14bus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.52
+Version: 0.0.53
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.52/eltakobus/bus.py` & `eltako14bus-0.0.53/eltakobus/bus.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/eltakobus/coap.py` & `eltako14bus-0.0.53/eltakobus/coap.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/eltakobus/device.py` & `eltako14bus-0.0.53/eltakobus/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -916,16 +916,16 @@
 
                 # FIXME: Find out where "send confirmation as dimmer telegram"
                 # is stored, and provide a way to ensure that
 
                 14: [
                     MemoryFileStartOfSectionComment("function group 1"),
                     MemoryFileNibbleExplanationComment(
-                         "AD DR ES S, KY FN CH ??",
-                         "key (5 = left, 6 = right), function (eg. 32 = A5-38-08), ch = channel"),
+                         "AD DR ES S, KY FN CH V ",
+                         "key (5 = left, 6 = right), function (eg. 32 = A5-38-08), ch = channel (0x10 = broadcast), v = value (e.g. dimming in percentage, brightness)"),
                     ],
                 }
     
 
 class FAE14SSR(BusObject, HasProgrammableRPS):
     size = 2
     discovery_name = bytes((0x04, 0x16))
```

### Comparing `eltako14bus-0.0.52/eltakobus/eep.py` & `eltako14bus-0.0.53/eltakobus/eep.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/eltakobus/error.py` & `eltako14bus-0.0.53/eltakobus/error.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/eltakobus/locking.py` & `eltako14bus-0.0.53/eltakobus/locking.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/eltakobus/message.py` & `eltako14bus-0.0.53/eltakobus/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,15 @@
         reported_address = eltakomessage.payload[0]
         reported_size = eltakomessage.payload[1]
         memory_size = eltakomessage.payload[2]
         model = eltakomessage.payload[4:8]
 
         if double_size:
             reported_size *= 2
-            if model != bytes((0x04, 0x34, 0x41, 0x00)):
+            if model != bytes((0x04, 0x34, 0x41, 0x00)) and model != bytes((0x04, 0x34, 0x51, 0x00)):
                 raise ParseError("Odd 0e byte (where 00 or 08 would be consistent with the rest of the ecosystem) found on something else than a FDG14, please verify whether 0e actually means 'this device is actually twice as large on the bus as it annouces'.")
 
         return EltakoDiscoveryReply(reported_address, reported_size, memory_size, model, is_fam)
 
     def __repr__(self):
         return "<%s address %d size %d, model %s%s>"%(type(self).__name__, self.reported_address, self.reported_size, b2a(self.model), " (FAM)" if self.is_fam else "")
```

### Comparing `eltako14bus-0.0.52/eltakobus/serial.py` & `eltako14bus-0.0.53/eltakobus/serial.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/eltakobus/util.py` & `eltako14bus-0.0.53/eltakobus/util.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.52/setup.py` & `eltako14bus-0.0.53/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eltako14bus",
-    version="0.0.52",
+    version="0.0.53",
     author="chrysn, grimmpp",
     author_email="chrysn@fsfe.org, grimmpp14@gmail.com",
     description="Library for participating in the Eltako Series 14 RS485 bus",
     url="https://github.com/grimmpp/eltako14bus",
     packages=setuptools.find_packages(),
     extras_require=extras_require,
     # Not that there'd be tests, but at least it fetches the right dependencies and syntax checks everything
```

### Comparing `eltako14bus-0.0.52/tests/generic_eep_test.py` & `eltako14bus-0.0.53/tests/generic_eep_test.py`

 * *Files identical despite different names*

