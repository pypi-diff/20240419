# Comparing `tmp/aleatory-0.2.0.tar.gz` & `tmp/aleatory-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dialidsantiago/Git/aleatory/dist/.tmp-ul0r25ua/aleatory-0.2.0.tar", last modified: Sun Jan 14 16:55:22 2024, max compression
+gzip compressed data, was "/Users/dialidsantiago/Git/aleatory/dist/.tmp-x2_i0bwl/aleatory-0.3.0.tar", last modified: Fri Apr 19 20:10:55 2024, max compression
```

## Comparing `aleatory-0.2.0.tar` & `aleatory-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.946803 aleatory-0.2.0/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1072 2024-01-14 16:48:38.000000 aleatory-0.2.0/LICENSE
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3935 2024-01-14 16:55:22.946137 aleatory-0.2.0/PKG-INFO
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3020 2023-12-28 16:28:21.000000 aleatory-0.2.0/README.md
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.919530 aleatory-0.2.0/aleatory/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.2.0/aleatory/__init__.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.922953 aleatory-0.2.0/aleatory/processes/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      529 2024-01-13 23:20:51.000000 aleatory-0.2.0/aleatory/processes/__init__.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.929134 aleatory-0.2.0/aleatory/processes/analytical/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.2.0/aleatory/processes/analytical/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     6191 2024-01-08 21:57:15.000000 aleatory-0.2.0/aleatory/processes/analytical/bes.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5094 2024-01-08 21:57:20.000000 aleatory-0.2.0/aleatory/processes/analytical/besq.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5723 2024-01-07 16:45:04.000000 aleatory-0.2.0/aleatory/processes/analytical/brownian_motion.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     2064 2022-12-23 20:21:22.000000 aleatory-0.2.0/aleatory/processes/analytical/gaussian.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5062 2022-12-25 17:41:15.000000 aleatory-0.2.0/aleatory/processes/analytical/geometric_brownian.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     6430 2024-01-07 20:25:27.000000 aleatory-0.2.0/aleatory/processes/base.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.935330 aleatory-0.2.0/aleatory/processes/euler_maruyama/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.2.0/aleatory/processes/euler_maruyama/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5260 2023-04-29 10:54:19.000000 aleatory-0.2.0/aleatory/processes/euler_maruyama/cev_process.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5400 2023-06-10 09:19:44.000000 aleatory-0.2.0/aleatory/processes/euler_maruyama/cir_process.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1638 2022-12-25 18:20:27.000000 aleatory-0.2.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3312 2023-11-12 09:39:52.000000 aleatory-0.2.0/aleatory/processes/euler_maruyama/vasicek.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.937713 aleatory-0.2.0/aleatory/stats/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      427 2024-01-14 14:32:19.000000 aleatory-0.2.0/aleatory/stats/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4174 2024-01-14 14:26:45.000000 aleatory-0.2.0/aleatory/stats/non_central_chi.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.939097 aleatory-0.2.0/aleatory/utils/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.2.0/aleatory/utils/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     8789 2024-01-08 22:30:17.000000 aleatory-0.2.0/aleatory/utils/utils.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.945486 aleatory-0.2.0/aleatory.egg-info/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3935 2024-01-14 16:55:22.000000 aleatory-0.2.0/aleatory.egg-info/PKG-INFO
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1008 2024-01-14 16:55:22.000000 aleatory-0.2.0/aleatory.egg-info/SOURCES.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        1 2024-01-14 16:55:22.000000 aleatory-0.2.0/aleatory.egg-info/dependency_links.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      100 2024-01-14 16:55:22.000000 aleatory-0.2.0/aleatory.egg-info/requires.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        9 2024-01-14 16:55:22.000000 aleatory-0.2.0/aleatory.egg-info/top_level.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1008 2024-01-14 16:49:45.000000 aleatory-0.2.0/pyproject.toml
--rw-r--r--   0 dialidsantiago   (501) staff       (20)       38 2024-01-14 16:55:22.946963 aleatory-0.2.0/setup.cfg
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-01-14 16:55:22.944627 aleatory-0.2.0/tests/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4683 2024-01-08 22:41:25.000000 aleatory-0.2.0/tests/test_bes.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5852 2023-12-29 20:00:28.000000 aleatory-0.2.0/tests/test_charts.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      656 2024-01-11 14:27:54.000000 aleatory-0.2.0/tests/test_marginal_functions.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1616 2024-01-11 16:02:20.000000 aleatory-0.2.0/tests/test_ncx.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      258 2022-12-25 12:07:25.000000 aleatory-0.2.0/tests/test_transormation_em.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.770718 aleatory-0.3.0/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1090 2024-04-19 18:45:58.000000 aleatory-0.3.0/LICENSE
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4101 2024-04-19 20:10:55.769810 aleatory-0.3.0/PKG-INFO
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3186 2024-04-19 18:45:32.000000 aleatory-0.3.0/README.md
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.716492 aleatory-0.3.0/aleatory/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/__init__.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.721969 aleatory-0.3.0/aleatory/processes/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      756 2024-04-12 13:11:57.000000 aleatory-0.3.0/aleatory/processes/__init__.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.743036 aleatory-0.3.0/aleatory/processes/analytical/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/processes/analytical/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6191 2024-01-08 21:57:15.000000 aleatory-0.3.0/aleatory/processes/analytical/bes.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5094 2024-01-08 21:57:20.000000 aleatory-0.3.0/aleatory/processes/analytical/besq.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6085 2024-04-19 19:37:07.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_bridge.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2643 2024-04-19 18:36:09.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_excursion.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4335 2024-04-19 19:37:27.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_meander.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5740 2024-04-19 15:25:01.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_motion.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2064 2024-04-08 15:35:51.000000 aleatory-0.3.0/aleatory/processes/analytical/gaussian.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5062 2022-12-25 17:41:15.000000 aleatory-0.3.0/aleatory/processes/analytical/geometric_brownian.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6430 2024-04-12 14:05:19.000000 aleatory-0.3.0/aleatory/processes/base.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.753609 aleatory-0.3.0/aleatory/processes/euler_maruyama/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5260 2023-04-29 10:54:19.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/cev_process.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5400 2023-06-10 09:19:44.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/cir_process.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1638 2022-12-25 18:20:27.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3312 2023-11-12 09:39:52.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/vasicek.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.757083 aleatory-0.3.0/aleatory/stats/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      427 2024-01-14 14:32:19.000000 aleatory-0.3.0/aleatory/stats/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4174 2024-01-14 14:26:45.000000 aleatory-0.3.0/aleatory/stats/non_central_chi.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.759317 aleatory-0.3.0/aleatory/utils/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/utils/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)    10659 2024-04-19 18:15:19.000000 aleatory-0.3.0/aleatory/utils/utils.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.768791 aleatory-0.3.0/aleatory.egg-info/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4101 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/PKG-INFO
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1159 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/SOURCES.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        1 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/dependency_links.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      100 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/requires.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        9 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/top_level.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1008 2024-04-19 18:44:34.000000 aleatory-0.3.0/pyproject.toml
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)       38 2024-04-19 20:10:55.770917 aleatory-0.3.0/setup.cfg
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.767421 aleatory-0.3.0/tests/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4683 2024-01-08 22:41:25.000000 aleatory-0.3.0/tests/test_bes.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6644 2024-04-19 19:54:54.000000 aleatory-0.3.0/tests/test_charts.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      656 2024-01-11 14:27:54.000000 aleatory-0.3.0/tests/test_marginal_functions.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1616 2024-01-11 16:02:20.000000 aleatory-0.3.0/tests/test_ncx.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      258 2022-12-25 12:07:25.000000 aleatory-0.3.0/tests/test_transormation_em.py
```

### Comparing `aleatory-0.2.0/LICENSE` & `aleatory-0.3.0/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-2024 Quant Girl
+Copyright (c) 2022-2024 Dialid Santiago (Quant Girl)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aleatory-0.2.0/PKG-INFO` & `aleatory-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleatory
-Version: 0.2.0
+Version: 0.3.0
 Summary: Stochastic Processes Simulation and Visualisation
 Author-email: Dialid Santiago <d.santiago@outlook.com>
 Project-URL: Homepage, https://github.com/quantgirluk/aleatory
 Project-URL: Bug Tracker, https://github.com/quantgirluk/aleatory/issues
 Project-URL: Documentation, https://aleatory.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -36,22 +36,25 @@
 The **_aleatory_** (/ˈeɪliətəri/) Python library provides functionality for simulating and visualising
 stochastic processes. More precisely, it introduces objects representing a number of continuous-time
 stochastic processes $X = (X_t : t\geq 0)$ and provides methods to:
 
 - generate realizations/trajectories from each process —over discrete time sets
 - create visualisations to illustrate the processes properties and behaviour
 
