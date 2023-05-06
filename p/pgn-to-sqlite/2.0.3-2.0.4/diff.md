# Comparing `tmp/pgn_to_sqlite-2.0.3.tar.gz` & `tmp/pgn_to_sqlite-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_to_sqlite-2.0.3.tar", last modified: Thu Oct 27 23:41:20 2022, max compression
+gzip compressed data, was "pgn_to_sqlite-2.0.4.tar", last modified: Sat May  6 01:28:32 2023, max compression
```

## Comparing `pgn_to_sqlite-2.0.3.tar` & `pgn_to_sqlite-2.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       54 2022-10-27 23:41:16.669255 pgn_to_sqlite-2.0.3/.coveragerc
--rw-r--r--   0        0        0      620 2022-10-27 23:41:16.669255 pgn_to_sqlite-2.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      609 2022-10-27 23:41:16.669255 pgn_to_sqlite-2.0.3/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0       77 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/.gitignore
--rw-r--r--   0        0        0     1078 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/LICENSE
--rw-r--r--   0        0        0     3058 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/README.md
--rw-r--r--   0        0        0      111 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/pgn_to_sqlite/__init__.py
--rw-r--r--   0        0        0     8087 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/pgn_to_sqlite/cli.py
--rw-r--r--   0        0        0      850 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      155 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/pytest.ini
--rw-r--r--   0        0        0      255 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/requirements.in
--rw-r--r--   0        0        0    21525 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/tests/__init__.py
--rw-r--r--   0        0        0      506 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/tests/game_files/test_pgn_file_chess_dotcom.pgn
--rw-r--r--   0        0        0      885 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/tests/game_files/test_pgn_file_lichess.pgn
--rw-r--r--   0        0        0     1368 2022-10-27 23:41:16.673256 pgn_to_sqlite-2.0.3/tests/test_cli.py
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.coveragerc
+-rw-r--r--   0        0        0      620 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      694 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0       84 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/.gitignore
+-rw-r--r--   0        0        0     1078 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/LICENSE
+-rw-r--r--   0        0        0     2867 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/README.md
+-rw-r--r--   0        0        0      111 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pgn_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     8071 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pgn_to_sqlite/cli.py
+-rw-r--r--   0        0        0      896 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/pytest.ini
+-rw-r--r--   0        0        0      265 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/requirements.in
+-rw-r--r--   0        0        0    22534 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      506 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/game_files/test_pgn_file_chess_dotcom.pgn
+-rw-r--r--   0        0        0      885 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/game_files/test_pgn_file_lichess.pgn
+-rw-r--r--   0        0        0     1369 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tests/test_cli.py
+-rw-r--r--   0        0        0      159 2023-05-06 01:28:23.596881 pgn_to_sqlite-2.0.4/tox.ini
+-rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.0.4/PKG-INFO
```

### Comparing `pgn_to_sqlite-2.0.3/.github/workflows/publish.yml` & `pgn_to_sqlite-2.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.3/LICENSE` & `pgn_to_sqlite-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.3/README.md` & `pgn_to_sqlite-2.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -70,28 +70,16 @@
 
 If you find a bug, please file an [issue](https://github.com/EndlessTrax/pgn-to-sqlite/issues).
 
 If you have feature requests, please [file an issue](https://github.com/EndlessTrax/pgn-to-sqlite/issues) and use the appropriate label.
 
 Please **raise an issue before making a PR**, so that the issue and implementation can be discussed before you write any code. This will save you time, and increase the chances of your PR being merged without significant changes.
 
-Please **format you code** with [Black](https://pypi.org/project/black/).
+Please **format you code** with [Black](https://pypi.org/project/black/) and [isort](https://pypi.org/project/isort/).
 
 Please **include tests** for any PR's that include code (unless current tests cover your code contribution).
 
 ## Support
 
 If you would like to show your support for the project, I would be very grateful if you would donate to a charity close to my heart, [Walk AS One](https://walkasone.org/donate).
 
 And if you would prefer to donate to me personally instead, [you can sponsor me on Github](https://github.com/sponsors/EndlessTrax)? 🤓
-
-## Changelog
-
-### 2.0
-
-- Breaking changes to CLI commands
-- Added ability to add games from locally saved `.pgn` files to the output database
-
-### 1.0
-
-- Fetch games from _chess.com_ and _lichess.org_
-- Saves games to SQlite3 database
```

### Comparing `pgn_to_sqlite-2.0.3/pgn_to_sqlite/cli.py` & `pgn_to_sqlite-2.0.4/pgn_to_sqlite/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,27 +34,31 @@
         print("INFO:    Connection to DB successful")
     except sqlite3.Error as e:
         print(f"ERROR:   The error '{e}' occurred")
 
     return connection
 
 
-def execute_db_query(connection, query: str) -> None:
+def execute_db_query(connection, query: str, values: tuple = None) -> None:
     """Executes a SQL query on the Sqlite3 database
 
     Args:
         connection: A database connection object
         query: The SQL query as a string
+        values: A tuple of values to be inserted into the query
 
     Returns:
         Nothing.
     """
     cursor = connection.cursor()
     try:
-        cursor.execute(query)
+        if values:
+            cursor.execute(query, values)
+        else:
+            cursor.execute(query)
         connection.commit()
     except sqlite3.Error as e:
         print(f"The error '{e}' occurred")
 
 
 def save_game_to_db(connection, pgn: dict) -> None:
     """Saves a Game to the Sqlite3 database
@@ -62,50 +66,37 @@
     Args:
         connection: A database connection object
         pgn: A PGN dictionary representation
 
     Returns:
         Nothing.
     """
+
     execute_db_query(
         connection,
-        f"""INSERT INTO
-        games (
-            event,
-            site,
-            date,
-            round,
-            white,
-            black,
-            result,
-            eco,
-            white_elo,
-            black_elo,
-            variant,
-            time_control,
-            termination,
-            moves)
-        VALUES
+        """INSERT INTO
+        games(event, site, date, round, white, black, result, eco, white_elo,
+        black_elo, variant, time_control, termination, moves) 
+        VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);""",
         (
-            '{pgn["event"]}',
-            '{pgn["site"]}',
-            '{pgn["date"]}',
-            '{pgn["round"]}',
-            '{pgn["white"]}',
-            '{pgn["black"]}',
-            '{pgn["result"]}',
-            '{pgn["eco"]}',
-            '{pgn["white_elo"]}',
-            '{pgn["black_elo"]}',
-            '{pgn["variant"]}',
-            '{pgn["time_control"]}',
-            '{pgn["termination"]}',
-            '{pgn["moves"]}'
-        );
-        """,
+            pgn["event"],
+            pgn["site"],
+            pgn["date"],
+            pgn["round"],
+            pgn["white"],
+            pgn["black"],
+            pgn["result"],
+            pgn["eco"],
+            pgn["white_elo"],
+            pgn["black_elo"],
+            pgn["variant"],
+            pgn["time_control"],
+            pgn["termination"],
+            pgn["moves"],
+        ),
     )
 
 
 def fetch_chess_dotcom_games(user: str) -> list:
     """Uses the chess.com API to fetch the requested users games.
 
     Args:
```

### Comparing `pgn_to_sqlite-2.0.3/pyproject.toml` & `pgn_to_sqlite-2.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 home-page = "https://github.com/EndlessTrax/pgn-to-sqlite"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ] 
 description-file = "README.md"
 requires = [
     "click",
     "requests",
     "berserk"
 ]
```

### Comparing `pgn_to_sqlite-2.0.3/requirements.txt` & `pgn_to_sqlite-2.0.4/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 attrs==22.1.0 \
     --hash=sha256:29adc2665447e5191d0e7c568fde78b21f9672d344281d0c6e1ab085429b22b6 \
     --hash=sha256:86efa402f67bf2df34f51a335487cf46b1ec130d02b8d39fd248abfd30da551c
     # via pytest
 berserk==0.10.0 \
     --hash=sha256:0ef813bacbbd3cf2c905ac146a06a9e3934b4bbbe500bced6560bdf9fc5dfd60 \
     --hash=sha256:ce61951f22bd8997628acb70dada035c69aa8815beb604919b28d6fda8828ca5
-    # via -r .\requirements.in
+    # via -r requirements.in
 black==22.10.0 \
     --hash=sha256:14ff67aec0a47c424bc99b71005202045dc09270da44a27848d534600ac64fc7 \
     --hash=sha256:197df8509263b0b8614e1df1756b1dd41be6738eed2ba9e9769f3880c2b9d7b6 \
     --hash=sha256:1e464456d24e23d11fced2bc8c47ef66d471f845c7b7a42f3bd77bf3d1789650 \
     --hash=sha256:2039230db3c6c639bd84efe3292ec7b06e9214a2992cd9beb293d639c6402edb \
     --hash=sha256:21199526696b8f09c3997e2b4db8d0b108d801a348414264d2eb8eb2532e540d \
     --hash=sha256:2644b5d63633702bc2c5f3754b1b475378fbbfb481f62319388235d0cd104c2d \
@@ -30,35 +30,29 @@
     --hash=sha256:9311e99228ae10023300ecac05be5a296f60d2fd10fff31cf5c1fa4ca4b1988d \
     --hash=sha256:974308c58d057a651d182208a484ce80a26dac0caef2895836a92dd6ebd725e0 \
     --hash=sha256:b8b49776299fece66bffaafe357d929ca9451450f5466e997a7285ab0fe28e3b \
     --hash=sha256:c957b2b4ea88587b46cf49d1dc17681c1e672864fd7af32fc1e9664d572b3458 \
     --hash=sha256:e41a86c6c650bcecc6633ee3180d80a025db041a8e2398dcc059b3afa8382cd4 \
     --hash=sha256:f513588da599943e0cde4e32cc9879e825d58720d6557062d1098c5ad80080e1 \
     --hash=sha256:fba8a281e570adafb79f7755ac8721b6cf1bbf691186a287e990c7929c7692ff
-    # via -r .\requirements.in
-certifi==2022.9.24 \
-    --hash=sha256:0d9c601124e5a6ba9712dbc60d9c53c21e34f5f641fe83002317394311bdce14 \
-    --hash=sha256:90c1a32f1d68f940488354e36370f6cca89f0f106db09518524c88d6ed83f382
+    # via -r requirements.in
+certifi==2022.12.7 \
+    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
+    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
     # via requests
 charset-normalizer==2.1.1 \
     --hash=sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845 \
     --hash=sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via
-    #   -r .\requirements.in
+    #   -r requirements.in
     #   black
-colorama==0.4.6 \
-    --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
-    --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-    # via
-    #   click
-    #   pytest
 coverage[toml]==6.5.0 \
     --hash=sha256:027018943386e7b942fa832372ebc120155fd970837489896099f5cfa2890f79 \
     --hash=sha256:11b990d520ea75e7ee8dcab5bc908072aaada194a794db9f6d7d5cfd19661e5a \
     --hash=sha256:12adf310e4aafddc58afdb04d686795f33f4d7a6fa67a7a9d4ce7d6ae24d949f \
     --hash=sha256:1431986dac3923c5945271f169f59c45b8802a114c8f548d611f2015133df77a \
     --hash=sha256:1ef221513e6f68b69ee9e159506d583d31aa3567e0ae84eaad9d6ec1107dddaa \
     --hash=sha256:20c8ac5386253717e5ccc827caad43ed66fea0efe255727b1053a8154d952398 \
@@ -107,85 +101,105 @@
     --hash=sha256:f642e90754ee3e06b0e7e51bce3379590e76b7f76b708e1a71ff043f87025c84 \
     --hash=sha256:fc2af30ed0d5ae0b1abdb4ebdce598eafd5b35397d4d75deb341a614d333d987
     # via pytest-cov
 deprecated==1.2.13 \
     --hash=sha256:43ac5335da90c31c24ba028af536a91d41d53f9e6901ddb021bcc572ce44e38d \
     --hash=sha256:64756e3e14c8c5eea9795d93c524551432a0be75629f8f29e67ab8caf076c76d
     # via berserk
+distlib==0.3.6 \
+    --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
+    --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
+    # via virtualenv
 docutils==0.19 \
     --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
     --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
     # via flit
-exceptiongroup==1.0.0 \
-    --hash=sha256:2ac84b496be68464a2da60da518af3785fff8b7ec0d090a581604bc870bdee41 \
-    --hash=sha256:affbabf13fb6e98988c38d9c5650e701569fe3c1de3233cfb61c5f33774690ad
-    # via pytest
+filelock==3.8.0 \
+    --hash=sha256:55447caa666f2198c5b6b13a26d2084d26fa5b115c00d065664b2124680c4edc \
+    --hash=sha256:617eb4e5eedc82fc5f47b6d61e4d11cb837c56cb4544e39081099fa17ad109d4
+    # via
+    #   tox
+    #   virtualenv
 flit==3.7.1 \
     --hash=sha256:06a93a6737fa9380ba85fe8d7f28efb6c93c4f4ee9c7d00cc3375a81f33b91a4 \
     --hash=sha256:3c9bd9c140515bfe62dd938c6610d10d6efb9e35cc647fc614fe5fb3a5036682
-    # via -r .\requirements.in
+    # via -r requirements.in
 flit-core==3.7.1 \
     --hash=sha256:14955af340c43035dbfa96b5ee47407e377ee337f69e70f73064940d27d0a44f \
     --hash=sha256:e454fdbf68c7036e1c7435ec7479383f9d9a1650ca5b304feb184eba1efcdcef
     # via flit
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 importlib-metadata==5.0.0 \
     --hash=sha256:da31db32b304314d044d3c12c79bd59e307889b287ad12ff387b3500835fc2ab \
     --hash=sha256:ddb0e35065e8938f867ed4928d0ae5bf2a53b7773871bfe6bcc7e4fcdc7dea43
-    # via -r .\requirements.in
+    # via -r requirements.in
 iniconfig==1.1.1 \
     --hash=sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3 \
     --hash=sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32
     # via pytest
+isort==5.10.1 \
+    --hash=sha256:6f62d78e2f89b4500b080fe3a81690850cd254227f27f75c3a0c491a1f351ba7 \
+    --hash=sha256:e8443a5e7a020e9d7f97f1d7d9cd17c88bcb3bc7e218bf9cf5095fe550be2951
+    # via -r requirements.in
 mypy-extensions==0.4.3 \
     --hash=sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d \
     --hash=sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8
     # via black
 ndjson==0.3.1 \
     --hash=sha256:839c22275e6baa3040077b83c005ac24199b94973309a8a1809be962c753a410 \
     --hash=sha256:bf9746cb6bb1cb53d172cda7f154c07c786d665ff28341e4e689b796b229e5d6
     # via berserk
 packaging==21.3 \
     --hash=sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb \
     --hash=sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522
-    # via pytest
+    # via
+    #   pytest
+    #   tox
 pathspec==0.10.1 \
     --hash=sha256:46846318467efc4556ccfd27816e004270a9eeeeb4d062ce5e6fc7a87c573f93 \
     --hash=sha256:7ace6161b621d31e7902eb6b5ae148d12cfd23f4a249b9ffb6b9fee12084323d
     # via black
 platformdirs==2.5.2 \
     --hash=sha256:027d8e83a2d7de06bbac4e5ef7e023c02b863d7ea5d079477e722bb41ab25788 \
     --hash=sha256:58c8abb07dcb441e6ee4b11d8df0ac856038f944ab98b7be6b27b2a3c7feef19
-    # via black
+    # via
+    #   black
+    #   virtualenv
 pluggy==1.0.0 \
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
-    # via pytest
+    # via
+    #   pytest
+    #   tox
+py==1.11.0 \
+    --hash=sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719 \
+    --hash=sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378
+    # via tox
 pyparsing==3.0.9 \
     --hash=sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb \
     --hash=sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc
     # via packaging
 pytest==7.2.0 \
     --hash=sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71 \
     --hash=sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59
     # via
-    #   -r .\requirements.in
+    #   -r requirements.in
     #   pytest-cov
 pytest-cov==4.0.0 \
     --hash=sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b \
     --hash=sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470
-    # via -r .\requirements.in
+    # via -r requirements.in
 requests==2.28.1 \
     --hash=sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983 \
     --hash=sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349
     # via
-    #   -r .\requirements.in
+    #   -r requirements.in
     #   berserk
     #   flit
 ruff==0.0.86 \
     --hash=sha256:0da330ff6d0a993d9a2fd86792600676b63be2a82fbe1d8dddb5971ceec51838 \
     --hash=sha256:17738ac99d7a7ba09a1907d15c48e80dcdf616744f1557ef8abb773353bee2c3 \
     --hash=sha256:303cf504981c2b340511f0897966dfdfd8c8dbd8c1ed4106be592b969836d8e6 \
     --hash=sha256:323ab3bb65c71994511fc4bdb173a41337cff912b944a39ae9d7ac00df4cb600 \
@@ -197,27 +211,31 @@
     --hash=sha256:80b8a74a4a9b937fe4f38cbda1dab94c1184ebc49834006763546c0076b7e8ff \
     --hash=sha256:88faa1275197f6b01dd91a575b8c9afb2cc72fd7d6fc16b386adc4197bba4b3a \
     --hash=sha256:9315bfa2f8d93155778f2802390dbb82dd84f7665bbde01a4abed2b3e43c2d82 \
     --hash=sha256:b62444fe116e3b9cdaa9f7bdc9a8cd4e169d9df4bedc3ba52acb089ad19f2080 \
     --hash=sha256:b96aca791d0eef857f631514e96f5c1ebaf729c009865271a32717bb635013a8 \
     --hash=sha256:f23403f2cad4ed6a53f5c790df6b9eb936d55687cb2cc1251a39285bdb3866b9 \
     --hash=sha256:f8de9d89e9fedb272c5694bade256ca2842550845ede96480ec611bde0627373
-    # via -r .\requirements.in
+    # via -r requirements.in
+six==1.16.0 \
+    --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
+    --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
+    # via tox
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-    # via
-    #   black
-    #   coverage
-    #   flit
-    #   pytest
+    # via flit
 tomli-w==1.0.0 \
     --hash=sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463 \
     --hash=sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9
     # via flit
+tox==3.27.0 \
+    --hash=sha256:89e4bc6df3854e9fc5582462e328dd3660d7d865ba625ae5881bbc63836a6324 \
+    --hash=sha256:d2c945f02a03d4501374a3d5430877380deb69b218b1df9b7f1d2f2a10befaf9
+    # via -r requirements.in
 typed-ast==1.5.4 \
     --hash=sha256:0261195c2062caf107831e92a76764c81227dae162c4f75192c0d489faf751a2 \
     --hash=sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1 \
     --hash=sha256:183afdf0ec5b1b211724dfef3d2cad2d767cbefac291f24d69b00546c1837fb6 \
     --hash=sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62 \
     --hash=sha256:267e3f78697a6c00c689c03db4876dd1efdfea2f251a5ad6555e82a26847b4ac \
     --hash=sha256:2efae9db7a8c05ad5547d522e7dbe62c83d838d3906a3716d1478b6c1d61388d \
@@ -235,24 +253,28 @@
     --hash=sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72 \
     --hash=sha256:a94d55d142c9265f4ea46fab70977a1944ecae359ae867397757d836ea5a3f47 \
     --hash=sha256:a9916d2bb8865f973824fb47436fa45e1ebf2efd920f2b9f99342cb7fab93f72 \
     --hash=sha256:c542eeda69212fa10a7ada75e668876fdec5f856cd3d06829e6aa64ad17c8dfe \
     --hash=sha256:cf4afcfac006ece570e32d6fa90ab74a17245b83dfd6655a6f68568098345ff6 \
     --hash=sha256:ebd9d7f80ccf7a82ac5f88c521115cc55d84e35bf8b446fcd7836eb6b98929a3 \
     --hash=sha256:ed855bbe3eb3715fca349c80174cfcfd699c2f9de574d40527b8429acae23a66
-    # via -r .\requirements.in
+    # via -r requirements.in
 typing-extensions==3.10.0.0 \
     --hash=sha256:0ac0f89795dd19de6b97debb0c6af1c70987fd80a2d62d1958f7e56fcc31b497 \
     --hash=sha256:50b6f157849174217d0656f99dc82fe932884fb250826c18350e159ec6cdf342 \
     --hash=sha256:779383f6086d90c99ae41cf0ff39aac8a7937a9283ce0a414e5dd782f4c94a84
-    # via -r .\requirements.in
+    # via -r requirements.in
 urllib3==1.26.12 \
     --hash=sha256:3fa96cf423e6987997fc326ae8df396db2a8b7c667747d47ddd8ecba91f4a74e \
     --hash=sha256:b930dd878d5a8afb066a637fbb35144fe7901e3b209d1cd4f524bd0e9deee997
     # via requests
+virtualenv==20.16.6 \
+    --hash=sha256:186ca84254abcbde98180fd17092f9628c5fe742273c02724972a1d8a2035108 \
+    --hash=sha256:530b850b523c6449406dfba859d6345e48ef19b8439606c5d74d7d3c9e14d76e
+    # via tox
 wrapt==1.14.1 \
     --hash=sha256:00b6d4ea20a906c0ca56d84f93065b398ab74b927a7a3dbd470f6fc503f95dc3 \
     --hash=sha256:01c205616a89d09827986bc4e859bcabd64f5a0662a7fe95e0d359424e0e071b \
     --hash=sha256:02b41b633c6261feff8ddd8d11c711df6842aba629fdd3da10249a53211a72c4 \
     --hash=sha256:07f7a7d0f388028b2df1d916e94bbb40624c59b48ecc6cbc232546706fac74c2 \
     --hash=sha256:11871514607b15cfeb87c547a49bca19fde402f32e2b1c24a632506c0a756656 \
     --hash=sha256:1b376b3f4896e7930f1f772ac4b064ac12598d1c38d04907e696cc4d794b43d3 \
```

### Comparing `pgn_to_sqlite-2.0.3/tests/game_files/test_pgn_file_lichess.pgn` & `pgn_to_sqlite-2.0.4/tests/game_files/test_pgn_file_lichess.pgn`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.3/tests/test_cli.py` & `pgn_to_sqlite-2.0.4/tests/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from click.testing import CliRunner
-from pgn_to_sqlite.cli import build_pgn_dict, convert_to_snake_case, cli
+
+from pgn_to_sqlite.cli import build_pgn_dict, cli, convert_to_snake_case
 
 
 def test_snake_case_conversion():
     result = convert_to_snake_case("SpamSpam")
     assert result == "spam_spam"
```

### Comparing `pgn_to_sqlite-2.0.3/PKG-INFO` & `pgn_to_sqlite-2.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pgn_to_sqlite
-Version: 2.0.3
+Version: 2.0.4
 Summary: Fetch your games from chess.com and lichess.org and add them to a sqlite database
 Home-page: https://github.com/EndlessTrax/pgn-to-sqlite
 Author: Ricky White
 Author-email: ricky@whitelionmedia.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click
 Requires-Dist: requests
 Requires-Dist: berserk
 Project-URL: Documentation, https://github.com/EndlessTrax/pgn-to-sqlite/blob/master/README.md
 Project-URL: Issues, https://github.com/EndlessTrax/pgn-to-sqlite/issues
 
 # PGN to Sqlite
@@ -90,29 +91,17 @@
 
 If you find a bug, please file an [issue](https://github.com/EndlessTrax/pgn-to-sqlite/issues).
 
 If you have feature requests, please [file an issue](https://github.com/EndlessTrax/pgn-to-sqlite/issues) and use the appropriate label.
 
 Please **raise an issue before making a PR**, so that the issue and implementation can be discussed before you write any code. This will save you time, and increase the chances of your PR being merged without significant changes.
 
-Please **format you code** with [Black](https://pypi.org/project/black/).
+Please **format you code** with [Black](https://pypi.org/project/black/) and [isort](https://pypi.org/project/isort/).
 
 Please **include tests** for any PR's that include code (unless current tests cover your code contribution).
 
 ## Support
 
 If you would like to show your support for the project, I would be very grateful if you would donate to a charity close to my heart, [Walk AS One](https://walkasone.org/donate).
 
 And if you would prefer to donate to me personally instead, [you can sponsor me on Github](https://github.com/sponsors/EndlessTrax)? 🤓
 
-## Changelog
-
-### 2.0
-
-- Breaking changes to CLI commands
-- Added ability to add games from locally saved `.pgn` files to the output database
-
-### 1.0
-
-- Fetch games from _chess.com_ and _lichess.org_
-- Saves games to SQlite3 database
-
```

