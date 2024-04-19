# Comparing `tmp/luma-ml-0.6.6.tar.gz` & `tmp/luma-ml-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.6.6.tar", last modified: Sun Apr 14 08:07:54 2024, max compression
+gzip compressed data, was "luma-ml-0.7.0.tar", last modified: Fri Apr 19 13:30:16 2024, max compression
```

## Comparing `luma-ml-0.6.6.tar` & `luma-ml-0.7.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.809416 luma-ml-0.6.6/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.6.6/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5553 2024-04-14 08:07:54.809083 luma-ml-0.6.6/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4947 2024-04-14 08:05:18.000000 luma-ml-0.6.6/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.787294 luma-ml-0.6.6/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)     9858 2024-04-14 08:03:23.000000 luma-ml-0.6.6/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.6.6/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.789537 luma-ml-0.6.6/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12269 2024-04-04 10:30:54.000000 luma-ml-0.6.6/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7627 2024-04-04 10:35:57.000000 luma-ml-0.6.6/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5539 2024-04-04 10:36:09.000000 luma-ml-0.6.6/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8951 2024-04-04 10:36:38.000000 luma-ml-0.6.6/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8854 2024-04-04 18:17:19.000000 luma-ml-0.6.6/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9534 2024-04-04 10:37:54.000000 luma-ml-0.6.6/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.794968 luma-ml-0.6.6/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17258 2024-04-04 10:38:24.000000 luma-ml-0.6.6/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17399 2024-04-04 10:39:29.000000 luma-ml-0.6.6/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7670 2024-04-04 10:39:48.000000 luma-ml-0.6.6/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17693 2024-04-04 10:41:26.000000 luma-ml-0.6.6/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8017 2024-04-04 11:10:57.000000 luma-ml-0.6.6/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11402 2024-04-04 11:13:10.000000 luma-ml-0.6.6/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.795715 luma-ml-0.6.6/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5248 2024-04-14 08:02:38.000000 luma-ml-0.6.6/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-04-11 15:05:45.000000 luma-ml-0.6.6/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10620 2024-04-14 08:01:24.000000 luma-ml-0.6.6/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.797551 luma-ml-0.6.6/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9715 2024-04-04 11:13:31.000000 luma-ml-0.6.6/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19224 2024-04-04 11:16:30.000000 luma-ml-0.6.6/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9631 2024-04-04 11:17:33.000000 luma-ml-0.6.6/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13548 2024-04-04 11:17:49.000000 luma-ml-0.6.6/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6479 2024-04-04 11:18:40.000000 luma-ml-0.6.6/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.798031 luma-ml-0.6.6/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.6.6/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14236 2024-04-14 07:13:23.000000 luma-ml-0.6.6/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.798731 luma-ml-0.6.6/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1471 2024-03-17 17:44:55.000000 luma-ml-0.6.6/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5709 2024-03-17 18:40:44.000000 luma-ml-0.6.6/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1551 2024-03-19 13:36:06.000000 luma-ml-0.6.6/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1646 2024-03-19 16:59:18.000000 luma-ml-0.6.6/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.798893 luma-ml-0.6.6/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.6.6/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.800062 luma-ml-0.6.6/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3267 2024-04-04 17:34:24.000000 luma-ml-0.6.6/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7679 2024-04-04 17:35:02.000000 luma-ml-0.6.6/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11844 2024-04-11 14:17:07.000000 luma-ml-0.6.6/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3472 2024-04-12 16:33:14.000000 luma-ml-0.6.6/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.800773 luma-ml-0.6.6/luma/neural/
--rw-r--r--   0 chanlee    (501) staff       (20)     1891 2024-04-04 11:21:05.000000 luma-ml-0.6.6/luma/neural/activation.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16698 2024-04-14 08:07:19.000000 luma-ml-0.6.6/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19581 2024-04-14 08:02:42.000000 luma-ml-0.6.6/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8208 2024-04-11 14:52:27.000000 luma-ml-0.6.6/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.800955 luma-ml-0.6.6/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7217 2024-04-11 12:45:03.000000 luma-ml-0.6.6/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.801658 luma-ml-0.6.6/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5293 2024-04-10 12:13:12.000000 luma-ml-0.6.6/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5531 2024-04-10 12:30:21.000000 luma-ml-0.6.6/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3600 2024-04-10 19:13:28.000000 luma-ml-0.6.6/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2553 2024-04-11 08:17:54.000000 luma-ml-0.6.6/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.802474 luma-ml-0.6.6/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18446 2024-04-04 11:25:12.000000 luma-ml-0.6.6/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39139 2024-04-04 15:10:56.000000 luma-ml-0.6.6/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16170 2024-04-05 18:23:54.000000 luma-ml-0.6.6/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.804458 luma-ml-0.6.6/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19091 2024-04-06 10:17:17.000000 luma-ml-0.6.6/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12178 2024-04-07 16:01:11.000000 luma-ml-0.6.6/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6636 2024-04-07 19:41:56.000000 luma-ml-0.6.6/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2960 2024-04-07 20:18:45.000000 luma-ml-0.6.6/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10678 2024-04-08 19:03:59.000000 luma-ml-0.6.6/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7486 2024-04-10 11:10:31.000000 luma-ml-0.6.6/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7187 2024-04-10 11:41:01.000000 luma-ml-0.6.6/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.806152 luma-ml-0.6.6/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.6.6/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24471 2024-04-13 15:18:20.000000 luma-ml-0.6.6/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.807349 luma-ml-0.6.6/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5553 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1614 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-14 08:07:54.809499 luma-ml-0.6.6/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-14 08:07:32.000000 luma-ml-0.6.6/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.808463 luma-ml-0.6.6/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-03-30 12:09:50.000000 luma-ml-0.6.6/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2085 2024-04-14 07:50:54.000000 luma-ml-0.6.6/test/_mlp_clf.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2220 2024-04-14 08:01:16.000000 luma-ml-0.6.6/test/_mlp_reg.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1200 2024-04-14 07:04:45.000000 luma-ml-0.6.6/test/_opt.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.188654 luma-ml-0.7.0/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.0/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-19 13:30:16.188345 luma-ml-0.7.0/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-04-19 13:29:32.000000 luma-ml-0.7.0/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.165301 luma-ml-0.7.0/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10173 2024-04-18 20:22:41.000000 luma-ml-0.7.0/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.0/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.168248 luma-ml-0.7.0/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12269 2024-04-04 10:30:54.000000 luma-ml-0.7.0/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7627 2024-04-04 10:35:57.000000 luma-ml-0.7.0/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5539 2024-04-04 10:36:09.000000 luma-ml-0.7.0/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8951 2024-04-04 10:36:38.000000 luma-ml-0.7.0/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8854 2024-04-04 18:17:19.000000 luma-ml-0.7.0/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9534 2024-04-04 10:37:54.000000 luma-ml-0.7.0/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.170910 luma-ml-0.7.0/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17258 2024-04-04 10:38:24.000000 luma-ml-0.7.0/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17399 2024-04-04 10:39:29.000000 luma-ml-0.7.0/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7670 2024-04-04 10:39:48.000000 luma-ml-0.7.0/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17693 2024-04-04 10:41:26.000000 luma-ml-0.7.0/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8017 2024-04-04 11:10:57.000000 luma-ml-0.7.0/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11402 2024-04-04 11:13:10.000000 luma-ml-0.7.0/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.171949 luma-ml-0.7.0/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5248 2024-04-14 08:02:38.000000 luma-ml-0.7.0/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-04-18 09:50:34.000000 luma-ml-0.7.0/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11480 2024-04-18 20:49:42.000000 luma-ml-0.7.0/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.174458 luma-ml-0.7.0/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9715 2024-04-04 11:13:31.000000 luma-ml-0.7.0/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19224 2024-04-04 11:16:30.000000 luma-ml-0.7.0/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9631 2024-04-04 11:17:33.000000 luma-ml-0.7.0/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13548 2024-04-04 11:17:49.000000 luma-ml-0.7.0/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6479 2024-04-04 11:18:40.000000 luma-ml-0.7.0/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.175138 luma-ml-0.7.0/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.0/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17510 2024-04-19 13:20:09.000000 luma-ml-0.7.0/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.175994 luma-ml-0.7.0/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1471 2024-03-17 17:44:55.000000 luma-ml-0.7.0/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5709 2024-03-17 18:40:44.000000 luma-ml-0.7.0/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1551 2024-03-19 13:36:06.000000 luma-ml-0.7.0/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1646 2024-03-19 16:59:18.000000 luma-ml-0.7.0/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.176172 luma-ml-0.7.0/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.0/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.178227 luma-ml-0.7.0/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3267 2024-04-04 17:34:24.000000 luma-ml-0.7.0/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7679 2024-04-04 17:35:02.000000 luma-ml-0.7.0/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11844 2024-04-11 14:17:07.000000 luma-ml-0.7.0/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5219 2024-04-18 21:02:26.000000 luma-ml-0.7.0/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.179628 luma-ml-0.7.0/luma/neural/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1387 2024-04-18 21:57:58.000000 luma-ml-0.7.0/luma/neural/activation.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    20652 2024-04-19 13:30:12.000000 luma-ml-0.7.0/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      669 2024-04-18 23:27:35.000000 luma-ml-0.7.0/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16728 2024-04-18 19:59:40.000000 luma-ml-0.7.0/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    20833 2024-04-18 21:58:02.000000 luma-ml-0.7.0/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8208 2024-04-11 14:52:27.000000 luma-ml-0.7.0/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.179840 luma-ml-0.7.0/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7217 2024-04-11 12:45:03.000000 luma-ml-0.7.0/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.180544 luma-ml-0.7.0/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5293 2024-04-10 12:13:12.000000 luma-ml-0.7.0/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5531 2024-04-10 12:30:21.000000 luma-ml-0.7.0/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3600 2024-04-10 19:13:28.000000 luma-ml-0.7.0/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2553 2024-04-18 16:23:01.000000 luma-ml-0.7.0/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.181791 luma-ml-0.7.0/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18446 2024-04-04 11:25:12.000000 luma-ml-0.7.0/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39139 2024-04-04 15:10:56.000000 luma-ml-0.7.0/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16170 2024-04-05 18:23:54.000000 luma-ml-0.7.0/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.183678 luma-ml-0.7.0/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19091 2024-04-06 10:17:17.000000 luma-ml-0.7.0/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12178 2024-04-07 16:01:11.000000 luma-ml-0.7.0/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6636 2024-04-07 19:41:56.000000 luma-ml-0.7.0/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2960 2024-04-07 20:18:45.000000 luma-ml-0.7.0/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10678 2024-04-08 19:03:59.000000 luma-ml-0.7.0/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7486 2024-04-10 11:10:31.000000 luma-ml-0.7.0/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7187 2024-04-10 11:41:01.000000 luma-ml-0.7.0/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.184321 luma-ml-0.7.0/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.0/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24471 2024-04-13 15:18:20.000000 luma-ml-0.7.0/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.186155 luma-ml-0.7.0/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1636 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-19 13:30:16.000000 luma-ml-0.7.0/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-19 13:30:16.188716 luma-ml-0.7.0/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-19 13:29:14.000000 luma-ml-0.7.0/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-19 13:30:16.187665 luma-ml-0.7.0/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-03-30 12:09:50.000000 luma-ml-0.7.0/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2005 2024-04-19 13:25:48.000000 luma-ml-0.7.0/test/__test.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2059 2024-04-18 22:07:38.000000 luma-ml-0.7.0/test/_mlp.py
```

### Comparing `luma-ml-0.6.6/LICENSE` & `luma-ml-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/PKG-INFO` & `luma-ml-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.6.6
+Version: 0.7.0
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.8k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.01k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.6</td>
+                    <td>0.7.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~16.3K</td>
+                    <td>~17.4K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.6.6 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.0 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.8k-red][GitHub code size in bytes][Code Style]
+5.01k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.6
-Lines of Code  ~16.3K
+Latest Version 0.7.0
+Lines of Code  ~17.4K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.6/README.md` & `luma-ml-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.8k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.01k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.6</td>
+                    <td>0.7.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~16.3K</td>
+                    <td>~17.4K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.8k-red][GitHub code size in bytes][Code Style]
+5.01k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.6
-Lines of Code  ~16.3K
+Latest Version 0.7.0
+Lines of Code  ~17.4K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.6/luma/__import__.py` & `luma-ml-0.7.0/luma/__import__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,21 @@
     UnsupportedParameterError,
     ModelExtensionError,
     InvalidRangeError,
 )
 from luma.interface.util import (
     Matrix,
     Vector,
+    Tensor,
     Scalar,
     DecisionTreeNode,
     NearestNeighbors,
 )
 from luma.interface.util import SilhouetteUtil, DBUtil, KernelUtil, ActivationUtil
