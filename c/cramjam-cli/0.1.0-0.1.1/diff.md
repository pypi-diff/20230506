# Comparing `tmp/cramjam_cli-0.1.0.tar.gz` & `tmp/cramjam_cli-0.1.1.tar.gz`

## Comparing `cramjam_cli-0.1.0.tar` & `cramjam_cli-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/Cargo.toml
--rw-r--r--   0     1000     1000      119 2023-05-06 03:24:57.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/README.md
--rw-r--r--   0     1000     1000      960 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/brotli.rs
--rw-r--r--   0     1000     1000      846 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/bzip2.rs
--rw-r--r--   0     1000     1000      878 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/deflate.rs
--rw-r--r--   0     1000     1000     1442 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/gzip.rs
--rw-r--r--   0     1000     1000     3637 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/lib.rs
--rw-r--r--   0     1000     1000     1230 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/lz4.rs
--rw-r--r--   0     1000     1000     1690 2023-05-06 03:24:57.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/snappy.rs
--rw-r--r--   0     1000     1000      837 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/local_dependencies/libcramjam/src/zstd.rs
--rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 cramjam_cli-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000     1136 2023-05-06 03:24:57.000000 cramjam_cli-0.1.0/README.md
--rw-r--r--   0     1000     1000      548 2023-05-03 18:20:54.000000 cramjam_cli-0.1.0/pyproject.toml
--rw-r--r--   0     1000     1000     6124 2023-05-06 03:24:57.000000 cramjam_cli-0.1.0/src/main.rs
--rw-r--r--   0     1000     1000       29 2023-05-06 03:24:15.000000 cramjam_cli-0.1.0/tests/test_cli.py
--rw-r--r--   0     1000     1000    19594 2023-05-06 03:24:57.000000 cramjam_cli-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 cramjam_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/Cargo.toml
+-rw-r--r--   0      501       20      119 2023-05-06 21:36:50.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/README.md
+-rw-r--r--   0      501       20      960 2023-05-06 21:36:50.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/brotli.rs
+-rw-r--r--   0      501       20      846 2023-05-06 21:36:50.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/bzip2.rs
+-rw-r--r--   0      501       20      878 2023-05-06 21:36:51.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/deflate.rs
+-rw-r--r--   0      501       20     1442 2023-05-06 21:36:51.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/gzip.rs
+-rw-r--r--   0      501       20     3637 2023-05-06 21:36:51.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/lib.rs
+-rw-r--r--   0      501       20     1230 2023-05-06 21:36:51.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/lz4.rs
+-rw-r--r--   0      501       20     1690 2023-05-06 21:36:51.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/snappy.rs
+-rw-r--r--   0      501       20      837 2023-05-06 21:36:51.000000 cramjam_cli-0.1.1/local_dependencies/libcramjam/src/zstd.rs
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 cramjam_cli-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20     1136 2023-05-06 21:36:47.000000 cramjam_cli-0.1.1/README.md
+-rw-r--r--   0      501       20      548 2023-05-06 21:36:48.000000 cramjam_cli-0.1.1/pyproject.toml
+-rw-r--r--   0      501       20     7182 2023-05-06 21:36:48.000000 cramjam_cli-0.1.1/src/main.rs
+-rw-r--r--   0      501       20     2244 2023-05-06 21:36:48.000000 cramjam_cli-0.1.1/tests/test_cli.py
+-rw-r--r--   0      501       20    19594 2023-05-06 21:38:13.000000 cramjam_cli-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 cramjam_cli-0.1.1/PKG-INFO
```

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/brotli.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/brotli.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/bzip2.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/bzip2.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/deflate.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/deflate.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/gzip.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/gzip.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/lib.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/lz4.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/lz4.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/snappy.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/snappy.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/local_dependencies/libcramjam/src/zstd.rs` & `cramjam_cli-0.1.1/local_dependencies/libcramjam/src/zstd.rs`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/README.md` & `cramjam_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/pyproject.toml` & `cramjam_cli-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cramjam_cli-0.1.0/src/main.rs` & `cramjam_cli-0.1.1/src/main.rs`

 * *Files 20% similar despite different names*

```diff
@@ -121,36 +121,56 @@
     let start = Instant::now();
     let nbytes = match m.codec {
         Codec::Snappy(conf) => match conf.action {
             Action::Compress => libcramjam::snappy::compress(input, &mut output),
             Action::Decompress => libcramjam::snappy::decompress(input, &mut output),
         },
         Codec::Lz4(conf) => {
-            // TODO: lz4 doesn't impl Read for their Encoder, so cannot determine
-            // number of bytes compressed without using Seek, which stdout doesn't have,
-            // as it's streaming. So here, we'll go ahead and read everything in then
-            // send it in as a cursor, file can remain as is.
-            // When lz4 implements Reader for the Encoder, then all this can go away.
-            // along with the `Seek` trait bound on the internal::compress function
-            if let Some(stdout) = ((&mut *output).as_any_mut()).downcast_mut::<StdoutLock>() {
-                let mut data = vec![];
-                libcramjam::lz4::compress(input, &mut Cursor::new(&mut data), conf.level.map(|v| v as _))?;
-                io::copy(&mut Cursor::new(data), stdout).map(|v| v as usize)
-            } else {
-                match ((&mut *output).as_any_mut()).downcast_mut::<File>() {
-                    Some(file) => libcramjam::lz4::compress(input, file, conf.level.map(|v| v as _)),
-                    None => unreachable!("Did we implement something other than Stdout and File for output?"),
+            match conf.action {
+                Action::Compress => {
+                    // TODO: lz4 doesn't impl Read for their Encoder, so cannot determine
+                    // number of bytes compressed without using Seek, which stdout doesn't have,
+                    // as it's streaming. So here, we'll go ahead and read everything in then
+                    // send it in as a cursor, file can remain as is.
+                    // When lz4 implements Reader for the Encoder, then all this can go away.
+                    // along with the `Seek` trait bound on the internal::compress function
+                    if let Some(stdout) = ((&mut *output).as_any_mut()).downcast_mut::<StdoutLock>() {
+                        let mut data = vec![];
+                        libcramjam::lz4::compress(input, &mut Cursor::new(&mut data), conf.level.map(|v| v as _))?;
+                        io::copy(&mut Cursor::new(data), stdout).map(|v| v as usize)
+                    } else {
+                        match ((&mut *output).as_any_mut()).downcast_mut::<File>() {
+                            Some(file) => libcramjam::lz4::compress(input, file, conf.level.map(|v| v as _)),
+                            None => unreachable!("Did we implement something other than Stdout and File for output?"),
+                        }
+                    }
                 }
+                Action::Decompress => libcramjam::lz4::decompress(input, &mut output),
             }
         }
-        Codec::Bzip2(conf) => libcramjam::bzip2::compress(input, &mut output, conf.level.map(|v| v as _)),
-        Codec::Gzip(conf) => libcramjam::gzip::compress(input, &mut output, conf.level.map(|v| v as _)),
-        Codec::ZSTD(conf) => libcramjam::zstd::compress(input, &mut output, conf.level.map(|v| v as _)),
-        Codec::Deflate(conf) => libcramjam::deflate::compress(input, &mut output, conf.level.map(|v| v as _)),
-        Codec::Brotli(conf) => libcramjam::brotli::compress(input, &mut output, conf.level.map(|v| v as _)),
+        Codec::Bzip2(conf) => match conf.action {
+            Action::Compress => libcramjam::bzip2::compress(input, &mut output, conf.level.map(|v| v as _)),
+            Action::Decompress => libcramjam::bzip2::decompress(input, &mut output),
+        },
+        Codec::Gzip(conf) => match conf.action {
+            Action::Compress => libcramjam::gzip::compress(input, &mut output, conf.level.map(|v| v as _)),
+            Action::Decompress => libcramjam::gzip::decompress(input, &mut output),
+        },
+        Codec::ZSTD(conf) => match conf.action {
+            Action::Compress => libcramjam::zstd::compress(input, &mut output, conf.level.map(|v| v as _)),
+            Action::Decompress => libcramjam::zstd::decompress(input, &mut output),
+        },
+        Codec::Deflate(conf) => match conf.action {
+            Action::Compress => libcramjam::deflate::compress(input, &mut output, conf.level.map(|v| v as _)),
+            Action::Decompress => libcramjam::deflate::decompress(input, &mut output),
+        },
+        Codec::Brotli(conf) => match conf.action {
+            Action::Compress => libcramjam::brotli::compress(input, &mut output, conf.level.map(|v| v as _)),
+            Action::Decompress => libcramjam::brotli::decompress(input, &mut output),
+        },
     }?;
     let duration = start.elapsed();
 
     if !m.quiet {
         if let Some(len) = maybe_len {
             println!("Input:      {}", ByteSize(len as _));
             println!("Output:     {}", ByteSize(nbytes as _));
```

### Comparing `cramjam_cli-0.1.0/Cargo.lock` & `cramjam_cli-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "cramjam-cli"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "bytesize",
  "clap",
  "libcramjam",
 ]
 
 [[package]]
```

### Comparing `cramjam_cli-0.1.0/PKG-INFO` & `cramjam_cli-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cramjam-cli
-Version: 0.1.0
-Requires-Dist: pytest >=5.30 ; extra == 'dev'
-Requires-Dist: hypothesis ; extra == 'dev'
+Version: 0.1.1
+Requires-Dist: pytest>=5.30; extra == 'dev'
+Requires-Dist: hypothesis; extra == 'dev'
 Provides-Extra: dev
 Keywords: compression,decompression,snappy,zstd,bz2,gzip,lz4,brotli,deflate
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/milesgranger/pyrus-cramjam
-Project-URL: documentation, https://docs.rs/cramjam/latest/cramjam
 Project-URL: repository, https://github.com/milesgranger/pyrus-cramjam
+Project-URL: documentation, https://docs.rs/cramjam/latest/cramjam
 
 # cramjam-cli
 
 [![CI](https://github.com/milesgranger/pyrus-cramjam/workflows/CI/badge.svg?branch=master)](https://github.com/milesgranger/pyrus-cramjam/actions?query=branch=master)
 [![PyPI](https://img.shields.io/pypi/v/cramjam-cli.svg)](https://pypi.org/project/cramjam-cli)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cramjam-cli/badges/version.svg)](https://anaconda.org/conda-forge/cramjam-cli)
 [![Downloads](https://pepy.tech/badge/cramjam-cli/month)](https://pepy.tech/project/cramjam-cli)
```

