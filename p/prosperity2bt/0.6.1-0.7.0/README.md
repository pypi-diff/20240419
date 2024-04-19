# Comparing `tmp/prosperity2bt-0.6.1.tar.gz` & `tmp/prosperity2bt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.6.1.tar", last modified: Thu Apr 18 18:25:51 2024, max compression
+gzip compressed data, was "prosperity2bt-0.7.0.tar", last modified: Fri Apr 19 18:41:05 2024, max compression
```

## Comparing `prosperity2bt-0.6.1.tar` & `prosperity2bt-0.7.0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.077940 prosperity2bt-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-18 18:25:51.077940 prosperity2bt-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.057940 prosperity2bt-0.6.1/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.057940 prosperity2bt-0.6.1/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.057940 prosperity2bt-0.6.1/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.065940 prosperity2bt-0.6.1/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.073940 prosperity2bt-0.6.1/prosperity2bt/resources/round3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-04-18 18:25:46.000000 prosperity2bt-0.6.1/prosperity2bt/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:51.073940 prosperity2bt-0.6.1/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 18:25:51.000000 prosperity2bt-0.6.1/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-18 18:25:48.000000 prosperity2bt-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:25:51.077940 prosperity2bt-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.600824 prosperity2bt-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-19 18:41:05.600824 prosperity2bt-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.576823 prosperity2bt-0.7.0/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.576823 prosperity2bt-0.7.0/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.580824 prosperity2bt-0.7.0/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.584823 prosperity2bt-0.7.0/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.596824 prosperity2bt-0.7.0/prosperity2bt/resources/round3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2581061 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580446 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2580491 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   148534 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142870 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146400 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.600824 prosperity2bt-0.7.0/prosperity2bt/resources/round4/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1224274 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round4/prices_round_4_day_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1235320 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round4/prices_round_4_day_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1190339 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round4/prices_round_4_day_3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69259 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69601 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    67862 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-04-19 18:41:01.000000 prosperity2bt-0.7.0/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:41:05.600824 prosperity2bt-0.7.0/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-19 18:41:05.000000 prosperity2bt-0.7.0/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-19 18:41:05.000000 prosperity2bt-0.7.0/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:41:05.000000 prosperity2bt-0.7.0/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 18:41:05.000000 prosperity2bt-0.7.0/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 18:41:05.000000 prosperity2bt-0.7.0/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 18:41:05.000000 prosperity2bt-0.7.0/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-19 18:41:03.000000 prosperity2bt-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:41:05.600824 prosperity2bt-0.7.0/setup.cfg
```

### Comparing `prosperity2bt-0.6.1/LICENSE` & `prosperity2bt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/PKG-INFO` & `prosperity2bt-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.6.1
+Version: 0.7.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.6.1/README.md` & `prosperity2bt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/__main__.py` & `prosperity2bt-0.7.0/prosperity2bt/__main__.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/data.py` & `prosperity2bt-0.7.0/prosperity2bt/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     "AMETHYSTS": 20,
     "STARFRUIT": 20,
     "ORCHIDS": 100,
     "CHOCOLATE": 250,
     "STRAWBERRIES": 350,
     "ROSES": 60,
     "GIFT_BASKET": 60,
+    "COCONUT": 300,
+    "COCONUT_COUPON": 600,
 }
 
 @dataclass
 class PriceRow:
     day: int
     timestamp: int
     product: Symbol
```

### Comparing `prosperity2bt-0.6.1/prosperity2bt/datamodel.py` & `prosperity2bt-0.7.0/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/file_reader.py` & `prosperity2bt-0.7.0/prosperity2bt/file_reader.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/models.py` & `prosperity2bt-0.7.0/prosperity2bt/models.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_0.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round3/prices_round_3_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_1.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round3/prices_round_3_day_1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round3/prices_round_3_day_2.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round3/prices_round_3_day_2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv` & `prosperity2bt-0.7.0/prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt/runner.py` & `prosperity2bt-0.7.0/prosperity2bt/runner.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.6.1/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.7.0/prosperity2bt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.6.1
+Version: 0.7.0
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.6.1/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.7.0/prosperity2bt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -27,8 +27,15 @@
 prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
 prosperity2bt/resources/round3/__init__.py
 prosperity2bt/resources/round3/prices_round_3_day_0.csv
 prosperity2bt/resources/round3/prices_round_3_day_1.csv
 prosperity2bt/resources/round3/prices_round_3_day_2.csv
 prosperity2bt/resources/round3/trades_round_3_day_0_nn.csv
 prosperity2bt/resources/round3/trades_round_3_day_1_nn.csv
-prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+prosperity2bt/resources/round3/trades_round_3_day_2_nn.csv
+prosperity2bt/resources/round4/__init__.py
+prosperity2bt/resources/round4/prices_round_4_day_1.csv
+prosperity2bt/resources/round4/prices_round_4_day_2.csv
+prosperity2bt/resources/round4/prices_round_4_day_3.csv
+prosperity2bt/resources/round4/trades_round_4_day_1_nn.csv
+prosperity2bt/resources/round4/trades_round_4_day_2_nn.csv
+prosperity2bt/resources/round4/trades_round_4_day_3_nn.csv
```

### Comparing `prosperity2bt-0.6.1/pyproject.toml` & `prosperity2bt-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.6.1"
+version = "0.7.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

