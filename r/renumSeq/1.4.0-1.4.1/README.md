# Comparing `tmp/renumSeq-1.4.0.tar.gz` & `tmp/renumSeq-1.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renumSeq-1.4.0.tar", last modified: Tue Sep 26 21:17:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

