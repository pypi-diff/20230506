# Comparing `tmp/hamqtt_fs_publisher-0.1.0.tar.gz` & `tmp/hamqtt_fs_publisher-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamqtt_fs_publisher-0.1.0.tar", max compression
+gzip compressed data, was "hamqtt_fs_publisher-0.1.1.tar", max compression
```

## Comparing `hamqtt_fs_publisher-0.1.0.tar` & `hamqtt_fs_publisher-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-06 12:54:33.031449 hamqtt_fs_publisher-0.1.0/LICENSE
--rw-r--r--   0        0        0     1371 2023-05-06 12:54:33.031449 hamqtt_fs_publisher-0.1.0/README.md
--rw-r--r--   0        0        0       54 2023-05-06 12:54:33.031449 hamqtt_fs_publisher-0.1.0/hamqtt_fs_publisher/__init__.py
--rw-r--r--   0        0        0     4853 2023-05-06 12:54:33.031449 hamqtt_fs_publisher-0.1.0/hamqtt_fs_publisher/__main__.py
--rw-r--r--   0        0        0     3314 2023-05-06 12:54:33.031449 hamqtt_fs_publisher-0.1.0/hamqtt_fs_publisher/configuration.py
--rw-r--r--   0        0        0     9263 2023-05-06 12:54:33.031449 hamqtt_fs_publisher-0.1.0/hamqtt_fs_publisher/configuration.schema.json
--rw-r--r--   0        0        0     1508 2023-05-06 12:54:33.031449 hamqtt_fs_publisher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 hamqtt_fs_publisher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2117 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/README.md
+-rw-r--r--   0        0        0       54 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/__main__.py
+-rw-r--r--   0        0        0     3314 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.py
+-rw-r--r--   0        0        0     9263 2023-05-06 13:25:28.204413 hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.schema.json
+-rw-r--r--   0        0        0     1508 2023-05-06 13:25:28.208413 hamqtt_fs_publisher-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 hamqtt_fs_publisher-0.1.1/PKG-INFO
```

### Comparing `hamqtt_fs_publisher-0.1.0/LICENSE` & `hamqtt_fs_publisher-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hamqtt_fs_publisher-0.1.0/hamqtt_fs_publisher/__main__.py` & `hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,20 +38,19 @@
             '{}: Initialized reader for file "{}".',
             self._log_name,
             entity_config.read_path,
         )
 
     def publish_read(self):
         """Read a value from file and publish it to MQTT broker."""
-        with open(self._config.read_path, encoding="utf-8") as read_file:
-            state = read_file.read()
-            if self._config.read_strip:
-                state = state.strip()
-            logger.debug('{}: Publishing state "{}".', self._log_name, state)
-            self._entity.publish_state(state)
+        state = self._config.read_path.read_text("utf-8")
+        if self._config.read_strip:
+            state = state.strip()
+        logger.debug('{}: Publishing state "{}".', self._log_name, state)
+        self._entity.publish_state(state)
         if not self._stop_event.is_set():
             self.start(False)
 
     def start(self, log: bool = True):
         """Start the periodic reading."""
         if self._stop_event.is_set():
             return
@@ -76,20 +75,37 @@
 
 
 @click.command()
 @click.option(
     "--config",
     "-c",
     default="config.yaml",
-    type=click.Path(exists=True, dir_okay=False, path_type=Path),
+    type=click.Path(dir_okay=False, path_type=Path),
     help="Configuration file (either YAML or JSON).",
 )
 def main(config: Path):
     """Run the HA MQTT filesystem publisher."""
     logger.info("Parsing configuration...")
+    config_found = False
+    config_default_dir = Path("hamqtt_fs_publisher")
+    for prefix in (
+        Path(),
+        Path("/etc") / config_default_dir,
+        Path.home() / ".config" / config_default_dir,
+    ):
+        tried_path = prefix / config
+        if tried_path.exists() and not tried_path.is_dir():
+            config_found = True
+            config = tried_path
+            logger.debug('Found configuration in "{}".', config)
+            break
+
+    if not config_found:
+        logger.error('Configuration not found at "{}" path.', config)
+
     config_parsed = Config.parse_file(config)
 
     logger.info("Connecting to MQTT broker...")
     mqtt_config = config_parsed.mqtt
     client = Client(mqtt_config.client_id)
     if mqtt_config.user is not None:
         client.username_pw_set(mqtt_config.user, mqtt_config.password)
```

### Comparing `hamqtt_fs_publisher-0.1.0/hamqtt_fs_publisher/configuration.py` & `hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.py`

 * *Files identical despite different names*

### Comparing `hamqtt_fs_publisher-0.1.0/hamqtt_fs_publisher/configuration.schema.json` & `hamqtt_fs_publisher-0.1.1/hamqtt_fs_publisher/configuration.schema.json`

 * *Files identical despite different names*

### Comparing `hamqtt_fs_publisher-0.1.0/pyproject.toml` & `hamqtt_fs_publisher-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hamqtt-fs-publisher"
-version = "0.1.0"
+version = "0.1.1"
 description = "Publish file content as MQTT topic compatible with HomeAssistant."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent",
```

### Comparing `hamqtt_fs_publisher-0.1.0/PKG-INFO` & `hamqtt_fs_publisher-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamqtt-fs-publisher
-Version: 0.1.0
+Version: 0.1.1
 Summary: Publish file content as MQTT topic compatible with HomeAssistant.
 Home-page: https://github.com/MarekPikula/homeassistant-mqtt-filesystem-publisher
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
@@ -30,24 +30,44 @@
 Publish file content as an MQTT topic compatible with HomeAssistant.
 
 It can be useful, e.g., to publish system metrics from `/sys`.
 
 ## Quick start
 
 1. Install the Python package: `pip install hamqtt-fs-publisher`.
-2. Create a configuration (example in `config.example.yaml`). It can be either
-   YAML or JSON. There is a pre-generated JSON schema in
+2. Create a configuration (example in `examples/config.example.yaml`). It can be
+   in either YAML or JSON format. There is a pre-generated JSON schema in
    `hamqtt_fs_publisher/configuration.schema.json`, which can be used, e.g.,
    with VS Code (the current repository is pre-configured for `config.json` and
    `config.yaml`). Remember to set proper authorization details for the MQTT
    broker. If you are using the standard Mosquitto broker add-on in Home
    Assistant, please refer to the [official
    documentation](https://github.com/home-assistant/addons/blob/master/mosquitto/DOCS.md).
 3. Run `hamqtt_fs_publisher --config <config_file_name>`.
 
+> **Note:** The configuration file path could be either a relative/absolute
+> path, or a file under `/etc/hamqtt_fs_publisher` or
+> `~/.config/hamqtt_fs_publisher`.
+
+## Systemd service
+
+If you want to run this script as a systemd service you could copy the example
+service file from `examples/hamqtt_fs_publisher@.service` to either
+`/etc/systemd/system/` or `~/.config/systemd/user/` (if you want to run it in
+user mode). Then copy the configuration file to one of the standard
+configuration directories (i.e., `/etc/hamqtt_fs_publisher` or
+`~/.config/hamqtt_fs_publisher`.)
+
+To enable and start the unit in system mode run:
+
+```shell
+$ systemd daemon-reload
+$ systemd enable --now hamqtt_fs_publisher@<config_file_name>
+```
+
 ## Supported features
 
 - Auto-discovery in HomeAssistant.
 - Configuration with a simple YAML/JSON file.
 - Possibility to create read-only sensor device entities with values taken
   from a file and published to the MQTT broker periodically with set intervals.
```

