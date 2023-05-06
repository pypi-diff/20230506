# Comparing `tmp/bananaproto-1.1.1.tar.gz` & `tmp/bananaproto-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bananaproto-1.1.1.tar", max compression
+gzip compressed data, was "bananaproto-1.1.2.tar", max compression
```

## Comparing `bananaproto-1.1.1.tar` & `bananaproto-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    16280 2023-05-06 00:10:49.508651 bananaproto-1.1.1/README.md
--rw-r--r--   0        0        0     3451 2023-05-06 00:11:45.076772 bananaproto-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    56436 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/__init__.py
--rw-r--r--   0        0        0      295 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/_types.py
--rw-r--r--   0        0        0       99 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/_version.py
--rw-r--r--   0        0        0     3543 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/casing.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/compile/__init__.py
--rw-r--r--   0        0        0     6337 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/compile/importing.py
--rw-r--r--   0        0        0      286 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/compile/naming.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/__init__.py
--rw-r--r--   0        0        0     5295 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/grpclib_client.py
--rw-r--r--   0        0        0      982 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/grpclib_server.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/util/__init__.py
--rw-r--r--   0        0        0     6793 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/util/async_channel.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/lib/google/__init__.py
--rw-r--r--   0        0        0    70836 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/__init__.py
--rw-r--r--   0        0        0     7057 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/compiler/__init__.py
--rw-r--r--   0        0        0       23 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/__init__.py
--rw-r--r--   0        0        0       32 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/__main__.py
--rw-r--r--   0        0        0     1320 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/compiler.py
--rwxr-xr-x   0        0        0     1471 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/main.py
--rw-r--r--   0        0        0    28084 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/models.py
--rw-r--r--   0        0        0     7649 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/parser.py
--rw-r--r--   0        0        0       48 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/plugin.bat
--rw-r--r--   0        0        0        0 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/py.typed
--rw-r--r--   0        0        0     8391 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/templates/template.py.j2
--rw-r--r--   0        0        0    18193 1970-01-01 00:00:00.000000 bananaproto-1.1.1/setup.py
--rw-r--r--   0        0        0    17389 1970-01-01 00:00:00.000000 bananaproto-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    16280 2023-05-06 11:29:30.286586 bananaproto-1.1.2/README.md
+-rw-r--r--   0        0        0     3488 2023-05-06 11:30:30.853748 bananaproto-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    56436 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/_types.py
+-rw-r--r--   0        0        0       99 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/_version.py
+-rw-r--r--   0        0        0     3543 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/casing.py
+-rw-r--r--   0        0        0        0 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/compile/__init__.py
+-rw-r--r--   0        0        0     6337 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/compile/importing.py
+-rw-r--r--   0        0        0      286 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/compile/naming.py
+-rw-r--r--   0        0        0        0 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/grpc/__init__.py
+-rw-r--r--   0        0        0     5295 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/grpc/grpclib_client.py
+-rw-r--r--   0        0        0      982 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/grpc/grpclib_server.py
+-rw-r--r--   0        0        0        0 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/grpc/util/__init__.py
+-rw-r--r--   0        0        0     6793 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/grpc/util/async_channel.py
+-rw-r--r--   0        0        0        0 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/lib/google/__init__.py
+-rw-r--r--   0        0        0    70836 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/lib/google/protobuf/__init__.py
+-rw-r--r--   0        0        0     7057 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/lib/google/protobuf/compiler/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/plugin/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/plugin/__main__.py
+-rw-r--r--   0        0        0     1320 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/plugin/compiler.py
+-rwxr-xr-x   0        0        0     1471 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/plugin/main.py
+-rw-r--r--   0        0        0    28084 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/plugin/models.py
+-rw-r--r--   0        0        0     7649 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/plugin/parser.py
+-rw-r--r--   0        0        0       48 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/plugin/plugin.bat
+-rw-r--r--   0        0        0        0 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/py.typed
+-rw-r--r--   0        0        0     8391 2023-05-06 11:29:30.290587 bananaproto-1.1.2/src/bananaproto/templates/template.py.j2
+-rw-r--r--   0        0        0    18193 1970-01-01 00:00:00.000000 bananaproto-1.1.2/setup.py
+-rw-r--r--   0        0        0    17389 1970-01-01 00:00:00.000000 bananaproto-1.1.2/PKG-INFO
```

### Comparing `bananaproto-1.1.1/README.md` & `bananaproto-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/pyproject.toml` & `bananaproto-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bananaproto"
-version = "v1.1.1"
+version = "v1.1.2"
 description = "A BANANA Protobuf / gRPC generator & library"
 authors = ["Daniel G. Taylor <danielgtaylor@gmail.com>"]
 maintainers = ["BananaLoaf <bananaloaf@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/BananaLoaf/python-bananaproto"
 keywords = ["protobuf", "gRPC"]
 license = "MIT"
@@ -34,14 +34,16 @@
 pytest-mock = "^3.1.1"
 sphinx = "3.1.2"
 sphinx-rtd-theme = "0.5.0"
 tomlkit = "^0.7.0"
 tox = "^3.15.1"
 pre-commit = "^2.17.0"
 pydantic = ">=1.8.0"
+black = ">=19.3b0"
+isort = "^5.11.5"
 
 
 [tool.poetry.scripts]
 protoc-gen-python_bananaproto = "bananaproto.plugin:main"
 
 [tool.poetry.extras]
 compiler = ["black", "isort", "jinja2"]
```

### Comparing `bananaproto-1.1.1/src/bananaproto/__init__.py` & `bananaproto-1.1.2/src/bananaproto/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/casing.py` & `bananaproto-1.1.2/src/bananaproto/casing.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/compile/importing.py` & `bananaproto-1.1.2/src/bananaproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/grpc/grpclib_client.py` & `bananaproto-1.1.2/src/bananaproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/grpc/grpclib_server.py` & `bananaproto-1.1.2/src/bananaproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/grpc/util/async_channel.py` & `bananaproto-1.1.2/src/bananaproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/__init__.py` & `bananaproto-1.1.2/src/bananaproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/compiler/__init__.py` & `bananaproto-1.1.2/src/bananaproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/plugin/compiler.py` & `bananaproto-1.1.2/src/bananaproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/plugin/main.py` & `bananaproto-1.1.2/src/bananaproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/plugin/models.py` & `bananaproto-1.1.2/src/bananaproto/plugin/models.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/plugin/parser.py` & `bananaproto-1.1.2/src/bananaproto/plugin/parser.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/src/bananaproto/templates/template.py.j2` & `bananaproto-1.1.2/src/bananaproto/templates/template.py.j2`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.1/setup.py` & `bananaproto-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 {'compiler': ['black>=19.3b0', 'jinja2>=3.0.3', 'isort>=5.11.5,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['protoc-gen-python_bananaproto = bananaproto.plugin:main']}
 
 setup_kwargs = {
     'name': 'bananaproto',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'A BANANA Protobuf / gRPC generator & library',
     'long_description': '# BANANA Protobuf / gRPC Support for Python\n\n![](https://github.com/danielgtaylor/python-bananaproto/workflows/CI/badge.svg)\n> :octocat: If you\'re reading this on github, please be aware that it might mention unreleased features! See the latest released README on [pypi](https://pypi.org/project/bananaproto/).\n\nThis project aims to provide an improved experience when using Protobuf / gRPC in a modern Python environment by making use of modern language features and generating readable, understandable, idiomatic Python code. It will not support legacy features or environments (e.g. Protobuf 2). The following are supported:\n\n- Protobuf 3 & gRPC code generation\n  - Both binary & JSON serialization is built-in\n- Python 3.7+ making use of:\n  - Enums\n  - Dataclasses\n  - `async`/`await`\n  - Timezone-aware `datetime` and `timedelta` objects\n  - Relative imports\n  - Mypy type checking\n- [Pydantic Models](https://docs.pydantic.dev/) generation (see #generating-pydantic-models)\n\nThis project is heavily inspired by, and borrows functionality from:\n\n- https://github.com/protocolbuffers/protobuf/tree/master/python\n- https://github.com/eigenein/protobuf/\n- https://github.com/vmagamedov/grpclib\n\n## Motivation\n\nThis project exists because I am unhappy with the state of the official Google protoc plugin for Python.\n\n- No `async` support (requires additional `grpclib` plugin)\n- No typing support or code completion/intelligence (requires additional `mypy` plugin)\n- No `__init__.py` module files get generated\n- Output is not importable\n  - Import paths break in Python 3 unless you mess with `sys.path`\n- Bugs when names clash (e.g. `codecs` package)\n- Generated code is not idiomatic\n  - Completely unreadable runtime code-generation\n  - Much code looks like C++ or Java ported 1:1 to Python\n  - Capitalized function names like `HasField()` and `SerializeToString()`\n  - Uses `SerializeToString()` rather than the built-in `__bytes__()`\n  - Special wrapped types don\'t use Python\'s `None`\n  - Timestamp/duration types don\'t use Python\'s built-in `datetime` module\n\n\nThis project is a reimplementation from the ground up focused on idiomatic modern Python to help fix some of the above. While it may not be a 1:1 drop-in replacement due to changed method names and call patterns, the wire format is identical.\n\n## Installation\n\nFirst, install the package. Note that the `[compiler]` feature flag tells it to install extra dependencies only needed by the `protoc` plugin:\n\n```sh\n# Install both the library and compiler\npip install "bananaproto[compiler]"\n\n# Install just the library (to use the generated code output)\npip install bananaproto\n```\n\n*Bananaproto* is under active development. To install the latest beta version, use `pip install --pre bananaproto`.\n\n## Getting Started\n\n### Compiling proto files\n\nGiven you installed the compiler and have a proto file, e.g `example.proto`:\n\n```protobuf\nsyntax = "proto3";\n\npackage hello;\n\n// Greeting represents a message you can tell a user.\nmessage Greeting {\n  string message = 1;\n}\n```\n\nYou can run the following to invoke protoc directly:\n\n```sh\nmkdir lib\nprotoc -I . --python_bananaproto_out=lib example.proto\n```\n\nor run the following to invoke protoc via grpcio-tools:\n\n```sh\npip install grpcio-tools\npython -m grpc_tools.protoc -I . --python_bananaproto_out=lib example.proto\n```\n\nThis will generate `lib/hello/__init__.py` which looks like:\n\n```python\n# Generated by the protocol buffer compiler.  DO NOT EDIT!\n# sources: example.proto\n# plugin: python-bananaproto\nfrom dataclasses import dataclass\n\nimport bananaproto\n\n\n@dataclass\nclass Greeting(bananaproto.Message):\n  """Greeting represents a message you can tell a user."""\n\n  message: str = bananaproto.string_field(1)\n```\n\nNow you can use it!\n\n```python\n>>> from lib.hello import Greeting\n>>> test = Greeting()\n>>> test\nGreeting(message=\'\')\n\n>>> test.message = "Hey!"\n>>> test\nGreeting(message="Hey!")\n\n>>> serialized = bytes(test)\n>>> serialized\nb\'\\n\\x04Hey!\'\n\n>>> another = Greeting().parse(serialized)\n>>> another\nGreeting(message="Hey!")\n\n>>> another.to_dict()\n{"message": "Hey!"}\n>>> another.to_json(indent=2)\n\'{\\n  "message": "Hey!"\\n}\'\n```\n\n### Async gRPC Support\n\nThe generated Protobuf `Message` classes are compatible with [grpclib](https://github.com/vmagamedov/grpclib) so you are free to use it if you like. That said, this project also includes support for async gRPC stub generation with better static type checking and code completion support. It is enabled by default.\n\nGiven an example service definition:\n\n```protobuf\nsyntax = "proto3";\n\npackage echo;\n\nmessage EchoRequest {\n  string value = 1;\n  // Number of extra times to echo\n  uint32 extra_times = 2;\n}\n\nmessage EchoResponse {\n  repeated string values = 1;\n}\n\nmessage EchoStreamResponse  {\n  string value = 1;\n}\n\nservice Echo {\n  rpc Echo(EchoRequest) returns (EchoResponse);\n  rpc EchoStream(EchoRequest) returns (stream EchoStreamResponse);\n}\n```\n\nGenerate echo proto file:\n\n```\npython -m grpc_tools.protoc -I . --python_bananaproto_out=. echo.proto\n```\n\nA client can be implemented as follows:\n```python\nimport asyncio\nimport echo\n\nfrom grpclib.client import Channel\n\n\nasync def main():\n    channel = Channel(host="127.0.0.1", port=50051)\n    service = echo.EchoStub(channel)\n    response = await service.echo(echo.EchoRequest(value="hello", extra_times=1))\n    print(response)\n\n    async for response in service.echo_stream(echo.EchoRequest(value="hello", extra_times=1)):\n        print(response)\n\n    # don\'t forget to close the channel when done!\n    channel.close()\n\n\nif __name__ == "__main__":\n    loop = asyncio.get_event_loop()\n    loop.run_until_complete(main())\n\n```\n\nwhich would output\n```python\nEchoResponse(values=[\'hello\', \'hello\'])\nEchoStreamResponse(value=\'hello\')\nEchoStreamResponse(value=\'hello\')\n```\n\nThis project also produces server-facing stubs that can be used to implement a Python\ngRPC server.\nTo use them, simply subclass the base class in the generated files and override the\nservice methods:\n\n```python\nimport asyncio\nfrom echo import EchoBase, EchoRequest, EchoResponse, EchoStreamResponse\nfrom grpclib.server import Server\nfrom typing import AsyncIterator\n\n\nclass EchoService(EchoBase):\n    async def echo(self, echo_request: "EchoRequest") -> "EchoResponse":\n        return EchoResponse([echo_request.value for _ in range(echo_request.extra_times)])\n\n    async def echo_stream(self, echo_request: "EchoRequest") -> AsyncIterator["EchoStreamResponse"]:\n        for _ in range(echo_request.extra_times):\n            yield EchoStreamResponse(echo_request.value)\n\n\nasync def main():\n    server = Server([EchoService()])\n    await server.start("127.0.0.1", 50051)\n    await server.wait_closed()\n\nif __name__ == \'__main__\':\n    loop = asyncio.get_event_loop()\n    loop.run_until_complete(main())\n```\n\n### JSON\n\nBoth serializing and parsing are supported to/from JSON and Python dictionaries using the following methods:\n\n- Dicts: `Message().to_dict()`, `Message().from_dict(...)`\n- JSON: `Message().to_json()`, `Message().from_json(...)`\n\nFor compatibility the default is to convert field names to `camelCase`. You can control this behavior by passing a casing value, e.g:\n\n```python\nMyMessage().to_dict(casing=bananaproto.Casing.SNAKE)\n```\n\n### Determining if a message was sent\n\nSometimes it is useful to be able to determine whether a message has been sent on the wire. This is how the Google wrapper types work to let you know whether a value is unset, set as the default (zero value), or set as something else, for example.\n\nUse `bananaproto.serialized_on_wire(message)` to determine if it was sent. This is a little bit different from the official Google generated Python code, and it lives outside the generated `Message` class to prevent name clashes. Note that it **only** supports Proto 3 and thus can **only** be used to check if `Message` fields are set. You cannot check if a scalar was sent on the wire.\n\n```py\n# Old way (official Google Protobuf package)\n>>> mymessage.HasField(\'myfield\')\n\n# New way (this project)\n>>> bananaproto.serialized_on_wire(mymessage.myfield)\n```\n\n### One-of Support\n\nProtobuf supports grouping fields in a `oneof` clause. Only one of the fields in the group may be set at a given time. For example, given the proto:\n\n```protobuf\nsyntax = "proto3";\n\nmessage Test {\n  oneof foo {\n    bool on = 1;\n    int32 count = 2;\n    string name = 3;\n  }\n}\n```\n\nYou can use `bananaproto.which_one_of(message, group_name)` to determine which of the fields was set. It returns a tuple of the field name and value, or a blank string and `None` if unset.\n\n```py\n>>> test = Test()\n>>> bananaproto.which_one_of(test, "foo")\n["", None]\n\n>>> test.on = True\n>>> bananaproto.which_one_of(test, "foo")\n["on", True]\n\n# Setting one member of the group resets the others.\n>>> test.count = 57\n>>> bananaproto.which_one_of(test, "foo")\n["count", 57]\n>>> test.on\nFalse\n\n# Default (zero) values also work.\n>>> test.name = ""\n>>> bananaproto.which_one_of(test, "foo")\n["name", ""]\n>>> test.count\n0\n>>> test.on\nFalse\n```\n\nAgain this is a little different than the official Google code generator:\n\n```py\n# Old way (official Google protobuf package)\n>>> message.WhichOneof("group")\n"foo"\n\n# New way (this project)\n>>> bananaproto.which_one_of(message, "group")\n["foo", "foo\'s value"]\n```\n\n### Well-Known Google Types\n\nGoogle provides several well-known message types like a timestamp, duration, and several wrappers used to provide optional zero value support. Each of these has a special JSON representation and is handled a little differently from normal messages. The Python mapping for these is as follows:\n\n| Google Message              | Python Type                              | Default                |\n| --------------------------- | ---------------------------------------- | ---------------------- |\n| `google.protobuf.duration`  | [`datetime.timedelta`][td]               | `0`                    |\n| `google.protobuf.timestamp` | Timezone-aware [`datetime.datetime`][dt] | `1970-01-01T00:00:00Z` |\n| `google.protobuf.*Value`    | `Optional[...]`                          | `None`                 |\n| `google.protobuf.*`         | `bananaproto.lib.google.protobuf.*`      | `None`                 |\n\n[td]: https://docs.python.org/3/library/datetime.html#timedelta-objects\n[dt]: https://docs.python.org/3/library/datetime.html#datetime.datetime\n\nFor the wrapper types, the Python type corresponds to the wrapped type, e.g. `google.protobuf.BoolValue` becomes `Optional[bool]` while `google.protobuf.Int32Value` becomes `Optional[int]`. All of the optional values default to `None`, so don\'t forget to check for that possible state. Given:\n\n```protobuf\nsyntax = "proto3";\n\nimport "google/protobuf/duration.proto";\nimport "google/protobuf/timestamp.proto";\nimport "google/protobuf/wrappers.proto";\n\nmessage Test {\n  google.protobuf.BoolValue maybe = 1;\n  google.protobuf.Timestamp ts = 2;\n  google.protobuf.Duration duration = 3;\n}\n```\n\nYou can do stuff like:\n\n```py\n>>> t = Test().from_dict({"maybe": True, "ts": "2019-01-01T12:00:00Z", "duration": "1.200s"})\n>>> t\nTest(maybe=True, ts=datetime.datetime(2019, 1, 1, 12, 0, tzinfo=datetime.timezone.utc), duration=datetime.timedelta(seconds=1, microseconds=200000))\n\n>>> t.ts - t.duration\ndatetime.datetime(2019, 1, 1, 11, 59, 58, 800000, tzinfo=datetime.timezone.utc)\n\n>>> t.ts.isoformat()\n\'2019-01-01T12:00:00+00:00\'\n\n>>> t.maybe = None\n>>> t.to_dict()\n{\'ts\': \'2019-01-01T12:00:00Z\', \'duration\': \'1.200s\'}\n```\n\n## Generating Pydantic Models\n\nYou can use python-bananaproto to generate pydantic based models, using\npydantic dataclasses. This means the results of the protobuf unmarshalling will\nbe typed checked. The usage is the same, but you need to add a custom option\nwhen calling the protobuf compiler:\n\n\n```\nprotoc -I . --custom_opt=pydantic_dataclasses --python_bananaproto_out=lib example.proto\n```\n\nWith the important change being `--custom_opt=pydantic_dataclasses`. This will\nswap the dataclass implementation from the builtin python dataclass to the\npydantic dataclass. You must have pydantic as a dependency in your project for\nthis to work.\n\n\n\n## Development\n\n- _See how you can help &rarr; [Contributing](.github/CONTRIBUTING.md)_\n\n### Requirements\n\n- Python (3.7 or higher)\n\n- [poetry](https://python-poetry.org/docs/#installation)\n  *Needed to install dependencies in a virtual environment*\n\n- [poethepoet](https://github.com/nat-n/poethepoet) for running development tasks as defined in pyproject.toml\n  - Can be installed to your host environment via `pip install poethepoet` then executed as simple `poe`\n  - or run from the poetry venv as `poetry run poe`\n\n### Setup\n\n```sh\n# Get set up with the virtual env & dependencies\npoetry install -E compiler\n\n# Activate the poetry environment\npoetry shell\n```\n\n### Code style\n\nThis project enforces [black](https://github.com/psf/black) python code formatting.\n\nBefore committing changes run:\n\n```sh\npoe format\n```\n\nTo avoid merge conflicts later, non-black formatted python code will fail in CI.\n\n### Tests\n\nThere are two types of tests:\n\n1. Standard tests\n2. Custom tests\n\n#### Standard tests\n\nAdding a standard test case is easy.\n\n- Create a new directory `bananaproto/tests/inputs/<name>`\n  - add `<name>.proto`  with a message called `Test`\n  - add `<name>.json` with some test data (optional)\n\nIt will be picked up automatically when you run the tests.\n\n- See also: [Standard Tests Development Guide](tests/README.md)\n\n#### Custom tests\n\nCustom tests are found in `tests/test_*.py` and are run with pytest.\n\n#### Running\n\nHere\'s how to run the tests.\n\n```sh\n# Generate assets from sample .proto files required by the tests\npoe generate\n# Run the tests\npoe test\n```\n\nTo run tests as they are run in CI (with tox) run:\n\n```sh\npoe full-test\n```\n\n### (Re)compiling Google Well-known Types\n\nBananaproto includes compiled versions for Google\'s well-known types at [src/bananaproto/lib/google](src/bananaproto/lib/google).\nBe sure to regenerate these files when modifying the plugin output format, and validate by running the tests.\n\nNormally, the plugin does not compile any references to `google.protobuf`, since they are pre-compiled. To force compilation of `google.protobuf`, use the option `--custom_opt=INCLUDE_GOOGLE`.\n\nAssuming your `google.protobuf` source files (included with all releases of `protoc`) are located in `/usr/local/include`, you can regenerate them as follows:\n\n```sh\nprotoc \\\n    --plugin=protoc-gen-custom=src/bananaproto/plugin/main.py \\\n    --custom_opt=INCLUDE_GOOGLE \\\n    --custom_out=src/bananaproto/lib \\\n    -I /usr/local/include/ \\\n    /usr/local/include/google/protobuf/*.proto\n```\n\n### TODO\n\n- [x] Fixed length fields\n  - [x] Packed fixed-length\n- [x] Zig-zag signed fields (sint32, sint64)\n- [x] Don\'t encode zero values for nested types\n- [x] Enums\n- [x] Repeated message fields\n- [x] Maps\n  - [x] Maps of message fields\n- [x] Support passthrough of unknown fields\n- [x] Refs to nested types\n- [x] Imports in proto files\n- [x] Well-known Google types\n  - [ ] Support as request input\n  - [ ] Support as response output\n    - [ ] Automatically wrap/unwrap responses\n- [x] OneOf support\n  - [x] Basic support on the wire\n  - [x] Check which was set from the group\n  - [x] Setting one unsets the others\n- [ ] JSON that isn\'t completely naive.\n  - [x] 64-bit ints as strings\n  - [x] Maps\n  - [x] Lists\n  - [x] Bytes as base64\n  - [ ] Any support\n  - [x] Enum strings\n  - [x] Well known types support (timestamp, duration, wrappers)\n  - [x] Support different casing (orig vs. camel vs. others?)\n- [x] Async service stubs\n  - [x] Unary-unary\n  - [x] Server streaming response\n  - [x] Client streaming request\n- [x] Renaming messages and fields to conform to Python name standards\n- [x] Renaming clashes with language keywords\n- [x] Python package\n- [x] Automate running tests\n- [ ] Cleanup!\n\n### Banana TODO\n\n- [x] Fix input types imports\n- [x] Non-string type hint\n- [ ] Add *Reflections* chapter to README\n- [ ] Return original folder structure\n  - [ ] Automatically import *_pb2 for reflections\n- [x] Pass metadata to Service methods\n- [ ] Fix comments in generated code\n- [ ] Omit Empty argument from Stub and Service\n\n## License\n\nCopyright © 2019 Daniel G. Taylor\n\nhttp://dgt.mit-license.org/\n',
     'author': 'Daniel G. Taylor',
     'author_email': 'danielgtaylor@gmail.com',
     'maintainer': 'BananaLoaf',
     'maintainer_email': 'bananaloaf@protonmail.com',
     'url': 'https://github.com/BananaLoaf/python-bananaproto',
```

### Comparing `bananaproto-1.1.1/PKG-INFO` & `bananaproto-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bananaproto
-Version: 1.1.1
+Version: 1.1.2
 Summary: A BANANA Protobuf / gRPC generator & library
 Home-page: https://github.com/BananaLoaf/python-bananaproto
 License: MIT
 Keywords: protobuf,gRPC
 Author: Daniel G. Taylor
 Author-email: danielgtaylor@gmail.com
 Maintainer: BananaLoaf
```

