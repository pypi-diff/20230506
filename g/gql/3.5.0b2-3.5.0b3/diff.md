# Comparing `tmp/gql-3.5.0b2.tar.gz` & `tmp/gql-3.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gql-3.5.0b2.tar", last modified: Thu Feb 23 17:07:07 2023, max compression
+gzip compressed data, was "gql-3.5.0b3.tar", last modified: Thu Feb 23 22:06:15 2023, max compression
```

## Comparing `gql-3.5.0b2.tar` & `gql-3.5.0b3.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.374376 gql-3.5.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-23 17:07:01.000000 gql-3.5.0b2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-23 17:07:01.000000 gql-3.5.0b2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-02-23 17:07:01.000000 gql-3.5.0b2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-23 17:07:01.000000 gql-3.5.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-23 17:07:01.000000 gql-3.5.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-23 17:07:01.000000 gql-3.5.0b2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-02-23 17:07:07.374376 gql-3.5.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-23 17:07:01.000000 gql-3.5.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.358376 gql-3.5.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.358376 gql-3.5.0b2/docs/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/advanced/async_advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/advanced/async_permanent_session.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/advanced/dsl_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/advanced/error_handling.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/advanced/local_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/advanced/logging.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.358376 gql-3.5.0b2/docs/async/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/async/async_intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/async/async_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/async/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.362376 gql-3.5.0b2/docs/code_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/aiohttp_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/aiohttp_async_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/aiohttp_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.362376 gql-3.5.0b2/docs/code_examples/appsync/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/appsync/mutation_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/appsync/mutation_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/appsync/subscription_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/appsync/subscription_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/console_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/fastapi_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/httpx_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/phoenix_channel_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/reconnecting_mutation_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/reconnecting_mutation_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/reconnecting_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/requests_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/requests_sync_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/code_examples/websockets_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.362376 gql-3.5.0b2/docs/gql-cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/gql-cli/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.362376 gql-3.5.0b2/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/dsl.rst
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/gql.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_appsync_auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_appsync_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_httpx.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_phoenix_channel_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_requests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/transport_websockets_base.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/modules/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.362376 gql-3.5.0b2/docs/transports/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/appsync.rst
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/async_transports.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/httpx.rst
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/httpx_async.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/phoenix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/requests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/sync_transports.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/transports/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.362376 gql-3.5.0b2/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/custom_scalars_and_enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/file_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/headers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/subscriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-23 17:07:01.000000 gql-3.5.0b2/docs/usage/variables.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.366376 gql-3.5.0b2/gql/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    51693 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35952 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.366376 gql-3.5.0b2/gql/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/async_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/local_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/phoenix_channel_websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/transport/websockets_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.366376 gql-3.5.0b2/gql/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utilities/build_client_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utilities/get_introspection_query_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utilities/parse_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utilities/serialize_variable_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utilities/update_schema_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utilities/update_schema_scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-23 17:07:01.000000 gql-3.5.0b2/gql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.366376 gql-3.5.0b2/gql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-02-23 17:07:06.000000 gql-3.5.0b2/gql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-02-23 17:07:07.000000 gql-3.5.0b2/gql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:07:06.000000 gql-3.5.0b2/gql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-23 17:07:06.000000 gql-3.5.0b2/gql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:07:06.000000 gql-3.5.0b2/gql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-23 17:07:06.000000 gql-3.5.0b2/gql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-23 17:07:06.000000 gql-3.5.0b2/gql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-23 17:07:07.374376 gql-3.5.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-02-23 17:07:01.000000 gql-3.5.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.370376 gql-3.5.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.370376 gql-3.5.0b2/tests/custom_scalars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/custom_scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/custom_scalars/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/custom_scalars/test_enum_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/custom_scalars/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/custom_scalars/test_money.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/custom_scalars/test_parse_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.370376 gql-3.5.0b2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.370376 gql-3.5.0b2/tests/fixtures/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/aws/fake_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/aws/fake_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/aws/fake_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/aws/fake_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.370376 gql-3.5.0b2/tests/fixtures/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/graphql/sample.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.370376 gql-3.5.0b2/tests/fixtures/vcr_cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/vcr_cassettes/client.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    78820 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/fixtures/vcr_cassettes/queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.374376 gql-3.5.0b2/tests/nested_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/nested_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/nested_input/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/nested_input/test_nested_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:07.374376 gql-3.5.0b2/tests/starwars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22874 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/test_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/test_parse_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/starwars/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43147 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_aiohttp_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_appsync_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_async_client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_graphqlws_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_graphqlws_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_http_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)    38462 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_httpx_online.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_localhost.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_localhost.pem
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_phoenix_channel_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_phoenix_channel_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_phoenix_channel_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    26692 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_websocket_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_websocket_online.py
--rw-r--r--   0 runner    (1001) docker     (123)    17431 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_websocket_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-02-23 17:07:01.000000 gql-3.5.0b2/tests/test_websocket_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-02-23 17:07:01.000000 gql-3.5.0b2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-23 22:06:12.000000 gql-3.5.0b3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-23 22:06:12.000000 gql-3.5.0b3/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-02-23 22:06:12.000000 gql-3.5.0b3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-23 22:06:12.000000 gql-3.5.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-23 22:06:12.000000 gql-3.5.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-23 22:06:12.000000 gql-3.5.0b3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-02-23 22:06:15.198130 gql-3.5.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-23 22:06:12.000000 gql-3.5.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.182130 gql-3.5.0b3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.182130 gql-3.5.0b3/docs/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/async_advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/async_permanent_session.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/dsl_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/error_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/local_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/logging.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.182130 gql-3.5.0b3/docs/async/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/async/async_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/async/async_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/async/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/code_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/aiohttp_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/aiohttp_async_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/aiohttp_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/code_examples/appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/mutation_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/mutation_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/subscription_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/subscription_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/console_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/fastapi_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/httpx_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/phoenix_channel_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/reconnecting_mutation_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/reconnecting_mutation_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/reconnecting_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/requests_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/requests_sync_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/websockets_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/gql-cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/gql-cli/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/dsl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/gql.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_appsync_auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_appsync_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_phoenix_channel_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_requests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_websockets_base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/appsync.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/async_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/httpx_async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/phoenix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/requests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/sync_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/custom_scalars_and_enums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/file_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/headers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/subscriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/validation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/variables.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51634 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35952 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/gql/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/async_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/local_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/phoenix_channel_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/websockets_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.194130 gql-3.5.0b3/gql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/build_client_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/get_introspection_query_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/serialize_variable_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/update_schema_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/update_schema_scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/gql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-23 22:06:15.198130 gql-3.5.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-02-23 22:06:12.000000 gql-3.5.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.194130 gql-3.5.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/custom_scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_enum_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_parse_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/graphql/sample.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/vcr_cassettes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/vcr_cassettes/client.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    78820 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/vcr_cassettes/queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/nested_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/nested_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/nested_input/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/nested_input/test_nested_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/starwars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22874 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_parse_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43147 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_aiohttp_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_appsync_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_async_client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_graphqlws_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_graphqlws_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_http_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38462 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_httpx_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_localhost.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_localhost.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_phoenix_channel_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_phoenix_channel_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_phoenix_channel_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26692 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17431 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-02-23 22:06:12.000000 gql-3.5.0b3/tox.ini
```

### Comparing `gql-3.5.0b2/.readthedocs.yaml` & `gql-3.5.0b3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/CONTRIBUTING.md` & `gql-3.5.0b3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/LICENSE` & `gql-3.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/Makefile` & `gql-3.5.0b3/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/PKG-INFO` & `gql-3.5.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.5.0b2
+Version: 3.5.0b3
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
```

### Comparing `gql-3.5.0b2/README.md` & `gql-3.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/Makefile` & `gql-3.5.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/advanced/async_advanced_usage.rst` & `gql-3.5.0b3/docs/advanced/async_advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/advanced/async_permanent_session.rst` & `gql-3.5.0b3/docs/advanced/async_permanent_session.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/advanced/dsl_module.rst` & `gql-3.5.0b3/docs/advanced/dsl_module.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/advanced/error_handling.rst` & `gql-3.5.0b3/docs/advanced/error_handling.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/advanced/local_schema.rst` & `gql-3.5.0b3/docs/advanced/local_schema.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/advanced/logging.rst` & `gql-3.5.0b3/docs/advanced/logging.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/async/async_intro.rst` & `gql-3.5.0b3/docs/async/async_intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/async/async_usage.rst` & `gql-3.5.0b3/docs/async/async_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/aiohttp_async.py` & `gql-3.5.0b3/docs/code_examples/aiohttp_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/aiohttp_async_dsl.py` & `gql-3.5.0b3/docs/code_examples/aiohttp_async_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/aiohttp_sync.py` & `gql-3.5.0b3/docs/code_examples/aiohttp_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/appsync/mutation_api_key.py` & `gql-3.5.0b3/docs/code_examples/appsync/mutation_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/appsync/mutation_iam.py` & `gql-3.5.0b3/docs/code_examples/appsync/mutation_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/appsync/subscription_api_key.py` & `gql-3.5.0b3/docs/code_examples/appsync/subscription_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/appsync/subscription_iam.py` & `gql-3.5.0b3/docs/code_examples/appsync/subscription_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/console_async.py` & `gql-3.5.0b3/docs/code_examples/console_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/fastapi_async.py` & `gql-3.5.0b3/docs/code_examples/fastapi_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/httpx_async.py` & `gql-3.5.0b3/docs/code_examples/httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/phoenix_channel_async.py` & `gql-3.5.0b3/docs/code_examples/phoenix_channel_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/reconnecting_mutation_http.py` & `gql-3.5.0b3/docs/code_examples/reconnecting_mutation_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/reconnecting_mutation_ws.py` & `gql-3.5.0b3/docs/code_examples/reconnecting_mutation_ws.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/reconnecting_subscription.py` & `gql-3.5.0b3/docs/code_examples/reconnecting_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/requests_sync_dsl.py` & `gql-3.5.0b3/docs/code_examples/requests_sync_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/code_examples/websockets_async.py` & `gql-3.5.0b3/docs/code_examples/websockets_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/conf.py` & `gql-3.5.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/gql-cli/intro.rst` & `gql-3.5.0b3/docs/gql-cli/intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/intro.rst` & `gql-3.5.0b3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/make.bat` & `gql-3.5.0b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/transports/aiohttp.rst` & `gql-3.5.0b3/docs/transports/aiohttp.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/transports/appsync.rst` & `gql-3.5.0b3/docs/transports/appsync.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/transports/httpx_async.rst` & `gql-3.5.0b3/docs/transports/httpx_async.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/transports/phoenix.rst` & `gql-3.5.0b3/docs/transports/phoenix.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/transports/websockets.rst` & `gql-3.5.0b3/docs/transports/websockets.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/usage/basic_usage.rst` & `gql-3.5.0b3/docs/usage/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/usage/custom_scalars_and_enums.rst` & `gql-3.5.0b3/docs/usage/custom_scalars_and_enums.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/usage/extensions.rst` & `gql-3.5.0b3/docs/usage/extensions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/usage/file_upload.rst` & `gql-3.5.0b3/docs/usage/file_upload.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/usage/subscriptions.rst` & `gql-3.5.0b3/docs/usage/subscriptions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/usage/validation.rst` & `gql-3.5.0b3/docs/usage/validation.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/docs/usage/variables.rst` & `gql-3.5.0b3/docs/usage/variables.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/cli.py` & `gql-3.5.0b3/gql/cli.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/client.py` & `gql-3.5.0b3/gql/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,23 +589,22 @@
                     generator_task
                 )  # type: ignore
                 yield result
 
         except StopAsyncIteration:
             pass
 
