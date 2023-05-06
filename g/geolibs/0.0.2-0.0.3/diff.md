# Comparing `tmp/geolibs-0.0.2.tar.gz` & `tmp/geolibs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolibs-0.0.2.tar", max compression
+gzip compressed data, was "geolibs-0.0.3.tar", max compression
```

## Comparing `geolibs-0.0.2.tar` & `geolibs-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      528 2023-05-04 20:41:51.294192 geolibs-0.0.2/README.rst
--rwxr-xr-x   0        0        0      465 2023-05-04 20:42:02.507036 geolibs-0.0.2/geolibs/__init__.py
--rwxr-xr-x   0        0        0     5514 2023-05-04 20:24:29.362348 geolibs-0.0.2/geolibs/engine_cocoext.py
--rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.2/geolibs/engine_cocometric.py
--rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.2/geolibs/enginelogger_hook.py
--rwxr-xr-x   0        0        0    12295 2023-05-04 20:24:29.371193 geolibs-0.0.2/geolibs/loading.py
--rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.2/geolibs/misc.py
--rwxr-xr-x   0        0        0     1066 2023-05-04 20:42:02.499532 geolibs-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 geolibs-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      528 2023-05-04 20:41:51.294192 geolibs-0.0.3/README.rst
+-rwxr-xr-x   0        0        0      465 2023-05-06 20:54:28.831474 geolibs-0.0.3/geolibs/__init__.py
+-rwxr-xr-x   0        0        0     5514 2023-05-06 20:36:53.288107 geolibs-0.0.3/geolibs/engine_cocoext.py
+-rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.3/geolibs/engine_cocometric.py
+-rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.3/geolibs/enginelogger_hook.py
+-rwxr-xr-x   0        0        0    12304 2023-05-06 20:53:44.332058 geolibs-0.0.3/geolibs/loading.py
+-rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.3/geolibs/misc.py
+-rwxr-xr-x   0        0        0     1066 2023-05-06 20:54:28.826392 geolibs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 geolibs-0.0.3/PKG-INFO
```

### Comparing `geolibs-0.0.2/README.rst` & `geolibs-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.2/geolibs/engine_cocoext.py` & `geolibs-0.0.3/geolibs/engine_cocoext.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.2/geolibs/engine_cocometric.py` & `geolibs-0.0.3/geolibs/engine_cocometric.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.2/geolibs/enginelogger_hook.py` & `geolibs-0.0.3/geolibs/enginelogger_hook.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.2/geolibs/loading.py` & `geolibs-0.0.3/geolibs/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,16 +129,16 @@
         except Exception as e:
             if self.ignore_empty:
                 return None
             else:
                 raise e
 
         results["img"] = bands
-        results["img_shape"] = bands.shape
-        results["ori_shape"] = bands.shape
+        results["img_shape"] = bands.shape[:2]
+        results["ori_shape"] = bands.shape[:2]
         results["img_meta"] = metadata
 
         num_channels = 1 if len(bands.shape) < 3 else bands.shape[2]
 
         results['img_norm_cfg'] = dict(
                 mean=np.zeros(num_channels, dtype=np.float32),
                 std=np.ones(num_channels, dtype=np.float32),
@@ -307,14 +307,15 @@
             label = annotation['bbox_label'] + 1
             gt_semantic_seg = cv2.fillPoly(gt_semantic_seg, pts=[pts], color=label)
         if self.reduce_zero_label:
             # avoid using underflow conversion
             gt_semantic_seg[gt_semantic_seg == 0] = 255
             gt_semantic_seg = gt_semantic_seg - 1
             gt_semantic_seg[gt_semantic_seg == 254] = 255
+
         results['gt_seg_map'] = gt_semantic_seg
         results['seg_fields'].append('gt_seg_map')
 
     def __repr__(self) -> str:
         repr_str = self.__class__.__name__
         repr_str += f'(reduce_zero_label={self.reduce_zero_label}, '
         repr_str += f"imdecode_backend='{self.imdecode_backend}', "
```

### Comparing `geolibs-0.0.2/geolibs/misc.py` & `geolibs-0.0.3/geolibs/misc.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.2/pyproject.toml` & `geolibs-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geolibs"
-version = "v0.0.2"
+version = "v0.0.3"
 description = "A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development."
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "geolibs"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `geolibs-0.0.2/PKG-INFO` & `geolibs-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolibs
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development.
 Home-page: https://github.com/granularai/geolibs
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

