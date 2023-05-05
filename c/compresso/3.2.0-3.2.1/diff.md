# Comparing `tmp/compresso-3.2.0.tar.gz` & `tmp/compresso-3.2.1-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compresso-3.2.0.tar", last modified: Wed Jan  4 04:39:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

