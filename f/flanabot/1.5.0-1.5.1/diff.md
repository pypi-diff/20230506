# Comparing `tmp/flanabot-1.5.0.tar.gz` & `tmp/flanabot-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flanabot-1.5.0.tar", last modified: Wed Jan 11 00:33:10 2023, max compression
+gzip compressed data, was "flanabot-1.5.1.tar", last modified: Sat May  6 18:44:59 2023, max compression
```

## Comparing `flanabot-1.5.0.tar` & `flanabot-1.5.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:33:10.774408 flanabot-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-11 00:32:55.000000 flanabot-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-11 00:33:10.774408 flanabot-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-01-11 00:32:55.000000 flanabot-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:33:10.770408 flanabot-1.5.0/flanabot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:33:10.774408 flanabot-1.5.0/flanabot/bots/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/connect_4_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/flana_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/flana_disc_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/flana_tele_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/penalty_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/poll_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/scraper_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/bots/weather_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/connect_4_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:33:10.774408 flanabot-1.5.0/flanabot/models/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/bot_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/player.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/punishment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/models/weather_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:33:10.774408 flanabot-1.5.0/flanabot/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    82944 2023-01-11 00:32:55.000000 flanabot-1.5.0/flanabot/resources/mucho_texto.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:33:10.770408 flanabot-1.5.0/flanabot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-11 00:33:10.000000 flanabot-1.5.0/flanabot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-01-11 00:33:10.000000 flanabot-1.5.0/flanabot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 00:33:10.000000 flanabot-1.5.0/flanabot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-11 00:33:10.000000 flanabot-1.5.0/flanabot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-11 00:33:10.000000 flanabot-1.5.0/flanabot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-11 00:32:55.000000 flanabot-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-01-11 00:33:10.778408 flanabot-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:44:42.000000 flanabot-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-06 18:44:59.363792 flanabot-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-06 18:44:42.000000 flanabot-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.359792 flanabot-1.5.1/flanabot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/flanabot/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/connect_4_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/flana_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/flana_disc_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/flana_tele_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/penalty_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/poll_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/scraper_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/ubereats_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/weather_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/connect_4_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/flanabot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/bot_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/punishment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/weather_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/flanabot/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    82944 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/resources/mucho_texto.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.359792 flanabot-1.5.1/flanabot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:44:42.000000 flanabot-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-06 18:44:59.367792 flanabot-1.5.1/setup.cfg
```

### Comparing `flanabot-1.5.0/LICENSE` & `flanabot-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.0/PKG-INFO` & `flanabot-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: flanabot
-Version: 1.5.0
+Version: 1.5.1
 Summary: Bot based on https://github.com/AlberLC/multibot to manage Discord, Telegram and Twitch chats, moderate them and add functionalities.
 Home-page: https://github.com/AlberLC/flanabot
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanabot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `flanabot-1.5.0/README.rst` & `flanabot-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.0/flanabot/bots/connect_4_bot.py` & `flanabot-1.5.1/flanabot/bots/connect_4_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,16 +280,16 @@
             edit_kwargs = {'winner': winner, 'loser': loser, 'win_position': (i, j)}
         elif turn >= constants.CONNECT_4_N_ROWS * constants.CONNECT_4_N_COLUMNS:
             edit_kwargs = {'tie': True}
         else:
             return False
 
         try:
-            message.data['is_active'] = False
-        except AttributeError:
+            message.data['connect_4']['is_active'] = False
+        except KeyError:
             pass
 
         await self.edit(
             Media(
                 connect_4_frontend.make_image(board, highlight=(i, j), **edit_kwargs),
                 MediaType.IMAGE,
                 'png',
@@ -444,15 +444,15 @@
 
         if winner := self._check_winner_down_left(i, j, board):
             winners.add(winner)
 
         return winners
 
     def _winning_positions(self, board: list[list[int | None]]) -> defaultdict[int, list[tuple[int, int]]]:
-        winning_positions = defaultdict(list)
+        winning_positions: defaultdict[int, list[tuple[int, int]]] = defaultdict(list)
         for next_i, next_j in self._available_positions(board):
             for player_number in self._check_winners(next_i, next_j, board):
                 winning_positions[player_number].append((next_i, next_j))
 
         return winning_positions
 
     # ---------------------------------------------- #
```

### Comparing `flanabot-1.5.0/flanabot/bots/flana_bot.py` & `flanabot-1.5.1/flanabot/bots/flana_bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,99 @@
 __all__ = ['FlanaBot']
 
+import asyncio
 import datetime
 import random
+import time
 from abc import ABC
 from typing import Iterable
 
 import flanautils
 import pymongo
 import pytz
 from flanaapis import InstagramLoginError, MediaNotFoundError, PlaceNotFoundError
 from flanautils import return_if_first_empty
-from multibot import BadRoleError, MultiBot, Role, bot_mentioned, constants as multibot_constants, group, inline, owner
+from multibot import BadRoleError, MultiBot, RegisteredCallback, Role, User, bot_mentioned, constants as multibot_constants, group, inline, owner
 
 from flanabot import constants
 from flanabot.bots.connect_4_bot import Connect4Bot
 from flanabot.bots.penalty_bot import PenaltyBot
 from flanabot.bots.poll_bot import PollBot
 from flanabot.bots.scraper_bot import ScraperBot
