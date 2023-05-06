# Comparing `tmp/nanomock-0.0.6.tar.gz` & `tmp/nanomock-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomock-0.0.6.tar", last modified: Fri May  5 21:48:35 2023, max compression
+gzip compressed data, was "nanomock-0.0.7.tar", last modified: Sat May  6 15:00:39 2023, max compression
```

## Comparing `nanomock-0.0.6.tar` & `nanomock-0.0.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.126675 nanomock-0.0.6/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       44 2023-05-02 13:35:20.000000 nanomock-0.0.6/MANIFEST.in
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)     2959 2023-05-05 21:48:35.126675 nanomock-0.0.6/PKG-INFO
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.6/README.md
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       22 2023-05-05 13:26:19.000000 nanomock-0.0.6/nanomock/__init__.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/docker/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1043 2023-05-04 20:29:22.000000 nanomock-0.0.6/nanomock/docker/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2804 2023-05-04 18:55:41.000000 nanomock-0.0.6/nanomock/docker/autoheal.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1063 2023-05-04 20:35:54.000000 nanomock-0.0.6/nanomock/docker/interface.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      392 2023-05-04 20:29:56.000000 nanomock-0.0.6/nanomock/docker/linux.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      389 2023-05-04 20:30:32.000000 nanomock-0.0.6/nanomock/docker/macos.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     3170 2023-05-04 18:48:04.000000 nanomock-0.0.6/nanomock/docker/mixin.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      401 2023-05-04 20:30:11.000000 nanomock-0.0.6/nanomock/docker/windows.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 11:22:58.000000 nanomock-0.0.6/nanomock/internal/__init__.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 19:50:05.000000 nanomock-0.0.6/nanomock/internal/data/__init__.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-01 19:50:25.000000 nanomock-0.0.6/nanomock/internal/data/services/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      432 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/custom_Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      297 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/default_config-node.toml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      298 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/default_config-node_voting-disabled.toml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      220 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/default_config-rpc.toml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1822 2023-05-04 22:06:12.000000 nanomock-0.0.6/nanomock/internal/data/services/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/nanolooker/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      960 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/nanolooker/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:41:55.000000 nanomock-0.0.6/nanomock/internal/data/services/nanolooker/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.6/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/nanomonitor/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:41:59.000000 nanomock-0.0.6/nanomock/internal/data/services/nanomonitor/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      659 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/nanomonitor/default_config.php
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      354 2023-05-03 09:06:45.000000 nanomock-0.0.6/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/nanoticker/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/nanoticker/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:02.000000 nanomock-0.0.6/nanomock/internal/data/services/nanoticker/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      466 2023-05-03 12:43:51.000000 nanomock-0.0.6/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/nanovotevisu/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      768 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/nanovotevisu/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:05.000000 nanomock-0.0.6/nanomock/internal/data/services/nanovotevisu/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      503 2023-05-03 12:43:54.000000 nanomock-0.0.6/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      325 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/promexporter/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      323 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:14.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1555 2023-05-04 19:53:21.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/default_docker-compose.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      420 2023-05-04 19:54:54.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.118675 nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.118675 nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      132 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      515 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/promexporter/prometheus.yml
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/internal/data/services/tcpdump/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      119 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/tcpdump/Dockerfile
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-02 08:42:10.000000 nanomock-0.0.6/nanomock/internal/data/services/tcpdump/__init__.py
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)      221 2023-05-03 21:35:04.000000 nanomock-0.0.6/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      685 2023-04-27 20:34:19.000000 nanomock-0.0.6/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.6/nanomock/internal/dependency_checker.py
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)      806 2023-05-03 21:35:04.000000 nanomock-0.0.6/nanomock/internal/feature_toggle.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.6/nanomock/internal/nl_block_tools.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     7682 2023-05-02 21:23:27.000000 nanomock-0.0.6/nanomock/internal/nl_initialise.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     5695 2023-05-05 21:23:17.000000 nanomock-0.0.6/nanomock/internal/utils.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     1568 2023-05-05 13:17:03.000000 nanomock-0.0.6/nanomock/main.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/modules/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-04-27 15:36:50.000000 nanomock-0.0.6/nanomock/modules/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.6/nanomock/modules/nl_nanolib.py
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)    43726 2023-05-05 20:38:11.000000 nanomock-0.0.6/nanomock/modules/nl_parse_config.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.6/nanomock/modules/nl_rpc.py
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)    17717 2023-05-05 21:37:03.000000 nanomock-0.0.6/nanomock/nanomock_manager.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock/os_operations/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-04 18:54:54.000000 nanomock-0.0.6/nanomock/os_operations/__init__.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      250 2023-05-04 18:54:54.000000 nanomock-0.0.6/nanomock/os_operations/interface.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      159 2023-05-04 18:54:54.000000 nanomock-0.0.6/nanomock/os_operations/linux.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      159 2023-05-04 18:54:54.000000 nanomock-0.0.6/nanomock/os_operations/macos.py
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      825 2023-05-04 19:05:01.000000 nanomock-0.0.6/nanomock/os_operations/mixin.py
-drwxrwxr-x   0 gr0vity   (1000) gr0vity   (1000)        0 2023-05-05 21:48:35.122675 nanomock-0.0.6/nanomock.egg-info/
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2959 2023-05-05 21:48:35.000000 nanomock-0.0.6/nanomock.egg-info/PKG-INFO
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)     2989 2023-05-05 21:48:35.000000 nanomock-0.0.6/nanomock.egg-info/SOURCES.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        1 2023-05-05 21:48:35.000000 nanomock-0.0.6/nanomock.egg-info/dependency_links.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       48 2023-05-05 21:48:35.000000 nanomock-0.0.6/nanomock.egg-info/entry_points.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)       54 2023-05-05 21:48:35.000000 nanomock-0.0.6/nanomock.egg-info/requires.txt
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)        9 2023-05-05 21:48:35.000000 nanomock-0.0.6/nanomock.egg-info/top_level.txt
--rw-rw-r--   0 gr0vity   (1000) gr0vity   (1000)       38 2023-05-05 21:48:35.126675 nanomock-0.0.6/setup.cfg
--rw-r--r--   0 gr0vity   (1000) gr0vity   (1000)      784 2023-05-05 21:46:43.000000 nanomock-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 13:35:20.000000 nanomock-0.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-06 15:00:39.582845 nanomock-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.578845 nanomock-0.0.7/nanomock/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-05 21:48:35.000000 nanomock-0.0.7/nanomock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/docker/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 20:29:22.000000 nanomock-0.0.7/nanomock/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 18:55:41.000000 nanomock-0.0.7/nanomock/docker/autoheal.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-04 20:35:54.000000 nanomock-0.0.7/nanomock/docker/interface.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-04 20:29:56.000000 nanomock-0.0.7/nanomock/docker/linux.py
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 20:30:32.000000 nanomock-0.0.7/nanomock/docker/macos.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-04 18:48:04.000000 nanomock-0.0.7/nanomock/docker/mixin.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-04 20:30:11.000000 nanomock-0.0.7/nanomock/docker/windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 11:22:58.000000 nanomock-0.0.7/nanomock/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:05.000000 nanomock-0.0.7/nanomock/internal/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:25.000000 nanomock-0.0.7/nanomock/internal/data/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/custom_Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/default_config-node.toml
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/default_config-node_voting-disabled.toml
+-rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/default_config-rpc.toml
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-05-04 22:06:12.000000 nanomock-0.0.7/nanomock/internal/data/services/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/nanolooker/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/nanolooker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:55.000000 nanomock-0.0.7/nanomock/internal/data/services/nanolooker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.7/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/nanomonitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:59.000000 nanomock-0.0.7/nanomock/internal/data/services/nanomonitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/nanomonitor/default_config.php
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-03 09:06:45.000000 nanomock-0.0.7/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/nanoticker/
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/nanoticker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:02.000000 nanomock-0.0.7/nanomock/internal/data/services/nanoticker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-03 12:43:51.000000 nanomock-0.0.7/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/nanovotevisu/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/nanovotevisu/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:05.000000 nanomock-0.0.7/nanomock/internal/data/services/nanovotevisu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-03 12:43:54.000000 nanomock-0.0.7/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/promexporter/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:14.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-04 19:53:21.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 19:54:54.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.578845 nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.578845 nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
+-rw-r--r--   0 root         (0) root         (0)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/promexporter/prometheus.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/internal/data/services/tcpdump/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/tcpdump/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:10.000000 nanomock-0.0.7/nanomock/internal/data/services/tcpdump/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-05-03 21:35:04.000000 nanomock-0.0.7/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 20:34:19.000000 nanomock-0.0.7/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.7/nanomock/internal/dependency_checker.py
+-rw-rw-r--   0 root         (0) root         (0)      806 2023-05-03 21:35:04.000000 nanomock-0.0.7/nanomock/internal/feature_toggle.py
+-rw-r--r--   0 root         (0) root         (0)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.7/nanomock/internal/nl_block_tools.py
+-rw-r--r--   0 root         (0) root         (0)     7743 2023-05-06 14:53:34.000000 nanomock-0.0.7/nanomock/internal/nl_initialise.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-05-05 21:23:17.000000 nanomock-0.0.7/nanomock/internal/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-05-05 13:17:03.000000 nanomock-0.0.7/nanomock/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 15:36:50.000000 nanomock-0.0.7/nanomock/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.7/nanomock/modules/nl_nanolib.py
+-rw-rw-r--   0 root         (0) root         (0)    44025 2023-05-06 14:40:17.000000 nanomock-0.0.7/nanomock/modules/nl_parse_config.py
+-rw-r--r--   0 root         (0) root         (0)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.7/nanomock/modules/nl_rpc.py
+-rw-rw-r--   0 root         (0) root         (0)    18011 2023-05-06 14:53:58.000000 nanomock-0.0.7/nanomock/nanomock_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock/os_operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 18:54:54.000000 nanomock-0.0.7/nanomock/os_operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-04 18:54:54.000000 nanomock-0.0.7/nanomock/os_operations/interface.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.7/nanomock/os_operations/linux.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.7/nanomock/os_operations/macos.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-05-04 19:05:01.000000 nanomock-0.0.7/nanomock/os_operations/mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 15:00:39.582845 nanomock-0.0.7/nanomock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-06 15:00:39.000000 nanomock-0.0.7/nanomock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-06 15:00:39.000000 nanomock-0.0.7/nanomock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 15:00:39.000000 nanomock-0.0.7/nanomock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-06 15:00:39.000000 nanomock-0.0.7/nanomock.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-06 15:00:39.000000 nanomock-0.0.7/nanomock.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-06 15:00:39.000000 nanomock-0.0.7/nanomock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 15:00:39.582845 nanomock-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-06 14:57:47.000000 nanomock-0.0.7/setup.py
```

### Comparing `nanomock-0.0.6/PKG-INFO` & `nanomock-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.6
+Version: 0.0.7
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.6/README.md` & `nanomock-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/docker/__init__.py` & `nanomock-0.0.7/nanomock/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/docker/autoheal.py` & `nanomock-0.0.7/nanomock/docker/autoheal.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/docker/interface.py` & `nanomock-0.0.7/nanomock/docker/interface.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/docker/mixin.py` & `nanomock-0.0.7/nanomock/docker/mixin.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/default_docker-compose.yml` & `nanomock-0.0.7/nanomock/internal/data/services/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/nanolooker/Dockerfile` & `nanomock-0.0.7/nanomock/internal/data/services/nanolooker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/nanolooker/default_docker-compose.yml` & `nanomock-0.0.7/nanomock/internal/data/services/nanolooker/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/nanomonitor/default_config.php` & `nanomock-0.0.7/nanomock/internal/data/services/nanomonitor/default_config.php`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/nanoticker/Dockerfile` & `nanomock-0.0.7/nanomock/internal/data/services/nanoticker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/nanovotevisu/Dockerfile` & `nanomock-0.0.7/nanomock/internal/data/services/nanovotevisu/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/promexporter/default_docker-compose.yml` & `nanomock-0.0.7/nanomock/internal/data/services/promexporter/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json` & `nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml` & `nanomock-0.0.7/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/promexporter/prometheus.yml` & `nanomock-0.0.7/nanomock/internal/data/services/promexporter/prometheus.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json` & `nanomock-0.0.7/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/dependency_checker.py` & `nanomock-0.0.7/nanomock/internal/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/feature_toggle.py` & `nanomock-0.0.7/nanomock/internal/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/nl_block_tools.py` & `nanomock-0.0.7/nanomock/internal/nl_block_tools.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/internal/nl_initialise.py` & `nanomock-0.0.7/nanomock/internal/nl_initialise.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 from nanomock.modules.nl_nanolib import raw_high_precision_percent
 from nanomock.modules.nl_parse_config import ConfigParser
 from nanomock.internal.utils import NanoLocalLogger
 
 
 class InitialBlocks:
 
-    def __init__(self, data_dir, rpc_url, logger: NanoLocalLogger = None):
+    def __init__(self,
+                 config_parser: ConfigParser,
+                 rpc_url,
+                 logger: NanoLocalLogger = None):
         if logger is None:
             logger = NanoLocalLogger.get_logger(__name__)
         self.logger = logger
         self.api = NanoRpc(rpc_url)
-        self.config = ConfigParser(data_dir)
+        self.conf_p = config_parser
 
     def __epoch_link(self, epoch: int):
         message = f"epoch v{epoch} block"
         as_hex = bytearray(message, "ascii").hex()
         link = as_hex.upper().ljust(64, '0')
         return link
 
     def __publish_epochs(self):
         e = 1
         self.__log_active_difficulty()
-        while e <= self.config.get_all()["epoch_count"]:
+        while e <= self.conf_p.get_all()["epoch_count"]:
             link = self.__epoch_link(e)
             epoch_block = self.api.create_epoch_block(
                 link,
-                self.config.get_genesis_account_data()["private"],
-                self.config.get_genesis_account_data()["account"],
+                self.conf_p.get_genesis_account_data()["private"],
+                self.conf_p.get_genesis_account_data()["account"],
             )
             self.logger.append_log(
                 "InitialBlocks", "INFO",
                 "EPOCH {} sent by genesis : HASH {}".format(
                     e, epoch_block["hash"]))
             self.__log_active_difficulty()
             e += 1
@@ -42,112 +45,112 @@
         self.logger.append_log(
             "InitialBlocks", "INFO",
             f'current_diff : [{diff["network_current"]}]  current_receive_diff: [{diff["network_receive_current"]}]'
         )
 
     def __publish_canary(self):
         fv_canary_send_block = self.api.create_send_block_pkey(
-            self.config.get_genesis_account_data()["private"],
-            self.config.get_canary_account_data()["account"], 1)
+            self.conf_p.get_genesis_account_data()["private"],
+            self.conf_p.get_canary_account_data()["account"], 1)
         self.logger.append_log(
             "InitialBlocks", "INFO",
             "SEND FINAL VOTES CANARY BLOCK FROM {} To {} : HASH {}".format(
-                self.config.get_genesis_account_data()["account"],
-                self.config.get_canary_account_data()["account"],
+                self.conf_p.get_genesis_account_data()["account"],
+                self.conf_p.get_canary_account_data()["account"],
                 fv_canary_send_block["hash"]))
 
         fv_canary_open_block = self.api.create_open_block(
-            self.config.get_canary_account_data()["account"],
-            self.config.get_canary_account_data()["private"], 1,
-            self.config.get_genesis_account_data()["account"],
+            self.conf_p.get_canary_account_data()["account"],
+            self.conf_p.get_canary_account_data()["private"], 1,
+            self.conf_p.get_genesis_account_data()["account"],
             fv_canary_send_block["hash"])
         self.logger.append_log(
             "InitialBlocks", "INFO",
             "OPENED CANARY ACCOUNT {} : HASH {}".format(
-                self.config.get_canary_account_data()["account"],
+                self.conf_p.get_canary_account_data()["account"],
                 fv_canary_open_block["hash"]))
 
     def __send_to_burn(self):
-        if "burn_amount" not in self.config.get_all():
+        if "burn_amount" not in self.conf_p.get_all():
             self.logger.debug("[burn_amount] is not set. exit send_to_burn()")
             return False
 
         genesis_balance = int(
-            self.api.check_balance(self.config.get_genesis_account_data()
+            self.api.check_balance(self.conf_p.get_genesis_account_data()
                                    ["account"])["balance_raw"])
-        if int(self.config.get_all()["burn_amount"]) > genesis_balance:
+        if int(self.conf_p.get_all()["burn_amount"]) > genesis_balance:
             self.logger.append_log(
                 "InitialBlocks", "WARNING",
                 "[burn_amount] exceeds genesis balance. exit send_to_burn()")
             return False
 
         send_block = self.api.create_send_block_pkey(
-            self.config.get_genesis_account_data()["private"],
-            self.config.get_burn_account_data()["account"],
-            self.config.get_all()["burn_amount"])
+            self.conf_p.get_genesis_account_data()["private"],
+            self.conf_p.get_burn_account_data()["account"],
+            self.conf_p.get_all()["burn_amount"])
 
         self.logger.append_log(
             "InitialBlocks", "INFO",
             "SENT {:>40} FROM {} To {} : HASH {}".format(
                 send_block["amount_raw"],
-                self.config.get_genesis_account_data()["account"],
-                self.config.get_burn_account_data()["account"],
+                self.conf_p.get_genesis_account_data()["account"],
+                self.conf_p.get_burn_account_data()["account"],
                 send_block["hash"]))
 
     def __convert_weight_percentage_to_balance(self):
         genesis_balance = int(
             self.api.check_balance(
-                self.config.get_genesis_account_data()["account"],
+                self.conf_p.get_genesis_account_data()["account"],
                 include_only_confirmed=False)["balance_raw"])
         genesis_remaing = genesis_balance
 
-        for node_conf in self.config.get_nodes_config():
+        for node_conf in self.conf_p.get_nodes_config():
 
             if "vote_weight_percent" not in node_conf and "balance" not in node_conf:
                 continue  #skip genesis that was added as node
             if "vote_weight_percent" in node_conf:
                 node_conf["balance"] = raw_high_precision_percent(
                     genesis_balance, node_conf["vote_weight_percent"])
             node_conf["balance"] = int(node_conf["balance"])
 
             if genesis_remaing <= 0:
                 self.logger.append_log(
                     "InitialBlocks", "WARNING",
                     f'No Genesis funds remaining! Account [{node_conf["account_data"]["account"]}] will not be opened!'
                 )
-                #self.config["node_account_data"].remove(node_account_data)
+                #self.conf_p["node_account_data"].remove(node_account_data)
                 continue
             if genesis_remaing < node_conf["balance"]:
                 self.logger.append_log(
                     "InitialBlocks", "WARNING",
                     f'Genesis remaining balance is too small! Send {genesis_remaing} instead of {node_conf["balance"]}.'
                 )
 
-            self.config.set_node_balance(
+            self.conf_p.set_node_balance(
                 node_conf["name"], min(node_conf["balance"], genesis_remaing))
             genesis_remaing = max(0, genesis_remaing - node_conf["balance"])
 
     def __send_vote_weigh(self):
 
-        for node_conf in self.config.get_nodes_config():
+        for node_conf in self.conf_p.get_nodes_config():
 
             if "balance" not in node_conf:
 
                 continue  #skip genesis that was added as node
             node_account_data = node_conf["account_data"]
 
             send_block = self.api.create_send_block_pkey(
-                self.config.get_genesis_account_data()["private"],
+                self.conf_p.get_genesis_account_data()["private"],
                 node_account_data["account"], node_conf["balance"])
 
             self.logger.append_log(
                 "InitialBlocks", "INFO",
                 "SENT {:>40} FROM {} To {} : HASH {}".format(
                     send_block["amount_raw"],
-                    self.config.get_genesis_account_data()["account"],
+                    self.conf_p.get_genesis_account_data()["account"],
                     node_account_data["account"], send_block["hash"]))
 
             open_block = self.api.create_open_block(
                 node_account_data["account"], node_account_data["private"],
                 node_conf["balance"], node_account_data["account"],
                 send_block["hash"])
```

