# Comparing `tmp/drf_pipeline_views-0.8.5.tar.gz` & `tmp/drf_pipeline_views-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pipeline_views-0.8.5.tar", max compression
+gzip compressed data, was "drf_pipeline_views-0.9.0.tar", max compression
```

## Comparing `drf_pipeline_views-0.8.5.tar` & `drf_pipeline_views-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-01-29 16:49:35.422343 drf_pipeline_views-0.8.5/LICENSE
--rw-r--r--   0        0        0     3754 2023-01-29 16:49:35.422343 drf_pipeline_views-0.8.5/README.md
--rw-r--r--   0        0        0      356 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/__init__.py
--rw-r--r--   0        0        0      478 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/exceptions.py
--rw-r--r--   0        0        0     9305 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/inference.py
--rw-r--r--   0        0        0     3542 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/meta.py
--rw-r--r--   0        0        0        0 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/py.typed
--rw-r--r--   0        0        0    41214 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/schema.py
--rw-r--r--   0        0        0     4805 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/serializers.py
--rw-r--r--   0        0        0     1500 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/typing/__init__.py
--rw-r--r--   0        0        0     3599 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/typing/general.py
--rw-r--r--   0        0        0    37148 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/typing/openapi.py
--rw-r--r--   0        0        0     4020 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/utils.py
--rw-r--r--   0        0        0     6908 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pipeline_views/views.py
--rw-r--r--   0        0        0     4263 2023-01-29 16:49:35.426343 drf_pipeline_views-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     4810 1970-01-01 00:00:00.000000 drf_pipeline_views-0.8.5/setup.py
--rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 drf_pipeline_views-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3754 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/README.md
+-rw-r--r--   0        0        0      193 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/exceptions.py
+-rw-r--r--   0        0        0     3554 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/meta.py
+-rw-r--r--   0        0        0        0 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/py.typed
+-rw-r--r--   0        0        0     3889 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/serializers.py
+-rw-r--r--   0        0        0     1584 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/typing.py
+-rw-r--r--   0        0        0     3762 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/utils.py
+-rw-r--r--   0        0        0     6822 2023-05-06 13:01:05.761154 drf_pipeline_views-0.9.0/pipeline_views/views.py
+-rw-r--r--   0        0        0     4423 2023-05-06 13:01:05.765154 drf_pipeline_views-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 drf_pipeline_views-0.9.0/PKG-INFO
```

### Comparing `drf_pipeline_views-0.8.5/LICENSE` & `drf_pipeline_views-0.9.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Matti Lamppu
+Copyright (c) 2023 Matti Lamppu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `drf_pipeline_views-0.8.5/README.md` & `drf_pipeline_views-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `drf_pipeline_views-0.8.5/pipeline_views/meta.py` & `drf_pipeline_views-0.9.0/pipeline_views/meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ListSerializer,
     ManyRelatedField,
     ReadOnlyField,
     RelatedField,
     Serializer,
 )
 
-from .typing import TYPE_CHECKING, ClassVar, Dict, List, Set, Type, Union
+from .typing import TYPE_CHECKING, Any, ClassVar, Union
 
 if TYPE_CHECKING:
     from .views import BasePipelineView
 
 
 __all__ = [
     "PipelineMetadata",
@@ -24,17 +24,17 @@
 
 class PipelineMetadata(SimpleMetadata):
     """Metadata class that adds input and output info for
     each of the attached views methods based on
     the serializers for that method.
     """
 
-    recognized_methods: ClassVar[Set[str]] = {"GET", "POST", "PUT", "PATCH", "DELETE"}
-    skip_fields: ClassVar[Set[Type[Field]]] = {ReadOnlyField, HiddenField, SerializerMethodField}
-    used_attrs: ClassVar[List[str]] = ["label", "help_text", "min_length", "max_length", "min_value", "max_value"]
+    recognized_methods: ClassVar[set[str]] = {"GET", "POST", "PUT", "PATCH", "DELETE"}
+    skip_fields: ClassVar[set[type[Field]]] = {ReadOnlyField, HiddenField, SerializerMethodField}
+    used_attrs: ClassVar[list[str]] = ["label", "help_text", "min_length", "max_length", "min_value", "max_value"]
 
     def determine_actions(self, request: Request, view: "BasePipelineView"):
         """Return information about the fields that are accepted for methods in self.recognized_methods."""
         actions = {}
         for method in self.recognized_methods & set(view.allowed_methods):
             view.request = clone_request(request, method)
 
@@ -46,30 +46,30 @@
                 "output": self.get_serializer_info(output_serializer),
             }
 
             view.request = request
 
         return actions
 
