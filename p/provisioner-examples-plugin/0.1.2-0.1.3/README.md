# Comparing `tmp/provisioner_examples_plugin-0.1.2-py3-none-any.whl.zip` & `tmp/provisioner_examples_plugin-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 24739 bytes, number of entries: 31
+Zip file size: 24738 bytes, number of entries: 31
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner_examples_plugin/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner_examples_plugin/anchor/__init__.py
 -rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 provisioner_examples_plugin/anchor/anchor_cmd.py
 -rw-r--r--  2.0 unx     1822 b- defN 80-Jan-01 00:00 provisioner_examples_plugin/anchor/cli.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner_examples_plugin/ansible/__init__.py
 -rw-r--r--  2.0 unx     1406 b- defN 80-Jan-01 00:00 provisioner_examples_plugin/ansible/cli.py
 -rw-r--r--  2.0 unx     1187 b- defN 80-Jan-01 00:00 provisioner_examples_plugin/ansible/hello_world_cmd.py
@@ -22,12 +22,12 @@
 -rw-r--r--  2.0 unx     7890 b- defN 80-Jan-01 00:00 provisioner_features_lib/remote/typer_remote_opts.py
 -rw-r--r--  2.0 unx    12929 b- defN 80-Jan-01 00:00 provisioner_features_lib/sd_card/image_burner.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner_features_lib/shared/domain/__init__.py
 -rw-r--r--  2.0 unx      495 b- defN 80-Jan-01 00:00 provisioner_features_lib/shared/domain/config.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 provisioner_features_lib/vcs/domain/__init__.py
 -rw-r--r--  2.0 unx     1862 b- defN 80-Jan-01 00:00 provisioner_features_lib/vcs/domain/config.py
 -rw-r--r--  2.0 unx     3283 b- defN 80-Jan-01 00:00 provisioner_features_lib/vcs/typer_vcs_opts.py
--rw-r--r--  2.0 unx      397 b- defN 80-Jan-01 00:00 provisioner_examples_plugin-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_examples_plugin-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      135 b- defN 80-Jan-01 00:00 provisioner_examples_plugin-0.1.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3164 b- defN 16-Jan-01 00:00 provisioner_examples_plugin-0.1.2.dist-info/RECORD
-31 files, 72083 bytes uncompressed, 19395 bytes compressed:  73.1%
+-rw-r--r--  2.0 unx      397 b- defN 80-Jan-01 00:00 provisioner_examples_plugin-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 provisioner_examples_plugin-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      135 b- defN 80-Jan-01 00:00 provisioner_examples_plugin-0.1.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3164 b- defN 16-Jan-01 00:00 provisioner_examples_plugin-0.1.3.dist-info/RECORD
+31 files, 72083 bytes uncompressed, 19394 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: provisioner_features_lib/vcs/domain/config.py
 Comment: 
 
 Filename: provisioner_features_lib/vcs/typer_vcs_opts.py
 Comment: 
 
-Filename: provisioner_examples_plugin-0.1.2.dist-info/METADATA
+Filename: provisioner_examples_plugin-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: provisioner_examples_plugin-0.1.2.dist-info/WHEEL
+Filename: provisioner_examples_plugin-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: provisioner_examples_plugin-0.1.2.dist-info/entry_points.txt
+Filename: provisioner_examples_plugin-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: provisioner_examples_plugin-0.1.2.dist-info/RECORD
+Filename: provisioner_examples_plugin-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## provisioner_examples_plugin/resources/version.txt

```diff
@@ -1 +1 @@
-0.1.2
+0.1.3
```

