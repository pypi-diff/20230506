# Comparing `tmp/ExcelAlchemy-0.1a2.tar.gz` & `tmp/ExcelAlchemy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExcelAlchemy-0.1a2.tar", last modified: Fri Feb 24 08:15:39 2023, max compression
+gzip compressed data, was "ExcelAlchemy-1.0.0.tar", last modified: Sat May  6 02:07:47 2023, max compression
```

## Comparing `ExcelAlchemy-0.1a2.tar` & `ExcelAlchemy-1.0.0.tar`

### file list

```diff
@@ -1,46 +1,40 @@
--rw-r--r--   0        0        0     3187 2023-02-24 06:02:05.822738 ExcelAlchemy-0.1a2/.gitignore
--rw-r--r--   0        0        0     1456 2023-02-24 06:30:51.166309 ExcelAlchemy-0.1a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-02-24 06:02:05.822930 ExcelAlchemy-0.1a2/LICENSE
--rwxr-xr-x   0        0        0     2296 2023-02-24 06:02:05.823013 ExcelAlchemy-0.1a2/README.md
--rw-r--r--   0        0        0     3233 2023-02-24 08:15:38.653220 ExcelAlchemy-0.1a2/excelalchemy/__init__.py
--rw-r--r--   0        0        0     1333 2023-02-24 06:30:51.072371 ExcelAlchemy-0.1a2/excelalchemy/abstract.py
--rw-r--r--   0        0        0    35181 2023-02-24 06:30:51.174113 ExcelAlchemy-0.1a2/excelalchemy/alchemy.py
--rw-r--r--   0        0        0     1419 2023-02-24 06:30:51.105497 ExcelAlchemy-0.1a2/excelalchemy/const.py
--rw-r--r--   0        0        0     1927 2023-02-24 06:30:51.063495 ExcelAlchemy-0.1a2/excelalchemy/exception.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.823675 ExcelAlchemy-0.1a2/excelalchemy/helper/__init__.py
--rw-r--r--   0        0        0     7335 2023-02-24 06:30:51.087128 ExcelAlchemy-0.1a2/excelalchemy/helper/pydantic.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.823849 ExcelAlchemy-0.1a2/excelalchemy/model/__init__.py
--rw-r--r--   0        0        0    18460 2023-02-24 06:30:51.170856 ExcelAlchemy-0.1a2/excelalchemy/model/abstract.py
--rw-r--r--   0        0        0     5751 2023-02-24 06:30:51.093398 ExcelAlchemy-0.1a2/excelalchemy/model/excel.py
--rw-r--r--   0        0        0      456 2023-02-24 06:02:05.824152 ExcelAlchemy-0.1a2/excelalchemy/model/identity.py
--rw-r--r--   0        0        0     2433 2023-02-24 06:30:51.183138 ExcelAlchemy-0.1a2/excelalchemy/model/result.py
--rw-r--r--   0        0        0      278 2023-02-24 06:30:51.097098 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/__init__.py
--rw-r--r--   0        0        0     2021 2023-02-24 06:30:51.188212 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/boolean.py
--rw-r--r--   0        0        0     4012 2023-02-24 06:30:51.161662 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date.py
--rw-r--r--   0        0        0     6009 2023-02-24 06:30:51.129907 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date_range.py
--rw-r--r--   0        0        0      585 2023-02-24 06:30:51.077370 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/email.py
--rw-r--r--   0        0        0      335 2023-02-24 06:30:51.178048 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/money.py
--rw-r--r--   0        0        0     3284 2023-02-24 06:30:51.146249 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/multi_checkbox.py
--rw-r--r--   0        0        0     4363 2023-02-24 06:30:51.079918 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/number.py
--rw-r--r--   0        0        0     4758 2023-02-24 06:30:51.155194 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/number_range.py
--rw-r--r--   0        0        0     2811 2023-02-24 06:30:51.157636 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/organization.py
--rw-r--r--   0        0        0      614 2023-02-24 06:30:51.163555 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/phone_number.py
--rw-r--r--   0        0        0     2578 2023-02-24 06:30:51.095292 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/radio.py
--rw-r--r--   0        0        0     2955 2023-02-24 06:30:51.065628 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/staff.py
--rw-r--r--   0        0        0     4947 2023-02-24 06:30:51.089259 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/string.py
--rw-r--r--   0        0        0     2975 2023-02-24 06:30:51.113232 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/tree.py
--rw-r--r--   0        0        0      773 2023-02-24 06:30:51.074855 ExcelAlchemy-0.1a2/excelalchemy/model/value_type/url.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825504 ExcelAlchemy-0.1a2/excelalchemy/plugin/__init__.py
--rw-r--r--   0        0        0      576 2023-02-24 06:30:51.082414 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/__init__.py
--rw-r--r--   0        0        0     4113 2023-02-24 06:30:51.127323 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/builder.py
--rw-r--r--   0        0        0     5070 2023-02-24 06:30:51.085015 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/config.py
--rw-r--r--   0        0        0    12752 2023-02-24 06:30:51.056689 ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/screen.py
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825884 ExcelAlchemy-0.1a2/excelalchemy/py.typed
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.825956 ExcelAlchemy-0.1a2/excelalchemy/tool/__init__.py
--rw-r--r--   0        0        0     1470 2023-02-24 06:30:51.124528 ExcelAlchemy-0.1a2/excelalchemy/tool/convertor.py
--rw-r--r--   0        0        0     2736 2023-02-24 06:30:51.159637 ExcelAlchemy-0.1a2/excelalchemy/util.py
--rw-r--r--   0        0        0    16607 2023-02-24 06:30:51.110554 ExcelAlchemy-0.1a2/excelalchemy/writer.py
--rw-r--r--   0        0        0     2332 2023-02-24 08:15:23.458018 ExcelAlchemy-0.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-24 06:02:05.826382 ExcelAlchemy-0.1a2/tests/__init__.py
--rw-r--r--   0        0        0     6470 2023-02-24 06:30:51.103701 ExcelAlchemy-0.1a2/tests/test_alchemy.py
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 ExcelAlchemy-0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     6282 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/README.md
+-rw-r--r--   0        0        0     3182 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/__init__.py
+-rw-r--r--   0        0        0     3199 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/const.py
+-rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/__init__.py
+-rw-r--r--   0        0        0     1674 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/abstract.py
+-rw-r--r--   0        0        0    37296 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/alchemy.py
+-rw-r--r--   0        0        0    18140 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/writer.py
+-rw-r--r--   0        0        0     2067 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/exc.py
+-rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/helper/__init__.py
+-rw-r--r--   0        0        0     7334 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/helper/pydantic.py
+-rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/py.typed
+-rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/__init__.py
+-rw-r--r--   0        0        0     3724 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/abstract.py
+-rw-r--r--   0        0        0     4790 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/alchemy.py
+-rw-r--r--   0        0        0    15756 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/field.py
+-rw-r--r--   0        0        0      941 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/header.py
+-rw-r--r--   0        0        0      546 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/identity.py
+-rw-r--r--   0        0        0     2676 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/result.py
+-rw-r--r--   0        0        0      377 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/__init__.py
+-rw-r--r--   0        0        0     1703 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/boolean.py
+-rw-r--r--   0        0        0     3997 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/date.py
+-rw-r--r--   0        0        0     6463 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/date_range.py
+-rw-r--r--   0        0        0      748 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/email.py
+-rw-r--r--   0        0        0      341 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/money.py
+-rw-r--r--   0        0        0     2724 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/multi_checkbox.py
+-rw-r--r--   0        0        0     5335 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/number.py
+-rw-r--r--   0        0        0     4203 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/number_range.py
+-rw-r--r--   0        0        0     2440 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/organization.py
+-rw-r--r--   0        0        0      498 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/phone_number.py
+-rw-r--r--   0        0        0     2262 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/radio.py
+-rw-r--r--   0        0        0     2547 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/staff.py
+-rw-r--r--   0        0        0     4898 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/string.py
+-rw-r--r--   0        0        0     1914 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/tree.py
+-rw-r--r--   0        0        0      659 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/url.py
+-rw-r--r--   0        0        0        0 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/util/__init__.py
+-rw-r--r--   0        0        0     1557 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/util/convertor.py
+-rw-r--r--   0        0        0     2736 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/util/file.py
+-rw-r--r--   0        0        0     2487 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7315 1970-01-01 00:00:00.000000 ExcelAlchemy-1.0.0/PKG-INFO
```

### Comparing `ExcelAlchemy-0.1a2/LICENSE` & `ExcelAlchemy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/__init__.py` & `ExcelAlchemy-1.0.0/excelalchemy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-"""ExcelAlchemy, a Python library for reading and writing Excel files."""
-# pre-alpha
-__version__ = '0.1a2'
+"""A Python Library for Reading and Writing Excel Files"""
 
-from excelalchemy.alchemy import ExcelAlchemy
-from excelalchemy.exception import ExcelCellError
-from excelalchemy.exception import ProgrammaticError
-from excelalchemy.model.abstract import CharacterSet
-from excelalchemy.model.abstract import DataRangeOption
-from excelalchemy.model.abstract import DateFormat
-from excelalchemy.model.abstract import FieldMeta
-from excelalchemy.model.abstract import Option
-from excelalchemy.model.abstract import PatchFieldMeta
-from excelalchemy.model.excel import ExcelExporterConfig
-from excelalchemy.model.excel import ExcelImporterConfig
-from excelalchemy.model.excel import ImportMode
-from excelalchemy.model.identity import ColumnIndex
-from excelalchemy.model.identity import Key
-from excelalchemy.model.identity import Label
-from excelalchemy.model.identity import OptionId
-from excelalchemy.model.identity import RowIndex
-from excelalchemy.model.identity import UniqueKey
-from excelalchemy.model.identity import UniqueLabel
-from excelalchemy.model.result import ImportDataResult
-from excelalchemy.model.result import ImportExcelResult
-from excelalchemy.model.result import ImportRowResult
-from excelalchemy.model.result import ValidateHeaderResult
-from excelalchemy.model.value_type.boolean import Boolean
-from excelalchemy.model.value_type.date import Date
-from excelalchemy.model.value_type.date_range import DateRange
-from excelalchemy.model.value_type.email import Email
-from excelalchemy.model.value_type.money import Money
-from excelalchemy.model.value_type.multi_checkbox import MultiCheckbox
-from excelalchemy.model.value_type.number import Number
-from excelalchemy.model.value_type.number_range import NumberRange
-from excelalchemy.model.value_type.organization import MultiOrganization
-from excelalchemy.model.value_type.organization import SingleOrganization
-from excelalchemy.model.value_type.phone_number import PhoneNumber
-from excelalchemy.model.value_type.radio import Radio
-from excelalchemy.model.value_type.staff import MultiStaff
-from excelalchemy.model.value_type.staff import SingleStaff
-from excelalchemy.model.value_type.string import String
-from excelalchemy.model.value_type.tree import MultiTreeNode
-from excelalchemy.model.value_type.tree import SingleTreeNode
-from excelalchemy.model.value_type.url import Url
-from excelalchemy.util import flatten
+__version__ = '1.0.0'
+from excelalchemy.const import CharacterSet
+from excelalchemy.const import DataRangeOption
+from excelalchemy.const import DateFormat
+from excelalchemy.const import Option
+from excelalchemy.core.alchemy import ExcelAlchemy
+from excelalchemy.exc import ConfigError
+from excelalchemy.exc import ExcelCellError
+from excelalchemy.exc import ProgrammaticError
+from excelalchemy.helper.pydantic import extract_pydantic_model
+from excelalchemy.types.alchemy import ExporterConfig
+from excelalchemy.types.alchemy import ImporterConfig
+from excelalchemy.types.alchemy import ImportMode
+from excelalchemy.types.field import FieldMeta
+from excelalchemy.types.field import PatchFieldMeta
+from excelalchemy.types.identity import ColumnIndex
+from excelalchemy.types.identity import Key
+from excelalchemy.types.identity import Label
+from excelalchemy.types.identity import OptionId
+from excelalchemy.types.identity import RowIndex
+from excelalchemy.types.identity import UniqueKey
+from excelalchemy.types.identity import UniqueLabel
+from excelalchemy.types.result import ImportResult
+from excelalchemy.types.result import ValidateHeaderResult
+from excelalchemy.types.result import ValidateResult
+from excelalchemy.types.result import ValidateRowResult
+from excelalchemy.types.value.boolean import Boolean
+from excelalchemy.types.value.date import Date
+from excelalchemy.types.value.date_range import DateRange
+from excelalchemy.types.value.email import Email
+from excelalchemy.types.value.money import Money
+from excelalchemy.types.value.multi_checkbox import MultiCheckbox
+from excelalchemy.types.value.number import Number
+from excelalchemy.types.value.number_range import NumberRange
+from excelalchemy.types.value.organization import MultiOrganization
+from excelalchemy.types.value.organization import SingleOrganization
+from excelalchemy.types.value.phone_number import PhoneNumber
+from excelalchemy.types.value.radio import Radio
+from excelalchemy.types.value.staff import MultiStaff
+from excelalchemy.types.value.staff import SingleStaff
+from excelalchemy.types.value.string import String
+from excelalchemy.types.value.tree import MultiTreeNode
+from excelalchemy.types.value.tree import SingleTreeNode
+from excelalchemy.types.value.url import Url
+from excelalchemy.util.file import flatten
 
 __all__ = [
+    'Boolean',
+    'ColumnIndex',
+    'Date',
+    'DateFormat',
+    'DateRange',
+    'DataRangeOption',
+    'Email',
     'ExcelAlchemy',
     'ExcelCellError',
-    'ProgrammaticError',
-    'CharacterSet',
-    'DataRangeOption',
-    'DateFormat',
+    'ExporterConfig',
     'FieldMeta',
-    'Option',
-    'PatchFieldMeta',
-    'ExcelExporterConfig',
-    'ExcelImporterConfig',
     'ImportMode',
-    'ColumnIndex',
+    'ImportResult',
+    'ImporterConfig',
     'Key',
     'Label',
-    'OptionId',
-    'RowIndex',
-    'UniqueKey',
-    'UniqueLabel',
-    'ImportDataResult',
-    'ImportExcelResult',
-    'ImportRowResult',
-    'ValidateHeaderResult',
-    'Boolean',
-    'Date',
-    'DateRange',
-    'Email',
     'Money',
     'MultiCheckbox',
+    'MultiOrganization',
+    'MultiStaff',
+    'MultiTreeNode',
     'Number',
     'NumberRange',
-    'MultiOrganization',
-    'SingleOrganization',
+    'Option',
+    'OptionId',
+    'PatchFieldMeta',
     'PhoneNumber',
+    'ProgrammaticError',
+    'ConfigError',
     'Radio',
-    'MultiStaff',
+    'RowIndex',
+    'SingleOrganization',
     'SingleStaff',
+    'SingleTreeNode',
     'String',
+    'UniqueKey',
+    'UniqueLabel',
     'Url',
+    'ValidateHeaderResult',
+    'ValidateResult',
+    'ValidateRowResult',
+    'extract_pydantic_model',
     'flatten',
-    'SingleTreeNode',
-    'MultiTreeNode',
 ]
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/abstract.py` & `ExcelAlchemy-1.0.0/excelalchemy/core/abstract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 from abc import ABC
 from abc import abstractmethod
 from typing import Any
 from typing import Generic
 
