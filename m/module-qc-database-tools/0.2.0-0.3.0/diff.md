# Comparing `tmp/module_qc_database_tools-0.2.0.tar.gz` & `tmp/module_qc_database_tools-0.3.0.tar.gz`

## Comparing `module_qc_database_tools-0.2.0.tar` & `module_qc_database_tools-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.env.template
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/ci/pre-commit-update.sh
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/chip_config_api.py
--rw-r--r--   0        0        0    15393 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/core.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/utils.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_config_api.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_package.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/.gitignore
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/README.md
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 module_qc_database_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/.env.template
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0    11136 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/README.md
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 module_qc_database_tools-0.3.0/PKG-INFO
```

### Comparing `module_qc_database_tools-0.2.0/.gitlab-ci.yml` & `module_qc_database_tools-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/.pre-commit-config.yaml` & `module_qc_database_tools-0.3.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     rev: "23.3.0"
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.4.0"
     hooks:
-      - id: check-added-large-files
+      # - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
         exclude: mkdocs.yml
       - id: check-yaml
         name: check-yaml (unsafe)
@@ -36,36 +36,42 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.0.1
+    hooks:
+      - id: check-added-large-files
+
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.6"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
+        language_version: 16.14.2
 
   - repo: https://github.com/asottile/blacken-docs
     rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.8.0]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.264
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
```

### Comparing `module_qc_database_tools-0.2.0/tbump.toml` & `module_qc_database_tools-0.3.0/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e32 2e30 220a 0a23 2045  t = "0.2.0"..# E
+00000010: 7420 3d20 2230 2e33 2e30 220a 0a23 2045  t = "0.3.0"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -14,15 +14,15 @@
 000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 322e  mp version: 0.2.
+00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 332e  mp version: 0.3.
 00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section
```

### Comparing `module_qc_database_tools-0.2.0/ci/pre-commit-update.sh` & `module_qc_database_tools-0.3.0/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/src/module_qc_database_tools/chip_config_api.py` & `module_qc_database_tools-0.3.0/src/module_qc_database_tools/chip_config_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,23 +181,26 @@
 
             log.info("pixelcfg md5 hash = %s", md5)
 
             if self.client.localdb.fs.files.find_one({"md5": md5}) is not None:
                 log.info(
                     "info: identified the same pixel config data in gridfs, reusing it."
                 )
-                pixelcfg_id = self.client.localdb.fs.files.find_one({"md5": md5})
+                pixelcfg_doc = self.client.localdb.fs.files.find_one({"md5": md5})
                 is_pixelcfg_revised = False
             else:
                 pixelcfg_id = filesystem.put(binary)
+                pixelcfg_doc = self.client.localdb.fs.files.find_one(
+                    {"_id": ObjectId(pixelcfg_id)}
+                )
                 is_pixelcfg_revised = True
 
         else:
             log.info("pixelcfg is None, skipping pickling")
-            pixelcfg_id = None
+            pixelcfg_doc = None
             is_pixelcfg_revised = True
 
         _ = [fe_cfg.get("RD53B").pop(key) for key in keys_to_remove]
 
         config = self.database.fe_configs.find_one({"_id": ObjectId(config_id)})
         previous_revision_id = config.get("current_revision_id")
 
@@ -227,15 +230,15 @@
             return previous_revision_id
 
         # Save the revision and update the config to point to it
         revision_doc = {
             "parent_revision_id": previous_revision_id,
             "config_data": fe_cfg,
             "diff": the_diff,
-            "pix_config": pixelcfg_id,
+            "pix_config": pixelcfg_doc,
             "message": message,
             "timestamp": timestamp,
             "tags": [],
         }
 
         result = self.database.fe_config_revision.insert_one(revision_doc)
         revision_id = result.inserted_id
```

### Comparing `module_qc_database_tools-0.2.0/src/module_qc_database_tools/core.py` & `module_qc_database_tools-0.3.0/src/module_qc_database_tools/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import copy
 import json
 import logging
 import math
 from pathlib import Path
 
 import pandas as pd
