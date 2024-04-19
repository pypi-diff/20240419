# Comparing `tmp/qieyun-encoder-0.4.2.tar.gz` & `tmp/qieyun_encoder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qieyun-encoder-0.4.2.tar", last modified: Tue Jun  1 08:35:37 2021, max compression
+gzip compressed data, was "qieyun_encoder-0.5.0.tar", last modified: Fri Apr 19 00:32:28 2024, max compression
```

## Comparing `qieyun-encoder-0.4.2.tar` & `qieyun_encoder-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-01 08:35:37.291601 qieyun-encoder-0.4.2/
--rw-r--r--   0 runner     (501) staff       (20)     7048 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       16 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1426 2021-06-01 08:35:37.291790 qieyun-encoder-0.4.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      166 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/README.md
--rw-r--r--   0 runner     (501) staff       (20)       74 2021-06-01 08:35:37.292410 qieyun-encoder-0.4.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1576 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-01 08:35:37.255301 qieyun-encoder-0.4.2/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-01 08:35:37.259649 qieyun-encoder-0.4.2/src/QieyunEncoder/
--rw-r--r--   0 runner     (501) staff       (20)      155 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/src/QieyunEncoder/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3777 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/src/QieyunEncoder/_拓展音韻屬性.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-01 08:35:37.283926 qieyun-encoder-0.4.2/src/QieyunEncoder/工具/
--rw-r--r--   0 runner     (501) staff       (20)      134 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/src/QieyunEncoder/工具/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5942 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/src/QieyunEncoder/工具/反切.py
--rw-r--r--   0 runner     (501) staff       (20)     1727 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/src/QieyunEncoder/工具/正則化韻.py
--rw-r--r--   0 runner     (501) staff       (20)     1565 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/src/QieyunEncoder/常量.py
--rw-r--r--   0 runner     (501) staff       (20)    20466 2021-06-01 08:35:08.000000 qieyun-encoder-0.4.2/src/QieyunEncoder/音韻地位.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-01 08:35:37.291252 qieyun-encoder-0.4.2/src/qieyun_encoder.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1426 2021-06-01 08:35:36.000000 qieyun-encoder-0.4.2/src/qieyun_encoder.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      462 2021-06-01 08:35:37.000000 qieyun-encoder-0.4.2/src/qieyun_encoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2021-06-01 08:35:36.000000 qieyun-encoder-0.4.2/src/qieyun_encoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       14 2021-06-01 08:35:36.000000 qieyun-encoder-0.4.2/src/qieyun_encoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:32:28.229074 qieyun_encoder-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-19 00:32:28.229074 qieyun_encoder-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:32:28.229074 qieyun_encoder-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:32:28.225074 qieyun_encoder-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:32:28.225074 qieyun_encoder-0.5.0/src/QieyunEncoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/_母對應的標準等.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:32:28.225074 qieyun_encoder-0.5.0/src/QieyunEncoder/工具/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/工具/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/工具/反切.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/工具/音韻地位到韻鏡位置.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/工具/音韻屬性到韻鏡位置們.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/工具/韻鏡位置到音韻地位.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/常量.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:32:28.225074 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/母到清濁.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/母到組.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/母到音.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/母與等到類.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/韻到攝.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/轉換/韻目到韻.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18043 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/音韻地位.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/src/QieyunEncoder/韻鏡位置.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:32:28.229074 qieyun_encoder-0.5.0/src/qieyun_encoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-19 00:32:28.000000 qieyun_encoder-0.5.0/src/qieyun_encoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 00:32:28.000000 qieyun_encoder-0.5.0/src/qieyun_encoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:32:28.000000 qieyun_encoder-0.5.0/src/qieyun_encoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 00:32:28.000000 qieyun_encoder-0.5.0/src/qieyun_encoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:32:28.229074 qieyun_encoder-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 00:32:13.000000 qieyun_encoder-0.5.0/tests/test.py
```

### Comparing `qieyun-encoder-0.4.2/LICENSE` & `qieyun_encoder-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qieyun-encoder-0.4.2/PKG-INFO` & `qieyun_encoder-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: qieyun-encoder
-Version: 0.4.2
+Version: 0.5.0
 Summary: A Python library for the operating the basic structure of the Qieyun phonological system
