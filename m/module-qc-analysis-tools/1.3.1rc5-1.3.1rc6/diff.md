# Comparing `tmp/module_qc_analysis_tools-1.3.1rc5.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc6.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc5.tar` & `module_qc_analysis_tools-1.3.1rc6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
--rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
--rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/TUNING.py
--rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/info_schema.json
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
--rw-r--r--   0        0        0    25563 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    34961 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/LICENSE
--rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/README.md
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/pyproject.toml
--rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc5/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    26971 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    35037 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/LICENSE
+-rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/README.md
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/pyproject.toml
+-rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc6/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/tbump.toml` & `module_qc_analysis_tools-1.3.1rc6/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3522 0a0a  t = "1.3.1rc5"..
+00000010: 7420 3d20 2231 2e33 2e31 7263 3622 0a0a  t = "1.3.1rc6"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e31 7263 3520 e286 9220 7b6e 6577  .3.1rc5 ... {new
+00000150: 2e33 2e31 7263 3620 e286 9220 7b6e 6577  .3.1rc6 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,22 +69,14 @@
 
     log.info("")
     log.info(" ===============================================")
     log.info(" \tPerforming ADC calibration analysis")
     log.info(" ===============================================")
     log.info("")
 
-    if submit and site == "":
-        log.error(
-            bcolors.ERROR
-            + "You have supplied the --submit option without specifying --site (testing site). Please specify your testing site if you would like to submit these results"
-            + bcolors.ENDC
-        )
-        return
-
     allinputs = get_inputs(input_meas)
     qc_config = get_qc_config(qc_criteria_path, test_type)
 
     alloutput = []
     timestamps = []
     for filename in sorted(allinputs):
         log.info("")
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/LP_MODE.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/LP_MODE.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,17 @@
             results.update({"LP_VINA": calculated_data["VinA"]["Values"][0]})
             results.update({"LP_VIND": calculated_data["VinD"]["Values"][0]})
             results.update({"LP_VOFFS": calculated_data["Vofs"]["Values"][0]})
             results.update({"LP_IINA": calculated_data["IinA"]["Values"][0]})
             results.update({"LP_IIND": calculated_data["IinD"]["Values"][0]})
             results.update({"LP_ISHUNTA": calculated_data["IshuntA"]["Values"][0]})
             results.update({"LP_ISHUNTD": calculated_data["IshuntD"]["Values"][0]})
+            results.update(
+                {"LP_DIGITAL_FAIL": int(calculated_data["FailingPixels"]["Values"][0])}
+            )
 
             # Perform QC analysis
             chiplog = logging.FileHandler(f"{output_dir}/{chipname}.log")
             log.addHandler(chiplog)
             passes_qc, summary = perform_qc_analysis(
                 test_type, qc_config, layer, results
             )
@@ -231,14 +234,17 @@
             )
             data.add_parameter(
                 "LP_ISHUNTA", round(calculated_data["IshuntA"]["Values"][0], 4)
             )
             data.add_parameter(
                 "LP_ISHUNTD", round(calculated_data["IshuntD"]["Values"][0], 4)
             )