+from flanabot.bots.ubereats_bot import UberEatsBot
 from flanabot.bots.weather_bot import WeatherBot
 from flanabot.models import Action, BotAction, ButtonsGroup, Chat, Message
 
 
 # ----------------------------------------------------------------------------------------------------- #
 # --------------------------------------------- FLANA_BOT --------------------------------------------- #
 # ----------------------------------------------------------------------------------------------------- #
-class FlanaBot(Connect4Bot, PenaltyBot, PollBot, ScraperBot, WeatherBot, MultiBot, ABC):
+class FlanaBot(Connect4Bot, PenaltyBot, PollBot, ScraperBot, UberEatsBot, WeatherBot, MultiBot, ABC):
     Chat = Chat
     Message = Message
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.tunnel_chat = None
+        self.help_calls = {}
+
     # -------------------------------------------------------- #
     # ------------------- PROTECTED METHODS ------------------ #
     # -------------------------------------------------------- #
     def _add_handlers(self):
         super()._add_handlers()
 
+        self.register(self._on_activate_tunnel, (multibot_constants.KEYWORDS['activate'], constants.KEYWORDS['tunnel']))
+
         self.register(self._on_bye, multibot_constants.KEYWORDS['bye'])
 
         self.register(self._on_config, multibot_constants.KEYWORDS['config'])
         self.register(self._on_config, (multibot_constants.KEYWORDS['show'], multibot_constants.KEYWORDS['config']))
 
         self.register(self._on_database_messages, (multibot_constants.KEYWORDS['last'], multibot_constants.KEYWORDS['message']))
+        self.register(lambda message: self._on_database_messages(message, simple=True), (multibot_constants.KEYWORDS['last'], multibot_constants.KEYWORDS['message'], multibot_constants.KEYWORDS['simple']))
 
-        self.register(self._on_database_messages_simple, (multibot_constants.KEYWORDS['last'], multibot_constants.KEYWORDS['message'], multibot_constants.KEYWORDS['simple']))
+        self.register(self._on_deactivate_tunnel, (multibot_constants.KEYWORDS['deactivate'], constants.KEYWORDS['tunnel']))
 
         self.register(self._on_delete, multibot_constants.KEYWORDS['delete'])
         self.register(self._on_delete, (multibot_constants.KEYWORDS['delete'], multibot_constants.KEYWORDS['message']))
 
         self.register(self._on_hello, multibot_constants.KEYWORDS['hello'])
 
+        self.register(self._on_help, multibot_constants.KEYWORDS['help'])
+
         self.register(self._on_new_message_default, default=True)
 
         self.register(self._on_recover_message, multibot_constants.KEYWORDS['reset'])
         self.register(self._on_recover_message, multibot_constants.KEYWORDS['message'])
         self.register(self._on_recover_message, (multibot_constants.KEYWORDS['reset'], multibot_constants.KEYWORDS['message']))
 
         self.register(self._on_roles, multibot_constants.KEYWORDS['permission'])
         self.register(self._on_roles, multibot_constants.KEYWORDS['role'])
         self.register(self._on_roles, (multibot_constants.KEYWORDS['permission'], multibot_constants.KEYWORDS['role']))
         self.register(self._on_roles, (multibot_constants.KEYWORDS['change'], multibot_constants.KEYWORDS['permission']))
         self.register(self._on_roles, (multibot_constants.KEYWORDS['activate'], multibot_constants.KEYWORDS['role']))
         self.register(self._on_roles, (multibot_constants.KEYWORDS['deactivate'], multibot_constants.KEYWORDS['role']))
 
