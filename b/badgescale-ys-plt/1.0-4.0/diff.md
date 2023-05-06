# Comparing `tmp/badgescale_ys_plt-1.0.tar.gz` & `tmp/badgescale_ys_plt-4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgescale_ys_plt-1.0.tar", last modified: Fri Apr 28 20:37:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

