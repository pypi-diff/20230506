# Comparing `tmp/pyvroom-1.13.0.tar.gz` & `tmp/pyvroom-1.13.1-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvroom-1.13.0.tar", last modified: Mon Mar 20 08:22:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

