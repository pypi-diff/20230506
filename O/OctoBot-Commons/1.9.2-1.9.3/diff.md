# Comparing `tmp/OctoBot-Commons-1.9.2.tar.gz` & `tmp/OctoBot-Commons-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Commons-1.9.2.tar", last modified: Tue May  2 17:19:48 2023, max compression
+gzip compressed data, was "OctoBot-Commons-1.9.3.tar", last modified: Fri May  5 22:05:56 2023, max compression
```

## Comparing `OctoBot-Commons-1.9.2.tar` & `OctoBot-Commons-1.9.3.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.344442 OctoBot-Commons-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.320441 OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-02 17:19:48.000000 OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-02 17:19:48.000000 OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:19:48.000000 OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:19:48.000000 OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-02 17:19:48.000000 OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 17:19:48.000000 OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-02 17:19:48.344442 OctoBot-Commons-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.324442 OctoBot-Commons-1.9.2/octobot_commons/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/aiohttp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/async_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/asyncio_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/channels_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.328441 OctoBot-Commons-1.9.2/octobot_commons/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/configuration/config_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/configuration/config_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/configuration/fields_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/configuration/user_input_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/configuration/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/data_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.328441 OctoBot-Commons-1.9.2/octobot_commons/databases/
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.328441 OctoBot-Commons-1.9.2/octobot_commons/databases/bases/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/bases/base_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/bases/document_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/cache_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.328441 OctoBot-Commons-1.9.2/octobot_commons/databases/database_caches/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/database_caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/database_caches/chronological_read_database_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/database_caches/generic_database_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.328441 OctoBot-Commons-1.9.2/octobot_commons/databases/databases_util/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/databases_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/databases_util/cache_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.328441 OctoBot-Commons-1.9.2/octobot_commons/databases/document_database_adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/document_database_adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.328441 OctoBot-Commons-1.9.2/octobot_commons/databases/global_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/global_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/global_storage/global_shared_memory_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.332441 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/_exchange_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/cache_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/cache_timestamp_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/db_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/db_writer_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/meta_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.332441 OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.332441 OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.332441 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/run_databases_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/run_databases_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/run_databases_pruning_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/dict_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.332441 OctoBot-Commons-1.9.2/octobot_commons/display/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/display/display_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/display/display_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/display/plot_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/evaluators_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/external_resources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.332441 OctoBot-Commons-1.9.2/octobot_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/logging/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/logical_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/multiprocessing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/number_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/optimization_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/os_clock_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/pretty_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.332441 OctoBot-Commons-1.9.2/octobot_commons/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/profiles/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/profiles/profile_sharing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.336442 OctoBot-Commons-1.9.2/octobot_commons/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/signal_builder_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/signal_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/signal_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/signal_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/signals/signals_emitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.336442 OctoBot-Commons-1.9.2/octobot_commons/singleton/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/singleton/singleton_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.336442 OctoBot-Commons-1.9.2/octobot_commons/symbols/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/symbols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/symbols/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/symbols/symbol_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/system_resources_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.336442 OctoBot-Commons-1.9.2/octobot_commons/tentacles_management/
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tentacles_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tentacles_management/abstract_tentacle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tentacles_management/class_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.336442 OctoBot-Commons-1.9.2/octobot_commons/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/thread_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/time_frame_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/timestamp_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.336442 OctoBot-Commons-1.9.2/octobot_commons/tree/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tree/base_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tree/event_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/octobot_commons/tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:19:48.344442 OctoBot-Commons-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.320441 OctoBot-Commons-1.9.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/configuration/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/configuration/test_fields_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/databases/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/databases/global_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/global_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/global_storage/test_global_shared_memory_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/databases/relational_databases/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/relational_databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/databases/relational_databases/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/relational_databases/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/relational_databases/sqlite/test_sqlite_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/databases/run_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/run_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/databases/run_databases/test_run_databases_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/logging/test_logging_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16320 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/profiles/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/profiles/test_profile_sharing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.340442 OctoBot-Commons-1.9.2/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/signals/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/signals/test_signal_builder_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/signals/test_signal_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/signals/test_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/signals/test_signal_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/signals/test_signal_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.344442 OctoBot-Commons-1.9.2/tests/symbols/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/symbols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/symbols/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/symbols/test_symbol_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.344442 OctoBot-Commons-1.9.2/tests/tentacles_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/tentacles_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/tentacles_management/test_abstract_tentacle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/tentacles_management/test_class_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:48.344442 OctoBot-Commons-1.9.2/tests/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/tree/test_base_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-02 17:19:07.000000 OctoBot-Commons-1.9.2/tests/tree/test_event_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    19192 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.208658 OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 22:05:56.000000 OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-05 22:05:56.000000 OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:05:56.000000 OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:05:56.000000 OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 22:05:56.000000 OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 22:05:56.000000 OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/aiohttp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/async_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/asyncio_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/channels_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/configuration/config_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/configuration/config_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/configuration/fields_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/configuration/user_input_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/configuration/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/data_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/databases/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/bases/base_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/bases/document_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/cache_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/databases/database_caches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/database_caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/database_caches/chronological_read_database_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/database_caches/generic_database_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/databases/databases_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/databases_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/databases_util/cache_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/databases/document_database_adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/document_database_adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.212658 OctoBot-Commons-1.9.3/octobot_commons/databases/global_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/global_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/global_storage/global_shared_memory_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/_exchange_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/cache_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/cache_timestamp_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/db_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/db_writer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/meta_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/run_databases_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/run_databases_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/run_databases_pruning_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/dict_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/display/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/display/display_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/display/display_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/display/plot_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/evaluators_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/external_resources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/logging/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/logical_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/multiprocessing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/number_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/optimization_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/os_clock_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/pretty_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/profiles/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/profiles/profile_sharing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/signal_builder_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/signal_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/signal_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/signal_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/signals/signals_emitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/singleton/singleton_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/symbols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/symbols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/symbols/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/symbols/symbol_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/system_resources_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/tentacles_management/
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tentacles_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tentacles_management/abstract_tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tentacles_management/class_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/thread_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/time_frame_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/timestamp_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/octobot_commons/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tree/base_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tree/event_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/octobot_commons/tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.208658 OctoBot-Commons-1.9.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/configuration/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/configuration/test_fields_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.216658 OctoBot-Commons-1.9.3/tests/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/databases/global_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/global_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/global_storage/test_global_shared_memory_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/databases/relational_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/relational_databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/databases/relational_databases/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/relational_databases/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/relational_databases/sqlite/test_sqlite_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/databases/run_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/run_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/databases/run_databases/test_run_databases_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/logging/test_logging_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16320 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/profiles/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/profiles/test_profile_sharing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/signals/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/signals/test_signal_builder_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/signals/test_signal_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/signals/test_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/signals/test_signal_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/signals/test_signal_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/symbols/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/symbols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/symbols/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/symbols/test_symbol_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/tentacles_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/tentacles_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/tentacles_management/test_abstract_tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/tentacles_management/test_class_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:56.220658 OctoBot-Commons-1.9.3/tests/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/tree/test_base_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-05 22:05:27.000000 OctoBot-Commons-1.9.3/tests/tree/test_event_tree.py
```

### Comparing `OctoBot-Commons-1.9.2/CHANGELOG.md` & `OctoBot-Commons-1.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.9.3] - 2023-05-05
+### Fixed
+- make archive path
+
 ## [1.9.2] - 2023-05-02
 ### Updated
 - setup.py
 
 ## [1.9.1] - 2023-05-02
 ### Updated
 - setup.py