### Comparing `nanomock-0.0.6/nanomock/internal/utils.py` & `nanomock-0.0.7/nanomock/internal/utils.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/main.py` & `nanomock-0.0.7/nanomock/main.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/modules/nl_nanolib.py` & `nanomock-0.0.7/nanomock/modules/nl_nanolib.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/modules/nl_parse_config.py` & `nanomock-0.0.7/nanomock/modules/nl_parse_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                       default_flow_style=False)
 
 
 class ConfigParser:
 
     preconfigured_peers = []
 
-    def __init__(self, app_dir, config_file=None, logger=None):
+    def __init__(self, app_dir, config_file, logger=None):
         self.logger = logger or NanoLocalLogger.get_logger(__name__)
 
         self.enabled_services = []
         self._set_path_variables(app_dir, config_file)
         self.conf_rw = ConfigReadWrite(self.nl_config_path)
         self.nano_lib = NanoLibTools()
         self.config_dict = self.conf_rw.read_toml(self.nl_config_path)
@@ -106,16 +106,14 @@
         self.__set_node_accounts()
         self.__set_balance_from_vote_weight()
         self.__set_special_account_data()
         #self.__set_docker_compose()
 
     def _set_path_variables(self, app_dir, config_file):
         user_app_dir = Path(app_dir).resolve()