-from luma.interface.util import Clone, ParamRange
+from luma.interface.util import Clone, ParamRange, Layer, Loss
 
 from luma.classifier.discriminant import (
     LDAClassifier,
     QDAClassifier,
     RDAClassifier,
     KDAClassifier,
 )
@@ -70,29 +71,31 @@
     AdaDeltaOptimizer,
     AdaMaxOptimizer,
     AdamWOptimizer,
     NAdamOptimizer,
 )
 from luma.neural.single import PerceptronClassifier, PerceptronRegressor
 from luma.neural.network import MLPClassifier, MLPRegressor
+from luma.neural.layer import Convolution, Pooling, Dense, Dropout, Flatten, Sequential
+from luma.neural.loss import CategoricalCrossEntropy
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
     MeanAbsolutePercentageError,
     RSquaredScore,
     AdjustedRSquaredScore,
 )
 from luma.metric.clustering import SilhouetteCoefficient, DaviesBouldin, Inertia
 from luma.metric.distance import Euclidean, Manhattan, Chebyshev, Minkowski
 from luma.metric.distance import CosineSimilarity, Correlation, Mahalanobis
 
-from luma.model_selection.split import TrainTestSplit
+from luma.model_selection.split import TrainTestSplit, BatchGenerator
 from luma.model_selection.search import GridSearchCV, RandomizedSearchCV
 from luma.model_selection.cv import CrossValidator
 from luma.model_selection.fold import KFold, StratifiedKFold
 
 from luma.preprocessing.scaler import StandardScaler, MinMaxScaler
 from luma.preprocessing.encoder import OneHotEncoder, LabelEncoder, OrdinalEncoder
 from luma.preprocessing.encoder import LabelBinarizer
