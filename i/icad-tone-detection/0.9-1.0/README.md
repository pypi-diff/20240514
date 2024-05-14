# Comparing `tmp/icad_tone_detection-0.9.tar.gz` & `tmp/icad_tone_detection-1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icad_tone_detection-0.9.tar", last modified: Mon May 13 05:53:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