-    def get_serializer_info(self, serializer: Serializer) -> Union[Dict, List]:
+    def get_serializer_info(self, serializer: Serializer) -> Union[dict[Any, Any], list[Any]]:
         """Given an instance of a serializer, return a dictionary of metadata about its fields."""
         data_serializer = getattr(serializer, "child", serializer)
 
         input_data = {
             field_name: self.get_field_info(field)
             for field_name, field in data_serializer.fields.items()
             if not any(isinstance(field, field_type) for field_type in self.skip_fields)
         }
 
         if isinstance(serializer, ListSerializer):
             input_data = [input_data]
 
         return input_data
 
-    def get_field_info(self, field: Union[Field, Serializer, ListSerializer]) -> Union[Dict, List]:
+    def get_field_info(self, field: Union[Field, Serializer, ListSerializer]) -> Union[dict[Any, Any], list[Any]]:
         if getattr(field, "child", False):
             if isinstance(field, DictField):
                 return {"<key>": self.get_field_info(field.child)}
             return [self.get_field_info(field.child)]
 
         if getattr(field, "fields", False):
             return self.get_serializer_info(field)
```

### Comparing `drf_pipeline_views-0.8.5/pipeline_views/serializers.py` & `drf_pipeline_views-0.9.0/pipeline_views/serializers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,23 @@
 from django.utils.functional import cached_property
 from rest_framework import serializers
 from rest_framework.exceptions import ErrorDetail, ValidationError
 from rest_framework.request import Request
 from rest_framework.settings import api_settings
 
-from .typing import Any, ClassVar, Dict, List, Optional, Type, Union
+from .typing import Any, ClassVar, Optional
 
 __all__ = [
     "CookieSerializerMixin",
-    "EmptySerializer",
     "HeaderAndCookieSerializer",
     "HeaderSerializerMixin",
-    "MockSerializer",
     "RequestFromContextMixin",
 ]
 
 
-class EmptySerializer(serializers.Serializer):
-    # Used for schema 204 responses
-    pass
-
-
-class MockSerializer(serializers.Serializer):
-    # Serializer that simply passes initial data to output.
-
-    _example: Union[List[Any], Dict[str, Any], Any] = {}
-
-    @classmethod
-    def with_example(cls, description: str, response: Union[List[Any], Dict[str, Any], Any]) -> Type["MockSerializer"]:
-        """Sets OpenAPI example response."""
-        new_cls = type(MockSerializer.__name__, (cls,), {"_example": response})  # type: ignore
-        new_cls.__doc__ = description
-        return new_cls  # type: ignore
-
-    def to_internal_value(self, data: Any) -> Dict[str, Any]:
-        return self.initial_data  # type: ignore
-
-    def to_representation(self, instance: Any) -> Dict[str, Any]:
-        return self.initial_data  # type: ignore
-
-
 class RequestFromContextMixin:
     @cached_property
     def request_from_context(self) -> Request:
         request: Optional[Request] = self.context.get("request")
         if request is None or not isinstance(request, Request):
             raise ValidationError(
                 {
@@ -53,80 +27,78 @@
                     )
                 }
             )
         return request
 
 
 class HeaderSerializerMixin(RequestFromContextMixin):
-
-    take_from_headers: ClassVar[List[str]] = []
+    take_from_headers: ClassVar[list[str]] = []
     """Headers to take values from.
     Header names will be converted to snake_case.
     """
 
     @cached_property
-    def header_values(self) -> Dict[str, Any]:
+    def header_values(self) -> dict[str, Any]:
         request = self.request_from_context
         return {key.replace("-", "_").lower(): request.headers.get(key, None) for key in self.take_from_headers}
 
