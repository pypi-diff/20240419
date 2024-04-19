# Comparing `tmp/MyGaiaDB-0.4.1.tar.gz` & `tmp/MyGaiaDB-0.4.2-cp38-cp38-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyGaiaDB-0.4.1.tar", last modified: Sun Oct  8 04:07:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