-<figure>
-  <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"
-    width="900" height="450">
-</figure>
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
+</p>
 
 Currently, `aleatory` supports the following processes:
 
 - Brownian Motion
+- Brownian Bridge
+- Brownian Excursion
+- Brownian Meander
 - Geometric Brownian Motion
 - Ornstein–Uhlenbeck
 - Vasicek
 - Cox–Ingersoll–Ross
 - Constant Elasticity
 - Bessel Process
 - Squared Bessel Processs
@@ -89,24 +92,26 @@
 brownian = BrownianMotion()
 brownian.draw(n=100, N=100, colormap="cool", figsize=(12,9))
 
 ```
 
 generates a chart like this:
 
-<figure>
-  <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"
-    width="900" height="450">
-</figure>
+<p align="center">
+<img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
+</p>
+
+For more examples visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
 
-For more example visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
+
+⭐️ **If you like this project, please give it a star!** ⭐️
 
 ## Thanks for Visiting! ✨
 
 Connect with me via:
 
 - 🦜 [Twitter](https://twitter.com/Quant_Girl)
 - 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
 - 📸 [Instagram](https://www.instagram.com/quant_girl/)
 - 👾 [Personal Website](https://quantgirl.blog)
 
-⭐️ **If you like this projet, please give it a star!** ⭐️
+
```