-    def add_headers(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    def add_headers(self, data: dict[str, Any]) -> dict[str, Any]:
         # Remove any values added to original header names.
         for key in self.take_from_headers:
             data.pop(key, None)
         data.update(self.header_values)
         return data
 
-    def to_internal_value(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    def to_internal_value(self, data: dict[str, Any]) -> dict[str, Any]:
         ret = super().to_internal_value(data)
         ret = self.add_headers(ret)
         return ret
 
-    def to_representation(self, instance) -> Dict[str, Any]:
+    def to_representation(self, instance) -> dict[str, Any]:
         ret = super().to_representation(instance)
         ret = self.add_headers(ret)
         return ret
 
 
 class CookieSerializerMixin(RequestFromContextMixin):
-
-    take_from_cookies: ClassVar[List[str]] = []
+    take_from_cookies: ClassVar[list[str]] = []
     """Cookies to take values from.
     Cookie names will be converted to snake_case.
     """
 
     @cached_property
-    def cookie_values(self) -> Dict[str, Any]:
+    def cookie_values(self) -> dict[str, Any]:
         request = self.request_from_context
         return {key.replace("-", "_").lower(): request.COOKIES.get(key, None) for key in self.take_from_cookies}
 
-    def add_cookies(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    def add_cookies(self, data: dict[str, Any]) -> dict[str, Any]:
         # Remove any values added to original cookie names.
         for key in self.take_from_cookies:
             data.pop(key, None)
         data.update(self.cookie_values)
         return data
 
-    def to_internal_value(self, data: Dict[str, Any]) -> Dict[str, Any]:
+    def to_internal_value(self, data: dict[str, Any]) -> dict[str, Any]:
         ret = super().to_internal_value(data)
         ret = self.add_cookies(ret)
         return ret
 
-    def to_representation(self, instance) -> Dict[str, Any]:
+    def to_representation(self, instance) -> dict[str, Any]:
         ret = super().to_representation(instance)
         ret = self.add_cookies(ret)
         return ret
 
 
 class HeaderAndCookieSerializer(HeaderSerializerMixin, CookieSerializerMixin, serializers.Serializer):
     """Serializer that adds the specified headers and cookies from request to the serializer data.
     Serializer must have the incoming request object in its context dictionary.
     If the specified header or cookie is not found in the request, the value will be None.
     """
 
     @cached_property
-    def fields(self) -> Dict[str, serializers.Field]:
+    def fields(self) -> dict[str, serializers.Field]:
         fields = super().fields
         for header_name in self.take_from_headers:
             fields[header_name] = serializers.CharField(default=None, allow_null=True, allow_blank=True)
         for cookie_name in self.take_from_cookies:
             fields[cookie_name] = serializers.CharField(default=None, allow_null=True, allow_blank=True)
         return fields
```

### Comparing `drf_pipeline_views-0.8.5/pipeline_views/utils.py` & `drf_pipeline_views-0.9.0/pipeline_views/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import re
 from contextlib import contextmanager
 from functools import wraps
 from itertools import chain
 
 from django.conf import settings
 from django.utils.translation import get_language as current_language
 from django.utils.translation import override
@@ -18,68 +17,64 @@
 
 from .typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     DataDict,
     Generator,
+    GenericView,
     HTTPMethod,
-    List,
     LogicCallable,
     Optional,
     ParamSpec,
     SerializerType,
-    Tuple,
     TypeGuard,
     TypeVar,
     Union,
-    ViewMethod,
 )
 
 if TYPE_CHECKING:
     from .views import BasePipelineView
 
 
 __all__ = [
     "get_language",
-    "get_path_parameters",
     "get_view_method",
     "is_pydantic_model",
     "is_serializer_class",
     "run_parallel",
     "Sentinel",
     "translate",
 ]
 
 
 T = TypeVar("T")
 P = ParamSpec("P")
-url_variables_pattern = re.compile("{([^}]+)}")
 
 
 class Sentinel:
     """Sentinel value."""
 
 
 def is_serializer_class(obj: Any) -> TypeGuard[BaseSerializer]:
     return isinstance(obj, type) and issubclass(obj, BaseSerializer)
 
 
 def is_pydantic_model(obj: Any):
-    if BaseModel is None:
-        return False  # pragma: no cover
+    if BaseModel is None:  # pragma: no cover
+        return False
 
     return isinstance(obj, type) and issubclass(obj, BaseModel)
 
 
 def get_language(request: Request) -> str:
     """Get language based on request Accept-Language header or 'lang' query parameter."""
     lang: Optional[str] = request.query_params.get("lang")
     language_code: Optional[str] = getattr(request, "LANGUAGE_CODE", None)
-    available_languages: List[str] = [key for (key, value) in settings.LANGUAGES]
+    available_languages: list[str] = [key for (key, value) in settings.LANGUAGES]
 
     if lang and lang in available_languages:
         return lang
     if language_code and language_code in available_languages:
         return language_code
 
     return current_language()
@@ -112,19 +107,19 @@
     def context_manager(request: Request) -> Generator[Any, Any, None]:
         with override(get_language(request)):
             yield
 
     return context_manager(item)
 
 
-async def run_parallel(step: Tuple[Union[LogicCallable, SerializerType], ...], data: DataDict) -> Tuple[DataDict, ...]:
+async def run_parallel(step: tuple[Union[LogicCallable, SerializerType], ...], data: DataDict) -> tuple[DataDict, ...]:
     return await asyncio.gather(*(task(**data) for task in step))  # noqa
 
 
-def get_view_method(method: HTTPMethod) -> ViewMethod:
+def get_view_method(method: HTTPMethod) -> GenericView:
     source = "query_params" if method == "GET" else "data"
 
     def inner(
         self: "BasePipelineView",
         request: Request,
         *args: Any,
         **kwargs: Any,
@@ -135,12 +130,7 @@
                 for key, value in getattr(request, source, {}).items()
                 if key not in getattr(self, f"ignored_{method.lower()}_params", set())
             }
         )
         return self.process_request(data=kwargs)
 
     return inner  # type: ignore
-
-
-def get_path_parameters(path: str) -> Generator[str, Any, None]:
-    for match in url_variables_pattern.finditer(path):
-        yield match.groups()[0]
```

### Comparing `drf_pipeline_views-0.8.5/pipeline_views/views.py` & `drf_pipeline_views-0.9.0/pipeline_views/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 import asyncio
 
 from asgiref.sync import async_to_sync
+from openapi_schema.schema import APISchema
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_framework.views import APIView
+from serializer_inference import serializer_from_callable
 
 from .exceptions import NextLogicBlock
-from .inference import serializer_from_callable
 from .meta import PipelineMetadata
-from .schema import PipelineSchema
 from .typing import (
     Any,
     ClassVar,
     DataDict,
     DataReturn,
     Iterable,
     Optional,
     PipelineLogic,
     PipelinesDict,
     SerializerType,
-    Set,
-    Tuple,
     ViewContext,
 )
 from .utils import Sentinel, get_view_method, is_pydantic_model, is_serializer_class, run_parallel, translate
 
 __all__ = [
     "BasePipelineView",
 ]
 
 
 class BasePipelineView(APIView):
-
     pipelines: ClassVar[PipelinesDict] = {}
     """Dictionary describing the HTTP method pipelines."""
 
-    schema = PipelineSchema()
+    schema = APISchema()
     metadata_class = PipelineMetadata
 
-    ignored_get_params: ClassVar[Set[str]] = {"lang", "format"}
-    ignored_post_params: ClassVar[Set[str]] = {"csrfmiddlewaretoken", "lang", "format"}
-    ignored_put_params: ClassVar[Set[str]] = {"lang", "format"}
-    ignored_patch_params: ClassVar[Set[str]] = {"lang", "format"}
-    ignored_delete_params: ClassVar[Set[str]] = {"lang", "format"}
+    ignored_get_params: ClassVar[set[str]] = {"lang", "format"}
+    ignored_post_params: ClassVar[set[str]] = {"csrfmiddlewaretoken", "lang", "format"}
+    ignored_put_params: ClassVar[set[str]] = {"lang", "format"}
+    ignored_patch_params: ClassVar[set[str]] = {"lang", "format"}
+    ignored_delete_params: ClassVar[set[str]] = {"lang", "format"}
 
     def __new__(cls, *args, **kwargs):
         for key in cls.pipelines:
             if not hasattr(cls, key.lower()):
                 setattr(cls, key.lower(), get_view_method(key))
 
         return super().__new__(cls)
@@ -76,15 +73,14 @@
             if asyncio.iscoroutinefunction(logic):
                 logic = async_to_sync(logic)
 
             return logic(**data)
 
         try:
             for step in logic:
-
                 # Conditional logic path
                 if isinstance(data, tuple):
                     key, data = data
                     try:
                         step = step[key]
                     except (KeyError, TypeError) as error:
                         raise TypeError(f"Next logic step doesn't have a conditional logic path '{key}'.") from error
@@ -96,22 +92,19 @@
                 # Pydantic Model
                 elif is_pydantic_model(step):
                     data = self.run_model(model_class=step, data=data)
 
                 # Parallel block
                 elif isinstance(step, tuple):
                     old_kwargs: Optional[DataDict] = None
-                    try:
-                        step.index(...)
+                    if ... in step:
                         step = tuple(task for task in step if task is not ...)
                         old_kwargs = data
-                    except ValueError:
-                        pass
 
-                    results: Tuple[DataDict, ...] = async_to_sync(run_parallel)(step, data)
+                    results: tuple[DataDict, ...] = async_to_sync(run_parallel)(step, data)
                     data = {key: value for result in results for key, value in result.items()}
 
                     if old_kwargs is not None:
                         old_kwargs.update(data)
                         data = old_kwargs
 
                 # Logic block or callable
@@ -166,18 +159,18 @@
                 *_, step = step
             else:
                 step = next(iter(step))
 
         if is_serializer_class(step):
             return step
 
-        if is_pydantic_model(step):
+        if is_pydantic_model(step):  # pragma: no cover
             return serializer_from_callable(step)
 
         if callable(step):
             return serializer_from_callable(step, output=output)
 
         raise TypeError("Only Serializers and callables are supported in the pipeline.")
 
     def get_serializer_context(self) -> ViewContext:
-        """Return serializer context, mainly for browerable api."""
+        """Return serializer context, mainly for browsable api."""
         return {"request": self.request, "format": self.format_kwarg, "view": self}
```

### Comparing `drf_pipeline_views-0.8.5/pyproject.toml` & `drf_pipeline_views-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pipeline-views"
-version = "0.8.5"
+version = "0.9.0"
 description = "Django REST framework views using the pipeline pattern."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "pipeline_views" },
 ]
