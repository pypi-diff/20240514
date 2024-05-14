# Comparing `tmp/AlphaDSSP-0.1.tar.gz` & `tmp/AlphaDSSP-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlphaDSSP-0.1.tar", last modified: Tue May 14 18:49:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

