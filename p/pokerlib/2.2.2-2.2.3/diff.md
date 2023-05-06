# Comparing `tmp/pokerlib-2.2.2.tar.gz` & `tmp/pokerlib-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerlib-2.2.2.tar", max compression
+gzip compressed data, was "pokerlib-2.2.3.tar", max compression
```

## Comparing `pokerlib-2.2.2.tar` & `pokerlib-2.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.2/LICENSE
--rw-r--r--   0        0        0     6276 2023-05-02 19:42:40.871493 pokerlib-2.2.2/README.md
--rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.2/pokerlib/__init__.py
--rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/_handparser.py
--rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/_player.py
--rw-r--r--   0        0        0    17675 2023-05-05 19:27:14.959085 pokerlib-2.2.2/pokerlib/_round.py
--rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.2/pokerlib/_table.py
--rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/enums.py
--rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/implementations/__init__.py
--rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/implementations/_no_muck_showdown_table.py
--rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.2/pokerlib/implementations/_no_muck_table.py
--rw-r--r--   0        0        0      663 2023-05-05 19:32:10.249004 pokerlib-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     7001 1970-01-01 00:00:00.000000 pokerlib-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.3/LICENSE
+-rw-r--r--   0        0        0     5980 2023-05-05 21:16:26.697525 pokerlib-2.2.3/README.md
+-rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.3/pokerlib/__init__.py
+-rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/_handparser.py
+-rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/_player.py
+-rw-r--r--   0        0        0    17750 2023-05-06 18:50:56.359624 pokerlib-2.2.3/pokerlib/_round.py
+-rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.3/pokerlib/_table.py
+-rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/enums.py
+-rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/implementations/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/implementations/_no_muck_showdown_table.py
+-rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.3/pokerlib/implementations/_no_muck_table.py
+-rw-r--r--   0        0        0      663 2023-05-06 18:52:00.259619 pokerlib-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 pokerlib-2.2.3/PKG-INFO
```

### Comparing `pokerlib-2.2.2/LICENSE` & `pokerlib-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.2/README.md` & `pokerlib-2.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -135,27 +135,32 @@
 table.publicIn(player2.id, RoundPublicInId.CHECK)
 table.publicIn(player1.id, RoundPublicInId.ALLIN)
 table.publicIn(player2.id, RoundPublicInId.CALL)
 ```
 
 Wrong inputs are mostly ignored, though they can produce a response, when it seems useful. As noted before, when providing input, the `table` object responds with output ids (e.g. `PLAYERACTIONREQUIRED`) along with additional data that depends on the output id. For all possible outputs, check `RoundPublicInId` and `TablePublicInId` enums.
 
-A new round has to be initiated by one of the players every time the previous one ends (or at the beginning). A simple command line game, where you respond by enum names, can be implemented simply as in `examples/round_simulate.py`.
+A simple command line game, where you respond with enum names, can be implemented simply as in `examples/round_simulate.py`. Command
+```bash
+python examples/round_simulate.py 3
+```
+runs a poker game with 3 players using the terminal as IO. Note that responses are in non-formatted raw form.
 
-The library is highly customizable, allowing you to override specific class methods such as `_showdown` that let you define the way that cards get shown (see `pokerlib/implementations/_no_muck_showdown_table.py`). The IO identifiers can also be extended or reduced and set either as `Table` or `Round` class attributes.
 
 ## Tests
-Basic tests for this library are included. You can test HandParser by running
+Basic tests for this library are included. You can test `HandParser` by running
 ```bash
 python tests/handparser_reactive.py
 ```
-initiate a poker round simulation with
+and `Round` with
 ```bash
-python tests/round_test.py <number_of_players>
+python tests/round_test.py
 ```
-which will run a poker game simulation with raw data getting printed to stdout. The HandParser functionality was also tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface). You can run those tests with
+Note that HandParser can be fuzz tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface) with
+Those tests can be run with
 ```bash
 python tests/handparser_against_pokerface.py
 ```
+which means it is considered safe. On the other hand, `Table` may still have some bugs.
 
 ## License
 GNU General Public License v3.0
```

