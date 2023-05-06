# Comparing `tmp/mythic_container-0.2.3rc4.tar.gz` & `tmp/mythic_container-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic_container-0.2.3rc4.tar", last modified: Thu Apr 27 21:30:45 2023, max compression
+gzip compressed data, was "mythic_container-0.2.4.tar", last modified: Sat May  6 01:34:06 2023, max compression
```

## Comparing `mythic_container-0.2.3rc4.tar` & `mythic_container-0.2.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-27 21:30:45.225650 mythic_container-0.2.3rc4/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.3rc4/LICENSE.md
--rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-04-27 21:30:45.225409 mythic_container-0.2.3rc4/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.3rc4/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-27 21:30:45.187882 mythic_container-0.2.3rc4/mythic_container/
--rw-r--r--   0 itsafeature   (501) staff       (20)    29960 2023-04-19 16:52:07.000000 mythic_container-0.2.3rc4/mythic_container/C2ProfileBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.3rc4/mythic_container/LoggingBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    77811 2023-04-20 00:07:13.000000 mythic_container-0.2.3rc4/mythic_container/MythicCommandBase.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-27 21:30:45.222794 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.3rc4/mythic_container/MythicRPC.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    22324 2023-04-21 19:16:23.000000 mythic_container-0.2.3rc4/mythic_container/PayloadBuilder.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7251 2023-04-19 16:38:54.000000 mythic_container-0.2.3rc4/mythic_container/TranslationBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-04-25 19:08:24.000000 mythic_container-0.2.3rc4/mythic_container/WebhookBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2578 2023-04-27 21:30:35.000000 mythic_container-0.2.3rc4/mythic_container/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    37152 2023-04-27 04:38:26.000000 mythic_container-0.2.3rc4/mythic_container/agent_utils.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.3rc4/mythic_container/c2_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.3rc4/mythic_container/config.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-27 21:30:45.224522 mythic_container-0.2.3rc4/mythic_container/grpc/
--rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.3rc4/mythic_container/grpc/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.3rc4/mythic_container/grpc/translationContainerGRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.3rc4/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.3rc4/mythic_container/logging.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.3rc4/mythic_container/logging_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)    29520 2023-04-27 21:29:31.000000 mythic_container-0.2.3rc4/mythic_container/mythic_service.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    15080 2023-04-27 21:25:32.000000 mythic_container-0.2.3rc4/mythic_container/rabbitmq.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.3rc4/mythic_container/utils_mythic_file_transfer.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.3rc4/mythic_container/webhook_utils.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-27 21:30:45.189839 mythic_container-0.2.3rc4/mythic_container.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-04-27 21:30:45.000000 mythic_container-0.2.3rc4/mythic_container.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-04-27 21:30:45.000000 mythic_container-0.2.3rc4/mythic_container.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-27 21:30:45.000000 mythic_container-0.2.3rc4/mythic_container.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-04-27 21:30:45.000000 mythic_container-0.2.3rc4/mythic_container.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-04-27 21:30:45.000000 mythic_container-0.2.3rc4/mythic_container.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-27 21:30:45.225754 mythic_container-0.2.3rc4/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1093 2023-04-27 21:30:21.000000 mythic_container-0.2.3rc4/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-06 01:34:06.664799 mythic_container-0.2.4/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.4/LICENSE.md
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-05-06 01:34:06.664277 mythic_container-0.2.4/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.4/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-06 01:34:06.611482 mythic_container-0.2.4/mythic_container/
+-rw-r--r--   0 itsafeature   (501) staff       (20)    29960 2023-04-19 16:52:07.000000 mythic_container-0.2.4/mythic_container/C2ProfileBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.4/mythic_container/LoggingBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    77811 2023-04-20 00:07:13.000000 mythic_container-0.2.4/mythic_container/MythicCommandBase.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-06 01:34:06.660405 mythic_container-0.2.4/mythic_container/MythicGoRPC/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.4/mythic_container/MythicRPC.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    22456 2023-05-05 22:49:39.000000 mythic_container-0.2.4/mythic_container/PayloadBuilder.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7251 2023-04-19 16:38:54.000000 mythic_container-0.2.4/mythic_container/TranslationBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-04-25 19:08:24.000000 mythic_container-0.2.4/mythic_container/WebhookBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2573 2023-05-06 01:24:42.000000 mythic_container-0.2.4/mythic_container/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    37152 2023-04-27 04:38:26.000000 mythic_container-0.2.4/mythic_container/agent_utils.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.4/mythic_container/c2_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.4/mythic_container/config.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-06 01:34:06.663094 mythic_container-0.2.4/mythic_container/grpc/
+-rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.4/mythic_container/grpc/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.4/mythic_container/grpc/translationContainerGRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.4/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.4/mythic_container/logging.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.4/mythic_container/logging_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)    29520 2023-04-27 21:29:31.000000 mythic_container-0.2.4/mythic_container/mythic_service.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    15080 2023-04-27 21:25:32.000000 mythic_container-0.2.4/mythic_container/rabbitmq.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.4/mythic_container/utils_mythic_file_transfer.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.4/mythic_container/webhook_utils.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-06 01:34:06.613714 mythic_container-0.2.4/mythic_container.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-05-06 01:34:06.000000 mythic_container-0.2.4/mythic_container.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-05-06 01:34:06.000000 mythic_container-0.2.4/mythic_container.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-06 01:34:06.000000 mythic_container-0.2.4/mythic_container.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-05-06 01:34:06.000000 mythic_container-0.2.4/mythic_container.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-05-06 01:34:06.000000 mythic_container-0.2.4/mythic_container.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-06 01:34:06.664979 mythic_container-0.2.4/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1088 2023-05-06 01:24:33.000000 mythic_container-0.2.4/setup.py
```

### Comparing `mythic_container-0.2.3rc4/LICENSE.md` & `mythic_container-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/PKG-INFO` & `mythic_container-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic_container
-Version: 0.2.3rc4
+Version: 0.2.4
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.3rc4/README.md` & `mythic_container-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/C2ProfileBase.py` & `mythic_container-0.2.4/mythic_container/C2ProfileBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/LoggingBase.py` & `mythic_container-0.2.4/mythic_container/LoggingBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicCommandBase.py` & `mythic_container-0.2.4/mythic_container/MythicCommandBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/__init__.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/__init__.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py` & `mythic_container-0.2.4/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/MythicRPC.py` & `mythic_container-0.2.4/mythic_container/MythicRPC.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/PayloadBuilder.py` & `mythic_container-0.2.4/mythic_container/PayloadBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,21 +53,24 @@
             The user can supply multiple values in an Array format
         Date:
             The user can select a Date in YYYY-MM-DD format
         Dictionary:
             The user can supply a dictionary of values
         Boolean:
             The user can toggle a switch for True/False
