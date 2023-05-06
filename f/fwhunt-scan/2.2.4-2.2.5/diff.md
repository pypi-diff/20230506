# Comparing `tmp/fwhunt_scan-2.2.4.tar.gz` & `tmp/fwhunt_scan-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwhunt_scan-2.2.4.tar", last modified: Fri Mar 31 14:01:52 2023, max compression
+gzip compressed data, was "fwhunt_scan-2.2.5.tar", last modified: Sat May  6 19:49:33 2023, max compression
```

## Comparing `fwhunt_scan-2.2.4.tar` & `fwhunt_scan-2.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-03-31 14:01:52.882723 fwhunt_scan-2.2.4/
--rw-r--r--   0 yv         (501) staff       (20)    35149 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.4/LICENSE
--rw-r--r--   0 yv         (501) staff       (20)     4302 2023-03-31 14:01:52.882764 fwhunt_scan-2.2.4/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)     3728 2023-03-17 22:44:15.000000 fwhunt_scan-2.2.4/README.md
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-03-31 14:01:52.881651 fwhunt_scan-2.2.4/fwhunt_scan/
--rw-r--r--   0 yv         (501) staff       (20)      615 2023-03-31 14:01:07.000000 fwhunt_scan-2.2.4/fwhunt_scan/__init__.py
--rw-r--r--   0 yv         (501) staff       (20)      362 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/__init__.pyi
--rw-r--r--   0 yv         (501) staff       (20)       64 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.4/fwhunt_scan/py.typed
--rw-r--r--   0 yv         (501) staff       (20)      817 2023-02-20 11:45:24.000000 fwhunt_scan-2.2.4/fwhunt_scan/test_internal.py
--rw-r--r--   0 yv         (501) staff       (20)    27550 2022-10-11 01:00:17.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     2686 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_analyzer.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5237 2023-02-20 13:44:10.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_extractor.py
--rw-r--r--   0 yv         (501) staff       (20)   304114 2022-05-30 08:29:58.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_protocols.py
--rw-r--r--   0 yv         (501) staff       (20)      218 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_protocols.pyi
--rw-r--r--   0 yv         (501) staff       (20)    36316 2023-03-06 19:27:41.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_scanner.py
--rw-r--r--   0 yv         (501) staff       (20)     2634 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_scanner.pyi
--rw-r--r--   0 yv         (501) staff       (20)     9985 2022-09-20 15:07:51.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_smm.py
--rw-r--r--   0 yv         (501) staff       (20)     1337 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_smm.pyi
--rw-r--r--   0 yv         (501) staff       (20)     5596 2022-05-30 08:30:06.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_tables.py
--rw-r--r--   0 yv         (501) staff       (20)      280 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_tables.pyi
--rw-r--r--   0 yv         (501) staff       (20)     3035 2022-07-27 15:10:58.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_te.py
--rw-r--r--   0 yv         (501) staff       (20)      727 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_te.pyi
--rw-r--r--   0 yv         (501) staff       (20)     3875 2022-04-13 18:03:37.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_types.py
--rw-r--r--   0 yv         (501) staff       (20)     1596 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_types.pyi
--rw-r--r--   0 yv         (501) staff       (20)     2112 2022-07-15 12:35:57.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_utils.py
--rw-r--r--   0 yv         (501) staff       (20)      418 2023-03-31 14:01:45.000000 fwhunt_scan-2.2.4/fwhunt_scan/uefi_utils.pyi
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-03-31 14:01:52.882388 fwhunt_scan-2.2.4/fwhunt_scan.egg-info/
--rw-r--r--   0 yv         (501) staff       (20)     4302 2023-03-31 14:01:52.000000 fwhunt_scan-2.2.4/fwhunt_scan.egg-info/PKG-INFO
--rw-r--r--   0 yv         (501) staff       (20)      888 2023-03-31 14:01:52.000000 fwhunt_scan-2.2.4/fwhunt_scan.egg-info/SOURCES.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2023-03-31 14:01:52.000000 fwhunt_scan-2.2.4/fwhunt_scan.egg-info/dependency_links.txt
--rw-r--r--   0 yv         (501) staff       (20)        1 2022-05-30 08:58:37.000000 fwhunt_scan-2.2.4/fwhunt_scan.egg-info/not-zip-safe
--rw-r--r--   0 yv         (501) staff       (20)      127 2023-03-31 14:01:52.000000 fwhunt_scan-2.2.4/fwhunt_scan.egg-info/requires.txt
--rw-r--r--   0 yv         (501) staff       (20)       12 2023-03-31 14:01:52.000000 fwhunt_scan-2.2.4/fwhunt_scan.egg-info/top_level.txt
--rw-r--r--   0 yv         (501) staff       (20)     6684 2023-03-17 22:33:11.000000 fwhunt_scan-2.2.4/fwhunt_scan_analyzer.py
--rw-r--r--   0 yv         (501) staff       (20)     3860 2023-03-17 22:40:12.000000 fwhunt_scan-2.2.4/fwhunt_scan_docker.py
--rw-r--r--   0 yv         (501) staff       (20)      116 2023-03-31 14:01:52.882919 fwhunt_scan-2.2.4/setup.cfg
--rw-r--r--   0 yv         (501) staff       (20)     1408 2023-02-20 17:31:56.000000 fwhunt_scan-2.2.4/setup.py
-drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-03-31 14:01:52.882607 fwhunt_scan-2.2.4/test/
--rw-r--r--   0 yv         (501) staff       (20)     1208 2022-05-30 08:09:52.000000 fwhunt_scan-2.2.4/test/test.py
--rw-r--r--   0 yv         (501) staff       (20)      230 2022-08-03 15:21:16.000000 fwhunt_scan-2.2.4/test/test_variants.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.727982 fwhunt_scan-2.2.5/
+-rw-r--r--   0 yv         (501) staff       (20)    35149 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.5/LICENSE
+-rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-06 19:49:33.728029 fwhunt_scan-2.2.5/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)     3728 2023-03-17 22:44:15.000000 fwhunt_scan-2.2.5/README.md
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.726987 fwhunt_scan-2.2.5/fwhunt_scan/
+-rw-r--r--   0 yv         (501) staff       (20)      615 2023-05-06 19:46:06.000000 fwhunt_scan-2.2.5/fwhunt_scan/__init__.py
+-rw-r--r--   0 yv         (501) staff       (20)      362 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/__init__.pyi
+-rw-r--r--   0 yv         (501) staff       (20)       64 2022-04-11 15:38:46.000000 fwhunt_scan-2.2.5/fwhunt_scan/py.typed
+-rw-r--r--   0 yv         (501) staff       (20)      817 2023-02-20 11:45:24.000000 fwhunt_scan-2.2.5/fwhunt_scan/test_internal.py
+-rw-r--r--   0 yv         (501) staff       (20)    27550 2022-10-11 01:00:17.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     2686 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5237 2023-02-20 13:44:10.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_extractor.py
+-rw-r--r--   0 yv         (501) staff       (20)   304114 2022-05-30 08:29:58.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_protocols.py
+-rw-r--r--   0 yv         (501) staff       (20)      218 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_protocols.pyi
+-rw-r--r--   0 yv         (501) staff       (20)    36316 2023-03-06 19:27:41.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.py
+-rw-r--r--   0 yv         (501) staff       (20)     2634 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     9985 2022-09-20 15:07:51.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.py
+-rw-r--r--   0 yv         (501) staff       (20)     1337 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     5596 2022-05-30 08:30:06.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_tables.py
+-rw-r--r--   0 yv         (501) staff       (20)      280 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_tables.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     3035 2022-07-27 15:10:58.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.py
+-rw-r--r--   0 yv         (501) staff       (20)      727 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     3875 2022-04-13 18:03:37.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.py
+-rw-r--r--   0 yv         (501) staff       (20)     1596 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.pyi
+-rw-r--r--   0 yv         (501) staff       (20)     2112 2022-07-15 12:35:57.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_utils.py
+-rw-r--r--   0 yv         (501) staff       (20)      418 2023-05-06 19:49:27.000000 fwhunt_scan-2.2.5/fwhunt_scan/uefi_utils.pyi
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.727662 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/
+-rw-r--r--   0 yv         (501) staff       (20)     4302 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/PKG-INFO
+-rw-r--r--   0 yv         (501) staff       (20)      888 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/SOURCES.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/dependency_links.txt
+-rw-r--r--   0 yv         (501) staff       (20)        1 2022-05-30 08:58:37.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/not-zip-safe
+-rw-r--r--   0 yv         (501) staff       (20)      127 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/requires.txt
+-rw-r--r--   0 yv         (501) staff       (20)       12 2023-05-06 19:49:33.000000 fwhunt_scan-2.2.5/fwhunt_scan.egg-info/top_level.txt
+-rw-r--r--   0 yv         (501) staff       (20)     7250 2023-05-06 19:42:48.000000 fwhunt_scan-2.2.5/fwhunt_scan_analyzer.py
+-rw-r--r--   0 yv         (501) staff       (20)     3860 2023-03-17 22:40:12.000000 fwhunt_scan-2.2.5/fwhunt_scan_docker.py
+-rw-r--r--   0 yv         (501) staff       (20)      116 2023-05-06 19:49:33.728199 fwhunt_scan-2.2.5/setup.cfg
+-rw-r--r--   0 yv         (501) staff       (20)     1408 2023-02-20 17:31:56.000000 fwhunt_scan-2.2.5/setup.py
+drwxr-xr-x   0 yv         (501) staff       (20)        0 2023-05-06 19:49:33.727872 fwhunt_scan-2.2.5/test/
+-rw-r--r--   0 yv         (501) staff       (20)     1208 2022-05-30 08:09:52.000000 fwhunt_scan-2.2.5/test/test.py
+-rw-r--r--   0 yv         (501) staff       (20)      230 2022-08-03 15:21:16.000000 fwhunt_scan-2.2.5/test/test_variants.py
```

### Comparing `fwhunt_scan-2.2.4/LICENSE` & `fwhunt_scan-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/PKG-INFO` & `fwhunt_scan-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwhunt_scan
-Version: 2.2.4
+Version: 2.2.5
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fwhunt_scan-2.2.4/README.md` & `fwhunt_scan-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/__init__.py` & `fwhunt_scan-2.2.5/fwhunt_scan/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 """
 
 __author__ = "FwHunt team"
 __email__ = "fwhunt@binarly.io"
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 
 from .uefi_analyzer import UefiAnalyzer, UefiAnalyzerError
 from .uefi_scanner import UefiRule, UefiScanner, UefiScannerError
 from .uefi_te import TerseExecutableParser
 from .uefi_extractor import UefiBinary, UefiExtractor
 
 __all__ = [
```

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/test_internal.py` & `fwhunt_scan-2.2.5/fwhunt_scan/test_internal.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_analyzer.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_analyzer.pyi` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_analyzer.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_extractor.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_extractor.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_protocols.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_protocols.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_scanner.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_scanner.pyi` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_scanner.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_smm.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_smm.pyi` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_smm.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_tables.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_tables.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_te.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_te.pyi` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_te.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_types.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_types.pyi` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_types.pyi`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan/uefi_utils.py` & `fwhunt_scan-2.2.5/fwhunt_scan/uefi_utils.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan.egg-info/PKG-INFO` & `fwhunt_scan-2.2.5/fwhunt_scan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwhunt-scan
-Version: 2.2.4
+Version: 2.2.5
 Summary: Tools for analyzing UEFI firmware and checking UEFI modules with FwHunt rules
 Home-page: https://github.com/binarly-io/fwhunt-scan
 Author: FwHunt team
 Author-email: fwhunt@binarly.io
 License: GPL-3.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan.egg-info/SOURCES.txt` & `fwhunt_scan-2.2.5/fwhunt_scan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan_analyzer.py` & `fwhunt_scan-2.2.5/fwhunt_scan_analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,23 +111,42 @@
     else:
         rules += list(map(str, pathlib.Path(rules_dir).rglob("*.yml")))
 
     if not os.path.isfile(image_path):
         print(f"{error_prefix} check image path")
         return False
 
+    prefix = click.style("Scanner result", fg="green")
+    no_threat = click.style("No threat detected", fg="green")
+    threat = click.style(
+        "FwHunt rule has been triggered and threat detected!", fg="red"
+    )
+
     # on linux platforms you can pass blob via shm://
     # uefi_analyzer = UefiAnalyzer(blob=data)
 
     uefi_rules: List[UefiRule] = list()
 
     for r in rules:
         with open(r, "r") as f:
             uefi_rules.append(UefiRule(rule_content=f.read()))
 
+    # Select the rules with `target: firmware`
+    uefi_rules_fw: List[UefiRule] = list(
+        filter(lambda rule: rule.target == "firmware", uefi_rules)
+    )
+    if len(uefi_rules_fw):
+        with UefiAnalyzer(image_path=image_path) as uefi_analyzer_fw:
+            scanner_fw = UefiScanner(uefi_analyzer_fw, uefi_rules_fw)
+            for result in scanner_fw.results:
+                msg = threat if result.res else no_threat
+                print(
+                    f"{prefix} {result.rule.name} (variant: {result.variant_label}) {msg}"
+                )
+
     # Group rules by guids
     rules_guids: Dict[str, List[UefiRule]] = dict()
     for uefi_rule in uefi_rules:
         if uefi_rule.volume_guids is None:
             print(f"[I] Specify volume_guids in {uefi_rule.name} or use scan command")
             continue
         for guid in [g.lower() for g in uefi_rule.volume_guids]:
@@ -141,20 +160,14 @@
             f"{error_prefix} None of the rules specify volume_guids (use scan command)"
         )
         return False
 
     with open(image_path, "rb") as f:
         firmware_data = f.read()
 
-    prefix = click.style("Scanner result", fg="green")
-    no_threat = click.style("No threat detected", fg="green")
-    threat = click.style(
-        "FwHunt rule has been triggered and threat detected!", fg="red"
-    )
-
     extractor = UefiExtractor(firmware_data, list(rules_guids.keys()))
     extractor.extract_all(ignore_guid=False)
 
     if not len(extractor.binaries):
         print("No modules were found for scanning")
         return False
```

### Comparing `fwhunt_scan-2.2.4/fwhunt_scan_docker.py` & `fwhunt_scan-2.2.5/fwhunt_scan_docker.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/setup.py` & `fwhunt_scan-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `fwhunt_scan-2.2.4/test/test.py` & `fwhunt_scan-2.2.5/test/test.py`

 * *Files identical despite different names*

