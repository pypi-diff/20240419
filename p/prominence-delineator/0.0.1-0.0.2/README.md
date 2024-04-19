# Comparing `tmp/prominence-delineator-0.0.1.tar.gz` & `tmp/prominence_delineator-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prominence-delineator-0.0.1.tar", last modified: Thu Apr  4 10:12:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