## Comparing `provisioner_examples_plugin-0.1.2.dist-info/RECORD` & `provisioner_examples_plugin-0.1.3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 provisioner_examples_plugin/ansible/hello_world_cmd.py,sha256=48_FIR7QLwsbmFi_QeaomaaguB7c4RRGEy1KyO8Hgis,1187
 provisioner_examples_plugin/ansible/hello_world_runner.py,sha256=56feFyvUpp-MHuU2ODei8j6cgWTMab1RttyELVcBeVQ,3908
 provisioner_examples_plugin/config/domain/config.py,sha256=jfTd3eGoSkvpkQN8nBPzERA2iX287dE1DJPmsvRtF3A,1575
 provisioner_examples_plugin/main.py,sha256=ygt4o6WrTkgZMBWRU9ZNCG3P5mK_6sY0Fwi1-34V9ak,1698
 provisioner_examples_plugin/main_dev.py,sha256=sx8u0fUxnuV04qYBgu-0UNwdPVWNwXyt3L28DWs-a6w,1827
 provisioner_examples_plugin/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner_examples_plugin/resources/config.yaml,sha256=8aG6GSAUttnTvY8f7ldRSMYVsrU0MiaWqPVin0ome9g,353
-provisioner_examples_plugin/resources/version.txt,sha256=VKRsZExOtvEo-Z9_CENJGGF7MbaAUi7UrLV8lCQ3KCc,5
+provisioner_examples_plugin/resources/version.txt,sha256=2_CXjsK1h6XWGH_cxBzOn_LA647vrboOtR84QKtu60Y,5
 provisioner_features_lib/anchor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner_features_lib/anchor/anchor_runner.py,sha256=vtqoY43clkLJJWr2DQVyUkipCbS7YcGDQHIZHiHghIs,5320
 provisioner_features_lib/anchor/playbooks/anchor_run.yaml,sha256=p4uLc55sTiRc3RjY3bU5q0-oHZGrT5xiZ54ep9DTkVA,243
 provisioner_features_lib/remote/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner_features_lib/remote/domain/config.py,sha256=aj4uae7pYlS2gWn0aaf4dktEJSkN4USmtODvw34qac4,3897
 provisioner_features_lib/remote/remote_connector.py,sha256=HEjcOkG40KkndfkbZdeiCV_QDy2n-lk_zNjeugWVIas,17078
 provisioner_features_lib/remote/typer_remote_opts.py,sha256=3-q_70X2QZ_d3u-Ewe-qgIUrfA-6H8jfpw_NESerp9A,7890
 provisioner_features_lib/sd_card/image_burner.py,sha256=RMDDKbGnP9lUXNxR9eXFRrJsBjMFN-h7Pa1DVBhbn2g,12929
 provisioner_features_lib/shared/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner_features_lib/shared/domain/config.py,sha256=3DdHOrh3DZo-ye7KznROB15jwCLoY2tTzSrTQ4k26RI,495
 provisioner_features_lib/vcs/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 provisioner_features_lib/vcs/domain/config.py,sha256=8Uq1LI0hUTj4OvQK3EBmd9bXAcA7D4pkO7-LcEZbiYs,1862
 provisioner_features_lib/vcs/typer_vcs_opts.py,sha256=pVw_qPJUNjv8dz7f_UmjnGOOoTU6Bs_Lu3p9kMvPID4,3283
-provisioner_examples_plugin-0.1.2.dist-info/METADATA,sha256=ug03LiTeaddHvDIJcflkBuPB4quzy-MCjknRSGlg4Jc,397
-provisioner_examples_plugin-0.1.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-provisioner_examples_plugin-0.1.2.dist-info/entry_points.txt,sha256=N5E52bmnvgBxOGME4Be0ZOaQfsuSZcMsN6Lew8Ozfw0,135
-provisioner_examples_plugin-0.1.2.dist-info/RECORD,,
+provisioner_examples_plugin-0.1.3.dist-info/METADATA,sha256=_3aqGEkQDs_7IVubN4Gpnqj5rAjrieAyr-9epQ3mW5A,397
+provisioner_examples_plugin-0.1.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+provisioner_examples_plugin-0.1.3.dist-info/entry_points.txt,sha256=N5E52bmnvgBxOGME4Be0ZOaQfsuSZcMsN6Lew8Ozfw0,135
+provisioner_examples_plugin-0.1.3.dist-info/RECORD,,
```

