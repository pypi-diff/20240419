# Comparing `tmp/xrayutilities-1.7.6.tar.gz` & `tmp/xrayutilities-1.7.7-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrayutilities-1.7.6.tar", last modified: Thu Nov 16 16:22:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