+        File:
+            The user can select a file that gets uploaded - a file UUID gets passed in during build
     """
     String = "String"
     ChooseOne = "ChooseOne"
     Array = "Array"
     Date = "Date"
     Dictionary = "Dictionary"
     Boolean = "Boolean"
+    File = "File"
 
 
 class DictionaryChoice:
     """A single dictionary choice/option for the UI when select C2 Profile Parameters
 
     Attributes:
         name (str): Name of the choice
```

### Comparing `mythic_container-0.2.3rc4/mythic_container/TranslationBase.py` & `mythic_container-0.2.4/mythic_container/TranslationBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/WebhookBase.py` & `mythic_container-0.2.4/mythic_container/WebhookBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/__init__.py` & `mythic_container-0.2.4/mythic_container/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rabbitmq import rabbitmqConnectionClass
 from .mythic_service import start_and_run_forever, test_command
 
-containerVersion = "v1.0.0"
+containerVersion = "v1.0.2"
 
-PyPi_version = "0.2.3-rc04"
+PyPi_version = "0.2.4"
 
 RabbitmqConnection = rabbitmqConnectionClass()
 
 MYTHIC_RPC_OTHER_SERVICES_RPC = "mythic_rpc_other_service_rpc"
 PAYLOAD_BUILD_C2_ROUTING_KEY = "payload_c2_build"
 # payload routes
 PT_SYNC_ROUTING_KEY = "pt_sync"
```

### Comparing `mythic_container-0.2.3rc4/mythic_container/agent_utils.py` & `mythic_container-0.2.4/mythic_container/agent_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/c2_utils.py` & `mythic_container-0.2.4/mythic_container/c2_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/grpc/translationContainerGRPC_pb2.py` & `mythic_container-0.2.4/mythic_container/grpc/translationContainerGRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py` & `mythic_container-0.2.4/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/logging.py` & `mythic_container-0.2.4/mythic_container/logging.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/logging_utils.py` & `mythic_container-0.2.4/mythic_container/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/mythic_service.py` & `mythic_container-0.2.4/mythic_container/mythic_service.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/rabbitmq.py` & `mythic_container-0.2.4/mythic_container/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/utils_mythic_file_transfer.py` & `mythic_container-0.2.4/mythic_container/utils_mythic_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container/webhook_utils.py` & `mythic_container-0.2.4/mythic_container/webhook_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/mythic_container.egg-info/PKG-INFO` & `mythic_container-0.2.4/mythic_container.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic-container
-Version: 0.2.3rc4
+Version: 0.2.4
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.3rc4/mythic_container.egg-info/SOURCES.txt` & `mythic_container-0.2.4/mythic_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.3rc4/setup.py` & `mythic_container-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic_container",
-    version="0.2.3-rc04",
+    version="0.2.4",
     description="Functionality for Mythic Services",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/customizing/payload-type-development",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

