# Comparing `tmp/hgchat-0.1.2.tar.gz` & `tmp/hgchat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgchat-0.1.2.tar", max compression
+gzip compressed data, was "hgchat-0.1.3.tar", max compression
```

## Comparing `hgchat-0.1.2.tar` & `hgchat-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      683 2023-04-30 10:09:45.807393 hgchat-0.1.2/README.md
--rw-r--r--   0        0        0     4031 2023-05-05 20:06:48.846991 hgchat-0.1.2/hgchat/__init__.py
--rw-r--r--   0        0        0      438 2023-05-05 20:06:55.649969 hgchat-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 hgchat-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-30 10:09:45.807393 hgchat-0.1.3/README.md
+-rw-r--r--   0        0        0     4257 2023-05-06 17:20:37.953118 hgchat-0.1.3/hgchat/__init__.py
+-rw-r--r--   0        0        0      438 2023-05-06 17:20:54.300165 hgchat-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 hgchat-0.1.3/PKG-INFO
```

### Comparing `hgchat-0.1.2/README.md` & `hgchat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hgchat-0.1.2/hgchat/__init__.py` & `hgchat-0.1.3/hgchat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,18 +91,23 @@
         )
         if r.status_code != 200:
             raise Exception("Failed to send message")
 
         for chunk in r.iter_content(chunk_size=None):
             data = chunk.decode("utf-8")
             if chunk:
-                data = json.loads(chunk[5:])
-                if "error" not in data:
-                    yield data
-                else:
-                    print("error: ", data["error"])
-                    break
+                try:
+                    data = json.loads(chunk[5:].strip())
+                    if "error" not in data:
+                        yield data
+                    else:
+                        print("error: ", data["error"])
+                        break
+                except json.decoder.JSONDecodeError:
+                    # sometimes the response is not valid json
+                    # like b'' 
+                    pass
 
 if __name__ == "__main__":
     chat = HGChat()
     for data in chat.ask("Hello"):
         print(data)
```

### Comparing `hgchat-0.1.2/PKG-INFO` & `hgchat-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgchat
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: 0xMRTT
 Author-email: 0xMRTT@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

