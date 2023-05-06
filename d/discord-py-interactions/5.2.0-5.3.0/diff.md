# Comparing `tmp/discord-py-interactions-5.2.0.tar.gz` & `tmp/discord-py-interactions-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-py-interactions-5.2.0.tar", last modified: Sun Apr 30 10:06:25 2023, max compression
+gzip compressed data, was "discord-py-interactions-5.3.0.tar", last modified: Sat May  6 07:14:37 2023, max compression
```

## Comparing `discord-py-interactions-5.2.0.tar` & `discord-py-interactions-5.3.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.598552 discord-py-interactions-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-30 10:06:25.598552 discord-py-interactions-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.566552 discord-py-interactions-5.2.0/discord_py_interactions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-30 10:06:25.000000 discord-py-interactions-5.2.0/discord_py_interactions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-30 10:06:25.000000 discord-py-interactions-5.2.0/discord_py_interactions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 10:06:25.000000 discord-py-interactions-5.2.0/discord_py_interactions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 10:06:25.000000 discord-py-interactions-5.2.0/discord_py_interactions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 10:06:25.000000 discord-py-interactions-5.2.0/discord_py_interactions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.566552 discord-py-interactions-5.2.0/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.566552 discord-py-interactions-5.2.0/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.566552 discord-py-interactions-5.2.0/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.570552 discord-py-interactions-5.2.0/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.570552 discord-py-interactions-5.2.0/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.570552 discord-py-interactions-5.2.0/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.574552 discord-py-interactions-5.2.0/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35371 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.574552 discord-py-interactions-5.2.0/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.578552 discord-py-interactions-5.2.0/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.578552 discord-py-interactions-5.2.0/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    88416 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.578552 discord-py-interactions-5.2.0/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.582552 discord-py-interactions-5.2.0/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.582552 discord-py-interactions-5.2.0/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.582552 discord-py-interactions-5.2.0/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/debug_extension/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.582552 discord-py-interactions-5.2.0/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.586552 discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.586552 discord-py-interactions-5.2.0/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.594552 discord-py-interactions-5.2.0/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   102768 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    30028 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    37383 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.594552 discord-py-interactions-5.2.0/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.594552 discord-py-interactions-5.2.0/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    55413 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    34488 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.598552 discord-py-interactions-5.2.0/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.598552 discord-py-interactions-5.2.0/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/interactions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-30 10:06:25.598552 discord-py-interactions-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-30 10:06:15.000000 discord-py-interactions-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:25.598552 discord-py-interactions-5.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-30 10:06:02.000000 discord-py-interactions-5.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.990332 discord-py-interactions-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-06 07:14:37.990332 discord-py-interactions-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.954333 discord-py-interactions-5.3.0/discord_py_interactions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-06 07:14:37.000000 discord-py-interactions-5.3.0/discord_py_interactions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-06 07:14:37.000000 discord-py-interactions-5.3.0/discord_py_interactions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:14:37.000000 discord-py-interactions-5.3.0/discord_py_interactions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-06 07:14:37.000000 discord-py-interactions-5.3.0/discord_py_interactions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 07:14:37.000000 discord-py-interactions-5.3.0/discord_py_interactions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.954333 discord-py-interactions-5.3.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.954333 discord-py-interactions-5.3.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.954333 discord-py-interactions-5.3.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.958333 discord-py-interactions-5.3.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.962333 discord-py-interactions-5.3.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.962333 discord-py-interactions-5.3.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.966333 discord-py-interactions-5.3.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35371 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.970333 discord-py-interactions-5.3.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.970333 discord-py-interactions-5.3.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.974333 discord-py-interactions-5.3.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88891 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.974333 discord-py-interactions-5.3.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.978333 discord-py-interactions-5.3.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.978333 discord-py-interactions-5.3.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.978333 discord-py-interactions-5.3.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/debug_extension/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.982333 discord-py-interactions-5.3.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.982333 discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.982333 discord-py-interactions-5.3.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.986333 discord-py-interactions-5.3.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102931 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95578 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38185 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.990332 discord-py-interactions-5.3.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.990332 discord-py-interactions-5.3.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55485 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35094 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.990332 discord-py-interactions-5.3.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.990332 discord-py-interactions-5.3.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/interactions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-06 07:14:37.994333 discord-py-interactions-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-06 07:14:31.000000 discord-py-interactions-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:37.990332 discord-py-interactions-5.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-06 07:14:21.000000 discord-py-interactions-5.3.0/tests/utils.py
```

### Comparing `discord-py-interactions-5.2.0/LICENSE` & `discord-py-interactions-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/PKG-INFO` & `discord-py-interactions-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.2.0
+Version: 5.3.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.2.0/README.md` & `discord-py-interactions-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/discord_py_interactions.egg-info/PKG-INFO` & `discord-py-interactions-5.3.0/discord_py_interactions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.2.0
+Version: 5.3.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.2.0/discord_py_interactions.egg-info/SOURCES.txt` & `discord-py-interactions-5.3.0/discord_py_interactions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/discord_py_interactions.egg-info/requires.txt` & `discord-py-interactions-5.3.0/discord_py_interactions.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 uvloop
 
 [console]
 aioconsole>=0.6.0
 
 [dev]
 pytest
