# Comparing `tmp/scikit-fibers-0.9.3.2.tar.gz` & `tmp/scikit_fibers-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-fibers-0.9.3.2.tar", last modified: Mon Dec 11 22:16:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