@@ -159,17 +162,18 @@
     Supervised, Unsupervised, Distance
 
     # ----------------- [ luma.interface ] ---------------------
     NotFittedError, NotConvergedError,
     UnsupportedParameterError, ModelExtensionError,
     InvalidRangeError
 
-    Matrix, Vector, Scalar, DecisionTreeNode, NearestNeighbors,
+    Matrix, Vector, Tensor, Scalar,
+    DecisionTreeNode, NearestNeighbors,
     SilhouetteUtil, DBUtil, KernelUtil, ActivationUtil,
-    Clone, ParamRange
+    Clone, ParamRange, Layer, Loss
 
     # ----------------- [ luma.classifier ] --------------------
     LDAClassifier, QDAClassifier, RDAClassifier, KDAClassifier
 
     LogisticRegressor, SoftmaxRegressor
 
     GaussianNaiveBayes, BernoulliNaiveBayes
@@ -216,28 +220,32 @@
 
     ReLU, LeakyReLU, ELU, Tanh, Sigmoid, Softmax
 
     SGDOptimizer, MomentumOptimizer, RMSPropOptimizer,
     AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
     AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
+    Convolution, Pooling, Dense, Dropout, Flatten, Sequential
+
+    CategoricalCrossEntropy
+
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
     MeanAbsolutePercentageError, RSquaredScore,
     AdjustedRSquaredScore
 
     SilhouetteCoefficient, DaviesBouldin, Inertia
 
     Euclidean, Manhattan, Chebyshev, Minkowski,
     CosineSimilarity, Correlation, Mahalanobis
 
     # --------------- [ luma.module_selection ] ----------------