### Comparing `aleatory-0.2.0/README.md` & `aleatory-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,25 @@
 The **_aleatory_** (/ˈeɪliətəri/) Python library provides functionality for simulating and visualising
 stochastic processes. More precisely, it introduces objects representing a number of continuous-time
 stochastic processes $X = (X_t : t\geq 0)$ and provides methods to:
 
 - generate realizations/trajectories from each process —over discrete time sets
 - create visualisations to illustrate the processes properties and behaviour
 
-<figure>
-  <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"
-    width="900" height="450">
-</figure>
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
+</p>
 
 Currently, `aleatory` supports the following processes:
 
 - Brownian Motion
+- Brownian Bridge
+- Brownian Excursion
+- Brownian Meander
 - Geometric Brownian Motion
 - Ornstein–Uhlenbeck
 - Vasicek
 - Cox–Ingersoll–Ross
 - Constant Elasticity
 - Bessel Process
 - Squared Bessel Processs
@@ -66,24 +69,26 @@
 brownian = BrownianMotion()
 brownian.draw(n=100, N=100, colormap="cool", figsize=(12,9))
 
 ```
 
 generates a chart like this:
 
-<figure>
-  <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"
-    width="900" height="450">
-</figure>
+<p align="center">
+<img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
+</p>
+
+For more examples visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
 
-For more example visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
+
+⭐️ **If you like this project, please give it a star!** ⭐️
 
 ## Thanks for Visiting! ✨
 
 Connect with me via:
 
 - 🦜 [Twitter](https://twitter.com/Quant_Girl)
 - 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
 - 📸 [Instagram](https://www.instagram.com/quant_girl/)
 - 👾 [Personal Website](https://quantgirl.blog)
 
-⭐️ **If you like this projet, please give it a star!** ⭐️
+
```

### Comparing `aleatory-0.2.0/aleatory/processes/__init__.py` & `aleatory-0.3.0/aleatory/processes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,7 +2,10 @@
 from aleatory.processes.euler_maruyama.ornstein_uhlenbeck import OUProcess
 from aleatory.processes.euler_maruyama.cir_process import CIRProcess
 from aleatory.processes.euler_maruyama.cev_process import CEVProcess
 from aleatory.processes.analytical.geometric_brownian import GBM
 from aleatory.processes.analytical.brownian_motion import BrownianMotion
 from aleatory.processes.analytical.bes import BESProcess
 from aleatory.processes.analytical.besq import BESQProcess
