# Comparing `tmp/bartbroere_eland-8.9.0.tar.gz` & `tmp/bartbroere_eland-8.9.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bartbroere_eland-8.9.0.tar", last modified: Fri Sep  1 08:13:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

