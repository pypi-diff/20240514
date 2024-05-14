# Comparing `tmp/comun_va-3.4.tar.gz` & `tmp/comun_va-3.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-3.4.tar", last modified: Thu May  9 07:51:33 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

