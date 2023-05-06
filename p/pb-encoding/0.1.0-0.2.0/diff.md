# Comparing `tmp/pb_encoding-0.1.0.tar.gz` & `tmp/pb_encoding-0.2.0.tar.gz`

## Comparing `pb_encoding-0.1.0.tar` & `pb_encoding-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/src/pb_encoding/__init__.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/src/pb_encoding/decoder.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/src/pb_encoding/encoder.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/src/pb_encoding/typing.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/.gitignore
--rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/LICENSE
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/LICENSE_origin
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/README.md
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pb_encoding-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/__init__.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/decoder.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/encoder.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/src/pb_encoding/typing.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/LICENSE_origin
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/README.md
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pb_encoding-0.2.0/PKG-INFO
```

### Comparing `pb_encoding-0.1.0/src/pb_encoding/decoder.py` & `pb_encoding-0.2.0/src/pb_encoding/decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,26 +96,33 @@
 
 def DecodeString(buffer, pos):
     size, pos = DecodeVarint(buffer, pos)
     new_pos = pos + size
     return buffer[pos:new_pos].decode("utf-8"), new_pos
 
 
+def DecodeBytes(buffer, pos) -> Tuple[bytes, int]:
+    size, pos = DecodeVarint(buffer, pos)
+    new_pos = pos + size
+    return bytes(buffer[pos:new_pos]), new_pos
+
+
 _field_decoder_mapping = {
     "int32": DecodeSignedVarint32,
     "int64": DecodeSignedVarint,
     "uint32": DecodeVarint32,
     "uint64": DecodeVarint,
     "sint32": DecodeSignedVarint32ZigZag,
     "sint64": DecodeSignedVarintZigZag,
     "fixed32": DecodeFixed32,
     "fixed64": DecodeFixed64,
     "sfixed32": DecodeSFixed32,
     "sfixed64": DecodeSFixed64,
     "string": DecodeString,
+    "bytes": DecodeBytes,
 }
 
 
 def getDecoder(type: SupportedType) -> Callable:
     return _field_decoder_mapping[type]
```

### Comparing `pb_encoding-0.1.0/src/pb_encoding/encoder.py` & `pb_encoding-0.2.0/src/pb_encoding/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 def _StructPackEncoder(format):
     def _EncodeField(write, value):
         write(struct.pack(format, value))
 
     return _EncodeField
 
 
+def EncodeBytes(write, value: bytes):
+    EncodeVarint(write, len(value))
+    write(value)
+
+
 EncodeFixed32 = _StructPackEncoder("<I")
 EncodeFixed64 = _StructPackEncoder("<Q")
 EncodeSFixed32 = _StructPackEncoder("<i")
 EncodeSFixed64 = _StructPackEncoder("<q")
 
 
 def EncodeString(write, value):
@@ -70,14 +75,15 @@
     "sint32": EncodeSignedVarintZigZag,
     "sint64": EncodeSignedVarintZigZag,
     "fixed32": EncodeFixed32,
     "fixed64": EncodeFixed64,
     "sfixed32": EncodeSFixed32,
     "sfixed64": EncodeSFixed64,
     "string": EncodeString,
+    "bytes": EncodeBytes,
 }
 
 
 def getEncoder(type: SupportedType) -> Callable:
     return _field_encoder_mapping[type]
```

### Comparing `pb_encoding-0.1.0/.gitignore` & `pb_encoding-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.1.0/LICENSE` & `pb_encoding-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.1.0/LICENSE_origin` & `pb_encoding-0.2.0/LICENSE_origin`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.1.0/pyproject.toml` & `pb_encoding-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pb_encoding-0.1.0/PKG-INFO` & `pb_encoding-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pb_encoding
-Version: 0.1.0
+Version: 0.2.0
 Summary: Some encode/decode functions extracted from google.protobuf
 Project-URL: homepage, https://github.com/Grvzard/pb_encoding
 License-File: LICENSE
 License-File: LICENSE_origin
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

