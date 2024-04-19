# Comparing `tmp/arts-2024.4.13.tar.gz` & `tmp/arts-2024.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-2024.4.13.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arts-2024.4.19.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arts-2024.4.13.tar` & `arts-2024.4.19.tar`

### file list

```diff
@@ -1,239 +1,239 @@
--rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.13/.gitignore
--rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.13/README.md
--rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.13/arts/CoolMemory-English/Copyright
--rw-r--r--   0        0        0    10492 2024-04-12 03:24:43.904296 arts-2024.4.13/arts/CoolMemory-English/README.md
--rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.13/arts/CoolMemory-English/art.json
--rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/CoolMemory-English/licenses/README.md
--rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
--rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
--rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
--rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
--rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.13/arts/WeChat-Art-Museum/art.json
--rw-r--r--   0        0        0    53616 2024-04-13 08:11:29.182384 arts-2024.4.13/arts/WeChat-Art-Museum/index.html
--rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.13/arts/__init__.py
--rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.13/arts/articles/010-赚钱宝典/010-财富的本质/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.13/arts/articles/010-赚钱宝典/010-财富的本质/art.json
--rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.13/arts/articles/010-赚钱宝典/020-商业价值/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.13/arts/articles/010-赚钱宝典/020-商业价值/art.json
--rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.13/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
--rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.13/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
--rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.13/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.13/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
--rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.13/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.13/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
--rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.13/arts/articles/150-小民参政/300-广义的民主/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.13/arts/articles/150-小民参政/300-广义的民主/art.json
--rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.13/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.13/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
--rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.13/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.13/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
--rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.13/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.13/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
--rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.13/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.13/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
--rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.13/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.13/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
--rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.13/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.13/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
--rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.13/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.13/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
--rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.13/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.13/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
--rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.13/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.13/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
--rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.13/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.13/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
--rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.13/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.13/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
--rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.13/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.13/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
--rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.13/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.13/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
--rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.13/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.13/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
--rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.4.13/arts/articles/450-万象思考/700-堕胎自由权/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.13/arts/articles/450-万象思考/700-堕胎自由权/art.json
--rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.13/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.13/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
--rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.13/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.13/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
--rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.13/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.13/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
--rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.13/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.13/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
--rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.13/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.13/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
--rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.13/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
--rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.13/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
--rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.13/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.13/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.13/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.13/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.13/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.13/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
--rw-r--r--   0        0        0    11275 2024-04-13 03:33:01.837811 arts-2024.4.13/arts/base95/LICENSE
--rw-r--r--   0        0        0     2733 2024-04-13 07:56:54.808841 arts-2024.4.13/arts/base95/README.md
--rw-r--r--   0        0        0       33 2024-04-13 03:21:49.855973 arts-2024.4.13/arts/base95/__init__.py
--rw-r--r--   0        0        0     1822 2024-04-13 04:05:56.297240 arts-2024.4.13/arts/base95/_core.py
--rw-r--r--   0        0        0       98 2024-04-13 08:02:33.643534 arts-2024.4.13/arts/base95/art.json
--rw-r--r--   0        0        0       44 2024-04-13 03:22:45.204180 arts-2024.4.13/arts/base95/base95.py
--rw-r--r--   0        0        0      672 2024-04-13 08:17:13.839226 arts-2024.4.13/arts/base95/pyproject.toml
--rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.13/arts/cooltypes/LICENSE
--rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.13/arts/cooltypes/__init__.py
--rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.13/arts/cooltypes/envname/README.md
--rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.13/arts/cooltypes/envname/__init__.py
--rw-r--r--   0        0        0      447 2024-04-08 07:02:42.471320 arts-2024.4.13/arts/cooltypes/envname/_core.py
--rw-r--r--   0        0        0      548 2024-04-08 07:01:42.600503 arts-2024.4.13/arts/cooltypes/moduledb/README.md
--rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.13/arts/cooltypes/moduledb/__init__.py
--rw-r--r--   0        0        0     3515 2024-04-08 06:57:45.544745 arts-2024.4.13/arts/cooltypes/moduledb/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.13/arts/cooltypes/modules/coolstr/__init__.py
--rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.13/arts/cooltypes/modules/coolstr/_core.py
--rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.13/arts/cooltypes/modules/cooltime/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.13/arts/cooltypes/modules/cooltime/__init__.py
--rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.13/arts/cooltypes/modules/cooltime/_art.json
--rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.13/arts/cooltypes/modules/cooltime/_core.py
--rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.13/arts/cooltypes/modules/rslice/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.13/arts/cooltypes/modules/rslice/__init__.py
--rw-r--r--   0        0        0     2801 2024-03-22 15:12:37.864736 arts-2024.4.13/arts/cooltypes/modules/rslice/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.13/arts/cooltypes/modules/vtype/__init__.py
--rw-r--r--   0        0        0    10012 2024-04-13 01:46:07.477663 arts-2024.4.13/arts/cooltypes/modules/vtype/_core.py
--rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.13/arts/cooltypes/设计.md
--rw-r--r--   0        0        0    61538 2024-04-13 08:26:22.430802 arts-2024.4.13/arts/index.html
--rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.13/arts/life/2018/莆田学院·毕业生留影/art.json
--rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.13/arts/life/2018/莆田学院·毕业生留影/index.html
--rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.13/arts/life/2019/苏州市虎丘山/art.json
--rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.13/arts/life/2019/苏州市虎丘山/index.html
--rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.13/arts/life/2022/泉州市丰泽区·雨后街道/art.json
--rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.13/arts/life/2022/泉州市丰泽区·雨后街道/index.html
--rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.13/arts/life/2023/更换微信账号了/art.json
--rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.13/arts/life/2023/更换微信账号了/index.html
--rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.13/arts/life/2024/泉州市承天禅寺/art.json
--rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.13/arts/life/2024/泉州市承天禅寺/index.html
--rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.13/arts/miumapp/LICENSE
--rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.13/arts/miumapp/README.md
--rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.13/arts/miumapp/__init__.py
--rw-r--r--   0        0        0     7645 2024-04-12 04:07:11.111023 arts-2024.4.13/arts/miumapp/_core.py
--rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.13/arts/miumapp/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.13/arts/miumapp/licenses/README.md
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/miumapp/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.13/arts/miumapp/licenses/tornado/LICENSE
--rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.13/arts/miumapp/miumapp/__init__.py
--rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.13/arts/miumapp/miumapp/demo.html
--rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.13/arts/miumapp/miumapp/demo.py
--rw-r--r--   0        0        0      644 2024-04-13 08:19:45.878790 arts-2024.4.13/arts/miumapp/pyproject.toml
--rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.13/arts/oodb/LICENSE
--rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.13/arts/oodb/README.md
--rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.13/arts/oodb/__init__.py
--rw-r--r--   0        0        0    19029 2024-03-06 09:46:30.072966 arts-2024.4.13/arts/oodb/_core.py
--rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.13/arts/oodb/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.13/arts/oodb/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.13/arts/oodb/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.13/arts/oodb/oodb.py
--rw-r--r--   0        0        0      627 2024-04-13 08:20:16.552792 arts-2024.4.13/arts/oodb/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.13/arts/oomongo/LICENSE
--rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.13/arts/oomongo/README.md
--rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.13/arts/oomongo/__init__.py
--rw-r--r--   0        0        0    27613 2024-03-06 00:34:47.221863 arts-2024.4.13/arts/oomongo/_core.py
--rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.13/arts/oomongo/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.13/arts/oomongo/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.13/arts/oomongo/licenses/motor/LICENSE
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.13/arts/oomongo/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.13/arts/oomongo/oomongo.py
--rw-r--r--   0        0        0      564 2024-04-13 08:20:16.553795 arts-2024.4.13/arts/oomongo/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.13/arts/oomysql/LICENSE
--rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.13/arts/oomysql/README.md
--rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.13/arts/oomysql/__init__.py
--rw-r--r--   0        0        0    35301 2024-03-24 00:57:24.021318 arts-2024.4.13/arts/oomysql/_core.py
--rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.13/arts/oomysql/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.13/arts/oomysql/licenses/README.md
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.13/arts/oomysql/licenses/aiomysql/LICENSE
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.13/arts/oomysql/licenses/pymysql/LICENSE
--rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.13/arts/oomysql/oomysql.py
--rw-r--r--   0        0        0      642 2024-04-13 08:20:16.553795 arts-2024.4.13/arts/oomysql/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.13/arts/openai2/LICENSE
--rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 arts-2024.4.13/arts/openai2/README.md
--rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 arts-2024.4.13/arts/openai2/__init__.py
--rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 arts-2024.4.13/arts/openai2/_core/chat.py
--rw-r--r--   0        0        0     2286 2024-04-08 06:59:43.786636 arts-2024.4.13/arts/openai2/_core/chat_in_cmd.py
--rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 arts-2024.4.13/arts/openai2/_core/group_chat.py
--rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.13/arts/openai2/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.13/arts/openai2/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.13/arts/openai2/licenses/openai/LICENSE
--rw-r--r--   0        0        0      204 2024-04-07 03:59:45.705745 arts-2024.4.13/arts/openai2/openai2.py
--rw-r--r--   0        0        0      804 2024-04-13 08:15:29.737274 arts-2024.4.13/arts/openai2/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.13/arts/skybox/Copyright
--rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.13/arts/skybox/README.md
--rw-r--r--   0        0        0      320 2024-04-03 06:26:06.014092 arts-2024.4.13/arts/skybox/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.13/arts/skybox/skybox/Copyright
--rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.13/arts/skybox/skybox/__init__.py
--rw-r--r--   0        0        0    12718 2024-04-13 08:14:33.486175 arts-2024.4.13/arts/skybox/skybox/files_hashes
--rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.13/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
--rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.13/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.13/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
--rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.13/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.13/arts/thoughts/2023/专利是个公平的赛道/art.json
--rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.13/arts/thoughts/2023/专利是个公平的赛道/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.13/arts/thoughts/2023/事情的真实性是由度的/art.json
--rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.13/arts/thoughts/2023/事情的真实性是由度的/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.13/arts/thoughts/2023/人无法摆脱兽性/art.json
--rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.13/arts/thoughts/2023/人无法摆脱兽性/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.13/arts/thoughts/2023/什么是极端？/art.json
--rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.13/arts/thoughts/2023/什么是极端？/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.13/arts/thoughts/2023/保护好人/art.json
--rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.13/arts/thoughts/2023/保护好人/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.13/arts/thoughts/2023/只筛选，不教化/art.json
--rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.13/arts/thoughts/2023/只筛选，不教化/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.13/arts/thoughts/2023/喊高考加油是刷存在感/art.json
--rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.13/arts/thoughts/2023/喊高考加油是刷存在感/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.13/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
--rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.13/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.13/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
--rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.13/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.13/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
--rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.13/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.13/arts/thoughts/2023/想去国外了解自己/art.json
--rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.13/arts/thoughts/2023/想去国外了解自己/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.13/arts/thoughts/2023/现代化的分工合作机制/art.json
--rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.13/arts/thoughts/2023/现代化的分工合作机制/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.13/arts/thoughts/2023/用理性处理简单的事情/art.json
--rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.13/arts/thoughts/2023/用理性处理简单的事情/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.13/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
--rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.13/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.13/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
--rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.13/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.13/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
--rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.13/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
--rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.13/arts/thoughts/2024/不要害怕犯错/art.json
--rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.13/arts/thoughts/2024/不要害怕犯错/index.html
--rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.13/arts/thoughts/2024/新年题诗/art.json
--rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.13/arts/thoughts/2024/新年题诗/index.html
--rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.13/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
--rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.13/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
--rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.13/arts/thoughts/2024/编程语言的进化/art.json
--rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.13/arts/thoughts/2024/编程语言的进化/example.html
--rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.13/arts/thoughts/2024/编程语言的进化/index.html
--rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.13/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
--rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.13/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
--rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.13/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
--rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.13/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
--rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.13/arts/tutorials/150-操作MySQL/art.json
--rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.13/arts/tutorials/225-操作MongoDB/art.json
--rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.13/arts/tutorials/300-开发桌面GUI应用/art.json
--rw-r--r--   0        0        0      102 2024-04-13 07:55:06.222216 arts-2024.4.13/arts/tutorials/375-Base95编码/art.json
--rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.13/arts/tutorials/450-对接ChatGPT/art.json
--rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.13/arts/tutorials/525-时间模块/art.json
--rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.13/arts/tutorials/562-面向对象数据库/art.json
--rw-r--r--   0        0        0      470 2024-04-11 14:14:02.840194 arts-2024.4.13/arts/tutorials/581-编程心得/README.md
--rw-r--r--   0        0        0       44 2024-04-11 06:30:42.340203 arts-2024.4.13/arts/tutorials/581-编程心得/art.json
--rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.13/arts/tutorials/600-用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.13/arts/tutorials/600-用37行代码实现AI五子棋/art.json
--rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.13/arts/tutorials/750-正则表达式/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.13/arts/tutorials/750-正则表达式/art.json
--rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.13/arts/videos/200-秦时明月[项羽]·谪居/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.13/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.13/arts/videos/600-楚门的世界·五月雨/art.json
--rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.13/arts/videos/800-AI是这样画包拯的/art.json
--rw-r--r--   0        0        0      525 2024-04-13 08:14:50.653687 arts-2024.4.13/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 arts-2024.4.13/PKG-INFO
+-rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.19/.gitignore
+-rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.19/README.md
+-rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.19/arts/CoolMemory-English/Copyright
+-rw-r--r--   0        0        0    10492 2024-04-12 03:24:43.904296 arts-2024.4.19/arts/CoolMemory-English/README.md
+-rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.19/arts/CoolMemory-English/art.json
+-rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/CoolMemory-English/licenses/README.md
+-rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
+-rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
+-rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
+-rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.19/arts/WeChat-Art-Museum/art.json
+-rw-r--r--   0        0        0    53616 2024-04-13 08:11:29.182384 arts-2024.4.19/arts/WeChat-Art-Museum/index.html
+-rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.19/arts/__init__.py
+-rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.19/arts/articles/010-赚钱宝典/010-财富的本质/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.19/arts/articles/010-赚钱宝典/010-财富的本质/art.json
+-rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.19/arts/articles/010-赚钱宝典/020-商业价值/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.19/arts/articles/010-赚钱宝典/020-商业价值/art.json
+-rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.19/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
+-rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.19/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
+-rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.19/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.19/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
+-rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.19/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.19/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
+-rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.19/arts/articles/150-小民参政/300-广义的民主/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.19/arts/articles/150-小民参政/300-广义的民主/art.json
+-rw-r--r--   0        0        0     3056 2024-04-15 06:41:13.052262 arts-2024.4.19/arts/articles/150-小民参政/450-我们处于史上最好的时代/README.md
+-rw-r--r--   0        0        0       44 2024-04-14 07:59:47.314020 arts-2024.4.19/arts/articles/150-小民参政/450-我们处于史上最好的时代/art.json
+-rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.19/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.19/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
+-rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.19/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.19/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
+-rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.19/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.19/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
+-rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.19/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.19/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
+-rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.19/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.19/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
+-rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.19/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.19/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
+-rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.19/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.19/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
+-rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.19/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.19/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
+-rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.19/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.19/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
+-rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.19/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.19/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
+-rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.19/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.19/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
+-rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.19/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.19/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
+-rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.19/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.19/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
+-rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.19/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.19/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
+-rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.4.19/arts/articles/450-万象思考/700-堕胎自由权/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.19/arts/articles/450-万象思考/700-堕胎自由权/art.json
+-rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.19/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.19/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
+-rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.19/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.19/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
+-rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.19/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.19/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
+-rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.19/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.19/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
+-rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.19/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.19/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
+-rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.19/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
+-rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.19/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
+-rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.19/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.19/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.19/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.19/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.19/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.19/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
+-rw-r--r--   0        0        0    11275 2024-04-13 03:33:01.837811 arts-2024.4.19/arts/base95/LICENSE
+-rw-r--r--   0        0        0     2678 2024-04-19 09:42:08.567290 arts-2024.4.19/arts/base95/README.md
+-rw-r--r--   0        0        0       63 2024-04-19 09:19:32.694427 arts-2024.4.19/arts/base95/__init__.py
+-rw-r--r--   0        0        0     3553 2024-04-19 09:19:14.294026 arts-2024.4.19/arts/base95/_core.py
+-rw-r--r--   0        0        0       98 2024-04-13 08:02:33.643534 arts-2024.4.19/arts/base95/art.json
+-rw-r--r--   0        0        0       74 2024-04-19 09:19:40.646468 arts-2024.4.19/arts/base95/base95.py
+-rw-r--r--   0        0        0      672 2024-04-19 09:47:07.876329 arts-2024.4.19/arts/base95/pyproject.toml
+-rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.19/arts/cooltypes/LICENSE
+-rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.19/arts/cooltypes/__init__.py
+-rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.19/arts/cooltypes/envname/README.md
+-rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.19/arts/cooltypes/envname/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-08 07:02:42.471320 arts-2024.4.19/arts/cooltypes/envname/_core.py
+-rw-r--r--   0        0        0      548 2024-04-08 07:01:42.600503 arts-2024.4.19/arts/cooltypes/moduledb/README.md
+-rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.19/arts/cooltypes/moduledb/__init__.py
+-rw-r--r--   0        0        0     3515 2024-04-08 06:57:45.544745 arts-2024.4.19/arts/cooltypes/moduledb/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.19/arts/cooltypes/modules/coolstr/__init__.py
+-rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.19/arts/cooltypes/modules/coolstr/_core.py
+-rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.19/arts/cooltypes/modules/cooltime/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.19/arts/cooltypes/modules/cooltime/__init__.py
+-rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.19/arts/cooltypes/modules/cooltime/_art.json
+-rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.19/arts/cooltypes/modules/cooltime/_core.py
+-rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.19/arts/cooltypes/modules/rslice/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.19/arts/cooltypes/modules/rslice/__init__.py
+-rw-r--r--   0        0        0     2764 2024-04-15 07:46:47.281317 arts-2024.4.19/arts/cooltypes/modules/rslice/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.19/arts/cooltypes/modules/vtype/__init__.py
+-rw-r--r--   0        0        0    10012 2024-04-13 01:46:07.477663 arts-2024.4.19/arts/cooltypes/modules/vtype/_core.py
+-rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.19/arts/cooltypes/设计.md
+-rw-r--r--   0        0        0    61654 2024-04-14 08:01:25.083311 arts-2024.4.19/arts/index.html
+-rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.19/arts/life/2018/莆田学院·毕业生留影/art.json
+-rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.19/arts/life/2018/莆田学院·毕业生留影/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.19/arts/life/2019/苏州市虎丘山/art.json
+-rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.19/arts/life/2019/苏州市虎丘山/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.19/arts/life/2022/泉州市丰泽区·雨后街道/art.json
+-rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.19/arts/life/2022/泉州市丰泽区·雨后街道/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.19/arts/life/2023/更换微信账号了/art.json
+-rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.19/arts/life/2023/更换微信账号了/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.19/arts/life/2024/泉州市承天禅寺/art.json
+-rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.19/arts/life/2024/泉州市承天禅寺/index.html
+-rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.19/arts/miumapp/LICENSE
+-rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.19/arts/miumapp/README.md
+-rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.19/arts/miumapp/__init__.py
+-rw-r--r--   0        0        0     7645 2024-04-12 04:07:11.111023 arts-2024.4.19/arts/miumapp/_core.py
+-rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.19/arts/miumapp/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19/arts/miumapp/licenses/README.md
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/miumapp/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.19/arts/miumapp/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.19/arts/miumapp/miumapp/__init__.py
+-rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.19/arts/miumapp/miumapp/demo.html
+-rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.19/arts/miumapp/miumapp/demo.py
+-rw-r--r--   0        0        0      644 2024-04-13 08:19:45.878790 arts-2024.4.19/arts/miumapp/pyproject.toml
+-rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.19/arts/oodb/LICENSE
+-rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.19/arts/oodb/README.md
+-rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.19/arts/oodb/__init__.py
+-rw-r--r--   0        0        0    19029 2024-03-06 09:46:30.072966 arts-2024.4.19/arts/oodb/_core.py
+-rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.19/arts/oodb/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19/arts/oodb/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.19/arts/oodb/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.19/arts/oodb/oodb.py
+-rw-r--r--   0        0        0      627 2024-04-13 08:20:16.552792 arts-2024.4.19/arts/oodb/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.19/arts/oomongo/LICENSE
+-rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.19/arts/oomongo/README.md
+-rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.19/arts/oomongo/__init__.py
+-rw-r--r--   0        0        0    27613 2024-04-15 07:46:47.281317 arts-2024.4.19/arts/oomongo/_core.py
+-rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.19/arts/oomongo/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19/arts/oomongo/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.19/arts/oomongo/licenses/motor/LICENSE
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.19/arts/oomongo/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.19/arts/oomongo/oomongo.py
+-rw-r--r--   0        0        0      564 2024-04-13 08:20:16.553795 arts-2024.4.19/arts/oomongo/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.19/arts/oomysql/LICENSE
+-rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.19/arts/oomysql/README.md
+-rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.19/arts/oomysql/__init__.py
+-rw-r--r--   0        0        0    35301 2024-04-15 07:46:47.271326 arts-2024.4.19/arts/oomysql/_core.py
+-rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.19/arts/oomysql/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19/arts/oomysql/licenses/README.md
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.19/arts/oomysql/licenses/aiomysql/LICENSE
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.19/arts/oomysql/licenses/pymysql/LICENSE
+-rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.19/arts/oomysql/oomysql.py
+-rw-r--r--   0        0        0      642 2024-04-13 08:20:16.553795 arts-2024.4.19/arts/oomysql/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.19/arts/openai2/LICENSE
+-rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 arts-2024.4.19/arts/openai2/README.md
+-rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 arts-2024.4.19/arts/openai2/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 arts-2024.4.19/arts/openai2/_core/chat.py
+-rw-r--r--   0        0        0     2286 2024-04-08 06:59:43.786636 arts-2024.4.19/arts/openai2/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 arts-2024.4.19/arts/openai2/_core/group_chat.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.19/arts/openai2/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19/arts/openai2/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.19/arts/openai2/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      204 2024-04-07 03:59:45.705745 arts-2024.4.19/arts/openai2/openai2.py
+-rw-r--r--   0        0        0      804 2024-04-13 08:15:29.737274 arts-2024.4.19/arts/openai2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.19/arts/skybox/Copyright
+-rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.19/arts/skybox/README.md
+-rw-r--r--   0        0        0      321 2024-04-13 08:32:12.081508 arts-2024.4.19/arts/skybox/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.19/arts/skybox/skybox/Copyright
+-rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.19/arts/skybox/skybox/__init__.py
+-rw-r--r--   0        0        0    12359 2024-04-13 09:08:11.529449 arts-2024.4.19/arts/skybox/skybox/files_hashes
+-rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.19/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
+-rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.19/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.19/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
+-rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.19/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.19/arts/thoughts/2023/专利是个公平的赛道/art.json
+-rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.19/arts/thoughts/2023/专利是个公平的赛道/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.19/arts/thoughts/2023/事情的真实性是由度的/art.json
+-rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.19/arts/thoughts/2023/事情的真实性是由度的/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.19/arts/thoughts/2023/人无法摆脱兽性/art.json
+-rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.19/arts/thoughts/2023/人无法摆脱兽性/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.19/arts/thoughts/2023/什么是极端？/art.json
+-rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.19/arts/thoughts/2023/什么是极端？/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.19/arts/thoughts/2023/保护好人/art.json
+-rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.19/arts/thoughts/2023/保护好人/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.19/arts/thoughts/2023/只筛选，不教化/art.json
+-rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.19/arts/thoughts/2023/只筛选，不教化/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.19/arts/thoughts/2023/喊高考加油是刷存在感/art.json
+-rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.19/arts/thoughts/2023/喊高考加油是刷存在感/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.19/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
+-rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.19/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.19/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
+-rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.19/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.19/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
+-rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.19/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.19/arts/thoughts/2023/想去国外了解自己/art.json
+-rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.19/arts/thoughts/2023/想去国外了解自己/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.19/arts/thoughts/2023/现代化的分工合作机制/art.json
+-rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.19/arts/thoughts/2023/现代化的分工合作机制/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.19/arts/thoughts/2023/用理性处理简单的事情/art.json
+-rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.19/arts/thoughts/2023/用理性处理简单的事情/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.19/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
+-rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.19/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.19/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
+-rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.19/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.19/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
+-rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.19/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
+-rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.19/arts/thoughts/2024/不要害怕犯错/art.json
+-rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.19/arts/thoughts/2024/不要害怕犯错/index.html
+-rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.19/arts/thoughts/2024/新年题诗/art.json
+-rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.19/arts/thoughts/2024/新年题诗/index.html
+-rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.19/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
+-rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.19/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.19/arts/thoughts/2024/编程语言的进化/art.json
+-rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.19/arts/thoughts/2024/编程语言的进化/example.html
+-rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.19/arts/thoughts/2024/编程语言的进化/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.19/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
+-rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.19/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
+-rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.19/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
+-rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.19/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
+-rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.19/arts/tutorials/150-操作MySQL/art.json
+-rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.19/arts/tutorials/225-操作MongoDB/art.json
+-rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.19/arts/tutorials/300-开发桌面GUI应用/art.json
+-rw-r--r--   0        0        0      102 2024-04-13 07:55:06.222216 arts-2024.4.19/arts/tutorials/375-Base95编码/art.json
+-rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.19/arts/tutorials/450-对接ChatGPT/art.json
+-rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.19/arts/tutorials/525-时间模块/art.json
+-rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.19/arts/tutorials/562-面向对象数据库/art.json
+-rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.19/arts/tutorials/600-用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.19/arts/tutorials/600-用37行代码实现AI五子棋/art.json
+-rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.19/arts/tutorials/750-正则表达式/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.19/arts/tutorials/750-正则表达式/art.json
+-rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.19/arts/videos/200-秦时明月[项羽]·谪居/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.19/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.19/arts/videos/600-楚门的世界·五月雨/art.json
+-rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.19/arts/videos/800-AI是这样画包拯的/art.json
+-rw-r--r--   0        0        0      525 2024-04-19 09:46:52.877717 arts-2024.4.19/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 arts-2024.4.19/PKG-INFO
```

