# Comparing `tmp/policyengine-us-0.770.0.tar.gz` & `tmp/policyengine_us-0.770.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-us-0.770.0.tar", last modified: Fri May 10 15:56:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

