# Comparing `tmp/OctoBot-Tentacles-Manager-2.9.0.tar.gz` & `tmp/OctoBot-Tentacles-Manager-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Tentacles-Manager-2.9.0.tar", last modified: Tue May  2 20:03:10 2023, max compression
+gzip compressed data, was "OctoBot-Tentacles-Manager-2.9.1.tar", last modified: Fri May  5 22:07:26 2023, max compression
```

## Comparing `OctoBot-Tentacles-Manager-2.9.0.tar` & `OctoBot-Tentacles-Manager-2.9.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 20:03:10.000000 OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/tentacles_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/compiled_package_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.541178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Mode_config.template
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Social_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Strategies_config.template
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/TA_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Util_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/description_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/artifact_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/profiles_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/artifact_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/metadata_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/profile_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_requirements_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/s3_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.545178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/repair_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/single_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/tentacles_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/update_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.537178 OctoBot-Tentacles-Manager-2.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/api/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacles_setup_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/exporters/test_tentacle_bundle_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/loaders/test_tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/managers/test_tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/util/test_tentacle_fetching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/tests/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_update_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:03:10.549178 OctoBot-Tentacles-Manager-2.9.0/upload_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/upload_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/upload_tests/_test_nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-02 20:02:24.000000 OctoBot-Tentacles-Manager-2.9.0/upload_tests/test_s3_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.731238 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-05 22:07:26.000000 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-05 22:07:26.000000 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:07:26.000000 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 22:07:26.000000 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:07:26.000000 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-05 22:07:26.000000 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 22:07:26.000000 OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.731238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/util/tentacles_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22458 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/compiled_package_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Mode_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Social_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Strategies_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/TA_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Util_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/description_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/artifact_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/tentacle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/loaders/tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.735238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/profiles_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/tentacle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.739238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.739238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/artifact_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/metadata_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/profile_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_requirements_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.739238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/s3_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.739238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.739238 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/repair_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/single_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/tentacles_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/update_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.731238 OctoBot-Tentacles-Manager-2.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.739238 OctoBot-Tentacles-Manager-2.9.1/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/api/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/api/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/api/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/api/test_tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/api/test_uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/api/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.739238 OctoBot-Tentacles-Manager-2.9.1/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/configuration/test_tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/configuration/test_tentacles_setup_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/tests/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/exporters/test_tentacle_bundle_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/loaders/test_tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/managers/test_tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/util/test_tentacle_fetching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/tests/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/workers/test_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/workers/test_uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/tests/workers/test_update_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:07:26.743238 OctoBot-Tentacles-Manager-2.9.1/upload_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/upload_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/upload_tests/_test_nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-05 22:06:46.000000 OctoBot-Tentacles-Manager-2.9.1/upload_tests/test_s3_uploader.py
```

### Comparing `OctoBot-Tentacles-Manager-2.9.0/CHANGELOG.md` & `OctoBot-Tentacles-Manager-2.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.9.1] - 2023-05-05
+### Fixed
+- Disable tentacles error
+
 ## [2.9.0] - 2023-05-02
 ### Updated
 - Supported python versions
 
 ## [2.8.6] - 2022-04-15
 ### Added
 - [API] add deactivate_all
```

### Comparing `OctoBot-Tentacles-Manager-2.9.0/LICENSE` & `OctoBot-Tentacles-Manager-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.9.0
+Version: 2.9.1
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
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
 
-# OctoBot-Tentacles-Manager [2.9.0](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.1](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.0/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt` & `OctoBot-Tentacles-Manager-2.9.1/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/PKG-INFO` & `OctoBot-Tentacles-Manager-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Tentacles-Manager
-Version: 2.9.0
+Version: 2.9.1
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
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
 
-# OctoBot-Tentacles-Manager [2.9.0](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.1](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.0/README.md` & `OctoBot-Tentacles-Manager-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Tentacles-Manager [2.9.0](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.9.1](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-VERSION = "2.9.0"
+VERSION = "2.9.1"
 PROJECT_NAME = "OctoBot-Tentacles-Manager"