-from excelalchemy.model.abstract import ContextT
-from excelalchemy.model.abstract import ExcelConfigT
-from excelalchemy.model.identity import Base64Str
-from excelalchemy.model.identity import Key
-from excelalchemy.model.result import ImportDataResult
-
-
-class ABCExcelAlchemy(ABC, Generic[ContextT, ExcelConfigT]):
+from excelalchemy.const import ContextT
+from excelalchemy.const import CreateModelT
+from excelalchemy.const import ExporterModelT
+from excelalchemy.const import ImporterCreateModelT
+from excelalchemy.const import ImporterUpdateModelT
+from excelalchemy.const import UpdateModelT
+from excelalchemy.types.identity import Base64Str
+from excelalchemy.types.identity import Key
+from excelalchemy.types.identity import UrlStr
+from excelalchemy.types.result import ImportResult
+
+
+class ABCExcelAlchemy(
+    ABC,
+    Generic[
+        ContextT,
+        ImporterCreateModelT,
+        ImporterUpdateModelT,
+        CreateModelT,
+        UpdateModelT,
+        ExporterModelT,
+    ],
+):
     @abstractmethod
     def download_template(self, sample_data: list[dict[str, Any]] | None = None) -> str:
         """下载导入模版, Excel 字段顺序与定义的导出模型一致"""
 
     @abstractmethod
-    async def import_data(self, input_excel_name: str, output_excel_name: str) -> ImportDataResult:
+    async def import_data(self, input_excel_name: str, output_excel_name: str) -> ImportResult:
         """导入数据"""
 
     @abstractmethod
-    def export_excel(self, output_excel_name: str, data: list[dict[str, Any]], keys: list[Key] | None = None) -> bool:
-        """导出数据, 自动将文件上传到 Minio，字段顺序与定义的导出模型一致"""
+    def export(self, data: list[dict[str, Any]], keys: list[Key] | None = None) -> Base64Str:
+        """导出数据，返回 base64 编码的 excel 文件, 字段顺序与定义的导出模型一致"""
 
     @abstractmethod
-    def export_excel_data(self, data: list[dict[str, Any]], keys: list[Key] | None = None) -> Base64Str:
-        """导出数据，返回 base64 编码的 excel 文件, 字段顺序与定义的导出模型一致"""
+    def export_upload(self, output_name: str, data: list[dict[str, Any]], keys: list[Key] | None = None) -> UrlStr:
+        """导出数据, 自动将文件上传到 Minio，字段顺序与定义的导出模型一致"""
 
     @abstractmethod
     def add_context(self, context: ContextT):
         """添加上下文"""
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/alchemy.py` & `ExcelAlchemy-1.0.0/excelalchemy/core/alchemy.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,81 +6,103 @@
 from itertools import chain
 from os import PathLike
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Generator
 from typing import Iterable
+from typing import Type
 from typing import cast
 
 import pandas
 from pandas import DataFrame
 from pandas import concat
 from pydantic import BaseModel
 
-from excelalchemy.abstract import ABCExcelAlchemy
 from excelalchemy.const import DEFAULT_FIELD_META_ORDER
 from excelalchemy.const import REASON_COLUMN_KEY
 from excelalchemy.const import REASON_COLUMN_LABEL
 from excelalchemy.const import RESULT_COLUMN_KEY
 from excelalchemy.const import RESULT_COLUMN_LABEL
-from excelalchemy.exception import ExcelCellError
-from excelalchemy.exception import ExcelRowError
+from excelalchemy.const import ContextT
+from excelalchemy.const import CreateModelT
+from excelalchemy.const import ExporterModelT
+from excelalchemy.const import ImporterCreateModelT
+from excelalchemy.const import ImporterUpdateModelT
+from excelalchemy.const import UpdateModelT
+from excelalchemy.core.abstract import ABCExcelAlchemy
+from excelalchemy.core.writer import render_data_excel
+from excelalchemy.core.writer import render_merged_header_excel
+from excelalchemy.core.writer import render_simple_header_excel
+from excelalchemy.exc import ConfigError
+from excelalchemy.exc import ExcelCellError
+from excelalchemy.exc import ExcelRowError
 from excelalchemy.helper.pydantic import extract_pydantic_model
 from excelalchemy.helper.pydantic import instantiate_pydantic_model
-from excelalchemy.model.abstract import ContextT
-from excelalchemy.model.abstract import ExcelConfigT
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.abstract import SystemReservedValueType
-from excelalchemy.model.excel import ExcelExporterConfig
-from excelalchemy.model.excel import ExcelHeader
-from excelalchemy.model.excel import ExcelImporterConfig
-from excelalchemy.model.excel import ExcelMode
-from excelalchemy.model.excel import ImportMode
-from excelalchemy.model.identity import Base64Str
-from excelalchemy.model.identity import ColumnIndex
-from excelalchemy.model.identity import Key
-from excelalchemy.model.identity import Label
-from excelalchemy.model.identity import RowIndex
-from excelalchemy.model.identity import UniqueKey
-from excelalchemy.model.identity import UniqueLabel
-from excelalchemy.model.result import ImportDataResult
-from excelalchemy.model.result import ImportExcelResult
-from excelalchemy.model.result import ImportRowResult
-from excelalchemy.model.result import ValidateHeaderResult
-from excelalchemy.util import flatten
-from excelalchemy.util import read_file_from_minio_object
-from excelalchemy.util import remove_excel_prefix
-from excelalchemy.util import upload_file_from_minio_object
-from excelalchemy.writer import render_data_excel
-from excelalchemy.writer import render_merged_header_excel
-from excelalchemy.writer import render_simple_header_excel
+from excelalchemy.types.abstract import SystemReserved
+from excelalchemy.types.alchemy import ExcelMode
+from excelalchemy.types.alchemy import ExporterConfig
+from excelalchemy.types.alchemy import ImporterConfig
+from excelalchemy.types.alchemy import ImportMode
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.header import ExcelHeader
+from excelalchemy.types.identity import Base64Str
+from excelalchemy.types.identity import ColumnIndex
+from excelalchemy.types.identity import Key
+from excelalchemy.types.identity import Label
+from excelalchemy.types.identity import RowIndex
+from excelalchemy.types.identity import UniqueKey
+from excelalchemy.types.identity import UniqueLabel
+from excelalchemy.types.identity import UrlStr
+from excelalchemy.types.result import ImportResult
+from excelalchemy.types.result import ValidateHeaderResult
+from excelalchemy.types.result import ValidateResult
+from excelalchemy.types.result import ValidateRowResult
+from excelalchemy.util.file import flatten
+from excelalchemy.util.file import read_file_from_minio_object
+from excelalchemy.util.file import remove_excel_prefix
+from excelalchemy.util.file import upload_file_from_minio_object
 
 HEADER_HINT_LINE_COUNT = 1  # HEADER_HINT 占用的行数
 
 # 导入结果的字段元数据, 依据产品定义，占两列
 # 1. 导入结果结果列
 RESULT_COLUMN = FieldMetaInfo(label=RESULT_COLUMN_LABEL)
 RESULT_COLUMN.parent_label = RESULT_COLUMN.label
 RESULT_COLUMN.key = RESULT_COLUMN.parent_key = RESULT_COLUMN_KEY
-RESULT_COLUMN.value_type = SystemReservedValueType
+RESULT_COLUMN.value_type = SystemReserved
 
 # 2. 导入结果错误信息列
 REASON_COLUMN = FieldMetaInfo(label=REASON_COLUMN_LABEL)
 REASON_COLUMN.parent_label = REASON_COLUMN.label
 REASON_COLUMN.key = REASON_COLUMN.parent_key = REASON_COLUMN_KEY
-REASON_COLUMN.value_type = SystemReservedValueType
+REASON_COLUMN.value_type = SystemReserved
 
 
-class ExcelAlchemy(ABCExcelAlchemy[ContextT, ExcelConfigT]):
-    def __init__(self, config: ExcelConfigT):
-
+class ExcelAlchemy(
+    ABCExcelAlchemy[
+        ContextT,
+        ImporterCreateModelT,
+        ImporterUpdateModelT,
+        CreateModelT,
+        UpdateModelT,
+        ExporterModelT,
+    ],
+):
+    def __init__(
+        self,
+        config: ImporterConfig[ContextT, ImporterCreateModelT, ImporterUpdateModelT] | ExporterConfig[ExporterModelT],
+    ):
         self.df = DataFrame()  # 初始化一个空的DataFrame
         self.header_df = DataFrame()  # 初始化一个空的DataFrame
