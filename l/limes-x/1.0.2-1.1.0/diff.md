# Comparing `tmp/limes_x-1.0.2-py3-none-any.whl.zip` & `tmp/limes_x-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,28 @@
-Zip file size: 35742 bytes, number of entries: 21
--rw-rw-r--  2.0 unx      220 b- defN 23-Apr-19 01:42 limes_x/__init__.py
--rw-rw-r--  2.0 unx       69 b- defN 23-Apr-19 01:42 limes_x/constants.py
+Zip file size: 40946 bytes, number of entries: 26
+-rw-rw-r--  2.0 unx      243 b- defN 23-May-05 17:54 limes_x/__init__.py
+-rw-rw-r--  2.0 unx       61 b- defN 23-May-05 17:54 limes_x/__main__.py
+-rw-rw-r--  2.0 unx     2931 b- defN 23-May-05 23:53 limes_x/cli.py
 -rw-rw-r--  2.0 unx     2864 b- defN 23-Apr-19 01:42 limes_x/telemetry.py
--rw-rw-r--  2.0 unx    38931 b- defN 23-Apr-30 09:08 limes_x/workflow.py
+-rw-rw-r--  2.0 unx        5 b- defN 23-May-05 17:42 limes_x/version.txt
+-rw-rw-r--  2.0 unx    38900 b- defN 23-May-06 05:54 limes_x/workflow.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/common/__init__.py
 -rw-rw-r--  2.0 unx     8098 b- defN 23-Apr-19 01:42 limes_x/common/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/environments/__init__.py
 -rw-rw-r--  2.0 unx     1202 b- defN 23-Apr-19 01:42 limes_x/environments/_setup.py
 -rw-rw-r--  2.0 unx     6151 b- defN 23-May-01 01:12 limes_x/environments/hpc.py
 -rw-rw-r--  2.0 unx     3654 b- defN 23-Apr-19 01:42 limes_x/environments/local.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/execution/__init__.py
 -rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-19 01:42 limes_x/execution/comms.py
 -rw-rw-r--  2.0 unx     9506 b- defN 23-Apr-29 08:02 limes_x/execution/executors.py
 -rw-rw-r--  2.0 unx     5105 b- defN 23-Apr-19 01:42 limes_x/execution/instances.py
 -rw-rw-r--  2.0 unx    14052 b- defN 23-Apr-19 01:42 limes_x/execution/modules.py
 -rw-rw-r--  2.0 unx     4419 b- defN 23-Apr-19 01:42 limes_x/execution/solver.py
 -rw-rw-r--  2.0 unx      677 b- defN 23-Apr-19 01:42 limes_x/execution/template_module_definition.py
--rw-rw-r--  2.0 unx     9991 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1717 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/RECORD
-21 files, 109570 bytes uncompressed, 32944 bytes compressed:  69.9%
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-05 23:55 limes_x/presets/__init__.py
+-rw-rw-r--  2.0 unx     9137 b- defN 23-May-06 07:00 limes_x/presets/slurm.py
+-rw-rw-r--  2.0 unx     9991 b- defN 23-May-06 07:57 limes_x-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-06 07:57 limes_x-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       36 b- defN 23-May-06 07:57 limes_x-1.1.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-06 07:57 limes_x-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2117 b- defN 23-May-06 07:57 limes_x-1.1.0.dist-info/RECORD
+26 files, 122063 bytes uncompressed, 37522 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
 Filename: limes_x/__init__.py
 Comment: 
 
-Filename: limes_x/constants.py
+Filename: limes_x/__main__.py
+Comment: 
+
+Filename: limes_x/cli.py
 Comment: 
 
 Filename: limes_x/telemetry.py
 Comment: 
 
+Filename: limes_x/version.txt
+Comment: 
+
 Filename: limes_x/workflow.py
 Comment: 
 
 Filename: limes_x/common/__init__.py
 Comment: 
 
 Filename: limes_x/common/utils.py
@@ -45,20 +51,29 @@
 
 Filename: limes_x/execution/solver.py
 Comment: 
 
 Filename: limes_x/execution/template_module_definition.py
 Comment: 
 
-Filename: limes_x-1.0.2.dist-info/METADATA
+Filename: limes_x/presets/__init__.py
+Comment: 
+
+Filename: limes_x/presets/slurm.py
+Comment: 
+
+Filename: limes_x-1.1.0.dist-info/METADATA
+Comment: 
+
+Filename: limes_x-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: limes_x-1.0.2.dist-info/WHEEL
+Filename: limes_x-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: limes_x-1.0.2.dist-info/top_level.txt
+Filename: limes_x-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: limes_x-1.0.2.dist-info/RECORD
+Filename: limes_x-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## limes_x/__init__.py

```diff
@@ -1,3 +1,5 @@
 from .workflow import Workflow, InputGroup
 from .execution.modules import ModuleBuilder, ComputeModule, Item, JobContext, JobResult, Params, LoadComputeModules
 from .execution.executors import Job, Executor, HpcExecutor
+from .cli import main
+
```

## limes_x/workflow.py

