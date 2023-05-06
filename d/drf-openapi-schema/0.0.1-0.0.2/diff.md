# Comparing `tmp/drf_openapi_schema-0.0.1.tar.gz` & `tmp/drf_openapi_schema-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_openapi_schema-0.0.1.tar", max compression
+gzip compressed data, was "drf_openapi_schema-0.0.2.tar", max compression
```

## Comparing `drf_openapi_schema-0.0.1.tar` & `drf_openapi_schema-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1090 2023-05-01 08:24:17.420862 drf_openapi_schema-0.0.1/LICENSE
--rw-r--r--   0        0        0      283 2023-05-01 08:51:08.246340 drf_openapi_schema-0.0.1/openapi_schema/__init__.py
--rw-r--r--   0        0        0     9990 2023-05-01 08:31:55.366939 drf_openapi_schema-0.0.1/openapi_schema/generator.py
--rw-r--r--   0        0        0        0 2023-05-01 08:24:17.513862 drf_openapi_schema-0.0.1/openapi_schema/py.typed
--rw-r--r--   0        0        0    19524 2023-05-01 09:19:16.104845 drf_openapi_schema-0.0.1/openapi_schema/schema.py
--rw-r--r--   0        0        0    41959 2023-05-01 09:56:41.158964 drf_openapi_schema-0.0.1/openapi_schema/typing.py
--rw-r--r--   0        0        0    13140 2023-05-01 09:31:52.313933 drf_openapi_schema-0.0.1/openapi_schema/utils.py
--rw-r--r--   0        0        0     4921 2023-05-01 08:58:10.783161 drf_openapi_schema-0.0.1/openapi_schema/views.py
--rw-r--r--   0        0        0     4235 2023-05-01 09:33:35.984775 drf_openapi_schema-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2005 2023-05-01 08:30:13.797114 drf_openapi_schema-0.0.1/README.md
--rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 drf_openapi_schema-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1963 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/README.md
+-rw-r--r--   0        0        0      266 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/openapi_schema/__init__.py
+-rw-r--r--   0        0        0     9718 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/openapi_schema/generator.py
+-rw-r--r--   0        0        0        0 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/openapi_schema/py.typed
+-rw-r--r--   0        0        0    19026 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/openapi_schema/schema.py
+-rw-r--r--   0        0        0    42633 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/openapi_schema/typing.py
+-rw-r--r--   0        0        0    14439 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/openapi_schema/utils.py
+-rw-r--r--   0        0        0     4755 2023-05-06 10:16:25.897361 drf_openapi_schema-0.0.2/openapi_schema/views.py
+-rw-r--r--   0        0        0     3999 2023-05-06 10:16:25.901361 drf_openapi_schema-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 drf_openapi_schema-0.0.2/PKG-INFO
```

### Comparing `drf_openapi_schema-0.0.1/openapi_schema/views.py` & `drf_openapi_schema-0.0.2/openapi_schema/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from types import ModuleType
-from typing import Dict, List, Optional, Type, Union
-
-from django.urls import URLPattern, URLResolver
-from rest_framework.authentication import BaseAuthentication
-from rest_framework.permissions import BasePermission
-from rest_framework.renderers import BrowsableAPIRenderer, JSONOpenAPIRenderer, OpenAPIRenderer
-from rest_framework.request import Request
-from rest_framework.response import Response
-from rest_framework.settings import api_settings
-from rest_framework.views import APIView
-
-from .generator import PipelineSchemaGenerator
-from .typing import (
-    APIContact,
-    APILicense,
-    APISecurityScheme,
-    AsView,
-    EventName,
-    GenericView,
-    SchemaWebhook,
-    SchemeName,
-    SecurityRules,
-    UrlPath,
-)
-
-
-class PipelineSchemaView(APIView):
-    _ignore_model_permissions: bool = True
-    schema = None  # exclude from schema
-    schema_generator = PipelineSchemaGenerator()
-    renderer_classes = [OpenAPIRenderer, JSONOpenAPIRenderer]
-    public: bool = True
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        if BrowsableAPIRenderer in api_settings.DEFAULT_RENDERER_CLASSES:
-            self.renderer_classes += [BrowsableAPIRenderer]
-
-    def get(self, request: Request, *args, **kwargs) -> Response:
-        schema = self.schema_generator.get_schema(request, self.public)
-        return Response(schema)
-
-    def handle_exception(self, exc: Exception) -> Response:  # pragma: no cover
-        # Schema renderers do not render exceptions, so re-perform content
-        # negotiation with default renderers.
-        self.renderer_classes = api_settings.DEFAULT_RENDERER_CLASSES
-        neg = self.perform_content_negotiation(self.request, force=True)
-        self.request.accepted_renderer, self.request.accepted_media_type = neg
-        return super().handle_exception(exc)
-
-
-def get_schema_view(
-    *,
-    title: Optional[str] = None,
-    root_url: Optional[UrlPath] = None,
-    description: Optional[str] = None,
-    patterns: Optional[List[Union[URLPattern, URLResolver]]] = None,
-    urlconf: Optional[Union[str, ModuleType]] = None,
-    version: Optional[str] = None,
-    webhooks: Optional[Dict[EventName, SchemaWebhook]] = None,
-    contact: Optional[APIContact] = None,
-    license: Optional[APILicense] = None,
-    terms_of_service: UrlPath = "",
-    public: Optional[bool] = None,
-    security_schemes: Optional[Dict[SchemeName, APISecurityScheme]] = None,
-    security_rules: Optional[SecurityRules] = None,
-    authentication_classes: Optional[List[Type[BaseAuthentication]]] = None,
-    permission_classes: Optional[List[Type[BasePermission]]] = None,
-) -> AsView[GenericView]:
-    """Return a schema view.
-
-    :param title: The name of the API (required).
-    :param root_url: The root URL prefix of the API schema. Useful for defining versioned API.
-    :param description: Longer descriptive text.
-    :param patterns: A list of URLs to inspect when generating the schema.
-                     Defaults to the project's URL conf.
-    :param urlconf: A URL conf module to use when generating the schema.
-                    Defaults to settings.ROOT_URLCONF.
-    :param version: The version of the API. Defaults to 0.1.0.
-    :param webhooks: Webhooks defined in the API.
-    :param contact: API developer contact information.
-    :param license: API license information.
-    :param terms_of_service: API terms of service link.
-    :param public: If False, hide endpoint schema if the user does not have permissions to view it.
-    :param security_schemes: Mapping of security scheme name to its definition.
-    :param security_rules: Security schemes to apply if defined authentication or
-                           permission class(es) exist on an endpoint.
-    :param authentication_classes: Authentication classes for the OpenAPI SchemaView.
-    :param permission_classes: Permission classes for the OpenAPI SchemaView.
-    """
-
-    generator = PipelineSchemaGenerator(
-        title=title,
-        root_url=root_url,
-        description=description,
-        patterns=patterns,
-        urlconf=urlconf,
-        version=version,
-        webhooks=webhooks,
-        contact=contact,
-        license=license,
-        security_schemes=security_schemes,
-        security_rules=security_rules,
-        terms_of_service=terms_of_service,
-    )
-
-    return PipelineSchemaView.as_view(  # type: ignore
-        schema_generator=generator,
-        public=public,
-        authentication_classes=(
-            authentication_classes
-            if authentication_classes is not None
-            else api_settings.DEFAULT_AUTHENTICATION_CLASSES
-        ),
-        permission_classes=(
-            permission_classes if permission_classes is not None else api_settings.DEFAULT_PERMISSION_CLASSES
-        ),
-    )
+from django.urls import URLPattern, URLResolver
+from rest_framework.authentication import BaseAuthentication
+from rest_framework.permissions import BasePermission
+from rest_framework.renderers import BrowsableAPIRenderer, JSONOpenAPIRenderer, OpenAPIRenderer
+from rest_framework.request import Request
+from rest_framework.response import Response
+from rest_framework.settings import api_settings
+from rest_framework.views import APIView
+
+from .generator import OpenAPISchemaGenerator
+from .typing import (
+    APIContact,
+    APILicense,
+    APISecurityScheme,
+    AsView,
+    EventName,
+    GenericView,
+    ModuleType,
+    Optional,
+    SchemaWebhook,
+    SchemeName,
+    SecurityRules,
+    Union,
+    UrlPath,
+)
+
+
+class OpenAPISchemaView(APIView):
+    _ignore_model_permissions: bool = True
+    schema = None  # exclude from schema
+    schema_generator = OpenAPISchemaGenerator()
+    renderer_classes = [OpenAPIRenderer, JSONOpenAPIRenderer]
+    public: bool = True
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        if BrowsableAPIRenderer in api_settings.DEFAULT_RENDERER_CLASSES:
+            self.renderer_classes += [BrowsableAPIRenderer]
+
+    def get(self, request: Request, *args, **kwargs) -> Response:
+        schema = self.schema_generator.get_schema(request, self.public)
+        return Response(schema)
+
+    def handle_exception(self, exc: Exception) -> Response:  # pragma: no cover
+        # Schema renderers do not render exceptions, so re-perform content
+        # negotiation with default renderers.
+        self.renderer_classes = api_settings.DEFAULT_RENDERER_CLASSES
+        neg = self.perform_content_negotiation(self.request, force=True)
+        self.request.accepted_renderer, self.request.accepted_media_type = neg
+        return super().handle_exception(exc)
+
+
+def get_schema_view(
+    *,
+    title: Optional[str] = None,
+    root_url: Optional[UrlPath] = None,
+    description: Optional[str] = None,
+    patterns: Optional[list[Union[URLPattern, URLResolver]]] = None,
+    urlconf: Optional[Union[str, ModuleType]] = None,
+    version: Optional[str] = None,
+    webhooks: Optional[dict[EventName, SchemaWebhook]] = None,
+    contact: Optional[APIContact] = None,
+    license: Optional[APILicense] = None,
+    terms_of_service: UrlPath = "",
+    public: Optional[bool] = None,
+    security_schemes: Optional[dict[SchemeName, APISecurityScheme]] = None,
+    security_rules: Optional[SecurityRules] = None,
+    authentication_classes: Optional[list[type[BaseAuthentication]]] = None,
+    permission_classes: Optional[list[type[BasePermission]]] = None,
+) -> AsView[GenericView]:
+    """Return a schema view.
+
+    :param title: The name of the API (required).
+    :param root_url: The root URL prefix of the API schema. Useful for defining versioned API.
+    :param description: Longer descriptive text.
+    :param patterns: A list of URLs to inspect when generating the schema.
+                     Defaults to the project's URL conf.
+    :param urlconf: A URL conf module to use when generating the schema.
+                    Defaults to settings.ROOT_URLCONF.
+    :param version: The version of the API. Defaults to 0.1.0.
+    :param webhooks: Webhooks defined in the API.
+    :param contact: API developer contact information.
+    :param license: API license information.
+    :param terms_of_service: API terms of service link.
+    :param public: If False, hide endpoint schema if the user does not have permissions to view it.
+    :param security_schemes: Mapping of security scheme name to its definition.
+    :param security_rules: Security schemes to apply if defined authentication or
+                           permission class(es) exist on an endpoint.
+    :param authentication_classes: Authentication classes for the OpenAPI SchemaView.
+    :param permission_classes: Permission classes for the OpenAPI SchemaView.
+    """
+
+    generator = OpenAPISchemaGenerator(
+        title=title,
+        root_url=root_url,
+        description=description,
+        patterns=patterns,
+        urlconf=urlconf,
+        version=version,
+        webhooks=webhooks,
+        contact=contact,
+        license=license,
+        security_schemes=security_schemes,
+        security_rules=security_rules,
+        terms_of_service=terms_of_service,
+    )
+
+    return OpenAPISchemaView.as_view(  # type: ignore
+        schema_generator=generator,
+        public=public,
+        authentication_classes=(
+            authentication_classes
+            if authentication_classes is not None
+            else api_settings.DEFAULT_AUTHENTICATION_CLASSES
+        ),
+        permission_classes=(
+            permission_classes if permission_classes is not None else api_settings.DEFAULT_PERMISSION_CLASSES
+        ),
+    )
```

### Comparing `drf_openapi_schema-0.0.1/pyproject.toml` & `drf_openapi_schema-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,191 +1,190 @@
-[tool.poetry]
-name = "drf-openapi-schema"
-version = "0.0.1"
-description = "Django Rest Framework OpenAPI Schema generation."
-authors = [
-    "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
-]
-packages = [
-    { include = "openapi_schema" },
-]
-license = "MIT"
-readme = "README.md"
-homepage = "https://mrthearman.github.io/drf-openapi-schema"
-repository = "https://github.com/MrThearMan/drf-openapi-schema"
-keywords = [
-    "drf",
-    "django",
-    "rest_framework",
-    "rest",
-    "framework",
-    "openapi",
-    "schema",
-    "generator",
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
-"Bug Tracker" = "https://github.com/MrThearMan/drf-openapi-schema/issues"
-
-[tool.poetry.dependencies]
-python = ">=3.9,<4"
-Django = ">=3.2"
-djangorestframework = ">=3.12.0"
-drf-serializer-inference = ">=0.0.1"
-PyYAML = ">=6.0"
-typing-extensions = {version = ">=4.4.0", python = "<3.11"}
-pydantic = {version = ">=1.6.2", optional = true}
-uritemplate = {version = ">=4.1.1", optional = true}
-
-[tool.poetry.group.test.dependencies]
-pytest = "7.3.0"
-coverage = "6.5.0"
-pytest-django = "4.5.2"
-pre-commit = "3.2.2"
-tox = "4.4.12"
-tox-gh-actions = "3.1.0"
-coveralls = "3.3.1"
-drf-pipeline-views = "0.8.5"
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
-uritemplate = ["uritemplate"]
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
-    "openapi_schema.typing",
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
-[tool.ruff.per-file-ignores]
-"openapi_schema/schema.py" = ["C901"]
-"openapi_schema/utils.py" = ["C901"]
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
-[tool.django-stubs]
-django_settings_module = "tests.django.settings"
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
-    3.9: py39
-    3.10: py310
-    3.11: py311
-
-[testenv]
-allowlist_externals =
-    poetry
-setenv =
-    PYTHONPATH = {toxinidir}
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
-    drf-serializer-inference
-
-    pytest
-    coverage
-    pytest-django
-    typing-extensions
-    pydantic
-    pyyaml
-    uritemplate
-    drf-pipeline-views
-commands =
-    coverage run -m pytest -vv -s --log-cli-level=INFO
-"""
-
-[build-system]
-requires = ["poetry-core>=1.5.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "drf-openapi-schema"
+version = "0.0.2"
+description = "Django Rest Framework OpenAPI Schema generation."
+authors = [
+    "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
+]
+packages = [
+    { include = "openapi_schema" },
+]
+license = "MIT"
+readme = "README.md"
+homepage = "https://mrthearman.github.io/drf-openapi-schema"
+repository = "https://github.com/MrThearMan/drf-openapi-schema"
+keywords = [
+    "drf",
+    "django",
+    "rest_framework",
+    "rest",
+    "framework",
+    "openapi",
+    "schema",
+    "generator",
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
+"Bug Tracker" = "https://github.com/MrThearMan/drf-openapi-schema/issues"
+
+[tool.poetry.dependencies]
+python = ">=3.9,<4"
+Django = ">=3.2"
+djangorestframework = ">=3.12.0"
+drf-serializer-inference = ">=0.0.1"
+PyYAML = ">=6.0"
+typing-extensions = {version = ">=4.4.0", python = "<3.11"}
+pydantic = {version = ">=1.6.2", optional = true}
+uritemplate = {version = ">=4.1.1", optional = true}
+
+[tool.poetry.group.test.dependencies]
+pytest = "7.3.0"
+coverage = "6.5.0"
+pytest-django = "4.5.2"
+pre-commit = "3.2.2"
+tox = "4.4.12"
+tox-gh-actions = "3.1.0"
+coveralls = "3.3.1"
+drf-pipeline-views = "0.8.5"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "1.4.2"
+pymdown-extensions = "9.11"
+mkdocs-mermaid2-plugin = "0.6.0"
+
+[tool.poetry.group.lint.dependencies]
+mypy = "1.2.0"
+django-stubs = "1.16.0"
+djangorestframework-stubs = "1.10.0"
+
+[tool.poetry.extras]
+pydantic = ["pydantic"]
+uritemplate = ["uritemplate"]
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
+    "openapi_schema.typing",
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
+[tool.ruff.per-file-ignores]
+"openapi_schema/schema.py" = ["C901"]
+"openapi_schema/utils.py" = ["C901"]
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
+[tool.django-stubs]
+django_settings_module = "tests.django.settings"
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
+setenv =
+    PYTHONPATH = {toxinidir}
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
+    drf-serializer-inference
+
+    pytest
+    coverage
+    pytest-django
+    typing-extensions
+    pydantic
+    pyyaml
+    uritemplate
+    drf-pipeline-views
+commands =
+    coverage run -m pytest -vv -s --log-cli-level=INFO
+"""
+
+[build-system]
+requires = ["poetry-core>=1.5.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `drf_openapi_schema-0.0.1/README.md` & `drf_openapi_schema-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Django Rest Framework OpenAPI Schema
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
-pip install drf-openapi-schema
-```
-
----
-
-**Documentation**: [https://mrthearman.github.io/drf-openapi-schema/](https://mrthearman.github.io/drf-openapi-schema/)
-
-**Source Code**: [https://github.com/MrThearMan/drf-openapi-schema/](https://github.com/MrThearMan/drf-openapi-schema/)
-
-**Contributing**: [https://github.com/MrThearMan/drf-openapi-schema/blob/main/CONTRIBUTING.md](https://github.com/MrThearMan/drf-openapi-schema/blob/main/CONTRIBUTING.md)
-
----
-
-...
-
-[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/drf-openapi-schema/badge.svg?branch=main
-[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/drf-openapi-schema/test.yml?branch=main
-[pypi-badge]: https://img.shields.io/pypi/v/drf-openapi-schema
-[licence-badge]: https://img.shields.io/github/license/MrThearMan/drf-openapi-schema
-[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/drf-openapi-schema
-[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/drf-openapi-schema
-[version-badge]: https://img.shields.io/pypi/pyversions/drf-openapi-schema
-[downloads-badge]: https://img.shields.io/pypi/dm/drf-openapi-schema
-
-[coverage]: https://coveralls.io/github/MrThearMan/drf-openapi-schema?branch=main
-[status]: https://github.com/MrThearMan/drf-openapi-schema/actions/workflows/test.yml
-[pypi]: https://pypi.org/project/drf-openapi-schema
-[licence]: https://github.com/MrThearMan/drf-openapi-schema/blob/main/LICENSE
-[repo]: https://github.com/MrThearMan/drf-openapi-schema/commits/main
-[issues]: https://github.com/MrThearMan/drf-openapi-schema/issues
+# Django Rest Framework OpenAPI Schema
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
+pip install drf-openapi-schema
+```
+
+---
+
+**Documentation**: [https://mrthearman.github.io/drf-openapi-schema/](https://mrthearman.github.io/drf-openapi-schema/)
+
+**Source Code**: [https://github.com/MrThearMan/drf-openapi-schema/](https://github.com/MrThearMan/drf-openapi-schema/)
+
+**Contributing**: [https://github.com/MrThearMan/drf-openapi-schema/blob/main/CONTRIBUTING.md](https://github.com/MrThearMan/drf-openapi-schema/blob/main/CONTRIBUTING.md)
+
+---
+
+...
+
+[coverage-badge]: https://coveralls.io/repos/github/MrThearMan/drf-openapi-schema/badge.svg?branch=main
+[status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/drf-openapi-schema/test.yml?branch=main
+[pypi-badge]: https://img.shields.io/pypi/v/drf-openapi-schema
+[licence-badge]: https://img.shields.io/github/license/MrThearMan/drf-openapi-schema
+[repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/drf-openapi-schema
+[issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/drf-openapi-schema
+[version-badge]: https://img.shields.io/pypi/pyversions/drf-openapi-schema
+[downloads-badge]: https://img.shields.io/pypi/dm/drf-openapi-schema
+
+[coverage]: https://coveralls.io/github/MrThearMan/drf-openapi-schema?branch=main
+[status]: https://github.com/MrThearMan/drf-openapi-schema/actions/workflows/test.yml
+[pypi]: https://pypi.org/project/drf-openapi-schema
+[licence]: https://github.com/MrThearMan/drf-openapi-schema/blob/main/LICENSE
+[repo]: https://github.com/MrThearMan/drf-openapi-schema/commits/main
+[issues]: https://github.com/MrThearMan/drf-openapi-schema/issues
```

### Comparing `drf_openapi_schema-0.0.1/PKG-INFO` & `drf_openapi_schema-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-openapi-schema
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django Rest Framework OpenAPI Schema generation.
 Home-page: https://mrthearman.github.io/drf-openapi-schema
 License: MIT
 Keywords: drf,django,rest_framework,rest,framework,openapi,schema,generator
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
@@ -18,15 +18,14 @@
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
 Provides-Extra: uritemplate
 Requires-Dist: Django (>=3.2)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: djangorestframework (>=3.12.0)
 Requires-Dist: drf-serializer-inference (>=0.0.1)
```

