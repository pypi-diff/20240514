# Comparing `tmp/anycrc-0.6.3.tar.gz` & `tmp/anycrc-0.7.0-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.6.3.tar", last modified: Mon May 13 16:49:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