-pytest-recording
 pytest-asyncio
 pytest-cov
 python-dotenv
 typeguard
 PyNaCl<1.6,>=1.5.0
 aiodns
 orjson
@@ -80,15 +79,14 @@
 faust-cchardet
 
 [speedup:sys_platform != "win32"]
 uvloop
 
 [tests]
 pytest
-pytest-recording
 pytest-asyncio
 pytest-cov
 python-dotenv
 typeguard
 
 [voice]
 PyNaCl<1.6,>=1.5.0
```

### Comparing `discord-py-interactions-5.2.0/interactions/__init__.py` & `discord-py-interactions-5.3.0/interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/__init__.py` & `discord-py-interactions-5.3.0/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/base.py` & `discord-py-interactions-5.3.0/interactions/api/events/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
     override_name: str = attrs.field(repr=False, kw_only=True, default=None)
     """Custom name of the event to be used when dispatching."""
     bot: "Client" = attrs.field(repr=False, kw_only=True, default=MISSING)
     """The client instance that dispatched this event."""
 
     @property
+    def client(self) -> "Client":
+        """The client instance that dispatched this event."""
+        return self.bot
+
+    @property
     def resolved_name(self) -> str:
         """The name of the event, defaults to the class name if not overridden."""
         name = self.override_name or self.__class__.__name__
         return _event_reg.sub("_", name).lower()
 
     @classmethod
     def listen(cls, coro: AsyncCallable, client: "Client") -> "models.Listener":
```

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/discord.py` & `discord-py-interactions-5.3.0/interactions/api/events/discord.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/internal.py` & `discord-py-interactions-5.3.0/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/__init__.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/_template.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/auto_mod.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/channel_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/guild_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/integrations.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/member_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/message_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/reaction_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/reaction_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import TYPE_CHECKING
 
 import interactions.api.events as events
 from interactions.models import PartialEmoji, Reaction
+
 from ._template import EventMixinTemplate, Processor
 
 if TYPE_CHECKING:
     from interactions.api.events import RawGatewayEvent
 
 __all__ = ("ReactionEvents",)
 
 
 class ReactionEvents(EventMixinTemplate):
     async def _handle_message_reaction_change(self, event: "RawGatewayEvent", add: bool) -> None:
         if member := event.data.get("member"):
             author = self.cache.place_member_data(event.data.get("guild_id"), member)
+        elif guild_id := event.data.get("guild_id"):
+            author = await self.cache.fetch_member(guild_id, event.data.get("user_id"))
         else:
             author = await self.cache.fetch_user(event.data.get("user_id"))
 
         emoji = PartialEmoji.from_dict(event.data.get("emoji"))  # type: ignore
         message = self.cache.get_message(event.data.get("channel_id"), event.data.get("message_id"))
         reaction = None
```

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/role_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/stage_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/thread_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/user_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/events/processors/voice_events.py` & `discord-py-interactions-5.3.0/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/gateway/gateway.py` & `discord-py-interactions-5.3.0/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/gateway/state.py` & `discord-py-interactions-5.3.0/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/gateway/websocket.py` & `discord-py-interactions-5.3.0/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_client.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/__init__.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/bot.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/channels.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/channels.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/emojis.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/guild.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/guild.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/interactions.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/members.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/messages.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/reactions.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/scheduled_events.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/stickers.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/threads.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/threads.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/users.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/http_requests/webhooks.py` & `discord-py-interactions-5.3.0/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/http/route.py` & `discord-py-interactions-5.3.0/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/voice/audio.py` & `discord-py-interactions-5.3.0/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/voice/audio_writer.py` & `discord-py-interactions-5.3.0/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/voice/encryption.py` & `discord-py-interactions-5.3.0/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/voice/opus.py` & `discord-py-interactions-5.3.0/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/voice/player.py` & `discord-py-interactions-5.3.0/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/voice/recorder.py` & `discord-py-interactions-5.3.0/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/api/voice/voice_gateway.py` & `discord-py-interactions-5.3.0/interactions/api/voice/voice_gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/bin/opus-x64.dll` & `discord-py-interactions-5.3.0/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/bin/opus-x86.dll` & `discord-py-interactions-5.3.0/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/__init__.py` & `discord-py-interactions-5.3.0/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/auto_shard_client.py` & `discord-py-interactions-5.3.0/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/client.py` & `discord-py-interactions-5.3.0/interactions/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,19 +567,25 @@
                 if (
                     not isinstance(_event, (events.Error, events.RawGatewayEvent))
                     and coro.delay_until_ready
                     and not self.is_ready
                 ):
                     await self.wait_until_ready()
 
-                if len(_event.__attrs_attrs__) == 2 and coro.event != "event":
-                    # override_name & bot & logging
-                    await _coro()
-                else:
+                # don't pass event object if listener doesn't expect it
+                if _coro.pass_event_object:
                     await _coro(_event, *_args, **_kwargs)
