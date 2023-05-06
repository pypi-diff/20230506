# Comparing `tmp/xhs-0.1.5.tar.gz` & `tmp/xhs-0.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.5.tar", last modified: Tue Apr 25 14:08:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