-    TrainTestSplit
+    TrainTestSplit, BatchGenerator
 
     GridSearchCV, RandomizedSearchCV
 
     CrossValidator
 
     KFold, StratifiedKFold
```

### Comparing `luma-ml-0.6.6/luma/__init__.py` & `luma-ml-0.7.0/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/classifier/discriminant.py` & `luma-ml-0.7.0/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/classifier/logistic.py` & `luma-ml-0.7.0/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/classifier/naive_bayes.py` & `luma-ml-0.7.0/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/classifier/neighbors.py` & `luma-ml-0.7.0/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/classifier/svm.py` & `luma-ml-0.7.0/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/classifier/tree.py` & `luma-ml-0.7.0/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/clustering/affinity.py` & `luma-ml-0.7.0/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/clustering/density.py` & `luma-ml-0.7.0/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/clustering/hierarchy.py` & `luma-ml-0.7.0/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/clustering/kmeans.py` & `luma-ml-0.7.0/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/clustering/mixture.py` & `luma-ml-0.7.0/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/clustering/spectral.py` & `luma-ml-0.7.0/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/core/base.py` & `luma-ml-0.7.0/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/core/super.py` & `luma-ml-0.7.0/luma/core/super.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,25 +81,38 @@
           estimators for improved performance or functionality. When
           integrating `TimeSeries` models with `Meta` estimators,
           special consideration is needed to ensure compatibility and
           effective integration.
 
         """
 
+    class NeuralNet:
+        """
+        An inner class of `Estimator` dedicated to neural networks.
+
+        Neural networks are computational models inspired by the human brain,
+        consisting of layers of interconnected nodes (neurons) that process
+        information through weighted connections. These models include an input
+        layer to receive data, hidden layers that perform computations, and an
+        output layer to deliver results.
+        """
+
+        def dump(self, **kwargs) -> None: ...
+
     @abstractmethod
     def fit(self, *args) -> Self: ...
 
     @abstractmethod
     def predict(self, *args) -> Any: ...
 
     @abstractmethod
     def score(self, *args) -> float: ...
 
-    def set_params(self, ignore_missing: bool = False, **kwargs) -> None:
-        return super().set_params(ignore_missing=ignore_missing, **kwargs)
+    def set_params(self, **kwargs) -> None:
+        return super().set_params(**kwargs)
 
     def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
         return super().set_param_ranges(range_dict)
 
     def check_param_ranges(self) -> None:
         return super().check_param_ranges()
 
@@ -203,16 +216,16 @@
 
     @abstractmethod
     def transform(self, *args) -> Any: ...
 
     @abstractmethod
     def fit_transform(self, *args) -> Any: ...
 
-    def set_params(self, ignore_missing: bool = False, **kwargs) -> None:
-        return super().set_params(ignore_missing=ignore_missing, **kwargs)
+    def set_params(self, **kwargs) -> None:
+        return super().set_params(**kwargs)
 
     def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
         return super().set_param_ranges(range_dict)
 
     def check_param_ranges(self) -> None:
         return super().check_param_ranges()
 
@@ -225,15 +238,15 @@
     fine-tuning machine learning models. It provides an abstract base for
     different optimization strategies, offering a standardized interface for
     systematically exploring and evaluating different combinations of model
     parameters.
 
     Properties
     ----------
-    Get the best(optimized) estimator or transformer:
+    Get the best(optimized) estimator or transformer (not for `Neural`):
     ```py
         @property
         def best_model(self) -> Estimator | Transformer
 
     """
 
     class Neural:
