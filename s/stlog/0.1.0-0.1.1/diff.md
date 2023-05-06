# Comparing `tmp/stlog-0.1.0.tar.gz` & `tmp/stlog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlog-0.1.0.tar", max compression
+gzip compressed data, was "stlog-0.1.1.tar", max compression
```

## Comparing `stlog-0.1.0.tar` & `stlog-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-05 11:49:10.364241 stlog-0.1.0/LICENSE
--rw-r--r--   0        0        0     8415 2023-05-05 11:49:10.364241 stlog-0.1.0/README.md
--rw-r--r--   0        0        0     1089 2023-05-05 11:49:33.904414 stlog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      593 2023-05-05 11:49:33.548411 stlog-0.1.0/stlog/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/adapter.py
--rw-r--r--   0        0        0     7771 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/base.py
--rw-r--r--   0        0        0     2638 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/context.py
--rw-r--r--   0        0        0    13298 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/formatter.py
--rw-r--r--   0        0        0     2499 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/handler.py
--rw-r--r--   0        0        0     5173 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/kvformatter.py
--rw-r--r--   0        0        0     5109 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/output.py
--rw-r--r--   0        0        0     7070 2023-05-05 11:49:10.368241 stlog-0.1.0/stlog/setup.py
--rw-r--r--   0        0        0     8967 1970-01-01 00:00:00.000000 stlog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 14:19:55.564902 stlog-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8415 2023-05-06 14:19:55.564902 stlog-0.1.1/README.md
+-rw-r--r--   0        0        0     1089 2023-05-06 14:20:16.933072 stlog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      593 2023-05-06 14:20:16.585071 stlog-0.1.1/stlog/__init__.py
+-rw-r--r--   0        0        0     2658 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/adapter.py
+-rw-r--r--   0        0        0     7783 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/base.py
+-rw-r--r--   0        0        0     2638 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/context.py
+-rw-r--r--   0        0        0    14032 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/formatter.py
+-rw-r--r--   0        0        0     2499 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/handler.py
+-rw-r--r--   0        0        0     5276 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/kvformatter.py
+-rw-r--r--   0        0        0     5249 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/output.py
+-rw-r--r--   0        0        0     7077 2023-05-06 14:19:55.568902 stlog-0.1.1/stlog/setup.py
+-rw-r--r--   0        0        0     8967 1970-01-01 00:00:00.000000 stlog-0.1.1/PKG-INFO
```

### Comparing `stlog-0.1.0/LICENSE` & `stlog-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stlog-0.1.0/README.md` & `stlog-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `stlog-0.1.0/pyproject.toml` & `stlog-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stlog"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Fabien MARTY <fabien.marty@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "stlog"}]
 
 [tool.poetry.dependencies]
```

### Comparing `stlog-0.1.0/stlog/__init__.py` & `stlog-0.1.1/stlog/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     "base": False,
     "adapter": False,
     "handler": False,
     "context": False,
     "warn": False,
     "fatal": False,
 }
-VERSION = "0.1.0"
+VERSION = "0.1.1"
```

### Comparing `stlog-0.1.0/stlog/adapter.py` & `stlog-0.1.1/stlog/adapter.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.0/stlog/base.py` & `stlog-0.1.1/stlog/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import inspect
 import json
 import numbers
 import os
 import re
+import string
 import types
 from dataclasses import dataclass, field
 from string import Template
 from typing import Any, Callable, Match
 
 STLOG_EXTRA_KEY = "_stlog_extra"
 RICH_AVAILABLE = False
@@ -18,14 +19,17 @@
     RICH_AVAILABLE = True
 except ImportError:
     pass
 
 
 TRUE_VALUES = ("1", "true", "yes")
 FALSE_VALUES = ("0", "false", "no")
+ALLOWED_CHARS_WITHOUT_LOGFMT_QUOTING: set = set(
+    string.ascii_letters + string.digits + ",-.@_~:"
+)
 
 
 class StlogError(Exception):
     pass
 
 
 @dataclass
@@ -91,20 +95,18 @@
         for key, value in to_check.items():
             if not isinstance(key, str):
                 raise StlogError("dict keys should be str, found %s" % type(key))
             check_json_types_or_raise(value)
 
 
 # Adapted from https://github.com/jteppinette/python-logfmter/blob/main/logfmter/formatter.py
-# FIXME: have a look at golang code to see if the encoding here is enough
-# https://github.com/go-logfmt/logfmt/blob/v0.6.0/encode.go#L236
 def logfmt_format_string(value: str) -> str:
     needs_dquote_escaping = '"' in value
     needs_newline_escaping = "\n" in value
