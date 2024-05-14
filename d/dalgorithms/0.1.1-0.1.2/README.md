# Comparing `tmp/dalgorithms-0.1.1.tar.gz` & `tmp/dalgorithms-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalgorithms-0.1.1.tar", last modified: Mon May 13 23:21:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

