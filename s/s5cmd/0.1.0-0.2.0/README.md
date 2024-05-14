# Comparing `tmp/s5cmd-0.1.0.tar.gz` & `tmp/s5cmd-0.2.0-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5cmd-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