@@ -245,16 +258,27 @@
         For updating weights:
         ```py
         @abstractmethod
         def update(self, **kwargs) -> tuple
         ```
         """
 
-        @abstractmethod
-        def update(self, **kwargs) -> tuple: ...
+        def __init__(self) -> None:
+            self.updated_weights = None
+            self.updated_biases = None
+
+        def update(self, weights, biases, grad_weights, grad_biases) -> None:
+            if weights is not None:
+                self.updated_weights = self._update_weights(weights, grad_weights)
+            if biases is not None:
+                self.updated_biases = self._update_biases(biases, grad_biases)
+
+        def _update_weights(self) -> Any: ...
+
+        def _update_biases(self) -> Any: ...
 
     @property
     def best_model(self) -> Estimator | Transformer: ...
 
     def fit(self, **kwargs) -> Any:
         return super().fit(**kwargs)
```

### Comparing `luma-ml-0.6.6/luma/ensemble/bagging.py` & `luma-ml-0.7.0/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/ensemble/boost.py` & `luma-ml-0.7.0/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/ensemble/forest.py` & `luma-ml-0.7.0/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/ensemble/stack.py` & `luma-ml-0.7.0/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/ensemble/vote.py` & `luma-ml-0.7.0/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/interface/exception.py` & `luma-ml-0.7.0/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/interface/util.py` & `luma-ml-0.7.0/luma/interface/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,107 @@
-from typing import Any, AnyStr, Callable, Literal, Type, TypeGuard
+from typing import Any, AnyStr, Callable, Literal, Self, Tuple, Type, TypeGuard
 import numpy as np
 
 from luma.interface.exception import UnsupportedParameterError, InvalidRangeError
 from luma.neural import activation
 
 
 __all__ = (
     "Matrix",
     "Vector",
+    "Tensor",
     "Scalar",
     "DecisionTreeNode",
     "NearestNeighbors",
     "SilhouetteUtil",
     "DBUtil",
     "KernelUtil",
     "ActivationUtil",
     "Clone",
     "ParamRange",
+    "Layer",
+    "Loss",
 )
 
 
+type TensorLike = Matrix | Tensor | Vector
+
+
 class Matrix(np.ndarray):
     """