### Comparing `arts-2024.4.13/.gitignore` & `arts-2024.4.19/.gitignore`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/CoolMemory-English/README.md` & `arts-2024.4.19/arts/CoolMemory-English/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE` & `arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE` & `arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/Python/LICENSE` & `arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/Python/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE` & `arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE` & `arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE` & `arts-2024.4.19/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/WeChat-Art-Museum/index.html` & `arts-2024.4.19/arts/WeChat-Art-Museum/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/010-赚钱宝典/010-财富的本质/README.md` & `arts-2024.4.19/arts/articles/010-赚钱宝典/010-财富的本质/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/010-赚钱宝典/020-商业价值/README.md` & `arts-2024.4.19/arts/articles/010-赚钱宝典/020-商业价值/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md` & `arts-2024.4.19/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md` & `arts-2024.4.19/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md` & `arts-2024.4.19/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/150-小民参政/300-广义的民主/README.md` & `arts-2024.4.19/arts/articles/150-小民参政/300-广义的民主/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md` & `arts-2024.4.19/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md` & `arts-2024.4.19/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md` & `arts-2024.4.19/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md` & `arts-2024.4.19/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md` & `arts-2024.4.19/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/700-堕胎自由权/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/700-堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md` & `arts-2024.4.19/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md` & `arts-2024.4.19/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md` & `arts-2024.4.19/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md` & `arts-2024.4.19/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md` & `arts-2024.4.19/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md` & `arts-2024.4.19/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md` & `arts-2024.4.19/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md` & `arts-2024.4.19/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md` & `arts-2024.4.19/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/base95/LICENSE` & `arts-2024.4.19/arts/base95/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/base95/pyproject.toml` & `arts-2024.4.19/arts/base95/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "base95"
-version = "1.0"
-description = "Base95 是一种用 95 个可见的 ASCII 字符（含空格）表示任意二进制数据的编码方法，具有比 Base64 编码更高的信息密度。"
-dependencies = ["arts>=2024.4.13"]
+version = "2.0"
+description = "Base95 是一种用 95 个可见的 ASCII 字符（含空格）表示任意二进制数据的编码方法，编码后的信息密度高于 Base64 编码。"
+dependencies = ["arts>=2024.4.19"]
 keywords = ["base64", "base85", "base95"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `arts-2024.4.13/arts/cooltypes/LICENSE` & `arts-2024.4.19/arts/cooltypes/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/envname/README.md` & `arts-2024.4.19/arts/cooltypes/envname/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/moduledb/README.md` & `arts-2024.4.19/arts/cooltypes/moduledb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/moduledb/_core.py` & `arts-2024.4.19/arts/cooltypes/moduledb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/modules/coolstr/_core.py` & `arts-2024.4.19/arts/cooltypes/modules/coolstr/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/modules/cooltime/README.md` & `arts-2024.4.19/arts/cooltypes/modules/cooltime/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/modules/cooltime/_core.py` & `arts-2024.4.19/arts/cooltypes/modules/cooltime/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/modules/rslice/README.md` & `arts-2024.4.19/arts/cooltypes/modules/rslice/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/cooltypes/modules/rslice/_core.py` & `arts-2024.4.19/arts/cooltypes/modules/rslice/_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,176 +1,173 @@
-00000000: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000010: 7274 2055 6e69 6f6e 0d0a 0d0a 0d0a 636c  rt Union......cl
-00000020: 6173 7320 5273 6c69 6365 3a0d 0a20 2020  ass Rslice:..   
-00000030: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000040: 6c66 2c20 636f 7265 3a20 556e 696f 6e5b  lf, core: Union[
-00000050: 6c69 7374 2c20 7475 706c 652c 2073 7472  list, tuple, str
-00000060: 5d29 3a20 7365 6c66 2e63 6f72 6520 3d20  ]): self.core = 
-00000070: 636f 7265 0d0a 2020 2020 0d0a 2020 2020  core..    ..    
-00000080: 6465 6620 5f5f 6c65 6e5f 5f28 7365 6c66  def __len__(self
-00000090: 293a 2072 6574 7572 6e20 6c65 6e28 7365  ): return len(se
-000000a0: 6c66 2e63 6f72 6529 0d0a 0d0a 2020 2020  lf.core)....    
-000000b0: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
-000000c0: 7365 6c66 2c20 6b65 7929 3a0d 0a20 2020  self, key):..   
-000000d0: 2020 2020 2063 6f72 6520 3d20 7365 6c66       core = self
-000000e0: 2e63 6f72 650d 0a20 2020 2020 2020 2069  .core..        i
-000000f0: 6620 6973 696e 7374 616e 6365 286b 6579  f isinstance(key
-00000100: 2c20 696e 7429 3a0d 0a20 2020 2020 2020  , int):..       
-00000110: 2020 2020 2069 6620 6b65 7920 3e20 303a       if key > 0:
-00000120: 2072 6574 7572 6e20 636f 7265 5b6b 6579   return core[key
-00000130: 202d 2031 5d0d 0a20 2020 2020 2020 2020   - 1]..         
-00000140: 2020 2069 6620 6b65 7920 3c20 303a 2072     if key < 0: r
-00000150: 6574 7572 6e20 636f 7265 5b6b 6579 5d0d  eturn core[key].
-00000160: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00000170: 6572 7420 6b65 7920 213d 2030 0d0a 2020  ert key != 0..  
-00000180: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00000190: 7461 6e63 6528 6b65 792c 2073 6c69 6365  tance(key, slice
-000001a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000001b0: 4c2c 2052 2c20 5320 3d20 6b65 792e 7374  L, R, S = key.st
-000001c0: 6172 742c 206b 6579 2e73 746f 702c 206b  art, key.stop, k
-000001d0: 6579 2e73 7465 7020 6f72 2031 0d0a 2020  ey.step or 1..  
-000001e0: 2020 2020 2020 2020 2020 744c 2c20 7452            tL, tR
-000001f0: 2c20 7453 203d 2074 7970 6528 4c29 2c20  , tS = type(L), 
-00000200: 7479 7065 2852 292c 2074 7970 6528 5329  type(R), type(S)
-00000210: 0d0a 2020 2020 2020 2020 2020 2020 6173  ..            as
-00000220: 7365 7274 207b 744c 2c20 7452 2c20 7453  sert {tL, tR, tS
-00000230: 7d20 3c3d 207b 696e 742c 2074 7970 6528  } <= {int, type(
-00000240: 4e6f 6e65 297d 0d0a 2020 2020 2020 2020  None)}..        
-00000250: 2020 2020 6173 7365 7274 2030 206e 6f74      assert 0 not
-00000260: 2069 6e20 284c 2c20 5229 0d0a 2020 2020   in (L, R)..    
-00000270: 2020 2020 2020 2020 6173 7365 7274 2053          assert S
-00000280: 203e 2030 0d0a 2020 2020 2020 2020 2020   > 0..          
-00000290: 2020 6966 2027 2d27 2069 6e20 6622 7b4c    if '-' in f"{L
-000002a0: 7d7b 527d 223a 2020 2320 2de6 98af e8b4  }{R}":  # -.....
-000002b0: 9fe5 8fb7 0d0a 2020 2020 2020 2020 2020  ......          
-000002c0: 2020 2020 2020 6c65 6e53 6865 6574 203d        lenSheet =
-000002d0: 206c 656e 2873 656c 6629 0d0a 2020 2020   len(self)..    
-000002e0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
-000002f0: 2d27 2069 6e20 7374 7228 4c29 3a20 4c20  -' in str(L): L 
-00000300: 3d20 6c65 6e53 6865 6574 202b 204c 202b  = lenSheet + L +
-00000310: 2031 2020 2320 52e7 b4a2 e5bc 950d 0a20   1  # R........ 
-00000320: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000330: 6620 272d 2720 696e 2073 7472 2852 293a  f '-' in str(R):
-00000340: 2052 203d 206c 656e 5368 6565 7420 2b20   R = lenSheet + 
-00000350: 5220 2b20 3120 2023 2052 e7b4 a2e5 bc95  R + 1  # R......
-00000360: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000370: 2074 4c20 6973 2074 5220 6973 2069 6e74   tL is tR is int
-00000380: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000390: 2020 2069 6620 6d61 7828 4c2c 2052 2920     if max(L, R) 
-000003a0: 3c20 313a 2072 6574 7572 6e20 636f 7265  < 1: return core
-000003b0: 5b30 3a30 5d0d 0a20 2020 2020 2020 2020  [0:0]..         
-000003c0: 2020 2020 2020 2069 6620 5220 3e3d 204c         if R >= L
-000003d0: 3a20 7265 7475 726e 2063 6f72 655b 6d61  : return core[ma
-000003e0: 7828 302c 4c2d 3129 3a52 3a53 5d0d 0a20  x(0,L-1):R:S].. 
-000003f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00000400: 6620 5220 3e3d 2032 3a20 7265 7475 726e  f R >= 2: return
-00000410: 2063 6f72 655b 4c2d 313a 522d 323a 2d53   core[L-1:R-2:-S
-00000420: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00000430: 2020 2072 6574 7572 6e20 636f 7265 5b4c     return core[L
-00000440: 2d31 3a4e 6f6e 653a 2d53 5d0d 0a20 2020  -1:None:-S]..   
-00000450: 2020 2020 2020 2020 2065 6c69 6620 744c           elif tL
-00000460: 2069 7320 696e 743a 0d0a 2020 2020 2020   is int:..      
-00000470: 2020 2020 2020 2020 2020 6966 204c 203e            if L >
-00000480: 2030 3a20 7265 7475 726e 2063 6f72 655b   0: return core[
-00000490: 4c2d 313a 4e6f 6e65 3a53 5d0d 0a20 2020  L-1:None:S]..   
-000004a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000004b0: 7572 6e20 636f 7265 5b4c 3a4e 6f6e 653a  urn core[L:None:
-000004c0: 535d 0d0a 2020 2020 2020 2020 2020 2020  S]..            
-000004d0: 656c 6966 2074 5220 6973 2069 6e74 3a0d  elif tR is int:.
-000004e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004f0: 2069 6620 5220 3e3d 2031 3a20 7265 7475   if R >= 1: retu
-00000500: 726e 2063 6f72 655b 4e6f 6e65 3a52 3a53  rn core[None:R:S
-00000510: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00000520: 2020 2069 6620 5220 3d3d 2030 3a20 7265     if R == 0: re
-00000530: 7475 726e 2063 6f72 655b 303a 303a 535d  turn core[0:0:S]
-00000540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000550: 2020 6966 2052 203d 3d20 2d31 3a20 7265    if R == -1: re
-00000560: 7475 726e 2063 6f72 655b 4e6f 6e65 3a4e  turn core[None:N
-00000570: 6f6e 653a 535d 0d0a 2020 2020 2020 2020  one:S]..        
-00000580: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00000590: 6f72 655b 4e6f 6e65 3a52 202b 2031 5d0d  ore[None:R + 1].
-000005a0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000005b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000005c0: 2020 2020 7265 7475 726e 2063 6f72 655b      return core[
-000005d0: 4e6f 6e65 3a4e 6f6e 653a 535d 0d0a 2020  None:None:S]..  
-000005e0: 2020 2020 2020 7261 6973 6520 4b65 7945        raise KeyE
-000005f0: 7272 6f72 286b 6579 290d 0a20 2020 200d  rror(key)..    .
-00000600: 0a20 2020 2064 6566 205f 5f73 6574 6974  .    def __setit
-00000610: 656d 5f5f 2873 656c 662c 206b 6579 2c20  em__(self, key, 
-00000620: 7661 6c75 6529 3a0d 0a20 2020 2020 2020  value):..       
-00000630: 2073 656c 662e 636f 7265 5b73 656c 662e   self.core[self.
-00000640: 5f73 6574 6974 656d 4261 7365 286b 6579  _setitemBase(key
-00000650: 295d 203d 2076 616c 7565 0d0a 2020 2020  )] = value..    
-00000660: 0d0a 2020 2020 6465 6620 5f73 6574 6974  ..    def _setit
-00000670: 656d 4261 7365 2873 656c 662c 206b 6579  emBase(self, key
-00000680: 293a 0d0a 2020 2020 2020 2020 6966 2069  ):..        if i
-00000690: 7369 6e73 7461 6e63 6528 6b65 792c 2069  sinstance(key, i
-000006a0: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
-000006b0: 2020 6966 206b 6579 203e 2030 3a20 7265    if key > 0: re
-000006c0: 7475 726e 206b 6579 202d 2031 0d0a 2020  turn key - 1..  
-000006d0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
-000006e0: 203c 2030 3a20 7265 7475 726e 206b 6579   < 0: return key
-000006f0: 0d0a 2020 2020 2020 2020 2020 2020 6173  ..            as
-00000700: 7365 7274 206b 6579 2021 3d20 300d 0a20  sert key != 0.. 
-00000710: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00000720: 7374 616e 6365 286b 6579 2c20 736c 6963  stance(key, slic
-00000730: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00000740: 204c 2c20 522c 2053 203d 206b 6579 2e73   L, R, S = key.s
-00000750: 7461 7274 2c20 6b65 792e 7374 6f70 2c20  tart, key.stop, 
-00000760: 6b65 792e 7374 6570 206f 7220 310d 0a20  key.step or 1.. 
-00000770: 2020 2020 2020 2020 2020 2074 4c2c 2074             tL, t
-00000780: 522c 2074 5320 3d20 7479 7065 284c 292c  R, tS = type(L),
-00000790: 2074 7970 6528 5229 2c20 7479 7065 2853   type(R), type(S
-000007a0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-000007b0: 7373 6572 7420 7b74 4c2c 2074 522c 2074  ssert {tL, tR, t
-000007c0: 537d 203c 3d20 7b69 6e74 2c20 7479 7065  S} <= {int, type
-000007d0: 284e 6f6e 6529 7d0d 0a20 2020 2020 2020  (None)}..       
-000007e0: 2020 2020 2061 7373 6572 7420 3020 6e6f       assert 0 no
-000007f0: 7420 696e 2028 4c2c 2052 290d 0a20 2020  t in (L, R)..   
-00000800: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00000810: 5320 3e20 300d 0a20 2020 2020 2020 2020  S > 0..         
-00000820: 2020 2069 6620 272d 2720 696e 2066 227b     if '-' in f"{
-00000830: 4c7d 7b52 7d22 3a20 2023 202d e698 afe8  L}{R}":  # -....
-00000840: b49f e58f b70d 0a20 2020 2020 2020 2020  .......         
-00000850: 2020 2020 2020 206c 656e 5368 6565 7420         lenSheet 
-00000860: 3d20 6c65 6e28 7365 6c66 290d 0a20 2020  = len(self)..   
-00000870: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000880: 272d 2720 696e 2073 7472 284c 293a 204c  '-' in str(L): L
-00000890: 203d 206c 656e 5368 6565 7420 2b20 4c20   = lenSheet + L 
-000008a0: 2b20 3120 2023 2052 e7b4 a2e5 bc95 0d0a  + 1  # R........
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 6966 2027 2d27 2069 6e20 7374 7228 5229  if '-' in str(R)
-000008d0: 3a20 5220 3d20 6c65 6e53 6865 6574 202b  : R = lenSheet +
-000008e0: 2052 202b 2031 2020 2320 52e7 b4a2 e5bc   R + 1  # R.....
-000008f0: 950d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00000900: 6620 744c 2069 7320 7452 2069 7320 696e  f tL is tR is in
-00000910: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00000920: 2020 2020 6966 2052 3c4c 3a20 4c2c 5220      if R<L: L,R 
-00000930: 3d20 522c 4c0d 0a20 2020 2020 2020 2020  = R,L..         
-00000940: 2020 2020 2020 2069 6620 5220 3c20 313a         if R < 1:
-00000950: 2072 6574 7572 6e20 736c 6963 6528 4e6f   return slice(No
-00000960: 6e65 2c20 3029 2020 2320 e5b7 a6e4 bea7  ne, 0)  # ......
-00000970: e68f 92e5 85a5 0d0a 2020 2020 2020 2020  ........        
-00000980: 2020 2020 2020 2020 6966 204c 203e 2030          if L > 0
-00000990: 3a20 7265 7475 726e 2073 6c69 6365 284c  : return slice(L
-000009a0: 2d31 2c20 522c 204e 6f6e 6529 0d0a 2020  -1, R, None)..  
-000009b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000009c0: 7475 726e 2073 6c69 6365 284e 6f6e 652c  turn slice(None,
-000009d0: 2052 2c20 4e6f 6e65 290d 0a20 2020 2020   R, None)..     
-000009e0: 2020 2020 2020 2065 6c69 6620 744c 2069         elif tL i
-000009f0: 7320 696e 743a 0d0a 2020 2020 2020 2020  s int:..        
-00000a00: 2020 2020 2020 2020 6966 204c 203e 2030          if L > 0
-00000a10: 3a20 7265 7475 726e 2073 6c69 6365 284c  : return slice(L
-00000a20: 2d31 2c20 4e6f 6e65 290d 0a20 2020 2020  -1, None)..     
-00000a30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000a40: 6e20 736c 6963 6528 4e6f 6e65 2c20 4e6f  n slice(None, No
-00000a50: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-00000a60: 2065 6c69 6620 7452 2069 7320 696e 743a   elif tR is int:
-00000a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000a80: 2020 7265 7475 726e 2073 6c69 6365 284e    return slice(N
-00000a90: 6f6e 652c 2052 290d 0a20 2020 2020 2020  one, R)..       
-00000aa0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000ab0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000ac0: 726e 2073 6c69 6365 284e 6f6e 652c 204e  rn slice(None, N
-00000ad0: 6f6e 6529 0d0a 2020 2020 2020 2020 7261  one)..        ra
-00000ae0: 6973 6520 4b65 7945 7272 6f72 286b 6579  ise KeyError(key
-00000af0: 29                                       )
+00000000: 0d0a 636c 6173 7320 5273 6c69 6365 3a0d  ..class Rslice:.
+00000010: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00000020: 5f28 7365 6c66 2c20 636f 7265 3a20 6c69  _(self, core: li
+00000030: 7374 7c74 7570 6c65 7c73 7472 293a 2073  st|tuple|str): s
+00000040: 656c 662e 636f 7265 203d 2063 6f72 650d  elf.core = core.
+00000050: 0a20 2020 200d 0a20 2020 2064 6566 205f  .    ..    def _
+00000060: 5f6c 656e 5f5f 2873 656c 6629 3a20 7265  _len__(self): re
+00000070: 7475 726e 206c 656e 2873 656c 662e 636f  turn len(self.co
+00000080: 7265 290d 0a0d 0a20 2020 2064 6566 205f  re)....    def _
+00000090: 5f67 6574 6974 656d 5f5f 2873 656c 662c  _getitem__(self,
+000000a0: 206b 6579 293a 0d0a 2020 2020 2020 2020   key):..        
+000000b0: 636f 7265 203d 2073 656c 662e 636f 7265  core = self.core
+000000c0: 0d0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+000000d0: 6e73 7461 6e63 6528 6b65 792c 2069 6e74  nstance(key, int
+000000e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000000f0: 6966 206b 6579 203e 2030 3a20 7265 7475  if key > 0: retu
+00000100: 726e 2063 6f72 655b 6b65 7920 2d20 315d  rn core[key - 1]
+00000110: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000120: 206b 6579 203c 2030 3a20 7265 7475 726e   key < 0: return
+00000130: 2063 6f72 655b 6b65 795d 0d0a 2020 2020   core[key]..    
+00000140: 2020 2020 2020 2020 6173 7365 7274 206b          assert k
+00000150: 6579 2021 3d20 300d 0a20 2020 2020 2020  ey != 0..       
+00000160: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00000170: 286b 6579 2c20 736c 6963 6529 3a0d 0a20  (key, slice):.. 
+00000180: 2020 2020 2020 2020 2020 204c 2c20 522c             L, R,
+00000190: 2053 203d 206b 6579 2e73 7461 7274 2c20   S = key.start, 
+000001a0: 6b65 792e 7374 6f70 2c20 6b65 792e 7374  key.stop, key.st
+000001b0: 6570 206f 7220 310d 0a20 2020 2020 2020  ep or 1..       
+000001c0: 2020 2020 2074 4c2c 2074 522c 2074 5320       tL, tR, tS 
+000001d0: 3d20 7479 7065 284c 292c 2074 7970 6528  = type(L), type(
+000001e0: 5229 2c20 7479 7065 2853 290d 0a20 2020  R), type(S)..   
+000001f0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00000200: 7b74 4c2c 2074 522c 2074 537d 203c 3d20  {tL, tR, tS} <= 
+00000210: 7b69 6e74 2c20 7479 7065 284e 6f6e 6529  {int, type(None)
+00000220: 7d0d 0a20 2020 2020 2020 2020 2020 2061  }..            a
+00000230: 7373 6572 7420 3020 6e6f 7420 696e 2028  ssert 0 not in (
+00000240: 4c2c 2052 290d 0a20 2020 2020 2020 2020  L, R)..         
+00000250: 2020 2061 7373 6572 7420 5320 3e20 300d     assert S > 0.
+00000260: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000270: 272d 2720 696e 2066 227b 4c7d 7b52 7d22  '-' in f"{L}{R}"
+00000280: 3a20 2023 202d e698 afe8 b49f e58f b70d  :  # -..........
+00000290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000002a0: 206c 656e 5368 6565 7420 3d20 6c65 6e28   lenSheet = len(
+000002b0: 7365 6c66 290d 0a20 2020 2020 2020 2020  self)..         
+000002c0: 2020 2020 2020 2069 6620 272d 2720 696e         if '-' in
+000002d0: 2073 7472 284c 293a 204c 203d 206c 656e   str(L): L = len
+000002e0: 5368 6565 7420 2b20 4c20 2b20 3120 2023  Sheet + L + 1  #
+000002f0: 2052 e7b4 a2e5 bc95 0d0a 2020 2020 2020   R........      
+00000300: 2020 2020 2020 2020 2020 6966 2027 2d27            if '-'
+00000310: 2069 6e20 7374 7228 5229 3a20 5220 3d20   in str(R): R = 
+00000320: 6c65 6e53 6865 6574 202b 2052 202b 2031  lenSheet + R + 1
+00000330: 2020 2320 52e7 b4a2 e5bc 950d 0a20 2020    # R........   
+00000340: 2020 2020 2020 2020 2069 6620 744c 2069           if tL i
+00000350: 7320 7452 2069 7320 696e 743a 0d0a 2020  s tR is int:..  
+00000360: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000370: 206d 6178 284c 2c20 5229 203c 2031 3a20   max(L, R) < 1: 
+00000380: 7265 7475 726e 2063 6f72 655b 303a 305d  return core[0:0]
+00000390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000003a0: 2020 6966 2052 203e 3d20 4c3a 2072 6574    if R >= L: ret
+000003b0: 7572 6e20 636f 7265 5b6d 6178 2830 2c4c  urn core[max(0,L
+000003c0: 2d31 293a 523a 535d 0d0a 2020 2020 2020  -1):R:S]..      
+000003d0: 2020 2020 2020 2020 2020 6966 2052 203e            if R >
+000003e0: 3d20 323a 2072 6574 7572 6e20 636f 7265  = 2: return core
+000003f0: 5b4c 2d31 3a52 2d32 3a2d 535d 0d0a 2020  [L-1:R-2:-S]..  
+00000400: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000410: 7475 726e 2063 6f72 655b 4c2d 313a 4e6f  turn core[L-1:No
+00000420: 6e65 3a2d 535d 0d0a 2020 2020 2020 2020  ne:-S]..        
+00000430: 2020 2020 656c 6966 2074 4c20 6973 2069      elif tL is i
+00000440: 6e74 3a0d 0a20 2020 2020 2020 2020 2020  nt:..           
+00000450: 2020 2020 2069 6620 4c20 3e20 303a 2072       if L > 0: r
+00000460: 6574 7572 6e20 636f 7265 5b4c 2d31 3a4e  eturn core[L-1:N
+00000470: 6f6e 653a 535d 0d0a 2020 2020 2020 2020  one:S]..        
+00000480: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00000490: 6f72 655b 4c3a 4e6f 6e65 3a53 5d0d 0a20  ore[L:None:S].. 
+000004a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000004b0: 7452 2069 7320 696e 743a 0d0a 2020 2020  tR is int:..    
+000004c0: 2020 2020 2020 2020 2020 2020 6966 2052              if R
+000004d0: 203e 3d20 313a 2072 6574 7572 6e20 636f   >= 1: return co
+000004e0: 7265 5b4e 6f6e 653a 523a 535d 0d0a 2020  re[None:R:S]..  
+000004f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000500: 2052 203d 3d20 303a 2072 6574 7572 6e20   R == 0: return 
+00000510: 636f 7265 5b30 3a30 3a53 5d0d 0a20 2020  core[0:0:S]..   
+00000520: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000530: 5220 3d3d 202d 313a 2072 6574 7572 6e20  R == -1: return 
+00000540: 636f 7265 5b4e 6f6e 653a 4e6f 6e65 3a53  core[None:None:S
+00000550: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00000560: 2020 2072 6574 7572 6e20 636f 7265 5b4e     return core[N
+00000570: 6f6e 653a 5220 2b20 315d 0d0a 2020 2020  one:R + 1]..    
+00000580: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000590: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000005a0: 6574 7572 6e20 636f 7265 5b4e 6f6e 653a  eturn core[None:
+000005b0: 4e6f 6e65 3a53 5d0d 0a20 2020 2020 2020  None:S]..       
+000005c0: 2072 6169 7365 204b 6579 4572 726f 7228   raise KeyError(
+000005d0: 6b65 7929 0d0a 2020 2020 0d0a 2020 2020  key)..    ..    
+000005e0: 6465 6620 5f5f 7365 7469 7465 6d5f 5f28  def __setitem__(
+000005f0: 7365 6c66 2c20 6b65 792c 2076 616c 7565  self, key, value
+00000600: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00000610: 2e63 6f72 655b 7365 6c66 2e5f 7365 7469  .core[self._seti
+00000620: 7465 6d42 6173 6528 6b65 7929 5d20 3d20  temBase(key)] = 
+00000630: 7661 6c75 650d 0a20 2020 200d 0a20 2020  value..    ..   
+00000640: 2064 6566 205f 7365 7469 7465 6d42 6173   def _setitemBas
+00000650: 6528 7365 6c66 2c20 6b65 7929 3a0d 0a20  e(self, key):.. 
+00000660: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00000670: 616e 6365 286b 6579 2c20 696e 7429 3a0d  ance(key, int):.
+00000680: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000690: 6b65 7920 3e20 303a 2072 6574 7572 6e20  key > 0: return 
+000006a0: 6b65 7920 2d20 310d 0a20 2020 2020 2020  key - 1..       
+000006b0: 2020 2020 2069 6620 6b65 7920 3c20 303a       if key < 0:
+000006c0: 2072 6574 7572 6e20 6b65 790d 0a20 2020   return key..   
+000006d0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000006e0: 6b65 7920 213d 2030 0d0a 2020 2020 2020  key != 0..      
+000006f0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00000700: 6528 6b65 792c 2073 6c69 6365 293a 0d0a  e(key, slice):..
+00000710: 2020 2020 2020 2020 2020 2020 4c2c 2052              L, R
+00000720: 2c20 5320 3d20 6b65 792e 7374 6172 742c  , S = key.start,
+00000730: 206b 6579 2e73 746f 702c 206b 6579 2e73   key.stop, key.s
+00000740: 7465 7020 6f72 2031 0d0a 2020 2020 2020  tep or 1..      
+00000750: 2020 2020 2020 744c 2c20 7452 2c20 7453        tL, tR, tS
+00000760: 203d 2074 7970 6528 4c29 2c20 7479 7065   = type(L), type
+00000770: 2852 292c 2074 7970 6528 5329 0d0a 2020  (R), type(S)..  
+00000780: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00000790: 207b 744c 2c20 7452 2c20 7453 7d20 3c3d   {tL, tR, tS} <=
+000007a0: 207b 696e 742c 2074 7970 6528 4e6f 6e65   {int, type(None
+000007b0: 297d 0d0a 2020 2020 2020 2020 2020 2020  )}..            
+000007c0: 6173 7365 7274 2030 206e 6f74 2069 6e20  assert 0 not in 
+000007d0: 284c 2c20 5229 0d0a 2020 2020 2020 2020  (L, R)..        
+000007e0: 2020 2020 6173 7365 7274 2053 203e 2030      assert S > 0
+000007f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000800: 2027 2d27 2069 6e20 6622 7b4c 7d7b 527d   '-' in f"{L}{R}
+00000810: 223a 2020 2320 2de6 98af e8b4 9fe5 8fb7  ":  # -.........
+00000820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000830: 2020 6c65 6e53 6865 6574 203d 206c 656e    lenSheet = len
+00000840: 2873 656c 6629 0d0a 2020 2020 2020 2020  (self)..        
+00000850: 2020 2020 2020 2020 6966 2027 2d27 2069          if '-' i
+00000860: 6e20 7374 7228 4c29 3a20 4c20 3d20 6c65  n str(L): L = le
+00000870: 6e53 6865 6574 202b 204c 202b 2031 2020  nSheet + L + 1  
+00000880: 2320 52e7 b4a2 e5bc 950d 0a20 2020 2020  # R........     
+00000890: 2020 2020 2020 2020 2020 2069 6620 272d             if '-
+000008a0: 2720 696e 2073 7472 2852 293a 2052 203d  ' in str(R): R =
+000008b0: 206c 656e 5368 6565 7420 2b20 5220 2b20   lenSheet + R + 
+000008c0: 3120 2023 2052 e7b4 a2e5 bc95 0d0a 2020  1  # R........  
+000008d0: 2020 2020 2020 2020 2020 6966 2074 4c20            if tL 
+000008e0: 6973 2074 5220 6973 2069 6e74 3a0d 0a20  is tR is int:.. 
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000900: 6620 523c 4c3a 204c 2c52 203d 2052 2c4c  f R<L: L,R = R,L
+00000910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000920: 2020 6966 2052 203c 2031 3a20 7265 7475    if R < 1: retu
+00000930: 726e 2073 6c69 6365 284e 6f6e 652c 2030  rn slice(None, 0
+00000940: 2920 2023 20e5 b7a6 e4be a7e6 8f92 e585  )  # ...........
+00000950: a50d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00000960: 2020 2069 6620 4c20 3e20 303a 2072 6574     if L > 0: ret
+00000970: 7572 6e20 736c 6963 6528 4c2d 312c 2052  urn slice(L-1, R
+00000980: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
+00000990: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000009a0: 736c 6963 6528 4e6f 6e65 2c20 522c 204e  slice(None, R, N
+000009b0: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+000009c0: 2020 656c 6966 2074 4c20 6973 2069 6e74    elif tL is int
+000009d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000009e0: 2020 2069 6620 4c20 3e20 303a 2072 6574     if L > 0: ret
+000009f0: 7572 6e20 736c 6963 6528 4c2d 312c 204e  urn slice(L-1, N
+00000a00: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
+00000a10: 2020 2020 2020 7265 7475 726e 2073 6c69        return sli
+00000a20: 6365 284e 6f6e 652c 204e 6f6e 6529 0d0a  ce(None, None)..
+00000a30: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00000a40: 2074 5220 6973 2069 6e74 3a0d 0a20 2020   tR is int:..   
+00000a50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000a60: 7572 6e20 736c 6963 6528 4e6f 6e65 2c20  urn slice(None, 
+00000a70: 5229 0d0a 2020 2020 2020 2020 2020 2020  R)..            
+00000a80: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00000a90: 2020 2020 2020 2072 6574 7572 6e20 736c         return sl
+00000aa0: 6963 6528 4e6f 6e65 2c20 4e6f 6e65 290d  ice(None, None).
+00000ab0: 0a20 2020 2020 2020 2072 6169 7365 204b  .        raise K
+00000ac0: 6579 4572 726f 7228 6b65 7929            eyError(key)
```

### Comparing `arts-2024.4.13/arts/cooltypes/modules/vtype/_core.py` & `arts-2024.4.19/arts/cooltypes/modules/vtype/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/index.html` & `arts-2024.4.19/arts/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 <!DOCTYPE html>
 <html class='ch_157 ch_158'><head>
 <title id=ch_150>江南雨上</title><meta name='msvalidate.01' content='FFA2094263C9178678410FC784304549'><meta name='google-site-verification' content='UNx53G5kjiaAzNZavgTE604GQpveJ6pEtTPi3IMDfPg'><meta charset='utf-8'><meta name='viewport' content='width=device-width, initial-scale=1.0'>
 <style>
     * {vertical-align:middle; text-decoration:none; position:relative; padding:0; overflow:auto; outline:none; margin:0; font-family:'Chinese Quote', 'Segoe UI', Roboto, RobotoNum, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'Helvetica Neue', Helvetica, Arial, sans-serif; box-sizing:border-box; border-width:0; border-style:solid;}
     .ch_157 {width:100vw; height:100vh; display:block; background-color:white;}
-    .ch_185 {display:inline-block; align-self:end;}
+    .ch_186 {display:inline-block; align-self:end;}
     .ch_187 {display:inline-block; align-self:start;}
     .ch_159 {width:100%; padding:0.5rem 0 0 0; height:100%; grid-auto-rows:3rem 1fr; display:inline-grid; background-color:white;}
     .ch_170 {z-index:100; width:100%; min-height:calc(100vh - 3rem - 3.1rem); display:inline-grid; align-content:start;}
     .ch_171 {padding:0 1.25rem; margin:0.5rem 0; justify-content:flex-start; font-weight:500; font-size:1.5rem; display:inline-grid; color:rgb(225, 172, 12);}
-    .ch_175 {width:15rem; text-decoration:none; height:9.27rem; grid-template-rows:1fr auto; display:inline-grid; color:black; background-size:cover; background-color:rgb(255, 237, 195);}
+    .ch_174 {width:15rem; text-decoration:none; height:9.27rem; grid-template-rows:1fr auto; display:inline-grid; color:black; background-size:cover; background-color:rgb(255, 237, 195);}
     .ch_176 {width:100%; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-size:1.1rem; display:inline-grid; align-items:center;}
     .ch_177 {padding:0 0.25rem 0.25rem 0.25rem; justify-items:end; display:inline-grid; color:green; align-items:end;}
     .ch_178 {width:100%; display:inline-grid;}
     .ch_180 {width:100%; text-shadow:black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-weight:600; font-size:1.2rem; display:inline-grid; color:white; align-items:center; -webkit-font-smoothing:antialiased;}
     .ch_181 {display:inline-grid;}
-    .ch_184 {row-gap:0.5rem; justify-items:center; justify-content:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; align-content:center;}
-    body[is_x_screen='False'] .ch_183 {grid-auto-flow:row; display:inline-grid;}
-    body[is_x_screen='False'] .ch_186 {padding:1.5em 0 0 0; display:inline-grid; color:rgb(225, 172, 12);}
-    .ch_161 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; max-width:100%; margin:0 1.25rem; justify-content:space-between; display:inline-block; background-color:white; -ms-overflow-style:none;}
-    .ch_160::-webkit-scrollbar {display:none;}
+    .ch_183 {row-gap:0.5rem; justify-items:center; justify-content:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; align-content:center;}
+    body[is_x_screen='False'] .ch_184 {grid-auto-flow:row; display:inline-grid;}
+    body[is_x_screen='False'] .ch_185 {padding:1.5em 0 0 0; display:inline-grid; color:rgb(225, 172, 12);}
+    .ch_160 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; max-width:100%; margin:0 1.25rem; justify-content:space-between; display:inline-block; background-color:white; -ms-overflow-style:none;}
+    .ch_161::-webkit-scrollbar {display:none;}
     .ch_172 {row-gap:1.5rem; justify-content:center; grid-template-columns:repeat(auto-fill, 15rem); display:inline-grid; column-gap:1.5rem;}
     .ch_163 {padding:0.618em 1em 0.618em 1em; font-size:1rem; border-radius:3em; background-color:transparent;}