+from aleatory.processes.analytical.brownian_bridge import BrownianBridge
+from aleatory.processes.analytical.brownian_excursion import BrownianExcursion
+from aleatory.processes.analytical.brownian_meander import BrownianMeander
```

### Comparing `aleatory-0.2.0/aleatory/processes/analytical/bes.py` & `aleatory-0.3.0/aleatory/processes/analytical/bes.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/analytical/besq.py` & `aleatory-0.3.0/aleatory/processes/analytical/besq.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/analytical/brownian_motion.py` & `aleatory-0.3.0/aleatory/processes/analytical/brownian_motion.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
     .. math::
 
         X_t = x_0 +  \mu t + \sigma W_t \ \ \ \ t \in [0,T]
 
     and each :math:`X_t \sim N(\mu t, \sigma^2 t)`.
 
+    Parameters:
+
     :param float drift: the parameter :math:`\mu` in the above SDE
     :param float scale: the parameter :math:`\sigma>0` in the above SDE
     :param float initial: the initial condition :math:`x_0` in the above SDE
     :param float T: the right hand endpoint of the time interval :math:`[0,T]`
         for the process
     :param numpy.random.Generator rng: a custom random number generator
```

### Comparing `aleatory-0.2.0/aleatory/processes/analytical/gaussian.py` & `aleatory-0.3.0/aleatory/processes/analytical/gaussian.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/analytical/geometric_brownian.py` & `aleatory-0.3.0/aleatory/processes/analytical/geometric_brownian.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/base.py` & `aleatory-0.3.0/aleatory/processes/base.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/euler_maruyama/cev_process.py` & `aleatory-0.3.0/aleatory/processes/euler_maruyama/cev_process.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/euler_maruyama/cir_process.py` & `aleatory-0.3.0/aleatory/processes/euler_maruyama/cir_process.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py` & `aleatory-0.3.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/processes/euler_maruyama/vasicek.py` & `aleatory-0.3.0/aleatory/processes/euler_maruyama/vasicek.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/stats/non_central_chi.py` & `aleatory-0.3.0/aleatory/stats/non_central_chi.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/aleatory/utils/utils.py` & `aleatory-0.3.0/aleatory/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,100 +75,116 @@
                                    marginalT=marginalT,
                                    envelope=envelope,
                                    lower=lower, upper=upper, style=style, colormap=colormap, **fig_kw)
     else:
         raise ValueError('orientation can only take values horizontal, vertical')
 
 
-def draw_paths_horizontal(times, paths, N, expectations, title=None, KDE=False, marginal=False, marginalT=None,
+def draw_paths_horizontal(times, paths, N, expectations=None, title=None, KDE=False, marginal=False, marginalT=None,
                           envelope=False,
-                          lower=None, upper=None, style="seaborn-v0_8-whitegrid", colormap="RdYlBu_r", **fig_kw):
+                          lower=None, upper=None,
+                          style="seaborn-v0_8-whitegrid", colormap="RdYlBu_r", colorspos=None,
+                          **fig_kw):
+    cm = plt.colormaps[colormap]
+    last_points = [path[-1] for path in paths]
+    n_bins = int(np.sqrt(N))
+    col = np.linspace(0, 1, n_bins, endpoint=True)
+
     with plt.style.context(style):
         if marginal:
             fig = plt.figure(**fig_kw)
             gs = GridSpec(1, 5)
             ax1 = fig.add_subplot(gs[:4])
             ax2 = fig.add_subplot(gs[4:], sharey=ax1)
 
-            last_points = [path[-1] for path in paths]
-            cm = plt.colormaps[colormap]
-            n_bins = int(np.sqrt(N))
             n, bins, patches = ax2.hist(last_points, n_bins, orientation='horizontal', density=True)
