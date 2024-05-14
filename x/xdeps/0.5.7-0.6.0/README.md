# Comparing `tmp/xdeps-0.5.7.tar.gz` & `tmp/xdeps-0.6.0-cp38-cp38-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdeps-0.5.7.tar", last modified: Fri Apr 19 13:21:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

