# Comparing `tmp/pyaffalddk-2.0.23.tar.gz` & `tmp/pyaffalddk-2.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.23.tar", last modified: Tue Apr 16 12:03:02 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.24.tar", last modified: Fri Apr 19 17:22:19 2024, max compression
```

## Comparing `pyaffalddk-2.0.23.tar` & `pyaffalddk-2.0.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:03:02.659210 pyaffalddk-2.0.23/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 12:03:02.655210 pyaffalddk-2.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:03:02.655210 pyaffalddk-2.0.23/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11165 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:03:02.655210 pyaffalddk-2.0.23/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 12:03:02.000000 pyaffalddk-2.0.23/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:03:02.659210 pyaffalddk-2.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 12:02:57.000000 pyaffalddk-2.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:22:19.336523 pyaffalddk-2.0.24/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-19 17:22:19.332523 pyaffalddk-2.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:22:19.332523 pyaffalddk-2.0.24/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:22:19.332523 pyaffalddk-2.0.24/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-19 17:22:19.000000 pyaffalddk-2.0.24/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 17:22:19.000000 pyaffalddk-2.0.24/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:22:19.000000 pyaffalddk-2.0.24/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 17:22:19.000000 pyaffalddk-2.0.24/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:22:19.336523 pyaffalddk-2.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 17:22:15.000000 pyaffalddk-2.0.24/setup.py
```

### Comparing `pyaffalddk-2.0.23/LICENSE` & `pyaffalddk-2.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.23/PKG-INFO` & `pyaffalddk-2.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.23
+Version: 2.0.24
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.23/pyaffalddk/__init__.py` & `pyaffalddk-2.0.24/pyaffalddk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     AffaldDKNoConnection,
 )
 from pyaffalddk.data import PickupEvents, PickupType, AffaldDKAddressInfo
 
 from pyaffalddk.const import ICON_LIST, MUNICIPALITIES_ARRAY, NAME_ARRAY, NAME_LIST, WEEKDAYS, WEEKDAYS_SHORT
 
 __title__ = "pyaffalddk"
-__version__ = "2.0.23"
+__version__ = "2.0.24"
 __author__ = "briis"
 __license__ = "MIT"
```

### Comparing `pyaffalddk-2.0.23/pyaffalddk/api.py` & `pyaffalddk-2.0.24/pyaffalddk/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,19 +207,19 @@
                 if row["toemningsdato"] not in NON_SUPPORTED_ITEMS:
                     _pickup_date = to_date(row["toemningsdato"])
                 elif str(row["toemningsdage"]).capitalize() in WEEKDAYS:
                     _pickup_date = get_next_weekday(row["toemningsdage"])
                 else:
                     continue
 
-                if (
-                    "genbrug" in row["ordningnavn"].lower()
-                    or "papir og glas/dåser" in row["ordningnavn"].lower()
-                    or "miljøkasse/tekstiler" in row["ordningnavn"].lower()
-                ):
+                if any(
+                        group in row["ordningnavn"].lower()
+                        for group in [
+                            "genbrug", "storskrald","papir og glas/dåser","miljøkasse/tekstiler"
+                        ]):
                     key = get_garbage_type_from_material(row["materielnavn"])
                 else:
                     key = get_garbage_type(row["ordningnavn"])
 
                 if key == row["ordningnavn"] and key != "Bestillerordning":
                     _LOGGER.warning(
                         "Garbage type [%s] is not defined in the system. Please notify the developer",
```

### Comparing `pyaffalddk-2.0.23/pyaffalddk/const.py` & `pyaffalddk-2.0.24/pyaffalddk/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         "4delt beholder",
         "Ressourcebeholder (pap/papir og glas/metal)",
     ],
     "plastmetalmadmdk": [
         "Plast/Metal/Mad- & drikkekartoner",
         "Plast, mad- og drikkekartoner og metal",
     ],