-            col = np.linspace(0, 1, n_bins, endpoint=True)
             for c, p in zip(col, patches):
                 plt.setp(p, 'facecolor', cm(c))
             my_bins = pd.cut(last_points, bins=bins, labels=range(len(bins) - 1), include_lowest=True)
             colors = [col[b] for b in my_bins]
 
             if KDE:
                 kde = sm.nonparametric.KDEUnivariate(last_points)
                 kde.fit()  # Estimate the densities
                 ax2.plot(kde.density, kde.support, '--', lw=1.75, alpha=0.6, label='$X_T$  KDE', zorder=10)
                 ax2.axhline(y=np.mean(last_points), linestyle='--', lw=1.75, label=r'$\overline{X_T}$')
-            else:
+            elif marginal and marginalT:
                 marginaldist = marginalT
                 x = np.linspace(marginaldist.ppf(0.001), marginaldist.ppf(0.999), 100)
                 ax2.plot(marginaldist.pdf(x), x, '-', lw=1.75, alpha=0.6, label='$X_T$ pdf')
                 ax2.axhline(y=marginaldist.mean(), linestyle='--', lw=1.75, label='$E[X_T]$')
 
             plt.setp(ax2.get_yticklabels(), visible=False)
             ax2.set_title('$X_T$')
             ax2.legend()
 
             for i in range(N):
                 ax1.plot(times, paths[i], '-', lw=1.0, color=cm(colors[i]))
-            ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
+
+            if expectations is not None:
+                ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
+                ax1.legend()
             if envelope:
                 ax1.fill_between(times, upper, lower, alpha=0.25, color='grey')
             plt.subplots_adjust(wspace=0.025, hspace=0.025)
 
         else:
             fig, ax1 = plt.subplots(**fig_kw)
-            for i in range(N):
-                ax1.plot(times, paths[i], '-', lw=1.0)
-            ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
+            if colorspos:
+                colors = [path[colorspos]/np.max(np.abs(path)) for path in paths]
+            else:
+                _, bins = np.histogram(last_points, n_bins)
+                my_bins = pd.cut(last_points, bins=bins, labels=range(len(bins) - 1), include_lowest=True)
+                colors = [col[b] for b in my_bins]
+
+            for path, color in zip(paths,colors):
+                ax1.plot(times, path, '-',  color=cm(color), lw=0.75)
+            if expectations is not None:
+                ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
+                ax1.legend()
             if envelope:
                 ax1.fill_between(times, upper, lower, color='grey', alpha=0.25)
 
         fig.suptitle(title)
         ax1.set_title(r'Simulated Paths $X_t, t \in [t_0, T]$')  # Title
         ax1.set_xlabel('$t$')
         ax1.set_ylabel('$X(t)$')
-        ax1.legend()
         plt.show()
 
     return fig
 
 
 def draw_paths_vertical(times, paths, N, expectations, title=None, KDE=False, marginal=False, marginalT=None,
                         envelope=False,
                         lower=None, upper=None, style="seaborn-v0_8-whitegrid", colormap="RdYlBu_r", **fig_kw):
     with plt.style.context(style):
+
+        cm = plt.colormaps[colormap]
+        last_points = [path[-1] for path in paths]
+        n_bins = int(np.sqrt(N))
+        col = np.linspace(0, 1, n_bins, endpoint=True)
+
         if marginal:
             fig = plt.figure(**fig_kw)
             gs = GridSpec(1, 7)
             ax1 = fig.add_subplot(gs[:4])
             ax2 = fig.add_subplot(gs[4:])
 
-            last_points = [path[-1] for path in paths]
-            cm = plt.colormaps[colormap]
-            n_bins = int(np.sqrt(N))
             n, bins, patches = ax2.hist(last_points, n_bins, orientation='vertical', density=True)
-            col = np.linspace(0, 1, n_bins, endpoint=True)
             for c, p in zip(col, patches):
                 plt.setp(p, 'facecolor', cm(c))
             my_bins = pd.cut(last_points, bins=bins, labels=range(len(bins) - 1), include_lowest=True)
             colors = [col[b] for b in my_bins]
 
             if KDE:
                 kde = sm.nonparametric.KDEUnivariate(last_points)
                 kde.fit()  # Estimate the densities
                 ax2.plot(kde.support, kde.density, '--', lw=1.75, alpha=0.6, label='$X_T$  KDE', zorder=10)
                 ax2.axvline(x=np.mean(last_points), linestyle='--', lw=1.75, label=r'$\overline{X_T}$')