-        self.config: ExcelConfigT = config
+        self.config: ImporterConfig[
+            ContextT,
+            ImporterCreateModelT,
+            ImporterUpdateModelT,
+        ] | ExporterConfig[ExporterModelT] = config
         # 每个单元格的错误, 用于标红单元格, 索引与 df 位置对应
         self.cell_errors: dict[RowIndex, dict[ColumnIndex, list[ExcelCellError]]] = {}
         # 行错误, 用于标记错误信息，单元格错误会在行错误中显示，行标索引与 df 位置对应
         self.row_errors: dict[RowIndex, list[ExcelRowError | ExcelCellError]] = defaultdict(list)
         # 固定的两列作为结果列
         self.import_result_field_meta: list[FieldMetaInfo] = [RESULT_COLUMN, REASON_COLUMN]
         self.import_result_label_to_field_meta: dict[UniqueLabel, FieldMetaInfo] = {  # 在导出验证结果时，补充结果列
@@ -101,82 +123,91 @@
         self.__state_df_has_been_loaded__ = False  # df 是否已经被加载
 
         # 初始化·最后调用
         self.__init_from_config__()
 
     def __init_from_config__(self) -> None:
         """从配置类初始化"""
+        self.context = getattr(self.config, 'context', None)
+        importer_model = self.__get_importer_model__()
+        self.__init_field_meta__(importer_model)
 
-        if self.excel_mode == ExcelMode.IMPORT:
-            if not isinstance(self.config, ExcelImporterConfig):
-                raise TypeError('导入模式的配置类必须是 ImportExcelConfig')
-            self.context = self.config.context
-            if self.config.import_mode in (ImportMode.CREATE, ImportMode.CREATE_OR_UPDATE):
-                config_importer_model = self.config.create_importer_model
-            elif self.config.import_mode == ImportMode.UPDATE:
-                config_importer_model = self.config.update_importer_model
-            else:
-                raise RuntimeError('不支持的导入模式')
-        elif self.excel_mode == ExcelMode.EXPORT:
-            if not isinstance(self.config, ExcelExporterConfig):
-                raise TypeError('导出模式的配置类必须是 ExportExcelConfig')
-            config_importer_model = self.config.exporter_model
-        else:
-            raise RuntimeError('不支持的模式')
-
-        self.field_metas = extract_pydantic_model(config_importer_model)
+    def __init_field_meta__(self, importer_model: type[BaseModel]) -> None:
+        """从配置类初始化"""
+        self.field_metas = extract_pydantic_model(importer_model)
         self._check_field_meta_order(self.field_metas)
         if len(self.field_metas) == 0:
-            raise RuntimeError(f'没有从模型 {config_importer_model} 中提取到字段元数据，请检查模型是否定义了字段')
+            raise ConfigError(f'没有从模型 {importer_model} 中提取到字段元数据，请检查模型是否定义了字段')
         self.ordered_field_meta: list[FieldMetaInfo] = self._sort_field_meta(self.field_metas)  # type: ignore[no-redef]
 
         for field_meta in self.ordered_field_meta:
             if field_meta.parent_label is None:
-                raise RuntimeError('父标签不能为空')
+                raise ConfigError('父标签不能为空')
             if field_meta.parent_key is None:
-                raise RuntimeError('父键不能为空')
+                raise ConfigError('父键不能为空')
 
             self.parent_label_to_field_metas.setdefault(field_meta.parent_label, []).append(field_meta)
             self.parent_key_to_field_metas.setdefault(field_meta.parent_key, []).append(field_meta)
             self.unique_key_to_field_meta[field_meta.unique_key] = field_meta
             self.unique_label_to_field_meta[field_meta.unique_label] = field_meta
 
+    def __get_importer_model__(self) -> type[ImporterCreateModelT] | type[ImporterUpdateModelT] | type[ExporterModelT]:
+        if self.excel_mode == ExcelMode.IMPORT:
+            if not isinstance(self.config, ImporterConfig):
+                raise TypeError(f'导入模式的配置类必须是 {ImporterConfig.__name__}')
+            if self.config.import_mode in (ImportMode.CREATE, ImportMode.CREATE_OR_UPDATE):
+                importer_model = self.config.create_importer_model  # type: ignore[assignment]
+            elif self.config.import_mode == ImportMode.UPDATE:
+                importer_model = self.config.update_importer_model  # type: ignore[assignment]
+            else:
+                raise ConfigError('不支持的导入模式')
+
+        elif self.excel_mode == ExcelMode.EXPORT:
+            if not isinstance(self.config, ExporterConfig):
+                raise TypeError(f'导出模式的配置类必须是 {ExporterConfig.__name__}')
+            importer_model = self.config.exporter_model  # type: ignore[assignment]
+
+        else:
+            raise ConfigError('不支持的模式')
+
+        return importer_model  # type: ignore
+
     @staticmethod
     def _check_field_meta_order(field_metas: list[FieldMetaInfo]) -> None:
         """检查字段顺序是否有重复"""
         order_to_field_meta: dict[int, set[Label]] = defaultdict(set)
         for field_meta in field_metas:
             assert field_meta.parent_label is not None  # only for mypy, remove this line at runtime if you want
             order_to_field_meta[field_meta.order].add(field_meta.parent_label)
         duplicate_order = [v for k, v in order_to_field_meta.items() if len(v) > 1 and k != DEFAULT_FIELD_META_ORDER]
         if duplicate_order:
-            raise RuntimeError(f'字段顺序定义有重复：{list( itertools.chain.from_iterable(duplicate_order))}')
+            raise ConfigError(f'字段顺序定义有重复：{list(itertools.chain.from_iterable(duplicate_order))}')
 
     def download_template(self, sample_data: list[dict[str, Any]] | None = None) -> str:
         """下载导入模版"""
         if self.excel_mode != ExcelMode.IMPORT:
-            raise RuntimeError('只支持导入模式调用此方法')
+            raise ConfigError('只支持导入模式调用此方法')
         keys = self._select_output_excel_keys()
         has_merged_header = self.has_merged_header(keys)
         if has_merged_header:
             df = self._export_with_merged_header(sample_data, keys)
             return render_merged_header_excel(df, self.unique_label_to_field_meta)
         else:
             df = self._export_with_simple_header(sample_data, keys)
             return render_simple_header_excel(df, self.unique_label_to_field_meta)
 
-    async def import_data(self, input_excel_name: str, output_excel_name: str) -> ImportDataResult:
+    async def import_data(self, input_excel_name: str, output_excel_name: str) -> ImportResult:
         """导入数据"""
-        assert isinstance(self.config, ExcelImporterConfig)  # only for type check
+        assert isinstance(self.config, ImporterConfig)  # only for type check
         if self.excel_mode != ExcelMode.IMPORT:
-            raise RuntimeError('只支持导入模式调用此方法')
+            raise ConfigError('只支持导入模式调用此方法')
 
         validate_header = self._validate_header(input_excel_name)  # 验证表头
         if not validate_header.is_valid:
-            return ImportDataResult.from_validate_header_result(validate_header)
+            return ImportResult.from_validate_header_result(validate_header)
 
         self.df = self.df.iloc[1:]  # 去掉表头
         self._set_columns(self.df)  # pyright: reportGeneralTypeIssues=false
         self.df = self.df.reset_index(drop=True)  # 重置索引
 
         all_success, success_count, fail_count = True, 0, 0
         for pandas_row_index, row in self.df.iloc[self.extra_header_count_on_import :].iterrows():
@@ -186,95 +217,90 @@
             success_count, fail_count = (success_count + 1, fail_count) if success else (success_count, fail_count + 1)
 
         url = None
         if not all_success:
             self._add_result_column()
             content_with_prefix = self._render_import_result_excel()
             url = self._upload_file(output_excel_name, content_with_prefix)
-        return ImportDataResult(
-            result=(ImportExcelResult.DATA_INVALID, ImportExcelResult.SUCCESS)[int(all_success)],
+        return ImportResult(
+            result=(ValidateResult.DATA_INVALID, ValidateResult.SUCCESS)[int(all_success)],
             url=url,
             success_count=success_count,
             fail_count=fail_count,
         )
 
-    def export_excel_data(self, data: list[dict[str, Any]], keys: list[Key] | None = None) -> Base64Str:
+    def export(self, data: list[dict[str, Any]], keys: list[Key] | None = None) -> Base64Str:
         """导出数据, keys 控制导出的列, 如果为 None, [] 则导出所有列"""
-        assert isinstance(self.config, ExcelExporterConfig)  # only for type check
-
-        if self.excel_mode != ExcelMode.EXPORT:
-            raise RuntimeError('只支持导出模式调用此方法')
-        input_keys = keys or [x.unique_key for x in self.ordered_field_meta]
-        model_keys = cast(list[Key], self.config.exporter_model.__fields__.keys())
-        if unrecognized := (set(input_keys) - set(model_keys)):
-            logging.warning('导出的列 {%s} 不在模型 {%s} 中', unrecognized, model_keys)
-
-        intersection_keys = list(set(input_keys).intersection(set(model_keys)))
-        selected_keys = self._select_output_excel_keys(intersection_keys)
-        has_merged_header = self.has_merged_header(selected_keys)
-        if has_merged_header:
-            df = self._export_with_merged_header(data, selected_keys, self.config.data_converter)
-        else:
-            df = self._export_with_simple_header(data, selected_keys, self.config.data_converter)
-
+        df, has_merged_header = self._gen_export_df(data, keys)
         return render_data_excel(
             df,
             errors={},  # 数据导出没有错误
             field_meta_mapping=self.unique_label_to_field_meta,
             has_merged_header=has_merged_header,
         )
 
-    def export_excel(self, output_excel_name: str, data: list[dict[str, Any]], keys: list[Key] | None = None) -> bool:
+    def export_upload(self, output_name: str, data: list[dict[str, Any]], keys: list[Key] | None = None) -> UrlStr:
         """导出数据, keys 控制导出的列, 如果为 None, [] 则导出所有列"""
 
-        content_with_prefix = self.export_excel_data(data, keys)
-        url = self._upload_file(output_excel_name, content_with_prefix)
-        return url is not None
+        content_with_prefix = self.export(data, keys)
+        return self._upload_file(output_name, content_with_prefix)
 
     def add_context(self, context: ContextT) -> None:
         """添加转换模型上下文"""
-        if self.config is not None:
+        if self.context is not None:
             logging.warning('已经存在旧的转换模型上下文, 旧的上下文将被替换, 请确认此操作符合预期')
 
         self.context = context
 
     @cached_property
     def input_excel_has_merged_header(self) -> bool:
         """用户上传的 Excel 是否有合并的表头"""
         if not self.__state_df_has_been_loaded__:
-            raise RuntimeError('请保证 df 已经初始化')
+            raise ConfigError('请保证 df 已经初始化')
         return self._excel_has_merged_header()
 
     @cached_property
     def input_excel_headers(self) -> list[ExcelHeader]:
         """用户上传的 Excel 表头"""
         if not self.__state_df_has_been_loaded__:
-            raise RuntimeError('请保证 df 已经初始化')
+            raise ConfigError('请保证 df 已经初始化')
         return self._extract_header()
 
     @property
     def excel_mode(self) -> ExcelMode:
-        if self.config is None:
-            raise RuntimeError('请先设置转换模型配置')
-        if isinstance(self.config, ExcelImporterConfig):
+        if isinstance(self.config, ImporterConfig):
             return ExcelMode.IMPORT
-        if isinstance(self.config, ExcelExporterConfig):
-            return ExcelMode.EXPORT
-        raise RuntimeError('未知的转换模型配置')
+
+        return ExcelMode.EXPORT
 
     @property
     def extra_header_count_on_import(self) -> int:
         # 执行导入时，预期额外的表头行数, 有合并单元格为 1, 无合并单元格为 0
         if self.excel_mode != ExcelMode.IMPORT:
-            raise RuntimeError('只支持导入模式读取此属性')
+            raise ConfigError('只支持导入模式读取此属性')
         for input_excel_label in self.input_excel_headers:
             if input_excel_label.label != input_excel_label.parent_label:
                 return 1
         return 0
 
+    @property
+    def exporter_model(self) -> Type[ExporterModelT]:
+        if isinstance(self.config, ImporterConfig):
+            if self.config.create_importer_model and self.config.update_importer_model:
+                raise ConfigError('从导入模型推断导出模型失败, 请手动设置导出模型')
+            if self.config.create_importer_model:
+                logging.info('从导入模型推断导出模型, 请确认此操作符合预期,使用的是 create_importer_model')
+                return cast(Type[ExporterModelT], self.config.create_importer_model)
+            if self.config.update_importer_model:
+                logging.info('从导入模型推断导出模型, 请确认此操作符合预期,使用的是 update_importer_model')
+                return cast(Type[ExporterModelT], self.config.update_importer_model)
+            raise ConfigError('从导入模型推断导出模型失败, 请手动设置导出模型')
+
+        return self.config.exporter_model
+
     def has_merged_header(self, selected_keys: list[UniqueKey]) -> bool:
         """检查导出的键是否有合并的表头"""
         for key in selected_keys:
             if self.unique_key_to_field_meta[key].label != self.unique_key_to_field_meta[key].parent_label:
                 return True
         return False
 
@@ -288,19 +314,39 @@
     def get_output_child_excel_headers(self, selected_keys: list[UniqueKey] | None = None) -> list[Label]:
         """导出的 Excel 表头"""
         if not selected_keys:
             return [x.label for x in self.ordered_field_meta]
         else:
             return [self.unique_key_to_field_meta[key].label for key in selected_keys]
 
+    def _gen_export_df(self, data: list[dict[str, Any]], keys: list[Key] | None = None) -> tuple[DataFrame, bool]:
+        """导出数据, keys 控制导出的列, 如果为 None, [] 则导出所有列"""
+        if self.excel_mode == ExcelMode.IMPORT:
+            logging.info('导出模式为导入模式, 调用导出方法时自动切换为导出模式')
+
+        input_keys = keys or list(filter(None, [x.parent_key for x in self.ordered_field_meta]))
+        model_keys = cast(list[Key], self.exporter_model.__fields__.keys())
+        if unrecognized := (set(input_keys) - set(model_keys)):
+            logging.warning('导出的列 {%s} 不在模型 {%s} 中', unrecognized, model_keys)
+
+        intersection_keys = list(set(input_keys).intersection(set(model_keys)))
+        selected_keys = self._select_output_excel_keys(intersection_keys)
+        has_merged_header = self.has_merged_header(selected_keys)
+        if has_merged_header:
+            df = self._export_with_merged_header(data, selected_keys, self.config.data_converter)
+        else:
+            df = self._export_with_simple_header(data, selected_keys, self.config.data_converter)
+
+        return df, has_merged_header
+
     def _validate_header(self, input_excel_name: str) -> ValidateHeaderResult:
         """验证表头"""
         if self.excel_mode != ExcelMode.IMPORT:
-            raise RuntimeError('只支持导入模式调用此方法')
-        assert isinstance(self.config, ExcelImporterConfig)  # only for type hint, not for runtime
+            raise ConfigError('只支持导入模式调用此方法')
+        assert isinstance(self.config, ImporterConfig)  # only for type hint, not for runtime
         self._read_dataframe(input_excel_name)
 
         required_labels = [x.label for x in self.ordered_field_meta if x.required]
         primary_labels = [x.label for x in self.ordered_field_meta if x.is_primary_key]
         input_labels = [x.label for x in self.input_excel_headers]
 
         visited = set()
@@ -328,25 +374,25 @@
             errors=self.cell_errors,
             field_meta_mapping=self.import_result_label_to_field_meta | self.unique_label_to_field_meta,
             has_merged_header=self.input_excel_has_merged_header,
         )
 
         return content_with_prefix
 
-    def _upload_file(self, output_excel_name: str, content_with_prefix: str) -> str:
+    def _upload_file(self, output_name: str, content_with_prefix: str) -> UrlStr:
         """上传文件"""
-        assert isinstance(self.config, (ExcelExporterConfig, ExcelImporterConfig))  # only for type check
+        assert isinstance(self.config, (ExporterConfig, ImporterConfig))  # only for type check
         url = upload_file_from_minio_object(
             self.config.minio,
             self.config.bucket_name,
-            output_excel_name,
+            output_name,
             remove_excel_prefix(content_with_prefix),
             self.config.url_expires,
         )
-        return url
+        return UrlStr(url)
 
     def _order_errors(self, errors: list[ExcelRowError | ExcelCellError]) -> Iterable[ExcelCellError | ExcelRowError]:
         """对错误进行排序,依据 ordered_field_meta 的 unique_label 索引排序，ExcelRowError 错误在最后"""
         unique_key_to_index = {field_meta.unique_label: idx for idx, field_meta in enumerate(self.ordered_field_meta)}
         row_errors: list[ExcelRowError] = []
         cell_errors: list[ExcelCellError] = []
         for error in errors:
@@ -358,15 +404,15 @@
         return chain(cell_errors, row_errors)
 
     def _set_columns(self, df: DataFrame) -> DataFrame:
         """设置列名"""
         columns = []
         for header in self.input_excel_headers:
             if header.unique_label not in self.get_output_parent_excel_headers():
-                raise RuntimeError(f'不支持的列名: {header.unique_label}')
+                raise ConfigError(f'不支持的列名: {header.unique_label}')
             columns.append(header.unique_label)
 
         df.columns = columns  # type: ignore[assignment]
         return df
 
     def _select_output_excel_keys(self, keys: list[Key] | None = None) -> list[UniqueKey]:
         """选择出需要导出的键"""
@@ -403,15 +449,15 @@
                 orders.get(cast(Label, x.parent_label), Decimal('Infinity')),
                 x.offset,
             ),
         )
 
     def _read_dataframe(self, input_excel_name: str) -> pandas.DataFrame:
         """读取 DataFrame"""