### Comparing `pokerlib-2.2.2/pokerlib/_handparser.py` & `pokerlib-2.2.3/pokerlib/_handparser.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.2/pokerlib/_player.py` & `pokerlib-2.2.3/pokerlib/_player.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.2/pokerlib/_round.py` & `pokerlib-2.2.3/pokerlib/_round.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,16 @@
         self._executeAction(action, raise_by)
         self.current_player.played_turn = True
         self._postActionStateUpdate()
 
     def _finish(self):
         self.finished = True
         self.publicOut(self.PublicOutId.ROUNDFINISHED)
+        if self._muck_optioned_player_ids == []:
+            self._close()
 
     def _close(self):
         self.closed = True
         self.publicOut(self.PublicOutId.ROUNDCLOSED)
 
     def publicIn(self, player_id, action, **kwargs):
         """Processes invalidated user input"""
```

### Comparing `pokerlib-2.2.2/pokerlib/_table.py` & `pokerlib-2.2.3/pokerlib/_table.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.2/pokerlib/enums.py` & `pokerlib-2.2.3/pokerlib/enums.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.2/pyproject.toml` & `pokerlib-2.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokerlib"
-version = "2.2.2"
+version = "2.2.3"
 description = "Python poker library"
 repository = "https://github.com/kuco23/pokerlib/"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 keywords = ['python', 'poker', 'library']
 readme = "README.md"
 classifiers=  [
     'Development Status :: 3 - Alpha',
```

### Comparing `pokerlib-2.2.2/PKG-INFO` & `pokerlib-2.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerlib
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python poker library
 Home-page: https://github.com/kuco23/pokerlib/
 Keywords: python,poker,library
 Author: kuco23
 Author-email: nseverkar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -155,28 +155,33 @@
 table.publicIn(player2.id, RoundPublicInId.CHECK)
 table.publicIn(player1.id, RoundPublicInId.ALLIN)
 table.publicIn(player2.id, RoundPublicInId.CALL)
 ```
 
 Wrong inputs are mostly ignored, though they can produce a response, when it seems useful. As noted before, when providing input, the `table` object responds with output ids (e.g. `PLAYERACTIONREQUIRED`) along with additional data that depends on the output id. For all possible outputs, check `RoundPublicInId` and `TablePublicInId` enums.
 
-A new round has to be initiated by one of the players every time the previous one ends (or at the beginning). A simple command line game, where you respond by enum names, can be implemented simply as in `examples/round_simulate.py`.
+A simple command line game, where you respond with enum names, can be implemented simply as in `examples/round_simulate.py`. Command
+```bash
+python examples/round_simulate.py 3
+```
+runs a poker game with 3 players using the terminal as IO. Note that responses are in non-formatted raw form.
 
-The library is highly customizable, allowing you to override specific class methods such as `_showdown` that let you define the way that cards get shown (see `pokerlib/implementations/_no_muck_showdown_table.py`). The IO identifiers can also be extended or reduced and set either as `Table` or `Round` class attributes.
 
 ## Tests
-Basic tests for this library are included. You can test HandParser by running
+Basic tests for this library are included. You can test `HandParser` by running
 ```bash
 python tests/handparser_reactive.py
 ```
-initiate a poker round simulation with
+and `Round` with
 ```bash
-python tests/round_test.py <number_of_players>
+python tests/round_test.py
 ```
-which will run a poker game simulation with raw data getting printed to stdout. The HandParser functionality was also tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface). You can run those tests with
+Note that HandParser can be fuzz tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface) with
+Those tests can be run with
 ```bash
 python tests/handparser_against_pokerface.py
 ```
+which means it is considered safe. On the other hand, `Table` may still have some bugs.
 
 ## License
 GNU General Public License v3.0
```