+        self.register(self._on_tunnel_message, always=True)
+
         self.register(self._on_users, multibot_constants.KEYWORDS['user'])
 
         self.register_button(self._on_config_button_press, ButtonsGroup.CONFIG)
         self.register_button(self._on_roles_button_press, ButtonsGroup.ROLES)
         self.register_button(self._on_users_button_press, ButtonsGroup.USERS)
 
     async def _changeable_roles(self, group_: int | str | Chat | Message) -> list[Role]:
         return []
 
     @return_if_first_empty(exclude_self_types='FlanaBot', globals_=globals())
     async def _get_message(
         self,
         event: multibot_constants.MESSAGE_EVENT,
-        pull_overwrite_fields: Iterable[str] = ('_id', 'config')
+        pull_overwrite_fields: Iterable[str] = ('_id', 'config', 'date', 'ubereats')
     ) -> Message:
         return await super()._get_message(event, pull_overwrite_fields)
 
     @return_if_first_empty(exclude_self_types='FlanaBot', globals_=globals())
     async def _manage_exceptions(
         self,
         exceptions: Exception | Iterable[Exception],
@@ -116,37 +131,75 @@
         options.reverse()
 
         return options
 
     # ---------------------------------------------- #
     #                    HANDLERS                    #
     # ---------------------------------------------- #
+    async def _on_activate_tunnel(self, message: Message):
+        keywords = (*multibot_constants.KEYWORDS['activate'], *constants.KEYWORDS['tunnel'])
+        try:
+            chat_id_or_name = next(part for part in flanautils.remove_accents(message.text.lower()).split() if not flanautils.cartesian_product_string_matching(part, keywords, multibot_constants.PARSER_MIN_SCORE_DEFAULT))
+        except StopIteration:
+            return
+
+        chat_id_or_name = flanautils.cast_number(chat_id_or_name, raise_exception=False)
+        if (chat := await self.get_chat(chat_id_or_name)) or (chat := await self.get_chat(await self.get_user(chat_id_or_name))):
+            self.tunnel_chat = chat
+            await self.send(f"Túnel abierto con <b>{chat.name}{f' ({chat.group_name})' if chat.group_name else ''}</b>.", message)
+        else:
+            await self.send_error('Chat inválido.', message)
+
     async def _on_bye(self, message: Message):
         if message.chat.is_private or self.is_bot_mentioned(message):
             await self.send_bye(message)
 
-    @group
-    @bot_mentioned
     async def _on_config(self, message: Message):
-        if not message.chat.config:
+        if message.chat.is_private:
+            config_names = ('auto_insult', 'auto_scraping', 'scraping_delete_original', 'ubereats')
+        elif self.is_bot_mentioned(message):
+            config_names = (
+                'auto_insult',
+                'auto_scraping',
+                'auto_weather_chart',
+                'check_flood',
+                'punish',
+                'scraping_delete_original'
+            )
+        else:
             return
 
-        buttons_texts = [(f"{'✔' if v else '❌'} {k}", v) for k, v in message.chat.config.items()]
+        buttons_texts = []
+        for k, v in message.chat.config.items():
+            if k not in config_names:
+                continue
+            if k == 'ubereats':
+                k = f"ubereats (cada {flanautils.TimeUnits(seconds=message.chat.ubereats['seconds']).to_words()})"
+            buttons_texts.append((f"{'✔' if v else '❌'} {k}", v))
+
         await self.send('<b>Estos son los ajustes del chat:</b>\n\n', flanautils.chunks(buttons_texts, 3), message, buttons_key=ButtonsGroup.CONFIG)
         await self.delete_message(message)
 
     async def _on_config_button_press(self, message: Message):
         await self.accept_button_event(message)
 
-        if message.buttons_info.presser_user.is_admin is False:
+        if message.buttons_info.presser_user.is_admin is False or not message.buttons_info.pressed_button:
             return
 
         config_name = message.buttons_info.pressed_text.split()[1]
         message.chat.config[config_name] = not message.chat.config[config_name]
-        message.buttons_info.pressed_button.text = f"{'✔' if message.chat.config[config_name] else '❌'} {config_name}"
+        if config_name == 'ubereats':
+            if message.chat.config[config_name]:
+                await self.start_ubereats(message.chat)
+            else:
+                await self.stop_ubereats(message.chat)
+            button_text = f"ubereats (cada {flanautils.TimeUnits(seconds=message.chat.ubereats['seconds']).to_words()})"
+        else:
+            button_text = config_name
+        message.buttons_info.pressed_button.text = f"{'✔' if message.chat.config[config_name] else '❌'} {button_text}"
 
         await self.edit(message.buttons_info.buttons, message)
 
     @owner
     async def _on_database_messages(self, message: Message, simple=False):
         if message.chat.is_group and not self.is_bot_mentioned(message):
             return
@@ -159,31 +212,36 @@
             self.get_formatted_last_database_messages(
                 n_messages,
                 timezone=pytz.timezone('Europe/Madrid'),
                 simple=simple
             ),
             message
         )
+        await self.delete_message(message)
 
-    async def _on_database_messages_simple(self, message: Message):
-        await self._on_database_messages(message, simple=True)
+    async def _on_deactivate_tunnel(self, message: Message):
+        self.tunnel_chat = None
+        await self.send('Túnel cerrado.', message)
 
     @inline(False)
     async def _on_delete(self, message: Message):
         if message.replied_message:
-            if message.replied_message.author.id == self.id:
-                await self.delete_message(message.replied_message)
-                if message.chat.is_group:
-                    await self.delete_message(message)
+            if (
+                self.is_bot_mentioned(message)
+                and
+                (message.author.is_admin or message.replied_message.author.id == self.id)
+            ):
+                flanautils.do_later(flanautils.text_to_time(message.text).total_seconds(), self.delete_message, message.replied_message)
+                await self.delete_message(message)
             elif message.chat.is_group and self.is_bot_mentioned(message):
                 await self.send_negative(message)
         elif (
-                (message.chat.is_private or self.is_bot_mentioned(message))
-                and
-                (n_messages := flanautils.text_to_number(message.text))
+            (message.chat.is_private or self.is_bot_mentioned(message))
+            and
+            (n_messages := flanautils.text_to_number(message.text))
         ):
             if message.author.is_admin is False:
                 await self.send_negative(message)
                 return
 
             if n_messages <= 0:
                 await self.delete_message(message)
@@ -191,62 +249,117 @@
 
             await self.clear(n_messages + 1, message.chat)
 
     async def _on_hello(self, message: Message):
         if message.chat.is_private or self.is_bot_mentioned(message):
             await self.send_hello(message)
 
