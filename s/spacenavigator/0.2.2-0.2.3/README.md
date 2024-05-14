# Comparing `tmp/spacenavigator-0.2.2.tar.gz` & `tmp/spacenavigator-0.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\spacenavigator-0.2.2.tar", last modified: Thu Aug 29 15:38:30 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

