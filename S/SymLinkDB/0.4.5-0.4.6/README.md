# Comparing `tmp/SymLinkDB-0.4.5.tar.gz` & `tmp/SymLinkDB-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SymLinkDB-0.4.5.tar", last modified: Thu Apr 18 12:02:48 2024, max compression
+gzip compressed data, was "SymLinkDB-0.4.6.tar", last modified: Fri Apr 19 02:37:14 2024, max compression
```

## Comparing `SymLinkDB-0.4.5.tar` & `SymLinkDB-0.4.6.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/
--rw-rw-rw-   0        0        0    36975 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 12:02:47.994616 SymLinkDB-0.4.5/SymLinkDB/
--rw-rw-rw-   0        0        0    46923 2024-04-18 12:01:26.000000 SymLinkDB-0.4.5/SymLinkDB/__init__.py
--rw-rw-rw-   0        0        0    46374 2024-04-18 11:25:11.000000 SymLinkDB-0.4.5/SymLinkDB/__init__BACKUP_2024年4月18日-get_link_infoの書き換え前.py
--rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.5/SymLinkDB/document_code.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:02:47.970590 SymLinkDB-0.4.5/SymLinkDB/parts/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.015778 SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/
--rw-rw-rw-   0        0        0     3211 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/__init__.py
--rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/
--rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/__init__.py
--rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/test.py
--rw-rw-rw-   0        0        0    11537 2024-03-26 07:32:05.000000 SymLinkDB-0.4.5/SymLinkDB/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:02:48.010662 SymLinkDB-0.4.5/SymLinkDB.egg-info/
--rw-rw-rw-   0        0        0    36975 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2024-04-18 12:02:47.000000 SymLinkDB-0.4.5/SymLinkDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 12:02:48.018508 SymLinkDB-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-18 12:02:24.000000 SymLinkDB-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/
+-rw-rw-rw-   0        0        0    36975 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.037514 SymLinkDB-0.4.6/SymLinkDB/
+-rw-rw-rw-   0        0        0    47330 2024-04-19 02:36:24.000000 SymLinkDB-0.4.6/SymLinkDB/__init__.py
+-rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.6/SymLinkDB/document_code.py
+drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.021528 SymLinkDB-0.4.6/SymLinkDB/parts/
+drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/
+-rw-rw-rw-   0        0        0     3211 2024-03-26 07:32:05.000000 SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/__init__.py
+-rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/
+-rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/__init__.py
+-rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/test.py
+-rw-rw-rw-   0        0        0    11537 2024-04-19 02:36:35.000000 SymLinkDB-0.4.6/SymLinkDB/test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 02:37:14.045539 SymLinkDB-0.4.6/SymLinkDB.egg-info/
+-rw-rw-rw-   0        0        0    36975 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       69 2024-04-19 02:37:13.000000 SymLinkDB-0.4.6/SymLinkDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 02:37:14.053516 SymLinkDB-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-19 02:36:53.000000 SymLinkDB-0.4.6/setup.py
```

### Comparing `SymLinkDB-0.4.5/PKG-INFO` & `SymLinkDB-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.5
+Version: 0.4.6
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.5/README.md` & `SymLinkDB-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.5/SymLinkDB/__init__.py` & `SymLinkDB-0.4.6/SymLinkDB/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,16 +447,19 @@
 			# 検索インデックスの削除
 			del_search_idx(old_data, self.table.search_keys, self.table_id, self.id, self.table.backend)
 			# 検索インデックスの追加
 			add_search_idx(new_data, self.table.search_keys, self.table_id, self.id, self.table.backend)
 	# link_setの取得 [SymLinkDB]
 	def __getitem__(self, query):
 		self.is_deleted(raise_err = True)	# 自身が削除済みかどうかを判定
-		# クエリからlink情報取得 (キャッシュ化バージョン; クエリは「role名」または「関係名, role名」)
-		link_info = self.table.cached_link_info_getter(query)
+		# 注意: 「必要な情報はメモリではなくbackendから都度請求する」という設計思想に基づき、キャッシュ化を使わない
+		# # クエリからlink情報取得 (キャッシュ化バージョン; クエリは「role名」または「関係名, role名」)
+		# link_info = self.table.cached_link_info_getter(query)
+		# クエリからlink情報取得 (クエリは「role名」または「関係名, role名」)
+		link_info = get_link_info(query, self.table_id, self.table.sldb.backend)	# role名あるいはrole名とlink table名からlink情報を取得
 		# LinkSetオブジェクトを作成して返す
 		return LinkSet(	# LinkSetクラス [SymLinkDB]
 			link_info["link_table_id"],	# link table ID
 			link_info["link_table_name"],	# link table名
 			subj_role_info = link_info["subj_role_info"],	# 自roleの情報
 			obj_role_info = link_info["obj_role_info"],	# 相手側roleの情報
 			rec = self)	# linkオブジェクト
```

### Comparing `SymLinkDB-0.4.5/SymLinkDB/document_code.py` & `SymLinkDB-0.4.6/SymLinkDB/document_code.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/__init__.py` & `SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.5/SymLinkDB/parts/cfd_backend/test.py` & `SymLinkDB-0.4.6/SymLinkDB/parts/cfd_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/__init__.py` & `SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.5/SymLinkDB/parts/memory_backend/test.py` & `SymLinkDB-0.4.6/SymLinkDB/parts/memory_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.5/SymLinkDB/test.py` & `SymLinkDB-0.4.6/SymLinkDB/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.5/SymLinkDB.egg-info/PKG-INFO` & `SymLinkDB-0.4.6/SymLinkDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.5
+Version: 0.4.6
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.5/setup.py` & `SymLinkDB-0.4.6/setup.py`

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
-000000f0: 7273 696f 6e20 3d20 2230 2e34 2e35 222c  rsion = "0.4.5",
+000000f0: 7273 696f 6e20 3d20 2230 2e34 2e36 222c  rsion = "0.4.6",
 00000100: 0d0a 0909 6465 7363 7269 7074 696f 6e20  ....description 
 00000110: 3d20 2241 2067 7261 7068 2064 6174 6162  = "A graph datab
 00000120: 6173 6520 6368 6172 6163 7465 7269 7a65  ase characterize
 00000130: 6420 6279 2062 6964 6972 6563 7469 6f6e  d by bidirection
 00000140: 616c 206c 696e 6b73 2e20 4974 2061 6c6c  al links. It all
 00000150: 6f77 7320 666f 7220 696e 7475 6974 6976  ows for intuitiv
 00000160: 6520 6465 7369 676e 206f 6620 6461 7461  e design of data
```