+from rich.logging import RichHandler
 
 from module_qc_database_tools.utils import chip_serial_number_to_uid
 
 log = logging.getLogger(__name__)
-log.setLevel(logging.INFO)
+logging.basicConfig(
+    level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler()]
+)
 
 
 class Module:
     """
     Module class.
     """
 
@@ -59,30 +62,34 @@
             layer_config,
         )
 
         configs = {"module": {"chipType": "RD53B", "chips": []}, "chips": []}
 
         for chip_index, chip in enumerate(self.chips):
             if self.module_type == "triplet":
-                rx = [0, 1, 2][chip_index]
+                rx = [2, 1, 0][chip_index]
             else:
                 rx = [2, 1, 0, 3][chip_index]
 
-            configs["chips"].append(
-                chip.generate_config(
-                    copy.deepcopy(
-                        chip_template
-                    ),  # NB: make sure we copy as Chip::generate_config modifies this in-place
-                    chip_index,
-                    layer_config,
-                    self.module_type,
-                    suffix=suffix,
-                    version=version,
+            try:
+                configs["chips"].append(
+                    chip.generate_config(
+                        copy.deepcopy(
+                            chip_template
+                        ),  # NB: make sure we copy as Chip::generate_config modifies this in-place
+                        chip_index,
+                        layer_config,
+                        self.module_type,
+                        suffix=suffix,
+                        version=version,
+                    )
                 )
-            )
+            except RuntimeError as snake:
+                log.warning(snake)
+                continue
 
             # relative path: e.g. L2_warm/0x15499_L2_warm.json
             chip_config_path = (
                 Path(f"{layer_config}{'_'+suffix if suffix else ''}")
                 / f"{chip.uid}_{layer_config}{'_'+suffix if suffix else ''}.json"
             )
 
@@ -109,24 +116,28 @@
         self.client = client
         self.serial_number = serial_number
         self.uid = chip_serial_number_to_uid(serial_number)
         self.module_name = module_name or self.serial_number
         self.chip = client.get(
             "getComponent", json={"component": serial_number, "noEosToken": False}
         )
-        self.attachments = [
-            item for item in self.chip["attachments"] if item["type"] == "eos"
-        ]
+        self.attachments = list(self.chip["attachments"])
         self.test_run = None
 
         log.info("chip %s initiated.", self.uid)
 
     def get_latest_configs(self, item):
         """use title for filename: 'title': '0x12345_<layer_config>_<suffix>.json'"""
-        infile = self.client.get(item["url"])
+        if item.get("type") == "eos":
+            infile = self.client.get(item["url"])
+        else:
+            infile = self.client.get(
+                "uu-app-binarystore/getBinaryData", json={"code": item["code"]}
+            )
+
         with Path(infile.filename).open(mode="r", encoding="UTF-8") as fsnake:
             return json.loads(fsnake.read())
 
     def load_wafer_probing_data(self):
         """
         Load chip wafer probing data.
         """
@@ -156,28 +167,30 @@
         Generate chip config.
         """
         if version == "latest" and len(self.attachments) >= 3:
             checklist = [".json", layer_config, suffix]
             for item in self.attachments:
                 if all(check in item["title"] for check in checklist):
                     log.info(
-                        " Latest chip configs found for %s %s!", layer_config, suffix
+                        "Latest chip configs found for chip %s %s %s!",
+                        self.uid,
+                        layer_config,
+                        suffix,
                     )
                     try:
                         return self.get_latest_configs(item)
                     except RuntimeError as esnake:
                         log.warning(
-                            " Unable to find latest config: %s. Make sure all sets of configs are present in the database.",
+                            "Unable to find latest config: %s. Make sure all sets of configs are present in the database.",
                             esnake,
                         )
                         continue
-
                 else:
                     log.warning(
-                        " No layer_config %s or suffix %s found in %s",
+                        "No layer_config %s or suffix %s found in %s",
                         layer_config,
                         suffix,
                         item["title"],
                     )
                     continue
         elif version == "TESTONWAFER" or len(self.attachments) == 0:
             log.info(
@@ -383,17 +396,15 @@
                 ] = self.test_run.get_result("VINA_SHUNT_KFACTOR")
                 chip_template["RD53B"]["Parameter"][
                     "KShuntD"
                 ] = self.test_run.get_result("VIND_SHUNT_KFACTOR")
 
             return chip_template
         else:
-            msg = (
-                "Not able to generate chip config. Chip configs might not be complete."
-            )
+            msg = f"Not able to generate config for chip {self.uid}. Chip configs might not be complete."
             raise RuntimeError(msg)
         return None
 
 
 class TestRun:
     """
     TestRun class.
```

### Comparing `module_qc_database_tools-0.2.0/src/module_qc_database_tools/utils.py` & `module_qc_database_tools-0.3.0/src/module_qc_database_tools/utils.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/generate_yarr_config.py` & `module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/generate_yarr_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 )
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
 
 @app.command()
 def main(
-    serial_number: str = typer.Option(..., "-sn", "--sn", help="ATLAS serialNumber"),
+    serial_number: str = typer.Option(..., "-sn", "--sn", help="ATLAS serial number"),
     chip_template_path: Path = typer.Option(
         (module_qc_database_tools.data / "YARR" / "chip_template.json").resolve(),
         "-ch",
         "--chipTemplate",
         help="Default chip template from which the chip configs are generated.",
         exists=True,
         file_okay=True,
         readable=True,
         resolve_path=True,
     ),
     output_dir: Optional[Path] = typer.Option(
         None,
         "-o",
         "--outdir",
-        help="Path to output directory. Configs must be in Yarr/configs. If not specified, will store configs in mongodb.",
+        help="Path to output directory. If not specified, will store configs in mongodb.",
         exists=False,
         writable=True,
     ),
     modes: List[str] = typer.Option(
         ["warm", "cold", "LP"],
         "-m",
         "--mode",
```

### Comparing `module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-0.3.0/src/module_qc_database_tools/cli/register_component.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-0.3.0/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/tests/test_cli.py` & `module_qc_database_tools-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/tests/test_config_api.py` & `module_qc_database_tools-0.3.0/tests/test_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/.gitignore` & `module_qc_database_tools-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.2.0/README.md` & `module_qc_database_tools-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v0.2.0
+# Module QC Database Tools v0.3.0
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

### Comparing `module_qc_database_tools-0.2.0/pyproject.toml` & `module_qc_database_tools-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,22 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Development Status :: 1 - Planning",
 ]
 
 dependencies = [
-    "itkdb>=0.4.0",  # for interface with production database
+    "itkdb>=0.4.3",  # for interface with production database
     "pandas",
     "typer",
     "pymongo",
     "jsondiff",
     "importlib_resources>=1.4.0; python_version < '3.9'",  # for resources
     "jsbeautifier", # for chip config linebreaks vs size
+    "rich"
 ]
 
 [project.urls]
 Homepage = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues"
 Source = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools"
```

### Comparing `module_qc_database_tools-0.2.0/PKG-INFO` & `module_qc_database_tools-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-database-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules.
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>, Elisabetta Pianori <elisabetta.pianori@cern.ch>, Lingxin Meng <lingxin.meng@cern.ch>
 Classifier: Development Status :: 1 - Planning
@@ -20,23 +20,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
-Requires-Dist: itkdb>=0.4.0
+Requires-Dist: itkdb>=0.4.3
 Requires-Dist: jsbeautifier
 Requires-Dist: jsondiff
 Requires-Dist: pandas
 Requires-Dist: pymongo
+Requires-Dist: rich
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# Module QC Database Tools v0.2.0
+# Module QC Database Tools v0.3.0
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

