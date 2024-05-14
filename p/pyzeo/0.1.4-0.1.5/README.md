# Comparing `tmp/pyzeo-0.1.4.tar.gz` & `tmp/pyzeo-0.1.5-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzeo-0.1.4.tar", last modified: Sun Jun 18 13:26:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

