# Comparing `tmp/syops-0.0.4.tar.gz` & `tmp/syops-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/cgy/Transformers/SNN/syops-counter/dist/.tmp-n1_4ai9u/syops-0.0.4.tar", last modified: Thu Apr 27 09:06:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