```diff
@@ -755,15 +755,15 @@
         given: list[InputGroup],
         executor: Executor, params: Params=Params(),
         regenerate: Literal["failures"]|list[Item]=list(),
         max_concurrent: int = 256,
         max_per_module: dict[str, int] = dict(),
         _catch_errors: bool = True,
     ):
-        if isinstance(workspace, str): workspace = Path(os.path.abspath(workspace))
+        workspace = Path(os.path.abspath(workspace))
         if not workspace.exists():
             os.makedirs(workspace)
         params.reference_folder = self._reference_folder
 
         # abs. path before change to working dir
         sys.path = [os.path.abspath(p) for p in sys.path]
```

## Comparing `limes_x-1.0.2.dist-info/METADATA` & `limes_x-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limes-x
-Version: 1.0.2
+Version: 1.1.0
 Summary: declarative workflow automation
 Home-page: https://github.com/hallamlab/limes-x
 Author: Tony Liu
 Author-email: contacttonyliu@gmail.com
 Project-URL: Bug Tracker, https://github.com/hallamlab/limes-x/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `limes_x-1.0.2.dist-info/RECORD` & `limes_x-1.1.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-limes_x/__init__.py,sha256=WGf2TVIdLqa_d5xBlV5_ihUhZIM0Yhx_OakdgeOvqik,220
-limes_x/constants.py,sha256=yugKKsslkE48FwDWtzqkZ8EUK4XLX_NEh9cccmm_1IM,69
+limes_x/__init__.py,sha256=_AEbnQ0P9TPziUyt0ooift9JLVKTTfUuoCXfid4ahbI,243
+limes_x/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
+limes_x/cli.py,sha256=58IhGatrv17FoFRVv4yWbgTCDsIOAFs-o2O3ZsyAhqQ,2931
 limes_x/telemetry.py,sha256=6hUE1nxxKkPUGUNq0KlIbHQqa3pSqA0zZSjb57Wyngc,2864
-limes_x/workflow.py,sha256=taAErdX4P017ay4y8CJoeg9f43okaXjtlpSVpbnMBPU,38931
+limes_x/version.txt,sha256=f70hDr7BH2WpcZDvkAeVxLjaOAWvP1objR0nJVaykso,5
+limes_x/workflow.py,sha256=URbhxF2FmX-WG9pSgdkx2oiBaUATf2DAtuJ60HXHfp0,38900
 limes_x/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/common/utils.py,sha256=83ayvyp9oieN9CFF9VNxjQQwK06EWzqXKaLDjhGqC_c,8098
 limes_x/environments/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/environments/_setup.py,sha256=rI9gTVt2VMXfeAsuxkTx3ucBp5kd_K-Z6xbJqybzEvg,1202
 limes_x/environments/hpc.py,sha256=vNbqopLFFrk8AXfKeLgPNlgRPEl-fQMxFNLi-sJBR44,6151
 limes_x/environments/local.py,sha256=MF_-1XB4hiFUI9_0fhXCRrMshFSlc5hyO1rG1B35kik,3654
 limes_x/execution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/execution/comms.py,sha256=Yx_cIyvzuA7h_iKU4R3fyd1LvsKZzZx-NsVZh_MXHE4,2814
 limes_x/execution/executors.py,sha256=XQDQdbrahymtWE7xVqRMUudg-lu-lCcv2_yZSbSiE_I,9506
 limes_x/execution/instances.py,sha256=lT32W3nNSOrfovSNEl7ARY8Yt4SkhkA-1NjWUhBvOds,5105
 limes_x/execution/modules.py,sha256=AIEY-xyIDUhrQvw7qxJChTwXNTEtydKjrxHZCd4woWs,14052
 limes_x/execution/solver.py,sha256=y9XNSlZscAHxizN57PZTMphHw1PVWjFnEfHyrGN7SFU,4419
 limes_x/execution/template_module_definition.py,sha256=RxW4KsU1-iEScq_Y5GIafSfeXnQQeYGYr9FC9AZ8-VQ,677
-limes_x-1.0.2.dist-info/METADATA,sha256=1dM-4hli2KX_-9iXYqBEMte70A6eg4B5mQoB6365ON8,9991
-limes_x-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-limes_x-1.0.2.dist-info/top_level.txt,sha256=r9RGajCrNNSpim7JI2bx3UHGzgXw2vRLTNuxMRwPRNQ,8
-limes_x-1.0.2.dist-info/RECORD,,
+limes_x/presets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+limes_x/presets/slurm.py,sha256=HOeJ3n-3nujLmtkK8J-Rl15YbwErayoFLJw3OQDhe9E,9137
+limes_x-1.1.0.dist-info/METADATA,sha256=dE-wz50roGPUduEMY2l3Qlb0S3MfPJ8YxL5gjUQ9eKY,9991
+limes_x-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+limes_x-1.1.0.dist-info/entry_points.txt,sha256=P1UpWZ-q8GvFystMaHOUTH8844VaNMAOs1MX_R_KJXE,36
+limes_x-1.1.0.dist-info/top_level.txt,sha256=r9RGajCrNNSpim7JI2bx3UHGzgXw2vRLTNuxMRwPRNQ,8
+limes_x-1.1.0.dist-info/RECORD,,
```

