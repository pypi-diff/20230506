# Comparing `tmp/compose_viz-0.3.0.tar.gz` & `tmp/compose_viz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose_viz-0.3.0.tar", max compression
+gzip compressed data, was "compose_viz-0.3.1.tar", max compression
```

## Comparing `compose_viz-0.3.0.tar` & `compose_viz-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-01-10 17:08:24.406892 compose_viz-0.3.0/LICENSE
--rw-r--r--   0        0        0     7708 2023-01-10 17:08:24.406892 compose_viz-0.3.0/README.md
--rw-r--r--   0        0        0       51 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/__init__.py
--rw-r--r--   0        0        0       82 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/__main__.py
--rw-r--r--   0        0        0     1576 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/cli.py
--rw-r--r--   0        0        0     4943 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/graph.py
--rw-r--r--   0        0        0        0 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/__init__.py
--rw-r--r--   0        0        0      249 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/compose.py
--rw-r--r--   0        0        0      524 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/device.py
--rw-r--r--   0        0        0      347 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/extends.py
--rw-r--r--   0        0        0      546 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/port.py
--rw-r--r--   0        0        0     2194 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/service.py
--rw-r--r--   0        0        0      804 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/viz_formats.py
--rw-r--r--   0        0        0      654 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/models/volume.py
--rw-r--r--   0        0        0    12260 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/parser.py
--rw-r--r--   0        0        0        0 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/spec/__init__.py
--rw-r--r--   0        0        0    26333 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/spec/compose-spec.json
--rw-r--r--   0        0        0    16175 2023-01-10 17:08:24.406892 compose_viz-0.3.0/compose_viz/spec/compose_spec.py
--rw-r--r--   0        0        0      897 2023-01-10 17:08:24.410892 compose_viz-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8913 1970-01-01 00:00:00.000000 compose_viz-0.3.0/setup.py
--rw-r--r--   0        0        0     8599 1970-01-01 00:00:00.000000 compose_viz-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-06 14:48:50.439527 compose_viz-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7706 2023-05-06 14:48:50.439527 compose_viz-0.3.1/README.md
+-rw-r--r--   0        0        0       51 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/__main__.py
+-rw-r--r--   0        0        0     1576 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/cli.py
+-rw-r--r--   0        0        0     4943 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/graph.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/__init__.py
+-rw-r--r--   0        0        0      249 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/compose.py
+-rw-r--r--   0        0        0      524 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/device.py
+-rw-r--r--   0        0        0      347 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/extends.py
+-rw-r--r--   0        0        0      546 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/port.py
+-rw-r--r--   0        0        0     2194 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/service.py
+-rw-r--r--   0        0        0      804 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/viz_formats.py
+-rw-r--r--   0        0        0      654 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/models/volume.py
+-rw-r--r--   0        0        0    12260 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/parser.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/spec/__init__.py
+-rw-r--r--   0        0        0    26517 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/spec/compose-spec.json
+-rw-r--r--   0        0        0    16662 2023-05-06 14:48:50.439527 compose_viz-0.3.1/compose_viz/spec/compose_spec.py
+-rw-r--r--   0        0        0      897 2023-05-06 14:48:50.443527 compose_viz-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8597 1970-01-01 00:00:00.000000 compose_viz-0.3.1/PKG-INFO
```

### Comparing `compose_viz-0.3.0/LICENSE` & `compose_viz-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/README.md` & `compose_viz-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
 ## Contact
 
 ### Author
 
 - HSING-HAN, WU (Xyphuz)
   - Mail me: xyphuzwu@gmail.com
-  - About me: <https://about.xyphuz.com>
+  - About me: <https://www.xyphuz.com>
   - GitHub: <https://github.com/wst24365888>
 
 ### Project Link
 
 - <https://github.com/compose-viz/compose-viz>
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -73,15 +73,15 @@
 push origin feat/amazing-feature`) 5. Open a Pull Request
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See [LICENSE](https://
 github.com/compose-viz/compose-viz/blob/main/LICENSE) for more information.
                                                                   (back_to_top)
  ## Contact ### Author - HSING-HAN, WU (Xyphuz) - Mail me: xyphuzwu@gmail.com -
 About me:
-about.xyphuz.com> - GitHub:
+www.xyphuz.com> - GitHub:
 github.com/wst24365888> ### Project Link -
 github.com/compose-viz/compose-viz>
                                                                   (back_to_top)
 [contributors-shield]: https://img.shields.io/github/contributors/compose-viz/
 compose-viz.svg?style=for-the-badge [contributors-url]: https://github.com/
 compose-viz/compose-viz/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/compose-viz/compose-viz.svg?style=for-the-badge
```

### Comparing `compose_viz-0.3.0/compose_viz/cli.py` & `compose_viz-0.3.1/compose_viz/cli.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/graph.py` & `compose_viz-0.3.1/compose_viz/graph.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/models/device.py` & `compose_viz-0.3.1/compose_viz/models/device.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/models/port.py` & `compose_viz-0.3.1/compose_viz/models/port.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/models/service.py` & `compose_viz-0.3.1/compose_viz/models/service.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/models/viz_formats.py` & `compose_viz-0.3.1/compose_viz/models/viz_formats.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/models/volume.py` & `compose_viz-0.3.1/compose_viz/models/volume.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/parser.py` & `compose_viz-0.3.1/compose_viz/parser.py`

 * *Files identical despite different names*

