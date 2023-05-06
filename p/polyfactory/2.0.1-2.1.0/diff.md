# Comparing `tmp/polyfactory-2.0.1.tar.gz` & `tmp/polyfactory-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.0.1.tar", max compression
+gzip compressed data, was "polyfactory-2.1.0.tar", max compression
```

## Comparing `polyfactory-2.0.1.tar` & `polyfactory-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1092 2023-04-28 01:42:41.001077 polyfactory-2.0.1/LICENSE
--rw-r--r--   0        0        0     8276 2023-04-28 01:42:41.001077 polyfactory-2.0.1/README.md
--rw-r--r--   0        0        0      425 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/__init__.py
--rw-r--r--   0        0        0      642 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/constants.py
--rw-r--r--   0        0        0      591 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    30183 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1603 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2250 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     6275 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1471 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     2939 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     3311 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1838 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13431 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3845 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3633 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6030 2023-04-28 01:42:41.005077 polyfactory-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    10299 1970-01-01 00:00:00.000000 polyfactory-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-06 15:37:10.553226 polyfactory-2.1.0/LICENSE
+-rw-r--r--   0        0        0     9082 2023-05-06 15:37:10.553226 polyfactory-2.1.0/README.md
+-rw-r--r--   0        0        0      425 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    30193 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1603 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2193 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0     7389 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1471 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     2939 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2812 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1838 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13431 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0     3845 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0     3633 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-05-06 15:37:10.557226 polyfactory-2.1.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6030 2023-05-06 15:37:10.557226 polyfactory-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11105 1970-01-01 00:00:00.000000 polyfactory-2.1.0/PKG-INFO
```

### Comparing `polyfactory-2.0.1/LICENSE` & `polyfactory-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/README.md` & `polyfactory-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+
+[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
 hints and supporting dataclasses, typed-dicts, Pydantic models and more.
@@ -105,17 +107,20 @@
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
+Contributions of any kind welcome!
```

### Comparing `polyfactory-2.0.1/polyfactory/constants.py` & `polyfactory-2.1.0/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/exceptions.py` & `polyfactory-2.1.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/factories/base.py` & `polyfactory-2.1.0/polyfactory/factories/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,15 @@
         """
         result: dict[str, Any] = {**kwargs}
         generate_post: dict[str, PostGenerated] = {}
 
         for field_meta in cls.get_model_fields():
             field_build_parameters = cls.extract_field_build_parameters(field_meta=field_meta, build_args=kwargs)
             if cls.should_set_field_value(field_meta, **kwargs):
-                if hasattr(cls, field_meta.name) and field_meta.name in cls.__dict__:
+                if hasattr(cls, field_meta.name) and not hasattr(BaseFactory, field_meta.name):
                     field_value = getattr(cls, field_meta.name)
                     if isinstance(field_value, Ignore):
                         continue
 
                     if isinstance(field_value, Require) and field_meta.name not in kwargs:
                         raise MissingBuildKwargException(f"Require kwarg {field_meta.name} is missing")
```

### Comparing `polyfactory-2.0.1/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.1.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.1.0/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.1.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import decimal
 from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar, Union
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.pydantic_factory import ModelFactory
-from polyfactory.fields import Ignore
 from polyfactory.utils.predicates import is_safe_subclass
 from polyfactory.value_generators.primitives import create_random_bytes
 
 try:
     from bson.decimal128 import Decimal128, create_decimal128_context
     from odmantic import EmbeddedModel, Model, bson as odbson
 
@@ -32,16 +31,14 @@
         """Determine whether the given value is supported by the factory.
 
         :param value: An arbitrary value.
         :returns: A typeguard
         """
         return is_safe_subclass(value, Model) or is_safe_subclass(value, EmbeddedModel)
 
-    id = Ignore()
-
     @classmethod
     def get_provider_map(cls) -> dict[Any, Callable[[], Any]]:
         provider_map = super().get_provider_map()
         provider_map.update(
             {
                 odbson.Int64: lambda: odbson.Int64.validate(cls.__faker__.pyint()),
                 odbson.Decimal128: lambda: _to_decimal128(cls.__faker__.pydecimal()),
```

### Comparing `polyfactory-2.0.1/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.1.0/polyfactory/factories/pydantic_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
+
 from contextlib import suppress
 from inspect import isclass
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
     Mapping,
     TypeVar,
     cast,
 )
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
-from polyfactory.field_meta import FieldMeta, Null, Constraints
+from polyfactory.field_meta import Constraints, FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_new_type
 
 try:
     from pydantic import (
         BaseModel,
     )
     from pydantic.fields import DeferredType, ModelField, Undefined
@@ -90,22 +91,26 @@
                 "multiple_of": getattr(annotation, "multiple_of", None),
                 "upper_case": getattr(annotation, "to_upper", None),
                 "lower_case": getattr(annotation, "to_lower", None),
                 "item_type": getattr(annotation, "item_type", None),
             },
         )
 
+        children: list[FieldMeta] = []
+        if model_field.key_field:
+            children.append(PydanticFieldMeta.from_model_field(model_field.key_field, use_alias))
+        if model_field.sub_fields:
+            children.extend(
+                PydanticFieldMeta.from_model_field(sub_field, use_alias) for sub_field in model_field.sub_fields
+            )
+
         return PydanticFieldMeta(
             name=name,
             annotation=annotation,
-            children=[
-                PydanticFieldMeta.from_model_field(child, use_alias=use_alias) for child in model_field.sub_fields
-            ]
-            if model_field.sub_fields
-            else None,
+            children=children,
             default=default_value,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
         )
 
 
 class ModelFactory(Generic[T], BaseFactory[T]):
     """Base factory for pydantic models"""
@@ -133,15 +138,15 @@
     def get_model_fields(cls) -> list["FieldMeta"]:
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
 
         """
-        if not hasattr(cls, "_fields_metadata"):
+        if "_fields_metadata" not in cls.__dict__:
             cls._fields_metadata = [
                 PydanticFieldMeta.from_model_field(
                     field,
                     use_alias=not cls.__model__.__config__.allow_population_by_field_name,
                 )
                 for field in cls.__model__.__fields__.values()
             ]
@@ -160,7 +165,33 @@
         """
         processed_kwargs = cls.process_kwargs(**kwargs)
 
         if factory_use_construct:
             return cls.__model__.construct(**processed_kwargs)
 
         return cls.__model__(**processed_kwargs)
+
+    @classmethod
+    def is_custom_root_field(cls, field_meta: FieldMeta) -> bool:
+        """Determine whether the field is a custom root field.
+
+        :param field_meta: FieldMeta instance.
+
+        :returns: A boolean determining whether the field is a custom root.
+
+        """
+        return field_meta.name == "__root__"
+
+    @classmethod
+    def should_set_field_value(cls, field_meta: FieldMeta, **kwargs: Any) -> bool:
+        """Determine whether to set a value for a given field_name.
+        This is an override of BaseFactory.should_set_field_value.
+
+        :param field_meta: FieldMeta instance.
+        :param kwargs: Any kwargs passed to the factory.
+
+        :returns: A boolean determining whether a value should be set for the given field_meta.
+
+        """
+        return field_meta.name not in kwargs and (
+            not field_meta.name.startswith("_") or cls.is_custom_root_field(field_meta)
+        )
```

### Comparing `polyfactory-2.0.1/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.1.0/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/field_meta.py` & `polyfactory-2.1.0/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/fields.py` & `polyfactory-2.1.0/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/persistence.py` & `polyfactory-2.1.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/pytest_plugin.py` & `polyfactory-2.1.0/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/utils/helpers.py` & `polyfactory-2.1.0/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/utils/predicates.py` & `polyfactory-2.1.0/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/value_generators/complex_types.py` & `polyfactory-2.1.0/polyfactory/value_generators/complex_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,72 @@
 from __future__ import annotations
-from collections import deque
-from typing import TYPE_CHECKING, Any, MutableMapping, Tuple
+
+from typing import TYPE_CHECKING, AbstractSet, Any, Collection, MutableMapping, MutableSequence, Set, TypeVar
 
 from typing_extensions import is_typeddict
 
-from polyfactory.constants import TYPE_MAPPING
-from polyfactory.field_meta import FieldMeta
-from polyfactory.utils.helpers import unwrap_annotation, unwrap_args
+from polyfactory.utils.helpers import unwrap_annotation
 from polyfactory.utils.predicates import get_type_origin, is_any, is_union
 from polyfactory.value_generators.primitives import create_random_string
 
 if TYPE_CHECKING:
     from polyfactory.factories.base import BaseFactory
+    from polyfactory.field_meta import FieldMeta
 
 
-def handle_container_type(
-    container_type: type,
-    factory: type[BaseFactory],
-    field_meta: FieldMeta,
-) -> Any:
+def handle_collection_type(field_meta: FieldMeta, container_type: type, factory: type[BaseFactory]) -> Any:
     """Handle generation of container types recursively.
 
     :param container_type: A type that can accept type arguments.
     :param factory: A factory.
     :param field_meta: A field meta instance.
 
     :returns: A built result.
     """
-    if mapped_container_type := TYPE_MAPPING.get(container_type):
-        container_type = mapped_container_type
+    container = container_type()
+    if not field_meta.children:
+        return container
 
-    container = container_type() if container_type is not frozenset else set()
+    if issubclass(container_type, MutableMapping) or is_typeddict(container_type):
+        key = handle_complex_type(field_meta.children[0], factory)
+        value = handle_complex_type(field_meta.children[1], factory)
+        container[key] = value
 
-    if isinstance(container, MutableMapping) or is_typeddict(container):
-        key_type, value_type = unwrap_args(field_meta.annotation) or (str, str)
-        key = handle_complex_type(field_meta=FieldMeta.from_type(annotation=key_type), factory=factory)
-        value = handle_complex_type(field_meta=FieldMeta.from_type(annotation=value_type), factory=factory)
-        container[key] = value  # pyright: ignore
-    elif field_meta.children:
-        if isinstance(container, (list, deque)):
-            container.append(
-                handle_complex_type(
-                    field_meta=factory.__random__.choice(field_meta.children),
-                    factory=factory,
-                )
-            )
-        else:
-            container.add(
-                handle_complex_type(
-                    field_meta=factory.__random__.choice(field_meta.children),
-                    factory=factory,
-                )
-            )
-
-    return container if container_type is not frozenset else container_type(*container)
-
-
-def handle_complex_type(
-    factory: type[BaseFactory],
-    field_meta: FieldMeta,
-) -> Any:
-    """Recursive type generation based on typing info stored in the graph like structure of pydantic field_metas.
+    elif issubclass(container_type, MutableSequence):
+        container.append(handle_complex_type(field_meta.children[0], factory))
+
+    elif issubclass(container_type, Set):
+        container.add(handle_complex_type(field_meta.children[0], factory))
+
+    elif issubclass(container_type, AbstractSet):
+        container = container.union(handle_collection_type(field_meta, set, factory))
+
+    elif issubclass(container_type, tuple):
+        container = container_type(handle_complex_type(subfield_meta, factory) for subfield_meta in field_meta.children)
+
+    else:
+        raise NotImplementedError(f"Unsupported container type: {container_type}")
+
+    return container
+
+
+def handle_complex_type(field_meta: FieldMeta, factory: type[BaseFactory]) -> Any:
+    """Recursive type generation based on typing info stored in the graph like structure
+    of pydantic field_metas.
 
-    :param factory: A factory.
     :param field_meta: A field meta instance.
+    :param factory: A factory.
 
     :returns: A built result.
     """
-
-    if origin := get_type_origin(annotation=unwrap_annotation(field_meta.annotation)):
-        if origin not in (tuple, Tuple):
-            return handle_container_type(field_meta=field_meta, container_type=origin, factory=factory)
-
-        return tuple(
-            handle_complex_type(field_meta=sub_field, factory=factory) for sub_field in (field_meta.children or [])
-        )
+    if origin := get_type_origin(unwrap_annotation(field_meta.annotation)):
+        if issubclass(origin, Collection):
+            return handle_collection_type(field_meta, origin, factory)
+        return factory.get_mock_value(origin)
 
     if is_union(field_meta.annotation) and field_meta.children:
-        return handle_complex_type(field_meta=factory.__random__.choice(field_meta.children), factory=factory)
-
-    if is_any(field_meta.annotation):
-        return create_random_string(random=factory.__random__, min_length=1, max_length=10)
+        return handle_complex_type(factory.__random__.choice(field_meta.children), factory)
 
-    if factory.should_set_none_value(field_meta):
-        return None
+    if is_any(field_meta.annotation) or isinstance(field_meta.annotation, TypeVar):
+        return create_random_string(factory.__random__, min_length=1, max_length=10)
 
-    return factory.get_field_value(field_meta=field_meta, field_build_parameters=None)
+    return factory.get_field_value(field_meta)
```

### Comparing `polyfactory-2.0.1/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.1.0/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.1.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.1.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.1.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/value_generators/primitives.py` & `polyfactory-2.1.0/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/polyfactory/value_generators/regex.py` & `polyfactory-2.1.0/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.1/pyproject.toml` & `polyfactory-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.0.1"
+version = "2.1.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
```

### Comparing `polyfactory-2.0.1/PKG-INFO` & `polyfactory-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.0.1
+Version: 2.1.0
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: dataclasses,factory,faker,mock,pydantic,pytest,litestar,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -68,15 +68,17 @@
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+
+[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
+
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
 hints and supporting dataclasses, typed-dicts, Pydantic models and more.
@@ -152,18 +154,21 @@
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sygutss"><img src="https://avatars.githubusercontent.com/u/48909366?v=4?s=100" width="100px;" alt="sygutss"/><br /><sub><b>sygutss</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/issues?q=author%3Asygutss" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=sygutss" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/chrisbeardy"><img src="https://avatars.githubusercontent.com/u/20585410?v=4?s=100" width="100px;" alt="chrisbeardy"/><br /><sub><b>chrisbeardy</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=chrisbeardy" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
-This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
+Contributions of any kind welcome!
```