```

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/configurator.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/creator.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/inspector.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/installer.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/loader.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/loader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/updater.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/uploader.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/api/util/tentacles_management.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/api/util/tentacles_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/cli.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/config_file.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/config_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,18 +148,22 @@
             constants.TENTACLES_EVALUATOR_TA_PATH,
             constants.TENTACLES_EVALUATOR_SOCIAL_PATH,
             constants.TENTACLES_EVALUATOR_REALTIME_PATH,
             constants.TENTACLES_EVALUATOR_SCRIPTED_PATH
         ] if evaluators else []
         for element_type, element_names in self.tentacles_activation.items():
             for element_name in element_names:
-                if loaders.get_tentacle_classes()[element_name].get_simple_tentacle_type() \
-                        in to_deactivate_tentacles_types and self.tentacles_activation[element_type][element_name]:
-                    self.logger.info(f"Tentacles configuration updated: {element_name} {'deactivated'}")
-                    self.tentacles_activation[element_type][element_name] = False
+                try:
+                    if loaders.get_tentacle_classes()[element_name].get_simple_tentacle_type() \
+                            in to_deactivate_tentacles_types and self.tentacles_activation[element_type][element_name]:
+                        self.logger.info(f"Tentacles configuration updated: {element_name} {'deactivated'}")
+                        self.tentacles_activation[element_type][element_name] = False
+                except KeyError:
+                    # do not crash on missing tentacles
+                    pass
 
     def _deactivate_other_evaluators(self, new_config):
         something_changed = False
         for element_type, element_names in self.tentacles_activation.items():
             for element_name in element_names:
                 # for each activated element that is not in new_config
                 if element_name not in new_config and self.tentacles_activation[element_type][element_name]:
```

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/constants.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/compiled_package_manager.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/compiled_package_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Mode_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Mode_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/templates/Social_tentacle.template` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/templates/Social_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/creators/tentacle_creator.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/creators/tentacle_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/enums.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/artifact_exporter.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/artifact_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/tentacle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/exporters/tentacle_package_exporter.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/exporters/tentacle_package_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/loaders/tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/loaders/tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/profiles_manager.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/profiles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/python_modules_requirements_manager.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/python_modules_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacle_manager.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/tentacle_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_init_files_manager.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/tentacles_init_files_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/managers/tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/managers/tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/artifact.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/artifact.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/artifact_metadata.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/artifact_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/metadata_factory.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/metadata_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/profile_metadata.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/profile_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_metadata.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/tentacle_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/profile.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/profile.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_factory.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_package.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_package.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_requirements_tree.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_requirements_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/models/tentacle_type.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/models/tentacle_type.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/uploaders/uploader.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/uploaders/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/file_util.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/file_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/hashing.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/hashing.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/os_util.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/os_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_cleaner.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_cleaner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_explorer.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_explorer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/util/tentacle_filter.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/util/tentacle_filter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/install_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/repair_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/repair_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/single_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/single_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/tentacles_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/tentacles_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/octobot_tentacles_manager/workers/update_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/octobot_tentacles_manager/workers/update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/setup.py` & `OctoBot-Tentacles-Manager-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/api/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_configurator.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/api/test_configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_creator.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/api/test_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_installer.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/api/test_installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_uninstaller.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/api/test_uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/api/test_updater.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/api/test_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/configuration/test_tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/configuration/test_tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/configuration/test_tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/exporters/test_tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/exporters/test_tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/loaders/test_tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/loaders/test_tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/managers/test_tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/managers/test_tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/util/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/util/test_tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/util/test_tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_install_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/workers/test_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/workers/test_uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/tests/workers/test_update_worker.py` & `OctoBot-Tentacles-Manager-2.9.1/tests/workers/test_update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/upload_tests/__init__.py` & `OctoBot-Tentacles-Manager-2.9.1/upload_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/upload_tests/_test_nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.9.1/upload_tests/_test_nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.9.0/upload_tests/test_s3_uploader.py` & `OctoBot-Tentacles-Manager-2.9.1/upload_tests/test_s3_uploader.py`

 * *Files identical despite different names*