-        if config_file is None:
-            config_file = "nl_config.toml"
 
         if is_packaged_version():
             self.services_dir = "nanomock.internal.data.services"
             self.default_compose_path = f"{self.services_dir}.default_docker-compose.yml"
             self.default_nanomonitor_config = f"{self.services_dir}.nanomonitor.default_config.php"
             self.default_nanomonitor_config = f"{self.services_dir}.nanovotevisu.default_docker-compose.yml"
         else:
@@ -347,14 +345,22 @@
         return {"found": False, "value": None}
 
     def is_genesis(self, node_conf):
         if "is_genesis" in node_conf and node_conf["is_genesis"]:
             return True
         return False
 
+    def is_voting_enabled(self, node_name):
+        node_conf = self.get_node_config(node_name)
+        if node_conf:
+            return node_conf.get("enable_voting", True)
+        raise ValueError(
+            f"{node_name} undefined in {self.nl_config_path}\nValid names:{self.get_nodes_name()}"
+        )
+
     def _remove_keys_with_value(self, d, k, val):
         #if dict (d), search for key (k) that has value (val) and remove key-value pairfrom dict
         if k in d and d[k] == val:
             d.pop(k)
         for v in d.values():
             if isinstance(v, list):
                 for el in v:
@@ -380,14 +386,17 @@
 
         if save:
             self.config_dict = config_nested.data
             self.conf_rw.write_toml(self.nl_config_path, config_nested.data)
 
         return config_nested
 
