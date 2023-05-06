# Comparing `tmp/botocore-a-la-carte-osis-1.29.127.tar.gz` & `tmp/botocore_a_la_carte_osis-1.29.129-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.127.tar", last modified: Fri May  5 01:09:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