-    Internal class that extends `numpy.ndarray`.
+    Internal class for matrices(2D-array) that extends `numpy.ndarray`.
 
     This class provides a way to create matrix objects that have
     all the capabilities of numpy arrays with the potential for
     additional functionalities and readability.
 
     Example
     -------
     >>> m = Matrix([1, 2, 3])
     >>> isinstance(m, numpy.ndarray) # True
 
     """
 
-    def __new__(cls, array_like: Any) -> "Matrix":
+    def __new__(cls, array_like: Any) -> Self:
         if isinstance(array_like, (list, np.matrix)):
             obj = np.array(array_like)
         else:
             obj = array_like
         return obj
 
     def __array_finalize__(self, obj: np.ndarray | None) -> None:
         if obj is None:
             return
 
 
 class Vector(Matrix):
     """
-    Internal class for vector that extends `Matrix`.
+    Internal class for vectors(1D-array) that extends `Matrix`.
 
     This class represents a single row/column vector with its
     type of `numpy.ndarray` or `Matrix`.
 
     """
 
-    def __new__(cls, array_like: Any) -> "Vector":
+    def __new__(cls, array_like: Any) -> Self:
+        if isinstance(array_like, list):
+            obj = Matrix(array_like)
+        else:
+            obj = array_like
+        return obj
+
+
+class Tensor(Matrix):
+    """
+    Internal class for tensors(>=3D-arrray) that extends `Matrix`.
+
+    This class provides a way to create tensor objects that have
+    all the capabilities of numpy arrays with the potential for
+    additional functionalities and readability.
+    """
+
+    type Tensor_3D = "Tensor"
+    type Tensor_4D = "Tensor"
+
+    def __new__(cls, array_like: Any) -> Self:
         if isinstance(array_like, list):
             obj = Matrix(array_like)
         else:
             obj = array_like
         return obj
 
 
 class Scalar:
     """
     A placeholder class for scalar type.
 
     This class encompasses `int` and `float`.
     """
 
-    def __new__(cls, value: int | float) -> "Scalar":
+    def __new__(cls, value: int | float) -> Self:
         return float(value)
 
 
 class DecisionTreeNode:
     """
     Internal class for node used in tree-based models.
 
@@ -511,7 +537,99 @@
             return lambda x: lower < x < upper
         elif not lower_open and upper_open:
             return lambda x: lower <= x < upper
         elif not lower_open and not upper_open:
             return lambda x: lower <= x <= upper
         else:
             NotImplemented