+    def get_config_reader_writer(self):
+        return self.conf_rw
+
     def set_prom_runid(self, runid):
         self.runid = runid
 
     def get_name_with_prefix(self, node_name):
         return self.get_node_prefix() + node_name
 
     def get_node_prefix(self):
```

### Comparing `nanomock-0.0.6/nanomock/modules/nl_rpc.py` & `nanomock-0.0.7/nanomock/modules/nl_rpc.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock/nanomock_manager.py` & `nanomock-0.0.7/nanomock/nanomock_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import subprocess
 import logging
 from typing import List, Optional
 from .internal.dependency_checker import DependencyChecker
-from .modules.nl_parse_config import ConfigParser
+from .modules.nl_parse_config import ConfigParser, ConfigReadWrite
 from .internal.nl_initialise import InitialBlocks
 from .docker import create_docker_interface
 from .modules.nl_rpc import NanoRpc
 from .internal.utils import log_on_success, NanoLocalLogger, shutil_rmtree, extract_packaged_services_to_disk, subprocess_run_capture_output
 from typing import List, Dict, Optional, Tuple, Union
 import concurrent.futures
 from math import floor
@@ -18,17 +18,20 @@
 import inspect
 
 logger = NanoLocalLogger.get_logger(__name__)
 
 
 class NanoLocalManager:
 
