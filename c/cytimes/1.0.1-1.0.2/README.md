# Comparing `tmp/cytimes-1.0.1.tar.gz` & `tmp/cytimes-1.0.2-cp311-cp311-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytimes-1.0.1.tar", last modified: Tue May 14 03:52:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