+    "plastmdkglasmetal": [],
     "pappapir": ["Pap/Papir", "Papir/Pap", "Papir og Pap"],
     "tekstil": [
         "Tekstiler",
         "Standplads",
         "Tekstilaffald",
         "Miljøkasse/tekstiler",
         "Tekstil",
@@ -213,19 +214,22 @@
         "Indsamling af pap (løst og beholder) (1 stk.)",
         "240 L - Pap - Skel (1 stk.)",
         "Beholder til pap (1 stk.)",
     ],
     "plastmetal": [
         "Plast, småt metal & MDK - 240 l. (1 stk.)",
     ],
+    "plastmdkglasmetal": ["240 L todelt genbrugsspand hver 4. uge (1 stk.)",
+    ],
     "plast": [
         "Plast og MDK 240 L (ejer.kommune) (1 stk.)",
     ],
     "storskrald": [
         "Storskrald - fortovsindsamling (1 stk.)",
+        "Storskrald (1 stk.)"
     ],
     "storskraldogtekstilaffald": [""],
     "haveaffald": [
         "Gen-Skel 0-2 meter (1 stk.)",
         "Haveaffald henteordning (1 stk.)",
     ],
     "papirglas": [
@@ -247,14 +251,15 @@
     "plastmetalmadmdk": [""],
     "pappapir": [
         "Genbrugsbeholder PP-240L/6uge (1 stk.)",
     ],
     "tekstil": [
         "Tekstil pose (1 stk.)",
         "Tekstilpose tømning (1 stk.)",
+        "Tekstilaffald (1 stk.)"
     ],
     "glasplast": [""],
     "plastmetalpapir": [""],
     "papirglasmetalplast": [
         "4-kammer (370 l) (1 stk.)",
         "Pap og papir/metal, glas og hård plast - 240 L (1 stk.)",
         "240 l genbrug låg i låg (1 stk.)"
@@ -282,14 +287,15 @@
     "storskraldogtekstilaffald": "mdi:table-furniture",
     "haveaffald": "mdi:leaf",
     "papirglas": "mdi:greenhouse",
     "papirglasmetalplast": "mdi:trash-can",
     "plastmadkarton": "mdi:trash-can",
     "papirglasdaaser": "mdi:trash-can",
     "pappapirglasmetal": "mdi:trash-can",
+    "plastmdkglasmetal": "mdi:trash-can",
     "plastmetalmadmdk": "mdi:trash-can",
     "pappapir": "mdi:file",
     "tekstil": "mdi:recycle",
     "glasplast": "mdi:trash-can",
     "plastmetalpapir": "mdi:trash-can",
     "plast": "mdi:trash-can",
 }
@@ -314,14 +320,15 @@
     "papirglasmetalplast": "Papir, Glas, Metal & Plast",
     "papirmetal": "Papir & Metal",
     "pappapir": "Pap & Papir",
     "pappapirglasmetal": "Pap, Papir, Glas & Metal",
     "pappi": "Papir & Plast",
     "plast": "Plast",
     "plastmadkarton": "Plast & Madkarton",
+    "plastmdkglasmetal": "Plast, Madkarton, Glas & Metal",
     "plastmetal": "Plast & Metal",
     "plastmetalmadmdk": "Plast, Metal, Mad & Drikkekartoner",
     "plastmetalpapir": "Plast, Metal & Papir",
     "restaffaldmadaffald": "Rest & Madaffald",
     "storskrald": "Storskrald",
     "storskraldogtekstilaffald": "Storskrald & Tekstilaffald",
     "tekstil": "Tekstilaffald",
```

### Comparing `pyaffalddk-2.0.23/pyaffalddk/data.py` & `pyaffalddk-2.0.24/pyaffalddk/data.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.23/pyaffalddk/images.py` & `pyaffalddk-2.0.24/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.23/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.24/pyaffalddk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.23
+Version: 2.0.24
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.23/setup.py` & `pyaffalddk-2.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.23",
+    version="2.0.24",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

