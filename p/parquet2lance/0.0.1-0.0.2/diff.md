# Comparing `tmp/parquet2lance-0.0.1.tar.gz` & `tmp/parquet2lance-0.0.2.tar.gz`

## Comparing `parquet2lance-0.0.1.tar` & `parquet2lance-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/Cargo.toml
--rw-r--r--   0      503       20    88932 2023-05-06 09:14:46.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/Cargo.lock
--rw-r--r--   0      503       20     1064 2023-05-06 09:51:06.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/LICENSE
--rw-r--r--   0      503       20     1688 2023-05-06 09:54:28.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/README.md
--rw-r--r--   0      503       20     1513 2023-05-05 09:28:08.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/fs.rs
--rw-r--r--   0      503       20     3391 2023-05-05 09:33:32.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/gcs.rs
--rw-r--r--   0      503       20     1060 2023-05-05 10:03:50.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/reader.rs
--rw-r--r--   0      503       20     3908 2023-05-06 06:36:50.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/util.rs
--rw-r--r--   0      503       20     1081 2023-05-06 09:00:32.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io.rs
--rw-r--r--   0      503       20       44 2023-05-06 08:43:19.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/src/lib.rs
--rw-r--r--   0      503       20      698 2023-05-06 08:36:36.000000 parquet2lance-0.0.1/local_dependencies/parquet2lance/src/main.rs
--rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 parquet2lance-0.0.1/Cargo.toml
--rw-r--r--   0      503       20     1064 2023-05-06 09:51:20.000000 parquet2lance-0.0.1/LICENSE
--rw-r--r--   0      503       20       87 2023-05-06 09:51:57.000000 parquet2lance-0.0.1/README.md
--rw-r--r--   0      503       20      668 2023-05-06 10:02:04.000000 parquet2lance-0.0.1/pyproject.toml
--rw-r--r--   0      503       20      530 2023-05-06 09:09:08.000000 parquet2lance-0.0.1/src/lib.rs
--rw-r--r--   0      503       20    95728 2023-05-06 09:56:59.000000 parquet2lance-0.0.1/Cargo.lock
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 parquet2lance-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/Cargo.toml
+-rw-r--r--   0      503       20    88932 2023-05-06 09:14:46.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/Cargo.lock
+-rw-r--r--   0      503       20     1064 2023-05-06 09:51:06.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/LICENSE
+-rw-r--r--   0      503       20     1536 2023-05-06 10:10:19.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/README.md
+-rw-r--r--   0      503       20     1513 2023-05-05 09:28:08.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/fs.rs
+-rw-r--r--   0      503       20     3391 2023-05-05 09:33:32.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/gcs.rs
+-rw-r--r--   0      503       20     1060 2023-05-05 10:03:50.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/reader.rs
+-rw-r--r--   0      503       20     3908 2023-05-06 06:36:50.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/util.rs
+-rw-r--r--   0      503       20     1081 2023-05-06 09:00:32.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io.rs
+-rw-r--r--   0      503       20       44 2023-05-06 08:43:19.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/src/lib.rs
+-rw-r--r--   0      503       20      698 2023-05-06 08:36:36.000000 parquet2lance-0.0.2/local_dependencies/parquet2lance/src/main.rs
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 parquet2lance-0.0.2/Cargo.toml
+-rw-r--r--   0      503       20     1064 2023-05-06 09:51:20.000000 parquet2lance-0.0.2/LICENSE
+-rw-r--r--   0      503       20       87 2023-05-06 09:51:57.000000 parquet2lance-0.0.2/README.md
+-rw-r--r--   0      503       20      668 2023-05-06 10:07:52.000000 parquet2lance-0.0.2/pyproject.toml
+-rw-r--r--   0      503       20      562 2023-05-06 10:15:09.000000 parquet2lance-0.0.2/src/lib.rs
+-rw-r--r--   0      503       20    95728 2023-05-06 10:16:12.000000 parquet2lance-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 parquet2lance-0.0.2/PKG-INFO
```

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/Cargo.toml` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/Cargo.toml`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/Cargo.lock` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/Cargo.lock`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/LICENSE` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/LICENSE`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/README.md` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
+
 ## parquet2lance
 
 [CI]: https://github.com/haoxins/parquet2lance/actions/workflows/rust.yaml
 [CI Badge]: https://github.com/haoxins/parquet2lance/actions/workflows/rust.yaml/badge.svg
-[crates.io]: https://crates.io/crates/parquet2lance
-[crates.io badge]: https://img.shields.io/crates/v/parquet2lance.svg
 
 [![CI Badge]][CI]
-[![crates.io badge]][crates.io]
 
 - Convert parquet files to [lance](https://github.com/eto-ai/lance)
 
 ```zsh
 $ cargo install parquet2lance
 $ parquet2lance --help
 ```
```

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/fs.rs` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/fs.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/gcs.rs` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/gcs.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/reader.rs` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/reader.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io/util.rs` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io/util.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/src/io.rs` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/src/io.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/local_dependencies/parquet2lance/src/main.rs` & `parquet2lance-0.0.2/local_dependencies/parquet2lance/src/main.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/LICENSE` & `parquet2lance-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/pyproject.toml` & `parquet2lance-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.0.1/src/lib.rs` & `parquet2lance-0.0.2/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,12 @@
         let reader = Reader::new(&PathBuf::from(input), true).await;
         _p2l(reader, &PathBuf::from(output), true).await;
     });
     Ok(())
 }
 
 #[pymodule]
+#[pyo3(name = "parquet2lance")]
 fn python(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(p2l, m)?)?;
     Ok(())
 }
```

### Comparing `parquet2lance-0.0.1/Cargo.lock` & `parquet2lance-0.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2256,15 +2256,15 @@
 name = "outref"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4030760ffd992bef45b0ae3f10ce1aba99e33464c90d14dd7c039884963ddc7a"
 
 [[package]]
 name = "p2l"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "parquet2lance",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
```

### Comparing `parquet2lance-0.0.1/PKG-INFO` & `parquet2lance-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parquet2lance
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: The Python wrapper for the Rust parquet2lance
 Keywords: arrow,lance,parquet
 Author-email: Hao Xin <haoxinst@gmail.com>
```

