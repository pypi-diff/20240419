# Comparing `tmp/cheltuieli-0.2.0.tar.gz` & `tmp/cheltuieli-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheltuieli-0.2.0.tar", last modified: Fri Apr  5 10:07:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

