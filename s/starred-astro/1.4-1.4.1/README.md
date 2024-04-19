# Comparing `tmp/starred-astro-1.4.tar.gz` & `tmp/starred_astro-1.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred-astro-1.4.tar", last modified: Fri Mar  8 12:42:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