+            data.add_parameter(
+                "LP_DIGITAL_FAIL", int(calculated_data["FailingPixels"]["Values"][0])
+            )
 
             outputDF.set_results(data)
             outputDF.set_pass_flag(passes_qc)
             if submit:
                 submit_results(
                     outputDF.to_dict(True),
                     time_start,
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,15 @@
             outputDF.set_pass_flag(passes_qc)
             if submit:
                 submit_results(
                     outputDF.to_dict(True),
                     time_start,
                     institution,
                     output_dir.joinpath("submit.txt"),
+                    layer,
                 )
             if permodule:
                 alloutput += [outputDF.to_dict(True)]
                 timestamps += [meas_timestamp]
             else:
                 outfile = output_dir.joinpath(f"{chipname}.json")
                 log.info(f" Saving output of analysis to: {outfile}")
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/TUNING.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/load_yarr_scans.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/load_yarr_scans.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'OVERVOLTAGE_PROTECTION'": "{'OVP_VINA': {'LZero': [1.9, 2.1], 'LOne': [1.9, 2.1], 'LTwo': [1.9, "*

 * *                             "2.1]}, 'OVP_VIND': {'LZero': [1.9, 2.1], 'LOne': [1.9, 2.1], 'LTwo': "*

 * *                             "[1.9, 2.1]}, 'OVP_IINA': {'LZero': [0.636, 0.781], 'LOne': [0.636, "*

 * *                             "0.781], 'LTwo': [0.636, 0.781]}, 'OVP_IIND': {'LZero': [0.855, "*

 * *                             "1.045], 'LOne': [0.855, 1.045], 'LTwo': [0.855, 1.045]}}"}*

```diff
@@ -245,66 +245,66 @@
             0,
             1536
         ]
     },
     "OVERVOLTAGE_PROTECTION": {
         "OVP_IINA": {
             "LOne": [
-                0.681,
-                0.735
+                0.636,
+                0.781
             ],
             "LTwo": [
-                0.567,
-                0.626
+                0.636,
+                0.781
             ],
             "LZero": [
-                0.788,
-                0.85
+                0.636,
+                0.781
             ]
         },
         "OVP_IIND": {
             "LOne": [
-                0.917,
-                0.971
+                0.855,
+                1.045
             ],
             "LTwo": [
-                0.846,
-                0.905
+                0.855,
+                1.045
             ],
             "LZero": [
-                1.177,
-                1.24
+                0.855,
+                1.045
             ]
         },
         "OVP_VINA": {
             "LOne": [
-                1.469,
-                1.519
+                1.9,
+                2.1
             ],
             "LTwo": [
-                1.468,
-                1.518
+                1.9,
+                2.1
             ],
             "LZero": [
-                1.473,
-                1.523
+                1.9,
+                2.1
             ]
         },
         "OVP_VIND": {
             "LOne": [
-                1.469,
-                1.519
+                1.9,
+                2.1
             ],
             "LTwo": [
-                1.468,
-                1.518
+                1.9,
+                2.1
             ],
             "LZero": [
-                1.473,
-                1.523
+                1.9,
+                2.1
             ]
         },
         "OVP_VREFOVP": [
             1.95,
             2.05
         ]
     },
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/info_schema.json` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/info_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -505,14 +505,43 @@
 	&entry.346685867={outputDF.get('passed')}\
 	&entry.2076657244={analysis_version}\
 	&entry.2143111336={meas_version}\
 	&entry.1736672890={layer}\
 	&entry.104853658={outputDF.get('serialNumber')}\
 	&entry.802167553={site}\
 	&entry.1714546984={results.get('INJ_CAPACITANCE')}",
+        "LP_MODE": f"https://docs.google.com/forms/d/e/1FAIpQLSdVBudYiVFG9ts_0y6bQ4xhGJ-mIJNM-N1Hcs7jgPhiYVNAwA/formResponse?usp=pp_url\
+	&entry.1920584355={timestamp}\
+	&entry.104853658={outputDF.get('serialNumber')}\
+	&entry.1282466276={outputDF.get('passed')}\
+	&entry.141409196={analysis_version}\
+	&entry.1579707472={meas_version}\
+	&entry.913205750={layer}\
+	&entry.802167553={site}\
+	&entry.1592726943={results.get('LP_VINA')}\
+	&entry.422835427={results.get('LP_VIND')}\
+	&entry.1218296463={results.get('LP_VOFFS')}\
+	&entry.1682731027={results.get('LP_IINA')}\
+	&entry.784021623={results.get('LP_IIND')}\
+	&entry.1188204940={results.get('LP_ISHUNTA')}\
+	&entry.1456818826={results.get('LP_ISHUNTD')}\
+        &entry.1355617557={results.get('LP_DIGITAL_FAIL')}",
+        "OVERVOLTAGE_PROTECTION": f"https://docs.google.com/forms/d/e/1FAIpQLSc0lwqev5Yyozmnn3gkdnTOoH9BbSdjOuL7CAbhQOZ2rTJINg/formResponse?usp=pp_url\
+	&entry.1920584355={timestamp}\
+	&entry.104853658={outputDF.get('serialNumber')}\
+	&entry.1282466276={outputDF.get('passed')}\
+	&entry.141409196={analysis_version}\
+	&entry.1579707472={meas_version}\
+	&entry.913205750={layer}\
+	&entry.802167553={site}\
+	&entry.1592726943={results.get('OVP_VINA')}\
+	&entry.422835427={results.get('OVP_VIND')}\
+	&entry.1218296463={results.get('OVP_VREFOVP')}\
+	&entry.1682731027={results.get('OVP_IINA')}\
+	&entry.784021623={results.get('OVP_IIND')}",
         "SLDO": f"https://docs.google.com/forms/d/e/1FAIpQLSf3NC84OaYYjJ-DgQ29RvMV2dDQnUI0nxBFdnCUVMby7RXOFQ/formResponse?usp=pp_url\
 	&entry.910646842={outputDF.get('serialNumber')}\
 	&entry.1225658339={outputDF.get('passed')}\
 	&entry.2052956027={analysis_version}\
 	&entry.314862968={meas_version}\
 	&entry.137143573={layer}\
 	&entry.507508481={site}\
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/classification.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/classification.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc6/src/module_qc_analysis_tools/utils/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,15 @@
                     "Imux28",
                     "Imux30",
                     "Imux63",
                 ],
             },
             "LP_MODE": {
                 "required_keys": [
+                    "FailingPixels",
                     "Temperature",
                     "Current",
                     "Vmux30",
                     "Vmux33",
                     "Vmux36",
                     "Vmux37",
                     "Imux0",
@@ -302,15 +303,15 @@
                 )
                 raise LengthMismatchError()
 
     def check_positive_values(self) -> None:
         """Check whether the contents of measurements are valid, i.e. all positive."""
         for required_keyword in self.required_keywords:
             # Allow for negative temperatures
-            if required_keyword == "Temperature":
+            if required_keyword == "Temperature" or required_keyword == "FailingPixels":
                 continue
             if ((self.qcdataframe[required_keyword]) < 0).sum() > 0:
                 log.error(
                     bcolors.ERROR
                     + f"Negative measurements observed in {required_keyword}"
                     + bcolors.ENDC
                 )
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/.gitignore` & `module_qc_analysis_tools-1.3.1rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/LICENSE` & `module_qc_analysis_tools-1.3.1rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/README.md` & `module_qc_analysis_tools-1.3.1rc6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.1rc5
+# module-qc-analysis-tools v1.3.1rc6
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -69,15 +69,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc5
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc6
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

### Comparing `module_qc_analysis_tools-1.3.1rc5/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc5/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc5
+Version: 1.3.1rc6
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,15 +34,15 @@
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: module-qc-data-tools>=1.0.6
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc5
+# module-qc-analysis-tools v1.3.1rc6
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -109,15 +109,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc5
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc6
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

