# Comparing `tmp/pytrimal-0.7.0.tar.gz` & `tmp/pytrimal-0.8.0a1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrimal-0.7.0.tar", last modified: Fri Jul 21 18:59:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

