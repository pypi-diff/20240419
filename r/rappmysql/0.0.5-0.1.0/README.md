# Comparing `tmp/rappmysql-0.0.5.tar.gz` & `tmp/rappmysql-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rappmysql-0.0.5.tar", last modified: Mon Dec  4 16:32:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

