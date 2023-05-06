# Comparing `tmp/sag-py-logging-0.3.1.tar.gz` & `tmp/sag-py-logging-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-logging-0.3.1.tar", last modified: Thu Apr 20 09:27:54 2023, max compression
+gzip compressed data, was "sag-py-logging-0.3.2.tar", last modified: Sat May  6 07:49:28 2023, max compression
```

## Comparing `sag-py-logging-0.3.1.tar` & `sag-py-logging-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.340401 sag-py-logging-0.3.1/sag_py_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/log_config_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.340401 sag-py-logging-0.3.1/sag_py_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_log_config_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/sag_py_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/log_config_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/sag_py_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_log_config_processors.py
```

### Comparing `sag-py-logging-0.3.1/LICENSE.txt` & `sag-py-logging-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/PKG-INFO` & `sag-py-logging-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.1
+Version: 0.3.2
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
```

### Comparing `sag-py-logging-0.3.1/README.md` & `sag-py-logging-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/sag_py_logging/console_extra_field_filter.py` & `sag-py-logging-0.3.2/sag_py_logging/console_extra_field_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import json
 import logging
 from typing import Any, Dict, List, Set
 
 
 class ConsoleExtraFieldFilter(logging.Filter):
     def __init__(self, name: str = "") -> None:
@@ -44,8 +45,17 @@
         record.stringified_extra = ", ".join(extra_list)
         return True
 
     def _get_extra_fields(self, record: logging.LogRecord) -> Dict[str, Any]:
         return {key: value for key, value in record.__dict__.items() if key not in self.excluded_standard_fields}
 
     def _to_key_value_strings(self, extra_fields: Dict[str, Any]) -> List[str]:
-        return [f"{key}={json.dumps(value)}" for key, value in extra_fields.items()]
+        return [f"{key}={self._generate_string_value(value)}" for key, value in extra_fields.items()]
+
+    def _generate_string_value(self, value: Any) -> str:
+        with contextlib.suppress(Exception):
+            return json.dumps(value)
+
+        with contextlib.suppress(Exception):
+            return json.dumps(value.__dict__)
+
+        return str(value)
```

### Comparing `sag-py-logging-0.3.1/sag_py_logging/log_config_initializer.py` & `sag-py-logging-0.3.2/sag_py_logging/log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/sag_py_logging/log_config_loader.py` & `sag-py-logging-0.3.2/sag_py_logging/log_config_loader.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/sag_py_logging/log_config_processors.py` & `sag-py-logging-0.3.2/sag_py_logging/log_config_processors.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/sag_py_logging.egg-info/PKG-INFO` & `sag-py-logging-0.3.2/sag_py_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.1
+Version: 0.3.2
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
```

### Comparing `sag-py-logging-0.3.1/sag_py_logging.egg-info/SOURCES.txt` & `sag-py-logging-0.3.2/sag_py_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/setup.py` & `sag-py-logging-0.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 JINJA_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require jinia" in item]
 TOMLI_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require tomli" in item]
 
 setuptools.setup(
     name="sag-py-logging",
-    version="0.3.1",
+    version="0.3.2",
     description="Initialize logging from a configuration json",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_logging",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-logging-0.3.1/tests/test_console_extra_field_filter.py` & `sag-py-logging-0.3.2/tests/test_console_extra_field_filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from logging import INFO, LogRecord
 from typing import cast
 
 import pytest
 
 from sag_py_logging.console_extra_field_filter import ConsoleExtraFieldFilter
 from sag_py_logging.models import ExtraFieldsLogRecord
+from tests.test_data.extra_data_test_classes import ClassWithoutDict, NotSerializableClass
 
 
 @pytest.fixture()
 def log_record() -> LogRecord:
     return LogRecord(name="", level=INFO, pathname="", lineno=0, msg="Hello, world!", args=(), exc_info=None)
 
 
@@ -24,17 +25,24 @@
 
 
 def test_with_extra_fields(log_record: LogRecord) -> None:
     # Arrange
     filter_ = ConsoleExtraFieldFilter()
     log_record.my_extra_string = "test"
     log_record.my_extra_int = 1
-    log_record.my_extra_object = {"keyOne": "valueOne", "keyTwo": 2}
+    log_record.my_extra_bool = True
+    log_record.my_extra_dict_object = {"keyOne": "valueOne", "keyTwo": 2}
+    log_record.my_extra_not_serializable_object = NotSerializableClass("test")
+    log_record.my_extra_object_without_dict = ClassWithoutDict(x=123, y=456)
 
     # Act
     filter_.filter(log_record)
 
     # Assert
     assert (
-        cast(ExtraFieldsLogRecord, log_record).stringified_extra
-        == 'my_extra_string="test", my_extra_int=1, my_extra_object={"keyOne": "valueOne", "keyTwo": 2}'
+        cast(ExtraFieldsLogRecord, log_record).stringified_extra == 'my_extra_string="test", '
+        "my_extra_int=1, "
+        "my_extra_bool=true, "
+        'my_extra_dict_object={"keyOne": "valueOne", "keyTwo": 2}, '
+        'my_extra_not_serializable_object={"testtext": "test"}, '
+        "my_extra_object_without_dict=ClassWithoutDict(x=123, y=456)"
     )
```

### Comparing `sag-py-logging-0.3.1/tests/test_log_config_initializer.py` & `sag-py-logging-0.3.2/tests/test_log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/tests/test_log_config_loader.py` & `sag-py-logging-0.3.2/tests/test_log_config_loader.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.1/tests/test_log_config_processors.py` & `sag-py-logging-0.3.2/tests/test_log_config_processors.py`

 * *Files identical despite different names*