+                else:
+                    if not _coro.warned_no_event_arg and len(_event.__attrs_attrs__) > 2 and _coro.event != "event":
+                        self.logger.warning(
+                            f"{_coro} is listening to {_coro.event} event which contains event data. "
+                            f"Add an event argument to this listener to receive the event data object."
+                        )
+                        _coro.warned_no_event_arg = True
+                    await _coro()
             except asyncio.CancelledError:
                 pass
             except Exception as e:
                 if isinstance(event, events.Error):
                     # No infinite loops please
                     self.default_error_handler(repr(event), e)
                 else:
@@ -1198,14 +1204,16 @@
                         )
 
         # prevent the same callback being added twice
         if listener in self.listeners.get(listener.event, []):
             self.logger.debug(f"Listener {listener} has already been hooked, not re-hooking it again")
             return
 
+        listener.lazy_parse_params()
+
         if listener.event not in self.listeners:
             self.listeners[listener.event] = []
         self.listeners[listener.event].append(listener)
 
         # check if other listeners are to be deleted
         default_listeners = [c_listener.is_default_listener for c_listener in self.listeners[listener.event]]
         removes_defaults = [c_listener.disable_default_listeners for c_listener in self.listeners[listener.event]]
```

### Comparing `discord-py-interactions-5.2.0/interactions/client/const.py` & `discord-py-interactions-5.3.0/interactions/client/const.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/errors.py` & `discord-py-interactions-5.3.0/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/mixins/modal.py` & `discord-py-interactions-5.3.0/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/mixins/send.py` & `discord-py-interactions-5.3.0/interactions/client/mixins/send.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/mixins/serialization.py` & `discord-py-interactions-5.3.0/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/smart_cache.py` & `discord-py-interactions-5.3.0/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/__init__.py` & `discord-py-interactions-5.3.0/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/attr_converters.py` & `discord-py-interactions-5.3.0/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/attr_utils.py` & `discord-py-interactions-5.3.0/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/attr_utils.pyi` & `discord-py-interactions-5.3.0/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/cache.py` & `discord-py-interactions-5.3.0/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/deserialise_app_cmds.py` & `discord-py-interactions-5.3.0/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/formatting.py` & `discord-py-interactions-5.3.0/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/input_utils.py` & `discord-py-interactions-5.3.0/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/misc_utils.py` & `discord-py-interactions-5.3.0/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/serializer.py` & `discord-py-interactions-5.3.0/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/client/utils/text_utils.py` & `discord-py-interactions-5.3.0/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/console.py` & `discord-py-interactions-5.3.0/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/debug_extension/__init__.py` & `discord-py-interactions-5.3.0/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/debug_extension/debug_application_cmd.py` & `discord-py-interactions-5.3.0/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/debug_extension/debug_exec.py` & `discord-py-interactions-5.3.0/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/debug_extension/debug_exts.py` & `discord-py-interactions-5.3.0/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/debug_extension/utils.py` & `discord-py-interactions-5.3.0/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/jurigged.py` & `discord-py-interactions-5.3.0/interactions/ext/jurigged.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/mypy/__init__.py` & `discord-py-interactions-5.3.0/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/paginators.py` & `discord-py-interactions-5.3.0/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/__init__.py` & `discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/command.py` & `discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/context.py` & `discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/context.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/help.py` & `discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/manager.py` & `discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
         if not cmd.is_subcommand:
             self.add_command(cmd)
 
     @listen("extension_unload")
     async def _handle_ext_unload(self, event: ExtensionUnload) -> None:
         """Unregisters all prefixed commands in an extension as it is being unloaded."""
-        for name in self._ext_command_list[event.extension.extension_name]:
+        for name in self._ext_command_list[event.extension.extension_name].copy():
             self.remove_command(name)
 
     @listen("raw_message_create", is_default_listener=True)
     async def _dispatch_prefixed_commands(self, event: RawGatewayEvent) -> None:  # noqa: C901
         """Determine if a prefixed command is being triggered, and dispatch it."""
         # don't waste time processing this if there are no prefixed commands
         if not self.commands:
```

### Comparing `discord-py-interactions-5.2.0/interactions/ext/prefixed_commands/utils.py` & `discord-py-interactions-5.3.0/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/ext/sentry.py` & `discord-py-interactions-5.3.0/interactions/ext/sentry.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/__init__.py` & `discord-py-interactions-5.3.0/interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/__init__.py` & `discord-py-interactions-5.3.0/interactions/models/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/activity.py` & `discord-py-interactions-5.3.0/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/app_perms.py` & `discord-py-interactions-5.3.0/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/application.py` & `discord-py-interactions-5.3.0/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/asset.py` & `discord-py-interactions-5.3.0/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/auto_mod.py` & `discord-py-interactions-5.3.0/interactions/models/discord/auto_mod.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 
     type: AutoModTriggerType = attrs.field(
         default=AutoModTriggerType.HARMFUL_LINK,
         converter=AutoModTriggerType,
         repr=True,
         metadata=docs("The type of trigger"),
     )