+    async def _on_help(self, message: Message):
+        now = datetime.timedelta(seconds=time.time())
+        if (
+            message.chat.is_group
+            and
+            not self.is_bot_mentioned(message)
+            or
+            self.help_calls.get(message.chat.id)
+            and
+            now - self.help_calls[message.chat.id] <= datetime.timedelta(minutes=1)
+        ):
+            return
+
+        self.help_calls[message.chat.id] = now
+
+        await self.send(
+            '<b>Necesita ayuda:</b>\n'
+            '<b>User:</b>\n'
+            f'    <b>id:</b> <code>{message.author.id}</code>\n'
+            f'    <b>name:</b> <code>{message.author.name}</code>\n'
+            f'    <b>is_admin:<b> <code>{message.author.is_admin}</code>\n'
+            f'    <b>is_bot:</b> <code>{message.author.is_bot}</code>\n'
+            '\n'
+            '<b>Chat:</b>\n'
+            f'    <b>id:</b> <code>{message.chat.id}</code>\n'
+            f'    <b>name:</b> <code>{message.chat.name}</code>\n'
+            f'    <b>group_id:</b> <code>{message.chat.group_id}</code>\n'
+            f'    <b>group_name:</b> <code>{message.chat.group_name}</code>',
+            await self.owner_chat
+        )
+        await self.send('Se ha notificado a Flanagan. Se pondrá en contacto contigo cuando pueda.', message)
+
     async def _on_new_message_default(self, message: Message):
         if message.is_inline:
-            await self._scrape_and_send(message)
+            await self._on_scraping(message)
         elif (
-                (
-                        message.chat.is_group
-                        and
-                        not self.is_bot_mentioned(message)
-                        and
-                        not message.chat.config['auto_scraping']
-                        or
-                        not await self._scrape_send_and_delete(message)
-                )
+            (
+                message.chat.is_group
+                and
+                not self.is_bot_mentioned(message)
+                and
+                not message.chat.config['auto_scraping']
+                or
+                not await self._on_scraping(message, scrape_replied=False)
+            )
+            and
+            message.author.id != self.owner_id
+            and
+            (
+                not message.replied_message
+                or
+                message.replied_message.author.id != self.id
+                or
+                not message.replied_message.medias
+            )
+            and
+            (
+                self.is_bot_mentioned(message)
+                or
+                message.chat.config['auto_insult']
                 and
-                (
-                        message.author.id != self.owner_id
-                        and
-                        (
-                                not message.replied_message
-                                or
-                                message.replied_message.author.id != self.id
-                                or
-                                not message.replied_message.medias
-                        )
-                        and
-                        (
-                                self.is_bot_mentioned(message)
-                                or
-                                (
-                                        message.chat.config['auto_insult']
-                                        and
-                                        random.random() < constants.INSULT_PROBABILITY
-                                )
-                        )
-                )
+                random.random() < constants.INSULT_PROBABILITY
+            )
+            and
+            (
+                not self.tunnel_chat
+                or
+                self.tunnel_chat != message.chat
+            )
         ):
             await self.send_insult(message)
 
     async def _on_ready(self):
         await super()._on_ready()
-        await flanautils.do_every(multibot_constants.CHECK_OLD_DATABASE_MESSAGES_EVERY_SECONDS, self.check_old_database_actions)
+        flanautils.do_every(multibot_constants.CHECK_OLD_DATABASE_MESSAGES_EVERY_SECONDS, self.check_old_database_actions)
+        for chat in Chat.find({
+            'platform': self.platform.value,
+            'config.ubereats': {"$exists": True, "$eq": True},
+            'ubereats.cookies': {"$exists": True, "$ne": []}
+        }):
+            chat = await self.get_chat(chat.id)
+            chat.pull_from_database(overwrite_fields=('_id', 'config', 'ubereats'))
+            if (
+                chat.ubereats['next_execution']
+                and
+                (delta_time := chat.ubereats['next_execution'] - datetime.datetime.now(datetime.timezone.utc)) > datetime.timedelta()
+            ):
+                flanautils.do_later(delta_time, self.start_ubereats, chat)
+            else:
+                await self.start_ubereats(chat)
 
     @inline(False)
     async def _on_recover_message(self, message: Message):
         if message.replied_message and message.replied_message.author.id == self.id:
-            message_deleted_bot_action = BotAction.find_one({'action': Action.MESSAGE_DELETED.value, 'chat': message.chat.object_id, 'affected_objects': message.replied_message.object_id})
+            message_deleted_bot_action = BotAction.find_one({
+                'platform': self.platform.value,
+                'action': Action.MESSAGE_DELETED.value,
+                'chat': message.chat.object_id,
+                'affected_objects': message.replied_message.object_id
+            })
         elif self.is_bot_mentioned(message):
             message_deleted_bot_action = BotAction.find_one({
+                'platform': self.platform.value,
                 'action': Action.MESSAGE_DELETED.value,
                 'chat': message.chat.object_id,
                 'date': {'$gt': datetime.datetime.now(datetime.timezone.utc) - constants.RECOVERY_DELETED_MESSAGE_BEFORE}
             }, sort_keys=(('date', pymongo.DESCENDING),))
         else:
             return
 
@@ -294,14 +407,36 @@
             message.buttons_info.presser_user.roles.append(role)
             user_role_names.append(role.name)
 
         await self.edit(self.distribute_buttons(await self._role_state_options(message, user_role_names), vertically=True), message)
 
         message.buttons_info.presser_user.save()
 