-            else:
+            elif marginal and marginalT:
                 marginaldist = marginalT
                 x = np.linspace(marginaldist.ppf(0.001), marginaldist.ppf(0.999), 100)
                 ax2.plot(x, marginaldist.pdf(x), '-', lw=1.75, alpha=0.6, label='$X_T$ pdf')
                 ax2.axvline(x=marginaldist.mean(), linestyle='--', lw=1.75, label='$E[X_T]$')
 
             ax2.set_title('$X_T$')
             ax2.legend()
@@ -177,31 +193,64 @@
             for i in range(N):
                 ax1.plot(times, paths[i], '-', lw=1.0, color=cm(colors[i]))
             ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
             if envelope:
                 ax1.fill_between(times, upper, lower, alpha=0.25, color='grey')
 
         else:
+            _, bins = np.histogram(last_points, n_bins)
+            my_bins = pd.cut(last_points, bins=bins, labels=range(len(bins) - 1), include_lowest=True)
+            colors = [col[b] for b in my_bins]
+
             fig, ax1 = plt.subplots(**fig_kw)
             for i in range(N):
-                ax1.plot(times, paths[i], '-', lw=1.0)
+                ax1.plot(times, paths[i], '-', color=cm(colors[i]), lw=1.0)
             ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
             if envelope:
                 ax1.fill_between(times, upper, lower, color='grey', alpha=0.25)
 
         fig.suptitle(title)
         ax1.set_title(r'Simulated Paths $X_t, t \in [t_0, T]$')  # Title
         ax1.set_xlabel('$t$')
         ax1.set_ylabel('$X(t)$')
         ax1.legend()
         plt.show()
 
     return fig
 
 
+def draw_paths_with_end_point(times, paths, expectations=None, title=None, envelope=False,
+                          lower=None, upper=None,
+                          style="seaborn-v0_8-whitegrid", colormap="RdYlBu_r",
+                          **fig_kw):
+
+    cm = plt.colormaps[colormap]
+    mid = int(len(paths[0])/2)+1
+
+    with plt.style.context(style):
+
+        fig, ax1 = plt.subplots(**fig_kw)
+        for path in paths:
+            ax1.plot(times, path, '-',  color=cm(path[mid]/np.max(np.abs(path))), lw=0.75)
+        if expectations is not None:
+            ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
+            ax1.legend()
+
+        lower_and_upper_provided = lower is not None and upper is not None
+        if envelope and lower_and_upper_provided:
+            ax1.fill_between(times, upper, lower, color='grey', alpha=0.25)
+
+        fig.suptitle(title)
+        ax1.set_title(r'Simulated Paths $X_t, t \in [t_0, T]$')  # Title
+        ax1.set_xlabel('$t$')
+        ax1.set_ylabel('$X(t)$')
+        plt.show()
+
+    return fig
+
 def sample_besselq_global(T, initial, dim, n):
     t_size = T / n
     path = np.zeros(n)
     path[0] = initial
     x = initial
     for t in range(n - 1):
         sample = ncx2(df=dim, nc=x / t_size, scale=t_size).rvs(1)[0]
```

### Comparing `aleatory-0.2.0/aleatory.egg-info/PKG-INFO` & `aleatory-0.3.0/aleatory.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleatory
-Version: 0.2.0
+Version: 0.3.0
 Summary: Stochastic Processes Simulation and Visualisation
 Author-email: Dialid Santiago <d.santiago@outlook.com>
 Project-URL: Homepage, https://github.com/quantgirluk/aleatory
 Project-URL: Bug Tracker, https://github.com/quantgirluk/aleatory/issues
 Project-URL: Documentation, https://aleatory.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -36,22 +36,25 @@
 The **_aleatory_** (/ˈeɪliətəri/) Python library provides functionality for simulating and visualising
 stochastic processes. More precisely, it introduces objects representing a number of continuous-time
 stochastic processes $X = (X_t : t\geq 0)$ and provides methods to:
 
 - generate realizations/trajectories from each process —over discrete time sets
 - create visualisations to illustrate the processes properties and behaviour
 