### Comparing `compose_viz-0.3.0/compose_viz/spec/compose-spec.json` & `compose_viz-0.3.1/compose_viz/spec/compose-spec.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954072530879208%*

 * *Differences: {"'definitions'": "{'service': {'properties': {'build': {'oneOf': {1: {'properties': "*

 * *                  "{'dockerfile_inline': OrderedDict([('type', 'string')]), 'additional_contexts': "*

 * *                  "OrderedDict([('$ref', '#/definitions/list_or_dict')])}}}}, 'command': {replace: "*

 * *                  "OrderedDict([('$ref', '#/definitions/command')])}, 'depends_on': {'oneOf': {1: "*

 * *                  "{'patternProperties': {'^[a-zA-Z0-9._-]+$': {'properties': {'restart': "*

 * *                  "OrderedDict( […]*

```diff
@@ -25,14 +25,30 @@
                 },
                 "weight": {
                     "type": "integer"
                 }
             },
             "type": "object"
         },
+        "command": {
+            "oneOf": [
+                {
+                    "type": "null"
+                },
+                {
+                    "type": "string"
+                },
+                {
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                }
+            ]
+        },
         "config": {
             "additionalProperties": false,
             "id": "#/definitions/config",
             "patternProperties": {
                 "^x-": {}
             },
             "properties": {
@@ -633,14 +649,17 @@
                         },
                         {
                             "additionalProperties": false,
                             "patternProperties": {
                                 "^x-": {}
                             },
                             "properties": {
+                                "additional_contexts": {
+                                    "$ref": "#/definitions/list_or_dict"
+                                },
                                 "args": {
                                     "$ref": "#/definitions/list_or_dict"
                                 },
                                 "cache_from": {
                                     "items": {
                                         "type": "string"
                                     },
@@ -654,14 +673,17 @@
                                 },
                                 "context": {
                                     "type": "string"
                                 },
                                 "dockerfile": {
                                     "type": "string"
                                 },
+                                "dockerfile_inline": {
+                                    "type": "string"
+                                },
                                 "extra_hosts": {
                                     "$ref": "#/definitions/list_or_dict"
                                 },
                                 "isolation": {
                                     "type": "string"
                                 },
                                 "labels": {
@@ -732,25 +754,15 @@
                     ],
                     "type": "string"
                 },
                 "cgroup_parent": {
                     "type": "string"
                 },
                 "command": {
-                    "oneOf": [
-                        {
-                            "type": "string"
-                        },
-                        {
-                            "items": {
-                                "type": "string"
-                            },
-                            "type": "array"
-                        }
-                    ]
+                    "$ref": "#/definitions/command"
                 },
                 "configs": {
                     "$ref": "#/definitions/service_config_or_secret"
                 },
                 "container_name": {
                     "type": "string"
                 },
@@ -834,14 +846,17 @@
                                         "condition": {
                                             "enum": [
                                                 "service_started",
                                                 "service_healthy",
                                                 "service_completed_successfully"
                                             ],
                                             "type": "string"
+                                        },
+                                        "restart": {
+                                            "type": "boolean"
                                         }
                                     },
                                     "required": [
                                         "condition"
                                     ],
                                     "type": "object"
                                 }
@@ -876,25 +891,15 @@
                 "dns_search": {
                     "$ref": "#/definitions/string_or_list"
                 },
                 "domainname": {
                     "type": "string"
                 },
                 "entrypoint": {
-                    "oneOf": [
-                        {
-                            "type": "string"
-                        },
-                        {
-                            "items": {
-                                "type": "string"
-                            },
-                            "type": "array"
-                        }
-                    ]
+                    "$ref": "#/definitions/command"
                 },
                 "env_file": {
                     "$ref": "#/definitions/string_or_list"
                 },
                 "environment": {
                     "$ref": "#/definitions/list_or_dict"
                 },
@@ -1462,14 +1467,15 @@
                     "$ref": "#/definitions/config"
                 }
             },
             "type": "object"
         },
         "name": {
             "description": "define the Compose project name, until user defines one explicitly.",
+            "pattern": "^[a-z0-9][a-z0-9_-]*$",
             "type": "string"
         },
         "networks": {
             "id": "#/properties/networks",
             "patternProperties": {
                 "^[a-zA-Z0-9._-]+$": {
                     "$ref": "#/definitions/network"
```

### Comparing `compose_viz-0.3.0/compose_viz/spec/compose_spec.py` & `compose_viz-0.3.1/compose_viz/spec/compose_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  compose-spec.json
-#   timestamp: 2023-01-10T13:17:45+00:00
+#   timestamp: 2023-05-03T07:42:00+00:00
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import Extra, Field, conint, constr
 from pydantic_yaml import YamlModel, YamlStrEnum
@@ -13,53 +13,54 @@
 class Cgroup(YamlStrEnum):
     host = "host"
     private = "private"
 
 
 class CredentialSpec(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     config: Optional[str] = None
     file: Optional[str] = None
     registry: Optional[str] = None
 
 
 class Condition(YamlStrEnum):
     service_started = "service_started"
     service_healthy = "service_healthy"
     service_completed_successfully = "service_completed_successfully"
 
 
 class DependsOn(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
+    restart: Optional[bool] = None
     condition: Condition
 
 
 class Extend(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     service: str
     file: Optional[str] = None
 
 
 class Logging(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     driver: Optional[str] = None
     options: Optional[Dict[constr(regex=r"^.+$"), Optional[Union[str, float]]]] = None  # type: ignore  # noqa: F722
 
 
 class Port(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     mode: Optional[str] = None
     host_ip: Optional[str] = None
     target: Optional[int] = None
     published: Optional[Union[str, int]] = None
     protocol: Optional[str] = None
 
@@ -70,66 +71,66 @@
     if_not_present = "if_not_present"
     build = "build"
     missing = "missing"
 
 
 class Ulimit(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     hard: int
     soft: int
 
 
 class Selinux(YamlStrEnum):
     z = "z"
     Z = "Z"
 
 
 class Bind(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     propagation: Optional[str] = None
     create_host_path: Optional[bool] = None
     selinux: Optional[Selinux] = None
 
 
 class AdditionalVolumeOption(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     nocopy: Optional[bool] = None
 
 
 class Tmpfs(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     size: Optional[Union[conint(ge=0), str]] = None  # type: ignore
     mode: Optional[float] = None
 
 
 class ServiceVolume(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     type: str
     source: Optional[str] = None
     target: Optional[str] = None
     read_only: Optional[bool] = None
     consistency: Optional[str] = None
     bind: Optional[Bind] = None
     volume: Optional[AdditionalVolumeOption] = None
     tmpfs: Optional[Tmpfs] = None
 
 
 class Healthcheck(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     disable: Optional[bool] = None
     interval: Optional[str] = None
     retries: Optional[float] = None
     test: Optional[Union[str, List[str]]] = None
     timeout: Optional[str] = None
     start_period: Optional[str] = None
@@ -138,15 +139,15 @@
 class Order(YamlStrEnum):
     start_first = "start-first"
     stop_first = "stop-first"
 
 
 class RollbackConfig(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     parallelism: Optional[int] = None
     delay: Optional[str] = None
     failure_action: Optional[str] = None
     monitor: Optional[str] = None
     max_failure_ratio: Optional[float] = None
     order: Optional[Order] = None
@@ -155,317 +156,340 @@
 class ConfigOrder(YamlStrEnum):
     start_first = "start-first"
     stop_first = "stop-first"
 
 
 class UpdateConfig(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     parallelism: Optional[int] = None
     delay: Optional[str] = None
     failure_action: Optional[str] = None
     monitor: Optional[str] = None
     max_failure_ratio: Optional[float] = None
     order: Optional[ConfigOrder] = None
 
 
 class Limits(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     cpus: Optional[Union[float, str]] = None
     memory: Optional[str] = None
     pids: Optional[int] = None
 
 
 class RestartPolicy(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     condition: Optional[str] = None
     delay: Optional[str] = None
     max_attempts: Optional[int] = None
     window: Optional[str] = None
 
 
 class Preference(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     spread: Optional[str] = None
 
 
 class Placement(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     constraints: Optional[List[str]] = None
     preferences: Optional[List[Preference]] = None
     max_replicas_per_node: Optional[int] = None
 
 
 class DiscreteResourceSpec(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     kind: Optional[str] = None
     value: Optional[float] = None
 
 
 class GenericResource(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     discrete_resource_spec: Optional[DiscreteResourceSpec] = None
 
 
 class GenericResources(YamlModel):
+    class Config:
+        extra = Extra.allow
+
     __root__: List[GenericResource]
 
 
 class ConfigItem(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     subnet: Optional[str] = None
     ip_range: Optional[str] = None
     gateway: Optional[str] = None
     aux_addresses: Optional[Dict[constr(regex=r"^.+$"), str]] = None  # type: ignore  # noqa: F722
 
 
 class Ipam(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     driver: Optional[str] = None
     config: Optional[List[ConfigItem]] = None
     options: Optional[Dict[constr(regex=r"^.+$"), str]] = None  # type: ignore  # noqa: F722
 
 
 class ExternalNetwork(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     name: Optional[str] = None
 
 
 class ExternalVolume(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     name: Optional[str] = None
 
 
 class ExternalSecret(YamlModel):
     name: Optional[str] = None
 
 
 class ExternalConfig(YamlModel):
     name: Optional[str] = None
 
 
 class ListOfStrings(YamlModel):
+    class Config:
+        extra = Extra.allow
+
     __root__: List[str] = Field(..., unique_items=True)
 
 
 class ListOrDict(YamlModel):
+    class Config:
+        extra = Extra.allow
+
     __root__: Union[
         Dict[constr(regex=r".+"), Optional[Union[str, float, bool]]], List[str]  # type: ignore  # noqa: F722
     ]
 
 
 class BlkioLimit(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     path: Optional[str] = None
     rate: Optional[Union[int, str]] = None
 
 
 class BlkioWeight(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     path: Optional[str] = None
     weight: Optional[int] = None
 
 
 class ServiceConfigOrSecretItem(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     source: Optional[str] = None
     target: Optional[str] = None
     uid: Optional[str] = None
     gid: Optional[str] = None
     mode: Optional[float] = None
 
 
 class ServiceConfigOrSecret(YamlModel):
+    class Config:
+        extra = Extra.allow
+
     __root__: List[Union[str, ServiceConfigOrSecretItem]]
 
 
 class Constraints(YamlModel):
+    class Config:
+        extra = Extra.allow
+
     __root__: Any
 
 
 class BuildItem(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     context: Optional[str] = None
     dockerfile: Optional[str] = None
+    dockerfile_inline: Optional[str] = None
     args: Optional[ListOrDict] = None
     ssh: Optional[ListOrDict] = None
     labels: Optional[ListOrDict] = None
     cache_from: Optional[List[str]] = None
     cache_to: Optional[List[str]] = None
     no_cache: Optional[bool] = None
+    additional_contexts: Optional[ListOrDict] = None
     network: Optional[str] = None
     pull: Optional[bool] = None
     target: Optional[str] = None
     shm_size: Optional[Union[int, str]] = None
     extra_hosts: Optional[ListOrDict] = None
     isolation: Optional[str] = None
     privileged: Optional[bool] = None
     secrets: Optional[ServiceConfigOrSecret] = None
     tags: Optional[List[str]] = None
     platforms: Optional[List[str]] = None
 
 
 class BlkioConfig(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     device_read_bps: Optional[List[BlkioLimit]] = None
     device_read_iops: Optional[List[BlkioLimit]] = None
     device_write_bps: Optional[List[BlkioLimit]] = None
     device_write_iops: Optional[List[BlkioLimit]] = None
     weight: Optional[int] = None
     weight_device: Optional[List[BlkioWeight]] = None
 
 
 class ServiceNetwork(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     aliases: Optional[ListOfStrings] = None
     ipv4_address: Optional[str] = None
     ipv6_address: Optional[str] = None
     link_local_ips: Optional[ListOfStrings] = None
     priority: Optional[float] = None
 
 
 class Device(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     capabilities: Optional[ListOfStrings] = None
     count: Optional[Union[str, int]] = None
     device_ids: Optional[ListOfStrings] = None
     driver: Optional[str] = None
     options: Optional[ListOrDict] = None
 
 
 class Devices(YamlModel):
+    class Config:
+        extra = Extra.allow
+
     __root__: List[Device]
 
 
 class Network(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     name: Optional[str] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[constr(regex=r"^.+$"), Union[str, float]]] = None  # type: ignore  # noqa: F722
     ipam: Optional[Ipam] = None
     external: Optional[bool | ExternalNetwork] = None
     internal: Optional[bool] = None
     enable_ipv6: Optional[bool] = None
     attachable: Optional[bool] = None
     labels: Optional[ListOrDict] = None
 
 
 class Volume(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     name: Optional[str] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[constr(regex=r"^.+$"), Union[str, float]]] = None  # type: ignore  # noqa: F722
     external: Optional[ExternalVolume] = None
     labels: Optional[ListOrDict] = None
 
 
 class Secret(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     name: Optional[str] = None
     environment: Optional[str] = None
     file: Optional[str] = None
     external: Optional[ExternalSecret] = None
     labels: Optional[ListOrDict] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[constr(regex=r"^.+$"), Union[str, float]]] = None  # type: ignore  # noqa: F722
     template_driver: Optional[str] = None
 
 
 class Config(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     name: Optional[str] = None
     file: Optional[str] = None
     external: Optional[ExternalConfig] = None
     labels: Optional[ListOrDict] = None
     template_driver: Optional[str] = None
 
 
 class StringOrList(YamlModel):
+    class Config:
+        extra = Extra.allow
+
     __root__: Union[str, ListOfStrings]
 
 
 class Reservations(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     cpus: Optional[Union[float, str]] = None
     memory: Optional[str] = None
     generic_resources: Optional[GenericResources] = None
     devices: Optional[Devices] = None
 
 
 class Resources(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     limits: Optional[Limits] = None
     reservations: Optional[Reservations] = None
 
 
 class Deployment(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     mode: Optional[str] = None
     endpoint_mode: Optional[str] = None
     replicas: Optional[int] = None
     labels: Optional[ListOrDict] = None
     rollback_config: Optional[RollbackConfig] = None
     update_config: Optional[UpdateConfig] = None
     resources: Optional[Resources] = None
     restart_policy: Optional[RestartPolicy] = None
     placement: Optional[Placement] = None
 
 
 class Service(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     deploy: Optional[Deployment] = None
     build: Optional[Union[str, BuildItem]] = None
     blkio_config: Optional[BlkioConfig] = None
     cap_add: Optional[List[str]] = Field(None, unique_items=True)
     cap_drop: Optional[List[str]] = Field(None, unique_items=True)
     cgroup: Optional[Cgroup] = None
@@ -550,18 +574,18 @@
     volumes: Optional[List[Union[str, ServiceVolume]]] = Field(None, unique_items=True)
     volumes_from: Optional[List[str]] = Field(None, unique_items=True)
     working_dir: Optional[str] = None
 
 
 class ComposeSpecification(YamlModel):
     class Config:
-        extra = Extra.forbid
+        extra = Extra.allow
 
     version: Optional[str] = Field(None, description="declared for backward compatibility, ignored.")
-    name: Optional[str] = Field(
+    name: Optional[constr(regex=r"^[a-z0-9][a-z0-9_-]*$")] = Field(  # type: ignore  # noqa: F722
         None,
         description="define the Compose project name, until user defines one explicitly.",
     )
     services: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Service]] = None  # type: ignore  # noqa: F722
     networks: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Optional[Network]]] = None  # type: ignore  # noqa: F722
     volumes: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Optional[Volume]]] = None  # type: ignore  # noqa: F722
     secrets: Optional[Dict[constr(regex=r"^[a-zA-Z0-9._-]+$"), Secret]] = None  # type: ignore  # noqa: F722
```

### Comparing `compose_viz-0.3.0/pyproject.toml` & `compose_viz-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compose-viz"
-version = "0.3.0"
+version = "0.3.1"
 description = "A compose file visualization tool that supports compose-spec and allows you to gernerate graph in several formats."
 authors = ["Xyphuz Wu <xyphuzwu@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/compose-viz/compose-viz"
 repository = "https://github.com/compose-viz/compose-viz"
 include = [
```

### Comparing `compose_viz-0.3.0/setup.py` & `compose_viz-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,223 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: compose-viz
+Version: 0.3.1
+Summary: A compose file visualization tool that supports compose-spec and allows you to gernerate graph in several formats.
+Home-page: https://github.com/compose-viz/compose-viz
+License: MIT
+Author: Xyphuz Wu
+Author-email: xyphuzwu@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: graphviz (>=0.20,<0.21)
+Requires-Dist: pydantic-yaml (>=0.7.0,<0.8.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: typer (>=0.4.1,<0.5.0)
+Project-URL: Repository, https://github.com/compose-viz/compose-viz
+Description-Content-Type: text/markdown
 
-packages = \
-['compose_viz', 'compose_viz.models', 'compose_viz.spec']
+<div id="top"></div>
 
-package_data = \
-{'': ['*']}
+<!-- PROJECT SHIELDS -->
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'graphviz>=0.20,<0.21',
- 'pydantic-yaml>=0.7.0,<0.8.0',
- 'ruamel.yaml>=0.17.21,<0.18.0',
- 'typer>=0.4.1,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['cpv = compose_viz.cli:start_cli']}
-
-setup_kwargs = {
-    'name': 'compose-viz',
-    'version': '0.3.0',
-    'description': 'A compose file visualization tool that supports compose-spec and allows you to gernerate graph in several formats.',
-    'long_description': '<div id="top"></div>\n\n<!-- PROJECT SHIELDS -->\n\n[<div align="center"> ![Contributors][contributors-shield]][contributors-url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![MIT License][license-shield]][license-url]\n[![Issues][issues-shield]][issues-url]\n[![Issues Closed][issues-closed-shield]</div>][issues-closed-url]\n\n<br />\n\n<!-- PROJECT LOGO -->\n\n![compose-viz](https://socialify.git.ci/compose-viz/compose-viz/image?description=1&font=KoHo&name=1&owner=1&pattern=Circuit%20Board&theme=Light)\n\n<br />\n<div align="center">\n<p align="center">\n    <a href="https://github.com/compose-viz/compose-viz#usage"><strong>Explore Usage »</strong></a>\n    <br />\n    <br />\n    <a href="https://github.com/compose-viz/compose-viz/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/compose-viz/compose-viz/issues">Request Feature</a>\n  </p>\n</div>\n\n<!-- TABLE OF CONTENTS -->\n\n<details>\n  <summary>Table of Contents</summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisities">Prerequisities</a></li>\n        <li><a href="#installation">Installation</a></li>\n        <li><a href="#example">Example</a></li>\n        <li><a href="#usage">Usage</a></li>\n        <li><a href="#options">Options</a></li>\n      </ul>\n    </li>\n    <li><a href="#roadmap">Roadmap</a></li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#license">License</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\n`compose-viz` is a compose file visualization tool that follows [compose-spec](https://github.com/compose-spec/compose-spec/blob/master/spec.md) and allows you to gernerate graph in several formats.\n\nIf you are looking for a compose file vizualization tool, and you are using one of the [compose-spec](https://github.com/compose-spec/compose-spec/blob/master/spec.md) implementations (e.g. [docker-compose](https://github.com/docker/compose)/[podman-compose](https://github.com/containers/podman-compose)), then `compose-viz` is a great choice for you. \n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- GETTING STARTED -->\n\n## Getting Started\n\n### Prerequisities\n\n#### Graphviz\n\nYou need to install [Graphviz](https://graphviz.org/download/) to generate graphs.\n\n### Installation\n\n#### Using `pip`\n\n```\npip install compose-viz\n```\n\n#### Using `.whl`\n\nSee [releases](https://github.com/compose-viz/compose-viz/releases).\n\n#### Docker Image\n\nSee [wst24365888/compose-viz](https://hub.docker.com/r/wst24365888/compose-viz/tags).\n\n### Example\n\nThis example yml is from [docker compose beginner tutorial](https://github.com/docker/labs/blob/master/beginner/chapters/votingapp.md).\n\n```bash\ncd examples/voting-app/\n\n# using python script\ncpv -m svg docker-compose.yml\n\n# using docker image\ndocker run --rm -it -v $(pwd):/in wst24365888/compose-viz -m svg docker-compose.yml\n\n# using docker image in powershell\ndocker run --rm -it -v ${pwd}:/in wst24365888/compose-viz -m svg docker-compose.yml\n```\n\nAnd this is what the result looks like:\n\n![compose-viz.svg](https://github.com/compose-viz/compose-viz/blob/main/examples/voting-app/compose-viz.svg)\n\nCheck out the result [here](https://github.com/compose-viz/compose-viz/blob/main/examples/voting-app).\n\n### Usage\n\n`cpv [OPTIONS] INPUT_PATH`\n\n### Options\n\n| Option                            | Description                                                                                                                                                                         |\n| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| `-o, --output-filename FILENAME`  | Output filename for the generated visualization file. [default: compose-viz]                                                                                                        |\n| `-m, --format FORMAT`             | Output format for the generated visualization file. See [supported formats](https://github.com/compose-viz/compose-viz/blob/main/compose_viz/models/viz_formats.py). [default: png] |\n| `-r, --root-service SERVICE_NAME` | Root of the service tree (convenient for large compose yamls)                                                                                                                       |\n| `-v, --version`                   | Show the version of compose-viz.                                                                                                                                                    |\n| `--help`                          | Show help and exit.                                                                                                                                                                 |\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- ROADMAP -->\n\n## Roadmap\n\n- [ ] Support more vizualization components.\n\nSee the [open issues](https://github.com/compose-viz/compose-viz/issues)\nfor a full list of proposed features (and known issues).\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- CONTRIBUTING -->\n\n## Contributing\n\nContributions are what make the open source community such an amazing place to\nlearn, inspire, and create. Any contributions you make are **greatly\nappreciated**.\n\nIf you have a suggestion that would make this better, please fork the repo and\ncreate a pull request. You can also simply open an issue with the tag\n"enhancement". Don\'t forget to give the project a star! Thanks again!\n\n1. Fork the Project\n2. Create your Feature Branch (`git checkout -b feat/amazing-feature`)\n3. Commit your Changes with\n   [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)\n4. Push to the Branch (`git push origin feat/amazing-feature`)\n5. Open a Pull Request\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- LICENSE -->\n\n## License\n\nDistributed under the MIT License. See\n[LICENSE](https://github.com/compose-viz/compose-viz/blob/main/LICENSE)\nfor more information.\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n<!-- CONTACT -->\n\n## Contact\n\n### Author\n\n- HSING-HAN, WU (Xyphuz)\n  - Mail me: xyphuzwu@gmail.com\n  - About me: <https://about.xyphuz.com>\n  - GitHub: <https://github.com/wst24365888>\n\n### Project Link\n\n- <https://github.com/compose-viz/compose-viz>\n\n<p align="right">(<a href="#top">back to top</a>)</p>\n\n[contributors-shield]: https://img.shields.io/github/contributors/compose-viz/compose-viz.svg?style=for-the-badge\n[contributors-url]: https://github.com/compose-viz/compose-viz/graphs/contributors\n[forks-shield]: https://img.shields.io/github/forks/compose-viz/compose-viz.svg?style=for-the-badge\n[forks-url]: https://github.com/compose-viz/compose-viz/network/members\n[stars-shield]: https://img.shields.io/github/stars/compose-viz/compose-viz.svg?style=for-the-badge\n[stars-url]: https://github.com/compose-viz/compose-viz/stargazers\n[issues-shield]: https://img.shields.io/github/issues/compose-viz/compose-viz.svg?style=for-the-badge\n[issues-url]: https://github.com/compose-viz/compose-viz/issues\n[issues-closed-shield]: https://img.shields.io/github/issues-closed/compose-viz/compose-viz.svg?style=for-the-badge\n[issues-closed-url]: https://github.com/compose-viz/compose-viz/issues?q=is%3Aissue+is%3Aclosed\n[license-shield]: https://img.shields.io/github/license/compose-viz/compose-viz.svg?style=for-the-badge\n[license-url]: https://github.com/compose-viz/compose-viz/blob/main/LICENSE\n',
-    'author': 'Xyphuz Wu',
-    'author_email': 'xyphuzwu@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/compose-viz/compose-viz',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+[<div align="center"> ![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![MIT License][license-shield]][license-url]
+[![Issues][issues-shield]][issues-url]
+[![Issues Closed][issues-closed-shield]</div>][issues-closed-url]
 
+<br />
+
+<!-- PROJECT LOGO -->
+
+![compose-viz](https://socialify.git.ci/compose-viz/compose-viz/image?description=1&font=KoHo&name=1&owner=1&pattern=Circuit%20Board&theme=Light)
+
+<br />
+<div align="center">
+<p align="center">
+    <a href="https://github.com/compose-viz/compose-viz#usage"><strong>Explore Usage »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/compose-viz/compose-viz/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/compose-viz/compose-viz/issues">Request Feature</a>
+  </p>
+</div>
+
+<!-- TABLE OF CONTENTS -->
+
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisities">Prerequisities</a></li>
+        <li><a href="#installation">Installation</a></li>
+        <li><a href="#example">Example</a></li>
+        <li><a href="#usage">Usage</a></li>
+        <li><a href="#options">Options</a></li>
+      </ul>
+    </li>
+    <li><a href="#roadmap">Roadmap</a></li>
+    <li><a href="#contributing">Contributing</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+  </ol>
+</details>
+
+<!-- ABOUT THE PROJECT -->
+
+## About The Project
+
+`compose-viz` is a compose file visualization tool that follows [compose-spec](https://github.com/compose-spec/compose-spec/blob/master/spec.md) and allows you to gernerate graph in several formats.
+
+If you are looking for a compose file vizualization tool, and you are using one of the [compose-spec](https://github.com/compose-spec/compose-spec/blob/master/spec.md) implementations (e.g. [docker-compose](https://github.com/docker/compose)/[podman-compose](https://github.com/containers/podman-compose)), then `compose-viz` is a great choice for you. 
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- GETTING STARTED -->
+
+## Getting Started
+
+### Prerequisities
+
+#### Graphviz
+
+You need to install [Graphviz](https://graphviz.org/download/) to generate graphs.
+
+### Installation
+
+#### Using `pip`
+
+```
+pip install compose-viz
+```
+
+#### Using `.whl`
+
+See [releases](https://github.com/compose-viz/compose-viz/releases).
+
+#### Docker Image
+
+See [wst24365888/compose-viz](https://hub.docker.com/r/wst24365888/compose-viz/tags).
+
+### Example
+
+This example yml is from [docker compose beginner tutorial](https://github.com/docker/labs/blob/master/beginner/chapters/votingapp.md).
+
+```bash
+cd examples/voting-app/
+
+# using python script
+cpv -m svg docker-compose.yml
+
+# using docker image
+docker run --rm -it -v $(pwd):/in wst24365888/compose-viz -m svg docker-compose.yml
+
+# using docker image in powershell
+docker run --rm -it -v ${pwd}:/in wst24365888/compose-viz -m svg docker-compose.yml
+```
+
+And this is what the result looks like:
+
+![compose-viz.svg](https://github.com/compose-viz/compose-viz/blob/main/examples/voting-app/compose-viz.svg)
+
+Check out the result [here](https://github.com/compose-viz/compose-viz/blob/main/examples/voting-app).
+
+### Usage
+
+`cpv [OPTIONS] INPUT_PATH`
+
+### Options
+
+| Option                            | Description                                                                                                                                                                         |
+| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `-o, --output-filename FILENAME`  | Output filename for the generated visualization file. [default: compose-viz]                                                                                                        |
+| `-m, --format FORMAT`             | Output format for the generated visualization file. See [supported formats](https://github.com/compose-viz/compose-viz/blob/main/compose_viz/models/viz_formats.py). [default: png] |
+| `-r, --root-service SERVICE_NAME` | Root of the service tree (convenient for large compose yamls)                                                                                                                       |
+| `-v, --version`                   | Show the version of compose-viz.                                                                                                                                                    |
+| `--help`                          | Show help and exit.                                                                                                                                                                 |
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- ROADMAP -->
+
+## Roadmap
+
+- [ ] Support more vizualization components.
+
+See the [open issues](https://github.com/compose-viz/compose-viz/issues)
+for a full list of proposed features (and known issues).
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- CONTRIBUTING -->
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to
+learn, inspire, and create. Any contributions you make are **greatly
+appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and
+create a pull request. You can also simply open an issue with the tag
+"enhancement". Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feat/amazing-feature`)
+3. Commit your Changes with
+   [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
+4. Push to the Branch (`git push origin feat/amazing-feature`)
+5. Open a Pull Request
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- LICENSE -->
+
+## License
+
+Distributed under the MIT License. See
+[LICENSE](https://github.com/compose-viz/compose-viz/blob/main/LICENSE)
+for more information.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+<!-- CONTACT -->
+
+## Contact
+
+### Author
+
+- HSING-HAN, WU (Xyphuz)
+  - Mail me: xyphuzwu@gmail.com
+  - About me: <https://www.xyphuz.com>
+  - GitHub: <https://github.com/wst24365888>
+
+### Project Link
+
+- <https://github.com/compose-viz/compose-viz>
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+[contributors-shield]: https://img.shields.io/github/contributors/compose-viz/compose-viz.svg?style=for-the-badge
+[contributors-url]: https://github.com/compose-viz/compose-viz/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/compose-viz/compose-viz.svg?style=for-the-badge
+[forks-url]: https://github.com/compose-viz/compose-viz/network/members
+[stars-shield]: https://img.shields.io/github/stars/compose-viz/compose-viz.svg?style=for-the-badge
+[stars-url]: https://github.com/compose-viz/compose-viz/stargazers
+[issues-shield]: https://img.shields.io/github/issues/compose-viz/compose-viz.svg?style=for-the-badge
+[issues-url]: https://github.com/compose-viz/compose-viz/issues
+[issues-closed-shield]: https://img.shields.io/github/issues-closed/compose-viz/compose-viz.svg?style=for-the-badge
+[issues-closed-url]: https://github.com/compose-viz/compose-viz/issues?q=is%3Aissue+is%3Aclosed
+[license-shield]: https://img.shields.io/github/license/compose-viz/compose-viz.svg?style=for-the-badge
+[license-url]: https://github.com/compose-viz/compose-viz/blob/main/LICENSE
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,131 +1,110 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['compose_viz', 'compose_viz.models', 'compose_viz.spec'] package_data = \ {'':
-['*']} install_requires = \ ['PyYAML>=6.0,<7.0', 'graphviz>=0.20,<0.21',
-'pydantic-yaml>=0.7.0,<0.8.0', 'ruamel.yaml>=0.17.21,<0.18.0',
-'typer>=0.4.1,<0.5.0'] entry_points = \ {'console_scripts': ['cpv =
-compose_viz.cli:start_cli']} setup_kwargs = { 'name': 'compose-viz', 'version':
-'0.3.0', 'description': 'A compose file visualization tool that supports
-compose-spec and allows you to gernerate graph in several formats.',
-'long_description': '
-\n\n\n\n[
-   ![Contributors][contributors-shield]][contributors-url]\n[![Forks][forks-
-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![MIT License]
-  [license-shield]][license-url]\n[![Issues][issues-shield]][issues-url]\n[!
-                     [Issues Closed][issues-closed-shield]
-][issues-closed-url]\n\n
-\n\n\n\n![compose-viz](https://socialify.git.ci/compose-viz/compose-viz/
-image?description=1&font=KoHo&name=1&owner=1&pattern=Circuit%20Board&theme=Light)\n\n
-\n
-                                      \n
-                            \n Explore_Usage_Â»\n
-                                      \n
-                    \n Report_Bug\n Â·\n Request_Feature\n
-                                      \n
-\n\n\n\n\n Table of Contents\n
-   1. \n
-   2. \n About_The_Project\n
-   3. \n
-   4. \n Getting_Started\n
-          o \n
+Metadata-Version: 2.1 Name: compose-viz Version: 0.3.1 Summary: A compose file
+visualization tool that supports compose-spec and allows you to gernerate graph
+in several formats. Home-page: https://github.com/compose-viz/compose-viz
+License: MIT Author: Xyphuz Wu Author-email: xyphuzwu@gmail.com Requires-
+Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: PyYAML
+(>=6.0,<7.0) Requires-Dist: graphviz (>=0.20,<0.21) Requires-Dist: pydantic-
+yaml (>=0.7.0,<0.8.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-
+Dist: typer (>=0.4.1,<0.5.0) Project-URL: Repository, https://github.com/
+compose-viz/compose-viz Description-Content-Type: text/markdown
+ [
+   ![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+ shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![MIT License]
+[license-shield]][license-url] [![Issues][issues-shield]][issues-url] [![Issues
+                         Closed][issues-closed-shield]
+][issues-closed-url]
+ ![compose-viz](https://socialify.git.ci/compose-viz/compose-viz/
+image?description=1&font=KoHo&name=1&owner=1&pattern=Circuit%20Board&theme=Light)
+
+                               Explore_Usage_Â»
+
+                         Report_Bug Â· Request_Feature
+  Table of Contents
+   1. About_The_Project
+   2. Getting_Started
           o Prerequisities
-          o \n
           o Installation
-          o \n
           o Example
-          o \n
           o Usage
-          o \n
           o Options
-          o \n
-      \n
-   5. \n
-   6. Roadmap
-   7. \n
-   8. Contributing
-   9. \n
-  10. License
-  11. \n
-  12. Contact
-  13. \n
-\n\n\n\n\n## About The Project\n\n`compose-viz` is a compose file visualization
-tool that follows [compose-spec](https://github.com/compose-spec/compose-spec/
-blob/master/spec.md) and allows you to gernerate graph in several
-formats.\n\nIf you are looking for a compose file vizualization tool, and you
-are using one of the [compose-spec](https://github.com/compose-spec/compose-
-spec/blob/master/spec.md) implementations (e.g. [docker-compose](https://
-github.com/docker/compose)/[podman-compose](https://github.com/containers/
-podman-compose)), then `compose-viz` is a great choice for you. \n\n
-                                                                  (back_to_top)
-\n\n\n\n## Getting Started\n\n### Prerequisities\n\n#### Graphviz\n\nYou need
-to install [Graphviz](https://graphviz.org/download/) to generate
-graphs.\n\n### Installation\n\n#### Using `pip`\n\n```\npip install compose-
-viz\n```\n\n#### Using `.whl`\n\nSee [releases](https://github.com/compose-viz/
-compose-viz/releases).\n\n#### Docker Image\n\nSee [wst24365888/compose-viz]
-(https://hub.docker.com/r/wst24365888/compose-viz/tags).\n\n### Example\n\nThis
-example yml is from [docker compose beginner tutorial](https://github.com/
-docker/labs/blob/master/beginner/chapters/votingapp.md).\n\n```bash\ncd
-examples/voting-app/\n\n# using python script\ncpv -m svg docker-
-compose.yml\n\n# using docker image\ndocker run --rm -it -v $(pwd):/in
-wst24365888/compose-viz -m svg docker-compose.yml\n\n# using docker image in
-powershell\ndocker run --rm -it -v ${pwd}:/in wst24365888/compose-viz -m svg
-docker-compose.yml\n```\n\nAnd this is what the result looks like:\n\n!
-[compose-viz.svg](https://github.com/compose-viz/compose-viz/blob/main/
-examples/voting-app/compose-viz.svg)\n\nCheck out the result [here](https://
-github.com/compose-viz/compose-viz/blob/main/examples/voting-app).\n\n###
-Usage\n\n`cpv [OPTIONS] INPUT_PATH`\n\n### Options\n\n| Option | Description
-|\n| --------------------------------- | --------------------------------------
+   3. Roadmap
+   4. Contributing
+   5. License
+   6. Contact
+  ## About The Project `compose-viz` is a compose file visualization tool that
+follows [compose-spec](https://github.com/compose-spec/compose-spec/blob/
+master/spec.md) and allows you to gernerate graph in several formats. If you
+are looking for a compose file vizualization tool, and you are using one of the
+[compose-spec](https://github.com/compose-spec/compose-spec/blob/master/
+spec.md) implementations (e.g. [docker-compose](https://github.com/docker/
+compose)/[podman-compose](https://github.com/containers/podman-compose)), then
+`compose-viz` is a great choice for you.
+                                                                  (back_to_top)
+ ## Getting Started ### Prerequisities #### Graphviz You need to install
+[Graphviz](https://graphviz.org/download/) to generate graphs. ### Installation
+#### Using `pip` ``` pip install compose-viz ``` #### Using `.whl` See
+[releases](https://github.com/compose-viz/compose-viz/releases). #### Docker
+Image See [wst24365888/compose-viz](https://hub.docker.com/r/wst24365888/
+compose-viz/tags). ### Example This example yml is from [docker compose
+beginner tutorial](https://github.com/docker/labs/blob/master/beginner/
+chapters/votingapp.md). ```bash cd examples/voting-app/ # using python script
+cpv -m svg docker-compose.yml # using docker image docker run --rm -it -v $
+(pwd):/in wst24365888/compose-viz -m svg docker-compose.yml # using docker
+image in powershell docker run --rm -it -v ${pwd}:/in wst24365888/compose-viz -
+m svg docker-compose.yml ``` And this is what the result looks like: ![compose-
+viz.svg](https://github.com/compose-viz/compose-viz/blob/main/examples/voting-
+app/compose-viz.svg) Check out the result [here](https://github.com/compose-
+viz/compose-viz/blob/main/examples/voting-app). ### Usage `cpv [OPTIONS]
+INPUT_PATH` ### Options | Option | Description | | ----------------------------
+----- | -----------------------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------- |\n| `-o, --
-output-filename FILENAME` | Output filename for the generated visualization
-file. [default: compose-viz] |\n| `-m, --format FORMAT` | Output format for the
-generated visualization file. See [supported formats](https://github.com/
-compose-viz/compose-viz/blob/main/compose_viz/models/viz_formats.py). [default:
-png] |\n| `-r, --root-service SERVICE_NAME` | Root of the service tree
-(convenient for large compose yamls) |\n| `-v, --version` | Show the version of
-compose-viz. |\n| `--help` | Show help and exit. |\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Roadmap\n\n- [ ] Support more vizualization components.\n\nSee the
-[open issues](https://github.com/compose-viz/compose-viz/issues)\nfor a full
-list of proposed features (and known issues).\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Contributing\n\nContributions are what make the open source
-community such an amazing place to\nlearn, inspire, and create. Any
-contributions you make are **greatly\nappreciated**.\n\nIf you have a
-suggestion that would make this better, please fork the repo and\ncreate a pull
-request. You can also simply open an issue with the tag\n"enhancement". Don\'t
-forget to give the project a star! Thanks again!\n\n1. Fork the Project\n2.
-Create your Feature Branch (`git checkout -b feat/amazing-feature`)\n3. Commit
-your Changes with\n [Conventional Commits](https://www.conventionalcommits.org/
-en/v1.0.0/)\n4. Push to the Branch (`git push origin feat/amazing-feature`)\n5.
-Open a Pull Request\n\n
-                                                                  (back_to_top)
-\n\n\n\n## License\n\nDistributed under the MIT License. See\n[LICENSE](https:/
-/github.com/compose-viz/compose-viz/blob/main/LICENSE)\nfor more
-information.\n\n
-                                                                  (back_to_top)
-\n\n\n\n## Contact\n\n### Author\n\n- HSING-HAN, WU (Xyphuz)\n - Mail me:
-xyphuzwu@gmail.com\n - About me:
-about.xyphuz.com>\n - GitHub:
-github.com/wst24365888>\n\n### Project Link\n\n-
-github.com/compose-viz/compose-viz>\n\n
-                                                                  (back_to_top)
-\n\n[contributors-shield]: https://img.shields.io/github/contributors/compose-
-viz/compose-viz.svg?style=for-the-badge\n[contributors-url]: https://
-github.com/compose-viz/compose-viz/graphs/contributors\n[forks-shield]: https:/
-/img.shields.io/github/forks/compose-viz/compose-viz.svg?style=for-the-badge\n
-[forks-url]: https://github.com/compose-viz/compose-viz/network/members\n
-[stars-shield]: https://img.shields.io/github/stars/compose-viz/compose-
-viz.svg?style=for-the-badge\n[stars-url]: https://github.com/compose-viz/
-compose-viz/stargazers\n[issues-shield]: https://img.shields.io/github/issues/
-compose-viz/compose-viz.svg?style=for-the-badge\n[issues-url]: https://
-github.com/compose-viz/compose-viz/issues\n[issues-closed-shield]: https://
+----------------------------- | | `-o, --output-filename FILENAME` | Output
+filename for the generated visualization file. [default: compose-viz] | | `-m,
+--format FORMAT` | Output format for the generated visualization file. See
+[supported formats](https://github.com/compose-viz/compose-viz/blob/main/
+compose_viz/models/viz_formats.py). [default: png] | | `-r, --root-service
+SERVICE_NAME` | Root of the service tree (convenient for large compose yamls) |
+| `-v, --version` | Show the version of compose-viz. | | `--help` | Show help
+and exit. |
+                                                                  (back_to_top)
+ ## Roadmap - [ ] Support more vizualization components. See the [open issues]
+(https://github.com/compose-viz/compose-viz/issues) for a full list of proposed
+features (and known issues).
+                                                                  (back_to_top)
+ ## Contributing Contributions are what make the open source community such an
+amazing place to learn, inspire, and create. Any contributions you make are
+**greatly appreciated**. If you have a suggestion that would make this better,
+please fork the repo and create a pull request. You can also simply open an
+issue with the tag "enhancement". Don't forget to give the project a star!
+Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
+-b feat/amazing-feature`) 3. Commit your Changes with [Conventional Commits]
+(https://www.conventionalcommits.org/en/v1.0.0/) 4. Push to the Branch (`git
+push origin feat/amazing-feature`) 5. Open a Pull Request
+                                                                  (back_to_top)
+ ## License Distributed under the MIT License. See [LICENSE](https://
+github.com/compose-viz/compose-viz/blob/main/LICENSE) for more information.
+                                                                  (back_to_top)
+ ## Contact ### Author - HSING-HAN, WU (Xyphuz) - Mail me: xyphuzwu@gmail.com -
+About me:
+www.xyphuz.com> - GitHub:
+github.com/wst24365888> ### Project Link -
+github.com/compose-viz/compose-viz>
+                                                                  (back_to_top)
+[contributors-shield]: https://img.shields.io/github/contributors/compose-viz/
+compose-viz.svg?style=for-the-badge [contributors-url]: https://github.com/
+compose-viz/compose-viz/graphs/contributors [forks-shield]: https://
+img.shields.io/github/forks/compose-viz/compose-viz.svg?style=for-the-badge
+[forks-url]: https://github.com/compose-viz/compose-viz/network/members [stars-
+shield]: https://img.shields.io/github/stars/compose-viz/compose-
+viz.svg?style=for-the-badge [stars-url]: https://github.com/compose-viz/
+compose-viz/stargazers [issues-shield]: https://img.shields.io/github/issues/
+compose-viz/compose-viz.svg?style=for-the-badge [issues-url]: https://
+github.com/compose-viz/compose-viz/issues [issues-closed-shield]: https://
 img.shields.io/github/issues-closed/compose-viz/compose-viz.svg?style=for-the-
-badge\n[issues-closed-url]: https://github.com/compose-viz/compose-viz/
-issues?q=is%3Aissue+is%3Aclosed\n[license-shield]: https://img.shields.io/
-github/license/compose-viz/compose-viz.svg?style=for-the-badge\n[license-url]:
-https://github.com/compose-viz/compose-viz/blob/main/LICENSE\n', 'author':
-'Xyphuz Wu', 'author_email': 'xyphuzwu@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/compose-viz/compose-
-viz', 'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.9,<4.0', } setup(**setup_kwargs)
+badge [issues-closed-url]: https://github.com/compose-viz/compose-viz/
+issues?q=is%3Aissue+is%3Aclosed [license-shield]: https://img.shields.io/
+github/license/compose-viz/compose-viz.svg?style=for-the-badge [license-url]:
+https://github.com/compose-viz/compose-viz/blob/main/LICENSE
```