-        assert isinstance(self.config, ExcelImporterConfig)  # only for type check
+        assert isinstance(self.config, ImporterConfig)  # only for type check
         if not self.__state_df_has_been_loaded__:
             file_object = read_file_from_minio_object(
                 # pyright: reportUnknownMemberType=false
                 # pyright: reportUnknownArgumentType=false
                 self.config.minio,
                 self.config.bucket_name,
                 input_excel_name,
@@ -419,33 +465,22 @@
 
             df: DataFrame = pandas.read_excel(
                 cast(PathLike[str], file_object),  # cast to cheat type check
                 sheet_name=self.config.sheet_name,
                 skiprows=HEADER_HINT_LINE_COUNT,  # 跳过表头提示行
                 header=None,  # 不使用表头, 由程序自行解析
                 dtype=str,  # 读取所有数据为字符串
+                engine='openpyxl',  # 使用 openpyxl 引擎, 避免 xlrd 引擎读取 xlsx 文件时报错
             )
             file_object.close()
             self.df = df
             self.header_df = df.head(2)  # 只读取前两行, 用于解析表头
             self.__state_df_has_been_loaded__ = True
         return self.df
 
-    def _parse_download_data(self, data: list[BaseModel]) -> list[dict[str, Any]]:
-        """解析下载数据"""
-        parsed_data: list[dict[str, Any]] = []
-        for item in data:
-            rst = {}
-            dict_data = flatten(item.dict())
-            for key, value in dict_data.items():
-                field_meta = self.unique_key_to_field_meta[UniqueKey(key)]
-                rst[key] = field_meta.value_type.deserialize(value, field_meta)
-            parsed_data.append(rst)
-        return parsed_data
-
     def _generate_export_df(
         self,
         records: list[dict[str, Any]] | None,
         selected_keys: list[UniqueKey],
         data_converter: Callable[[dict[str, Any]], dict[str, Any]] | None = None,
     ) -> DataFrame:
         """生成导出的 DataFrame"""
@@ -492,72 +527,71 @@
         result: list[str] = []
         reason: list[str] = []
 
         # 遍历数据行, column 不算在 index 中
         for index in self.df.index[self.extra_header_count_on_import :]:
             row_errors = self.row_errors.get(index)
             if not row_errors:
-                result.append(str(ImportRowResult.SUCCESS))
+                result.append(str(ValidateRowResult.SUCCESS))
                 reason.append('')
             else:
-                result.append(str(ImportRowResult.FAIL))
+                result.append(str(ValidateRowResult.FAIL))
                 raw_reason = []
                 for idx, error in enumerate(self._order_errors(row_errors), start=1):  # 给每个错误加上序号，方便用户查看，从1开始
                     raw_reason.append(f'{idx}、{str(error)}')
                 reason.append('\n'.join(raw_reason))
         if self.extra_header_count_on_import == 1:  # 有合并表头
             result = [str(RESULT_COLUMN.unique_label)] + result
             reason = [str(REASON_COLUMN.unique_label)] + reason
         self.df.insert(loc=0, column=REASON_COLUMN.unique_label, value=reason)
         self.df.insert(loc=0, column=RESULT_COLUMN.unique_label, value=result)
 
         return self
 
     async def _dml_caller(self, row_index: RowIndex, data: dict[Key, Any]) -> bool:
         """调用 DML"""
-        if not isinstance(self.config, ExcelImporterConfig):
+        if not isinstance(self.config, ImporterConfig):
             raise TypeError('只有 ExcelImporterConfig 才支持 DML')
 
+        is_success = False
         match self.config.import_mode:
             case ImportMode.CREATE:
                 is_success = await self._creator_caller(row_index, data)
             case ImportMode.UPDATE:
                 is_success = await self._updater_caller(row_index, data)
             case ImportMode.CREATE_OR_UPDATE:
                 is_success = await self._creator_or_updater_caller(row_index, data)
-            case _:
-                raise ValueError(f'不支持的导入模式: {self.config.import_mode}')
 
         return is_success
 
     async def _creator_caller(self, row_index: RowIndex, data: dict[Key, Any]) -> bool:
         """调用创建函数, 返回是否创建成功"""
-        if not isinstance(self.config, ExcelImporterConfig):
+        if not isinstance(self.config, ImporterConfig):
             raise TypeError('只有 ExcelImporterConfig 才支持 DML')
         if self.config.creator is None:
-            raise RuntimeError('未配置 creator')
+            raise ConfigError('未配置 creator')
         if self.config.create_importer_model is None:
-            raise RuntimeError('未配置 create_importer_model')
+            raise ConfigError('未配置 create_importer_model')
         return await self.__caller_impl__(
             row_index,
             data,
             self.config.create_importer_model,
             self.config.creator,
             self.config.data_converter,
             self.config.exec_formatter,
         )
 
     async def _updater_caller(self, row_index: RowIndex, data: dict[Key, Any]) -> bool:
         """调用更新函数, 返回是否创建成功"""
-        if not isinstance(self.config, ExcelImporterConfig):
-            raise TypeError('只有 ExcelImporterConfig 才支持 DML')
+        if not isinstance(self.config, ImporterConfig):
+            raise TypeError(f'只有 {ImporterConfig.__name__} 才支持 DML')
         if self.config.updater is None:
-            raise RuntimeError('未配置 updater')
+            raise ConfigError('未配置 updater')
         if self.config.update_importer_model is None:
-            raise RuntimeError('未配置 update_importer_model')
+            raise ConfigError('未配置 update_importer_model')
         return await self.__caller_impl__(
             row_index,
             data,
             self.config.update_importer_model,
             self.config.updater,
             self.config.data_converter,
             self.config.exec_formatter,
@@ -596,19 +630,19 @@
             self.row_errors[row_index].append(ExcelRowError(exec_formatter(e)))
             return False
 
         return True
 
     async def _creator_or_updater_caller(self, row_index: RowIndex, data: dict[Key, Any]) -> bool:
         """调用 creator 或者 updater"""
-        if not isinstance(self.config, ExcelImporterConfig):
-            raise TypeError('只有 ExcelImporterConfig 才支持 DML')
+        if not isinstance(self.config, ImporterConfig):
+            raise TypeError(f'只有 {ImporterConfig.__name__} 才支持 DML')
         is_data_exists_func = self.config.is_data_exist
         if is_data_exists_func is None:
-            raise RuntimeError('未配置 is_data_exists')
+            raise ConfigError('未配置 is_data_exists')
 
         converted_data = self.config.data_converter(cast(dict[str, Any], data)) if self.config.data_converter else data
         is_data_exist = await is_data_exists_func(cast(dict[str, Any], converted_data), self.context)
         if is_data_exist:
             return await self._updater_caller(row_index, data)
         else:
             return await self._creator_caller(row_index, data)
@@ -616,33 +650,44 @@
     def _aggregate_data(self, row_data: dict[UniqueLabel, Any]) -> dict[Key, Any]:
         """聚合数据
 
         1、将复合类型的数据聚集到同一个 key 中
         2、将 Label 转换为 Key
 
         """
-        assert isinstance(self.config, ExcelImporterConfig)
+        agg_data: dict[Key, Any] = self.__agg_data__(row_data)
+        serialized_agg_data: dict[Key, Any] = self.__serialize_agg_data__(agg_data)
+
+        return serialized_agg_data
+
+    def __agg_data__(self, row_data: dict[UniqueLabel, Any]) -> dict[Key, Any]:
         agg_data: dict[Key, Any] = {}
         for unique_label, value in row_data.items():
             field_meta = self.unique_label_to_field_meta[unique_label]
+
             if field_meta.key is None or field_meta.parent_key is None:
-                raise RuntimeError(f' {type(field_meta).__name__} 未配置 key/parent_key')
+                raise ConfigError(f' {type(field_meta).__name__} 未配置 key/parent_key')
 
             if pandas.isna(value):
-                if self.config.import_mode in {ImportMode.UPDATE, ImportMode.CREATE_OR_UPDATE}:
+                if self.config.import_mode in {  # type: ignore[union-attr]
+                    ImportMode.UPDATE,
+                    ImportMode.CREATE_OR_UPDATE,
+                }:
                     value = None  # 如果是更新模式，且值为 NaN，表示将该值设置为 None
                 else:
                     continue
 
             if field_meta.parent_key == field_meta.key:
                 agg_data[field_meta.key] = value
             else:
                 agg_data.setdefault(field_meta.parent_key, {})
                 agg_data[field_meta.parent_key][field_meta.key] = value
+        return agg_data
 
+    def __serialize_agg_data__(self, agg_data: dict[Key, Any]) -> dict[Key, Any]:
         serialized_agg_data: dict[Key, Any] = {}
         for parent_key, value in agg_data.items():
             field_metas = self.parent_key_to_field_metas[parent_key]
             validator = field_metas[0]
             if value is None:
                 serialized_agg_data[parent_key] = None
             else:
@@ -688,17 +733,17 @@
                 column_index = cast(ColumnIndex, index + len(self.import_result_field_meta))
                 self.cell_errors.setdefault(row_index, {}).setdefault(column_index, []).append(error)
         return self
 
     def _excel_has_merged_header(self) -> bool:
         """判断是否有合并表头
 
-        如果第 0 行有合并单元格，则一定有 nan 值，否则没有合并单元格
+        如果第 0 行有合并单元格，则一定有 nan 值或 Unnamed ，否则没有合并单元格
         """
-        return any(pandas.isna(self.header_df.iloc[0]))
+        return any(pandas.isna(self.header_df.iloc[0])) or any(self.header_df.iloc[0].str.startswith('Unnamed'))
 
     def _extract_header(self) -> list[ExcelHeader]:
         """提取表头信息"""
         if self._excel_has_merged_header():
             return self._extract_merged_header()
         else:
             return self._extract_simple_header()
@@ -713,15 +758,15 @@
         header_row_index = 0
 
         last_header = None
         next_offset = 1
         for column_index, value in self.header_df.iloc[header_row_index].items():
             parent_value = value
             child_value = self.header_df.iloc[header_row_index + 1][column_index]  # type: ignore[call-overload]
-            if pandas.isna(parent_value):
+            if pandas.isna(parent_value) or parent_value.startswith('Unnamed'):
                 if pandas.isna(child_value):
                     raise ValueError('合并表头错误: 子表头不能为空')
                 current_header = ExcelHeader(
                     label=Label(child_value),
                     parent_label=Label(last_header),
                     offset=next_offset,
                 )
@@ -732,10 +777,13 @@
                 current_header = ExcelHeader(label=Label(child_value), parent_label=Label(value))
                 last_header, next_offset = value, 1
             headers.append(current_header)
 
         return headers
 
     def __setattr__(self, key: str, value: Any):
-        if key == 'config' and hasattr(self, 'config') and self.config is not None:
+        if key == 'config' and hasattr(self, 'config'):
             raise ValueError(f'{self.__class__.__name__} 已经被实例化, config 不能被修改')
         object.__setattr__(self, key, value)
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}(config={self.config!r})'
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/exception.py` & `ExcelAlchemy-1.0.0/excelalchemy/exc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 from excelalchemy.const import UNIQUE_HEADER_CONNECTOR
-from excelalchemy.model.identity import Label
-from excelalchemy.model.identity import UniqueLabel
+from excelalchemy.types.identity import Label
+from excelalchemy.types.identity import UniqueLabel
 
 
 class ExcelCellError(Exception):
     """Excel 单元格错误"""
 
     message = '导入 Excel 发生错误'
     label: Label
@@ -27,30 +27,33 @@
         self.detail = kwargs or {}
         self._validate()
 
     def __str__(self) -> str:
         return f'【{self.label}】{self.message}'
 
     def __repr__(self):
-        return f"{type(self).__name__}(label='{self.label}', message='{self.message}')"
+        return f"{type(self).__name__}(label=Label('{self.label}'), message='{self.message}')"
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, ExcelCellError):
+            return NotImplemented
+        return str(self) == str(other)
 
     @property
     def unique_label(self) -> UniqueLabel:
         label = (
             f'{self.parent_label}{UNIQUE_HEADER_CONNECTOR}{self.label}'
             if (self.parent_label and self.parent_label != self.label)
             else self.label
         )
         return UniqueLabel(label)
 
     def _validate(self) -> None:
         if not self.label:
             raise ValueError('label 不能为空')
-        if not self.message:
-            raise ValueError('message 不能为空')
 
 
 class ExcelRowError(Exception):
     """Excel 整行发生导入错误"""
 
     message = '导入 Excel 发生行错误'
 
@@ -63,12 +66,16 @@
         self.message = message or self.message
         self.detail = kwargs or {}
 
     def __str__(self):
         return self.message
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({self.message})'
+        return f"{type(self).__name__}(message='{self.message}')"
 
 
 class ProgrammaticError(Exception):
     ...
+
+
+class ConfigError(Exception):
+    ...
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/helper/pydantic.py` & `ExcelAlchemy-1.0.0/excelalchemy/helper/pydantic.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 from pydantic import NoneIsNotAllowedError
 from pydantic import ValidationError
 from pydantic.error_wrappers import ErrorList
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.fields import ModelField
 from pydantic.fields import UndefinedType
 
-from excelalchemy.exception import ExcelCellError
-from excelalchemy.exception import ProgrammaticError
-from excelalchemy.model.abstract import ABCValueType
-from excelalchemy.model.abstract import ComplexABCValueType
-from excelalchemy.model.abstract import CreateImporterModelT
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.abstract import UpdateImporterModelT
-from excelalchemy.model.identity import Key
+from excelalchemy.const import ImporterCreateModelT
+from excelalchemy.const import ImporterUpdateModelT
+from excelalchemy.exc import ExcelCellError
+from excelalchemy.exc import ProgrammaticError
+from excelalchemy.types.abstract import ABCValueType
+from excelalchemy.types.abstract import ComplexABCValueType
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.identity import Key
 
 ModelT = TypeVar('ModelT', bound=BaseModel)
 
 
 def extract_pydantic_model(
-    model: type[CreateImporterModelT] | type[UpdateImporterModelT] | None,
+    model: type[ImporterCreateModelT] | type[ImporterUpdateModelT] | type[BaseModel] | None,
 ) -> list[FieldMetaInfo]:
     """根据 Pydantic 模型提取 Excel 表头信息
     包含是否必填、值类型、注释等信息
     """
     if model is None:
         raise RuntimeError('模型不能为空')
     return list(_extract_pydantic_model(model))
 
 