-    body[is_x_screen='True'] .ch_164:not([is_current_nav="True"]):hover {background-color:rgba(247, 215, 114, 0.45);}
-    .ch_162[is_current_nav="True"] {background-color:rgba(247, 215, 114, 1);}
-    .ch_165 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
-    .ch_168:not(.ch_exec_goto_scrollLeft) {scroll-snap-type:x mandatory;}
-    .ch_167::-webkit-scrollbar {display:none;}
-    .ch_166 > * {white-space:normal;}
+    body[is_x_screen='True'] .ch_162:not([is_current_nav="True"]):hover {background-color:rgba(247, 215, 114, 0.45);}
+    .ch_164[is_current_nav="True"] {background-color:rgba(247, 215, 114, 1);}
+    .ch_167 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
+    .ch_166:not(.ch_exec_goto_scrollLeft) {scroll-snap-type:x mandatory;}
+    .ch_165::-webkit-scrollbar {display:none;}
+    .ch_168 > * {white-space:normal;}
     .ch_169 {width:100%; scroll-snap-align:start; padding:0; overflow:auto; margin:0; height:100%; flex-wrap:wrap; display:inline-flex;}
     .ch_191 {vertical-align:middle;}
     .ch_189 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
     .ch_188:hover {color:rgb(0, 55, 255);}
     .ch_190:visited {color:rgba(0, 89, 255, 0.758);}
     .ch_179 {border-width:0.02rem; border-color:rgb(205, 205, 205);}
     .ch_182 {margin:1em 0; justify-self:center; font-weight:500; font-size:1.5rem; color:rgb(225, 172, 12);}