-    needs_quoting = " " in value or "=" in value
+    needs_quoting = not set(value).issubset(ALLOWED_CHARS_WITHOUT_LOGFMT_QUOTING)
     if needs_dquote_escaping:
         value = value.replace('"', '\\"')
     if needs_newline_escaping:
         value = value.replace("\n", "\\n")
     if needs_quoting:
         value = f'"{value}"'
     return value if value else '""'
```

### Comparing `stlog-0.1.0/stlog/context.py` & `stlog-0.1.1/stlog/context.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.0/stlog/formatter.py` & `stlog-0.1.1/stlog/formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,28 +119,29 @@
     @property
     def placeholders_in_fmt(self) -> list[str]:
         if self._placeholders_in_fmt is None:
             self._placeholders_in_fmt = parse_format(self.fmt, self.style)
         return self._placeholders_in_fmt
 
     def _make_extras_string(
-        self,
-        record: logging.LogRecord,
+        self, record: logging.LogRecord, extra_kvs: dict[str, Any] | None = None
     ) -> str:
         if self.kv_formatter is None:
             return ""
         if not hasattr(record, STLOG_EXTRA_KEY):
             return ""
         kvs: dict[str, Any] = {}
         for k in list(getattr(record, STLOG_EXTRA_KEY)) + list(
             self.include_reserved_attrs_in_extras
         ):
             key = self._make_extra_key_name(k)
             if key:
                 kvs[key] = getattr(record, k)
+        if extra_kvs:
+            kvs.update(extra_kvs)
         return self.kv_formatter.format(kvs)
 
     def _make_extra_key_name(self, extra_key: str) -> str | None:
         new_extra_key: str | None = extra_key
         if self.extra_key_rename_fn is not None:
             new_extra_key = (self.extra_key_rename_fn)(extra_key)
         if new_extra_key is None:
@@ -265,32 +266,47 @@
     if key.startswith("_"):
         return key[1:]
     return key
 
 
 @dataclass
 class LogFmtFormatter(Formatter):
+    exc_info_key: str | None = "exc_info"
+    stack_info_key: str | None = "stack_info"
+
     def __post_init__(self):
         if self.kv_formatter is None:
             self.kv_formatter = LogFmtKVFormatter(prefix=" ", suffix="")
         if self.fmt is None:
             self.fmt = DEFAULT_STLOG_LOGFMT_FORMAT
+        if self.extra_key_max_length is None:
+            self.extra_key_max_length = 0
         super().__post_init__()
 
     def format(self, record: logging.LogRecord) -> str:
         record.message = record.getMessage()
         if self.usesTime():
             record.asctime = self.formatTime(record, self.datefmt)
         record_dict: dict[str, Any] = {
             k: logfmt_format_value(getattr(record, k))
             for k in self.placeholders_in_fmt
             if k != "extras"
         }
+        extra_kvs: dict[str, Any] = {}
+        if self.exc_info_key:
+            if record.exc_info:
+                extra_kvs[self.exc_info_key] = self.formatException(record.exc_info)
+            elif record.exc_text:
+                extra_kvs[self.exc_info_key] = record.exc_text
+        if self.stack_info_key and record.stack_info:
+            extra_kvs[self.stack_info_key] = self.formatStack(record.stack_info)
         if "extras" in self.placeholders_in_fmt:
-            record_dict["extras"] = self._make_extras_string(record)
+            record_dict["extras"] = self._make_extras_string(
+                record, extra_kvs=extra_kvs
+            )
         return format_string(self.fmt, self.style, record_dict)
 
 
 @dataclass
 class JsonFormatter(Formatter):
     """Formatter for a JSON / parsing friendly output."""
```

### Comparing `stlog-0.1.0/stlog/handler.py` & `stlog-0.1.1/stlog/handler.py`

 * *Files identical despite different names*

### Comparing `stlog-0.1.0/stlog/kvformatter.py` & `stlog-0.1.1/stlog/kvformatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     """
 
     value_max_serialized_length: int | None = None
 
     def __post_init__(self):
         if self.value_max_serialized_length is None:
-            self.value_max_serialzed_length = 40
+            self.value_max_serialized_length = 40
 
     def _serialize_value(self, v: Any) -> str:
         return _truncate_serialize(
             v,
             self.value_max_serialized_length
             if self.value_max_serialized_length is not None
             else 40,
@@ -133,14 +133,16 @@
 
     """
 
     def __post_init__(self):
         self.separator = " "
         if self.template is None:
             self.template = "{key}={value}"
+        if self.value_max_serialized_length is None:
+            self.value_max_serialized_length = 0
         return super().__post_init__()
 
     def _serialize_value(self, v: Any) -> str:
         return logfmt_format_value(super()._serialize_value(v))
 
 
 @dataclass