+    async def _on_tunnel_message(self, message: Message):
+        if (
+            not self.tunnel_chat
+            or
+            self._parse_callbacks(
+                message.text,
+                [
+                    RegisteredCallback(..., (multibot_constants.KEYWORDS['activate'], constants.KEYWORDS['tunnel'])),
+                    RegisteredCallback(..., (multibot_constants.KEYWORDS['deactivate'], constants.KEYWORDS['tunnel']))
+                ]
+            )
+        ):
+            return
+
+        if message.chat == self.tunnel_chat:
+            await self.send(f"<b>{message.author.name.split('#')[0]}:</b> {message.text}", await self.owner_chat)
+        elif message.author.id == self.owner_id and message.chat.is_private:
+            if message.text:
+                await self.send(message.text, self.tunnel_chat)
+            else:
+                await self.send('No puedo enviar un mensaje sin texto.', message)
+
     @group
     @bot_mentioned
     async def _on_users(self, message: Message):
         if not (role_names := [role.name for role in await self.get_group_roles(message.chat.group_id)]):
             return
 
         try:
@@ -341,21 +476,24 @@
             message.buttons_info.buttons,
             message
         )
 
     # -------------------------------------------------------- #
     # -------------------- PUBLIC METHODS -------------------- #
     # -------------------------------------------------------- #
-    @staticmethod
-    def check_old_database_actions():
+    def check_old_database_actions(self):
         before_date = datetime.datetime.now(datetime.timezone.utc) - multibot_constants.DATABASE_MESSAGE_EXPIRATION_TIME
-        BotAction.delete_many_raw({'date': {'$lte': before_date}})
-
-    async def send_bye(self, message: Message) -> multibot_constants.ORIGINAL_MESSAGE:
-        return await self.send(random.choice((*constants.BYE_PHRASES, flanautils.CommonWords.random_time_greeting())), message)
-
-    async def send_hello(self, message: Message) -> multibot_constants.ORIGINAL_MESSAGE:
-        return await self.send(random.choice((*constants.HELLO_PHRASES, flanautils.CommonWords.random_time_greeting())), message)
+        BotAction.delete_many_raw({'platform': self.platform.value, 'date': {'$lte': before_date}})
 
-    async def send_insult(self, message: Message) -> multibot_constants.ORIGINAL_MESSAGE | None:
-        await self.typing_delay(message)
-        return await self.send(random.choice(constants.INSULTS), message)
+    async def send_bye(self, chat: int | str | User | Chat | Message) -> multibot_constants.ORIGINAL_MESSAGE:
+        chat = await self.get_chat(chat)
+        return await self.send(random.choice((*constants.BYE_PHRASES, flanautils.CommonWords.random_time_greeting())), chat)
+
+    async def send_hello(self, chat: int | str | User | Chat | Message) -> multibot_constants.ORIGINAL_MESSAGE:
+        chat = await self.get_chat(chat)
+        return await self.send(random.choice((*constants.HELLO_PHRASES, flanautils.CommonWords.random_time_greeting())), chat)
+
+    async def send_insult(self, chat: int | str | User | Chat | Message) -> multibot_constants.ORIGINAL_MESSAGE | None:
+        chat = await self.get_chat(chat)
+        async with await self.typing(chat):
+            await asyncio.sleep(random.randint(1, 3))
+            return await self.send(random.choice(constants.INSULTS), chat)
```

### Comparing `flanabot-1.5.0/flanabot/bots/flana_disc_bot.py` & `flanabot-1.5.1/flanabot/bots/flana_disc_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import random
 
 import discord
 import flanautils
 import pytz
 from flanautils import Media, NotFoundError, OrderedSet
-from multibot import BadRoleError, DiscordBot, Role, User, bot_mentioned, constants as multibot_constants, group
+from multibot import BadRoleError, DiscordBot, Platform, Role, User, bot_mentioned, constants as multibot_constants, group
 
 from flanabot import constants
 from flanabot.bots.flana_bot import FlanaBot
 from flanabot.models import Chat, Message, Punishment
 
 
 # ---------------------------------------------------------------------------------------------------- #
@@ -35,15 +35,16 @@
         self.client.add_listener(self._on_member_remove, 'on_member_remove')
         self.client.add_listener(self._on_voice_state_update, 'on_voice_state_update')
 
         self.register(self._on_audit_log, multibot_constants.KEYWORDS['audit'])
 
     async def _changeable_roles(self, group_: int | str | Chat | Message) -> list[Role]:
         group_id = self.get_group_id(group_)
-        return [role for role in await self.get_group_roles(group_) if role.id in constants.CHANGEABLE_ROLES[group_id]]
+        r = await self.get_group_roles(group_)
+        return [role for role in r if role.id in constants.CHANGEABLE_ROLES[Platform.DISCORD][group_id]]
 
     async def _heat_channel(self, channel: discord.VoiceChannel):
         async def set_fire_to(channel_key: str, depends_on: str, firewall=0):
             fire_score = random.randint(0, channels[depends_on]['n_fires'] - channels[channel_key]['n_fires']) - firewall // 2
             if fire_score < 1:
                 if not channels[channel_key]['n_fires']:
                     return
@@ -56,17 +57,17 @@
             if channels[channel_key]['n_fires']:
                 new_name_ = '🔥' * channels[channel_key]['n_fires']
             else:
                 new_name_ = channels[channel_key]['original_name']
             await channels[channel_key]['object'].edit(name=new_name_)
 
         channels = {}