-        except (KeyboardInterrupt, Exception):
+        except (KeyboardInterrupt, Exception, GeneratorExit):
+
+            # Graceful shutdown
+            asyncio.ensure_future(async_generator.aclose(), loop=loop)
 
-            # Graceful shutdown by cancelling the task and waiting clean shutdown
             generator_task.cancel()
 
-            try:
-                loop.run_until_complete(generator_task)
-            except (StopAsyncIteration, asyncio.CancelledError):
-                pass
+            loop.run_until_complete(loop.shutdown_asyncgens())
 
             # Then reraise the exception
             raise
 
     async def connect_async(self, reconnecting=False, **kwargs):
         r"""Connect asynchronously with the underlying async transport to
         produce a session.
```

### Comparing `gql-3.5.0b2/gql/dsl.py` & `gql-3.5.0b3/gql/dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/gql.py` & `gql-3.5.0b3/gql/gql.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/aiohttp.py` & `gql-3.5.0b3/gql/transport/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/appsync_auth.py` & `gql-3.5.0b3/gql/transport/appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/appsync_websockets.py` & `gql-3.5.0b3/gql/transport/appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/async_transport.py` & `gql-3.5.0b3/gql/transport/async_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/exceptions.py` & `gql-3.5.0b3/gql/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/httpx.py` & `gql-3.5.0b3/gql/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/local_schema.py` & `gql-3.5.0b3/gql/transport/local_schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/phoenix_channel_websockets.py` & `gql-3.5.0b3/gql/transport/phoenix_channel_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/requests.py` & `gql-3.5.0b3/gql/transport/requests.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/transport.py` & `gql-3.5.0b3/gql/transport/transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/websockets.py` & `gql-3.5.0b3/gql/transport/websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/transport/websockets_base.py` & `gql-3.5.0b3/gql/transport/websockets_base.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utilities/__init__.py` & `gql-3.5.0b3/gql/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utilities/build_client_schema.py` & `gql-3.5.0b3/gql/utilities/build_client_schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utilities/get_introspection_query_ast.py` & `gql-3.5.0b3/gql/utilities/get_introspection_query_ast.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utilities/parse_result.py` & `gql-3.5.0b3/gql/utilities/parse_result.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utilities/serialize_variable_values.py` & `gql-3.5.0b3/gql/utilities/serialize_variable_values.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utilities/update_schema_enum.py` & `gql-3.5.0b3/gql/utilities/update_schema_enum.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utilities/update_schema_scalars.py` & `gql-3.5.0b3/gql/utilities/update_schema_scalars.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql/utils.py` & `gql-3.5.0b3/gql/utils.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql.egg-info/PKG-INFO` & `gql-3.5.0b3/gql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.5.0b2
+Version: 3.5.0b3
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
```

### Comparing `gql-3.5.0b2/gql.egg-info/SOURCES.txt` & `gql-3.5.0b3/gql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/gql.egg-info/requires.txt` & `gql-3.5.0b3/gql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/setup.py` & `gql-3.5.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/conftest.py` & `gql-3.5.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/custom_scalars/test_datetime.py` & `gql-3.5.0b3/tests/custom_scalars/test_datetime.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/custom_scalars/test_enum_colors.py` & `gql-3.5.0b3/tests/custom_scalars/test_enum_colors.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/custom_scalars/test_json.py` & `gql-3.5.0b3/tests/custom_scalars/test_json.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/custom_scalars/test_money.py` & `gql-3.5.0b3/tests/custom_scalars/test_money.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/custom_scalars/test_parse_results.py` & `gql-3.5.0b3/tests/custom_scalars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/fixtures/aws/fake_credentials.py` & `gql-3.5.0b3/tests/fixtures/aws/fake_credentials.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/fixtures/aws/fake_request.py` & `gql-3.5.0b3/tests/fixtures/aws/fake_request.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/fixtures/aws/fake_session.py` & `gql-3.5.0b3/tests/fixtures/aws/fake_session.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/fixtures/aws/fake_signer.py` & `gql-3.5.0b3/tests/fixtures/aws/fake_signer.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/fixtures/vcr_cassettes/client.yaml` & `gql-3.5.0b3/tests/fixtures/vcr_cassettes/client.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/fixtures/vcr_cassettes/queries.yaml` & `gql-3.5.0b3/tests/fixtures/vcr_cassettes/queries.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/nested_input/schema.py` & `gql-3.5.0b3/tests/nested_input/schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/nested_input/test_nested_input.py` & `gql-3.5.0b3/tests/nested_input/test_nested_input.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/starwars/fixtures.py` & `gql-3.5.0b3/tests/starwars/fixtures.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/starwars/schema.py` & `gql-3.5.0b3/tests/starwars/schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/starwars/test_dsl.py` & `gql-3.5.0b3/tests/starwars/test_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/starwars/test_parse_results.py` & `gql-3.5.0b3/tests/starwars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/starwars/test_query.py` & `gql-3.5.0b3/tests/starwars/test_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/starwars/test_subscription.py` & `gql-3.5.0b3/tests/starwars/test_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/starwars/test_validation.py` & `gql-3.5.0b3/tests/starwars/test_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_aiohttp.py` & `gql-3.5.0b3/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_aiohttp_online.py` & `gql-3.5.0b3/tests/test_aiohttp_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_appsync_auth.py` & `gql-3.5.0b3/tests/test_appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_appsync_http.py` & `gql-3.5.0b3/tests/test_appsync_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_appsync_websockets.py` & `gql-3.5.0b3/tests/test_appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_async_client_validation.py` & `gql-3.5.0b3/tests/test_async_client_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_cli.py` & `gql-3.5.0b3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_client.py` & `gql-3.5.0b3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_graphqlws_exceptions.py` & `gql-3.5.0b3/tests/test_graphqlws_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_graphqlws_subscription.py` & `gql-3.5.0b3/tests/test_graphqlws_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_http_async_sync.py` & `gql-3.5.0b3/tests/test_http_async_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_httpx.py` & `gql-3.5.0b3/tests/test_httpx.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_httpx_async.py` & `gql-3.5.0b3/tests/test_httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_httpx_online.py` & `gql-3.5.0b3/tests/test_httpx_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_localhost.pem` & `gql-3.5.0b3/tests/test_localhost.pem`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_phoenix_channel_exceptions.py` & `gql-3.5.0b3/tests/test_phoenix_channel_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_phoenix_channel_query.py` & `gql-3.5.0b3/tests/test_phoenix_channel_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_phoenix_channel_subscription.py` & `gql-3.5.0b3/tests/test_phoenix_channel_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_requests.py` & `gql-3.5.0b3/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_transport.py` & `gql-3.5.0b3/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_websocket_exceptions.py` & `gql-3.5.0b3/tests/test_websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_websocket_online.py` & `gql-3.5.0b3/tests/test_websocket_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_websocket_query.py` & `gql-3.5.0b3/tests/test_websocket_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b2/tests/test_websocket_subscription.py` & `gql-3.5.0b3/tests/test_websocket_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,14 +490,74 @@
 
         assert number == count
         count -= 1
 
     assert count == -1
 
 
+@pytest.mark.parametrize("server", [server_countdown], indirect=True)
+@pytest.mark.parametrize("subscription_str", [countdown_subscription_str])
+def test_websocket_subscription_sync_user_exception(server, subscription_str):
+    from gql.transport.websockets import WebsocketsTransport
+
+    url = f"ws://{server.hostname}:{server.port}/graphql"
+    print(f"url = {url}")
+
+    sample_transport = WebsocketsTransport(url=url)
+
+    client = Client(transport=sample_transport)
+
+    count = 10
+    subscription = gql(subscription_str.format(count=count))
+
+    with pytest.raises(Exception) as exc_info:
+        for result in client.subscribe(subscription):
+
+            number = result["number"]
+            print(f"Number received: {number}")
+
+            assert number == count
+            count -= 1
+
+            if count == 5:
+                raise Exception("This is an user exception")
+
+    assert count == 5
+    assert "This is an user exception" in str(exc_info.value)
+
+
+@pytest.mark.parametrize("server", [server_countdown], indirect=True)
+@pytest.mark.parametrize("subscription_str", [countdown_subscription_str])
+def test_websocket_subscription_sync_break(server, subscription_str):
+    from gql.transport.websockets import WebsocketsTransport
+
+    url = f"ws://{server.hostname}:{server.port}/graphql"
+    print(f"url = {url}")
+
+    sample_transport = WebsocketsTransport(url=url)
+
+    client = Client(transport=sample_transport)
+
+    count = 10
+    subscription = gql(subscription_str.format(count=count))
+
+    for result in client.subscribe(subscription):
+
+        number = result["number"]
+        print(f"Number received: {number}")
+
+        assert number == count
+        count -= 1
+
+        if count == 5:
+            break
+
+    assert count == 5
+
+
 @pytest.mark.skipif(sys.platform.startswith("win"), reason="test failing on windows")
 @pytest.mark.parametrize("server", [server_countdown], indirect=True)
 @pytest.mark.parametrize("subscription_str", [countdown_subscription_str])
 def test_websocket_subscription_sync_graceful_shutdown(server, subscription_str):
     """Note: this test will simulate a control-C happening while a sync subscription
     is in progress. To do that we will throw a KeyboardInterrupt exception inside
     the subscription async generator.
```

### Comparing `gql-3.5.0b2/tox.ini` & `gql-3.5.0b3/tox.ini`

 * *Files identical despite different names*

