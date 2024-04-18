# Comparing `tmp/Seq2SeqSharp-2.8.10.tar.gz` & `tmp/Seq2SeqSharp-2.8.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Works/Projects/Seq2SeqSharp/PyPackage/dist/.tmp-e38h21w3/Seq2SeqSharp-2.8.10.tar", last modified: Thu Apr 18 05:30:01 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

