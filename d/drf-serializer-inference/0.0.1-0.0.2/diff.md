# Comparing `tmp/drf_serializer_inference-0.0.1.tar.gz` & `tmp/drf_serializer_inference-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_serializer_inference-0.0.1.tar", max compression
+gzip compressed data, was "drf_serializer_inference-0.0.2.tar", max compression
```

## Comparing `drf_serializer_inference-0.0.1.tar` & `drf_serializer_inference-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-05-01 07:16:25.114261 drf_serializer_inference-0.0.1/LICENSE
--rw-r--r--   0        0        0     3897 2023-05-01 08:04:39.161028 drf_serializer_inference-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2194 2023-05-01 07:42:10.596204 drf_serializer_inference-0.0.1/README.md
--rw-r--r--   0        0        0      348 2023-05-01 07:36:18.080770 drf_serializer_inference-0.0.1/serializer_inference/__init__.py
--rw-r--r--   0        0        0     9228 2023-05-01 07:34:59.641488 drf_serializer_inference-0.0.1/serializer_inference/inference.py
--rw-r--r--   0        0        0        0 2023-05-01 07:16:25.178155 drf_serializer_inference-0.0.1/serializer_inference/py.typed
--rw-r--r--   0        0        0      921 2023-05-01 07:33:36.310300 drf_serializer_inference-0.0.1/serializer_inference/serializers.py
--rw-r--r--   0        0        0      775 2023-05-01 07:59:30.971706 drf_serializer_inference-0.0.1/serializer_inference/typing.py
--rw-r--r--   0        0        0      369 2023-05-01 07:35:14.649991 drf_serializer_inference-0.0.1/serializer_inference/utils.py
--rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 drf_serializer_inference-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 12:21:46.726678 drf_serializer_inference-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2152 2023-05-06 12:21:46.726678 drf_serializer_inference-0.0.2/README.md
+-rw-r--r--   0        0        0     3515 2023-05-06 12:21:46.730678 drf_serializer_inference-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      337 2023-05-06 12:21:46.730678 drf_serializer_inference-0.0.2/serializer_inference/__init__.py
+-rw-r--r--   0        0        0     9426 2023-05-06 12:21:46.730678 drf_serializer_inference-0.0.2/serializer_inference/inference.py
+-rw-r--r--   0        0        0        0 2023-05-06 12:21:46.730678 drf_serializer_inference-0.0.2/serializer_inference/py.typed
+-rw-r--r--   0        0        0      456 2023-05-06 12:21:46.730678 drf_serializer_inference-0.0.2/serializer_inference/serializers.py
+-rw-r--r--   0        0        0      668 2023-05-06 12:21:46.730678 drf_serializer_inference-0.0.2/serializer_inference/typing.py
+-rw-r--r--   0        0        0      356 2023-05-06 12:21:46.730678 drf_serializer_inference-0.0.2/serializer_inference/utils.py
+-rw-r--r--   0        0        0     3683 1970-01-01 00:00:00.000000 drf_serializer_inference-0.0.2/PKG-INFO
```

### Comparing `drf_serializer_inference-0.0.1/pyproject.toml` & `drf_serializer_inference-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,174 +1,166 @@
-[tool.poetry]
-name = "drf-serializer-inference"
-version = "0.0.1"
-description = "Infer Django Rest Framework serializers from callables like functions and classes."
-authors = [
-    "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
-]
-packages = [
-    { include = "serializer_inference" },
-]
-license = "MIT"
-readme = "README.md"
-homepage = "https://mrthearman.github.io/drf-serializer-inference"
-repository = "https://github.com/MrThearMan/drf-serializer-inference"
-keywords = [
-    "drf",
-    "django",
-    "rest_framework",
-    "rest",
-    "framework",
-    "inference",
-    "serializer",
-]
-classifiers = [
-    "Environment :: Web Environment",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-    "Natural Language :: English",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
-include = [
-    "README.md",
-    "LICENSE",
-]
-exclude = [
-    "tests",
-]
-
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/MrThearMan/drf-serializer-inference/issues"
-
-[tool.poetry.dependencies]
-python = ">=3.9,<4"
-Django = ">=3.2"
-djangorestframework = ">=3.12.0"
-typing-extensions = {version = ">=4.4.0", python = "<3.10"}
-pydantic = {version = ">=1.6.2", optional = true}
-
-[tool.poetry.group.test.dependencies]
-pytest = "7.3.0"
-coverage = "6.5.0"
-pre-commit = "3.2.2"
-tox = "4.4.12"
-tox-gh-actions = "3.1.0"
-coveralls = "3.3.1"
-
-[tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.2"
-pymdown-extensions = "9.11"
-mkdocs-mermaid2-plugin = "0.6.0"
-
-[tool.poetry.group.lint.dependencies]
-mypy = "1.2.0"
-django-stubs = "1.16.0"
-djangorestframework-stubs = "1.10.0"
-
-[tool.poetry.extras]
-pydantic = ["pydantic"]
-
-[tool.black]
-line-length = 120
-
-[tool.ruff]
-fix = true
-line-length = 120
-extend-exclude = [
-    "tests/*",
-]
-typing-modules = [
-    "serializer_inference.typing",
-]
-select = [
-    "F",  # pyflakes
-    "E",  # pycodestyle errors
-    "I",  # isort
-    "S",  # flake8-bandit
-    "C",  # flake8-comprehensions
-    "B",  # flake8-bugbear
-    "T",  # flake8-print
-    "W",  # pycodestyle warnings
-]
-ignore = [
-]
-
-[tool.mypy]
-python_version = "3.11"
-warn_return_any = "True"
-warn_unused_configs = "True"
-plugins = [
-    "mypy_django_plugin.main",
-    "mypy_drf_plugin.main",
-]
-
-[tool.coverage.run]
-relative_files = true
-
-[tool.coverage.report]
-omit = [
-    "tests/*",
-    "docs/*",
-    ".venv/*",
-    ".tox/*",
-]
-exclude_lines = [
-    "if TYPE_CHECKING:",
-    "except ImportError:",
-    "pragma: no cover",
-]
-
-[tool.pytest.ini_options]
-addopts = "-vv -s --log-cli-level=INFO"
-
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-envlist = py{39, 310, 311}-drf{312, 313, 314}
-isolated_build = true
-
-[gh-actions]
-python =
-    3.8: py38
-    3.9: py39
-    3.10: py310
-    3.11: py311
-
-[testenv]
-allowlist_externals =
-    poetry
-setenv =
-    PYTHONPATH = {toxinidir}
-    DJANGO_SETTINGS_MODULE = tests.django.settings
-deps =
-    py39: Django >=3.2,<4.0
-
-    py310-drf312: Django >=3.2,<4.0
-    py310-drf313: Django >=4.0,<4.1
-    py310-drf314: Django >=4.1,<4.2
-
-    py311-drf312: Django >=3.2,<4.0
-    py311-drf313: Django >=4.0,<4.1
-    py311-drf314: Django >=4.2,<4.3
-
-    drf312: djangorestframework >=3.12.0,<3.13.0
-    drf313: djangorestframework >=3.13.0,<3.14.0
-    drf314: djangorestframework >=3.14.0,<3.15.0
-
-    pytest
-    coverage
-    pytest-django
-    pydantic
-    typing-extensions
-commands =
-    coverage run -m pytest -vv -s --log-cli-level=INFO
-"""
-
-[build-system]
-requires = ["poetry-core>=1.5.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "drf-serializer-inference"
+version = "0.0.2"
+description = "Infer Django Rest Framework serializers from callables like functions and classes."
+authors = [
+    "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
+]
+packages = [
+    { include = "serializer_inference" },
+]
+license = "MIT"
+readme = "README.md"
+homepage = "https://mrthearman.github.io/drf-serializer-inference"
+repository = "https://github.com/MrThearMan/drf-serializer-inference"
+keywords = [
+    "drf",
+    "django",
+    "rest_framework",
+    "rest",
+    "framework",
+    "inference",
+    "serializer",
+]
+classifiers = [
+    "Environment :: Web Environment",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Developers",
+    "Natural Language :: English",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+include = [
+    "README.md",
+    "LICENSE",
+]
+exclude = [
+    "tests",
+]
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/MrThearMan/drf-serializer-inference/issues"
+
+[tool.poetry.dependencies]
+python = ">=3.9,<4"
+djangorestframework = ">=3.12.0"
+typing-extensions = {version = ">=4.4.0", python = "<3.10"}
+pydantic = {version = ">=1.6.2", optional = true}
+
+[tool.poetry.group.test.dependencies]
+pytest = "7.3.1"
+coverage = "6.5.0"
+pre-commit = "3.3.1"
+tox = "4.5.1"
+tox-gh-actions = "3.1.0"
+coveralls = "3.3.1"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "1.4.3"
+pymdown-extensions = "9.11"
+mkdocs-mermaid2-plugin = "0.6.0"
+
+[tool.poetry.group.lint.dependencies]
+mypy = "1.2.0"
+djangorestframework-stubs = "3.14.0"
+
+[tool.poetry.extras]
+pydantic = ["pydantic"]
+
+[tool.black]
+line-length = 120
+
+[tool.ruff]
+fix = true
+line-length = 120
+extend-exclude = [
+    "tests/*",
+]
+typing-modules = [
+    "serializer_inference.typing",
+]
+select = [
+    "F",  # pyflakes
+    "E",  # pycodestyle errors
+    "I",  # isort
+    "S",  # flake8-bandit
+    "C",  # flake8-comprehensions
+    "B",  # flake8-bugbear
+    "T",  # flake8-print
+    "W",  # pycodestyle warnings
+]
+ignore = [
+]
+
+[tool.mypy]
+python_version = "3.11"
+warn_return_any = "True"
+warn_unused_configs = "True"
+plugins = [
+    "mypy_django_plugin.main",
+    "mypy_drf_plugin.main",
+]
+
+[tool.coverage.run]
+relative_files = true
+
+[tool.coverage.report]
+omit = [
+    "tests/*",
+    "docs/*",
+    ".venv/*",
+    ".tox/*",
+]
+exclude_lines = [
+    "if TYPE_CHECKING:",
+    "except ImportError:",
+    "pragma: no cover",
+]
+
+[tool.pytest.ini_options]
+addopts = "-vv -s --log-cli-level=INFO"
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+envlist = py{39, 310, 311}-drf{312, 313, 314}
+isolated_build = true
+
+[gh-actions]
+python =
+    3.9: py39
+    3.10: py310
+    3.11: py311
+
+[testenv]
+allowlist_externals =
+    poetry
+deps =
+    py39: Django >=3.2,<4.0
+
+    py310-drf312: Django >=3.2,<4.0
+    py310-drf313: Django >=4.0,<4.1
+    py310-drf314: Django >=4.1,<4.2
+
+    py311-drf312: Django >=3.2,<4.0
+    py311-drf313: Django >=4.0,<4.1
+    py311-drf314: Django >=4.2,<4.3
+
+    drf312: djangorestframework >=3.12.0,<3.13.0
+    drf313: djangorestframework >=3.13.0,<3.14.0
+    drf314: djangorestframework >=3.14.0,<3.15.0
+
+    pytest
+    coverage
+    pydantic
+    typing-extensions
+commands =
+    coverage run -m pytest -vv -s --log-cli-level=INFO
+"""
+
+[build-system]
+requires = ["poetry-core>=1.5.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `drf_serializer_inference-0.0.1/README.md` & `drf_serializer_inference-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Serializer Inference
-
-[![Coverage Status][coverage-badge]][coverage]
-[![GitHub Workflow Status][status-badge]][status]
-[![PyPI][pypi-badge]][pypi]
-[![GitHub][licence-badge]][licence]
-[![GitHub Last Commit][repo-badge]][repo]
-[![GitHub Issues][issues-badge]][issues]
-[![Downloads][downloads-badge]][pypi]
-[![Python Version][version-badge]][pypi]
-
-```shell
-pip install drf-serializer-inference
-```
-
----
-
-**Documentation**: [https://mrthearman.github.io/drf-serializer-inference/](https://mrthearman.github.io/drf-serializer-inference/)
-
-**Source Code**: [https://github.com/MrThearMan/drf-serializer-inference/](https://github.com/MrThearMan/drf-serializer-inference/)
-
-**Contributing**: [https://github.com/MrThearMan/drf-serializer-inference/blob/main/CONTRIBUTING.md](https://github.com/MrThearMan/drf-serializer-inference/blob/main/CONTRIBUTING.md)
-
----
-
-Infer Django Rest Framework serializers from callables like functions and classes.
-
-[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/drf-serializer-inference/badge.svg?branch=main
-[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/drf-serializer-inference/test.yml?branch=main
-[pypi-badge]: https://img.shields.io/pypi/v/drf-serializer-inference
-[licence-badge]: https://img.shields.io/github/license/MrThearMan/drf-serializer-inference
-[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/drf-serializer-inference
-[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/drf-serializer-inference
-[version-badge]: https://img.shields.io/pypi/pyversions/drf-serializer-inference
-[downloads-badge]: https://img.shields.io/pypi/dm/drf-serializer-inference
-
-[coverage]: https://coveralls.io/github/MrThearMan/drf-serializer-inference?branch=main
-[status]: https://github.com/MrThearMan/drf-serializer-inference/actions/workflows/test.yml
-[pypi]: https://pypi.org/project/drf-serializer-inference
-[licence]: https://github.com/MrThearMan/drf-serializer-inference/blob/main/LICENSE
-[repo]: https://github.com/MrThearMan/drf-serializer-inference/commits/main
-[issues]: https://github.com/MrThearMan/drf-serializer-inference/issues
+# Serializer Inference
+
+[![Coverage Status][coverage-badge]][coverage]
+[![GitHub Workflow Status][status-badge]][status]
+[![PyPI][pypi-badge]][pypi]
+[![GitHub][licence-badge]][licence]
+[![GitHub Last Commit][repo-badge]][repo]
+[![GitHub Issues][issues-badge]][issues]
+[![Downloads][downloads-badge]][pypi]
+[![Python Version][version-badge]][pypi]
+
+```shell
+pip install drf-serializer-inference
+```
+
+---
+
+**Documentation**: [https://mrthearman.github.io/drf-serializer-inference/](https://mrthearman.github.io/drf-serializer-inference/)
+
+**Source Code**: [https://github.com/MrThearMan/drf-serializer-inference/](https://github.com/MrThearMan/drf-serializer-inference/)
+
+**Contributing**: [https://github.com/MrThearMan/drf-serializer-inference/blob/main/CONTRIBUTING.md](https://github.com/MrThearMan/drf-serializer-inference/blob/main/CONTRIBUTING.md)
+
+---
+
+Infer Django Rest Framework serializers from callables like functions and classes.
+
+[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/drf-serializer-inference/badge.svg?branch=main
+[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/drf-serializer-inference/test.yml?branch=main
+[pypi-badge]: https://img.shields.io/pypi/v/drf-serializer-inference
+[licence-badge]: https://img.shields.io/github/license/MrThearMan/drf-serializer-inference
+[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/drf-serializer-inference
+[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/drf-serializer-inference
+[version-badge]: https://img.shields.io/pypi/pyversions/drf-serializer-inference
+[downloads-badge]: https://img.shields.io/pypi/dm/drf-serializer-inference
+
+[coverage]: https://coveralls.io/github/MrThearMan/drf-serializer-inference?branch=main
+[status]: https://github.com/MrThearMan/drf-serializer-inference/actions/workflows/test.yml
+[pypi]: https://pypi.org/project/drf-serializer-inference
+[licence]: https://github.com/MrThearMan/drf-serializer-inference/blob/main/LICENSE
+[repo]: https://github.com/MrThearMan/drf-serializer-inference/commits/main
+[issues]: https://github.com/MrThearMan/drf-serializer-inference/issues
```

### Comparing `drf_serializer_inference-0.0.1/serializer_inference/inference.py` & `drf_serializer_inference-0.0.2/serializer_inference/inference.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,293 +1,304 @@
-from datetime import date, datetime, time, timedelta
-from decimal import Decimal
-from inspect import getfullargspec
-
-from rest_framework.fields import (
-    BooleanField,
-    CharField,
-    ChoiceField,
-    DateField,
-    DateTimeField,
-    DecimalField,
-    DictField,
-    DurationField,
-    Field,
-    FloatField,
-    IntegerField,
-    JSONField,
-    ListField,
-    TimeField,
-)
-from rest_framework.serializers import BaseSerializer, ListSerializer, Serializer
-
-from .typing import (
-    Any,
-    Callable,
-    Dict,
-    ForwardRef,
-    List,
-    Literal,
-    Optional,
-    Tuple,
-    Type,
-    TypesDict,
-    Union,
-    eval_type,
-    get_args,
-    get_origin,
-)
-from .utils import snake_case_to_pascal_case
-
-__all__ = [
-    "inline_serializer",
-    "serializer_from_callable",
-]
-
-
-def serializer_from_callable(func: Callable[..., Any], output: bool = False) -> Type[Serializer]:
-    """Create a serializer from the parameter type hints of a callable.
-    Attempt to infer the types from the default arguments if no typing information is available.
-    If output is true, infer from callable return type.
-    In this case, return type should be a TypedDict so that field conversion works.
-    """
-    types = _return_types(func) if output else _parameter_types(func)
-    is_list = isinstance(types, list)
-    fields = _get_fields(types[0]) if is_list else _get_fields(types)
-    serializer_name = snake_case_to_pascal_case(f"{func.__name__}_serializer")
-    return inline_serializer(serializer_name, fields=fields, many=is_list)
-
-
-def inline_serializer(
-    name: str,
-    super_class: Type[BaseSerializer] = Serializer,
-    fields: Dict[str, Field] = None,
-    many: bool = False,
-) -> Type[BaseSerializer]:
-    serializer: Type[BaseSerializer] = type(name, (super_class,), fields or {})  # type: ignore
-    serializer.many = many
-    return serializer
-
-
-def _parameter_types(func: Callable[..., Any]) -> TypesDict:
-    """Get the types for a callable's parameters."""
-    func = _unwrap_function(func)
-    args_spec = getfullargspec(func)
-    types = args_spec.annotations
-    types.pop("return", None)
-
-    # Get types based on argument default values
-    defaults: Tuple[Any, ...] = args_spec.defaults or ()
-    for name, value in zip(reversed(args_spec.args), reversed(defaults)):  # noqa
-        if name in types:
-            continue
-        types[name] = type(value)
-
-    # Get types based on keyword-only argument default values
-    defaults_kwonly: Dict[str, Any] = args_spec.kwonlydefaults or {}
-    for name, value in defaults_kwonly.items():
-        if name in types:
-            continue
-        types[name] = type(value)
-
-    # Add None for all positional arguments and keyword-only arguments
-    # for which a type was not found or could not be inferred
-    for name in args_spec.args + args_spec.kwonlyargs:
-        if name in types:
-            continue
-        types[name] = None
-
-    # Remove * and ** parameters from the typing dict
-    types.pop(args_spec.varargs or "", None)
-    types.pop(args_spec.varkw or "", None)
-
-    globalns = _get_globals(func)
-    for name, type_ in types.items():
-        types[name] = _unwrap_types(type_, globalns)
-
-    return types
-
-
-def _return_types(func: Callable[..., Any]) -> Union[TypesDict, List[TypesDict]]:
-    """Get the callables return types"""
-    func = _unwrap_function(func)
-    args_spec = getfullargspec(func)
-    return_type = args_spec.annotations.get("return")
-    return _unwrap_types(return_type, _get_globals(func))
-
-
-_type_to_serializer_field: Dict[Optional[Type], Type[Field]] = {
-    str: CharField,
-    int: IntegerField,
-    float: FloatField,
-    bool: BooleanField,
-    dict: DictField,
-    list: ListField,
-    date: DateField,
-    datetime: DateTimeField,
-    time: TimeField,
-    timedelta: DurationField,
-    Decimal: DecimalField,
-    None: CharField,
-    type: CharField,
-}
-
-
-def _get_fields(types: TypesDict) -> Dict[str, Field]:
-    """Convert types to serializer fields.
-    TypedDicts and other classes with __annotations__ dicts
-    are recursively converted to serializers based on their types.
-    """
-
-    fields: Dict[str, Field] = {}
-    for name, type_ in types.items():
-        # Could not determine forward referenced TypedDict
-        # from another file. This is the best guess.
-        if isinstance(type_, ForwardRef):
-            fields[name] = JSONField()
-            continue
-
-        if isinstance(type_, dict):
-            fields[name] = inline_serializer(name, fields=_get_fields(type_))()
-            continue
-
-        if isinstance(type_, list):
-            if isinstance(type_[0], dict):
-                fields[name] = inline_serializer(name, fields=_get_fields(type_[0]))(many=True)
-            else:
-                fields[name] = ListField(child=_type_to_serializer_field.get(type_[0], CharField)())
-
-            continue
-
-        if get_origin(type_) == Literal:
-            choices = [arg.__forward_arg__ for arg in get_args(type_)]
-            fields[name] = ChoiceField(choices=choices)
-            continue
-
-        field = _type_to_serializer_field.get(type_, CharField)
-        if issubclass(field, DecimalField):
-            fields[name] = field(max_digits=13, decimal_places=3)
-            continue
-
-        fields[name] = field()
-
-    return fields
-
-
-def _unwrap_types(
-    types: Union[Type, TypesDict, List[TypesDict]],
-    globalns: Dict[str, Any],
-) -> Union[Type, TypesDict, List[TypesDict]]:
-    """Recurively unwrap types from the given item."""
-    typ = _forward_refs_to_types(types, globalns)
-
-    if hasattr(typ, "__origin__"):
-        return _unwrap_generic(typ, globalns)
-
-    if not hasattr(typ, "__annotations__"):
-        return typ
-
-    annotations: TypesDict = typ.__annotations__
-    for name, annotation in annotations.items():
-        annotations[name] = _unwrap_types(annotation, globalns)
-
-    return annotations
-
-
-def _forward_refs_to_types(
-    types: Union[Type, TypesDict, List[TypesDict]],
-    globalns: Dict[str, Any],
-) -> Union[Type, TypesDict, List[TypesDict]]:
-    """Convert strings and forward references to types."""
-    if isinstance(types, str):
-        types = ForwardRef(types)
-
-    if isinstance(types, ForwardRef):
-        try:
-            types = eval_type(types, globalns, globalns)
-        except NameError:
-            pass
-
-    if hasattr(types, "__args__"):
-        args = []
-        for arg in types.__args__:
-            args.append(_forward_refs_to_types(arg, globalns))
-        types.__args__ = tuple(args)
-
-    return types
-
-
-def _unwrap_generic(type_: Type, globalns: Dict[str, Any]) -> Union[List[TypesDict], Dict[str, List[TypesDict]], Type]:
-    """Ungrap the arguments of generics like list and dicts into proper types."""
-    origin_type: Type = get_origin(type_)
-    origin_args: Tuple[Type, ...] = get_args(type_)
-    special_type = origin_type in (Union,)
-
-    try:
-        if not issubclass(origin_type, (tuple, list, set, dict)):  # pragma: no cover
-            return type_
-    except TypeError:
-        if not special_type:
-            return type_
-
-    if not special_type and issubclass(origin_type, dict):
-        origin_args = origin_args[1:]
-
-    arg_types = get_arg_types(origin_args, globalns)
-
-    if origin_type == Union:
-        return arg_types[0]
-
-    if issubclass(origin_type, dict):
-        return {"str": arg_types[0]}
-
-    return arg_types
-
-
-def get_arg_types(
-    origin_args: Tuple[Type, ...],
-    globalns: Dict[str, Any],
-) -> Union[List[TypesDict], Dict[str, List[TypesDict]], Type]:
-    arg_types = []
-
-    for arg_type in origin_args:
-        arg_type = _forward_refs_to_types(arg_type, globalns)
-
-        if not hasattr(arg_type, "__annotations__"):
-            if hasattr(arg_type, "__origin__"):
-                arg_type = _unwrap_generic(arg_type, globalns)
-
-            arg_types.append(arg_type)
-            continue
-
-        anns = {}
-        for name, annotation in arg_type.__annotations__.items():
-            anns[name] = _unwrap_types(annotation, globalns)
-
-        arg_types.append(anns)
-
-    return arg_types
-
-
-def _unwrap_function(func: Callable[..., Any]) -> Callable[..., Any]:
-    """Unwrap decorated functions to allow fetching types from them."""
-    while hasattr(func, "__wrapped__"):
-        func = func.__wrapped__
-    return func
-
-
-def _get_globals(func: Callable[..., Any]) -> Dict[str, Any]:
-    return getattr(_unwrap_function(func), "__globals__", {})
-
-
-def _to_comparable_dict(serializer: Serializer) -> Dict[str, Any]:
-    dct = {}
-    is_list = isinstance(serializer, ListSerializer)
-    fields = serializer.child.fields if is_list else serializer.fields
-    for name, field in fields.items():
-        if isinstance(field, ListSerializer):
-            dct[name] = [_to_comparable_dict(field.child)]
-        elif isinstance(field, Serializer):
-            dct[name] = _to_comparable_dict(field)
-        else:
-            dct[name] = str(field)
-    return [dct] if is_list else dct
+from datetime import date, datetime, time, timedelta
+from decimal import Decimal
+from inspect import getfullargspec
+from typing import Dict, List, Set, Tuple, Type
+
+from rest_framework.fields import (
+    BooleanField,
+    CharField,
+    ChoiceField,
+    DateField,
+    DateTimeField,
+    DecimalField,
+    DictField,
+    DurationField,
+    Field,
+    FloatField,
+    IntegerField,
+    JSONField,
+    ListField,
+    TimeField,
+)
+from rest_framework.serializers import ListSerializer, Serializer
+
+from .typing import (
+    Any,
+    Callable,
+    ForwardRef,
+    Literal,
+    Optional,
+    TypesDict,
+    TypeVar,
+    Union,
+    eval_type,
+    get_args,
+    get_origin,
+)
+from .utils import snake_case_to_pascal_case
+
+__all__ = [
+    "inline_serializer",
+    "serializer_from_callable",
+]
+
+
+TSerializer = TypeVar("T", bound=Serializer)
+
+
+def serializer_from_callable(func: Callable[..., Any], output: bool = False) -> type[Serializer]:
+    """Create a serializer from the parameter type hints of a callable.
+    Attempt to infer the types from the default arguments if no typing information is available.
+    If output is true, infer from callable return type.
+    In this case, return type should be a TypedDict so that field conversion works.
+    """
+    types = _return_types(func) if output else _parameter_types(func)
+    is_list = isinstance(types, list)
+    fields = _get_fields(types[0]) if is_list else _get_fields(types)
+    serializer_name = snake_case_to_pascal_case(f"{func.__name__}_serializer")
+    return inline_serializer(serializer_name, fields=fields, many=is_list)
+
+
+def inline_serializer(
+    name: str,
+    super_class: type[TSerializer] = Serializer,
+    fields: dict[str, Field] = None,
+    many: bool = False,
+) -> type[TSerializer]:
+    serializer: type[TSerializer] = type(name, (super_class,), fields or {})  # type: ignore
+    serializer.many = many
+    return serializer
+
+
+def _parameter_types(func: Callable[..., Any]) -> TypesDict:
+    """Get the types for a callable's parameters."""
+    func = _unwrap_function(func)
+    args_spec = getfullargspec(func)
+    types = args_spec.annotations
+    types.pop("return", None)
+
+    # Get types based on argument default values
+    defaults: tuple[Any, ...] = args_spec.defaults or ()
+    for name, value in zip(reversed(args_spec.args), reversed(defaults)):  # noqa
+        if name in types:
+            continue
+        types[name] = type(value)
+
+    # Get types based on keyword-only argument default values
+    defaults_kwonly: dict[str, Any] = args_spec.kwonlydefaults or {}
+    for name, value in defaults_kwonly.items():
+        if name in types:
+            continue
+        types[name] = type(value)
+
+    # Add None for all positional arguments and keyword-only arguments
+    # for which a type was not found or could not be inferred
+    for name in args_spec.args + args_spec.kwonlyargs:
+        if name in types:
+            continue
+        types[name] = None
+
+    # Remove * and ** parameters from the typing dict
+    types.pop(args_spec.varargs or "", None)
+    types.pop(args_spec.varkw or "", None)
+
+    global_namespace = _get_globals(func)
+    for name, type_ in types.items():
+        types[name] = _unwrap_types(type_, global_namespace)
+
+    return types
+
+
+def _return_types(func: Callable[..., Any]) -> Union[TypesDict, list[TypesDict]]:
+    """Get the callables return types"""
+    func = _unwrap_function(func)
+    args_spec = getfullargspec(func)
+    return_type = args_spec.annotations.get("return")
+    return _unwrap_types(return_type, _get_globals(func))
+
+
+_type_to_serializer_field: dict[Optional[type], type[Field]] = {
+    str: CharField,
+    int: IntegerField,
+    float: FloatField,
+    bool: BooleanField,
+    dict: DictField,
+    list: ListField,
+    date: DateField,
+    datetime: DateTimeField,
+    time: TimeField,
+    timedelta: DurationField,
+    Decimal: DecimalField,
+    None: CharField,
+    type: CharField,
+}
+_standard_generics_to_typing_equivalents: dict[str, type] = {
+    "list": List[Any],
+    "set": Set[Any],
+    "tuple": Tuple[Any],
+    "dict": Dict[Any, Any],
+    "type": Type[Any],
+}
+
+
+def _get_fields(types: TypesDict) -> dict[str, Field]:
+    """Convert types to serializer fields.
+    TypedDicts and other classes with __annotations__ dicts
+    are recursively converted to serializers based on their types.
+    """
+
+    fields: dict[str, Field] = {}
+    for name, type_ in types.items():
+        # Could not determine forward referenced TypedDict
+        # from another file. This is the best guess.
+        if isinstance(type_, ForwardRef):
+            fields[name] = JSONField()
+            continue
+
+        if isinstance(type_, dict):
+            fields[name] = inline_serializer(name, fields=_get_fields(type_))()
+            continue
+
+        if isinstance(type_, list):
+            if isinstance(type_[0], dict):
+                fields[name] = inline_serializer(name, fields=_get_fields(type_[0]))(many=True)
+            else:
+                fields[name] = ListField(child=_type_to_serializer_field.get(type_[0], CharField)())
+
+            continue
+
+        if get_origin(type_) == Literal:
+            choices = [arg.__forward_arg__ for arg in get_args(type_)]
+            fields[name] = ChoiceField(choices=choices)
+            continue
+
+        field = _type_to_serializer_field.get(type_, CharField)
+        if issubclass(field, DecimalField):
+            fields[name] = field(max_digits=13, decimal_places=3)
+            continue
+
+        fields[name] = field()
+
+    return fields
+
+
+def _unwrap_types(
+    types: Union[type, TypesDict, list[TypesDict]],
+    global_namespace: dict[str, Any],
+) -> Union[type, TypesDict, list[TypesDict]]:
+    """Recursively unwrap types from the given item."""
+    typ = _forward_refs_to_types(types, global_namespace)
+
+    if hasattr(typ, "__origin__"):
+        return _unwrap_generic(typ, global_namespace)
+
+    if not hasattr(typ, "__annotations__"):
+        return typ
+
+    annotations: TypesDict = typ.__annotations__
+    for name, annotation in annotations.items():
+        annotations[name] = _unwrap_types(annotation, global_namespace)
+
+    return annotations
+
+
+def _forward_refs_to_types(
+    types: Union[type, TypesDict, list[TypesDict]],
+    global_namespace: dict[str, Any],
+) -> Union[type, TypesDict, list[TypesDict]]:
+    """Convert strings and forward references to types."""
+    if isinstance(types, str):
+        types = ForwardRef(types)
+
+    if isinstance(types, ForwardRef):
+        try:
+            types = eval_type(types, global_namespace, global_namespace)
+        except NameError:
+            pass
+
+    if hasattr(types, "__args__"):
+        args = []
+        for arg in types.__args__:
+            args.append(_forward_refs_to_types(arg, global_namespace))
+        types = _standard_generics_to_typing_equivalents.get(getattr(types, "__qualname__", types), types)
+        types.__args__ = tuple(args)
+
+    return types
+
+
+def _unwrap_generic(
+    type_: type, global_namespace: dict[str, Any]
+) -> Union[list[TypesDict], dict[str, list[TypesDict]], type]:
+    """Unwrap the arguments of generics like list and dicts into proper types."""
+    origin_type: type = get_origin(type_)
+    origin_args: tuple[type, ...] = get_args(type_)
+    special_type = origin_type in (Union,)
+
+    try:
+        if not issubclass(origin_type, (tuple, list, set, dict)):  # pragma: no cover
+            return type_
+    except TypeError:
+        if not special_type:
+            return type_
+
+    if not special_type and issubclass(origin_type, dict):
+        origin_args = origin_args[1:]
+
+    arg_types = _get_arg_types(origin_args, global_namespace)
+
+    if origin_type == Union:
+        return arg_types[0]
+
+    if issubclass(origin_type, dict):
+        return {"str": arg_types[0]}
+
+    return arg_types
+
+
+def _get_arg_types(
+    origin_args: tuple[type, ...],
+    global_namespace: dict[str, Any],
+) -> Union[list[TypesDict], dict[str, list[TypesDict]], type]:
+    arg_types = []
+
+    for arg_type in origin_args:
+        arg_type = _forward_refs_to_types(arg_type, global_namespace)
+
+        if not hasattr(arg_type, "__annotations__"):
+            if hasattr(arg_type, "__origin__"):
+                arg_type = _unwrap_generic(arg_type, global_namespace)
+
+            arg_types.append(arg_type)
+            continue
+
+        annotations = {}
+        for name, annotation in arg_type.__annotations__.items():
+            annotations[name] = _unwrap_types(annotation, global_namespace)
+
+        arg_types.append(annotations)
+
+    return arg_types
+
+
+def _unwrap_function(func: Callable[..., Any]) -> Callable[..., Any]:
+    """Unwrap decorated functions to allow fetching types from them."""
+    while hasattr(func, "__wrapped__"):
+        func = func.__wrapped__
+    return func
+
+
+def _get_globals(func: Callable[..., Any]) -> dict[str, Any]:
+    return getattr(_unwrap_function(func), "__globals__", {})
+
+
+def _to_comparable_dict(serializer: Serializer) -> dict[str, Any]:
+    dct = {}
+    is_list = isinstance(serializer, ListSerializer)
+    fields = serializer.child.fields if is_list else serializer.fields
+    for name, field in fields.items():
+        if isinstance(field, ListSerializer):
+            dct[name] = [_to_comparable_dict(field.child)]
+        elif isinstance(field, Serializer):
+            dct[name] = _to_comparable_dict(field)
+        else:
+            dct[name] = str(field)
+    return [dct] if is_list else dct
```

### Comparing `drf_serializer_inference-0.0.1/PKG-INFO` & `drf_serializer_inference-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-inference
-Version: 0.0.1
+Version: 0.0.2
 Summary: Infer Django Rest Framework serializers from callables like functions and classes.
 Home-page: https://mrthearman.github.io/drf-serializer-inference
 License: MIT
 Keywords: drf,django,rest_framework,rest,framework,inference,serializer
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
@@ -18,18 +18,16 @@
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
-Requires-Dist: Django (>=3.2)
 Requires-Dist: djangorestframework (>=3.12.0)
 Requires-Dist: pydantic (>=1.6.2) ; extra == "pydantic"
 Requires-Dist: typing-extensions (>=4.4.0) ; python_version < "3.10"
 Project-URL: Bug Tracker, https://github.com/MrThearMan/drf-serializer-inference/issues
 Project-URL: Repository, https://github.com/MrThearMan/drf-serializer-inference
 Description-Content-Type: text/markdown
```

