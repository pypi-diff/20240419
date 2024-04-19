# Comparing `tmp/qh3-1.0.0.tar.gz` & `tmp/qh3-1.0.1-pp310-pypy310_pp73-manylinux_2_17_ppc64.manylinux2014_ppc64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