```

### Comparing `stlog-0.1.0/stlog/output.py` & `stlog-0.1.1/stlog/output.py`

 * *Files 22% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         self.set_handler(
             logging.StreamHandler(self.stream),
         )
 
 
 @dataclass
 class RichStreamOutput(StreamOutput):
-    force_terminal: bool = True
+    force_terminal: bool = False
     console: typing.Any = None
 
     def __post_init__(self):
         if not RICH_INSTALLED:
             raise StlogError("Rich is not installed and RichStreamOutput is specified")
         if self.formatter is None:
             self.formatter = RichHumanFormatter()
@@ -114,48 +114,54 @@
             )
         self.set_handler(CustomRichHandler(console=self.console))
 
 
 def make_stream_or_rich_stream_output(
     stream: typing.TextIO = sys.stderr,
     use_rich: bool | None = DEFAULT_USE_RICH,
+    formatter_kwargs: dict[str, typing.Any] | None = None,
     **kwargs,
 ) -> StreamOutput:
     """Create automatically a `stlog.output.RichStreamOutput` or a (classic)`stlog.output.StreamOutput`.
 
     To get a `stlog.output.RichStreamOutput`, following conditions must be true:
 
     - `rich` library must be installed and available in python path
     - `use_rich` parameter must be `True` (forced mode) or `None` (automatic mode)
     - (if `use_rich` is `None`): the selected `stream` must "output" in a real terminal (not in a shell filter
     or in a file through redirection...)
 
-    WARNING: if `use_rich` is set to True and if `rich` library is installed, the usage of `rich` library
-    is forced **even if the `rich` library thinks that the output is not "compatible"
-
     NOTE: the default value of the `use_rich` parameter is `None` (automatic) but it can be forced by
     the `STLOG_USE_RICH` env variable.
 
     Attributes:
         stream: the stream to use (`typing.TextIO`), default to `sys.stderr`.
         use_rich: if None, use [rich output](https://github.com/Textualize/rich/blob/master/README.md) if possible
-        (rich installed and supported tty), if True/False force the usage (or not).
+            (rich installed and supported tty), if True/False force the usage (or not).
+        formatter_kwargs: extra parameters for the formatter (can be a `HumanFormatter` or a `RichHumanFormatter`)
 
     """
-    for key in ("formatter", "force_terminal"):
-        if key in kwargs:
-            raise StlogError(f"you can't use {key} in kwargs for this function")
+    if "formatter" in kwargs:
+        raise StlogError(
+            "you can't use formatter in kwargs for this function (buy you can use formatter_kwargs to tune it)"
+        )
     _use_rich: bool = False
     if use_rich is not None:
         # manual mode
         _use_rich = use_rich
     else:
         # automatic mode
         if RICH_INSTALLED:
             c = Console(file=stream)
             _use_rich = c.is_terminal
     if _use_rich:
         return RichStreamOutput(
-            stream=stream, force_terminal=True, formatter=RichHumanFormatter(), **kwargs
+            stream=stream,
+            formatter=RichHumanFormatter(**(formatter_kwargs or {})),
+            **kwargs,
         )
     else:
-        return StreamOutput(stream=stream, **kwargs)
+        return StreamOutput(
+            stream=stream,
+            formatter=HumanFormatter(**(formatter_kwargs or {})),
+            **kwargs,
+        )
```

### Comparing `stlog-0.1.0/stlog/setup.py` & `stlog-0.1.1/stlog/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
             value is read in STLOG_LEVEL env var or set to INFO (if not set).
         outputs: iterable of Output to log to.
         program_name: the name of the program, the default value is read in STLOG_PROGRAM_NAME
             env var or auto-detected if not set.
         capture_warnings: capture warnings from the `warnings` module.
         logging_excepthook: if not None, override sys.excepthook with the given callable
             See https://docs.python.org/3/library/sys.html#sys.excepthook for details.
-        extra_levels: iterable of tuples (logger name, log level) for quick override of
-            the root log level.
+        extra_levels: dict "logger name => log level" for quick override of
+            the root log level (for some loggers).
         reinject_context_in_standard_logging: if True, reinject the LogContext
             in log record emitted with python standard loggers.
         read_extra_kwarg_from_standard_logging: if try to reinject the extra kwargs from standard logging.
     """
     root_logger = logging.getLogger(None)
     if program_name is not None:
         GLOBAL_LOGGING_CONFIG.program_name = program_name
```

### Comparing `stlog-0.1.0/PKG-INFO` & `stlog-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlog
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

