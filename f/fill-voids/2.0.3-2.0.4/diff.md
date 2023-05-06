# Comparing `tmp/fill_voids-2.0.3.tar.gz` & `tmp/fill_voids-2.0.4-cp310-cp310-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fill_voids-2.0.3.tar", last modified: Fri Dec  9 21:09:03 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

