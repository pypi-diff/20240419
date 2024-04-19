# Comparing `tmp/medicafe-0.240418.3.tar.gz` & `tmp/medicafe-0.240419.1.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240418.3.tar", last modified: Fri Apr 19 07:49:59 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

