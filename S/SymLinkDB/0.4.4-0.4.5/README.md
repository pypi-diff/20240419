# Comparing `tmp/SymLinkDB-0.4.4.tar.gz` & `tmp/SymLinkDB-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SymLinkDB-0.4.4.tar", last modified: Thu Apr 18 11:39:00 2024, max compression
+gzip compressed data, was "SymLinkDB-0.4.5.tar", last modified: Thu Apr 18 12:02:48 2024, max compression
```

## Comparing `SymLinkDB-0.4.4.tar` & `SymLinkDB-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/
--rw-rw-rw-   0        0        0    36975 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.248051 SymLinkDB-0.4.4/SymLinkDB/
--rw-rw-rw-   0        0        0    46974 2024-04-18 11:38:15.000000 SymLinkDB-0.4.4/SymLinkDB/__init__.py
--rw-rw-rw-   0        0        0    46374 2024-04-18 11:25:11.000000 SymLinkDB-0.4.4/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py
--rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.4/SymLinkDB/document_code.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.214854 SymLinkDB-0.4.4/SymLinkDB/parts/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.264128 SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/
--rw-rw-rw-   0        0        0     3211 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/__init__.py
--rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/
--rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/__init__.py
--rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/test.py
--rw-rw-rw-   0        0        0    11537 2024-03-26 07:32:05.000000 SymLinkDB-0.4.4/SymLinkDB/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:39:00.264128 SymLinkDB-0.4.4/SymLinkDB.egg-info/
--rw-rw-rw-   0        0        0    36975 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2024-04-18 11:39:00.000000 SymLinkDB-0.4.4/SymLinkDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:39:00.272140 SymLinkDB-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-18 11:38:34.000000 SymLinkDB-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/
+-rw-rw-rw-   0        0        0    36975 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 12:02:47.994616 SymLinkDB-0.4.5/SymLinkDB/
+-rw-rw-rw-   0        0        0    46923 2024-04-18 12:01:26.000000 SymLinkDB-0.4.5/SymLinkDB/__init__.py
+-rw-rw-rw-   0        0        0    46374 2024-04-18 11:25:11.000000 SymLinkDB-0.4.5/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py
+-rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.5/SymLinkDB/document_code.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:02:47.970590 SymLinkDB-0.4.5/SymLinkDB/parts/
+drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.015778 SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/
+-rw-rw-rw-   0        0        0     3211 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/__init__.py
+-rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/test.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/
+-rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/__init__.py
+-rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/test.py
+-rw-rw-rw-   0        0        0    11537 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/SymLinkDB/test.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.010662 SymLinkDB-0.4.5/SymLinkDB.egg-info/
+-rw-rw-rw-   0        0        0    36975 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       69 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-18 12:02:24.000000 SymLinkDB-0.4.5/setup.py
```

### Comparing `SymLinkDB-0.4.4/PKG-INFO` & `SymLinkDB-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.4
+Version: 0.4.5
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.4/README.md` & `SymLinkDB-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB/__init__.py` & `SymLinkDB-0.4.5/SymLinkDB/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,16 +607,15 @@
 			return rec_ls
 		# 単一要素を処理する場合
 		rec_id = to_rec_id(rec_id)	# rec指定をrec_id指定に統一化 (どちらでもないtypeは例外を投げる)
 		return Record(rec_id, table = self)	# レコードクラス [SymLinkDB]
 	# レコードの存在確認 [SymLinkDB]
 	def __contains__(self, rec_id):
 		rec_id = to_rec_id(rec_id)	# rec指定をrec_id指定に統一化 (どちらでもないtypeは例外を投げる)
-		all_rec_ids = self.backend[("table_info", "all_rec_ids", self.table_id)]
-		return (rec_id in all_rec_ids)
+		return (("rec", self.table_id, rec_id) in self.backend)
 	# レコード数取得 [SymLinkDB]
 	def __len__(self): return self.backend[("table_info", "rec_n", self.table_id)]
 	# tableのイテレート [SymLinkDB]
 	def __iter__(self):
 		for rec_id in self.backend[("table_info", "all_rec_ids", self.table_id)]:
 			yield self[rec_id]
 	# レコードの削除 [SymLinkDB]
```

### Comparing `SymLinkDB-0.4.4/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py` & `SymLinkDB-0.4.5/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB/document_code.py` & `SymLinkDB-0.4.5/SymLinkDB/document_code.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/__init__.py` & `SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB/parts/cfd_backend/test.py` & `SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/__init__.py` & `SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB/parts/memory_backend/test.py` & `SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB/test.py` & `SymLinkDB-0.4.5/SymLinkDB/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.4/SymLinkDB.egg-info/PKG-INFO` & `SymLinkDB-0.4.5/SymLinkDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.4
+Version: 0.4.5
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.4/setup.py` & `SymLinkDB-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 5379 6d4c 696e 6b44  develop_SymLinkD
 000000c0: 422f 2229 2061 7320 703a 0d0a 0973 6574  B/") as p:...set
 000000d0: 7570 280d 0a09 096e 616d 6520 3d20 2253  up(....name = "S
 000000e0: 796d 4c69 6e6b 4442 222c 0d0a 0909 7665  ymLinkDB",....ve
-000000f0: 7273 696f 6e20 3d20 2230 2e34 2e34 222c  rsion = "0.4.4",
+000000f0: 7273 696f 6e20 3d20 2230 2e34 2e35 222c  rsion = "0.4.5",
 00000100: 0d0a 0909 6465 7363 7269 7074 696f 6e20  ....description 
 00000110: 3d20 2241 2067 7261 7068 2064 6174 6162  = "A graph datab
 00000120: 6173 6520 6368 6172 6163 7465 7269 7a65  ase characterize
 00000130: 6420 6279 2062 6964 6972 6563 7469 6f6e  d by bidirection
 00000140: 616c 206c 696e 6b73 2e20 4974 2061 6c6c  al links. It all
 00000150: 6f77 7320 666f 7220 696e 7475 6974 6976  ows for intuitiv
 00000160: 6520 6465 7369 676e 206f 6620 6461 7461  e design of data
```