-def instantiate_pydantic_model(
+def instantiate_pydantic_model(  # noqa: C901
     data: dict[Key, Any],
     model: type[ModelT],
 ) -> ModelT | list[ExcelCellError]:
     """实例化 Pydantic 模型, 并返回错误.
 
     若实例化成功, 则返回实例化后的模型, 错误信息为 None
     若实例化失败, 则模型返回 None, 错误信息为 ExcelImportError 列表
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/result.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""导入 Excel 的结果"""
 from enum import Enum
 
 from pydantic import BaseModel
+from pydantic import Extra
 from pydantic import Field
 
-from excelalchemy.model.identity import Label
+from excelalchemy.types.identity import Label
 
 
-class ImportRowResult(str, Enum):
+class ValidateRowResult(str, Enum):
     """导入结果"""
 
     SUCCESS = '校验通过'
     FAIL = '校验不通过'
 
     def __str__(self):
         return self.value
@@ -27,41 +29,46 @@
 
     @property
     def is_required_missing(self) -> bool:
         """是否缺失必填表头"""
         return bool(self.missing_required)
 
 
-class ImportExcelResult(str, Enum):
+class ValidateResult(str, Enum):
     """导入结果类型"""
 
     HEADER_INVALID = 'HEADER_INVALID'  # 表头无效
     DATA_INVALID = 'DATA_INVALID'  # 数据无效
     SUCCESS = 'SUCCESS'  # 成功
 
 
-class ImportDataResult(BaseModel):
+class ImportResult(BaseModel):
     """导入数据结果"""
 
-    result: ImportExcelResult = Field(description='导入结果')
+    result: ValidateResult = Field(description='导入结果')
 
     is_required_missing: bool = Field(default=False, description='是否缺失必填表头')
+    missing_required: list[Label] = Field(default_factory=list, description='缺失的必填表头')
     missing_primary: list[Label] = Field(default_factory=list, description='缺失的关键列')
     unrecognized: list[Label] = Field(default_factory=list, description='无法识别的表头')
     duplicated: list[Label] = Field(default_factory=list, description='重复的表头')
 
     url: str | None = Field(default=None, description='导入结果文件的下载链接, 失败时有值')
     success_count: int = Field(default=0, description='导入成功的数据条数')
     fail_count: int = Field(default=0, description='导入失败的数据条数')
 
+    class Config:
+        extra = Extra.allow
+
     @classmethod
-    def from_validate_header_result(cls, result: ValidateHeaderResult) -> 'ImportDataResult':
+    def from_validate_header_result(cls, result: ValidateHeaderResult) -> 'ImportResult':
         """从校验表头结果构造导入结果"""
         if result.is_valid:
             raise RuntimeError('只有校验表头失败时才能构造导入结果')
         return cls(
-            result=ImportExcelResult.HEADER_INVALID,
+            result=ValidateResult.HEADER_INVALID,
             is_required_missing=result.is_required_missing,
             missing_primary=result.missing_primary,
             unrecognized=result.unrecognized,
             duplicated=result.duplicated,
+            missing_required=result.missing_required,
         )
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/boolean.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/multi_checkbox.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,71 @@
 import logging
-from typing import TYPE_CHECKING
 from typing import Any
+from typing import cast
 
-from excelalchemy.model.abstract import ABCValueType
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.value_type import excel_choice
+from excelalchemy.const import MULTI_CHECKBOX_SEPARATOR
+from excelalchemy.exc import ProgrammaticError
+from excelalchemy.types.abstract import ABCValueType
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.identity import OptionId
 
 
-@excel_choice
-class Boolean(ABCValueType):
-
-    __name__ = '布尔'
+class MultiCheckbox(ABCValueType, list[str]):
+    __name__ = '复选框组'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        required = '必填' if field_meta.required else '选填'
-        extra_hint = field_meta.hint
-        return f'必填性: {required}\n可选值: 是、否' + (f'\n提示: {extra_hint}' if extra_hint else '')
+        return '\n'.join(
+            [
+                field_meta.comment_required,
+                field_meta.comment_options,
+                '单/多选：多选',
+                field_meta.comment_hint,
+            ]
+        )
 
     @classmethod
-    def serialize(cls, value: Any, field_meta: FieldMetaInfo) -> str:
-        return str(value).strip()
+    def serialize(cls, value: str | Any, field_meta: FieldMetaInfo) -> list[str] | str:
+        # If the value is a list, convert all items to strings and strip whitespace
+        if isinstance(value, list):
+            return [str(item).strip() for item in cast(list[Any], value)]
+
+        # If the value is a string, split it into a list using MULTI_CHECKBOX_SEPARATOR and strip whitespace
+        if isinstance(value, str):
+            return [item.strip() for item in value.split(MULTI_CHECKBOX_SEPARATOR)]
+
+        # If the value is of an unsupported type, log a warning and return the original value
+        logging.warning('ValueType 类型 <%s> 无法解析 Excel 输入, 返回原值:%s', cls.__name__, value)
+        return value
 
     @classmethod
-    def _validate(cls, v: str | bool | Any, field_meta: FieldMetaInfo) -> bool:
-        if isinstance(v, bool):
-            return v
-
-        try:
-            parsed = str(v)
-        except Exception as exc:
-            raise ValueError('请输入“是”或“否”') from exc
+    def __validate__(cls, value: list[str] | Any, field_meta: FieldMetaInfo) -> list[str]:  # OptionId
+        if not isinstance(value, list):
+            raise ValueError('选项不存在，请参照表头的注释填写')
 
-        if parsed not in ('是', '否'):
-            raise ValueError('请输入“是”或“否”')
-        else:
-            return parsed == '是'
+        if field_meta.options is None:
+            raise ProgrammaticError(f'options cannot be None when validate {cls.__name__}')
 
-    @classmethod
-    def deserialize(cls, value: bool | str | None | Any, field_meta: FieldMetaInfo) -> str:
-        if value is None or value == '':
-            return '否'  # 产品要求，空值默认为否
-        if isinstance(value, bool):
-            return '是' if value else '否'
-
-        elif isinstance(value, str):
-            value = value.strip()
-            if value not in ('是', '否'):
-                logging.warning('无法识别布尔值 %s, 返回原值', value)
-                return value
+        if not field_meta.options:  # empty
+            logging.warning('类型【%s】的字段【%s】的选项为空, 将返回原值', cls.__name__, field_meta.label)
             return value
-        else:
-            logging.warning('类型【%s】无法为 %s 反序列化: %s, 返回默认值 "否" ', cls.__name__, field_meta.label, value)
 
-        return '是' if str(value) == '是' else '否'
+        if len(value) != len(set(value)):
+            raise ValueError('选项有重复')
 
+        result, errors = field_meta.exchange_names_to_option_ids_with_errors(value)
 
-if TYPE_CHECKING:
-    # pyright: reportGeneralTypeIssues=false
-    Boolean = bool  # type: ignore
+        if errors:
+            raise ValueError(*errors)
+        else:
+            return result
+
+    @classmethod
+    def deserialize(cls, value: str | list[OptionId] | None, field_meta: FieldMetaInfo) -> str:
+        match value:
+            case None | '':
+                return ''
+            case str():
+                return value
+            case list():
+                option_names = field_meta.exchange_option_ids_to_names(value)
+                return f'{MULTI_CHECKBOX_SEPARATOR}'.join(option_names)
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/date.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,90 +2,104 @@
 from datetime import datetime
 from typing import Any
 from typing import cast
 
 import pendulum
 from pendulum import DateTime
 
+from excelalchemy.const import DATE_FORMAT_TO_HINT_MAPPING
 from excelalchemy.const import MILLISECOND_TO_SECOND
-from excelalchemy.model.abstract import DATA_RANGE_OPTION_TO_CHINESE
-from excelalchemy.model.abstract import DATE_FORMAT_TO_HINT_MAPPING
-from excelalchemy.model.abstract import DATE_FORMAT_TO_PYTHON_MAPPING
-from excelalchemy.model.abstract import ABCValueType
-from excelalchemy.model.abstract import DataRangeOption
-from excelalchemy.model.abstract import FieldMetaInfo
+from excelalchemy.const import DataRangeOption
+from excelalchemy.exc import ConfigError
+from excelalchemy.types.abstract import ABCValueType
+from excelalchemy.types.field import FieldMetaInfo
 
 
 class Date(ABCValueType, datetime):
-
     __name__ = '日期选择'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        required = '必填' if field_meta.required else '选填'
-        if field_meta.date_format is None:
-            raise RuntimeError('日期格式未定义')
-        date_hint = DATE_FORMAT_TO_HINT_MAPPING[field_meta.date_format]
-        date_range_option = field_meta.date_range_option
-        range_hint = DATA_RANGE_OPTION_TO_CHINESE[date_range_option] if date_range_option else '无限制'
-        extra_hint = f'\n提示：{field_meta.hint}' if field_meta.hint else ''
-        return f"""必填性：{required}\n格式：日期（{date_hint }）\n范围：{range_hint}""" + extra_hint
+        if not field_meta.date_format:
+            raise ConfigError('日期格式未定义')
+        return '\n'.join(
+            [
+                field_meta.comment_required,
+                field_meta.comment_date_format,
+                field_meta.comment_date_range_option,
+                field_meta.comment_hint,
+            ]
+        )
 
     @classmethod
-    def serialize(cls, value: str | datetime | Any, field_meta: FieldMetaInfo) -> datetime | Any:
-        if isinstance(value, datetime):
+    def serialize(cls, value: str | DateTime | Any, field_meta: FieldMetaInfo) -> datetime | Any:
+        if isinstance(value, DateTime):
             logging.info('类型【%s】无需序列化: %s, 返回原值 %s ', cls.__name__, field_meta.label, value)
             return value
-        if field_meta.date_format is None:
-            raise RuntimeError('日期格式未定义')
+
+        if not field_meta.date_format:
+            raise ConfigError('日期格式未定义')
 
         value = str(value).strip()
         try:
             # pyright: reportPrivateImportUsage=false
             # pyright: reportUnknownMemberType=false
             # pyright: reportGeneralTypeIssues=false
             v = value.replace('/', '-')  # pendulum 不支持 / 作为日期分隔符
-            d: DateTime = cast(DateTime, pendulum.parse(v))
-            return d.replace(tzinfo=field_meta.timezone)
+            dt: DateTime = cast(DateTime, pendulum.parse(v))
+            return dt.replace(tzinfo=field_meta.timezone)
         except Exception as exc:
-            logging.warning('ValueType 类型 <%s> 无法解析 Excel 输入, 返回原值:%s, 原因 %s', cls.__name__, value, exc)
+            logging.warning('ValueType 类型 <%s> 无法解析 Excel 输入，返回原值：%s，原因：%s', cls.__name__, value, exc)
             return value
 
     @classmethod
-    def _validate(cls, v: Any, field_meta: FieldMetaInfo) -> int:
+    def deserialize(cls, value: str | datetime | None | Any, field_meta: FieldMetaInfo) -> str:
+        match value:
+            case None | '':
+                return ''
+            case datetime():
+                return value.strftime(field_meta.python_date_format)
+            case int() | float():
+                return datetime.fromtimestamp(int(value) / MILLISECOND_TO_SECOND).strftime(
+                    field_meta.python_date_format
+                )
+            case _:
+                return str(value) if value is not None else ''
+
+    @classmethod
+    def __validate__(cls, value: Any, field_meta: FieldMetaInfo) -> int:
         if field_meta.date_format is None:
-            raise RuntimeError('日期格式未定义')
-        if not isinstance(v, datetime):
+            raise ConfigError('日期格式未定义')
+
+        if not isinstance(value, datetime):
             raise ValueError(f'请输入格式为{DATE_FORMAT_TO_HINT_MAPPING[field_meta.date_format]}的日期')
 
-        parsed = v.replace(tzinfo=field_meta.timezone)
-        errors: list[str] = []
+        parsed = cls._parse_date(value, field_meta)
+        errors = cls._validate_date_range(parsed, field_meta)
+
+        if errors:
+            raise ValueError(*errors)
+        else:
+            return int(parsed.timestamp() * MILLISECOND_TO_SECOND)
+
+    @staticmethod
+    def _parse_date(v: datetime, field_meta: FieldMetaInfo) -> datetime:
+        format_ = field_meta.python_date_format
+        parsed = pendulum.parse(v.strftime(format_)).replace(tzinfo=field_meta.timezone)  # type: ignore
+        return parsed
+
+    @staticmethod
+    def _validate_date_range(parsed: datetime, field_meta: FieldMetaInfo) -> list[str]:
         now = datetime.now(tz=field_meta.timezone)
+        errors: list[str] = []
 
         match field_meta.date_range_option:
             case DataRangeOption.PRE:
                 if parsed > now:
                     errors.append('需早于当前时间（含当前时间）')
             case DataRangeOption.NEXT:
                 if parsed < now:
                     errors.append('需晚于当前时间（含当前时间）')
             case DataRangeOption.NONE | None:
-                ...  # do nothing
+                ...
 
-        if errors:
-            raise ValueError(*errors)
-        else:
-            return int(parsed.timestamp() * MILLISECOND_TO_SECOND)
-
-    @classmethod
-    def deserialize(cls, value: str | datetime | None | Any, field_meta: FieldMetaInfo) -> str:
-        if value is None or value == '':
-            return ''
-        if field_meta.date_format is None:
-            raise RuntimeError('日期格式未定义')
-        python_dateformat = DATE_FORMAT_TO_PYTHON_MAPPING[field_meta.date_format]
-        if isinstance(value, datetime):
-            return value.strftime(python_dateformat)
-        elif isinstance(value, (int, float)):
-            return datetime.fromtimestamp(value / MILLISECOND_TO_SECOND).strftime(python_dateformat)
-        else:
-            return value if value is not None else ''
+        return errors
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/date_range.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/date_range.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import logging
 from datetime import datetime
 from typing import Any
-from typing import cast
 
 import pendulum
 
 # pyright: reportPrivateImportUsage=false
 from pendulum import DateTime
 from pydantic import BaseModel
 
+from excelalchemy.const import DATE_FORMAT_TO_PYTHON_MAPPING
 from excelalchemy.const import MILLISECOND_TO_SECOND
-from excelalchemy.model.abstract import DATE_FORMAT_TO_HINT_MAPPING
-from excelalchemy.model.abstract import DATE_FORMAT_TO_PYTHON_MAPPING
-from excelalchemy.model.abstract import ComplexABCValueType
-from excelalchemy.model.abstract import DataRangeOption
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.identity import Key
+from excelalchemy.const import DataRangeOption
+from excelalchemy.types.abstract import ComplexABCValueType
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.identity import Key
 
 
 class _DateRangeImpl(BaseModel):
     start: datetime | None
     end: datetime | None
 
 
@@ -32,15 +30,14 @@
     @classmethod
     def parse_obj(cls, obj: Any) -> 'DateRange':
         impl = _DateRangeImpl.parse_obj(obj)
         self = cls(impl.start, impl.end)
         return self
 
     def __init__(self, start: datetime | None, end: datetime | None):
-
         # pyright: reportUnknownMemberType=false
         # trick, BaseMode.dict() 会得到时间戳，而不是 datetime 对象，这是预期的行为
         _start = int(start.timestamp() * MILLISECOND_TO_SECOND) if start else None
         _end = int(end.timestamp() * MILLISECOND_TO_SECOND) if end else None
         super().__init__(start=_start, end=_end)
         self.start = start
         self.end = end
@@ -50,59 +47,72 @@
         return [
             (Key('start'), FieldMetaInfo(label='开始日期')),
             (Key('end'), FieldMetaInfo(label='结束日期')),
         ]
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        required = '必填' if field_meta.required else '选填'
         if field_meta.date_format is None:
             raise RuntimeError('日期格式未定义')
-        extra_hint = field_meta.hint or ''
-        date_hint = DATE_FORMAT_TO_HINT_MAPPING[field_meta.date_format]
-        return f"""必填性：{required}\n格式：日期（{date_hint}）\n提示：开始日期不得晚于结束日期{extra_hint}"""
+
+        return '\n'.join(
+            [
+                field_meta.comment_required,
+                field_meta.comment_date_format,
+                f'提示：开始日期不得晚于结束日期{field_meta.hint or ""}',
+            ]
+        )
 
     @classmethod
     def serialize(cls, value: dict[str, str] | Any, field_meta: FieldMetaInfo) -> dict[str, DateTime | None] | Any:
-        if isinstance(value, dict):
-            try:
-                _start = value['start']
-                _end = value['end']
-
-                start: DateTime | None = (
-                    pendulum.parse(_start).replace(tzinfo=field_meta.timezone)  # type: ignore[union-attr,call-arg]
-                    if _start
-                    else None
-                )
-                end: DateTime | None = (
-                    pendulum.parse(_end).replace(tzinfo=field_meta.timezone)  # type: ignore[union-attr,call-arg]
-                    if _end
-                    else None
-                )
-                # pyright: reportGeneralTypeIssues=false
-                return {'start': start, 'end': end}
-            except Exception as exc:
-                logging.warning('ValueType 类型 <%s> 无法解析 Excel 输入, 返回原值:%s, 原因: %s', cls.__name__, value, exc)
+        match value:
+            case dict():
+                try:
+                    start_str, end_str = value.get('start'), value.get('end')
+                    # pyright: reportGeneralTypeIssues=false
+                    # pyright: reportUnknownArgumentType=false
+                    start_time = (
+                        pendulum.parse(start_str).replace(  # type: ignore
+                            tzinfo=field_meta.timezone,
+                        )
+                        if start_str
+                        else None
+                    )
+                    end_time = (
+                        pendulum.parse(end_str).replace(  # type: ignore
+                            tzinfo=field_meta.timezone,
+                        )
+                        if end_str
+                        else None
+                    )
+
+                    return {'start': start_time, 'end': end_time}
+                except Exception as e:
+                    logging.warning('Could not parse value %s for field %s. Reason: %s', value, cls.__name__, e)
+                    return value
+            case datetime():
+                return value
+            case str():
+                try:
+                    datetime_value = pendulum.parse(value).replace(tzinfo=field_meta.timezone)  # type: ignore
+                except Exception as e:
+                    logging.warning('Could not parse value %s for field %s. Reason: %s', value, cls.__name__, e)
+                    return value
+                return datetime_value
+            case _:
                 return value
-        elif isinstance(value, datetime):
-            return value
-        elif isinstance(value, str):
-            d: DateTime = cast(DateTime, pendulum.parse(value))
-            return d.replace(tzinfo=field_meta.timezone)
-        else:
-            return value
 
     @classmethod
-    def _validate(
+    def __validate__(
         cls,
-        v: dict[str, DateTime | None] | Any,
+        value: dict[str, DateTime | None] | Any,
         field_meta: FieldMetaInfo,
     ) -> 'DateRange':
         try:
-            parsed = DateRange.parse_obj(v)
+            parsed = DateRange.parse_obj(value)
             parsed.start = parsed.start.replace(tzinfo=field_meta.timezone) if parsed.start else parsed.start
             parsed.end = parsed.end.replace(tzinfo=field_meta.timezone) if parsed.end else parsed.end
         except Exception as exc:
             raise ValueError('无法识别的输入') from exc
 
         errors: list[str] = []
         now = datetime.now(tz=field_meta.timezone)
@@ -125,28 +135,35 @@
         else:
             return parsed
 
     @classmethod
     def deserialize(cls, value: dict[str, str] | str | Any | None, field_meta: FieldMetaInfo) -> str:
         if value is None or value == '':
             return ''
-        date_format = field_meta.date_format
-        if date_format is None:
-            raise RuntimeError('日期格式未定义')
+        date_format = field_meta.must_date_format
         py_date_format = DATE_FORMAT_TO_PYTHON_MAPPING[date_format]
+
         if isinstance(value, str):
             return value
 
         if isinstance(value, datetime):
             return value.strftime(py_date_format)
 
         if isinstance(value, dict):
-            start = value['start']
-            end = value['end']
-            if isinstance(start, (int, float)):
-                start = datetime.fromtimestamp(start / MILLISECOND_TO_SECOND).strftime(py_date_format)
-            if isinstance(end, (int, float)):
-                end = datetime.fromtimestamp(end / MILLISECOND_TO_SECOND).strftime(py_date_format)
-            return start + ' - ' + end
+            return cls.__deserialize__dict(py_date_format, value)
 
         logging.warning('%s 反序列化失败，返回原值', cls.__name__)
         return value if value is not None else ''
+
+    @classmethod
+    def __deserialize__dict(cls, py_date_format: str, value: dict[str, Any]) -> str:
+        start, end = value['start'], value['end']
+        if isinstance(start, datetime):
+            start = start.strftime(py_date_format)
+        elif isinstance(start, (int, float)):
+            start = datetime.fromtimestamp(start / MILLISECOND_TO_SECOND).strftime(py_date_format)
+
+        if isinstance(end, datetime):
+            end = end.strftime(py_date_format)
+        elif isinstance(end, (int, float)):
+            end = datetime.fromtimestamp(end / MILLISECOND_TO_SECOND).strftime(py_date_format)
+        return start + ' - ' + end
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/number_range.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/number.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,139 @@
 import logging
+from decimal import ROUND_DOWN
+from decimal import Context
 from decimal import Decimal
+from decimal import InvalidOperation
 from typing import Any
 
-from excelalchemy.model.abstract import ComplexABCValueType
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.identity import Key
-from excelalchemy.model.value_type.number import Number
-from excelalchemy.model.value_type.number import canonicalize_decimal
-from excelalchemy.model.value_type.number import transform_decimal
-
-
-class NumberRange(ComplexABCValueType):
-    start: float | int | None
-    end: float | int | None
-
-    __name__ = '数值范围'
-
-    def __init__(self, start: Decimal | int | float | None, end: Decimal | int | float | None):
-        # pyright: reportUnknownMemberType=false
-        # trick: for dict call to get the correct value
-        super().__init__(start=transform_decimal(start), end=transform_decimal(end))
-        self.start = transform_decimal(start)
-        self.end = transform_decimal(end)
+from excelalchemy.types.abstract import ABCValueType
+from excelalchemy.types.field import FieldMetaInfo
+
+
+def canonicalize_decimal(value: Decimal, digits_limit: int | None) -> Decimal:
+    """将 Decimal 转换为指定精度的 Decimal"""
+    # pyright: reportGeneralTypeIssues=false
+    if digits_limit is not None and abs(value.as_tuple().exponent) != digits_limit:  # type: ignore[arg-type]
+        try:
+            value = Decimal(value).quantize(
+                Decimal(f'0.{"0" * digits_limit}'),
+                context=Context(rounding=ROUND_DOWN),
+            )
+        except InvalidOperation as e:
+            logging.warning('精度设置的过小，导致精度丢失，%s', e)
+    return value
+
+
+def transform_decimal(value: Decimal | int | float | None) -> float | int | None:
+    """将 Decimal 转换为 float 或 int"""
+    if value is None:
+        return None
+
+    if isinstance(value, (int, float)):
+        return value
+
+    if not isinstance(value, Decimal):  # pyright: reportUnnecessaryIsInstance=false
+        raise TypeError(f'Expected Decimal, got {type(value)}')
+
+    if value.as_tuple().exponent == 0:
+        return int(value)
+    else:
+        return float(value)
 
-    @classmethod
-    def model_items(cls) -> list[tuple[Key, FieldMetaInfo]]:
-        return [
-            (Key('start'), FieldMetaInfo(label='最小值')),
-            (Key('end'), FieldMetaInfo(label='最大值')),
-        ]
+
+class Number(Decimal, ABCValueType):
+    __name__ = '数值输入'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        return Number.comment(field_meta)
+        return '\n'.join(
+            [
+                field_meta.comment_required,
+                '格式：数值',
+                field_meta.comment_fraction_digits,
+                f'可输入范围：{cls.__get_range_description__(field_meta)}',
+                field_meta.comment_unit,
+            ]
+        )
 
     @classmethod
-    def serialize(
-        cls,
-        value: dict[str, str] | str | Any,
-        field_meta: FieldMetaInfo,
-    ) -> Any:
+    def serialize(cls, value: str | int | float | None, field_meta: FieldMetaInfo) -> Decimal | Any:
         if isinstance(value, str):
             value = value.strip()
-
-        if isinstance(value, NumberRange):
-            return value
         try:
-            # pyright: reportGeneralTypeIssues=false
-            return NumberRange(Decimal(value['start']), Decimal(value['end']))  # type: ignore[index]
+            return transform_decimal(Decimal(value))  # type: ignore[arg-type]
         except Exception as exc:
             logging.warning('ValueType 类型 <%s> 无法解析 Excel 输入, 返回原值:%s, 原因: %s', cls.__name__, value, exc)
+            return str(value) if value is not None else ''
 
-        return value
+    @classmethod
+    def deserialize(cls, value: str | None | Any, field_meta: FieldMetaInfo) -> str:
+        if value is None or value == '':
+            return ''
+
+        try:
+            return str(transform_decimal(Decimal(value)))
+        except Exception as exc:
+            logging.warning('ValueType 类型 <%s> 无法解析 Excel 输入, 返回原值:%s, 原因: %s', cls.__name__, value, exc)
+            return str(value)
 
-    # pylint: disable=too-many-branches
     @classmethod
-    def _validate(cls, v: Any, field_meta: FieldMetaInfo) -> 'NumberRange':
-        if not isinstance(v, NumberRange):
-            try:
-                v['start'] = canonicalize_decimal(Decimal(v['start']), field_meta.fraction_digits)
-                v['end'] = canonicalize_decimal(Decimal(v['end']), field_meta.fraction_digits)
-                parsed = NumberRange(v['start'], v['end'])
-            except Exception as exc:
-                raise ValueError('请输入数字') from exc
-        else:
-            parsed = v
+    def __get_range_description__(cls, field_meta: FieldMetaInfo) -> str:  # type: ignore[return]
+        match (field_meta.importer_le, field_meta.importer_ge):
+            case (None, None):
+                return '无限制'
+            case (_, None):
+                return f'≤ {field_meta.importer_le}'
+            case (None, _):
+                return f'≥ {field_meta.importer_ge}'
+            case (le, ge):
+                return f'{ge}～{le}'
+
+    @staticmethod
+    def __maybe_decimal__(value: Any) -> Decimal | None:
+        # 如果输入不是 Decimal 类型，尝试转换。
+        if isinstance(value, Decimal):
+            return value
+
+        try:
+            parsed = Decimal(str(value))
+        except Exception as exc:
+            raise ValueError('无效输入，请输入数字。') from exc
+
+        return parsed
 
+    @staticmethod
+    def __check_range__(value: Decimal | float | int, field_meta: FieldMetaInfo) -> list[str]:
         errors: list[str] = []
-        if parsed.start is not None and parsed.end is not None and parsed.start > parsed.end:
-            errors.append('最小值不能大于最大值')
 
-        # importer_le 取值 field_meta.importer_le 或者无穷大
+        # 从 field_meta 对象中获取导入者上限和下限值。
         importer_le = field_meta.importer_le or Decimal('Infinity')
-        # importer_ge 取值 field_meta.importer_ge 或者无穷小
         importer_ge = field_meta.importer_ge or Decimal('-Infinity')
 
-        if parsed.start is not None:
-            if not importer_ge <= parsed.start <= importer_le:
-                if field_meta.importer_le and field_meta.importer_ge:
-                    errors.append(f'请输入{field_meta.importer_ge}～{field_meta.importer_le}范围内的数字')
-                elif field_meta.importer_le:
-                    errors.append(f'请输入-∞～{field_meta.importer_le}范围内的数字')
-                elif field_meta.importer_ge:
-                    errors.append(f'请输入{field_meta.importer_ge}～+∞范围内的数字')
-                else:
-                    pass
-
-        if parsed.end is not None:
-            if not importer_ge <= parsed.end <= importer_le:
-                if field_meta.importer_le and field_meta.importer_ge:
-                    errors.append(f'请输入{field_meta.importer_ge}～{field_meta.importer_le}范围内的数字')
-                elif field_meta.importer_le:
-                    errors.append(f'请输入-∞～{field_meta.importer_le}范围内的数字')
-                elif field_meta.importer_ge:
-                    errors.append(f'请输入{field_meta.importer_ge}～+∞范围内的数字')
-                else:
-                    pass
-
-        if errors:
-            raise ValueError(*errors)
-        else:
+        # 确保解析后的 decimal 在接受范围内。
+        if not importer_ge <= value <= importer_le:
+            if field_meta.importer_le and field_meta.importer_ge:
+                errors.append(f'请输入在 {field_meta.importer_ge} 和 {field_meta.importer_le} 之间的数字。')
+            elif field_meta.importer_le:
+                errors.append(f'请输入在 -∞ 和 {field_meta.importer_le} 之间的数字。')
+            elif field_meta.importer_ge:
+                errors.append(f'请输入在 {field_meta.importer_ge} 和 +∞ 之间的数字。')
+            else:
+                pass
 
-            return parsed
+        return errors
 
     @classmethod
-    def deserialize(cls, value: Any | None, field_meta: FieldMetaInfo) -> str:
-        if value is None or value == '':
-            return ''
-        try:
-            return str(transform_decimal(canonicalize_decimal(Decimal(value), field_meta.fraction_digits)))
-        except Exception as exc:
-            logging.warning('ValueType 类型 <%s> 无法解析 Excel 输入, 返回原值:%s, 原因: %s', cls.__name__, value, exc)
-            return str(value)
+    def __validate__(cls, value: Decimal | Any, field_meta: FieldMetaInfo) -> float | int:
+        # 如果输入不是 Decimal 类型，尝试转换。
+        parsed = cls.__maybe_decimal__(value)
+        if parsed is None:
+            raise ValueError('无效输入，请输入数字。')
+        # 初始化一个错误信息列表。
+        errors: list[str] = cls.__check_range__(value, field_meta)
+        if errors:
+            raise ValueError(*errors)
+        parsed = canonicalize_decimal(parsed, field_meta.fraction_digits)
+        value = transform_decimal(parsed)
+        if value is None:
+            raise ValueError('无效输入，请输入数字。')
+        return value
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/organization.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/organization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import logging
 from typing import Any
 
 from excelalchemy.const import MULTI_CHECKBOX_SEPARATOR
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.identity import OptionId
-from excelalchemy.model.value_type.multi_checkbox import MultiCheckbox
-from excelalchemy.model.value_type.radio import Radio
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.value.multi_checkbox import MultiCheckbox
+from excelalchemy.types.value.radio import Radio
 
 
 class SingleOrganization(Radio):
     __name__ = '组织单选'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        required = '必填' if field_meta.required else '非必填'
-        extra_hint = field_meta.hint or '需按照组织架构树填写组织完整路径，如“XX公司/一级部门/二级部门”.'
-        return f"""必填性：{required} \n提示：{extra_hint}"""
+        required_str = '必填' if field_meta.required else '非必填'
+        extra_hint = field_meta.hint or "需按照组织架构树填写组织完整路径，例如 'XX公司/一级部门/二级部门'."
+        return f"""必填性：{required_str}\n提示：{extra_hint}"""
 
     @classmethod
     def serialize(cls, value: Any, field_meta: FieldMetaInfo) -> Any:
         if isinstance(value, str):
             return value.strip()
         return value
 
@@ -34,40 +33,36 @@
 
 
 class MultiOrganization(MultiCheckbox):
     __name__ = '组织多选'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        required = '必填' if field_meta.required else '非必填'
-        extra_hint = field_meta.hint or '需按照组织架构树填写组织完整路径，如“XX公司/一级部门/二级部门”，多选时，选项之间用“、”连接'
-        return f"""必填性：{required} \n提示：{extra_hint}"""
+        return '\n'.join(
+            [
+                field_meta.comment_required,
+                f'提示：{field_meta.hint or "需按照组织架构树填写组织完整路径，如“XX公司/一级部门/二级部门”，多选时，选项之间用“、”连接"}',
+            ]
+        )
 
     @classmethod
     def serialize(cls, value: Any, field_meta: FieldMetaInfo) -> Any:
         return super().serialize(value, field_meta)
 
     @classmethod
-    def _validate(cls, v: Any, field_meta: FieldMetaInfo) -> list[str]:
-        return super()._validate(v, field_meta)
-
-    @classmethod
     def deserialize(cls, value: str | list[str] | None | Any, field_meta: FieldMetaInfo) -> str | Any:
         if value is None or value == '':
             return ''
+
         if isinstance(value, str):
             return value
 
         if isinstance(value, list):
-            rst: list[str] = []
-            for id_ in value:
-                id_ = OptionId(id_)
-                try:
-                    rst.append(field_meta.options_id_map[id_].name)
-                except KeyError:
-                    logging.warning('无法找到组织 %s 的选项, 返回原值', id_)
-                    rst.append(id_)
-            # pyright: reportUnknownArgumentType=false
-            return f'{MULTI_CHECKBOX_SEPARATOR}'.join(rst)
+            option_names = field_meta.exchange_option_ids_to_names(value)
+            return MULTI_CHECKBOX_SEPARATOR.join(map(str, option_names))
 
         logging.warning('%s 反序列化失败', cls.__name__)
         return value
+
+    @classmethod
+    def __validate__(cls, value: Any, field_meta: FieldMetaInfo) -> list[str]:
+        return super().__validate__(value, field_meta)
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/staff.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/staff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Any
 
 from excelalchemy.const import MULTI_CHECKBOX_SEPARATOR
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.identity import OptionId
-from excelalchemy.model.value_type.multi_checkbox import MultiCheckbox
-from excelalchemy.model.value_type.radio import Radio
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.identity import OptionId
+from excelalchemy.types.value.multi_checkbox import MultiCheckbox
+from excelalchemy.types.value.radio import Radio
 
 
 class SingleStaff(Radio):
     __name__ = '人员单选'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
@@ -35,43 +35,36 @@
 
 
 class MultiStaff(MultiCheckbox):
     __name__ = '人员多选'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        required = '必填' if field_meta.required else '非必填'
-        extra_hint = field_meta.hint or '请输入人员姓名和工号，如“张三/001”'
-        return f"""必填性：{required} \n提示：{extra_hint}"""
+        return '\n'.join(
+            [
+                field_meta.comment_required,
+                f'提示：{field_meta.hint or "请输入人员姓名和工号，如“张三/001”，多选时，选项之间用“、”连接"}',
+            ]
+        )
 
     @classmethod
     def serialize(cls, value: str | list[str] | Any, field_meta: FieldMetaInfo) -> Any:
-        if isinstance(value, str):
-            return value.strip()
-        if isinstance(value, list):
-            return MULTI_CHECKBOX_SEPARATOR.join(str(x) for x in value)
-        return value if value is not None else ''
+        return super().serialize(value, field_meta)
 
     @classmethod
-    def _validate(cls, v: Any, field_meta: FieldMetaInfo) -> list[str]:
-        return super()._validate(v, field_meta)
+    def __validate__(cls, value: Any, field_meta: FieldMetaInfo) -> list[str]:
+        return super().__validate__(value, field_meta)
 
     @classmethod
     def deserialize(cls, value: str | list[OptionId] | Any, field_meta: FieldMetaInfo) -> Any:
         if isinstance(value, str):
             return value
 
         if isinstance(value, list):
             if len(value) != len(set(value)):
                 raise ValueError('选项有重复')
-            rst: list[str] = []
-            for id_ in value:
-                id_ = OptionId(id_)
-                try:
-                    rst.append(field_meta.options_id_map[id_].name)
-                except KeyError:
-                    logging.warning('无法找到人员 %s 的选项, 返回原值', id_)
-                    rst.append(id_)
-            return f'{MULTI_CHECKBOX_SEPARATOR}'.join(rst)
+
+            option_names = field_meta.exchange_option_ids_to_names(value)
+            return f'{MULTI_CHECKBOX_SEPARATOR}'.join(option_names)
 
         logging.warning('%s 反序列化失败', cls.__name__)
         return value
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/string.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/string.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
-from excelalchemy.exception import ProgrammaticError
-from excelalchemy.model.abstract import ABCValueType
-from excelalchemy.model.abstract import CharacterSet
-from excelalchemy.model.abstract import FieldMetaInfo
+from excelalchemy.const import CharacterSet
+from excelalchemy.exc import ProgrammaticError
+from excelalchemy.types.abstract import ABCValueType
+from excelalchemy.types.field import FieldMetaInfo
 
 SPECIAL_SYMBOLS = set('!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~"。？！，、；：‘’“”（）《》〈〉【】〔〕｛｝｟｠〖〗〘〙〚〛〜〝〞〟〰–—‘‛“”„‟…‧﹏.')
 
 
 def _is_chinese_character(character: str) -> bool:
     # https://www.unicode.org/versions/Unicode15.0.0/ch18.pdf
     #
@@ -76,49 +76,54 @@
 def _format_character_set_names(cs: set[CharacterSet]) -> str:
     return '、'.join(_CHARACTER_SET_TO_NAME[c] for c in cs)
 
 
 class String(str, ABCValueType):
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        unique = '唯一' if field_meta.unique else '非唯一'
-        required = '必填' if field_meta.required else '非必填'
-        max_length = field_meta.importer_max_length or '无限制'
-        character_set = '中文、数字、大写字母、小写字母、符号'
-        extra_hint = field_meta.hint
-        return f'唯一性：{unique}\n必填性：{required}\n最大长度：{max_length}\n可输入内容：{character_set}' + (
-            f'\n提示: {extra_hint}' if extra_hint else ''
+        return '\n'.join(
+            [
+                field_meta.comment_unique,
+                field_meta.comment_required,
+                field_meta.comment_max_length,
+                '可输入内容:中文、数字、大写字母、小写字母、符号',
+                field_meta.comment_hint,
+            ]
         )
 
     @classmethod
     def serialize(cls, value: Any, field_meta: FieldMetaInfo) -> str:
         return str(value).strip()
 
     @classmethod
-    def _validate(cls, v: str, field_meta: FieldMetaInfo) -> str:
-        try:
-            parsed = str(v)
-        except Exception as exc:
-            raise ValueError('无法识别的输入') from exc
+    def deserialize(cls, value: str | None | Any, field_meta: FieldMetaInfo) -> str:
+        return str(value).strip() if value is not None else ''
 
+    # mccabe-complexity: 12
+    @classmethod
+    def __validate__(cls, value: str, field_meta: FieldMetaInfo) -> str:
+        parsed = str(value)
         errors: list[str] = []
 
         if field_meta.importer_max_length is not None:
             if len(parsed) > field_meta.importer_max_length:
                 errors.append(f'最长为{field_meta.importer_max_length}个字')
 
-        if field_meta.character_set is None:
-            raise ProgrammaticError('character_set 未设置')
-
-        for single_character in parsed:
-            if not any(_CHARACTER_SET_TO_VALIDATOR[cs](single_character) for cs in field_meta.character_set):
-                errors.append(f'仅允许输入{_format_character_set_names(field_meta.character_set)}')
-                break
+        errors.extend(cls.__check_character_set__(parsed, field_meta))
 
         if errors:
             raise ValueError(*errors)
         else:
             return parsed
 
     @classmethod
-    def deserialize(cls, value: str | None | Any, field_meta: FieldMetaInfo) -> str:
-        return str(value).strip() if value is not None else ''
+    def __check_character_set__(cls, value: str, field_meta: FieldMetaInfo) -> list[str]:
+        errors: list[str] = []
+        if field_meta.character_set is None:
+            raise ProgrammaticError('character_set 未设置')
+
+        for single_character in value:
+            if not any(_CHARACTER_SET_TO_VALIDATOR[cs](single_character) for cs in field_meta.character_set):
+                errors.append(f'仅允许输入{_format_character_set_names(field_meta.character_set)}')
+                break
+
+        return errors
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/tree.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/tree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 from typing import Any
 
-from excelalchemy.const import MULTI_CHECKBOX_SEPARATOR
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.identity import OptionId
-from excelalchemy.model.value_type.multi_checkbox import MultiCheckbox
-from excelalchemy.model.value_type.radio import Radio
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.value.multi_checkbox import MultiCheckbox
+from excelalchemy.types.value.radio import Radio
 
 
 class SingleTreeNode(Radio):
     __name__ = '树形单选'
 
     @classmethod
     def comment(cls, field_meta: FieldMetaInfo) -> str:
-        required = '必填' if field_meta.required else '非必填'
-        extra_hint = field_meta.hint or '请输入完整路径（包含根节点），层级之间用“/”连接，如“一级/二级/选项1”；多选时，选项之间用“，”连接'
-        return f"""必填性：{required} \n提示：{extra_hint}"""
+        return '\n'.join(
+            [
+                field_meta.comment_required,
+                f'提示：{field_meta.hint or "需按照组织架构树填写组织完整路径，如“XX公司/一级部门/二级部门”，多选时，选项之间用“、”连接"}',
+            ]
+        )
 
     @classmethod
     def serialize(cls, value: Any, field_meta: FieldMetaInfo) -> Any:
         if isinstance(value, str):
             return value.strip()
         return value
 
@@ -43,33 +44,9 @@
         return f"""必填性：{required} \n提示：{extra_hint}"""
 
     @classmethod
     def serialize(cls, value: Any, field_meta: FieldMetaInfo) -> Any:
         return super().serialize(value, field_meta)
 
     @classmethod
-    def _validate(cls, v: Any, field_meta: FieldMetaInfo) -> list[str]:
-        return super()._validate(v, field_meta)
-
-    @classmethod
-    def deserialize(cls, value: str | list[str] | None | Any, field_meta: FieldMetaInfo) -> str | Any:
-        if value is None or value == '':
-            return ''
-        if isinstance(value, str):
-            return value
-
-        if isinstance(value, list):
-            if len(value) != len(set(value)):
-                raise ValueError('选项有重复')
-            rst: list[str] = []
-            for id_ in value:
-                id_ = OptionId(id_)
-                try:
-                    rst.append(field_meta.options_id_map[id_].name)
-                except KeyError:
-                    logging.warning('无法找到树结点 %s 的选项, 返回原值', id_)
-                    rst.append(id_)
-            # pyright: reportUnknownArgumentType=false
-            return f'{MULTI_CHECKBOX_SEPARATOR}'.join(rst)
-
-        logging.warning('%s 反序列化失败', cls.__name__)
-        return value
+    def __validate__(cls, value: Any, field_meta: FieldMetaInfo) -> list[str]:
+        return super().__validate__(value, field_meta)
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/model/value_type/url.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/value/url.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from typing import Any
 
 from pydantic import BaseModel
 from pydantic import HttpUrl
 
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.value_type.string import String
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.value.string import String
 
 
 class HttpUrlValidator(BaseModel):
     url: HttpUrl
 
 
 class Url(String):
     @classmethod
-    def _validate(cls, v: Any, field_meta: FieldMetaInfo) -> str:
-        try:
-            parsed = str(v)
-        except Exception as exc:
-            raise ValueError('请输入正确的网址') from exc
-
+    def __validate__(cls, value: Any, field_meta: FieldMetaInfo) -> str:
+        parsed = str(value)
         errors: list[str] = []
 
         try:
             HttpUrlValidator.parse_obj({'url': parsed})
         except Exception:
             errors.append('请输入正确的网址')
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/plugin/esm/config.py` & `ExcelAlchemy-1.0.0/excelalchemy/types/alchemy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,123 @@
-import logging
+"""实例化 ExcelAlchemy 时的配置"""
 from dataclasses import dataclass
 from dataclasses import field
+from enum import Enum
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Generic
-from typing import Mapping
+from typing import Literal
+from typing import Type
 
-from esm_sdk.models import ESMScreen
 from minio import Minio
-from pydantic import BaseModel
 
-from excelalchemy.model.abstract import CreateImporterModelT
-from excelalchemy.model.abstract import Option
-from excelalchemy.model.abstract import UpdateImporterModelT
-from excelalchemy.model.excel import ContextT
-from excelalchemy.model.excel import ExcelExporterConfig
-from excelalchemy.model.excel import ExcelImporterConfig
-from excelalchemy.model.excel import ImportMode
+from excelalchemy.const import ContextT
+from excelalchemy.const import ExporterModelT
+from excelalchemy.const import ImporterCreateModelT
+from excelalchemy.const import ImporterUpdateModelT
+from excelalchemy.exc import ConfigError
+from excelalchemy.util.convertor import export_data_converter
+from excelalchemy.util.convertor import import_data_converter
+
+
+class ExcelMode(str, Enum):
+    """Excel 模式"""
+
+    IMPORT = 'IMPORT'
+    EXPORT = 'EXPORT'
+
+
+class ImportMode(str, Enum):
+    CREATE = 'CREATE'  # 创建
+    UPDATE = 'UPDATE'  # 更新
+    CREATE_OR_UPDATE = 'CREATE_OR_UPDATE'  # 创建或更新
 
 
 @dataclass
-class ESMExcelAlchemyImporterConfig(Generic[ContextT]):
-    auth_headers: Mapping[str, Any]  # x-authenticated-userid
-
-    primary_keys: list[str] = field(default_factory=list)  # 关键列
-    unique_keys: list[str] | None = field(default=None)  # 唯一列，关键列必定唯一，不用重复声明
-    # 对于支持 options 的类型字段，可以重新设置字段的 options, 如为人员和组织提供选项.
-    key_options: dict[str, list[Option]] | None = field(default=None)
-
-    # 创建模式下，字段的黑白名单。白名单字段必会导出，黑名单必会过滤
-    create_whitelist_keys: list[str] = field(default_factory=list)  # 关键列
-    create_blacklist_keys: list[str] = field(default_factory=list)  # 关键列
-
-    import_mode: ImportMode = field(default=ImportMode.CREATE)  # 导入模式
-
-    esm_url: str = field(default='http://esm-be:8000')  # esm url
-    create_template_id: str | None = field(default=None)  # 创建表单 Screen 的表单id
-    update_template_id: str | None = field(default=None)  # 更新表单 Screen 的模版id
+class ImporterConfig(Generic[ContextT, ImporterCreateModelT, ImporterUpdateModelT]):
+    create_importer_model: Type[ImporterCreateModelT] | None = field(default=None)
+    update_importer_model: Type[ImporterUpdateModelT] | None = field(default=None)
 
+    # Callable function receive Key as dict key instead of Label.
+    data_converter: Callable[[dict[str, Any]], dict[str, Any]] | None = field(default=import_data_converter)
     creator: Callable[[dict[str, Any], ContextT | None], Awaitable[Any]] | None = field(default=None)
     updater: Callable[[dict[str, Any], ContextT | None], Awaitable[Any]] | None = field(default=None)
-    is_data_exist: Callable[[dict[str, Any], ContextT | None], Awaitable[bool]] | None = field(default=None)
-    context: ContextT | None = field(default=None)
 
+    context: ContextT | None = field(default=None)
+    is_data_exist: Callable[[dict[str, Any], ContextT | None], Awaitable[bool]] | None = field(default=None)
     exec_formatter: Callable[[Exception], str] = field(default=str)
+
+    import_mode: ImportMode = field(default=ImportMode.CREATE)
+
     minio: Minio = field(default=None)
     bucket_name: str = field(default='excel')
     url_expires: int = field(default=3600)
 
-    create_screen: ESMScreen | None = field(default=None)
-    update_screen: ESMScreen | None = field(default=None)
+    sheet_name: Literal['Sheet1'] = field(default='Sheet1')
+
+    def validate_model(self):
+        if self.import_mode not in ImportMode.__members__.values():
+            raise ConfigError(f'导入模式 {self.import_mode} 不合法')
+
+        match self.import_mode:
+            case ImportMode.CREATE:
+                self._validate_create()
+            case ImportMode.UPDATE:
+                self._validate_update()
+            case ImportMode.CREATE_OR_UPDATE:
+                self._validate_create_or_update()
+
+        return self
+
+    # 创建模式验证
+    def _validate_create(self):
+        if self.import_mode != ImportMode.CREATE:
+            raise ConfigError(f'导入模式 {self.import_mode} 不合法')
+        if not self.create_importer_model:
+            raise ConfigError('当选择【创建模式】时，创建模型不能为空')
+
+    # 更新模式验证
+    def _validate_update(self):
+        if self.import_mode != ImportMode.UPDATE:
+            raise ConfigError(f'导入模式 {self.import_mode} 不合法')
+        if not self.update_importer_model:
+            raise ConfigError('当选择【更新模式】时，更新模型不能为空')
+
+    # 创建或更新模式验证
+    def _validate_create_or_update(self):
+        if self.import_mode != ImportMode.CREATE_OR_UPDATE:
+            raise ConfigError(f'导入模式 {self.import_mode} 不合法')
+
+        if not self.create_importer_model:
+            raise ConfigError('当选择【创建或更新模式】时，创建模型不能为空')
+        if not self.update_importer_model:
+            raise ConfigError('当选择【创建或更新模式】时，更新模型不能为空')
+        if not self.is_data_exist:
+            raise ConfigError('当选择【创建或更新模式】时，数据存在判断函数不能为空')
+        # 创建模型和更新模型的字段必须一致
+        if self.create_importer_model.__fields__.keys() != self.update_importer_model.__fields__.keys():
+            raise ConfigError('创建模型和更新模型的字段名称必须一致')
 
     def __post_init__(self):
-        if self.import_mode == ImportMode.CREATE:
-            if self.create_template_id is None:
-                raise ValueError('创建模式下，必须指定 create_template_id')
-            if self.update_template_id is not None:
-                logging.warning('创建模式下，指定 update_template_id 无效')
-        if self.import_mode == ImportMode.UPDATE:
-            if self.update_template_id is None:
-                raise ValueError('更新模式下，必须指定 update_template_id')
-            if self.create_template_id is not None:
-                logging.warning('更新模式下，指定 create_template_id 无效')
-        if self.import_mode == ImportMode.CREATE_OR_UPDATE:
-            if self.create_template_id is None or self.update_template_id is None:
-                raise ValueError('创建或更新模式下，必须指定 create_template_id 和 update_template_id ')
-
-    def to_excel_importer_config(
-        self,
-        create_importer: type[CreateImporterModelT] | None,
-        update_importer: type[UpdateImporterModelT] | None,
-    ) -> ExcelImporterConfig[ContextT, CreateImporterModelT, UpdateImporterModelT]:
-        return ExcelImporterConfig[ContextT, Any, Any](
-            import_mode=self.import_mode,
-            create_importer_model=create_importer,
-            update_importer_model=update_importer,
-            creator=self.creator,
-            updater=self.updater,
-            is_data_exist=self.is_data_exist,
-            # pyright: reportUnknownMemberType=false
-            # pyright: reportUnknownArgumentType=false
-            minio=self.minio,
-            bucket_name=self.bucket_name,
-            exec_formatter=self.exec_formatter,
-        )
+        self.validate_model()
 
 
 @dataclass
-class ESMExcelAlchemyExporterConfig(Generic[ContextT]):
-    auth_headers: Mapping[str, Any]  # x-authenticated-userid
-    template_id: str  # 导出 Screen 的表单id
-
-    primary_keys: list[str] = field(default_factory=list)
-    unique_keys: list[str] | None = field(default=None)
-    key_options: dict[str, list[Option]] | None = field(default=None)
-
-    esm_url: str = field(default='http://esm-be:8000')
-    context: ContextT | None = field(default=None)
+class ExporterConfig(Generic[ExporterModelT]):
+    exporter_model: Type[ExporterModelT]
+    # Callable function receive Key as dict key instead of Label.
+    data_converter: Callable[[dict[str, Any]], dict[str, Any]] | None = field(default=export_data_converter)
 
     minio: Minio = field(default=None)
     bucket_name: str = field(default='excel')
     url_expires: int = field(default=3600)
 
-    def to_excel_exporter_config(self, exporter: type[BaseModel]) -> ExcelExporterConfig[BaseModel]:
-        return ExcelExporterConfig[BaseModel](
-            exporter_model=exporter,
-            minio=self.minio,
-            bucket_name=self.bucket_name,
-        )
+    sheet_name: Literal['Sheet1'] = field(default='Sheet1')
+
+    def validate_model(self):
+        if not self.exporter_model:
+            raise ValueError('导出模型不能为空')
+        return self
+
+    def __post_init__(self):
+        self.validate_model()
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/tool/convertor.py` & `ExcelAlchemy-1.0.0/excelalchemy/util/convertor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import re
 from typing import Any
 
 from excelalchemy.const import FIELD_DATA_KEY
-from excelalchemy.model.identity import Key
+from excelalchemy.types.identity import Key
 
 
-def import_data_converter(data: dict[str, Any]) -> dict[str, Any]:
+def import_data_converter(data: dict[str, Any]) -> dict[str, Any]:  # noqa: C901
     # _to_snake_case
     result: dict[str, Any] = {}
     for k, v in data.items():
         snake_keys = [_to_snake_case(key) for key in k.split('.')]
         _nested_set(result, snake_keys, v)
     return result
 
 
-def export_data_converter(data: dict[str, Any]) -> dict[str, Any]:
+def export_data_converter(data: dict[str, Any], to_camel: bool = False) -> dict[str, Any]:  # noqa: C901
     result: dict[str, Any] = {}
     for k, v in data.items():
-        camel_key = _to_camel_case(k)
+        camel_key = _to_camel_case(k) if to_camel else _to_snake_case(k)
         if camel_key != FIELD_DATA_KEY:
             result[camel_key] = v
             continue
         if not v:
             continue
 
         for field_key, field_value in v.items():
```

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/util.py` & `ExcelAlchemy-1.0.0/excelalchemy/util/file.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-0.1a2/excelalchemy/writer.py` & `ExcelAlchemy-1.0.0/excelalchemy/core/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """负责将 pandas 写入 Excel 文件"""
 import base64
 from collections import defaultdict
 from math import ceil
 from tempfile import NamedTemporaryFile
+from typing import Any
 from typing import BinaryIO
 from typing import cast
 
 from openpyxl.comments import Comment
 from openpyxl.styles import Alignment
 from openpyxl.styles import Font
 from openpyxl.styles import PatternFill
@@ -21,25 +22,25 @@
 from excelalchemy.const import BACKGROUND_REQUIRED_COLOR
 from excelalchemy.const import CHARACTER_WIDTH
 from excelalchemy.const import DEFAULT_SHEET_NAME
 from excelalchemy.const import FONT_READ_COLOR
 from excelalchemy.const import HEADER_HINT
 from excelalchemy.const import REASON_COLUMN_LABEL
 from excelalchemy.const import RESULT_COLUMN_LABEL
-from excelalchemy.exception import ExcelCellError
-from excelalchemy.model.abstract import FieldMetaInfo
-from excelalchemy.model.identity import Base64Str
-from excelalchemy.model.identity import ColumnIndex
-from excelalchemy.model.identity import Label
-from excelalchemy.model.identity import RowIndex
-from excelalchemy.model.identity import UniqueLabel
-from excelalchemy.model.result import ImportRowResult
-from excelalchemy.model.value_type import EXCEL_CHOICE_VALUE_TYPE
-from excelalchemy.util import add_excel_prefix
-from excelalchemy.util import value_is_nan
+from excelalchemy.exc import ExcelCellError
+from excelalchemy.types.field import FieldMetaInfo
+from excelalchemy.types.identity import Base64Str
+from excelalchemy.types.identity import ColumnIndex
+from excelalchemy.types.identity import Label
+from excelalchemy.types.identity import RowIndex
+from excelalchemy.types.identity import UniqueLabel
+from excelalchemy.types.result import ValidateRowResult
+from excelalchemy.types.value import EXCEL_CHOICE_VALUE_TYPE
+from excelalchemy.util.file import add_excel_prefix
+from excelalchemy.util.file import value_is_nan
 
 # pandas 认为 Excel 的第一行是 0, 第一列是 0
 PANDAS_EXCEL_INDEX_START_AT = 0
 PANDAS_WRITE_START_AT = PANDAS_EXCEL_INDEX_START_AT + 1  # 从第二行开始写入数据,第一行写入 HEADER_HINT
 
 # openpyxl 认为 Excel 的第一行是 1, 第一列是 1
 OPENPYXL_EXCEL_INDEX_START_AT = 1  # Excel 从 1 开始
@@ -157,43 +158,21 @@
 
     if close_file:
         writer.close()
 
     return file
 
 
-def _write_merged_header(
+def _write_vertically_merged_header(
+    start_row: int,
     df: DataFrame,
+    column_write_offset: int,
     field_meta_mapping: dict[UniqueLabel, FieldMetaInfo],
-    file: BinaryIO,
-    sheet_name: str,
-    column_write_offset: int = 0,
-    row_write_offset: int = 0,
-    close_file: bool = True,
-    writer: ExcelWriter | None = None,
-) -> BinaryIO:
-    """写入含有合并的表头"""
-
-    writer = writer or ExcelWriter(file, engine='openpyxl')
-    worksheet: Worksheet = writer.sheets[sheet_name]
-
-    # 写入注释需要在合并表头之前
-    _write_simple_header(
-        df,
-        field_meta_mapping,
-        file,
-        sheet_name,
-        column_write_offset,
-        row_write_offset,
-        close_file=False,
-        writer=writer,
-        option_start_at=OPENPYXL_EXCEL_INDEX_START_AT + HEADER_HINT_LINE_COUNT + MERGE_HEADER_ROW_COUNT,
-    )
-    # 第一遍遍历，找出纵向合并的单元格
-    start_row = row_write_offset + OPENPYXL_EXCEL_INDEX_START_AT
+    worksheet: Worksheet,
+):
     for openpyxl_col_index, column in enumerate(
         df.columns[column_write_offset:],
         start=column_write_offset + OPENPYXL_EXCEL_INDEX_START_AT,
     ):
         field_meta = field_meta_mapping[column]
         if field_meta.label == field_meta.parent_label:
             # 如果 label 和 parent_label 相同，说明需要上下合并
@@ -204,15 +183,23 @@
                 end_column=openpyxl_col_index + column_write_offset,
             )
         worksheet.cell(
             row=start_row,
             column=openpyxl_col_index + column_write_offset,
         ).number_format = numbers.FORMAT_TEXT
 
-    # 第二遍遍历，找出横向合并的单元格
+
+def _write_horizontally_merged_header(
+    start_row: int,
+    df: DataFrame,
+    column_write_offset: int,
+    field_meta_mapping: dict[UniqueLabel, FieldMetaInfo],
+    worksheet: Worksheet,
+) -> None:
+    """写入横向合并的表头"""
     counter: dict[Label, int] = defaultdict(int)
     for field_meta in field_meta_mapping.values():
         if field_meta.parent_label is None:
             raise RuntimeError('运行时 parent_label 不能为空')
         counter[field_meta.parent_label] += 1
 
     for openpyxl_col_index, column in enumerate(
@@ -232,59 +219,81 @@
             worksheet.merge_cells(
                 start_row=start_row,
                 start_column=openpyxl_col_index + column_write_offset,
                 end_row=start_row,
                 end_column=openpyxl_col_index + column_write_offset + counter[field_meta.parent_label] - 1,
             )
 
+
+def _write_merged_header(  # pragma: no mccabe
+    df: DataFrame,
+    field_meta_mapping: dict[UniqueLabel, FieldMetaInfo],
+    file: BinaryIO,
+    sheet_name: str,
+    column_write_offset: int = 0,
+    row_write_offset: int = 0,
+    close_file: bool = True,
+    writer: ExcelWriter | None = None,
+) -> BinaryIO:
+    """写入含有合并的表头"""
+
+    writer = writer or ExcelWriter(file, engine='openpyxl')
+    worksheet: Worksheet = writer.sheets[sheet_name]
+
+    # 写入注释需要在合并表头之前
+    _write_simple_header(
+        df,
+        field_meta_mapping,
+        file,
+        sheet_name,
+        column_write_offset,
+        row_write_offset,
+        close_file=False,
+        writer=writer,
+        option_start_at=OPENPYXL_EXCEL_INDEX_START_AT + HEADER_HINT_LINE_COUNT + MERGE_HEADER_ROW_COUNT,
+    )
+    # 第一遍遍历，找出纵向合并的单元格
+    start_row = row_write_offset + OPENPYXL_EXCEL_INDEX_START_AT
+    _write_vertically_merged_header(start_row, df, column_write_offset, field_meta_mapping, worksheet)
+    # 第二遍遍历，找出横向合并的单元格
+    _write_horizontally_merged_header(start_row, df, column_write_offset, field_meta_mapping, worksheet)
+
     if close_file:
         writer.close()
 
     return file
 
 
 def _get_parsed_value(
     df: DataFrame,
     row_index: int,
     col_index: int,
     field_meta_mapping: dict[UniqueLabel, FieldMetaInfo],
 ) -> str:
     """用于把 pandas 读取的 Excel 之后的数据，转回用户可识别的数据"""
 
-    cell_value = df.iloc[row_index, col_index]
+    cell_value: str | Any | None = df.iloc[row_index, col_index]
 
-    if cell_value is None or value_is_nan(cell_value):
+    if value_is_nan(cell_value):
         return ''  # parse None for end-user
     col_label = cast(UniqueLabel, df.columns[col_index])
     if col_label not in field_meta_mapping:
         return str(cell_value)
     field_meta = field_meta_mapping[col_label]
     cell_value = field_meta.value_type.deserialize(cell_value, field_meta)
 
     return str(cell_value)
 
 
-# pylint: disable=too-many-locals
-def _write_value_mark_error(
-    df: DataFrame,
+def _mark_error(
+    worksheet: Worksheet,
     errors: dict[RowIndex, dict[ColumnIndex, list[ExcelCellError]]],
-    field_meta_mapping: dict[UniqueLabel, FieldMetaInfo],
-    file: BinaryIO,
-    sheet_name: str,
-    row_write_offset: int = 0,
-    column_write_offset: int = 0,
-    close_file: bool = True,
-    writer: ExcelWriter | None = None,
-    pands_data_start_index: int = 0,
-) -> BinaryIO:
-    """写入错误标记，并把对应位置标红"""
-
-    writer = writer or ExcelWriter(file, engine='openpyxl')
-    worksheet: Worksheet = writer.sheets[sheet_name]
-
+    column_write_offset: int,
+    row_write_offset: int,
+):
     for row_index, cols in errors.items():
         for col_index, exceptions in cols.items():
             if not exceptions:
                 continue
 
             openpyxl_col_index = col_index + column_write_offset + OPENPYXL_EXCEL_INDEX_START_AT
             openpyxl_row_index = row_index + row_write_offset + OPENPYXL_EXCEL_INDEX_START_AT
@@ -294,25 +303,34 @@
             cell.fill = PatternFill(
                 start_color=BACKGROUND_ERROR_COLOR,
                 end_color=BACKGROUND_ERROR_COLOR,
                 fill_type='solid',
             )
             cell.alignment = Alignment(wrap_text=True)
 
+
+def _write_value(
+    df: DataFrame,
+    worksheet: Worksheet,
+    field_meta_mapping: dict[UniqueLabel, FieldMetaInfo],
+    pands_data_start_index: int,
+    column_write_offset: int,
+    row_write_offset: int,
+) -> None:
     col_width_mapping: dict[ColumnIndex, float] = defaultdict(float)
     for row_index_ in range(pands_data_start_index, df.shape[0]):  # iterate over rows
         for column_index_ in range(df.shape[1]):  # iterate over columns
             openpyxl_col_index = column_index_ + column_write_offset + OPENPYXL_EXCEL_INDEX_START_AT
             openpyxl_row_index = row_index_ + row_write_offset + OPENPYXL_EXCEL_INDEX_START_AT
 
             cell = worksheet.cell(row=openpyxl_row_index, column=openpyxl_col_index)
             cell.value = _get_parsed_value(df, row_index_, column_index_, field_meta_mapping)
             cell.number_format = numbers.FORMAT_TEXT
             cell.alignment = Alignment(horizontal='left', vertical='center', wrap_text=True)
-            if RESULT_COLUMN_LABEL == df.columns[column_index_] and cell.value == str(ImportRowResult.FAIL):
+            if RESULT_COLUMN_LABEL == df.columns[column_index_] and cell.value == str(ValidateRowResult.FAIL):
                 cell.font = Font(color=FONT_READ_COLOR)  # 设置文字颜色为红色
             if REASON_COLUMN_LABEL == df.columns[column_index_]:
                 cell.alignment = Alignment(horizontal='left', vertical='center', wrap_text=True)
 
             col_width_mapping[ColumnIndex(openpyxl_col_index)] = max(
                 col_width_mapping[ColumnIndex(openpyxl_col_index)],
                 max(len(str(x)) for x in str(cell.value).split('\n')),
@@ -320,14 +338,49 @@
             )
 
     for openpyxl_col_index, width in col_width_mapping.items():
         worksheet.column_dimensions[get_column_letter(openpyxl_col_index)].width = round(
             (width + 4) * CHARACTER_WIDTH, 2
         )
 
+
+# pylint: disable=too-many-locals
+def _write_value_mark_error(  # pragma: no mccabe
+    df: DataFrame,
+    errors: dict[RowIndex, dict[ColumnIndex, list[ExcelCellError]]],
+    field_meta_mapping: dict[UniqueLabel, FieldMetaInfo],
+    file: BinaryIO,
+    sheet_name: str,
+    row_write_offset: int = 0,
+    column_write_offset: int = 0,
+    close_file: bool = True,
+    writer: ExcelWriter | None = None,
+    pands_data_start_index: int = 0,
+) -> BinaryIO:
+    """写入错误标记，并把对应位置标红"""
+
+    writer = writer or ExcelWriter(file, engine='openpyxl')
+    worksheet: Worksheet = writer.sheets[sheet_name]
+
+    _mark_error(
+        worksheet=worksheet,
+        errors=errors,
+        column_write_offset=column_write_offset,
+        row_write_offset=row_write_offset,
+    )
+
+    _write_value(
+        df=df,
+        worksheet=worksheet,
+        field_meta_mapping=field_meta_mapping,
+        pands_data_start_index=pands_data_start_index,
+        row_write_offset=row_write_offset,
+        column_write_offset=column_write_offset,
+    )
+
     if close_file:
         writer.close()
     return file
 
 
 def render_simple_header_excel(
     df: DataFrame,
```

### Comparing `ExcelAlchemy-0.1a2/pyproject.toml` & `ExcelAlchemy-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,26 @@
 [tool.flit.module]
 name = "excelalchemy"
 
 [project.urls]
 Home = "https://github.com/SundayWindy/excelalchemy"
 
 [project.optional-dependencies]
-development = ["pandas-stubs", "black", "isort", "mypy", "pylint", "pre-commit"]
+development = [
+    "pandas-stubs",
+    "black",
+    "isort",
+    "mypy",
+    "pylint",
+    "pre-commit",
+    "pyright",
+    "pytest",
+    "coverage",
+    "pytest-cov",
+]
 
 [tool.pyright]
 exclude = [
     ".venv",
     "venv",
     ".git",
     "**/.mypy_cache",
@@ -80,16 +91,23 @@
 ignore-paths = [
     ".git/",
     "venv/",
     ".venv/",
     ".mypy_cache/",
     "__pycache__/",
     ".pytest_cache/",
+    "tests/",
+    "dist/",
+]
+extension-pkg-whitelist = [
+    "pydantic",
+    "pandas",
+    "pendulum",
+
 ]
-extension-pkg-whitelist = ["pydantic"]
 
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
```

