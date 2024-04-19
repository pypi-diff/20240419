# Comparing `tmp/resc_backend-3.0.1.tar.gz` & `tmp/resc_backend-3.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-3.0.1.tar", last modified: Mon Apr  8 09:09:33 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

