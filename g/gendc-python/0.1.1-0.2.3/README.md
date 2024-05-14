# Comparing `tmp/gendc-python-0.1.1.tar.gz` & `tmp/gendc_python-0.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gendc-python-0.1.1.tar", last modified: Thu Jan 25 20:30:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