@@ -21,23 +21,21 @@
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Framework :: Django :: 3.0",
-    "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "Natural Language :: English",
 ]
 include = [
     "README.md",
     "LICENSE",
 ]
@@ -45,65 +43,62 @@
     "tests",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MrThearMan/drf-pipeline-views/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4"
-Django = ">=3.0"
+python = ">=3.9,<4"
+Django = ">=3.2"
 djangorestframework = ">=3.12.0"
+drf-serializer-inference = ">=0.0.2"
+drf-openapi-schema = ">=0.0.3"
 asgiref = ">=3.5.0"
 PyYAML = ">=6.0"
-typing-extensions = {version = ">=4.4.0", python = "<3.11"}
+typing-extensions = {version = ">=4.4.0", python = "<3.10"}
 pydantic = {version = ">=1.6.2", optional = true}
 uvloop = {version = ">=0.16.0", optional = true}
+uritemplate = {version = ">=4.1.1", optional = true}
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.2.1"
+pytest = "7.3.1"
 coverage = "6.5.0"
 pytest-django = "4.5.2"
-pre-commit = "3.0.1"
-tox = "4.4.2"
+pre-commit = "3.3.1"
+tox = "4.5.1"
+tox-gh-actions = "3.1.0"
 coveralls = "3.3.1"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.2"