-<figure>
-  <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"
-    width="900" height="450">
-</figure>
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
+</p>
 
 Currently, `aleatory` supports the following processes:
 
 - Brownian Motion
+- Brownian Bridge
+- Brownian Excursion
+- Brownian Meander
 - Geometric Brownian Motion
 - Ornstein–Uhlenbeck
 - Vasicek
 - Cox–Ingersoll–Ross
 - Constant Elasticity
 - Bessel Process
 - Squared Bessel Processs
@@ -89,24 +92,26 @@
 brownian = BrownianMotion()
 brownian.draw(n=100, N=100, colormap="cool", figsize=(12,9))
 
 ```
 
 generates a chart like this:
 
-<figure>
-  <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"
-    width="900" height="450">
-</figure>
+<p align="center">
+<img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
+</p>
+
+For more examples visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
 
-For more example visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
+
+⭐️ **If you like this project, please give it a star!** ⭐️
 
 ## Thanks for Visiting! ✨
 
 Connect with me via:
 
 - 🦜 [Twitter](https://twitter.com/Quant_Girl)
 - 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
 - 📸 [Instagram](https://www.instagram.com/quant_girl/)
 - 👾 [Personal Website](https://quantgirl.blog)
 
-⭐️ **If you like this projet, please give it a star!** ⭐️
+
```

### Comparing `aleatory-0.2.0/aleatory.egg-info/SOURCES.txt` & `aleatory-0.3.0/aleatory.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 aleatory.egg-info/requires.txt
 aleatory.egg-info/top_level.txt
 aleatory/processes/__init__.py
 aleatory/processes/base.py
 aleatory/processes/analytical/__init__.py
 aleatory/processes/analytical/bes.py
 aleatory/processes/analytical/besq.py
+aleatory/processes/analytical/brownian_bridge.py
+aleatory/processes/analytical/brownian_excursion.py
+aleatory/processes/analytical/brownian_meander.py
 aleatory/processes/analytical/brownian_motion.py
 aleatory/processes/analytical/gaussian.py
 aleatory/processes/analytical/geometric_brownian.py
 aleatory/processes/euler_maruyama/__init__.py
 aleatory/processes/euler_maruyama/cev_process.py
 aleatory/processes/euler_maruyama/cir_process.py
 aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
