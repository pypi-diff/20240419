# Comparing `tmp/quant2-0.1.5.tar.gz` & `tmp/quant2-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant2-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quant2-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quant2-0.1.5.tar` & `quant2-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.5/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.5/LICENSE
--rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.5/README.md
--rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.5/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
--rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.5/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
--rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.5/quant/README.md
--rw-r--r--   0        0        0      559 2024-04-17 08:12:03.953448 quant2-0.1.5/quant/__init__.py
--rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.5/quant/__main__.py
--rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.5/quant/evaluate/__init__.py
--rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.5/quant/evaluate/table20240326.py
--rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.5/quant/evaluate/utils.py
--rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.5/quant/football/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.5/quant/football/data/__init__.py
--rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.5/quant/football/data/dataset.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.5/quant/football/data/functional.py
--rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.5/quant/football/data/preprocessing.py
--rw-r--r--   0        0        0      993 2024-04-17 06:41:14.170874 quant2-0.1.5/quant/football/data/sampler.py
--rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.5/quant/football/data/stats.py
--rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.5/quant/football/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.5/quant/football/infer/__init__.py
--rw-r--r--   0        0        0     2024 2024-04-16 01:19:44.599739 quant2-0.1.5/quant/football/infer/fastapi_app.py
--rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.5/quant/football/infer/fastapi_app_test.py
--rw-r--r--   0        0        0     8033 2024-04-16 02:00:09.037054 quant2-0.1.5/quant/football/infer/football_infer_overunder_v1.py
--rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.5/quant/football/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.5/quant/football/models/mtnet.py
--rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.5/quant/football/models/stnet.py
--rw-r--r--   0        0        0      463 2024-04-15 20:54:36.028514 quant2-0.1.5/quant/football/transforms/__init__.py
--rw-r--r--   0        0        0     6622 2024-04-16 00:40:54.525920 quant2-0.1.5/quant/football/transforms/table20240326.py
--rw-r--r--   0        0        0     8541 2024-04-16 01:19:10.126956 quant2-0.1.5/quant/football/transforms/table20240410.py
--rw-r--r--   0        0        0     8825 2024-04-16 00:40:14.674251 quant2-0.1.5/quant/football/transforms/table20240414.py
--rw-r--r--   0        0        0     8396 2024-04-16 02:25:15.544645 quant2-0.1.5/quant/football/transforms/table20240415.py
--rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.5/quant/layers/__init__.py
--rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.5/quant/layers/layer_scale.py
--rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.5/quant/layers/mlp.py
--rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.5/quant/layers/normalization.py
--rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.5/quant/layers/swiglu_ffn.py
--rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.5/quant/utils/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.5/quant/utils/archive.py
--rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.5/quant/utils/config.py
--rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.5/quant/utils/io.py
--rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.5/quant/utils/logging.py
--rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.5/tests/football/data/test_utils.py
--rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.5/tools/analysis_tools/analyze_cls_results.py
--rw-r--r--   0        0        0     2645 2024-04-16 01:48:23.763355 quant2-0.1.5/tools/experimental/make_dataset.py
--rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.5/tools/experimental/make_split.py
--rw-r--r--   0        0        0     8078 2024-04-17 06:34:03.034798 quant2-0.1.5/tools/experimental/nni_football.py
--rw-r--r--   0        0        0      600 2024-04-17 07:13:13.694051 quant2-0.1.5/tools/experimental/nni_football_config.yaml
--rw-r--r--   0        0        0     1832 2024-04-17 08:12:07.193491 quant2-0.1.5/tools/experimental/nni_football_config_search_space.json
--rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.5/tools/experimental/nni_model.py
--rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.5/tools/experimental/nni_model_config.yaml
--rw-r--r--   0        0        0     2855 2024-04-15 11:07:14.941468 quant2-0.1.5/tools/fb_cls_test.py
--rw-r--r--   0        0        0     7897 2024-04-17 06:33:07.892275 quant2-0.1.5/tools/fb_cls_train.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.6/.gitignore
+-rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.6/LICENSE
+-rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.6/README.md
+-rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.6/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
+-rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.6/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
+-rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.6/quant/README.md
+-rw-r--r--   0        0        0      559 2024-04-19 13:13:26.503336 quant2-0.1.6/quant/__init__.py
+-rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.6/quant/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.6/quant/evaluate/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-18 14:45:48.737962 quant2-0.1.6/quant/evaluate/meters.py
+-rw-r--r--   0        0        0     2584 2024-04-19 09:07:38.924732 quant2-0.1.6/quant/evaluate/table20240326.py
+-rw-r--r--   0        0        0     3658 2024-04-19 09:14:49.360976 quant2-0.1.6/quant/evaluate/utils.py
+-rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.6/quant/football/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.6/quant/football/data/__init__.py
+-rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.6/quant/football/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.6/quant/football/data/functional.py
+-rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.6/quant/football/data/preprocessing.py
+-rw-r--r--   0        0        0      993 2024-04-17 06:41:14.170874 quant2-0.1.6/quant/football/data/sampler.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.6/quant/football/data/stats.py
+-rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.6/quant/football/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.6/quant/football/infer/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-16 01:19:44.599739 quant2-0.1.6/quant/football/infer/fastapi_app.py
+-rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.6/quant/football/infer/fastapi_app_test.py
+-rw-r--r--   0        0        0     8035 2024-04-19 08:10:26.065510 quant2-0.1.6/quant/football/infer/football_infer_overunder_v1.py
+-rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.6/quant/football/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.6/quant/football/models/mtnet.py
+-rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.6/quant/football/models/stnet.py
+-rw-r--r--   0        0        0      547 2024-04-19 12:53:57.861344 quant2-0.1.6/quant/football/transforms/__init__.py
+-rw-r--r--   0        0        0     6622 2024-04-16 00:40:54.525920 quant2-0.1.6/quant/football/transforms/table20240326.py
+-rw-r--r--   0        0        0     8541 2024-04-16 01:19:10.126956 quant2-0.1.6/quant/football/transforms/table20240410.py
+-rw-r--r--   0        0        0     8825 2024-04-16 00:40:14.674251 quant2-0.1.6/quant/football/transforms/table20240414.py
+-rw-r--r--   0        0        0     8396 2024-04-16 02:25:15.544645 quant2-0.1.6/quant/football/transforms/table20240415.py
+-rw-r--r--   0        0        0     8819 2024-04-19 12:52:59.748428 quant2-0.1.6/quant/football/transforms/table20240419.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.6/quant/layers/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.6/quant/layers/layer_scale.py
+-rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.6/quant/layers/mlp.py
+-rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.6/quant/layers/normalization.py
+-rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.6/quant/layers/swiglu_ffn.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.6/quant/utils/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.6/quant/utils/archive.py
+-rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.6/quant/utils/config.py
+-rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.6/quant/utils/io.py
+-rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.6/quant/utils/logging.py
+-rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.6/tests/football/data/test_utils.py
+-rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.6/tools/analysis_tools/analyze_cls_results.py
+-rw-r--r--   0        0        0     2645 2024-04-16 01:48:23.763355 quant2-0.1.6/tools/experimental/make_dataset.py
+-rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.6/tools/experimental/make_split.py
+-rw-r--r--   0        0        0     8078 2024-04-17 06:34:03.034798 quant2-0.1.6/tools/experimental/nni_football.py
+-rw-r--r--   0        0        0      600 2024-04-17 07:13:13.694051 quant2-0.1.6/tools/experimental/nni_football_config.yaml
+-rw-r--r--   0        0        0     1832 2024-04-17 08:12:07.193491 quant2-0.1.6/tools/experimental/nni_football_config_search_space.json
+-rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.6/tools/experimental/nni_model.py
+-rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.6/tools/experimental/nni_model_config.yaml
+-rw-r--r--   0        0        0     2867 2024-04-18 04:24:08.683016 quant2-0.1.6/tools/fb_cls_test.py
+-rw-r--r--   0        0        0     7897 2024-04-17 06:33:07.892275 quant2-0.1.6/tools/fb_cls_train.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.6/PKG-INFO
```

### Comparing `quant2-0.1.5/.gitignore` & `quant2-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/LICENSE` & `quant2-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg` & `quant2-0.1.6/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg` & `quant2-0.1.6/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/pyproject.toml` & `quant2-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/README.md` & `quant2-0.1.6/quant/README.md`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/__init__.py` & `quant2-0.1.6/quant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 help_doc_str = """\
 usage: quant [--version] [--help]
 
 shell command:
     quant -h
```

