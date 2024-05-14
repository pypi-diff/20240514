# Comparing `tmp/biomedisa-2024.5.16.tar.gz` & `tmp/biomedisa-2024.5.17-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedisa-2024.5.16.tar", last modified: Thu May  9 05:14:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