```

### Comparing `OctoBot-Commons-1.9.2/LICENSE` & `OctoBot-Commons-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/PKG-INFO` & `OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Commons
-Version: 1.9.2
+Version: 1.9.3
 Summary: OctoBot project common modules
 Home-page: https://github.com/Drakkar-Software/OctoBot-Commons
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Commons [1.9.2](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
+# OctoBot-Commons [1.9.3](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `OctoBot-Commons-1.9.2/OctoBot_Commons.egg-info/SOURCES.txt` & `OctoBot-Commons-1.9.3/OctoBot_Commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/PKG-INFO` & `OctoBot-Commons-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Commons
-Version: 1.9.2
+Version: 1.9.3
 Summary: OctoBot project common modules
 Home-page: https://github.com/Drakkar-Software/OctoBot-Commons
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Commons [1.9.2](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
+# OctoBot-Commons [1.9.3](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `OctoBot-Commons-1.9.2/README.md` & `OctoBot-Commons-1.9.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Commons [1.9.2](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
+# OctoBot-Commons [1.9.3](https://github.com/Drakkar-Software/OctoBot-Commons/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b31f3ab3511744a5a5ca6b9bb48e77bb)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Commons?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Commons&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Commons.svg)](https://pypi.python.org/pypi/OctoBot-Commons/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Commons/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Commons?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Commons/workflows/Github-Action-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Commons/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Commons/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Commons)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Commons"
-VERSION = "1.9.2"  # major.minor.revision
+VERSION = "1.9.3"  # major.minor.revision
 
 MARKET_SEPARATOR = "/"
 SETTLEMENT_ASSET_SEPARATOR = ":"
 DICT_BULLET_TOKEN_STR = "\n "
 
 OCTOBOT_KEY = b"uVEw_JJe7uiXepaU_DR4T-ThkjZlDn8Pzl8hYPIv7w0="  # TODO temp
```

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/aiohttp_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/aiohttp_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/async_job.py` & `OctoBot-Commons-1.9.3/octobot_commons/async_job.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/asyncio_tools.py` & `OctoBot-Commons-1.9.3/octobot_commons/asyncio_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/authentication.py` & `OctoBot-Commons-1.9.3/octobot_commons/authentication.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/channels_name.py` & `OctoBot-Commons-1.9.3/octobot_commons/channels_name.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/configuration/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/configuration/config_file_manager.py` & `OctoBot-Commons-1.9.3/octobot_commons/configuration/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/configuration/config_operations.py` & `OctoBot-Commons-1.9.3/octobot_commons/configuration/config_operations.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/configuration/configuration.py` & `OctoBot-Commons-1.9.3/octobot_commons/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/configuration/fields_utils.py` & `OctoBot-Commons-1.9.3/octobot_commons/configuration/fields_utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/configuration/user_input_configuration.py` & `OctoBot-Commons-1.9.3/octobot_commons/configuration/user_input_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/configuration/user_inputs.py` & `OctoBot-Commons-1.9.3/octobot_commons/configuration/user_inputs.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/constants.py` & `OctoBot-Commons-1.9.3/octobot_commons/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/data_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/data_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/bases/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/bases/base_database.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/bases/base_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/bases/document_database.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/bases/document_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/cache_client.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/cache_client.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/cache_manager.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/cache_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/database_caches/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/database_caches/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/database_caches/chronological_read_database_cache.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/database_caches/chronological_read_database_cache.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/database_caches/generic_database_cache.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/database_caches/generic_database_cache.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/databases_util/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/databases_util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/databases_util/cache_wrapper.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/databases_util/cache_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/document_database_adaptors/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/document_database_adaptors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/document_database_adaptors/abstract_document_database_adaptor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/document_database_adaptors/tinydb_adaptor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/global_storage/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/global_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/global_storage/global_shared_memory_storage.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/global_storage/global_shared_memory_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/_exchange_database.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/_exchange_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/cache_database.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/cache_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/cache_timestamp_database.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/cache_timestamp_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/db_reader.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/db_reader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/db_writer.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/db_writer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/db_writer_reader.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/db_writer_reader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/implementations/meta_database.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/implementations/meta_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/cursor_pool.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/cursor_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/relational_databases/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/abstract_run_databases_pruner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/file_system_run_databases_pruner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/run_databases_identifier.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/run_databases_identifier.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/run_databases_provider.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/run_databases_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/run_databases_pruning_factory.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/run_databases_pruning_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/storage.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/databases/run_databases/utils.py` & `OctoBot-Commons-1.9.3/octobot_commons/databases/run_databases/utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/dict_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/dict_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/display/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/display/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/display/display_factory.py` & `OctoBot-Commons-1.9.3/octobot_commons/display/display_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/display/display_translator.py` & `OctoBot-Commons-1.9.3/octobot_commons/display/display_translator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/display/plot_settings.py` & `OctoBot-Commons-1.9.3/octobot_commons/display/plot_settings.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/enums.py` & `OctoBot-Commons-1.9.3/octobot_commons/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/errors.py` & `OctoBot-Commons-1.9.3/octobot_commons/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/evaluators_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/evaluators_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/external_resources_manager.py` & `OctoBot-Commons-1.9.3/octobot_commons/external_resources_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/json_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/json_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/list_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/list_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/logging/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/logging/logging_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/logical_operators.py` & `OctoBot-Commons-1.9.3/octobot_commons/logical_operators.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/multiprocessing_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/multiprocessing_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/number_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/number_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/optimization_campaign.py` & `OctoBot-Commons-1.9.3/octobot_commons/optimization_campaign.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/os_clock_sync.py` & `OctoBot-Commons-1.9.3/octobot_commons/os_clock_sync.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/os_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/os_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/pretty_printer.py` & `OctoBot-Commons-1.9.3/octobot_commons/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/profiles/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/profiles/profile.py` & `OctoBot-Commons-1.9.3/octobot_commons/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/profiles/profile_sharing.py` & `OctoBot-Commons-1.9.3/octobot_commons/profiles/profile_sharing.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     if os.path.isfile(export_path_with_ext):
         os.remove(export_path_with_ext)
     # copy profile into a temp dir to edit it
     shutil.copytree(profile.path, temp_path)
     try:
         _filter_profile_export(temp_path)
         # export the edited profile
-        shutil.make_archive(export_path, constants.PROFILE_EXPORT_FORMAT, temp_path)
+        shutil.make_archive(
+            os.path.abspath(export_path), constants.PROFILE_EXPORT_FORMAT, temp_path
+        )
     finally:
         shutil.rmtree(temp_path)
     return export_path_with_ext
 
 
 def install_profile(
     import_path: str,
```

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/signal.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/signal_builder_wrapper.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/signal_builder_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/signal_bundle.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/signal_bundle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/signal_bundle_builder.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/signal_factory.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/signal_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/signal_publisher.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/signal_publisher.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/signals/signals_emitter.py` & `OctoBot-Commons-1.9.3/octobot_commons/signals/signals_emitter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/singleton/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/singleton/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/singleton/singleton_class.py` & `OctoBot-Commons-1.9.3/octobot_commons/singleton/singleton_class.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/support.py` & `OctoBot-Commons-1.9.3/octobot_commons/support.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/symbols/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/symbols/symbol.py` & `OctoBot-Commons-1.9.3/octobot_commons/symbols/symbol.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/symbols/symbol_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/symbols/symbol_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/system_resources_watcher.py` & `OctoBot-Commons-1.9.3/octobot_commons/system_resources_watcher.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tentacles_management/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/tentacles_management/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tentacles_management/abstract_tentacle.py` & `OctoBot-Commons-1.9.3/octobot_commons/tentacles_management/abstract_tentacle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tentacles_management/class_inspector.py` & `OctoBot-Commons-1.9.3/octobot_commons/tentacles_management/class_inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tests/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tests/test_config.py` & `OctoBot-Commons-1.9.3/octobot_commons/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/thread_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/thread_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/time_frame_manager.py` & `OctoBot-Commons-1.9.3/octobot_commons/time_frame_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/timestamp_util.py` & `OctoBot-Commons-1.9.3/octobot_commons/timestamp_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tree/__init__.py` & `OctoBot-Commons-1.9.3/octobot_commons/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tree/base_tree.py` & `OctoBot-Commons-1.9.3/octobot_commons/tree/base_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tree/event_provider.py` & `OctoBot-Commons-1.9.3/octobot_commons/tree/event_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/octobot_commons/tree/event_tree.py` & `OctoBot-Commons-1.9.3/octobot_commons/tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/setup.py` & `OctoBot-Commons-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/configuration/__init__.py` & `OctoBot-Commons-1.9.3/tests/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/configuration/test_configuration.py` & `OctoBot-Commons-1.9.3/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/configuration/test_fields_util.py` & `OctoBot-Commons-1.9.3/tests/configuration/test_fields_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/databases/global_storage/test_global_shared_memory_storage.py` & `OctoBot-Commons-1.9.3/tests/databases/global_storage/test_global_shared_memory_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/databases/relational_databases/sqlite/test_sqlite_database.py` & `OctoBot-Commons-1.9.3/tests/databases/relational_databases/sqlite/test_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/databases/run_databases/test_run_databases_provider.py` & `OctoBot-Commons-1.9.3/tests/databases/run_databases/test_run_databases_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/logging/test_logging_util.py` & `OctoBot-Commons-1.9.3/tests/logging/test_logging_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/profiles/__init__.py` & `OctoBot-Commons-1.9.3/tests/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/profiles/test_profile.py` & `OctoBot-Commons-1.9.3/tests/profiles/test_profile.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/profiles/test_profile_sharing.py` & `OctoBot-Commons-1.9.3/tests/profiles/test_profile_sharing.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/signals/__init__.py` & `OctoBot-Commons-1.9.3/tests/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/signals/test_signal.py` & `OctoBot-Commons-1.9.3/tests/signals/test_signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/signals/test_signal_builder_wrapper.py` & `OctoBot-Commons-1.9.3/tests/signals/test_signal_builder_wrapper.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/signals/test_signal_bundle.py` & `OctoBot-Commons-1.9.3/tests/signals/test_signal_bundle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/signals/test_signal_bundle_builder.py` & `OctoBot-Commons-1.9.3/tests/signals/test_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/signals/test_signal_factory.py` & `OctoBot-Commons-1.9.3/tests/signals/test_signal_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/signals/test_signal_publisher.py` & `OctoBot-Commons-1.9.3/tests/signals/test_signal_publisher.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/symbols/test_symbol.py` & `OctoBot-Commons-1.9.3/tests/symbols/test_symbol.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/symbols/test_symbol_util.py` & `OctoBot-Commons-1.9.3/tests/symbols/test_symbol_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/tentacles_management/test_abstract_tentacle.py` & `OctoBot-Commons-1.9.3/tests/tentacles_management/test_abstract_tentacle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/tentacles_management/test_class_inspector.py` & `OctoBot-Commons-1.9.3/tests/tentacles_management/test_class_inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/tree/test_base_tree.py` & `OctoBot-Commons-1.9.3/tests/tree/test_base_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Commons-1.9.2/tests/tree/test_event_tree.py` & `OctoBot-Commons-1.9.3/tests/tree/test_event_tree.py`

 * *Files identical despite different names*