### Comparing `quant2-0.1.5/quant/evaluate/table20240326.py` & `quant2-0.1.6/quant/evaluate/table20240326.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
-from quant.evaluate.utils import filter_odds_data_by_time_range, compute_bet_overunder
+from quant.evaluate.utils import filter_odds_by_time, compute_bet_overunder, compute_bet_overunder_ret
 from quant.utils.io import load_json, load_pkl
 
 
-def betting_experiment(results, sections, whole=True, time_range=(76, 80), conf_thr=0.7):
+def betting_experiment(results, sections, whole=True, time_range=(76, 80), ret_thr=1.2, ret_conf_thr=0.7):
     if isinstance(results, str):
         suffix = Path(results).suffix
         if suffix == ".json":
             results = load_json(results)
         elif suffix == ".pkl":
             results = load_pkl(results)
         else:
@@ -43,32 +43,28 @@
         if whole:
             score = int(titan["home_score"]) + int(titan["visiting_score"])
         else:
             score = int(titan["home_half_score"]) + int(titan["visiting_half_score"])
 
         bet_odds = []
         for _, odds_data in section["bets_titan"]["odds_overunder"].items():
-            bet_odds.extend(filter_odds_data_by_time_range(odds_data, time_range))
+            bet_odds.extend(filter_odds_by_time(odds_data, time_range))
 
         if len(bet_odds) < 1:
             continue
 