-    def __init__(self, dir_path, project_name):
+    def __init__(self, dir_path, project_name, config_file="nl_config.toml"):
         self.command_mapping = self._initialize_command_mapping()
-        self.conf_p = ConfigParser(dir_path, logger=logger)
+        self.conf_p = ConfigParser(dir_path,
+                                   config_file=config_file,
+                                   logger=logger)
+        self.conf_rw = ConfigReadWrite(dir_path)
         self.dependency_checker = DependencyChecker()
         self.dependency_checker.check_dependencies()
 
         self.dir_path = dir_path
         self.nano_nodes_path = self.conf_p.nano_nodes_path
         self.compose_yml_path = self.conf_p.compose_out_path
         self.compose_env_path = os.path.join(self.nano_nodes_path,
@@ -64,55 +67,59 @@
 
     def _get_default(self, config_name):
         """ Load config with default values"""
         #minimal node config if no file is provided in the nl_config.toml
         if config_name == "config_node":
             default_config_path = os.path.join(self.services_dir,
                                                "default_config-node.toml")
-            return self.conf_p.conf_rw.read_toml(default_config_path,
-                                                 is_packaged=True)
+            return self.conf_rw.read_toml(default_config_path,
+                                          is_packaged=True)
         elif config_name == "config_rpc":
             default_rpc_path = os.path.join(self.services_dir,
                                             "default_config-rpc.toml")
-            return self.conf_p.conf_rw.read_toml(default_rpc_path,
-                                                 is_packaged=True)
+            return self.conf_rw.read_toml(default_rpc_path, is_packaged=True)
         else:
             return {}
 
     def _generate_docker_compose_env_file(self):
         env_variables = self.conf_p.get_docker_compose_env_variables()
-        self.conf_p.conf_rw.write_list(f'{self.compose_env_path}',
-                                       env_variables)
+        self.conf_rw.write_list(f'{self.compose_env_path}', env_variables)
 
     def _generate_docker_compose_yml_file(self):
         self.conf_p.set_docker_compose()
         self.conf_p.write_docker_compose()
 
-    def _generate_config_node_file(self, node_name):
+    def _set_config_node_file(self, node_name):
         config_node = self.conf_p.get_config_from_path(node_name,
                                                        "config_node_path")
         if config_node is None:
             logger.warning(
                 "No config-node.toml found. minimal version was created")
             config_node = self._get_default("config_node")
 
         config_node["node"][
             "preconfigured_peers"] = self.conf_p.preconfigured_peers
-        self.conf_p.conf_rw.write_toml(
+        config_node["node"]["enable_voting"] = self.conf_p.is_voting_enabled(
+            node_name)
+        return config_node
+
+    def _generate_config_node_file(self, node_name):
+        config_node = self._set_config_node_file(node_name)
+        self.conf_rw.write_toml(
             self.config_node_path.format(node_name=node_name), config_node)
 
     def _generate_config_rpc_file(self, node_name):
         config_rpc = self.conf_p.get_config_from_path(node_name,
                                                       "config_rpc_path")
         if config_rpc is None:
             logger.warning(
                 "No config-rpc.toml found. minimal version was created")
             config_rpc = self._get_default("config_rpc")
 
-        self.conf_p.conf_rw.write_toml(
+        self.conf_rw.write_toml(
             self.config_rpc_path.format(node_name=node_name), config_rpc)
 
     def _generate_nanomonitor_config_file(self, node_name):
         if self.conf_p.get_config_value("nanomonitor_enable"):
             self.conf_p.write_nanomonitor_config(node_name)
 
     def _create_node_folders(self, node_name):
@@ -340,15 +347,15 @@
             responses.append(response)
 
         return json.dumps(responses, indent=2)
 
     @log_on_success
     def init_wallets(self):
         #self.start_nodes('all')  #fixes a bug on mac m1
-        init_blocks = InitialBlocks(self.dir_path,
+        init_blocks = InitialBlocks(self.conf_p,
                                     self.conf_p.get_nodes_rpc()[0])
         for node_name in self.conf_p.get_nodes_name():
             if node_name == self.conf_p.get_genesis_node_name():
                 init_blocks.create_node_wallet(
                     self.conf_p.get_node_config(
                         self.conf_p.get_genesis_node_name())["rpc_url"],
                     self.conf_p.get_genesis_node_name(),
@@ -359,15 +366,15 @@
                     node_name,
                     seed=self.conf_p.get_node_config(node_name)["seed"])
         return init_blocks.logger.pop("InitialBlocks")
 
     @log_on_success
     def init_nodes(self):
         self.init_wallets()
-        init_blocks = InitialBlocks(self.dir_path,
+        init_blocks = InitialBlocks(self.conf_p,
                                     self.conf_p.get_nodes_rpc()[0])
         return init_blocks.publish_initial_blocks()
 
     @log_on_success
     def reset_nodes_data(self, nodes: Optional[List[str]] = None):
         self.stop_containers(nodes)
         nodes_to_process = nodes or ['.']
```

### Comparing `nanomock-0.0.6/nanomock/os_operations/mixin.py` & `nanomock-0.0.7/nanomock/os_operations/mixin.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/nanomock.egg-info/PKG-INFO` & `nanomock-0.0.7/nanomock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.6
+Version: 0.0.7
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.6/nanomock.egg-info/SOURCES.txt` & `nanomock-0.0.7/nanomock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.6/setup.py` & `nanomock-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanomock",
-      version="0.0.6",
+      version="0.0.7",
       author="gr0vity",
       description="Create local dockerized nano-currency networks",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanomock",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
```

