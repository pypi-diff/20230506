# Comparing `tmp/hamqtt_fs_publisher-0.1.1.tar.gz` & `tmp/hamqtt_fs_publisher-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamqtt_fs_publisher-0.1.1.tar", max compression
+gzip compressed data, was "hamqtt_fs_publisher-0.1.2.tar", max compression
```

## Comparing `hamqtt_fs_publisher-0.1.1.tar` & `hamqtt_fs_publisher-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/LICENSE
--rw-r--r--   0        0        0     2117 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/README.md
--rw-r--r--   0        0        0       54 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/__main__.py
--rw-r--r--   0        0        0     3314 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.py
--rw-r--r--   0        0        0     9263 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.schema.json
--rw-r--r--   0        0        0     1508 2023-05-06 13:25:28.208413 hamqtt_fs_publisher-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 hamqtt_fs_publisher-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2702 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/README.md
+-rw-r--r--   0        0        0       54 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/__init__.py
+-rw-r--r--   0        0        0     5361 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/__main__.py
+-rw-r--r--   0        0        0     3505 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.py
+-rw-r--r--   0        0        0     9263 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.schema.json
+-rw-r--r--   0        0        0     1688 2023-05-06 14:54:27.043164 hamqtt_fs_publisher-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4054 1970-01-01 00:00:00.000000 hamqtt_fs_publisher-0.1.2/PKG-INFO
```

### Comparing `hamqtt_fs_publisher-0.1.1/LICENSE` & `hamqtt_fs_publisher-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hamqtt_fs_publisher-0.1.1/README.md` & `hamqtt_fs_publisher-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+[![build](https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher/workflows/build/badge.svg)](https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher/actions?query=workflow%3Abuild+branch%3Amain)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hamqtt-fs_publisher.svg)](https://pypi.org/project/hamqtt-fs_publisher)
+
 # HomeAssistant MQTT filesystem publisher
 
 Publish file content as an MQTT topic compatible with HomeAssistant.
 
 It can be useful, e.g., to publish system metrics from `/sys`.
 
 ## Quick start
 
-1. Install the Python package: `pip install hamqtt-fs-publisher`.
+1. Install the Python package: `pip install hamqtt-fs-publisher`. If you want to
+   have support for YAML configuration format install with `ruamel` or `pyyaml`
+   extras depending on the YAML library of choice (recommended `ruamel`, e.g.,
+   `pip install hamqtt-fs-publisher[ruamel]`).
 2. Create a configuration (example in `examples/config.example.yaml`). It can be
    in either YAML or JSON format. There is a pre-generated JSON schema in
    `hamqtt_fs_publisher/configuration.schema.json`, which can be used, e.g.,
    with VS Code (the current repository is pre-configured for `config.json` and
    `config.yaml`). Remember to set proper authorization details for the MQTT
    broker. If you are using the standard Mosquitto broker add-on in Home
    Assistant, please refer to the [official
```

### Comparing `hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/__main__.py` & `hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """HomeAssistant MQTT filesystem publisher service."""
 
+import sys
 import time
 from pathlib import Path
 from threading import Event, Timer
 from typing import List, Optional
 
 import click
 from ha_mqtt.ha_device import HaDevice  # type: ignore
@@ -97,14 +98,15 @@
             config_found = True
             config = tried_path
             logger.debug('Found configuration in "{}".', config)
             break
 
     if not config_found:
         logger.error('Configuration not found at "{}" path.', config)
+        sys.exit(1)
 
     config_parsed = Config.parse_file(config)
 
     logger.info("Connecting to MQTT broker...")
     mqtt_config = config_parsed.mqtt
     client = Client(mqtt_config.client_id)
     if mqtt_config.user is not None:
```

### Comparing `hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.py` & `hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 
 import json
 from pathlib import Path
 from typing import List, Optional
 
 from ha_mqtt.util import EntityCategory, HaDeviceClass  # type: ignore
 from pydantic import BaseModel, Field
-from pydantic_yaml import YamlModel
+
+try:
+    from pydantic_yaml import YamlModel
+except ImportError:
+    # Fall back to JSON-only model.
+    from pydantic import (  # type: ignore # pylint: disable=W0404,C0412 # isort: skip
+        BaseModel as YamlModel,
+    )
 
 
 class Mqtt(BaseModel):  # pylint: disable=R0903
     """MQTT configuration."""
 
     client_id: str = Field(description="MQTT client ID.")
     host: str = Field("localhost", description="MQTT broker host.")
```

### Comparing `hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.schema.json` & `hamqtt_fs_publisher-0.1.2/hamqtt_fs_publisher/configuration.schema.json`

 * *Files identical despite different names*

### Comparing `hamqtt_fs_publisher-0.1.1/pyproject.toml` & `hamqtt_fs_publisher-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hamqtt-fs-publisher"
-version = "0.1.1"
+version = "0.1.2"
 description = "Publish file content as MQTT topic compatible with HomeAssistant."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent",
@@ -16,20 +16,26 @@
     {include = "hamqtt_fs_publisher"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 homeassistant-mqtt-binding = "^2.0.2"
 pydantic = "^1.10.7"
-pydantic-yaml = {extras = ["ruamel"], version = "^0.11.2"}
+pydantic-yaml = {version = "^0.11.2", optional = true}
+ruamel-yaml = {version = "^0.17.24", optional = true}
+pyyaml = {version = "^6.0", optional = true}
 click = "^8.1.3"
 loguru = "^0.7.0"
 
+[tool.poetry.extras]
+ruamel = ["pydantic-yaml", "ruamel-yaml"]
+pyyaml = ["pydantic-yaml", "pyyaml"]
+
 [tool.poetry.scripts]
-hamqtt_fs_publisher = 'hamqtt_fs_publisher.__main__:main'
+hamqtt_fs_publisher = "hamqtt_fs_publisher.__main__:main"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 isort = "^5.12.0"
 ruff = "^0.0.265"
 pydocstyle = "^6.3.0"
@@ -37,15 +43,14 @@
 pylint-pydantic = "^0.1.8"
 types-paho-mqtt = "^1.6.0.6"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pylint-pytest = "^1.1.2"
 coveralls = "^3.3.1"
-pyyaml = "^6.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `hamqtt_fs_publisher-0.1.1/PKG-INFO` & `hamqtt_fs_publisher-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamqtt-fs-publisher
-Version: 0.1.1
+Version: 0.1.2
 Summary: Publish file content as MQTT topic compatible with HomeAssistant.
 Home-page: https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
@@ -13,31 +13,41 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: pyyaml
+Provides-Extra: ruamel
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: homeassistant-mqtt-binding (>=2.0.2,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pydantic-yaml[ruamel] (>=0.11.2,<0.12.0)
+Requires-Dist: pydantic-yaml (>=0.11.2,<0.12.0) ; extra == "ruamel" or extra == "pyyaml"
+Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "pyyaml"
+Requires-Dist: ruamel-yaml (>=0.17.24,<0.18.0) ; extra == "ruamel"
 Project-URL: Repository, https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher
 Description-Content-Type: text/markdown
 
+[![build](https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher/workflows/build/badge.svg)](https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher/actions?query=workflow%3Abuild+branch%3Amain)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hamqtt-fs_publisher.svg)](https://pypi.org/project/hamqtt-fs_publisher)
+
 # HomeAssistant MQTT filesystem publisher
 
 Publish file content as an MQTT topic compatible with HomeAssistant.
 
 It can be useful, e.g., to publish system metrics from `/sys`.
 
 ## Quick start
 
-1. Install the Python package: `pip install hamqtt-fs-publisher`.
+1. Install the Python package: `pip install hamqtt-fs-publisher`. If you want to
+   have support for YAML configuration format install with `ruamel` or `pyyaml`
+   extras depending on the YAML library of choice (recommended `ruamel`, e.g.,
+   `pip install hamqtt-fs-publisher[ruamel]`).
 2. Create a configuration (example in `examples/config.example.yaml`). It can be
    in either YAML or JSON format. There is a pre-generated JSON schema in
    `hamqtt_fs_publisher/configuration.schema.json`, which can be used, e.g.,
    with VS Code (the current repository is pre-configured for `config.json` and
    `config.yaml`). Remember to set proper authorization details for the MQTT
    broker. If you are using the standard Mosquitto broker add-on in Home
    Assistant, please refer to the [official
```