-        bet_p, bet_e, bet_ret = compute_bet_overunder(probs, bet_odds[-1], conf_thr)[:3]
-
-        if bet_e != "none":
-            if score > bet_p:
-                total_bet += 1
-                if bet_e == "over":
-                    correct_bet += 1
-                    correct_bet_ret += bet_ret
-            elif score < bet_p:
-                total_bet += 1
-                if bet_e == "under":
-                    correct_bet += 1
-                    correct_bet_ret += bet_ret
+        for odds in sorted(bet_odds, key=lambda x: int(x[0])):
+            bet_p, bet_c_over, bet_c_under, bet_e = compute_bet_overunder(probs, odds, ret_thr, ret_conf_thr)[:4]
+            if bet_e != "none":
+                break
+
+        a, b, c = compute_bet_overunder_ret(score, bet_p, bet_c_over, bet_c_under, bet_e)
+        total_bet += a
+        correct_bet += b
+        correct_bet_ret += c
 
     n_samples = len(results)
     bet_ratio = total_bet / n_samples
     correct_ratio = correct_bet / total_bet
 
     print(f"下注: {total_bet}/{n_samples} ({bet_ratio*100:.2f}%)")
     print(f"正确: {correct_bet}/{total_bet} ({correct_ratio*100:.2f}%)")
```

### Comparing `quant2-0.1.5/quant/football/data/dataset.py` & `quant2-0.1.6/quant/football/data/dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/data/preprocessing.py` & `quant2-0.1.6/quant/football/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/data/sampler.py` & `quant2-0.1.6/quant/football/data/sampler.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/data/utils.py` & `quant2-0.1.6/quant/football/data/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/infer/fastapi_app.py` & `quant2-0.1.6/quant/football/infer/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/infer/football_infer_overunder_v1.py` & `quant2-0.1.6/quant/football/infer/football_infer_overunder_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 conf_gt, conf_lt = sum(probs[_id + 2:]), sum(probs[:_id + 1])
                 ret2, ret_conf2 = self._ret_overunder(bet_e, bet_c, conf_gt, conf_lt)
 
                 ret, ret_conf = (ret1 + ret2) * 0.5, (ret_conf1 + ret_conf2) * 0.5
             else:
                 continue
 
-            if ret > ret_thr and ret_conf > ret_conf_thr:
+            if ret >= ret_thr and ret_conf >= ret_conf_thr:
                 bet = copy.deepcopy(bet)
                 bet["return"] = ret
                 bet["confidence"] = ret_conf
                 bet["model_id"] = self.model_id
                 ret_bets.append(bet)
 
         return ret_bets
```

### Comparing `quant2-0.1.5/quant/football/models/stnet.py` & `quant2-0.1.6/quant/football/models/stnet.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/transforms/table20240326.py` & `quant2-0.1.6/quant/football/transforms/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/transforms/table20240410.py` & `quant2-0.1.6/quant/football/transforms/table20240410.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/transforms/table20240414.py` & `quant2-0.1.6/quant/football/transforms/table20240414.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/football/transforms/table20240415.py` & `quant2-0.1.6/quant/football/transforms/table20240415.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/layers/mlp.py` & `quant2-0.1.6/quant/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/layers/normalization.py` & `quant2-0.1.6/quant/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/layers/swiglu_ffn.py` & `quant2-0.1.6/quant/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/utils/archive.py` & `quant2-0.1.6/quant/utils/archive.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/utils/config.py` & `quant2-0.1.6/quant/utils/config.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/utils/io.py` & `quant2-0.1.6/quant/utils/io.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/quant/utils/logging.py` & `quant2-0.1.6/quant/utils/logging.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/analysis_tools/analyze_cls_results.py` & `quant2-0.1.6/tools/analysis_tools/analyze_cls_results.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/experimental/make_dataset.py` & `quant2-0.1.6/tools/experimental/make_dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/experimental/make_split.py` & `quant2-0.1.6/tools/experimental/make_split.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/experimental/nni_football.py` & `quant2-0.1.6/tools/experimental/nni_football.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/experimental/nni_football_config.yaml` & `quant2-0.1.6/tools/experimental/nni_football_config.yaml`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/experimental/nni_football_config_search_space.json` & `quant2-0.1.6/tools/experimental/nni_football_config_search_space.json`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/experimental/nni_model.py` & `quant2-0.1.6/tools/experimental/nni_model.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/tools/fb_cls_test.py` & `quant2-0.1.6/tools/fb_cls_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import torch
 import torch.nn.functional as F
 from pathlib import Path
 from quant.football.models import get_model
 from quant.utils.io import load_json, load_pkl, make_dir, save_json
 
 
-def load_model(model, checkpoint):
-    model_type = model.pop("type")
-    model = get_model(model_type, **model)
+def load_model(model_cfg, checkpoint):
+    model_type = model_cfg.pop("type")
+    model = get_model(model_type, **model_cfg)
 
     model.load_state_dict(torch.load(checkpoint, map_location=torch.device("cpu")))
 
     return model
 
 
 def test_dataset(test_file, checkpoint_dir, output_dir=None, device="cuda"):
```

### Comparing `quant2-0.1.5/tools/fb_cls_train.py` & `quant2-0.1.6/tools/fb_cls_train.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.5/PKG-INFO` & `quant2-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant2
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: prettytable
 Requires-Dist: scikit-learn
```