-    .ch_173:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
-    .ch_174:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
+    .ch_175:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
+    .ch_173:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
 </style></head>
 <body class='ch_159'>
 <script>
 "use strict";
 
                     if (1 + 1 === 2) {
                         window.ch = new Proxy(
@@ -49,15 +49,15 @@
                         )
                     }
                     else {
                         window.ch = {}
                         console.log('type(ch) is not Map !')
                     }
                 
-</script><div class='ch_160 ch_161' id=ch_127><button class='is_nav ch_162 ch_163 ch_164' is_current_nav='True'>动态</button><button class='is_nav ch_162 ch_163 ch_164'>视频</button><button class='is_nav ch_162 ch_163 ch_164'>文章</button><button class='is_nav ch_162 ch_163 ch_164'>想法</button><button class='is_nav ch_162 ch_163 ch_164'>软件</button><button class='is_nav ch_162 ch_163 ch_164'>Python教程</button><button class='is_nav ch_162 ch_163 ch_164'>生活</button><button class='is_nav ch_162 ch_163 ch_164'>自述</button></div><div class='ch_165 ch_166 ch_167 ch_168' id=ch_142><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-04-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a></div><div class='ch_171'>2024-04-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/581-编程心得/README.md' target='_blank'><div class='ch_176'>编程心得</div><div class='ch_177'>2024-04-11</div></a></div><div class='ch_171'>2024-03-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_109></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_13></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a></div><div class='ch_171'>2024-02-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a></div><div class='ch_171'>2024-01-30</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a></div><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_17></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_21></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_25></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_29></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_33></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-12-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a></div><div class='ch_171'>2023-12-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><div class='ch_171'>2023-12-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a></div><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_37></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_41></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-24</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><div class='ch_171'>2023-10-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a></div><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_113></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a></div><div class='ch_171'>2023-09-20</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a></div><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_45></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_49></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_53></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_57></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-17</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a></div><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_61></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_65></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_69></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_73></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_77></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_81></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a></div><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_85></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-04</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a></div><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_89></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a></div><div class='ch_171'>2023-06-19</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div><div class='ch_171'>2023-06-18</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_93></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_97></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-26</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a></div><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_101></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-03-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a></div><div class='ch_171'>2023-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a></div><div class='ch_171'>2022-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><div class='ch_171'>2022-12-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a></div><div class='ch_171'>2022-12-16</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a></div><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_117></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-09-27</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a></div><div class='ch_171'>2022-09-21</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a></div><div class='ch_171'>2022-09-08</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a></div><div class='ch_171'>2022-08-12</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div><div class='ch_171'>2022-08-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a></div><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_105></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2021-07-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div><div class='ch_171'>2021-06-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><div class='ch_171'>2021-06-10</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a></div><div class='ch_171'>2021-06-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a></div><div class='ch_171'>2021-06-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a></div><div class='ch_171'>2021-06-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a></div><div class='ch_171'>2021-06-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a></div><div class='ch_171'>2021-06-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a></div><div class='ch_171'>2021-06-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a></div><div class='ch_171'>2020-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><div class='ch_171'>2019-08-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a></div><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_121></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_125></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>videos</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>赚钱宝典</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><h3 class='ch_182'>追英赶美</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><h3 class='ch_182'>小民参政</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><h3 class='ch_182'>批判那些伪文艺</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>万象思考</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>时空猜想</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><h3 class='ch_182'>论时事</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><h3 class='ch_182'>小说 / 陆小凤新传</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><h3 class='ch_182'>小说 / 一念天堂</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_10></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_15></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_19></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_23></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_27></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_31></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_35></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_39></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_43></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_47></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_51></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_55></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_59></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_63></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_67></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_71></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_75></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_79></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_83></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_87></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_91></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_95></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_99></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_103></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>software</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>tutorials</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/581-编程心得/README.md' target='_blank'><div class='ch_176'>编程心得</div><div class='ch_177'>2024-04-11</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_107></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_111></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_115></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_119></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_123></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170' style="align-content:stretch;"><div class='ch_183 ch_184'><div class='ch_185 ch_186'>邮箱</div><div class='ch_187'><a class='ch_188 ch_189 ch_190' href='mailto:lcctoor@outlook.com'>lcctoor@outlook.com</a></div><div class='ch_185 ch_186'>微信</div><div class='ch_187'><img class='ch_191' src='./ip_static/WeChatQRC.jpg' style="max-width:15rem; height:auto;"></div><div class='ch_185 ch_186'>捐赠</div><div class='ch_187'><img class='ch_191' src='./ip_static/DonationQRC-0rmb.jpg' style="max-width:15rem; height:auto;"></div></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div></div>
+</script><div class='ch_160 ch_161' id=ch_127><button class='ch_162 is_nav ch_163 ch_164' is_current_nav='True'>动态</button><button class='ch_162 is_nav ch_163 ch_164'>视频</button><button class='ch_162 is_nav ch_163 ch_164'>文章</button><button class='ch_162 is_nav ch_163 ch_164'>想法</button><button class='ch_162 is_nav ch_163 ch_164'>软件</button><button class='ch_162 is_nav ch_163 ch_164'>Python教程</button><button class='ch_162 is_nav ch_163 ch_164'>生活</button><button class='ch_162 is_nav ch_163 ch_164'>自述</button></div><div class='ch_165 ch_166 ch_167 ch_168' id=ch_142><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-04-14</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/450-我们处于史上最好的时代/README.md' target='_blank'><div class='ch_176'>我们处于史上最好的时代</div><div class='ch_177'>2024-04-14</div></a></div><div class='ch_171'>2024-04-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a></div><div class='ch_171'>2024-03-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_109></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_13></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a></div><div class='ch_171'>2024-02-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a></div><div class='ch_171'>2024-01-30</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a></div><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_17></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_21></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_25></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_29></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_33></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-12-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a></div><div class='ch_171'>2023-12-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><div class='ch_171'>2023-12-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a></div><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_37></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_41></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-24</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><div class='ch_171'>2023-10-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a></div><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_113></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a></div><div class='ch_171'>2023-09-20</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a></div><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_45></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_49></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_53></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_57></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-17</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a></div><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_61></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_65></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_69></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_73></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_77></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_81></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a></div><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_85></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-04</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a></div><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_89></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a></div><div class='ch_171'>2023-06-19</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div><div class='ch_171'>2023-06-18</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_93></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_97></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-26</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a></div><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_101></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-03-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a></div><div class='ch_171'>2023-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a></div><div class='ch_171'>2022-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><div class='ch_171'>2022-12-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a></div><div class='ch_171'>2022-12-16</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a></div><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_117></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-09-27</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a></div><div class='ch_171'>2022-09-21</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a></div><div class='ch_171'>2022-09-08</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a></div><div class='ch_171'>2022-08-12</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div><div class='ch_171'>2022-08-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a></div><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_105></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2021-07-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div><div class='ch_171'>2021-06-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><div class='ch_171'>2021-06-10</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a></div><div class='ch_171'>2021-06-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a></div><div class='ch_171'>2021-06-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a></div><div class='ch_171'>2021-06-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a></div><div class='ch_171'>2021-06-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a></div><div class='ch_171'>2021-06-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a></div><div class='ch_171'>2021-06-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a></div><div class='ch_171'>2020-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><div class='ch_171'>2019-08-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a></div><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_121></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_125></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>videos</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>赚钱宝典</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><h3 class='ch_182'>追英赶美</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><h3 class='ch_182'>小民参政</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/450-我们处于史上最好的时代/README.md' target='_blank'><div class='ch_176'>我们处于史上最好的时代</div><div class='ch_177'>2024-04-14</div></a><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><h3 class='ch_182'>批判那些伪文艺</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>万象思考</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>时空猜想</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><h3 class='ch_182'>论时事</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><h3 class='ch_182'>小说 / 陆小凤新传</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><h3 class='ch_182'>小说 / 一念天堂</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_10></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_15></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_19></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_23></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_27></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_31></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_35></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_39></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_43></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_47></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_51></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_55></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_59></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_63></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_67></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_71></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_75></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_79></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_83></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_87></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_91></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_95></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_99></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_103></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>software</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>tutorials</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_107></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_111></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_115></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_119></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_123></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170' style="align-content:stretch;"><div class='ch_183 ch_184'><div class='ch_185 ch_186'>邮箱</div><div class='ch_187'><a class='ch_188 ch_189 ch_190' href='mailto:lcctoor@outlook.com'>lcctoor@outlook.com</a></div><div class='ch_185 ch_186'>微信</div><div class='ch_187'><img class='ch_191' src='./ip_static/WeChatQRC.jpg' style="max-width:15rem; height:auto;"></div><div class='ch_185 ch_186'>捐赠</div><div class='ch_187'><img class='ch_191' src='./ip_static/DonationQRC-0rmb.jpg' style="max-width:15rem; height:auto;"></div></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div></div>
 <script>
 "use strict";
 
 ch.ch_2 = () => window.innerWidth > window.innerHeight
 ch.ch_3 = (ele, name, value) => {
             try {ele.setAttribute(name, value)} catch (e) {}
             try {ele[name] = value} catch (e) {}
@@ -170,15 +170,15 @@
 ch.ch_143 = document.getElementById("ch_142")
 ch.ch_144 = new Map([["current_index", null]])
 ch.ch_147 = ch.ch_141(ch.ch_143, ch.ch_144, 0.2)
 ch.ch_148 = new Map([])
 ch.ch_149 = [ch.ch_147, ch.ch_148]
 ch.ch_151 = document.getElementById("ch_150")
 ch.ch_154 = (value) => { ch.ch_151.firstChild.textContent = value }
-ch.ch_155 = new Map([["0", "动态"], ["1", "视频"], ["2", "文章"], ["3", "想法"], ["4", "软件"], ["5", "Python教程"], ["6", "生活"], ["7", "自述"]])
+ch.ch_155 = new Map([["1", "动态"], ["2", "视频"], ["3", "文章"], ["4", "想法"], ["5", "软件"], ["6", "Python教程"], ["7", "生活"], ["8", "自述"]])
 ch.ch_156 = [ch.ch_154, ch.ch_155]
 ch.ch_132 = [ch.ch_140, ch.ch_149, ch.ch_156]
 ch.ch_135 = new Map([])
 ch.ch_145 = new Map([])
 ch.ch_152 = new Map([])
 ch.ch_136 = ch.ch_131(ch.ch_132, null)
 ch.ch_137 = (navigation, navs, sync_value) => {
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 动态视频文章想法软件Python教程生活自述
+2024-04-14
+_我_们_处_于_史_上_最_好_的_时_代
+_2_0_2_4_-_0_4_-_1_4
 2024-04-13
 _b_a_s_e_9_5
 _（_字_节_编_码_方_法_）
 _2_0_2_4_-_0_4_-_1_3
 _B_a_s_e_9_5_编_码
 _2_0_2_4_-_0_4_-_1_3
-2024-04-11
-_编_程_心_得
-_2_0_2_4_-_0_4_-_1_1
 2024-03-31
 _W_e_C_h_a_t_ _A_r_t_ _M_u_s_e_u_m
 _（_微_信_艺_术_馆_）
 _2_0_2_4_-_0_3_-_3_1
 2024-03-18
 ===============================================================================
 ===============================================================================
@@ -230,14 +230,16 @@
 _产_业_升_级_与_失_业_潮
 _2_0_2_4_-_0_1_-_0_3
 _在_C_h_a_t_G_P_T_冲_击_下_，_打_造_国_家_级_公_共_知_识_库_迫_在_眉_睫
 _2_0_2_4_-_0_1_-_0_3
 ******** ?小?民?参?政 ********
 _广_义_的_民_主
 _2_0_2_2_-_1_2_-_1_6
+_我_们_处_于_史_上_最_好_的_时_代
+_2_0_2_4_-_0_4_-_1_4
 _年_轻_人_不_结_婚_是_文_明_的_进_步
 _2_0_2_3_-_1_0_-_2_4
 ******** ?批?判?那?些?伪?文?艺 ********
 _一_元_官_司_有_意_义_吗_？
 _2_0_2_3_-_0_7_-_0_9
 _唯_有_变_化_是_不_变_的_？
 _2_0_2_1_-_0_6_-_0_3
@@ -374,16 +376,14 @@
 _2_0_2_4_-_0_4_-_1_3
 _对_接_C_h_a_t_G_P_T
 _2_0_2_3_-_0_3_-_0_7
 _时_间_模_块
 _2_0_2_3_-_0_6_-_2_5
 _面_向_对_象_数_据_库
 _2_0_2_4_-_0_3_-_0_6
-_编_程_心_得
-_2_0_2_4_-_0_4_-_1_1
 _用_3_7_行_代_码_实_现_A_I_五_子_棋
 _2_0_1_9_-_0_8_-_0_5
 _正_则_表_达_式
 _2_0_2_3_-_0_6_-_1_9
 Copyright 2018-2024 lcctoor@outlook.com
 2024-03-18
 ===============================================================================
```

### Comparing `arts-2024.4.13/arts/life/2018/莆田学院·毕业生留影/index.html` & `arts-2024.4.19/arts/life/2018/莆田学院·毕业生留影/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/life/2019/苏州市虎丘山/index.html` & `arts-2024.4.19/arts/life/2019/苏州市虎丘山/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/life/2022/泉州市丰泽区·雨后街道/index.html` & `arts-2024.4.19/arts/life/2022/泉州市丰泽区·雨后街道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/life/2023/更换微信账号了/index.html` & `arts-2024.4.19/arts/life/2023/更换微信账号了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/life/2024/泉州市承天禅寺/index.html` & `arts-2024.4.19/arts/life/2024/泉州市承天禅寺/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/LICENSE` & `arts-2024.4.19/arts/miumapp/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/README.md` & `arts-2024.4.19/arts/miumapp/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/_core.py` & `arts-2024.4.19/arts/miumapp/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/licenses/pyppeteer/LICENSE` & `arts-2024.4.19/arts/miumapp/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/licenses/tornado/LICENSE` & `arts-2024.4.19/arts/miumapp/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/miumapp/demo.html` & `arts-2024.4.19/arts/miumapp/miumapp/demo.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/miumapp/demo.py` & `arts-2024.4.19/arts/miumapp/miumapp/demo.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/miumapp/pyproject.toml` & `arts-2024.4.19/arts/miumapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oodb/LICENSE` & `arts-2024.4.19/arts/oodb/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oodb/README.md` & `arts-2024.4.19/arts/oodb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oodb/_core.py` & `arts-2024.4.19/arts/oodb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oodb/licenses/pymongo/LICENSE` & `arts-2024.4.19/arts/oodb/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oodb/pyproject.toml` & `arts-2024.4.19/arts/oodb/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomongo/LICENSE` & `arts-2024.4.19/arts/oomongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomongo/README.md` & `arts-2024.4.19/arts/oomongo/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomongo/_core.py` & `arts-2024.4.19/arts/oomongo/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomongo/licenses/motor/LICENSE` & `arts-2024.4.19/arts/oomongo/licenses/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomongo/licenses/pymongo/LICENSE` & `arts-2024.4.19/arts/oomongo/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomongo/pyproject.toml` & `arts-2024.4.19/arts/oomongo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomysql/LICENSE` & `arts-2024.4.19/arts/oomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomysql/README.md` & `arts-2024.4.19/arts/oomysql/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomysql/_core.py` & `arts-2024.4.19/arts/oomysql/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomysql/licenses/aiomysql/LICENSE` & `arts-2024.4.19/arts/oomysql/licenses/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomysql/licenses/pymysql/LICENSE` & `arts-2024.4.19/arts/oomysql/licenses/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/oomysql/pyproject.toml` & `arts-2024.4.19/arts/oomysql/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/openai2/LICENSE` & `arts-2024.4.19/arts/openai2/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/openai2/README.md` & `arts-2024.4.19/arts/openai2/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/openai2/_core/chat.py` & `arts-2024.4.19/arts/openai2/_core/chat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/openai2/_core/chat_in_cmd.py` & `arts-2024.4.19/arts/openai2/_core/chat_in_cmd.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/openai2/_core/group_chat.py` & `arts-2024.4.19/arts/openai2/_core/group_chat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/openai2/licenses/openai/LICENSE` & `arts-2024.4.19/arts/openai2/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/openai2/pyproject.toml` & `arts-2024.4.19/arts/openai2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/skybox/README.md` & `arts-2024.4.19/arts/skybox/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/skybox/skybox/files_hashes` & `arts-2024.4.19/arts/skybox/skybox/files_hashes`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,18 @@
     arts -2024.1.17.zip                        -info {"size": 571603, "sha-512": "327342199a59a3678a8e09e3706a7885b0ad83ebd3c3183f74b7c95ce6e5e6350dad1a26ce32cdc08c3b2fee2e7f467000c571a4e366002063a683076bbf1a39", "sha3-512": "e21b1ba2bf287a6c356b96b8c9c08c439d99dab8d877669d087991479b3906eb5f25540c674655b7e4d99ca07e9d4eac62183d0c34815dd9c5c9862be62135cf"}
     arts -2024.1.30.zip                        -info {"size": 582125, "sha-512": "f33c6f44f62871b7f3660c91d19b80b9a03fa1f93d537b461a37e479e5b4fd823a57c97d52d0c6160d92d1bf8ae0a6e61101c5d759792303c094d5c8e5ec68fb", "sha3-512": "af8bf7c9d2b342de2296756c2048e5f4b14ee09fee032559a18f05ce471a85ad56c01d72b40f13369c848a0fff136be0d700b09ffc9df4fbe104a795abac1a99"}
     arts -2024.2.13.zip                        -info {"size": 633463, "sha-512": "335fc45861fd8785c077baa2b2035702340a1e0cd815ae11db258f61979948edf55139757d2991d3800a2398e89ac225dbff8150418aae0c9df980d92c895110", "sha3-512": "d4381233c7c640d474fea34eeebfa9e7cc0d2ba07b3bfe9ea9bad81a34d83828f511b395bf7b6b7d4d474798cb4950181d569200d95091ffd08b099e181e270a"}
     arts -2024.2.25.zip                        -info {"size": 662003, "sha-512": "430648c7c3e2623f4addad65ed6897d8d70b994c65612217cccb5f106596910e9eeadf5417d5036532921a4b8161cda8d93f73d6acf5572b1089cf7084a290e2", "sha3-512": "d0f228a0e9a5c8f6fcfca392fded9abfda2ab1b82939cb50a45b4977b00bd427c81913289924d704bdda8c21bc61eb3ef22cb6b09d311b768a2d52a62eafccdc"}
     arts -2024.3.25.zip                        -info {"size": 731537, "sha-512": "ab80e3c2c0e583552c45134a01991c40f7b02379249299ce19cd01fa411b7e034cb6cc9d8078b93a183577261f20ef6fcca8a0ba05e781d492c7e8d5d2192604", "sha3-512": "0e532cac08a44498c3f001ebdd262fd21e471165a6503264bca0b26b81d63b9de869cda5d94d741b6187e12f93b5167c5bda34ea274398a9da66168538f5a565"}
     arts -2024.3.31.zip                        -info {"size": 784894, "sha-512": "d14e1defcd1845602c68dfa1e2b01f08b970eaa0c2c08426eab9f7c2acc265ed2eaee024c7f9cb935e05477fc1e078e43cd2f09b2806d57a77880542e179a570", "sha3-512": "ee6ee0dd3247be1bbacde5819d8fb8e2a35422ce7e4c4ce20fef13ac80598ed654d65182d550e0f29d4a694dfba38eef825747a6565265af954a217d9c20ab86"}
     arts -2024.3.6.zip                         -info {"size": 729443, "sha-512": "f7d02e0c59ca5da9460ef8af9ed08d2c3c2bc903a3cec85411588badc42f81b64c0df2841b5fb790d24fb3eeb6728e2e7cb363d8bfa859afd7b23b8b997cd83b", "sha3-512": "8fa2af71bcb48993cb6be156c6e07a4ad052fb83cd1d35c89fcb237d135a0a05c2f3aeea7490b5874d3f0b8f61d0e72560163cc2d0c8ff6d58cd86bc902942f8"}
-    arts -2024.4.3.zip                         -info {"size": 792338, "sha-512": "7e8eab613cf52949bfa96c275571fb897bafd67cbdb4c1c94167cb6891336f8f1590853bb8fada5be5c0f227feeda2eb6dd6c2f25b9c773d0de1323d63ec9110", "sha3-512": "b3520b0c6dde6365f97b38232657c005250206cfcb5001085bae1f2610b1cb6d5c79403c4b58b1061c9d957e0e37154620869458119d15fd0cd70e13aa5227e7"}
+    arts -2024.4.13.zip                        -info {"size": 813929, "sha-512": "ef483a296af3c56b6d3b80f2baff07514e8cae1d386a27e98cf5d7ef21a4f57d790138670ec9bab24f3d89bb2cbaabe54f2d4ad2ccfc0599678ce372507c79ec", "sha3-512": "09d9958de1a143acc5b2b5e95dde5d64192dd3e110dc49152ff72a02d275bf380dd0bb44a678185e81ef78b2bb9bcfe556e57df5ebc9c9dd94580c5090414c27"}
     wss -20231220.zip                          -info {"size": 8614060, "sha-512": "473d3652c54b15af6fde766cea58974e63b66ba086d44d09b4de6b50d275d07bac4d4c4d6b632dde6e85e971d35566f958efd1b6741d6b96ae67ee6f2ee362b2", "sha3-512": "5f4c6eb204872dc7893c607afabb016ceec67561ddbe76bfb65610d91a3d7dfcce7a0a27da7c81d4f9bee442a97609bfa3d62bee15c2fd435c19ad3152693785"}
     wss -20240325.zip                          -info {"size": 8200568, "sha-512": "2539dd1162403630a705148c90d79b393e9f4a3b9eb81231bfa9fcfe31d1fe185e68c3226bf0d3ae76377c8e3465452e32497e5f470bfe07b60b6fabdd0d509c", "sha3-512": "d510ad8925838c974f2807c79b500a9a7eceddf7dc9f62169615cebfe24f4af484eddecd1ca7c7413e99b8f0a0870b2fe7b6184f475b77736bb754ccd2977f34"}
     wss -20240331.zip                          -info {"size": 8370828, "sha-512": "d644b57284a09ef8fcaeb516dad6d97a997d40cfc0dbcfa3f1f55593b8f76000d93c3708c43d5fc50e5d6255f0d8ca9e52016e618a595d32657bdd466849d772", "sha3-512": "05d33f34bdfcce247dc5ddf27ad9845f01c656711938ffef1f3d006c78c26d08b9d6a6c0f961d85a07393d26cc5c346bc7f27cb94e786d90434fbc70fc3b4284"}
-    wss -20240403.zip                          -info {"size": 8472849, "sha-512": "2a21df6fa9808250f384363a0eded43ba177364c8ec67c1b535f4ad9870e9a65fd4b60624b70f20aaa94f3d24e057d463d63268e7a0412ae7819acb4d93db084", "sha3-512": "1455a2ba7e55b3784e57e036fddcd6b080661ffeb35fc6c7447d4fd6573c6130914726a11f84dc0bb584b02d7ab5be51ee8dfbfe91a26c73bf9efce2d9e994a8"}
     wss -20240413.zip                          -info {"size": 8960665, "sha-512": "b9f57d8e1cce63d12398b7bf805c272f77fd16ea2a519ee8ec2f636d2c50d9a41d73f5ce581bedf01aa2651e6b2de14b842c290c6e5befc007f2661588b2fe23", "sha3-512": "4c1bf6de3863cf8f1ea68a343449687b3a820c6cafbee2ea616da39754c4728e9278da362b7344a55b23aca898cd820aab64dcb284d3d2772213ff1130ef49ed"}
 富文本笔记本.png                               -info {"size": 644251, "sha-512": "e8293b799d49e53501fb50e85f7025d3d1f7c83e05f8982af51cc75c309d5014a17fb2326b8476335575b6bf4f8c2d4ffe2f4de9c3c423ef92adc3766996832f", "sha3-512": "82aecb03ab4abb583a6791b32301d76dafc451a70ee2f22b0c2c71428a0f100471beae02195681b61d1f6d7d1efdeaac719ffafbce9410b2c5065fe05841b009"}
 按键行为和鼠标行为采集装置                 
     2023-09-12.zip                             -info {"size": 939254, "sha-512": "939a9ee1132c5a5ef837f3f77b2bb005caafcd4f7cbc8ea1d219f2b1a1f512c7b71faf2c7a96ab961f7f62918992f1122e497c08c435f9579ff6c5d13f00b90f", "sha3-512": "efedfc0ece0c44d2ea1fb705dac8ab5283e74faf6e3e973a91ce447ffae1cc85359f96b1b33092fe61032a1424c62ed6e37a9fb9107f9029008474f3977a4446"}
 捷鸟.jpg                                       -info {"size": 793233, "sha-512": "96da3cf6df87d85d59bbdf80ccbbf0c841fcdd52d37ca2556219020c94978c01cf648df52d51dc2733f5bc773b734d9ba5b17e9cc8056278857a9059f5c756e3", "sha3-512": "99dfdb17c8663587c7db7b18621c11743e89cb67f6ab8be395c5901adae0a3fe7838175fcba7194927deb1c3ae509c1577eb2ad4b4d3c04890c94b77b00cc311"}
 桌面APP导航栏.png                              -info {"size": 256699, "sha-512": "b5cc935b98f28f0354b401e5f6d8e9768376ba6be7be1996247155459792a2a27131fee396bf0c8384c9e504115eb84d86f713e5d229f132889fd2b03b44f1e8", "sha3-512": "64c1edea61003c4147974a0f81eb748d98de1678d5a3ec13149297219526de25656942b8eb6c21b0546a3ea2dc9af367def29f6a60e81aab01796e146fdb5f4a"}
 短视频
```

### Comparing `arts-2024.4.13/arts/thoughts/2022/现代工人的螺丝钉处境/index.html` & `arts-2024.4.19/arts/thoughts/2022/现代工人的螺丝钉处境/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html` & `arts-2024.4.19/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/专利是个公平的赛道/index.html` & `arts-2024.4.19/arts/thoughts/2023/专利是个公平的赛道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/事情的真实性是由度的/index.html` & `arts-2024.4.19/arts/thoughts/2023/事情的真实性是由度的/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/人无法摆脱兽性/index.html` & `arts-2024.4.19/arts/thoughts/2023/人无法摆脱兽性/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/什么是极端？/index.html` & `arts-2024.4.19/arts/thoughts/2023/什么是极端？/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/保护好人/index.html` & `arts-2024.4.19/arts/thoughts/2023/保护好人/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/只筛选，不教化/index.html` & `arts-2024.4.19/arts/thoughts/2023/只筛选，不教化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/喊高考加油是刷存在感/index.html` & `arts-2024.4.19/arts/thoughts/2023/喊高考加油是刷存在感/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html` & `arts-2024.4.19/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html` & `arts-2024.4.19/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html` & `arts-2024.4.19/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/想去国外了解自己/index.html` & `arts-2024.4.19/arts/thoughts/2023/想去国外了解自己/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/现代化的分工合作机制/index.html` & `arts-2024.4.19/arts/thoughts/2023/现代化的分工合作机制/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/用理性处理简单的事情/index.html` & `arts-2024.4.19/arts/thoughts/2023/用理性处理简单的事情/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/真正的问题无法通过花招解决/index.html` & `arts-2024.4.19/arts/thoughts/2023/真正的问题无法通过花招解决/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html` & `arts-2024.4.19/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html` & `arts-2024.4.19/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2024/不要害怕犯错/index.html` & `arts-2024.4.19/arts/thoughts/2024/不要害怕犯错/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2024/新年题诗/index.html` & `arts-2024.4.19/arts/thoughts/2024/新年题诗/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html` & `arts-2024.4.19/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2024/编程语言的进化/example.html` & `arts-2024.4.19/arts/thoughts/2024/编程语言的进化/example.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2024/编程语言的进化/index.html` & `arts-2024.4.19/arts/thoughts/2024/编程语言的进化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html` & `arts-2024.4.19/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html` & `arts-2024.4.19/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/tutorials/600-用37行代码实现AI五子棋/README.md` & `arts-2024.4.19/arts/tutorials/600-用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/arts/tutorials/750-正则表达式/README.md` & `arts-2024.4.19/arts/tutorials/750-正则表达式/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.13/pyproject.toml` & `arts-2024.4.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "arts"
-version = "2024.4.13"
+version = "2024.4.19"
 description = "对 Python 开发中常用功能的封装"
 dependencies = ["openai>=1.2.4", "numpy", "pymysql", "aiomysql", "pymongo", "motor", "pyppeteer>=2.0.0", "tornado"]
 
 
 requires-python = ">=3.10"
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
```

### Comparing `arts-2024.4.13/PKG-INFO` & `arts-2024.4.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arts
-Version: 2024.4.13
+Version: 2024.4.19
 Summary: 对 Python 开发中常用功能的封装
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.2.4
 Requires-Dist: numpy
 Requires-Dist: pymysql
```