-pymdown-extensions = "9.9.2"
-mkdocs-material = "8.5.10"
-Pygments = "2.13.0"
+mkdocs = "1.4.3"
+pymdown-extensions = "9.11"
+mkdocs-mermaid2-plugin = "0.6.0"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "0.991"
-django-stubs = "1.14.0"
-djangorestframework-stubs = "1.8.0"
+mypy = "1.2.0"
+django-stubs = "4.2.0"
+djangorestframework-stubs = "3.14.0"
 
 [tool.poetry.extras]
 uvloop = ["uvloop"]
 pydantic = ["pydantic"]
+uritemplate = ["uritemplate"]
 
 [tool.black]
 line-length = 120
 
-[tool.isort]
-profile = "black"
-line_length = 120
-skip_gitignore = "True"
-lines_after_imports = 2
-known_third_party = [
-    "django",
-    "rest_framework",
-]
-
 [tool.ruff]
 fix = true
 line-length = 120
 exclude = [
     "tests/*",
 ]
+typing-modules = [
+    "pipeline_views.typing",
+]
 select = [
     "F",  # pyflakes
     "E",  # pycodestyle errors
     "I",  # isort
     "S",  # flake8-bandit
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
@@ -114,19 +109,19 @@
     "B905",  # `zip()` without an explicit `strict=` parameter
     "F821",  # Undefined name
     "F722",  # Syntax error in forward annotation:
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
-"pipeline_views/schema.py" = ["C901"]
-
+"pipeline_views/openapi/schema.py" = ["C901"]
+"pipeline_views/openapi/utils.py" = ["C901"]
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 warn_return_any = "True"
 warn_unused_configs = "True"
 plugins = [
     "mypy_django_plugin.main",
     "mypy_drf_plugin.main",
 ]
 
@@ -151,45 +146,55 @@
 
 [tool.pytest.ini_options]
 addopts = "-vv -s --log-cli-level=INFO"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{38, 39, 310, 311}-drf{312, 313, 314}
+envlist = py{39, 310, 311}-drf{312, 313, 314}
 isolated_build = true
 
+[gh-actions]
+python =
+    3.9: py39
+    3.10: py310
+    3.11: py311
+
 [testenv]
 allowlist_externals =
     poetry
 setenv =
     PYTHONPATH = {toxinidir}
     DJANGO_SETTINGS_MODULE = tests.django.settings
 deps =
-    py38: Django >=3.1,<3.2
     py39: Django >=3.2,<4.0
 
     py310-drf312: Django >=3.2,<4.0
     py310-drf313: Django >=4.0,<4.1
     py310-drf314: Django >=4.1,<4.2
 
     py311-drf312: Django >=3.2,<4.0
     py311-drf313: Django >=4.0,<4.1
-    py311-drf314: Django >=4.1,<4.2
+    py311-drf314: Django >=4.2,<4.3
 
     drf312: djangorestframework >=3.12.0,<3.13.0
     drf313: djangorestframework >=3.13.0,<3.14.0
     drf314: djangorestframework >=3.14.0,<3.15.0
 
-    pytest
-    coverage
-    pytest-django
+    py39: typing-extensions
+    drf-openapi-schema
+    drf-serializer-inference
     asgiref
     pydantic
     pyyaml
+    uritemplate
+
+    pytest
+    coverage
+    pytest-django
 commands =
     coverage run -m pytest -vv -s --log-cli-level=INFO
 """
 
 [build-system]
-requires = ["poetry-core>=1.1.0"]
+requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `drf_pipeline_views-0.8.5/PKG-INFO` & `drf_pipeline_views-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: drf-pipeline-views
-Version: 0.8.5
+Version: 0.9.0
 Summary: Django REST framework views using the pipeline pattern.
 Home-page: https://github.com/MrThearMan/drf-pipeline-views
 License: MIT
 Keywords: django,djangorestframework,drf,pipeline,views
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: pydantic
+Provides-Extra: uritemplate
 Provides-Extra: uvloop
-Requires-Dist: Django (>=3.0)
+Requires-Dist: Django (>=3.2)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: asgiref (>=3.5.0)
 Requires-Dist: djangorestframework (>=3.12.0)
+Requires-Dist: drf-openapi-schema (>=0.0.3)
+Requires-Dist: drf-serializer-inference (>=0.0.2)
 Requires-Dist: pydantic (>=1.6.2) ; extra == "pydantic"
-Requires-Dist: typing-extensions (>=4.4.0) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.4.0) ; python_version < "3.10"
+Requires-Dist: uritemplate (>=4.1.1) ; extra == "uritemplate"
 Requires-Dist: uvloop (>=0.16.0) ; extra == "uvloop"
 Project-URL: Bug Tracker, https://github.com/MrThearMan/drf-pipeline-views/issues
 Project-URL: Repository, https://github.com/MrThearMan/drf-pipeline-views
 Description-Content-Type: text/markdown
 
 # Django REST Framework Pipeline Views
```