-        for key in constants.DISCORD_HOT_CHANNEL_IDS:
-            channel_ = flanautils.find(channel.guild.voice_channels, condition=lambda c: c.id == constants.DISCORD_HOT_CHANNEL_IDS[key])
-            channels[key] = {
+        for letter, channel_id in constants.DISCORD_HOT_CHANNEL_IDS.items():
+            channel_ = flanautils.find(channel.guild.voice_channels, condition=lambda c: c.id == channel_id)
+            channels[letter] = {
                 'object': channel_,
                 'original_name': channel_.name,
                 'n_fires': 0
             }
 
         while True:
             await asyncio.sleep(constants.HEAT_PERIOD_SECONDS)
@@ -80,15 +81,18 @@
                 if self.heat_level > len(constants.DISCORD_HEAT_NAMES) - 1:
                     self.heat_level = float(int(self.heat_level))
 
             if not self.heat_level.is_integer():
                 continue
 
             i = int(self.heat_level)
-            if i < len(constants.DISCORD_HEAT_NAMES):
+            if not i:
+                n_fires = 0
+                new_name = channels['C']['original_name']
+            elif i < len(constants.DISCORD_HEAT_NAMES):
                 n_fires = 0
                 new_name = constants.DISCORD_HEAT_NAMES[i]
             else:
                 n_fires = i - len(constants.DISCORD_HEAT_NAMES) + 1
                 n_fires = round(math.log(n_fires + 4, 1.2) - 8)
                 new_name = '🔥' * n_fires
             channels['C']['n_fires'] = n_fires
@@ -109,15 +113,15 @@
             raise BadRoleError(str(self._punish))
 
     async def _search_medias(
         self,
         message: Message,
         force=False,
         audio_only=False,
-        timeout_for_media: int | float = 15
+        timeout_for_media: int | float = constants.SCRAPING_TIMEOUT_SECONDS
     ) -> OrderedSet[Media]:
         return await super()._search_medias(message, force, audio_only, timeout_for_media)
 
     async def _unpunish(self, user: int | str | User, group_: int | str | Chat | Message, message: Message = None):
         user_id = self.get_user_id(user)
         try:
             await self.add_role(user_id, group_, 'Persona')
```

### Comparing `flanabot-1.5.0/flanabot/bots/flana_tele_bot.py` & `flanabot-1.5.1/flanabot/bots/flana_tele_bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 import os
 from typing import Callable
 
 import telethon.tl.functions
 from flanautils import Media, OrderedSet
 from multibot import TelegramBot, find_message, user_client
 
+from flanabot import constants
 from flanabot.bots.flana_bot import FlanaBot
 from flanabot.models import Message
 
 
 # ---------------------------------------------------- #
 # -------------------- DECORATORS -------------------- #
 # ---------------------------------------------------- #
 def whitelisted(func: Callable) -> Callable:
     @functools.wraps(func)
     @find_message
-    async def wrapper(self: FlanaTeleBot, message: Message):
+    async def wrapper(self: FlanaTeleBot, message: Message, *args, **kwargs):
         if message.author.id not in self.whitelist_ids:
             return
 
-        return await func(self, message)
+        return await func(self, message, *args, **kwargs)
 
     return wrapper
 
 
 # ---------------------------------------------------------------------------------------------------- #
 # ------------------------------------------ FLANA_TELE_BOT ------------------------------------------ #
 # ---------------------------------------------------------------------------------------------------- #
@@ -53,15 +54,15 @@
         return [contact.user_id for contact in contacts_data.contacts]
 
     async def _search_medias(
         self,
         message: Message,
         force=False,
         audio_only=False,
-        timeout_for_media: int | float = 15
+        timeout_for_media: int | float = constants.SCRAPING_TIMEOUT_SECONDS
     ) -> OrderedSet[Media]:
         return await super()._search_medias(message, force, audio_only, timeout_for_media)
 
     @user_client
     async def _update_whitelist(self):
         self.whitelist_ids = [self.owner_id, self.id] + await self._get_contacts_ids()
```

### Comparing `flanabot-1.5.0/flanabot/bots/penalty_bot.py` & `flanabot-1.5.1/flanabot/bots/penalty_bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             return
 
         for user in await self._find_users_to_punish(message):
             await self.punish(user, message, flanautils.text_to_time(await self.filter_mention_ids(message.text, message)), message)
 
     async def _on_ready(self):
         await super()._on_ready()
-        await flanautils.do_every(constants.CHECK_PUNISHMENTS_EVERY_SECONDS, self.check_old_punishments)
+        flanautils.do_every(constants.CHECK_PUNISHMENTS_EVERY_SECONDS, self.check_old_punishments)
 
     @bot_mentioned
     @group
     @admin(send_negative=True)
     async def _on_unban(self, message: Message):
         for user in await self._find_users_to_punish(message):
             await self.unban(user, message, message)
```

### Comparing `flanabot-1.5.0/flanabot/bots/poll_bot.py` & `flanabot-1.5.1/flanabot/bots/poll_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.0/flanabot/bots/weather_bot.py` & `flanabot-1.5.1/flanabot/bots/weather_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     # ---------------------------------------------- #
     async def _on_weather(self, message: Message):
         bot_state_message: Message | None = None
         if message.is_inline:
             show_progress_state = False
         elif message.chat.is_group and not self.is_bot_mentioned(message):
             if message.chat.config['auto_weather_chart']:
-                if BotAction.find_one({'action': Action.AUTO_WEATHER_CHART.value, 'chat': message.chat.object_id, 'date': {'$gt': datetime.datetime.now(datetime.timezone.utc) - constants.AUTO_WEATHER_EVERY}}):
+                if BotAction.find_one({'platform': self.platform.value, 'action': Action.AUTO_WEATHER_CHART.value, 'chat': message.chat.object_id, 'date': {'$gt': datetime.datetime.now(datetime.timezone.utc) - constants.AUTO_WEATHER_EVERY}}):
                     return
                 show_progress_state = False
             else:
                 return
         else:
             show_progress_state = True
 
@@ -157,15 +157,15 @@
         await self.send_inline_results(message)
 
         if bot_state_message:
             await self.delete_message(bot_state_message)
 
         if bot_message and not self.is_bot_mentioned(message):
             # noinspection PyTypeChecker
-            BotAction(Action.AUTO_WEATHER_CHART, message, affected_objects=[bot_message]).save()
+            BotAction(self.platform.value, Action.AUTO_WEATHER_CHART, message, affected_objects=[bot_message]).save()
 
     async def _on_weather_button_press(self, message: Message):
         await self.accept_button_event(message)
 
         weather_chart = message.data['weather_chart']
 
         match message.buttons_info.pressed_text:
```

### Comparing `flanabot-1.5.0/flanabot/connect_4_frontend.py` & `flanabot-1.5.1/flanabot/connect_4_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 CIRCLE_RADIUS = 36 * SIZE_MULTIPLIER
 CROSS_LINE_WIDTH = 24 * SIZE_MULTIPLIER
 FONT_SIZE = 32 * SIZE_MULTIPLIER
 TABLE_LINE_WIDTH = 4 * SIZE_MULTIPLIER
 
 BLUE = (66 / 255, 135 / 255, 245 / 255)
-BACKGROUND_COLOR = (54 / 255, 57 / 255, 63 / 255)
+BACKGROUND_COLOR = (49 / 255, 51 / 255, 56 / 255)
 GRAY = (200 / 255, 200 / 255, 200 / 255)
 HIGHLIGHT_COLOR = (104 / 255, 107 / 255, 113 / 255)
 RED = (255 / 255, 70 / 255, 70 / 255)
 PLAYER_1_COLOR = BLUE
 PLAYER_2_COLOR = RED
```

### Comparing `flanabot-1.5.0/flanabot/constants.py` & `flanabot-1.5.1/flanabot/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 AUDIT_LOG_LIMIT = 5
 AUTO_WEATHER_EVERY = datetime.timedelta(hours=6)
 CHECK_PUNISHMENTS_EVERY_SECONDS = datetime.timedelta(hours=1).total_seconds()
 CONNECT_4_AI_DELAY_SECONDS = 1
 CONNECT_4_CENTER_COLUMN_POINTS = 2
 CONNECT_4_N_COLUMNS = 7
 CONNECT_4_N_ROWS = 6
-
 FLOOD_2s_LIMIT = 2
 FLOOD_7s_LIMIT = 4
 HEAT_PERIOD_SECONDS = datetime.timedelta(minutes=15).total_seconds()
+HELP_MINUTES_LIMIT = 1
+INSTAGRAM_BAN_SLEEP = datetime.timedelta(days=1)
 INSULT_PROBABILITY = 0.00166666667
 MAX_PLACE_QUERY_LENGTH = 50
 PUNISHMENT_INCREMENT_EXPONENT = 6
 PUNISHMENTS_RESET_TIME = datetime.timedelta(weeks=2)
 RECOVERY_DELETED_MESSAGE_BEFORE = datetime.timedelta(hours=1)
+SCRAPING_TIMEOUT_SECONDS = 10
 
 BYE_PHRASES = ('Adiós.', 'adio', 'adioh', 'adios', 'adió', 'adiós', 'agur', 'bye', 'byyeeee', 'chao', 'hasta la vista',
                'hasta luego', 'hasta nunca', ' hasta pronto', 'hasta la próxima', 'nos vemos', 'taluego')
 
 CHANGEABLE_ROLES = defaultdict(
     lambda: defaultdict(list),
     {
@@ -34,15 +36,14 @@
                 862823584670285835: [976660580939202610, 984269640752590868]
             }
         )
     }
 )
 
 DISCORD_HEAT_NAMES = [
-    'Canal Congelado',
     'Canal Fresquito',
     'Canal Templaillo',
     'Canal Calentito',
     'Canal Caloret',
     'Canal Caliente',
     'Canal Olor a Vasco',
     'Canal Verano Cordobés al Sol',
@@ -92,20 +93,20 @@
     'multiple_answer': ('multi', 'multi-answer', 'multiple', 'multirespuesta'),
     'poll': ('encuesta', 'quiz'),
     'punish': ('acaba', 'aprende', 'ataca', 'atalo', 'azota', 'beating', 'boss', 'castiga', 'castigo', 'condena',
                'controla', 'destroy', 'destroza', 'duro', 'ejecuta', 'enseña', 'escarmiento', 'execute', 'fuck',
                'fusila', 'hell', 'humos', 'infierno', 'jefe', 'jode', 'learn', 'leccion', 'lesson', 'manda', 'paliza',
                'purgatorio', 'purgatory', 'sancion', 'shoot', 'teach', 'whip'),
     'random': ('aleatorio', 'azar', 'random'),
-    'scraping': ('api', 'aqui', 'busca', 'contenido', 'content', 'descarga', 'descargar', 'download', 'envia', 'habia',
-                 'media', 'redes', 'scrap', 'scraping', 'search', 'send', 'social', 'sociales', 'tenia', 'video',
-                 'videos'),
+    'scraping': ('busca', 'contenido', 'content', 'descarga', 'descargar', 'descargues', 'download', 'envia', 'scrap',
+                 'scrapea', 'scrapees', 'scraping', 'search', 'send'),
     'self': (('contigo', 'contra', 'ti'), ('mismo', 'ti')),
-    'song_info': ('aqui', 'cancion', 'data', 'datos', 'info', 'informacion', 'information', 'llama', 'media', 'name',
-                  'nombre', 'sonaba', 'sonando', 'song', 'sono', 'sound', 'suena', 'title', 'titulo', 'video'),
+    'song_info': ('cancion', 'data', 'datos', 'info', 'informacion', 'information', 'sonaba', 'sonando', 'song', 'sono',
+                  'sound', 'suena'),
+    'tunnel': ('canal', 'channel', 'tunel', 'tunnel'),
     'unpunish': ('absolve', 'forgive', 'innocent', 'inocente', 'perdona', 'spare'),
     'vote': ('votacion', 'votar', 'vote', 'voting', 'voto'),
     'weather': ('atmosfera', 'atmosferico', 'calle', 'calor', 'caloret', 'clima', 'climatologia', 'cloud', 'cloudless',
                 'cloudy', 'cold', 'congelar', 'congelado', 'denbora', 'despejado', 'diluvio', 'frio', 'frost', 'hielo',
                 'humedad', 'llover', 'llueva', 'llueve', 'lluvia', 'nevada', 'nieva', 'nieve', 'nube', 'nubes',
                 'nublado', 'meteorologia', 'rain', 'snow', 'snowfall', 'snowstorm', 'sol', 'solano', 'storm', 'sun',
                 'temperatura', 'tempo', 'tiempo', 'tormenta', 'ventisca', 'weather', 'wetter')
```

### Comparing `flanabot-1.5.0/flanabot/models/bot_action.py` & `flanabot-1.5.1/flanabot/models/bot_action.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 __all__ = ['BotAction']
 
 import datetime
 from dataclasses import dataclass, field
 
 from flanautils import DCMongoBase, FlanaBase
-from multibot.models.user import User
+from multibot import Platform, User
 
 from flanabot.models.chat import Chat
 from flanabot.models.enums import Action
 from flanabot.models.message import Message
 
 
 @dataclass(eq=False)
 class BotAction(DCMongoBase, FlanaBase):
     collection_name = 'bot_action'
     unique_keys = 'message'
     nullable_unique_keys = 'message'
 
+    platform: Platform = None
     action: Action = None
     message: Message = None
     author: User = None
     chat: Chat = None
     affected_objects: list = field(default_factory=list)
     date: datetime.datetime = field(default_factory=datetime.datetime.now)
```

### Comparing `flanabot-1.5.0/flanabot/models/message.py` & `flanabot-1.5.1/flanabot/models/message.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.0/flanabot/models/weather_chart.py` & `flanabot-1.5.1/flanabot/models/weather_chart.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.0/flanabot/resources/mucho_texto.png` & `flanabot-1.5.1/flanabot/resources/mucho_texto.png`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.0/flanabot.egg-info/PKG-INFO` & `flanabot-1.5.1/flanabot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: flanabot
-Version: 1.5.0
+Version: 1.5.1
 Summary: Bot based on https://github.com/AlberLC/multibot to manage Discord, Telegram and Twitch chats, moderate them and add functionalities.
 Home-page: https://github.com/AlberLC/flanabot
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanabot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `flanabot-1.5.0/flanabot.egg-info/SOURCES.txt` & `flanabot-1.5.1/flanabot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 flanabot/bots/connect_4_bot.py
 flanabot/bots/flana_bot.py
 flanabot/bots/flana_disc_bot.py
 flanabot/bots/flana_tele_bot.py
 flanabot/bots/penalty_bot.py
 flanabot/bots/poll_bot.py
 flanabot/bots/scraper_bot.py
+flanabot/bots/ubereats_bot.py
 flanabot/bots/weather_bot.py
 flanabot/models/__init__.py
 flanabot/models/bot_action.py
 flanabot/models/chat.py
 flanabot/models/enums.py
 flanabot/models/message.py
 flanabot/models/player.py
```

### Comparing `flanabot-1.5.0/setup.cfg` & `flanabot-1.5.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [metadata]
 name = flanabot
-version = v1.5.0
+version = v1.5.1
 author = AlberLC
-author_email = alberlc@outlook.com
 description = Bot based on https://github.com/AlberLC/multibot to manage Discord, Telegram and Twitch chats, moderate them and add functionalities.
 long_description = file: README.rst
 url = https://github.com/AlberLC/flanabot
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/flanabot/issues
 classifiers = 
 	Programming Language :: Python :: 3.10
```