```

### Comparing `aleatory-0.2.0/pyproject.toml` & `aleatory-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aleatory"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{ name = "Dialid Santiago", email = "d.santiago@outlook.com" }, ]
 description = "Stochastic Processes Simulation and Visualisation"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["pandas>=1.5.2",
                 "numpy>=1.23.5",
                 "scipy>=1.9.3",
```

### Comparing `aleatory-0.2.0/tests/test_bes.py` & `aleatory-0.3.0/tests/test_bes.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/tests/test_charts.py` & `aleatory-0.3.0/tests/test_charts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import matplotlib.figure
 import numpy as np
 
-from aleatory.processes import BrownianMotion, GBM, Vasicek, OUProcess, CIRProcess, CEVProcess, BESProcess, BESQProcess
+from aleatory.processes import (BrownianMotion, GBM, Vasicek, OUProcess, CIRProcess, CEVProcess, BESProcess,
+                                BESQProcess, BrownianBridge, BrownianExcursion, BrownianMeander)
 
 SAVE = False
 SAVE_PATH = '../docs/source/_static/'
 
 
 def test_sample(n=100):
     process = BrownianMotion()
@@ -35,44 +36,53 @@
 
     for v1, v2 in zip(sim1[0], sim2[0]):
         assert v1 == v2
 
 
 def test_figures_examples():
     bm = BrownianMotion()
+    bridge = BrownianBridge(initial=1.0, end=2.0)
+    excursion = BrownianExcursion()
+    meander = BrownianMeander()
+    meander_end = BrownianMeander(fixed_end=True, end=2.0)
+    meander_end_automatic = BrownianMeander(fixed_end=True)
     bmd = BrownianMotion(drift=-1.0, scale=0.5)
     gbm = GBM()
     vasicek = Vasicek()
     ouprocess = OUProcess()
     cirprocess = CIRProcess()
     cev = CEVProcess()
     bes = BESProcess(dim=10)
     bes_float = BESProcess(dim=4.5)
     besq = BESQProcess(dim=10)
     besq_float = BESQProcess(dim=3.5)
 
-    processes = [bm, bmd, gbm, vasicek, ouprocess, cirprocess, cev, bes, besq, bes_float, besq_float]
+    processes = [bridge, excursion, meander, meander_end, meander_end_automatic]
+    # processes = [bm, bmd, bridge, excursion, meander, gbm, vasicek, ouprocess, cirprocess, cev, bes, besq, bes_float, besq_float]
     # [bm, besq_float, bes_float]
+    # processes = [gbm, vasicek, ouprocess, cirprocess, cev, bes, besq]
+    # processes = [bes_float, besq_float]
+    # processes = [bm, bmd, bridge, excursion, meander, meander_end]
     # [bm, bmd, gbm,  cirprocess, cev, bes, besq, bes_float, besq_float]
-
     style = "https://raw.githubusercontent.com/quantgirluk/matplotlib-stylesheets/main/quant-pastel-light.mplstyle"
     # with plt.style.context(style):
     for process in processes:
-        # process.plot(n=100, N=5, figsize=(9.5, 6), dpi=200)
+        process.plot(n=100, N=5, figsize=(9.5, 6), dpi=200)
         # process.plot(n=100, N=5, title='My favourite figure', figsize=(9.5, 6), dpi=200)  # figure_with_title
         #
-        # name = process.name.replace(" ", "_").lower()
-        # if SAVE:
-        #     figure = process.plot(n=100, N=5, figsize=(9.5, 6), dpi=200)
-        #     figure.savefig(SAVE_PATH + name + '_simple_plot.png')
-        #     figure = process.draw(n=100, N=200, figsize=(12, 6), dpi=200)
-        #     figure.savefig(SAVE_PATH + name + '_drawn.png')
-
-        process.draw(n=100, N=100, figsize=(12, 6), dpi=200)
-        # process.draw(n=100, N=200, envelope=False, orientation='horizontal')
+        name = process.name.replace(" ", "_").lower()
+        if SAVE:
+            figure = process.plot(n=100, N=5, figsize=(9.5, 6), dpi=200)
+            figure.savefig(SAVE_PATH + name + '_simple_plot.png')
+            figure = process.draw(n=100, N=200, figsize=(10, 6), dpi=200, colormap="spring")
+            figure.savefig(SAVE_PATH + name + '_drawn.png')
+
+        process.draw(n=100, N=200, figsize=(10, 6), dpi=200, colormap="spring", envelope=False, marginal=True)
+        # process.draw(n=100, N=200, figsize=(10, 6), dpi=200, colormap="spring", envelope=True, marginal=True)
+        # process.draw(n=100, N=200, envelope=False, dpi=200, orientation='horizontal')
         # process.draw(n=100, N=250, envelope=False, orientation='vertical', figsize=(12, 6))
         # process.draw(n=100, N=250, envelope=True, orientation='vertical', figsize=(12, 6), style=style)
         # process.draw(n=100, N=250, envelope=True, orientation='horizontal', figsize=(12, 6), style=style)
         # process.draw(n=100, N=1, envelope=False, figsize=(12, 6),)
         # process.draw(n=100, N=2, envelope=False, figsize=(12, 6), dpi=200)
         # process.draw(n=100, N=3, envelope=False, figsize=(12, 6))
         # process.draw(n=100, N=3, envelope=False, orientation='vertical', figsize=(12, 6))
```

### Comparing `aleatory-0.2.0/tests/test_marginal_functions.py` & `aleatory-0.3.0/tests/test_marginal_functions.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.2.0/tests/test_ncx.py` & `aleatory-0.3.0/tests/test_ncx.py`

 * *Files identical despite different names*