+
+
+class Layer:
+    """
+    An internal class for layers in neural networks.
+
+    Neural network layers are composed of interconnected nodes,
+    each performing computations on input data. Common types include
+    fully connected, convolutional, and recurrent layers, each
+    serving distinct roles in learning from data.
+
+    Attributes
+    ----------
+    - `weights_` : Weight tensor
+    - `biases_` : Bias tensor
+    - `dX` : Gradient w.r.t. the input
+    - `dW` : Gradient w.r.t. the weights
+    - `dB` : Gradient w.r.t. the biases
+    - `optimizer` : Optimizer for certain layer
+    - `out_shape` : Shape of the output when forwarding
+
+    Properties
+    ----------
+    To get its parameter size (weights, biases):
+    ```py
+    (property) param_size: Tuple[int, int]
+    ```
+    """
+
+    def __init__(self) -> None:
+        self.input_: Tensor = None
+        self.weights_: Tensor = None
+        self.biases_: Vector = None
+
+        self.dX: Tensor = None
+        self.dW: Tensor = None
+        self.dB: Tensor = None
+
+        self.optimizer: object = None
+        self.out_shape: tuple = None
+
+    def forward(self) -> Tensor: ...
+
+    def backward(self) -> Tensor: ...
+
+    def update(self) -> None:
+        if self.optimizer is None:
+            return
+        weights_, biases_ = self.optimizer.update(
+            self.weights_, self.biases_, self.dW, self.dB
+        )
+        self.weights_ = Tensor(weights_)
+        self.biases_ = Tensor(biases_)
+
+    @property
+    def param_size(self) -> Tuple[int, int]:
+        w_size, b_size = 0, 0
+        if self.weights_ is not None:
+            w_size += len(self.weights_.flatten())
+        if self.biases_ is not None:
+            b_size += len(self.biases_.flatten())
+
+        return w_size, b_size
+
+    def __str__(self) -> str:
+        return type(self).__name__
+
+    def __repr__(self) -> str:
+        w_size, b_size = self.param_size
+        return (
+            f"{type(self).__name__}: "
+            + f"({w_size:,} weights, {b_size:,} biases)"
+            + f" -> {w_size + b_size:,} params"
+        )
+
+
+class Loss:
+    """
+    An internal class for loss functions used in neural networks.
+
+    Loss functions, integral to the training process of machine
+    learning models, serve as crucial metrics assessing the disparity
+    between predicted outcomes and ground truth labels. They play a
+    pivotal role in optimization algorithms, guiding parameter updates
+    towards minimizing the discrepancy between predictions and true values.
+    """
+
+    def __init__(self) -> None: ...
+
+    def loss(self) -> float: ...
+
+    def grad(self) -> Matrix: ...
```

### Comparing `luma-ml-0.6.6/luma/metric/classification.py` & `luma-ml-0.7.0/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/metric/clustering.py` & `luma-ml-0.7.0/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/metric/distance.py` & `luma-ml-0.7.0/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/metric/regression.py` & `luma-ml-0.7.0/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/migrate/port.py` & `luma-ml-0.7.0/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/model_selection/cv.py` & `luma-ml-0.7.0/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/model_selection/fold.py` & `luma-ml-0.7.0/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/model_selection/search.py` & `luma-ml-0.7.0/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/neural/network.py` & `luma-ml-0.7.0/luma/neural/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from luma.neural.activation import Softmax
 from luma.neural.optimizer import SGDOptimizer
 
 
 __all__ = ("MLPClassifier", "MLPRegressor")
 
 
-class MLPClassifier(Estimator, Supervised):
+class MLPClassifier(Estimator, Estimator.NeuralNet, Supervised):
     """
     An MLP (Multilayer Perceptron) is a type of neural network composed
     of one input layer, one or more hidden layers, and one output layer,
     with fully connected neurons. Each neuron uses a nonlinear activation
     function to allow the network to capture complex patterns in the data.
     MLPs are trained using backpropagation, where the network learns by
     adjusting weights to minimize the difference between its predictions
@@ -219,15 +219,15 @@
         dW += (self.lambda_ / m) * self.weights[-1]
         db = np.sum(delta, axis=0, keepdims=True) / m
         grad_weights.append(dW)
         grad_biases.append(db)
 
         for i in range(self.n_layers - 2, -1, -1):
             delta = np.dot(delta, self.weights[i + 1].T)
-            delta *= self.act_.derivative(as_[i + 1])
+            delta *= self.act_.grad(as_[i + 1])
 
             dW = np.dot(as_[i].T, delta)
             dW += (self.lambda_ / m) * self.weights[i]
             db = np.sum(delta, axis=0, keepdims=True) / m
 
             grad_weights.insert(0, dW)
             grad_biases.insert(0, db)
@@ -248,15 +248,15 @@
         return self._forward_pass(X)
 
     def score(self, X: Matrix, y: Matrix, metric: Evaluator = Accuracy) -> float:
         X_pred = self.predict(X)
         return metric.score(y_true=y, y_pred=X_pred)
 
 
-class MLPRegressor(Estimator, Supervised):
+class MLPRegressor(Estimator, Estimator.NeuralNet, Supervised):
     """
     Multilayer Perceptron for regression tasks. It employs a network similar
     to the MLP classifier, but the output layer uses a linear activation function
     to predict continuous values. The network is trained to minimize the mean
     squared error between the predicted and actual values.
 
     Parameters
@@ -443,15 +443,15 @@
         dW += (self.lambda_ / m) * self.weights[-1]
         db = np.sum(delta, axis=0, keepdims=True) / m
         grad_weights.append(dW)
         grad_biases.append(db)
 
         for i in range(self.n_layers - 2, -1, -1):
             delta = np.dot(delta, self.weights[i + 1].T)
