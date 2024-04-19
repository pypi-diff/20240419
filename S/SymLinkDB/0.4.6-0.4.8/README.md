# Comparing `tmp/SymLinkDB-0.4.6.tar.gz` & `tmp/SymLinkDB-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SymLinkDB-0.4.6.tar", last modified: Fri Apr 19 02:37:14 2024, max compression
+gzip compressed data, was "SymLinkDB-0.4.8.tar", last modified: Fri Apr 19 09:23:08 2024, max compression
```

## Comparing `SymLinkDB-0.4.6.tar` & `SymLinkDB-0.4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/
--rw-rw-rw-   0        0        0    36975 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.037514 SymLinkDB-0.4.6/SymLinkDB/
--rw-rw-rw-   0        0        0    47330 2024-04-19 02:36:24.000000 SymLinkDB-0.4.6/SymLinkDB/__init__.py
--rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.6/SymLinkDB/document_code.py
-drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.021528 SymLinkDB-0.4.6/SymLinkDB/parts/
-drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/
--rw-rw-rw-   0        0        0     3211 2024-03-26 07:32:05.000000 SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/__init__.py
--rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/test.py
-drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/
--rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/__init__.py
--rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/test.py
--rw-rw-rw-   0        0        0    11537 2024-04-19 02:36:35.000000 SymLinkDB-0.4.6/SymLinkDB/test.py
-drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.045539 SymLinkDB-0.4.6/SymLinkDB.egg-info/
--rw-rw-rw-   0        0        0    36975 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-19 02:36:53.000000 SymLinkDB-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.778354 SymLinkDB-0.4.8/
+-rw-rw-rw-   0        0        0    36975 2024-04-19 09:23:08.777322 SymLinkDB-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.754661 SymLinkDB-0.4.8/SymLinkDB/
+-rw-rw-rw-   0        0        0    47762 2024-04-19 09:18:37.000000 SymLinkDB-0.4.8/SymLinkDB/__init__.py
+-rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.8/SymLinkDB/document_code.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.740136 SymLinkDB-0.4.8/SymLinkDB/parts/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.772308 SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/
+-rw-rw-rw-   0        0        0     3680 2024-04-19 09:20:12.000000 SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/__init__.py
+-rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.775318 SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/
+-rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/__init__.py
+-rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/test.py
+-rw-rw-rw-   0        0        0    11537 2024-04-19 02:36:35.000000 SymLinkDB-0.4.8/SymLinkDB/test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.769708 SymLinkDB-0.4.8/SymLinkDB.egg-info/
+-rw-rw-rw-   0        0        0    36975 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       69 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:23:08.778354 SymLinkDB-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-19 09:22:48.000000 SymLinkDB-0.4.8/setup.py
```

### Comparing `SymLinkDB-0.4.6/PKG-INFO` & `SymLinkDB-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.6
+Version: 0.4.8
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.6/README.md` & `SymLinkDB-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.6/SymLinkDB/__init__.py` & `SymLinkDB-0.4.8/SymLinkDB/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,28 @@
 def memory_backend(backend_dir):
 	# 単純メモリbackend (SLDB-backend) [memory_backend]
 	from .parts import memory_backend as m_back_module
 	# メモリバックエンドへの接続 [memory_backend]
 	return m_back_module.conn(backend_dir)
 
 # CachedFileDicバックエンドの初期化 [SymLinkDB]
-def cfd_backend(backend_dir):
+def cfd_backend(backend_dir,
+	fmt = "fpkl",	# バックエンドのファイル形式 (fpkl: fast-pickle(default), pickle: pickle)
+	cont_size_th = 100 * 1024 ** 2,	# コンテナサイズ目安
+	cache_n = 3	# 最大loadコンテナ数
+):
 	# CachedFileDic-backend (SLDB-backend) [cfd_backend]
 	from .parts import cfd_backend as cfd_back_module
 	# CachedFileDicバックエンドへの接続 [cfd_backend]
-	return cfd_back_module.conn(backend_dir)
+	return cfd_back_module.conn(
+		backend_dir,
+		fmt = fmt,	# バックエンドのファイル形式 (fpkl: fast-pickle(default), pickle: pickle)
+		cont_size_th = cont_size_th,	# コンテナサイズ目安
+		cache_n = cache_n	# 最大loadコンテナ数
+	)
 
 # SLDB-backendとして初期化
 def init_sldb_backend(backend):
 	# このバックエンドを一意に特定するID
 	backend[("meta", "backend_id")] = gen_unique_id()	# 十分な長さの64進idの発行 (uuidの桁数を参考に決定)
 	# このバックエンドに格納されているデータの一覧
 	backend[("meta", "backend_contain_data")] = []