-Home-page: https://github.com/nk2028/qieyun-encoder-python
-Author: The nk2028 Project
-Author-email: support@nk2028.shn.hk
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/nk2028/qieyun-encoder-python/issues
-Project-URL: Source, https://github.com/nk2028/qieyun-encoder-python
-Description: # qieyun-encoder-python
-        
-        A Python library for the operating the basic structure of the Qieyun phonological system
-        
-        ## Install
-        
-        ```sh
-        $ pip install qieyun-encoder
-        ```
-        
-Keywords: middle-chinese historical-linguistics qieyun
-Platform: UNKNOWN
+Author-email: nk2028 Developers <support@nk2028.shn.hk>
+Project-URL: Homepage, https://github.com/nk2028/qieyun-encoder-python
+Project-URL: Issues, https://github.com/nk2028/qieyun-encoder-python/issues
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Natural Language :: Chinese (Traditional)
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6, <4
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Qieyun Encoder Python
+
+A Python library for the operating the basic structure of the Qieyun phonological system
+
+## Install
+
+```sh
+$ pip install qieyun-encoder
+```
+
+## Usage
+
+```python
+import QieyunEncoder as QE
+print(QE.音韻地位.from描述('幫三凡入').攝)  # output: 咸
+```
+
+For detailed usage, see [documentation](https://qieyun-encoder-python.readthedocs.io).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qieyun-encoder-0.4.2/src/QieyunEncoder/工具/反切.py` & `qieyun_encoder-0.5.0/src/QieyunEncoder/工具/反切.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 # -*- coding: utf-8 -*-
 
-'''
-根據反切規律自動完成反切過程。
-'''
-
-from typing import List
-from ..常量 import 常量
+from .. import 常量
+from .._母對應的標準等 import 母對應的標準等
 from ..音韻地位 import 音韻地位
-from .._拓展音韻屬性 import 母到標準等
-
 
-def _jointer(xs: List[str]):
+def _jointer(xs: list[str]):
     '''
     將多個字串以頓號和「或」字連接。
 
-    ```python
-    >>> _jointer(['A'])
-    'A'
-    >>> _jointer(['A', 'B'])
-    'A或B'
-    >>> _jointer(['A', 'B', 'C', 'D'])
-    'A、B、C或D'
-    ```
+    Examples:
+
+        >>> _jointer(['A'])
+        'A'
+        >>> _jointer(['A', 'B'])
+        'A或B'
+        >>> _jointer(['A', 'B', 'C', 'D'])
+        'A、B、C或D'
     '''
     return ''.join(x + '、' for x in xs[:-2]) + '或'.join(xs[-2:])
 
-
 def 反切(上字音韻地位: 音韻地位, 下字音韻地位: 音韻地位, 顯示步驟=False, 類隔切=False):
     '''
     根據反切規律自動完成反切過程。
 
-    當「顯示步驟」爲 `False` 時，回傳所有被切字音韻地位的列表。
+    當「顯示步驟」爲 ``False`` 時，回傳所有被切字音韻地位的列表。
 
-    當「顯示步驟」爲 `True` 時，回傳 `dict`，包含「被切字音韻地位們」與「步驟」兩個字段。
+    當「顯示步驟」爲 ``True`` 時，回傳 ``dict``，包含「被切字音韻地位們」與「步驟」兩個字段。
     '''
     if 類隔切:
         raise NotImplementedError
 
     步驟 = []
 
     母 = 上字音韻地位.母
@@ -135,15 +128,15 @@
         步驟.append('反切下字爲重紐B類或云母，被切字爲重紐B類')
     else:
         重紐 = 'AB'
         步驟.append('不能確定重紐，被切字可能爲重紐A類或重紐B類')
 
     # 母對等的約束
 
-    標準等 = 母到標準等[母]
+    標準等 = 母對應的標準等[母]
     if any(等1 not in 標準等 for 等1 in 等):
         等 = ''.join(等1 for 等1 in 等 if 等1 in 標準等)
         步驟.append(f'{母}母只能爲{標準等}等')
 
     # 組合被切字所有可能等音韻地位
 
     被切字音韻地位們 = [
```

### Comparing `qieyun-encoder-0.4.2/src/QieyunEncoder/音韻地位.py` & `qieyun_encoder-0.5.0/src/QieyunEncoder/音韻地位.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,259 +1,132 @@
 # -*- coding: utf-8 -*-
 
-'''
-定義切韻音系音韻地位及相關操作。
-
-## 音韻屬性
-
-### 母、音、組、清濁
-
-母採用三十八聲類的分類方法。
-
-<style>
-.big-table { border-collapse: collapse; margin: 1em 0; display: block; }
-.big-table th, .big-table td { border: 1px solid; padding: 4px 6px; text-align: center; }
-.admonition { border-radius: 14px; padding: 2px 18px !important; }
-.admonition > .admonition-title { display: none; }
-</style>
-
-<table class="big-table">
-<tbody>
-<tr><th></th><th>全清</th><th>次清</th><th>全濁</th><th>次濁</th><th>全清</th><th>全濁</th></tr>
-<tr><th>脣音</th><td>幫</td><td>滂</td><td>並</td><td>明</td><td></td><td></td></tr>
-<tr><th rowspan="3">舌音</th><td>端</td><td>透</td><td>定</td><td>泥</td><td></td><td></td></tr>
-<tr><td>知</td><td>徹</td><td>澄</td><td>孃</td><td></td><td></td></tr>
-<tr><td></td><td></td><td></td><td>來</td><td></td><td></td></tr>
-<tr><th rowspan="4">齒音</th><td>精</td><td>清</td><td>從</td><td></td><td>心</td><td>邪</td></tr>
-<tr><td>莊</td><td>初</td><td>崇</td><td></td><td>生</td><td>俟</td></tr>
-<tr><td>章</td><td>昌</td><td>常</td><td></td><td>書</td><td>船</td></tr>
-<tr><td></td><td></td><td></td><td>日</td><td></td><td></td></tr>
-<tr><th>牙音</th><td>見</td><td>溪</td><td>羣</td><td>疑</td><td></td><td></td></tr>
-<tr><th rowspan="2">喉音</th><td>影</td><td></td><td></td><td>云</td><td>曉</td><td>匣</td></tr>
-<tr><td></td><td></td><td></td><td>以</td><td></td><td></td></tr>
-</tbody>
-</table>
-
-上表中正文部分爲母，橫向爲音與組，縱向爲清濁。
-
-注意曉母爲全清，云母爲次濁。組不涵蓋來日以母。
-
-.. hint::
-
-    不要與中古後期三十六字母混淆。
-    
-    中古後期三十六字母：
-
-    <table class="big-table">
-    <tbody>
-    <tr><th></th><th>全清</th><th>次清</th><th>全濁</th><th>次濁</th><th>全清</th><th>全濁</th></tr>
-    <tr><th rowspan="2">脣音</th><td>幫</td><td>滂</td><td>並</td><td>明</td><td></td><td></td></tr>
-    <tr><td>非</td><td>敷</td><td>奉</td><td>微</td><td></td><td></td></tr>
-    <tr><th rowspan="3">舌音</th><td>端</td><td>透</td><td>定</td><td>泥</td><td></td><td></td></tr>
-    <tr><td>知</td><td>徹</td><td>澄</td><td>孃</td><td></td><td></td></tr>
-    <tr><td></td><td></td><td></td><td>來</td><td></td><td></td></tr>
-    <tr><th rowspan="3">齒音</th><td>精</td><td>清</td><td>從</td><td></td><td>心</td><td>邪</td></tr>
-    <tr><td>照</td><td>穿</td><td>牀</td><td></td><td>審</td><td>禪</td></tr>
-    <tr><td></td><td></td><td></td><td>日</td><td></td><td></td></tr>
-    <tr><th>牙音</th><td>見</td><td>溪</td><td>羣</td><td>疑</td><td></td><td></td></tr>
-    <tr><th>喉音</th><td>影</td><td></td><td></td><td>喻</td><td>曉</td><td>匣</td></tr>
-    </tbody>
-    </table>
-
-    區別如下：
-
-    - 幫滂並明在三等輕脣韻前分化爲非敷奉微
-    - 云以母合流爲喻母
-    - 莊章組合流爲照組
-
-### 呼
-
-取值：開、合、`None`。其中 `None` 表示開合中立。
-
-脣音的開合必爲 `None`。
-
-韻與開合的關係如下：
-
-- 開合皆有的韻：支脂微齊祭泰佳皆夬廢眞元寒刪山仙先歌麻陽唐庚耕清青蒸登
-- 必爲開口的韻：咍痕欣嚴之魚臻蕭宵肴豪侯侵覃談鹽添咸銜
-- 必爲合口的韻：灰魂文凡
-- 開合中立的韻：東冬鍾江虞模尤幽
-
-.. hint::
-
-    不要與韻圖的開合混淆。
-
-    以《韻鏡》爲例，開合有三種取值：開、合、開合。
-
-    - 在《韻鏡》中，對脣音沒有特殊處理。而在此處，脣音的開合必爲 `None`
-    - 《韻鏡》所標「開合」與此處開合中立的韻的劃分並不完全相同
-    - 《韻鏡》存在誤標開合的情況，如第四轉「內轉第四開合」當爲「內轉第四開」
-
-### 等
-
-取值：一、二、三、四。
-
-韻與等的關係如下：
-
-- 一等韻：冬模泰咍灰痕魂寒豪唐登侯覃談
-- 二等韻：江佳皆夬刪山肴耕咸銜
-- 三等韻：鍾支脂之微魚虞祭廢眞臻欣元文仙宵陽清蒸尤幽侵鹽嚴凡
-- 四等韻：齊先蕭青添
-- 一三等韻：東歌
-- 二三等韻：麻庚
-
-母對等沒有硬性約束條件，因爲存在「無音有字」的小韻。陳澧《切韻考》：「等之云者，當主乎韻，不當主乎聲」。
-
-.. hint::
-
-    不要與韻圖的等混淆。
-
-    - 韻圖將重紐 A 類字置於四等，實際爲三等
-    - 三等韻的莊組字列在二等
-    - 三等韻的精組字列在四等
-    - 三等的幽韻列在四等
-
-### 重紐
-
-取值：`None`、重紐A類、重紐B類。
-
-- 重紐母：幫滂並明見溪羣疑影曉
-- 重紐韻：支脂祭眞仙宵清侵鹽
-
-當聲紐不爲重紐母，或韻不爲重紐韻時，重紐必須爲 `None`。
-
-清韻重紐母取重紐A類。
-
-### 韻、攝
-
-- 通攝：東冬鍾
-- 江攝：江
-- 止攝：支脂之微
-- 遇攝：魚虞模
-- 蟹攝：齊佳皆灰咍祭泰夬廢
-- 臻攝：眞諄臻文欣元魂痕
-- 山攝：寒桓刪山先仙
-- 效攝：蕭宵肴豪
-- 果攝：歌戈
-- 假攝：麻
-- 宕攝：唐陽
-- 梗攝：庚耕清青
-- 曾攝：登蒸
-- 流攝：侯尤幽
-- 深攝：侵
-- 咸攝：覃談鹽添咸銜嚴凡
-
-.. hint::
-
-    元韻在臻攝而非山攝（註：下一版會改爲山攝）。
-
-    《廣韻》沒有諄桓戈韻，分別併入眞寒歌韻。殷韻爲欣韻（註：下一版會改爲殷韻）。
-
-### 聲
-
-取值：平、上、去、入；仄、舒。
-
-其中，仄表示上去入聲，舒表示平上去聲。
-'''
-
 import re
-from typing import Optional
 
-from .常量 import 常量
-from ._拓展音韻屬性 import 母到清濁, 母到音, 母到組, 韻到攝
+from . import 常量
+from ._母對應的標準等 import 母對應的標準等
+from .轉換 import 母到清濁, 母到音, 母到組, 韻到攝, 母與等到類
 
 編碼表 = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789'
-韻順序表 = '東_冬鍾江支脂之微魚虞模齊祭泰佳皆夬灰咍廢眞臻文欣元魂痕寒刪山仙先蕭宵肴豪歌_麻_陽唐庚_耕清青蒸登尤侯幽侵覃談鹽添咸銜嚴凡'
-
-解析音韻描述 = re.compile('([%s])([%s]?)([%s]?)([%s]?)([%s])([%s])' % (
-    常量.所有母, 常量.所有呼, 常量.所有等, 常量.所有重紐, 常量.所有韻, 常量.所有聲))
-
+韻順序表 = '東_冬鍾江支脂之微魚虞模齊祭泰佳皆夬灰咍廢真臻文殷元魂痕寒刪山仙先蕭宵肴豪歌_麻_陽唐庚_耕清青蒸登尤侯幽侵覃談鹽添咸銜嚴凡'
+解析音韻描述 = re.compile(fr'([{常量.所有母}])([{常量.所有呼}])?([{常量.所有等}])?([{常量.所有重紐}])?([{常量.所有韻}])([{常量.所有聲}])')
 
 class 音韻地位:
     '''
     切韻音系音韻地位。
+
+    :param 母: 聲母
+    :type 母: str
+    :param 呼: 呼（開/合），可以爲 ``None``
+    :type 呼: str, optional
+    :param 等: 等
+    :type 等: str
+    :param 重紐: 重紐，可以爲 ``None``
+    :type 重紐: str, optional
+    :param 韻: 韻
+    :type 韻: str
+    :param 聲: 聲調
+    :type 聲: str
     '''
 
-    def __init__(self, 母, 呼, 等, 重紐, 韻, 聲):
+    def __init__(self, 母: str, 呼: str | None, 等: str, 重紐: str | None, 韻: str, 聲: str):
+        韻 = 韻.replace('欣', '殷').replace('眞', '真')  # 容錯
+
         音韻地位.驗證(母, 呼, 等, 重紐, 韻, 聲)
 
         self.母 = 母
         self.呼 = 呼
         self.等 = 等
         self.重紐 = 重紐
         self.韻 = 韻
         self.聲 = 聲
 
     @property
     def 清濁(self) -> str:
         '''
         清濁（全清、次清、全濁、次濁）。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').清濁
-        '全清'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').清濁
-        '全濁'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').清濁
+            '全清'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').清濁
+            '全濁'
         '''
-        return 母到清濁[self.母]
+        return 母到清濁(self.母)
 
     @property
     def 音(self) -> str:
         '''
         音（脣音、舌音、齒音、牙音、喉音）。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').音
-        '脣'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').音
-        '牙'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').音
+            '脣'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').音
+            '牙'
         '''
-        return 母到音[self.母]
+        return 母到音(self.母)
 
     @property
-    def 組(self) -> Optional[str]:
+    def 組(self) -> str | None:
         '''
         組。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').組
-        '幫'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').組
-        '見'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').組
+            '幫'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').組
+            '見'
         '''
-        return 母到組[self.母]
+        return 母到組(self.母)
 
     @property
     def 攝(self) -> str:
         '''
         攝。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').攝
-        '咸'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').攝
-        '止'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').攝
+            '咸'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').攝
+            '止'
         '''
-        return 韻到攝[self.韻]
+        return 韻到攝(self.韻)
+
+    @property
+    def 類(self) -> str:
+        '''
+        五十一聲類。
+
+        注意五十一聲類中俟母獨立，故實為五十二個。
+
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').類
+            '方'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').類
+            '渠'
+        '''
+        return 母與等到類(self.母, self.等)
 
     @property
     def 描述(self) -> str:
         '''
         音韻描述。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').描述
-        '幫三凡入'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').描述
-        '羣開三A支平'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').描述
+            '幫三凡入'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').描述
+            '羣開三A支平'
         '''
         母 = self.母
         呼 = self.呼
         等 = self.等
         重紐 = self.重紐
         韻 = self.韻
         聲 = self.聲
@@ -261,46 +134,48 @@
         return 母 + (呼 or '') + 等 + (重紐 or '') + 韻 + 聲
 
     @property
     def 最簡描述(self) -> str:
         '''
         最簡音韻描述。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').最簡描述
-        '幫凡入'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').最簡描述
-        '羣開A支平'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').最簡描述
+            '幫凡入'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').最簡描述
+            '羣開A支平'
         '''
         母 = self.母
         呼 = self.呼
         等 = self.等
         重紐 = self.重紐
         韻 = self.韻
         聲 = self.聲
 
-        if 韻 not in 常量.開合皆有的韻:
-            呼 = None
+        if 韻 not in 常量.開合兼備的韻:
+            呼 = ''
         if 韻 not in 常量.一三等韻 and 韻 not in 常量.二三等韻:
-            等 = None
+            等 = ''
+        if 重紐 is None:
+            重紐 = ''
 
-        return 母 + (呼 or '') + (等 or '') + (重紐 or '') + 韻 + 聲
+        return f'{母}{呼}{等}{重紐}{韻}{聲}'
 
     @property
     def 表達式(self) -> str:
         '''
         音韻表達式。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').表達式
-        '幫母 三等 凡韻 入聲'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').表達式
-        '羣母 開口 三等 重紐A類 支韻 平聲'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').表達式
+            '幫母 三等 凡韻 入聲'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').表達式
+            '羣母 開口 三等 重紐A類 支韻 平聲'
         '''
         母 = self.母
         呼 = self.呼
         等 = self.等
         重紐 = self.重紐
         韻 = self.韻
         聲 = self.聲
@@ -311,51 +186,51 @@
         return f'{母}母 {呼字段}{等}等 {重紐字段}{韻}韻 {聲}聲'
 
     @property
     def 最簡表達式(self) -> str:
         '''
         最簡音韻表達式。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').最簡表達式
-        '幫母 凡韻 入聲'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').最簡表達式
-        '羣母 開口 重紐A類 支韻 平聲'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').最簡表達式
+            '幫母 凡韻 入聲'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').最簡表達式
+            '羣母 開口 重紐A類 支韻 平聲'
         '''
         母 = self.母
         呼 = self.呼
         等 = self.等
         重紐 = self.重紐
         韻 = self.韻
         聲 = self.聲
 
-        if 韻 not in 常量.開合皆有的韻:
+        if 韻 not in 常量.開合兼備的韻:
             呼 = None
         if 韻 not in 常量.一三等韻 and 韻 not in 常量.二三等韻:
-            等 = None
+            等 = ''
 
         呼字段 = f'{呼}口 ' if 呼 else ''
         等字段 = f'{等}等 ' if 等 else ''
         重紐字段 = f'重紐{重紐}類 ' if 重紐 else ''
         韻字段 = f'{韻}韻 ' if 韻 else ''
 
         return f'{母}母 {呼字段}{等字段}{重紐字段}{韻字段}{聲}聲'
 
     @property
     def 編碼(self) -> str:
         '''
         音韻編碼。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').編碼
-        'A9D'
-        >>> Qieyun.音韻地位.from描述('羣開三A支平').編碼
-        'fFA'
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').編碼
+            'A9D'
+            >>> QieyunEncoder.音韻地位.from描述('羣開三A支平').編碼
+            'fFA'
         '''
         母 = self.母
         呼 = self.呼
         等 = self.等
         重紐 = self.重紐
         韻 = self.韻
         聲 = self.聲
@@ -373,22 +248,22 @@
 
         return 編碼表[母編碼] + 編碼表[韻編碼] + 編碼表[其他編碼]
 
     def 屬於(self, 表達式: str) -> bool:
         '''
         判斷音韻地位是否符合給定的音韻表達式。
 
-        ```python
-        >>> Qieyun.音韻地位.from描述('幫三凡入').屬於('章母')
-        False
-        >>> Qieyun.音韻地位.from描述('幫三凡入').屬於('一四等')
-        False
-        >>> Qieyun.音韻地位.from描述('幫三凡入').屬於('幫組 或 陽韻')
-        True
-        ```
+        Examples:
+
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').屬於('章母')
+            False
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').屬於('一四等')
+            False
+            >>> QieyunEncoder.音韻地位.from描述('幫三凡入').屬於('幫組 或 陽韻')
+            True
         '''
         def inner(q: str):
             if q.endswith('母'):
                 母們 = q[:-1]
                 assert len(母們) > 0, '未指定母'
                 for 母 in 母們:
                     assert 母 in 常量.所有母, 母 + '母不存在'
@@ -464,57 +339,64 @@
             if q == '次濁':
                 return self.清濁 == '次濁'
 
             raise AssertionError('無此運算符：' + q)
 
         return any(all(inner(q) for q in p.split(' ')) for p in 表達式.split(' 或 '))
 
-    def __eq__(self, that):
-        if not isinstance(that, 音韻地位):
-            return False
-        return self.描述 == that.描述
-
     @staticmethod
-    def 驗證(母: str, 呼: Optional[str], 等: str, 重紐: Optional[str], 韻: str, 聲: str):
+    def 驗證(母: str, 呼: str | None, 等: str, 重紐: str | None, 韻: str, 聲: str):
         '''
         驗證給定的音韻地位六要素是否合法。
+
+        :param 母: 聲母
+        :type 母: str
+        :param 呼: 呼（開口呼/合口呼），可以爲 ``None``
+        :type 呼: str, optional
+        :param 等: 等
+        :type 等: str
+        :param 重紐: 重紐，可以爲 ``None``
+        :type 重紐: str, optional
+        :param 韻: 韻
+        :type 韻: str
+        :param 聲: 聲調
+        :type 聲: str
         '''
+
         assert len(母) == 1 and 母 in 常量.所有母, 'Unexpected 母: ' + repr(母)
         assert len(等) == 1 and 等 in 常量.所有等, 'Unexpected 等: ' + repr(等)
         assert len(韻) == 1 and 韻 in 常量.所有韻, 'Unexpected 韻: ' + repr(韻)
         assert len(聲) == 1 and 聲 in 常量.所有聲, 'Unexpected 聲: ' + repr(聲)
 
         if 母 in '幫滂並明' or 韻 in 常量.開合中立的韻:
             assert 呼 is None, 'Unexpected 呼: ' + repr(呼)
         elif 韻 in 常量.必爲開口的韻:
             assert 呼 == '開'
         elif 韻 in 常量.必爲合口的韻:
             assert 呼 == '合'
         else:
-            assert 呼 is not None and len(
-                呼) == 1 and 呼 in 常量.所有呼, 'Unexpected 呼: ' + repr(呼)
+            assert 呼 is not None and len(呼) == 1 and 呼 in 常量.所有呼, 'Unexpected 呼: ' + repr(呼)
 
         if 母 in 常量.重紐母 and 韻 in 常量.重紐韻:
-            assert 重紐 is not None and len(
-                重紐) == 1 and 重紐 in 常量.所有重紐, 'Unexpected 重紐: ' + repr(重紐)
+            assert 重紐 is not None and len(重紐) == 1 and 重紐 in 常量.所有重紐, 'Unexpected 重紐: ' + repr(重紐)
         else:
             assert 重紐 is None, 'Unexpected 重紐: ' + repr(重紐)
 
         if 韻 in 常量.一等韻:
             assert 等 == '一', 'Unexpected 等: ' + repr(等)
         elif 韻 in 常量.二等韻:
             assert 等 == '二', 'Unexpected 等: ' + repr(等)
         elif 韻 in 常量.三等韻:
             assert 等 == '三', 'Unexpected 等: ' + repr(等)
         elif 韻 in 常量.四等韻:
             assert 等 == '四', 'Unexpected 等: ' + repr(等)
         elif 韻 in 常量.一三等韻:
-            assert 等 in ('一', '三'), 'Unexpected 等: ' + repr(等)
+            assert 等 in '一三', 'Unexpected 等: ' + repr(等)
         elif 韻 in 常量.二三等韻:
-            assert 等 in ('二', '三'), 'Unexpected 等: ' + repr(等)
+            assert 等 in '二三', 'Unexpected 等: ' + repr(等)
 
     @staticmethod
     def from編碼(編碼: str):
         '''
         將音韻編碼轉換爲音韻地位。
         '''
         assert len(編碼) == 3, 'Invalid 編碼: ' + repr(編碼)
@@ -524,52 +406,53 @@
         其他編碼 = 編碼表.index(編碼[2])
 
         呼編碼 = 其他編碼 >> 3
         重紐編碼 = (其他編碼 >> 2) & 0b1
         聲編碼 = 其他編碼 & 0b11
 
         母 = 常量.所有母[母編碼]
-        呼 = 常量.所有呼[呼編碼]
-        重紐 = 常量.所有重紐[重紐編碼]
+        呼: str | None = 常量.所有呼[呼編碼]
+        重紐: str | None = 常量.所有重紐[重紐編碼]
         聲 = 常量.所有聲[聲編碼]
 
-        if 韻編碼 == 0:
-            韻 = '東'
-            等 = '一'
-        elif 韻編碼 == 1:
-            韻 = '東'
-            等 = '三'
-        elif 韻編碼 == 37:
-            韻 = '歌'
-            等 = '一'
-        elif 韻編碼 == 38:
-            韻 = '歌'
-            等 = '三'
-        elif 韻編碼 == 39:
-            韻 = '麻'
-            等 = '二'
-        elif 韻編碼 == 40:
-            韻 = '麻'
-            等 = '三'
-        elif 韻編碼 == 43:
-            韻 = '庚'
-            等 = '二'
-        elif 韻編碼 == 44:
-            韻 = '庚'
-            等 = '三'
-        else:
-            韻 = 韻順序表[韻編碼]
-            if 韻 in 常量.一等韻:
+        match 韻編碼:
+            case 0:
+                韻 = '東'
                 等 = '一'
-            elif 韻 in 常量.二等韻:
+            case 1:
+                韻 = '東'
+                等 = '三'
+            case 37:
+                韻 = '歌'
+                等 = '一'
+            case 38:
+                韻 = '歌'
+                等 = '三'
+            case 39:
+                韻 = '麻'
                 等 = '二'
-            elif 韻 in 常量.三等韻:
+            case 40:
+                韻 = '麻'
                 等 = '三'
-            elif 韻 in 常量.四等韻:
-                等 = '四'
+            case 43:
+                韻 = '庚'
+                等 = '二'
+            case 44:
+                韻 = '庚'
+                等 = '三'
+            case _:
+                韻 = 韻順序表[韻編碼]
+                if 韻 in 常量.一等韻:
+                    等 = '一'
+                elif 韻 in 常量.二等韻:
+                    等 = '二'
+                elif 韻 in 常量.三等韻:
+                    等 = '三'
+                elif 韻 in 常量.四等韻:
+                    等 = '四'
 
         if 母 in '幫滂並明' or 韻 in 常量.開合中立的韻:
             assert 呼 == '開'
             呼 = None
 
         if 母 not in 常量.重紐母 or 韻 not in 常量.重紐韻:
             assert 重紐 == 'A'
@@ -582,23 +465,20 @@
     @staticmethod
     def from描述(描述: str):
         '''
         將音韻描述或最簡音韻描述轉換爲音韻地位。
         '''
         # TODO: 重寫解析器，支援更多格式
 
+        描述 = 描述.replace('欣', '殷').replace('眞', '真')  # 容錯
+
         match = 解析音韻描述.fullmatch(描述)
-        assert match is not None
+        assert match is not None, 'Invalid 描述: ' + repr(描述)
 
-        母 = match.group(1)
-        呼 = match.group(2) or None
-        等 = match.group(3) or None
-        重紐 = match.group(4) or None
-        韻 = match.group(5)
-        聲 = match.group(6)
+        母, 呼, 等, 重紐, 韻, 聲 = match.groups()
 
         if 呼 is None and 母 not in '幫滂並明':
             if 韻 in 常量.必爲開口的韻:
                 呼 = '開'
             elif 韻 in 常量.必爲合口的韻:
                 呼 = '合'
 
@@ -607,14 +487,62 @@
                 等 = '一'
             elif 韻 in 常量.二等韻:
                 等 = '二'
             elif 韻 in 常量.三等韻:
                 等 = '三'
             elif 韻 in 常量.四等韻:
                 等 = '四'
+            else:
+                raise ValueError(f'Unexpected 韻: {韻}')
 
         音韻地位.驗證(母, 呼, 等, 重紐, 韻, 聲)
 
         return 音韻地位(母, 呼, 等, 重紐, 韻, 聲)
 
-    def __repr__(self):
+    def is_normal(self):
+        '''
+        是 normal 的音韻地位。
+
+        例如，端母二等不是 normal 的音韻地位。
+        '''
+        return self.等 in 母對應的標準等[self.母]
+
+    def __repr__(self) -> str:
         return '<音韻地位 ' + self.描述 + '>'
+
+    def __eq__(self, that) -> bool:
+        if not isinstance(that, 音韻地位):
+            return False
+        return self.最簡描述 == that.最簡描述
+
+    def __lt__(self, that) -> bool:
+        if not isinstance(that, 音韻地位):
+            raise TypeError("'<' not supported between instances of '音韻地位' and " + type(that).__name__)
+
+        def 母到編碼(母):
+            return 常量.所有母.index(母)
+
+        def 呼到編碼(呼):
+            return [None, '開', '合'].index(呼)
+
+        def 等到編碼(等):
+            return '一二三四'.index(等)
+
+        def 重紐到編碼(重紐):
+            return [None, 'A', 'B'].index(重紐)
+
+        def 韻到編碼(韻):
+            return 常量.所有韻.index(韻)
+
+        def 聲到編碼(聲):
+            return 常量.所有聲.index(聲)
+
+        return (聲到編碼(self.聲), 韻到編碼(self.韻), 重紐到編碼(self.重紐), 等到編碼(self.等), 呼到編碼(self.呼), 母到編碼(self.母)) \
+             < (聲到編碼(that.聲), 韻到編碼(that.韻), 重紐到編碼(that.重紐), 等到編碼(that.等), 呼到編碼(that.呼), 母到編碼(that.母))
+
+    def __le__(self, that) -> bool:
+        if not isinstance(that, 音韻地位):
+            raise TypeError("'<' not supported between instances of '音韻地位' and " + type(that).__name__)
+        return self == that or self < that
+
+    def __hash__(self) -> int:
+        return hash(self.最簡描述)
```

### Comparing `qieyun-encoder-0.4.2/src/qieyun_encoder.egg-info/PKG-INFO` & `qieyun_encoder-0.5.0/src/qieyun_encoder.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: qieyun-encoder
-Version: 0.4.2
+Version: 0.5.0
 Summary: A Python library for the operating the basic structure of the Qieyun phonological system
-Home-page: https://github.com/nk2028/qieyun-encoder-python
-Author: The nk2028 Project
-Author-email: support@nk2028.shn.hk
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/nk2028/qieyun-encoder-python/issues
-Project-URL: Source, https://github.com/nk2028/qieyun-encoder-python
-Description: # qieyun-encoder-python
-        
-        A Python library for the operating the basic structure of the Qieyun phonological system
-        
-        ## Install
-        
-        ```sh
-        $ pip install qieyun-encoder
-        ```
-        
-Keywords: middle-chinese historical-linguistics qieyun
-Platform: UNKNOWN
+Author-email: nk2028 Developers <support@nk2028.shn.hk>
+Project-URL: Homepage, https://github.com/nk2028/qieyun-encoder-python
+Project-URL: Issues, https://github.com/nk2028/qieyun-encoder-python/issues
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Natural Language :: Chinese (Traditional)
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6, <4
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Qieyun Encoder Python
+
+A Python library for the operating the basic structure of the Qieyun phonological system
+
+## Install
+
+```sh
+$ pip install qieyun-encoder
+```
+
+## Usage
+
+```python
+import QieyunEncoder as QE
+print(QE.音韻地位.from描述('幫三凡入').攝)  # output: 咸
+```
+
+For detailed usage, see [documentation](https://qieyun-encoder-python.readthedocs.io).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