-            delta *= self.act_.derivative(as_[i + 1])
+            delta *= self.act_.grad(as_[i + 1])
 
             dW = np.dot(as_[i].T, delta)
             dW += (self.lambda_ / m) * self.weights[i]
             db = np.sum(delta, axis=0, keepdims=True) / m
 
             grad_weights.insert(0, dW)
             grad_biases.insert(0, db)
```

### Comparing `luma-ml-0.6.6/luma/neural/single.py` & `luma-ml-0.7.0/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/pipe/pipeline.py` & `luma-ml-0.7.0/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/preprocessing/encoder.py` & `luma-ml-0.7.0/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/preprocessing/imputer.py` & `luma-ml-0.7.0/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/preprocessing/outlier.py` & `luma-ml-0.7.0/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/preprocessing/scaler.py` & `luma-ml-0.7.0/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/reduction/linear.py` & `luma-ml-0.7.0/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/reduction/manifold.py` & `luma-ml-0.7.0/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/reduction/selection.py` & `luma-ml-0.7.0/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/regressor/general.py` & `luma-ml-0.7.0/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/regressor/linear.py` & `luma-ml-0.7.0/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/regressor/neighbors.py` & `luma-ml-0.7.0/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/regressor/poly.py` & `luma-ml-0.7.0/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/regressor/robust.py` & `luma-ml-0.7.0/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/regressor/svm.py` & `luma-ml-0.7.0/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/regressor/tree.py` & `luma-ml-0.7.0/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/visual/eda.py` & `luma-ml-0.7.0/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma/visual/evaluation.py` & `luma-ml-0.7.0/luma/visual/evaluation.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.6/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.7.0/luma_ml.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.6.6
+Version: 0.7.0
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.8k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.01k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.6</td>
+                    <td>0.7.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~16.3K</td>
+                    <td>~17.4K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.6.6 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.0 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.8k-red][GitHub code size in bytes][Code Style]
+5.01k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.6
-Lines of Code  ~16.3K
+Latest Version 0.7.0
+Lines of Code  ~17.4K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.6/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.7.0/luma_ml.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 luma/metric/regression.py
 luma/migrate/port.py
 luma/model_selection/cv.py
 luma/model_selection/fold.py
 luma/model_selection/search.py
 luma/model_selection/split.py
 luma/neural/activation.py
+luma/neural/layer.py
+luma/neural/loss.py
 luma/neural/network.py
 luma/neural/optimizer.py
 luma/neural/single.py
 luma/pipe/pipeline.py
 luma/preprocessing/encoder.py
 luma/preprocessing/imputer.py
 luma/preprocessing/outlier.py
@@ -57,10 +59,9 @@
 luma/visual/evaluation.py
 luma_ml.egg-info/PKG-INFO
 luma_ml.egg-info/SOURCES.txt
 luma_ml.egg-info/dependency_links.txt
 luma_ml.egg-info/requires.txt
 luma_ml.egg-info/top_level.txt
 test/__local__.py
-test/_mlp_clf.py
-test/_mlp_reg.py
-test/_opt.py
+test/__test.py
+test/_mlp.py
```

### Comparing `luma-ml-0.6.6/setup.py` & `luma-ml-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.6.6",
+    version="0.7.0",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/LUMA",
     packages=setuptools.find_namespace_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.10",
+    python_requires=">=3.12",
     install_requires=["numpy", "scipy", "pandas", "matplotlib", "seaborn"],
 )
```

### Comparing `luma-ml-0.6.6/test/_mlp_clf.py` & `luma-ml-0.7.0/test/_mlp.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,13 @@
         mlp.batch_losses_, lw=0.5, label=f"{type(mlp.optimizer).__name__}", alpha=0.7
     )
 
 print(f"Best optimizer: {type(best_mlp.optimizer).__name__}")
 
 ax1.set_xlabel("Batches")
 ax1.set_ylabel("Loss")
-ax1.set_title(
-    f"MLP for Various Optimizers [Best Acc: {best_mlp.score(X_test, y_test):.4f}]"
-)
+ax1.set_title(f"MLP for Various Optimizers [Best Acc: {best_score:.4f}]")
 ax1.legend()
 ax1.grid(alpha=0.2)
 
 conf = ConfusionMatrix(y_all, best_mlp.predict(X_all))
 conf.plot(ax=ax2, show=True)
```