```

### Comparing `SymLinkDB-0.4.6/SymLinkDB/document_code.py` & `SymLinkDB-0.4.8/SymLinkDB/document_code.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/__init__.py` & `SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,162 +40,191 @@
 00000270: 4442 2d62 6163 6b65 6e64 2920 5b63 6664  DB-backend) [cfd
 00000280: 5f62 6163 6b65 6e64 5d0d 0a63 6c61 7373  _backend]..class
 00000290: 2043 4644 5f42 6163 6b65 6e64 3a0d 0a09   CFD_Backend:...
 000002a0: 2320 e588 9de6 9c9f e58c 96e5 87a6 e790  # ..............
 000002b0: 860d 0a09 6465 6620 5f5f 696e 6974 5f5f  ....def __init__
 000002c0: 2873 656c 662c 2064 6174 615f 6469 722c  (self, data_dir,
 000002d0: 0d0a 0909 666d 7420 3d20 2266 706b 6c22  ....fmt = "fpkl"
-000002e0: 0923 20e3 8390 e383 83e3 82af e382 a8e3  .# .............
-000002f0: 83b3 e383 89e3 81ae e383 95e3 82a1 e382  ................
-00000300: a4e3 83ab e5bd a2e5 bc8f 2028 6670 6b6c  .......... (fpkl
-00000310: 3a20 6661 7374 2d70 6963 6b6c 6528 6465  : fast-pickle(de
-00000320: 6661 756c 7429 2c20 7069 636b 6c65 3a20  fault), pickle: 
-00000330: 7069 636b 6c65 290d 0a09 293a 0d0a 0909  pickle)...):....
-00000340: 2320 e382 a4e3 83b3 e383 87e3 8383 e382  # ..............
-00000350: afe3 82b9 e381 a8e3 8387 e383 bce3 82bf  ................
-00000360: e382 92e6 a0bc e7b4 8de3 8199 e382 8b32  ...............2
-00000370: e381 a4e3 81ae e383 87e3 82a3 e383 ace3  ................
-00000380: 82af e383 88e3 83aa 0d0a 0909 6d65 6d5f  ............mem_
-00000390: 6964 785f 6469 7220 3d20 6f73 2e70 6174  idx_dir = os.pat
-000003a0: 682e 6a6f 696e 2864 6174 615f 6469 722c  h.join(data_dir,
-000003b0: 2022 6d65 6d5f 6964 7822 290d 0a09 0963   "mem_idx")....c
-000003c0: 6664 5f64 6174 615f 6469 7220 3d20 6f73  fd_data_dir = os
-000003d0: 2e70 6174 682e 6a6f 696e 2864 6174 615f  .path.join(data_
-000003e0: 6469 722c 2022 6366 645f 6461 7461 2229  dir, "cfd_data")
-000003f0: 0d0a 0909 6966 206e 6f74 206f 732e 7061  ....if not os.pa
-00000400: 7468 2e65 7869 7374 7328 6d65 6d5f 6964  th.exists(mem_id
-00000410: 785f 6469 7229 3a20 6f73 2e6d 616b 6564  x_dir): os.maked
-00000420: 6972 7328 6d65 6d5f 6964 785f 6469 7229  irs(mem_idx_dir)
-00000430: 0d0a 0909 6966 206e 6f74 206f 732e 7061  ....if not os.pa
-00000440: 7468 2e65 7869 7374 7328 6366 645f 6461  th.exists(cfd_da
-00000450: 7461 5f64 6972 293a 206f 732e 6d61 6b65  ta_dir): os.make
-00000460: 6469 7273 2863 6664 5f64 6174 615f 6469  dirs(cfd_data_di
-00000470: 7229 0d0a 0909 2320 e382 a4e3 83b3 e383  r)....# ........
-00000480: 87e3 8383 e382 afe3 82b9 e382 92e6 a0bc  ................
-00000490: e7b4 8de3 8199 e382 8b6d 656d 6f72 795f  .........memory_
-000004a0: 6261 636b 656e 64e3 81ae e588 9de6 9c9f  backend.........
-000004b0: e58c 960d 0a09 0973 656c 662e 6d65 6d5f  .......self.mem_
-000004c0: 6964 7820 3d20 6d65 6d6f 7279 5f62 6163  idx = memory_bac
-000004d0: 6b65 6e64 2e63 6f6e 6e28 6d65 6d5f 6964  kend.conn(mem_id
-000004e0: 785f 6469 722c 2066 6d74 203d 2066 6d74  x_dir, fmt = fmt
-000004f0: 2909 2320 e383 a1e3 83a2 e383 aae3 8390  ).# ............
-00000500: e383 83e3 82af e382 a8e3 83b3 e383 89e3  ................
-00000510: 81b8 e381 aee6 8ea5 e7b6 9a20 5b6d 656d  ........... [mem
-00000520: 6f72 795f 6261 636b 656e 645d 0d0a 0909  ory_backend]....
-00000530: 2320 e383 87e3 83bc e382 bfe3 8292 e6a0  # ..............
-00000540: bce7 b48d e381 99e3 828b 4361 6368 6564  ..........Cached
-00000550: 4669 6c65 4469 63e3 81ae e588 9de6 9c9f  FileDic.........
-00000560: e58c 960d 0a09 0973 656c 662e 6366 645f  .......self.cfd_
-00000570: 6461 7461 203d 2043 6163 6865 6446 696c  data = CachedFil
-00000580: 6544 6963 2e63 6f6e 6e28 6366 645f 6461  eDic.conn(cfd_da
-00000590: 7461 5f64 6972 2c20 666d 7420 3d20 666d  ta_dir, fmt = fm
-000005a0: 7429 0923 20e5 afbe e8b1 a1e3 8387 e382  t).# ...........
-000005b0: a3e3 83ac e382 afe3 8388 e383 aae3 81ab  ................
-000005c0: e68e a5e7 b69a 205b 4361 6368 6564 4669  ...... [CachedFi
-000005d0: 6c65 4469 635d 0d0a 0909 2320 e383 97e3  leDic]....# ....
-000005e0: 83ad e382 b0e3 83a9 e383 a0e7 b582 e4ba  ................
-000005f0: 86e6 9982 e381 ae63 6f6d 6d69 74e5 afbe  .......commit...
-00000600: e8b1 a1e3 81ab e887 aae8 baab e382 92e8  ................
-00000610: bfbd e58a a00d 0a09 0963 6f6d 6d69 745f  .........commit_
-00000620: 7461 7267 6574 5f6c 732e 6170 7065 6e64  target_ls.append
-00000630: 2873 656c 6629 0d0a 0923 2063 7265 6174  (self)...# creat
-00000640: 652c 2075 7064 6174 65e5 85b1 e980 9a20  e, update...... 
-00000650: 5b6d 656d 6f72 795f 6261 636b 656e 645d  [memory_backend]
-00000660: 0d0a 0964 6566 205f 5f73 6574 6974 656d  ...def __setitem
-00000670: 5f5f 2873 656c 662c 206b 6579 2c20 7661  __(self, key, va
-00000680: 6c75 6529 3a0d 0a09 0923 20e6 96b0 e381  lue):....# .....
-00000690: 97e3 8184 696e 6e65 725f 6b65 79e3 81ae  ....inner_key...
-000006a0: e794 9fe6 8890 0d0a 0909 696e 6e65 725f  ..........inner_
-000006b0: 6b65 7920 3d20 736c 696d 5f69 642e 6765  key = slim_id.ge
-000006c0: 6e28 6c61 6d62 6461 2065 3a20 2865 2069  n(lambda e: (e i
-000006d0: 6e20 7365 6c66 2e63 6664 5f64 6174 6129  n self.cfd_data)
-000006e0: 2c20 6c65 6e67 7468 203d 2032 3229 0923  , length = 22).#
-000006f0: 20e5 8d81 e588 86e3 81ab e995 b7e3 8184   ...............
-00000700: 6b65 790d 0a09 0923 20e4 b8a1 e696 b9e3  key....# .......
-00000710: 81ae e8be 9ee6 9bb8 e381 abe7 99bb e98c  ................
-00000720: b20d 0a09 0973 656c 662e 6d65 6d5f 6964  .....self.mem_id
-00000730: 785b 6b65 795d 203d 2069 6e6e 6572 5f6b  x[key] = inner_k
-00000740: 6579 0d0a 0909 7365 6c66 2e63 6664 5f64  ey....self.cfd_d
-00000750: 6174 615b 696e 6e65 725f 6b65 795d 203d  ata[inner_key] =
-00000760: 2076 616c 7565 0d0a 0923 206b 6579 e8aa   value...# key..
-00000770: ade3 81bf e587 bae3 8197 205b 6d65 6d6f  .......... [memo
-00000780: 7279 5f62 6163 6b65 6e64 5d0d 0a09 6465  ry_backend]...de
-00000790: 6620 5f5f 6765 7469 7465 6d5f 5f28 7365  f __getitem__(se
-000007a0: 6c66 2c20 6b65 7929 3a0d 0a09 0969 6e6e  lf, key):....inn
-000007b0: 6572 5f6b 6579 203d 2073 656c 662e 6d65  er_key = self.me
-000007c0: 6d5f 6964 785b 6b65 795d 0d0a 0909 7265  m_idx[key]....re
-000007d0: 7475 726e 2073 656c 662e 6366 645f 6461  turn self.cfd_da
-000007e0: 7461 5b69 6e6e 6572 5f6b 6579 5d0d 0a09  ta[inner_key]...
-000007f0: 2320 e589 8ae9 99a4 205b 6d65 6d6f 7279  # ...... [memory
-00000800: 5f62 6163 6b65 6e64 5d0d 0a09 6465 6620  _backend]...def 
-00000810: 5f5f 6465 6c69 7465 6d5f 5f28 7365 6c66  __delitem__(self
-00000820: 2c20 6b65 7929 3a20 6465 6c20 7365 6c66  , key): del self
-00000830: 2e6d 656d 5f69 6478 5b6b 6579 5d09 2320  .mem_idx[key].# 
-00000840: e383 a1e3 83a2 e383 aae3 83bc e383 90e3  ................
-00000850: 8383 e382 afe3 82a8 e383 b3e3 8389 e381  ................
-00000860: aee3 81bf e381 8be3 8289 e589 8ae9 99a4  ................
-00000870: 0d0a 0923 20e5 ad98 e59c a8e7 a2ba e8aa  ...# ...........
-00000880: 8d20 5b6d 656d 6f72 795f 6261 636b 656e  . [memory_backen
-00000890: 645d 0d0a 0964 6566 205f 5f63 6f6e 7461  d]...def __conta
-000008a0: 696e 735f 5f28 7365 6c66 2c20 6b65 7929  ins__(self, key)
-000008b0: 3a20 7265 7475 726e 2028 6b65 7920 696e  : return (key in
-000008c0: 2073 656c 662e 6d65 6d5f 6964 7829 0d0a   self.mem_idx)..
-000008d0: 0923 2069 7465 7220 2866 6f72 e696 87e8  .# iter (for....
-000008e0: 8488 e7ad 89e3 81a7 e381 aee5 88a9 e794  ................
-000008f0: a829 205b 6d65 6d6f 7279 5f62 6163 6b65  .) [memory_backe
-00000900: 6e64 5d0d 0a09 6465 6620 5f5f 6974 6572  nd]...def __iter
-00000910: 5f5f 2873 656c 6629 3a20 7265 7475 726e  __(self): return
-00000920: 2069 7465 7228 7365 6c66 2e6d 656d 5f69   iter(self.mem_i
-00000930: 6478 290d 0a09 2320 e5bc b7e5 88b6 636f  dx)...# ......co
-00000940: 6d6d 6974 205b 6d65 6d6f 7279 5f62 6163  mmit [memory_bac
-00000950: 6b65 6e64 5d0d 0a09 6465 6620 636f 6d6d  kend]...def comm
-00000960: 6974 2873 656c 6629 3a0d 0a09 0973 656c  it(self):....sel
-00000970: 662e 6d65 6d5f 6964 782e 636f 6d6d 6974  f.mem_idx.commit
-00000980: 2829 0d0a 0909 7365 6c66 2e63 6664 5f64  ()....self.cfd_d
-00000990: 6174 612e 636f 6d6d 6974 2829 0d0a 0923  ata.commit()...#
-000009a0: 20e6 9687 e5ad 97e5 8897 e58c 9620 28e3   ............ (.
-000009b0: 819d e381 ae31 2c20 e381 9de3 81ae 3229  .....1, ......2)
-000009c0: 0d0a 0964 6566 205f 5f73 7472 5f5f 2873  ...def __str__(s
-000009d0: 656c 6629 3a0d 0a09 0923 206d 656d 6f72  elf):....# memor
-000009e0: 792d 6261 636b 656e 64e3 81ae e99d 9ee5  y-backend.......
-000009f0: 85ac e5bc 8f41 5049 e382 92e5 88a9 e794  .....API........
-00000a00: a80d 0a09 0966 6f72 206b 6579 5f65 7861  .....for key_exa
-00000a10: 6d70 6c65 2069 6e20 7365 6c66 2e6d 656d  mple in self.mem
-00000a20: 5f69 6478 3a20 6272 6561 6b09 2320 6b65  _idx: break.# ke
-00000a30: 79e3 81ae e4be 8be3 8292 e58f 96e5 be97  y...............
-00000a40: 0d0a 0909 7369 7a65 203d 206c 656e 2873  ....size = len(s
-00000a50: 656c 662e 6d65 6d5f 6964 7829 0d0a 0909  elf.mem_idx)....
-00000a60: 6461 7461 5f73 7472 203d 2028 2222 2069  data_str = ("" i
-00000a70: 6620 7369 7a65 203d 3d20 300d 0a09 0909  f size == 0.....
-00000a80: 656c 7365 2066 277b 6b65 795f 6578 616d  else f'{key_exam
-00000a90: 706c 657d 3a20 7b73 6f75 7473 2873 656c  ple}: {souts(sel
-00000aa0: 665b 6b65 795f 6578 616d 706c 655d 297d  f[key_example])}
-00000ab0: 2720 2b0d 0a09 0909 0928 2222 2069 6620  ' +......("" if 
-00000ac0: 7369 7a65 203d 3d20 3120 656c 7365 2066  size == 1 else f
-00000ad0: 222c 202e 2e2e 286e 3d7b 7369 7a65 7d29  ", ...(n={size})
-00000ae0: 2229 0d0a 0909 290d 0a09 0972 6574 7572  ")....)....retur
-00000af0: 6e20 6622 3c53 4c44 422d 4346 445f 6261  n f"<SLDB-CFD_ba
-00000b00: 636b 656e 6420 7b7b 7b64 6174 615f 7374  ckend {{{data_st
-00000b10: 727d 7d7d 3e22 0d0a 0964 6566 205f 5f72  r}}}>"...def __r
-00000b20: 6570 725f 5f28 7365 6c66 293a 2072 6574  epr__(self): ret
-00000b30: 7572 6e20 7374 7228 7365 6c66 290d 0a0d  urn str(self)...
-00000b40: 0a23 2043 6163 6865 6446 696c 6544 6963  .# CachedFileDic
-00000b50: e383 90e3 8383 e382 afe3 82a8 e383 b3e3  ................
-00000b60: 8389 e381 b8e3 81ae e68e a5e7 b69a 205b  .............. [
-00000b70: 6366 645f 6261 636b 656e 645d 0d0a 6465  cfd_backend]..de
-00000b80: 6620 636f 6e6e 280d 0a09 6461 7461 5f64  f conn(...data_d
-00000b90: 6972 2c09 2320 e383 90e3 8383 e382 afe3  ir,.# ..........
-00000ba0: 82a8 e383 b3e3 8389 e381 aee6 8385 e5a0  ................
-00000bb0: b1e3 8292 e8a8 98e9 8cb2 e381 99e3 828b  ................
-00000bc0: e383 87e3 82a3 e383 ace3 82af e383 88e3  ................
-00000bd0: 83aa 0d0a 0966 6d74 203d 2022 6670 6b6c  .....fmt = "fpkl
-00000be0: 2209 2320 e383 90e3 8383 e382 afe3 82a8  ".# ............
-00000bf0: e383 b3e3 8389 e381 aee3 8395 e382 a1e3  ................
-00000c00: 82a4 e383 abe5 bda2 e5bc 8f20 2866 706b  ........... (fpk
-00000c10: 6c3a 2066 6173 742d 7069 636b 6c65 2864  l: fast-pickle(d
-00000c20: 6566 6175 6c74 292c 2070 6963 6b6c 653a  efault), pickle:
-00000c30: 2070 6963 6b6c 6529 0d0a 293a 0d0a 0923   pickle)..):...#
-00000c40: 20e3 8390 e383 83e3 82af e382 a8e3 83b3   ...............
-00000c50: e383 89e3 81ae e382 afe3 83a9 e382 b90d  ................
-00000c60: 0a09 7265 7475 726e 2043 4644 5f42 6163  ..return CFD_Bac
-00000c70: 6b65 6e64 2864 6174 615f 6469 722c 2066  kend(data_dir, f
-00000c80: 6d74 203d 2066 6d74 290d 0a              mt = fmt)..
+000002e0: 2c09 2320 e383 90e3 8383 e382 afe3 82a8  ,.# ............
+000002f0: e383 b3e3 8389 e381 aee3 8395 e382 a1e3  ................
+00000300: 82a4 e383 abe5 bda2 e5bc 8f20 2866 706b  ........... (fpk
+00000310: 6c3a 2066 6173 742d 7069 636b 6c65 2864  l: fast-pickle(d
+00000320: 6566 6175 6c74 292c 2070 6963 6b6c 653a  efault), pickle:
+00000330: 2070 6963 6b6c 6529 0d0a 0909 636f 6e74   pickle)....cont
+00000340: 5f73 697a 655f 7468 203d 2031 3030 202a  _size_th = 100 *
+00000350: 2031 3032 3420 2a2a 2032 2c09 2320 e382   1024 ** 2,.# ..
+00000360: b3e3 83b3 e383 86e3 838a e382 b5e3 82a4  ................
+00000370: e382 bae7 9bae e5ae 890d 0a09 0963 6163  .............cac
+00000380: 6865 5f6e 203d 2033 0923 20e6 9c80 e5a4  he_n = 3.# .....
+00000390: a76c 6f61 64e3 82b3 e383 b3e3 8386 e383  .load...........
+000003a0: 8ae6 95b0 0d0a 0929 3a0d 0a09 0923 20e3  .......):....# .
+000003b0: 82a4 e383 b3e3 8387 e383 83e3 82af e382  ................
+000003c0: b9e3 81a8 e383 87e3 83bc e382 bfe3 8292  ................
+000003d0: e6a0 bce7 b48d e381 99e3 828b 32e3 81a4  ............2...
+000003e0: e381 aee3 8387 e382 a3e3 83ac e382 afe3  ................
+000003f0: 8388 e383 aa0d 0a09 096d 656d 5f69 6478  .........mem_idx
+00000400: 5f64 6972 203d 206f 732e 7061 7468 2e6a  _dir = os.path.j
+00000410: 6f69 6e28 6461 7461 5f64 6972 2c20 226d  oin(data_dir, "m
+00000420: 656d 5f69 6478 2229 0d0a 0909 6366 645f  em_idx")....cfd_
+00000430: 6461 7461 5f64 6972 203d 206f 732e 7061  data_dir = os.pa
+00000440: 7468 2e6a 6f69 6e28 6461 7461 5f64 6972  th.join(data_dir
+00000450: 2c20 2263 6664 5f64 6174 6122 290d 0a09  , "cfd_data")...
+00000460: 0969 6620 6e6f 7420 6f73 2e70 6174 682e  .if not os.path.
+00000470: 6578 6973 7473 286d 656d 5f69 6478 5f64  exists(mem_idx_d
+00000480: 6972 293a 206f 732e 6d61 6b65 6469 7273  ir): os.makedirs
+00000490: 286d 656d 5f69 6478 5f64 6972 290d 0a09  (mem_idx_dir)...
+000004a0: 0969 6620 6e6f 7420 6f73 2e70 6174 682e  .if not os.path.
+000004b0: 6578 6973 7473 2863 6664 5f64 6174 615f  exists(cfd_data_
+000004c0: 6469 7229 3a20 6f73 2e6d 616b 6564 6972  dir): os.makedir
+000004d0: 7328 6366 645f 6461 7461 5f64 6972 290d  s(cfd_data_dir).
+000004e0: 0a09 0923 20e3 82a4 e383 b3e3 8387 e383  ...# ...........
+000004f0: 83e3 82af e382 b9e3 8292 e6a0 bce7 b48d  ................
+00000500: e381 99e3 828b 6d65 6d6f 7279 5f62 6163  ......memory_bac
+00000510: 6b65 6e64 e381 aee5 889d e69c 9fe5 8c96  kend............
+00000520: 0d0a 0909 7365 6c66 2e6d 656d 5f69 6478  ....self.mem_idx
+00000530: 203d 206d 656d 6f72 795f 6261 636b 656e   = memory_backen
+00000540: 642e 636f 6e6e 286d 656d 5f69 6478 5f64  d.conn(mem_idx_d
+00000550: 6972 2c20 666d 7420 3d20 666d 7429 0923  ir, fmt = fmt).#
+00000560: 20e3 83a1 e383 a2e3 83aa e383 90e3 8383   ...............
+00000570: e382 afe3 82a8 e383 b3e3 8389 e381 b8e3  ................
+00000580: 81ae e68e a5e7 b69a 205b 6d65 6d6f 7279  ........ [memory
+00000590: 5f62 6163 6b65 6e64 5d0d 0a09 0923 20e3  _backend]....# .
+000005a0: 8387 e383 bce3 82bf e382 92e6 a0bc e7b4  ................
+000005b0: 8de3 8199 e382 8b43 6163 6865 6446 696c  .......CachedFil
+000005c0: 6544 6963 e381 aee5 889d e69c 9fe5 8c96  eDic............
+000005d0: 0d0a 0909 7365 6c66 2e63 6664 5f64 6174  ....self.cfd_dat
+000005e0: 6120 3d20 4361 6368 6564 4669 6c65 4469  a = CachedFileDi
+000005f0: 632e 636f 6e6e 2863 6664 5f64 6174 615f  c.conn(cfd_data_
+00000600: 6469 722c 2066 6d74 203d 2066 6d74 2c20  dir, fmt = fmt, 
+00000610: 636f 6e74 5f73 697a 655f 7468 203d 2063  cont_size_th = c
+00000620: 6f6e 745f 7369 7a65 5f74 682c 2063 6163  ont_size_th, cac
+00000630: 6865 5f6e 203d 2063 6163 6865 5f6e 2909  he_n = cache_n).
+00000640: 2320 e5af bee8 b1a1 e383 87e3 82a3 e383  # ..............
+00000650: ace3 82af e383 88e3 83aa e381 abe6 8ea5  ................
+00000660: e7b6 9a20 5b43 6163 6865 6446 696c 6544  ... [CachedFileD
+00000670: 6963 5d0d 0a09 0923 20e3 8397 e383 ade3  ic]....# .......
+00000680: 82b0 e383 a9e3 83a0 e7b5 82e4 ba86 e699  ................
+00000690: 82e3 81ae 636f 6d6d 6974 e5af bee8 b1a1  ....commit......
+000006a0: e381 abe8 87aa e8ba abe3 8292 e8bf bde5  ................
+000006b0: 8aa0 0d0a 0909 636f 6d6d 6974 5f74 6172  ......commit_tar
+000006c0: 6765 745f 6c73 2e61 7070 656e 6428 7365  get_ls.append(se
+000006d0: 6c66 290d 0a09 2320 6372 6561 7465 2c20  lf)...# create, 
+000006e0: 7570 6461 7465 e585 b1e9 809a 205b 6d65  update...... [me
+000006f0: 6d6f 7279 5f62 6163 6b65 6e64 5d0d 0a09  mory_backend]...
+00000700: 6465 6620 5f5f 7365 7469 7465 6d5f 5f28  def __setitem__(
+00000710: 7365 6c66 2c20 6b65 792c 2076 616c 7565  self, key, value
+00000720: 293a 0d0a 0909 2320 e696 b0e3 8197 e381  ):....# ........
+00000730: 8469 6e6e 6572 5f6b 6579 e381 aee7 949f  .inner_key......
+00000740: e688 900d 0a09 0969 6e6e 6572 5f6b 6579  .......inner_key
+00000750: 203d 2073 6c69 6d5f 6964 2e67 656e 286c   = slim_id.gen(l
+00000760: 616d 6264 6120 653a 2028 6520 696e 2073  ambda e: (e in s
+00000770: 656c 662e 6366 645f 6461 7461 292c 206c  elf.cfd_data), l
+00000780: 656e 6774 6820 3d20 3232 2909 2320 e58d  ength = 22).# ..
+00000790: 81e5 8886 e381 abe9 95b7 e381 846b 6579  .............key
+000007a0: 0d0a 0909 2320 e4b8 a1e6 96b9 e381 aee8  ....# ..........
+000007b0: be9e e69b b8e3 81ab e799 bbe9 8cb2 0d0a  ................
+000007c0: 0909 7365 6c66 2e6d 656d 5f69 6478 5b6b  ..self.mem_idx[k
+000007d0: 6579 5d20 3d20 696e 6e65 725f 6b65 790d  ey] = inner_key.
+000007e0: 0a09 0973 656c 662e 6366 645f 6461 7461  ...self.cfd_data
+000007f0: 5b69 6e6e 6572 5f6b 6579 5d20 3d20 7661  [inner_key] = va
+00000800: 6c75 650d 0a09 2320 6b65 79e8 aaad e381  lue...# key.....
+00000810: bfe5 87ba e381 9720 5b6d 656d 6f72 795f  ....... [memory_
+00000820: 6261 636b 656e 645d 0d0a 0964 6566 205f  backend]...def _
+00000830: 5f67 6574 6974 656d 5f5f 2873 656c 662c  _getitem__(self,
+00000840: 206b 6579 293a 0d0a 0909 696e 6e65 725f   key):....inner_
+00000850: 6b65 7920 3d20 7365 6c66 2e6d 656d 5f69  key = self.mem_i
+00000860: 6478 5b6b 6579 5d0d 0a09 0972 6574 7572  dx[key]....retur
+00000870: 6e20 7365 6c66 2e63 6664 5f64 6174 615b  n self.cfd_data[
+00000880: 696e 6e65 725f 6b65 795d 0d0a 0923 20e5  inner_key]...# .
+00000890: 898a e999 a420 5b6d 656d 6f72 795f 6261  ..... [memory_ba
+000008a0: 636b 656e 645d 0d0a 0964 6566 205f 5f64  ckend]...def __d
+000008b0: 656c 6974 656d 5f5f 2873 656c 662c 206b  elitem__(self, k
+000008c0: 6579 293a 2064 656c 2073 656c 662e 6d65  ey): del self.me
+000008d0: 6d5f 6964 785b 6b65 795d 0923 20e3 83a1  m_idx[key].# ...
+000008e0: e383 a2e3 83aa e383 bce3 8390 e383 83e3  ................
+000008f0: 82af e382 a8e3 83b3 e383 89e3 81ae e381  ................
+00000900: bfe3 818b e382 89e5 898a e999 a40d 0a09  ................
+00000910: 2320 e5ad 98e5 9ca8 e7a2 bae8 aa8d 205b  # ............ [
+00000920: 6d65 6d6f 7279 5f62 6163 6b65 6e64 5d0d  memory_backend].
+00000930: 0a09 6465 6620 5f5f 636f 6e74 6169 6e73  ..def __contains
+00000940: 5f5f 2873 656c 662c 206b 6579 293a 2072  __(self, key): r
+00000950: 6574 7572 6e20 286b 6579 2069 6e20 7365  eturn (key in se
+00000960: 6c66 2e6d 656d 5f69 6478 290d 0a09 2320  lf.mem_idx)...# 
+00000970: 6974 6572 2028 666f 72e6 9687 e884 88e7  iter (for.......
+00000980: ad89 e381 a7e3 81ae e588 a9e7 94a8 2920  ..............) 
+00000990: 5b6d 656d 6f72 795f 6261 636b 656e 645d  [memory_backend]
+000009a0: 0d0a 0964 6566 205f 5f69 7465 725f 5f28  ...def __iter__(
+000009b0: 7365 6c66 293a 2072 6574 7572 6e20 6974  self): return it
+000009c0: 6572 2873 656c 662e 6d65 6d5f 6964 7829  er(self.mem_idx)
+000009d0: 0d0a 0923 20e5 bcb7 e588 b663 6f6d 6d69  ...# ......commi
+000009e0: 7420 5b6d 656d 6f72 795f 6261 636b 656e  t [memory_backen
+000009f0: 645d 0d0a 0964 6566 2063 6f6d 6d69 7428  d]...def commit(
+00000a00: 7365 6c66 293a 0d0a 0909 7365 6c66 2e6d  self):....self.m
+00000a10: 656d 5f69 6478 2e63 6f6d 6d69 7428 290d  em_idx.commit().
+00000a20: 0a09 0973 656c 662e 6366 645f 6461 7461  ...self.cfd_data
+00000a30: 2e63 6f6d 6d69 7428 290d 0a09 2320 e696  .commit()...# ..
+00000a40: 87e5 ad97 e588 97e5 8c96 2028 e381 9de3  .......... (....
+00000a50: 81ae 312c 20e3 819d e381 ae32 290d 0a09  ..1, ......2)...
+00000a60: 6465 6620 5f5f 7374 725f 5f28 7365 6c66  def __str__(self
+00000a70: 293a 0d0a 0909 2320 6d65 6d6f 7279 2d62  ):....# memory-b
+00000a80: 6163 6b65 6e64 e381 aee9 9d9e e585 ace5  ackend..........
+00000a90: bc8f 4150 49e3 8292 e588 a9e7 94a8 0d0a  ..API...........
+00000aa0: 0909 666f 7220 6b65 795f 6578 616d 706c  ..for key_exampl
+00000ab0: 6520 696e 2073 656c 662e 6d65 6d5f 6964  e in self.mem_id
+00000ac0: 783a 2062 7265 616b 0923 206b 6579 e381  x: break.# key..
+00000ad0: aee4 be8b e382 92e5 8f96 e5be 970d 0a09  ................
+00000ae0: 0973 697a 6520 3d20 6c65 6e28 7365 6c66  .size = len(self
+00000af0: 2e6d 656d 5f69 6478 290d 0a09 0964 6174  .mem_idx)....dat
+00000b00: 615f 7374 7220 3d20 2822 2220 6966 2073  a_str = ("" if s
+00000b10: 697a 6520 3d3d 2030 0d0a 0909 0965 6c73  ize == 0.....els
+00000b20: 6520 6627 7b6b 6579 5f65 7861 6d70 6c65  e f'{key_example
+00000b30: 7d3a 207b 736f 7574 7328 7365 6c66 5b6b  }: {souts(self[k
+00000b40: 6579 5f65 7861 6d70 6c65 5d29 7d27 202b  ey_example])}' +
+00000b50: 0d0a 0909 0909 2822 2220 6966 2073 697a  ......("" if siz
+00000b60: 6520 3d3d 2031 2065 6c73 6520 6622 2c20  e == 1 else f", 
+00000b70: 2e2e 2e28 6e3d 7b73 697a 657d 2922 290d  ...(n={size})").
+00000b80: 0a09 0929 0d0a 0909 7265 7475 726e 2066  ...)....return f
+00000b90: 223c 534c 4442 2d43 4644 5f62 6163 6b65  "<SLDB-CFD_backe
+00000ba0: 6e64 207b 7b7b 6461 7461 5f73 7472 7d7d  nd {{{data_str}}
+00000bb0: 7d3e 220d 0a09 6465 6620 5f5f 7265 7072  }>"...def __repr
+00000bc0: 5f5f 2873 656c 6629 3a20 7265 7475 726e  __(self): return
+00000bd0: 2073 7472 2873 656c 6629 0d0a 0d0a 2320   str(self)....# 
+00000be0: 4361 6368 6564 4669 6c65 4469 63e3 8390  CachedFileDic...
+00000bf0: e383 83e3 82af e382 a8e3 83b3 e383 89e3  ................
+00000c00: 81b8 e381 aee6 8ea5 e7b6 9a20 5b63 6664  ........... [cfd
+00000c10: 5f62 6163 6b65 6e64 5d0d 0a64 6566 2063  _backend]..def c
+00000c20: 6f6e 6e28 0d0a 0964 6174 615f 6469 722c  onn(...data_dir,
+00000c30: 0923 20e3 8390 e383 83e3 82af e382 a8e3  .# .............
+00000c40: 83b3 e383 89e3 81ae e683 85e5 a0b1 e382  ................
+00000c50: 92e8 a898 e98c b2e3 8199 e382 8be3 8387  ................
+00000c60: e382 a3e3 83ac e382 afe3 8388 e383 aa0d  ................
+00000c70: 0a09 666d 7420 3d20 2266 706b 6c22 2c09  ..fmt = "fpkl",.
+00000c80: 2320 e383 90e3 8383 e382 afe3 82a8 e383  # ..............
+00000c90: b3e3 8389 e381 aee3 8395 e382 a1e3 82a4  ................
+00000ca0: e383 abe5 bda2 e5bc 8f20 2866 706b 6c3a  ......... (fpkl:
+00000cb0: 2066 6173 742d 7069 636b 6c65 2864 6566   fast-pickle(def
+00000cc0: 6175 6c74 292c 2070 6963 6b6c 653a 2070  ault), pickle: p
+00000cd0: 6963 6b6c 6529 0d0a 0963 6f6e 745f 7369  ickle)...cont_si
+00000ce0: 7a65 5f74 6820 3d20 3130 3020 2a20 3130  ze_th = 100 * 10
+00000cf0: 3234 202a 2a20 322c 0923 20e3 82b3 e383  24 ** 2,.# .....
+00000d00: b3e3 8386 e383 8ae3 82b5 e382 a4e3 82ba  ................
+00000d10: e79b aee5 ae89 0d0a 0963 6163 6865 5f6e  .........cache_n
+00000d20: 203d 2033 0923 20e6 9c80 e5a4 a76c 6f61   = 3.# ......loa
+00000d30: 64e3 82b3 e383 b3e3 8386 e383 8ae6 95b0  d...............
+00000d40: 0d0a 293a 0d0a 0923 20e3 8390 e383 83e3  ..):...# .......
+00000d50: 82af e382 a8e3 83b3 e383 89e3 81ae e382  ................
+00000d60: afe3 83a9 e382 b90d 0a09 7265 7475 726e  ..........return
+00000d70: 2043 4644 5f42 6163 6b65 6e64 2864 6174   CFD_Backend(dat
+00000d80: 615f 6469 722c 0d0a 0909 666d 7420 3d20  a_dir,....fmt = 
+00000d90: 666d 742c 0923 20e3 8390 e383 83e3 82af  fmt,.# .........
+00000da0: e382 a8e3 83b3 e383 89e3 81ae e383 95e3  ................
+00000db0: 82a1 e382 a4e3 83ab e5bd a2e5 bc8f 2028  .............. (
+00000dc0: 6670 6b6c 3a20 6661 7374 2d70 6963 6b6c  fpkl: fast-pickl
+00000dd0: 6528 6465 6661 756c 7429 2c20 7069 636b  e(default), pick
+00000de0: 6c65 3a20 7069 636b 6c65 290d 0a09 0963  le: pickle)....c
+00000df0: 6f6e 745f 7369 7a65 5f74 6820 3d20 636f  ont_size_th = co
+00000e00: 6e74 5f73 697a 655f 7468 2c09 2320 e382  nt_size_th,.# ..
+00000e10: b3e3 83b3 e383 86e3 838a e382 b5e3 82a4  ................
+00000e20: e382 bae7 9bae e5ae 890d 0a09 0963 6163  .............cac
+00000e30: 6865 5f6e 203d 2063 6163 6865 5f6e 0923  he_n = cache_n.#
+00000e40: 20e6 9c80 e5a4 a76c 6f61 64e3 82b3 e383   ......load.....
+00000e50: b3e3 8386 e383 8ae6 95b0 0d0a 0929 0d0a  .............)..
```

### Comparing `SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/test.py` & `SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/__init__.py` & `SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/test.py` & `SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.6/SymLinkDB/test.py` & `SymLinkDB-0.4.8/SymLinkDB/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.6/SymLinkDB.egg-info/PKG-INFO` & `SymLinkDB-0.4.8/SymLinkDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.6
+Version: 0.4.8
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.6/setup.py` & `SymLinkDB-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 5379 6d4c 696e 6b44  develop_SymLinkD
 000000c0: 422f 2229 2061 7320 703a 0d0a 0973 6574  B/") as p:...set
 000000d0: 7570 280d 0a09 096e 616d 6520 3d20 2253  up(....name = "S
 000000e0: 796d 4c69 6e6b 4442 222c 0d0a 0909 7665  ymLinkDB",....ve
-000000f0: 7273 696f 6e20 3d20 2230 2e34 2e36 222c  rsion = "0.4.6",
+000000f0: 7273 696f 6e20 3d20 2230 2e34 2e38 222c  rsion = "0.4.8",
 00000100: 0d0a 0909 6465 7363 7269 7074 696f 6e20  ....description 
 00000110: 3d20 2241 2067 7261 7068 2064 6174 6162  = "A graph datab
 00000120: 6173 6520 6368 6172 6163 7465 7269 7a65  ase characterize
 00000130: 6420 6279 2062 6964 6972 6563 7469 6f6e  d by bidirection
 00000140: 616c 206c 696e 6b73 2e20 4974 2061 6c6c  al links. It all
 00000150: 6f77 7320 666f 7220 696e 7475 6974 6976  ows for intuitiv
 00000160: 6520 6465 7369 676e 206f 6620 6461 7461  e design of data
@@ -33,15 +33,15 @@
 00000200: 732c 0d0a 0909 696e 7374 616c 6c5f 7265  s,....install_re
 00000210: 7175 6972 6573 203d 205b 2265 7a70 6970  quires = ["ezpip
 00000220: 222c 2022 736f 7574 3e3d 312e 322e 3122  ", "sout>=1.2.1"
 00000230: 2c20 2272 656c 7061 7468 222c 2022 736c  , "relpath", "sl
 00000240: 696d 2d69 643e 3d30 2e30 2e32 222c 2022  im-id>=0.0.2", "
 00000250: 6669 6573 3e3d 312e 342e 3022 2c20 2243  fies>=1.4.0", "C
 00000260: 6163 6865 6446 696c 6544 6963 3e3d 302e  achedFileDic>=0.
-00000270: 322e 3022 5d2c 0d0a 0909 6c6f 6e67 5f64  2.0"],....long_d
+00000270: 322e 3122 5d2c 0d0a 0909 6c6f 6e67 5f64  2.1"],....long_d
 00000280: 6573 6372 6970 7469 6f6e 203d 2070 2e6c  escription = p.l
 00000290: 6f6e 675f 6465 7363 7269 7074 696f 6e2c  ong_description,
 000002a0: 0d0a 0909 6c6f 6e67 5f64 6573 6372 6970  ....long_descrip
 000002b0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 000002c0: 6520 3d20 2274 6578 742f 6d61 726b 646f  e = "text/markdo
 000002d0: 776e 222c 0d0a 0909 6c69 6365 6e73 6520  wn",....license 
 000002e0: 3d20 2243 4330 2076 312e 3022 2c0d 0a09  = "CC0 v1.0",...
```

