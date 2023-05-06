# Comparing `tmp/hyfi_template-0.3.1.tar.gz` & `tmp/hyfi_template-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.3.1.tar", max compression
+gzip compressed data, was "hyfi_template-0.3.2.tar", max compression
```

## Comparing `hyfi_template-0.3.1.tar` & `hyfi_template-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-05-06 20:39:16.905157 hyfi_template-0.3.1/LICENSE
--rw-r--r--   0        0        0     2001 2023-05-06 20:39:16.905157 hyfi_template-0.3.1/README.md
--rw-r--r--   0        0        0     3082 2023-05-06 20:39:44.877013 hyfi_template-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      294 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      379 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       22 2023-05-06 20:39:44.825013 hyfi_template-0.3.1/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      257 2023-05-06 20:39:44.825013 hyfi_template-0.3.1/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/copier/conf.yaml
--rw-r--r--   0        0        0      807 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0        0 2023-05-06 20:39:16.909157 hyfi_template-0.3.1/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 hyfi_template-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 20:41:50.600479 hyfi_template-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2001 2023-05-06 20:41:50.600479 hyfi_template-0.3.2/README.md
+-rw-r--r--   0        0        0     3082 2023-05-06 20:42:15.604867 hyfi_template-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      379 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-06 20:42:15.548866 hyfi_template-0.3.2/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-06 20:42:15.548866 hyfi_template-0.3.2/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      807 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-05-06 20:41:50.604479 hyfi_template-0.3.2/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 hyfi_template-0.3.2/PKG-INFO
```

### Comparing `hyfi_template-0.3.1/LICENSE` & `hyfi_template-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/README.md` & `hyfi_template-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/pyproject.toml` & `hyfi_template-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.3.1"
+version = "0.3.2"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
```

### Comparing `hyfi_template-0.3.1/src/hyfi_template/conf/copier/conf.yaml` & `hyfi_template-0.3.2/src/hyfi_template/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/src/hyfi_template/conf/dotenv/__init__.yaml` & `hyfi_template-0.3.2/src/hyfi_template/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.3.2/src/hyfi_template/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.3.2/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/src/hyfi_template/conf/path/__default__.yaml` & `hyfi_template-0.3.2/src/hyfi_template/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/src/hyfi_template/conf/path/__init__.yaml` & `hyfi_template-0.3.2/src/hyfi_template/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.1/PKG-INFO` & `hyfi_template-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.3.1
+Version: 0.3.2
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

