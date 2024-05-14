# Comparing `tmp/ddtrace-2.9.0rc6.tar.gz` & `tmp/ddtrace-2.9.0rc7-cp37-cp37m-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddtrace-2.9.0rc6.tar", last modified: Fri May 10 17:37:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

