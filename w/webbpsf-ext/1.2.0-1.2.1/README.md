# Comparing `tmp/webbpsf_ext-1.2.0.tar.gz` & `tmp/webbpsf_ext-1.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webbpsf_ext-1.2.0.tar", last modified: Tue May 14 02:30:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