-    ...
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class KeywordPresetTrigger(BaseTrigger):
     """A trigger that checks if content contains words from internal pre-defined wordsets"""
 
     type: AutoModTriggerType = attrs.field(
@@ -148,19 +147,31 @@
 
     mention_total_limit: int = attrs.field(
         default=3, repr=True, metadata=docs("The maximum number of mentions allowed")
     )
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class MemberProfileTrigger(BaseTrigger):
+    regex_patterns: list[str] = attrs.field(
+        factory=list, repr=True, metadata=docs("The regex patterns to check against")
+    )
+    keyword_filter: str | list[str] = attrs.field(
+        factory=list, repr=True, metadata=docs("The keywords to check against")
+    )
+    allow_list: list["Snowflake_Type"] = attrs.field(
+        factory=list, repr=True, metadata=docs("The roles exempt from this rule")
+    )
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class BlockMessage(BaseAction):
     """blocks the content of a message according to the rule"""
 
     type: AutoModAction = attrs.field(repr=False, default=AutoModAction.BLOCK_MESSAGE, converter=AutoModAction)
-    ...
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class AlertMessage(BaseAction):
     """logs user content to a specified channel"""
 
     channel_id: "Snowflake_Type" = attrs.field(repr=True)
@@ -171,14 +182,21 @@
 class TimeoutUser(BaseAction):
     """timeout user for a specified duration"""
 
     duration_seconds: int = attrs.field(repr=True, default=60)
     type: AutoModAction = attrs.field(repr=False, default=AutoModAction.TIMEOUT_USER, converter=AutoModAction)
 
 
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class BlockMemberInteraction(BaseAction):
+    """Block a member from using text, voice, or other interactions"""
+
+    # this action has no metadata
+
+
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class AutoModRule(DiscordObject):
     """A representation of an auto mod rule"""
 
     name: str = attrs.field(
         repr=False,
     )
@@ -341,15 +359,17 @@
         return self._client.cache.get_member(self._guild_id, self._user_id)
 
 
 ACTION_MAPPING = {
     AutoModAction.BLOCK_MESSAGE: BlockMessage,
     AutoModAction.ALERT_MESSAGE: AlertMessage,
     AutoModAction.TIMEOUT_USER: TimeoutUser,
+    AutoModAction.BLOCK_MEMBER_INTERACTION: BlockMemberInteraction,
 }
 
 TRIGGER_MAPPING = {
     AutoModTriggerType.KEYWORD: KeywordTrigger,
     AutoModTriggerType.HARMFUL_LINK: HarmfulLinkFilter,
     AutoModTriggerType.KEYWORD_PRESET: KeywordPresetTrigger,
     AutoModTriggerType.MENTION_SPAM: MentionSpamTrigger,
+    AutoModTriggerType.MEMBER_PROFILE: MemberProfileTrigger,
 }
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/base.py` & `discord-py-interactions-5.3.0/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/channel.py` & `discord-py-interactions-5.3.0/interactions/models/discord/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1897,14 +1897,19 @@
         return f"<#{self.id}>"
 
     @property
     def permission_overwrites(self) -> List["PermissionOverwrite"]:
         """The permission overwrites for this channel."""
         return []
 
+    @property
+    def clyde_created(self) -> bool:
+        """Whether this thread was created by Clyde."""
+        return ChannelFlags.CLYDE_THREAD in self.flags
+
     def permissions_for(self, instance: Snowflake_Type) -> Permissions:
         """
         Calculates permissions for an instance
 
         Args:
             instance: Member or Role instance (or its ID)
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/color.py` & `discord-py-interactions-5.3.0/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/components.py` & `discord-py-interactions-5.3.0/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/embed.py` & `discord-py-interactions-5.3.0/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/emoji.py` & `discord-py-interactions-5.3.0/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/enums.py` & `discord-py-interactions-5.3.0/interactions/models/discord/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,14 +453,16 @@
     """This message is an Interaction Response and the bot is "thinking"""
     FAILED_TO_MENTION_SOME_ROLES_IN_THREAD = 1 << 8
     """This message failed to mention some roles and add their members to the thread"""
     SHOULD_SHOW_LINK_NOT_DISCORD_WARNING = 1 << 10
     """This message contains a abusive website link, pops up a warning when clicked"""
     SILENT = 1 << 12
     """This message should not trigger push or desktop notifications"""
+    VOICE_MESSAGE = 1 << 13
+    """This message is a voice message"""
 
     # Special members
     NONE = 0
     ALL = AntiFlag()
 
 
 class Permissions(DiscordIntFlag):  # type: ignore
@@ -547,14 +549,24 @@
     """Allows the usage of custom stickers from other servers"""
     SEND_MESSAGES_IN_THREADS = 1 << 38
     """Allows for sending messages in threads"""
     START_EMBEDDED_ACTIVITIES = 1 << 39
     """Allows for using Activities (applications with the `EMBEDDED` flag) in a voice channel"""
     MODERATE_MEMBERS = 1 << 40
     """Allows for timing out users to prevent them from sending or reacting to messages in chat and threads, and from speaking in voice and stage channels"""
+    VIEW_CREATOR_MONETIZATION_ANALYTICS = 1 << 41
+    """Allows for viewing guild monetization insights"""
+    USE_SOUNDBOARD = 1 << 42
+    """Allows for using the soundboard in a voice channel"""
+    CREATE_GUILD_EXPRESSIONS = 1 << 43
+    """Allows for creating emojis, stickers, and soundboard sounds"""
+    USE_EXTERNAL_SOUNDS = 1 << 45
+    """Allows the usage of custom sounds from other servers"""
+    SEND_VOICE_MESSAGES = 1 << 46
+    """Allows for sending audio messages"""
 
     # Shortcuts/grouping/aliases
     REQUIRES_MFA = (
         KICK_MEMBERS
         | BAN_MEMBERS
         | ADMINISTRATOR
         | MANAGE_CHANNELS
@@ -776,14 +788,16 @@
     NONE = 0
     ALL = AntiFlag()
 
 
 class ChannelFlags(DiscordIntFlag):
     PINNED = 1 << 1
     """ Thread is pinned to the top of its parent forum channel """
+    CLYDE_THREAD = 1 << 8
+    """This thread was created by Clyde"""
 
     # Special members
     NONE = 0
 
 
 class VideoQualityMode(CursedIntEnum):
     """Video quality settings."""
@@ -960,34 +974,38 @@
     ROLE_PROMPT_UPDATE = 161
     ROLE_PROMPT_DELETE = 162
     ON_BOARDING_QUESTION_CREATE = 163
     ON_BOARDING_QUESTION_UPDATE = 164
     ONBOARDING_UPDATE = 167
     GUILD_HOME_FEATURE_ITEM = 171
     GUILD_HOME_FEATURE_ITEM_UPDATE = 172
+    BLOCKED_PHISHING_LINK = 180
     SERVER_GUIDE_CREATE = 190
     SERVER_GUIDE_UPDATE = 191
 
 
 class AutoModTriggerType(CursedIntEnum):
     KEYWORD = 1
     HARMFUL_LINK = 2
     SPAM = 3
     KEYWORD_PRESET = 4
     MENTION_SPAM = 5
+    MEMBER_PROFILE = 6
 
 
 class AutoModAction(CursedIntEnum):
     BLOCK_MESSAGE = 1
     ALERT_MESSAGE = 2
     TIMEOUT_USER = 3
+    BLOCK_MEMBER_INTERACTION = 4
 
 
 class AutoModEvent(CursedIntEnum):
     MESSAGE_SEND = 1
+    MEMBER_UPDATE = 2
 
 
 class AutoModLanuguageType(Enum):
     PROFANITY = "PROFANITY"
     SEXUAL = "SEXUAL_CONTENT"
     INSULTS_AND_SLURS = "SLURS"
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/file.py` & `discord-py-interactions-5.3.0/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/guild.py` & `discord-py-interactions-5.3.0/interactions/models/discord/guild.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,14 +435,29 @@
     def voice_states(self) -> List["models.VoiceState"]:
         """Get a list of the active voice states in this guild."""
         # this is *very* ick, but we cache by user_id, so we have to do it this way,
         # alternative would be maintaining a lookup table in this guild object, which is inherently unreliable
         # noinspection PyProtectedMember
         return [v_state for v_state in self._client.cache.voice_state_cache.values() if v_state._guild_id == self.id]
 
+    @property
+    def mention_onboarding_customize(self) -> str:
+        """Return a mention string for the customise section of Onboarding"""
+        return "<id:customize>"
+
+    @property
+    def mention_onboarding_browse(self) -> str:
+        """Return a mention string for the browse section of Onboarding"""
+        return "<id:browse>"
+
+    @property
+    def mention_onboarding_guide(self) -> str:
+        """Return a mention string for the guide section of Onboarding"""
+        return "<id:guide>"
+
     async def fetch_member(self, member_id: Snowflake_Type, *, force: bool = False) -> Optional["models.Member"]:
         """
         Return the Member with the given discord ID, fetching from the API if necessary.
 
         Args:
             member_id: The ID of the member.
             force: Whether to force a fetch from the API.
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/invite.py` & `discord-py-interactions-5.3.0/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/message.py` & `discord-py-interactions-5.3.0/interactions/models/discord/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import base64
 import re
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncGenerator,
     Dict,
@@ -85,20 +86,30 @@
     """a proxied url of file"""
     height: Optional[int] = attrs.field(repr=False, default=None)
     """height of file (if image)"""
     width: Optional[int] = attrs.field(repr=False, default=None)
     """width of file (if image)"""
     ephemeral: bool = attrs.field(repr=False, default=False)
     """whether this attachment is ephemeral"""
+    duration_secs: Optional[int] = attrs.field(repr=False, default=None)
+    """the duration of the audio file (currently for voice messages)"""
+    waveform: bytearray = attrs.field(repr=False, default=None)
+    """base64 encoded bytearray representing a sampled waveform (currently for voice messages)"""
 
     @property
     def resolution(self) -> tuple[Optional[int], Optional[int]]:
         """Returns the image resolution of the attachment file"""
         return self.height, self.width
 
+    @classmethod
+    def _process_dict(cls, data: Dict[str, Any], _) -> Dict[str, Any]:
+        if waveform := data.pop("waveform", None):
+            data["waveform"] = bytearray(base64.b64decode(waveform))
+        return data
+
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class ChannelMention(DiscordObject):
     guild_id: "Snowflake_Type" = attrs.field(
         repr=False,
     )
     """id of the guild containing the channel"""
@@ -365,14 +376,21 @@
             yield await self._client.cache.fetch_role(self._guild_id, r_id)
 
     @property
     def thread(self) -> "models.TYPE_THREAD_CHANNEL":
         """The thread that was started from this message, if any"""
         return self._client.cache.get_channel(self.id)
 
+    @property
+    def editable(self) -> bool:
+        """Whether this message can be edited by the current user"""
+        if self.author.id == self._client.user.id:
+            return MessageFlags.VOICE_MESSAGE not in self.flags
+        return False
+
     async def fetch_referenced_message(self, *, force: bool = False) -> Optional["Message"]:
         """
         Fetch the message this message is referencing, if any.
 
         Args:
             force: Whether to force a fetch from the API
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/modal.py` & `discord-py-interactions-5.3.0/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/reaction.py` & `discord-py-interactions-5.3.0/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/role.py` & `discord-py-interactions-5.3.0/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/scheduled_event.py` & `discord-py-interactions-5.3.0/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/snowflake.py` & `discord-py-interactions-5.3.0/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/stage_instance.py` & `discord-py-interactions-5.3.0/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/sticker.py` & `discord-py-interactions-5.3.0/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/team.py` & `discord-py-interactions-5.3.0/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/thread.py` & `discord-py-interactions-5.3.0/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/timestamp.py` & `discord-py-interactions-5.3.0/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/user.py` & `discord-py-interactions-5.3.0/interactions/models/discord/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,32 +47,38 @@
 class BaseUser(DiscordObject, _SendDMMixin):
     """Base class for User, essentially partial user discord model."""
 
     username: str = attrs.field(repr=True, metadata=docs("The user's username, not unique across the platform"))
     global_name: str | None = attrs.field(
         repr=True, metadata=docs("The user's chosen display name, platform-wide"), default=None
     )
-    discriminator: int = attrs.field(repr=True, metadata=docs("The user's 4-digit discord-tag"))
+    discriminator: str = attrs.field(
+        repr=True, metadata=docs("The user's 4-digit discord-tag"), default="0"
+    )  # will likely be removed in future api version
     avatar: "Asset" = attrs.field(repr=False, metadata=docs("The user's default avatar"))
 
     def __str__(self) -> str:
         return self.tag
 
     @classmethod
     def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
         if not isinstance(data["avatar"], Asset):
             if data["avatar"]:
                 data["avatar"] = Asset.from_path_hash(client, f"avatars/{data['id']}/{{}}", data["avatar"])
+            elif data["discriminator"] == "0":
+                data["avatar"] = Asset(client, f"{Asset.BASE}/embed/avatars/{(int(data['id']) >> 22) % 5}")
             else:
                 data["avatar"] = Asset(client, f"{Asset.BASE}/embed/avatars/{int(data['discriminator']) % 5}")
         return data
 
     @property
     def tag(self) -> str:
         """Returns the user's Discord tag."""
+        if self.discriminator == "0":
+            return f"@{self.username}"
         return f"{self.username}#{self.discriminator}"
 
     @property
     def mention(self) -> str:
         """Returns a string that would mention the user."""
         return f"<@{self.id}>"
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/user.pyi` & `discord-py-interactions-5.3.0/interactions/models/discord/user.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # and that understands isinstance(member, User) is false
 
 @type_check_only
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)  # properly typehints added attributes by attrs
 class FakeBaseUserMixin(DiscordObject, _SendDMMixin):
     username: str
     global_name: str | None
-    discriminator: int
+    discriminator: str
     avatar: Asset
     def __str__(self) -> str: ...
     @classmethod
     def _process_dict(cls, data: Dict[str, Any], client: Client) -> Dict[str, Any]: ...
     @property
     def tag(self) -> str: ...
     @property
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/voice_state.py` & `discord-py-interactions-5.3.0/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/discord/webhooks.py` & `discord-py-interactions-5.3.0/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/__init__.py` & `discord-py-interactions-5.3.0/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/active_voice_state.py` & `discord-py-interactions-5.3.0/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/annotations/slash.py` & `discord-py-interactions-5.3.0/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/application_commands.py` & `discord-py-interactions-5.3.0/interactions/models/internal/application_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -716,14 +716,15 @@
     ) -> "SlashCommand":
         return SlashCommand(
             name=self.name,
             description=self.description,
             group_name=name,
             group_description=description,
             scopes=self.scopes,
+            default_member_permissions=self.default_member_permissions,
             dm_permission=self.dm_permission,
             checks=self.checks.copy() if inherit_checks else [],
         )
 
     def subcommand(
         self,
         sub_cmd_name: Absent[LocalisedName | str] = MISSING,
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/auto_defer.py` & `discord-py-interactions-5.3.0/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/callback.py` & `discord-py-interactions-5.3.0/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/checks.py` & `discord-py-interactions-5.3.0/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/command.py` & `discord-py-interactions-5.3.0/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/context.py` & `discord-py-interactions-5.3.0/interactions/models/internal/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     process_message_payload,
 )
 from interactions.models.discord.snowflake import Snowflake, Snowflake_Type, to_snowflake, to_optional_snowflake
 from interactions.models.discord.embed import Embed
 from interactions.models.internal.application_commands import (
     OptionType,
     CallbackType,
+    SlashCommandChoice,
     SlashCommandOption,
     InteractionCommand,
 )
 
 __all__ = (
     "AutocompleteContext",
     "BaseContext",
@@ -776,14 +777,24 @@
             message_data = await self.client.http.get_interaction_message(self.client.app.id, self.token)
 
         if message_data:
             message = self.client.cache.place_message_data(message_data)
             self.message_id = message.id
             return message
 
+    @property
+    def component(self) -> typing.Optional[BaseComponent]:
+        """The component that was interacted with."""
+        if self.message is None or self.message.components is None:
+            return None
+        for action_row in self.message.components:
+            for component in action_row.components:
+                if component.custom_id == self.custom_id:
+                    return component
+
 
 class ModalContext(InteractionContext):
     responses: dict[str, str]
     """The responses of the modal. The key is the `custom_id` of the component."""
     custom_id: str
     """The developer defined custom ID of this modal"""
     edit_origin: bool
@@ -848,15 +859,17 @@
         return self.kwargs.get(str(self.focussed_option.name), "")
 
     def option_processing_hook(self, option: dict) -> None:
         if option.get("focused", False):
             self.focussed_option = SlashCommandOption.from_dict(option)
         return
 
-    async def send(self, choices: typing.Iterable[str | int | float | dict[str, int | float | str]]) -> None:
+    async def send(
+        self, choices: typing.Iterable[str | int | float | dict[str, int | float | str] | SlashCommandChoice]
+    ) -> None:
         """
         Send your autocomplete choices to discord. Choices must be either a list of strings, or a dictionary following the following format:
 
         ```json
             {
               "name": str,
               "value": str
@@ -878,14 +891,17 @@
             type_cast = None
 
         processed_choices = []
         for choice in choices:
             if isinstance(choice, dict):
                 name = choice["name"]
                 value = choice["value"]
+            elif isinstance(choice, SlashCommandChoice):
+                name = choice.name
+                value = choice.value
             else:
                 name = str(choice)
                 value = choice
 
             processed_choices.append({"name": name, "value": type_cast(value) if type_cast else value})
 
         payload = {"type": CallbackType.AUTOCOMPLETE_RESULT, "data": {"choices": processed_choices}}
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/converters.py` & `discord-py-interactions-5.3.0/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/cooldowns.py` & `discord-py-interactions-5.3.0/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/extension.py` & `discord-py-interactions-5.3.0/interactions/models/internal/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,29 +97,29 @@
         callables: list[tuple[str, typing.Callable]] = inspect.getmembers(
             instance, predicate=lambda x: isinstance(x, (CallbackObject, Task))
         )
 
         for _name, val in callables:
             if isinstance(val, models.BaseCommand):
                 val.extension = instance
-                val = wrap_partial(val, instance)
+                val = val.copy_with_binding(instance)
                 bot.add_command(val)
                 instance._commands.append(val)
 
             elif isinstance(val, Task):
                 wrap_partial(val, instance)
 
             elif isinstance(val, models.Listener):
                 val.extension = instance
-                val = wrap_partial(val, instance)
+                val = val.copy_with_binding(instance)
                 bot.add_listener(val)  # type: ignore
                 instance._listeners.append(val)
             elif isinstance(val, models.GlobalAutoComplete):
                 val.extension = instance
-                val = wrap_partial(val, instance)
+                val = val.copy_with_binding(instance)
                 bot.add_global_autocomplete(val)
         bot.dispatch(events.ExtensionCommandParse(extension=instance, callables=callables))
 
         instance.extension_name = inspect.getmodule(instance).__name__
         instance.bot.ext[instance.name] = instance
 
         if hasattr(instance, "async_start"):
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/listener.py` & `discord-py-interactions-5.3.0/interactions/models/internal/listener.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,26 +26,31 @@
         self,
         func: AsyncCallable,
         event: str,
         *,
         delay_until_ready: bool = False,
         is_default_listener: bool = False,
         disable_default_listeners: bool = False,
+        pass_event_object: Absent[bool] = MISSING,
     ) -> None:
         super().__init__()
 
         if is_default_listener:
             disable_default_listeners = False
 
         self.event = event
         self.callback = func
         self.delay_until_ready = delay_until_ready
         self.is_default_listener = is_default_listener
         self.disable_default_listeners = disable_default_listeners
 
+        self._params = inspect.signature(func).parameters.copy()
+        self.pass_event_object = pass_event_object
+        self.warned_no_event_arg = False
+
     def __repr__(self) -> str:
         return f"<Listener event={self.event!r} callback={self.callback!r}>"
 
     @classmethod
     def create(
         cls,
         event_name: Absent[str | BaseEvent] = MISSING,
@@ -94,14 +99,25 @@
                 delay_until_ready=delay_until_ready,
                 is_default_listener=is_default_listener,
                 disable_default_listeners=disable_default_listeners,
             )
 
         return wrapper
 
+    def lazy_parse_params(self):
+        """Process the parameters of this listener."""
+        if self.pass_event_object is not MISSING:
+            return
+
+        if self.has_binding:
+            # discard the first parameter, which is the class instance
+            self._params = list(self._params.values())[1:]
+
+        self.pass_event_object = len(self._params) != 0
+
 
 def listen(
     event_name: Absent[str | BaseEvent] = MISSING,
     *,
     delay_until_ready: bool = False,
     is_default_listener: bool = False,
     disable_default_listeners: bool = False,
```

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/localisation.py` & `discord-py-interactions-5.3.0/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/protocols.py` & `discord-py-interactions-5.3.0/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/tasks/task.py` & `discord-py-interactions-5.3.0/interactions/models/internal/tasks/task.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/tasks/triggers.py` & `discord-py-interactions-5.3.0/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/internal/wait.py` & `discord-py-interactions-5.3.0/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/misc/context_manager.py` & `discord-py-interactions-5.3.0/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/interactions/models/misc/iterator.py` & `discord-py-interactions-5.3.0/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/pyproject.toml` & `discord-py-interactions-5.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.2.0"
+version = "5.3.0"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
@@ -25,15 +25,14 @@
 mkdocs-awesome-pages-plugin = { version = "*", optional = true }
 mkdocs-material = { version = "*", optional = true }
 mkdocstrings-python = { version = "*", optional = true }
 mkdocs-minify-plugin = { version = "*", optional = true }
 mkdocs-git-committers-plugin-2 = { version = "*", optional = true }
 mkdocs-git-revision-date-localized-plugin = { version = "*", optional = true }
 pytest = { version = "*", optional = true }
-pytest-recording = { version = "*", optional = true }
 pytest-asyncio = { version = "*", optional = true }
 pytest-cov = { version = "*", optional = true }
 python-dotenv = { version = "*", optional = true }
 typeguard = { version = "*", optional = true }
 pre-commit = { version = "*", optional = true }
 
 [tool.poetry.group.voice.dependencies]
@@ -62,15 +61,14 @@
 mkdocstrings-python = "*"
 mkdocs-minify-plugin = "*"
 mkdocs-git-committers-plugin-2 = "*"
 mkdocs-git-revision-date-localized-plugin = "*"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "*"
-pytest-recording = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 python-dotenv = "*"
 typeguard = "*"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -112,15 +110,15 @@
 
 [tools.coverage.run]
 source = [
     "interactions",
 ]
 
 [tool.pytest.ini_options]
-addopts = "-l -ra --durations=2 --cov=./ --cov-report xml:coverage.xml --junitxml=TestResults.xml"
+addopts = "-l -ra --durations=2 --junitxml=TestResults.xml"
 doctest_optionflags = "NORMALIZE_WHITESPACE"
 asyncio_mode="auto"
 log_cli = "1"
 # log_cli_level = "DEBUG"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format="%Y-%m-%d %H:%M:%S"
```

### Comparing `discord-py-interactions-5.2.0/setup.py` & `discord-py-interactions-5.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     "mkdocstrings-python",
     "mkdocs-minify-plugin",
     "mkdocs-git-committers-plugin-2",
     "mkdocs-git-revision-date-localized-plugin",
 ]
 extras_require["tests"] = [
     "pytest",
-    "pytest-recording",
     "pytest-asyncio",
     "pytest-cov",
     "python-dotenv",
     "typeguard",
 ]
 extras_require["dev"] = extras_require["tests"] + extras_require["docs"] + ["pre-commit"]
```

### Comparing `discord-py-interactions-5.2.0/tests/consts.py` & `discord-py-interactions-5.3.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/tests/test_bot.py` & `discord-py-interactions-5.3.0/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/tests/test_cache.py` & `discord-py-interactions-5.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/tests/test_contexts.py` & `discord-py-interactions-5.3.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/tests/test_cooldowns.py` & `discord-py-interactions-5.3.0/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/tests/test_emoji.py` & `discord-py-interactions-5.3.0/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.2.0/tests/utils.py` & `discord-py-interactions-5.3.0/tests/utils.py`

 * *Files identical despite different names*

