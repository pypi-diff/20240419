# Comparing `tmp/edc_action_item-0.3.89.tar.gz` & `tmp/edc_action_item-0.3.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc_action_item-0.3.89.tar", last modified: Thu Apr 18 23:15:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

