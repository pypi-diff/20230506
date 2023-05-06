# Comparing `tmp/athletes_unlimited_py-0.0.2.tar.gz` & `tmp/athletes_unlimited_py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athletes_unlimited_py-0.0.2.tar", last modified: Tue Apr 25 18:57:16 2023, max compression
+gzip compressed data, was "athletes_unlimited_py-0.0.3.tar", last modified: Sat May  6 06:48:00 2023, max compression
```

## Comparing `athletes_unlimited_py-0.0.2.tar` & `athletes_unlimited_py-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/athetes_unlimited_py/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25042 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/aux_softball.py
--rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/basketball.py
--rw-r--r--   0 runner    (1001) docker     (123)    22245 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/lacrosse.py
--rw-r--r--   0 runner    (1001) docker     (123)    47203 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/softball.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/athetes_unlimited_py/volleyball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 18:57:16.000000 athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-25 18:56:50.000000 athletes_unlimited_py-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:57:16.229229 athletes_unlimited_py-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:48:00.362724 athletes_unlimited_py-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-06 06:48:00.362724 athletes_unlimited_py-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:48:00.358724 athletes_unlimited_py-0.0.3/athetes_unlimited_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/athetes_unlimited_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25042 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/athetes_unlimited_py/aux_softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31448 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/athetes_unlimited_py/basketball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22245 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/athetes_unlimited_py/lacrosse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47203 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/athetes_unlimited_py/softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/athetes_unlimited_py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/athetes_unlimited_py/volleyball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:48:00.362724 athletes_unlimited_py-0.0.3/athletes_unlimited_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-06 06:48:00.000000 athletes_unlimited_py-0.0.3/athletes_unlimited_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-06 06:48:00.000000 athletes_unlimited_py-0.0.3/athletes_unlimited_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:48:00.000000 athletes_unlimited_py-0.0.3/athletes_unlimited_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 06:48:00.000000 athletes_unlimited_py-0.0.3/athletes_unlimited_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 06:48:00.000000 athletes_unlimited_py-0.0.3/athletes_unlimited_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-06 06:47:37.000000 athletes_unlimited_py-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 06:48:00.362724 athletes_unlimited_py-0.0.3/setup.cfg
```

### Comparing `athletes_unlimited_py-0.0.2/LICENSE` & `athletes_unlimited_py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.2/PKG-INFO` & `athletes_unlimited_py-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes_unlimited_py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.2/README.md` & `athletes_unlimited_py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.2/athetes_unlimited_py/aux_softball.py` & `athletes_unlimited_py-0.0.3/athetes_unlimited_py/aux_softball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.2/athetes_unlimited_py/basketball.py` & `athletes_unlimited_py-0.0.3/athetes_unlimited_py/volleyball.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,224 +6,206 @@
 import requests
 from tqdm import tqdm
 
 from athetes_unlimited_py.utils import raise_html_status_code
 
 ############################################################################################################################################################################################################################################################
 ##
-## Basketball-only utilities
+## Volleyball-only utilities
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_basketball_season(season_id:int) -> int:
+def get_au_volleyball_season(season_id:int) -> int:
     """
-    Given a season ID, `get_au_basketball_season()` returns the proper season for the corresponding Athletes Unlimited basketball season.
+    Given a season ID, `get_au_volleyball_season()` returns the proper season for the corresponding Athletes Unlimited volleyball season.
 
     Parameters
     ----------
     `season_id` (int, mandatory):
-        The season ID you want a season for in Athletes Unlimited basketball. 
+        The season ID you want a season for in Athletes Unlimited volleyball. 
         If there isn't a season for the inputted `season_id`, a `ValueError()` exception will be raised.
     
     Returns
     ----------
-    The proper season corresponding to an Athletes Unlimited basketball season ID.
+    The proper season corresponding to an Athletes Unlimited volleyball season ID.
     """
     season = 0
     
-    if season_id == 6:
-        season= 2022
+    if season_id == 3:
+        season = 2021
+        return season 
+    elif season_id == 11:
+        season = 2022
         return season
-    elif season_id == 73:
+    elif season_id == 138:
         season = 2023
         return season 
     else:
-        raise ValueError(f'[season] can only be 2022 or 2023 at this time for basketball.\nYou entered :\n\t{season}')
+        raise ValueError(f'[season] can only be 2021, 2022, or 2023 at this time for volleyball.\nYou entered :\n\t{season}')
 
-def get_au_basketball_season_id(season:int) -> int:
+def get_au_volleyball_season_id(season:int) -> int:
     """
-    Given a season, `get_au_basketball_season_id()` returns the proper season ID for the Athletes Unlimited basketball season.
+    Given a season, `get_au_volleyball_season_id()` returns the proper season ID for the Athletes Unlimited volleyball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
-        The season you want a season ID for basketball. 
+        The season you want a season ID for volleyball. 
         If there isn't a season ID for the inputted `season`, a `ValueError()` exception will be raised.
     
     Returns
     ----------
-    The proper season ID corresponding to an Athletes Unlimited basketball season.
+    The proper season ID corresponding to an Athletes Unlimited volleyball season.
     """
     seasonId = 0
     
-    if season == 2022:
-        seasonId = 6
-        return seasonId
+    if season == 2021:
+        seasonId = 3
+        return seasonId 
+    elif season == 2022:
+        seasonId = 11
+        return seasonId 
     elif season == 2023:
-        seasonId = 73
+        seasonId = 138
         return seasonId 
     else:
-        raise ValueError(f'[season] can only be 2022 or 2023 at this time for basketball.\nYou entered :\n\t{season}')
+        raise ValueError(f'[season] can only be 2021, 2022, or 2023 at this time for volleyball.\nYou entered :\n\t{season}')
 
 ############################################################################################################################################################################################################################################################
 ##
 ## Game Functions
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_basketball_game_stats(season:int,game_num:int,get_team_stats=False,get_player_and_team_stats=False,rename_cols=False) -> pd.DataFrame():
+def get_au_volleyball_game_stats(season_id:int,game_num:int,get_team_stats=False,get_player_and_team_stats=False,rename_cols=False) -> pd.DataFrame():
     """
-    Retrieves the player and/or team game stats for an Atheltes Unlimited (AU) basketball game.
+    Retrieves the player and/or team game stats for an Atheltes Unlimited (AU) volleyball game.
 
     Parameters
     ----------
-    `season` (int, mandatory):
-        The AU basketball season you want a game from.
+    `season_id` (int, mandatory):
+        The AU volleyball season ID you want a game from.
     
     `game_num` (int, mandatory):
         The game number you want player and/or team stats from.
         This is not the game ID!
         A `ValueError` will be raised if `game_num` is set to less than 1.
     
     `get_team_stats` (bool, optional) = False:
         Optional boolean argument. 
-        If set to `True`, the pandas DataFrame returned by `get_basketball_game_stats()` will only return team stats for that game, 
+        If set to `True`, the pandas DataFrame returned by `get_volleyball_game_stats()` will only return team stats for that game, 
         and will not return player stats, unless `get_player_and_team_stats` is set to `True` if `get_team_stats` is set to `True`.
     
     `get_player_and_team_stats` (bool, optional) = False:
 
     `rename_cols` (bool, optional) = False:
         NOT IMPLEMENTED YET!
-        `get_basketball_game_stats()` will have no change in functionality at this time if `rename_cols` is set to `True`.
+        `get_volleyball_game_stats()` will have no change in functionality at this time if `rename_cols` is set to `True`.
         
 
     Returns
     ----------
-    A pandas DataFrame containing player and/or team stats for a given AU game within a given AU season.
+    A pandas DataFrame containing player and/or team stats for a given AU game within a given AU season ID.
     """
 
     headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
     player_stats_df = pd.DataFrame()
     team_stats_df = pd.DataFrame()
     row_df = pd.DataFrame()
-    
-    season_id = get_au_basketball_season_id(season)
-    
+
     if game_num < 1:
         raise ValueError('`game_num` cannot be less than 0.')
     
     key = int(time.time()) # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
-    
-    url = f"https://auprosports.com/proxy.php?request=/api/stats/basketball/v1/{season_id}/by-game/{game_num}?statType=basketball%26k={key}"
-    
+    url = f"https://auprosports.com/proxy.php?request=/api/stats/volleyball/v1/{season_id}/by-game/{game_num}?statType=volleyball%26k={key}"
+
     response = requests.get(url,headers=headers)
     raise_html_status_code(response.status_code)
     
     json_data = json.loads(response.text)
-    time.sleep(0.5)
 
     sport = json_data['metaSport']['sport']
     api_version = json_data['metaSport']['version']
 
-    print(f'\nOn game #{game_num} in the {season} AU Basketball season.')
     for i in tqdm(json_data['data']):
-        #print(i)
         row_df = pd.DataFrame({'sport':sport,'api_version':api_version},index=[0])
-        row_df['type'] = i['type']
-        row_df['teamId'] = i['teamId']
-
-        if i['homeTeamFlg'] == True:
-            row_df['homeTeamFlg'] = 1
-        else:
-            row_df['homeTeamFlg'] = 0
-
+        
         ##############################################################################################################################
         ## Player/Team info
         ##############################################################################################################################
-        row_df['season'] = get_au_basketball_season(i['seasonId'])
-        row_df['season_id'] = i['seasonId']
-        row_df['week_number'] = i['stats'][0]['weekNumber']
-        row_df['game_number'] = i['stats'][0]['gameNumber']
-        row_df['season_type'] = i['stats'][0]['seasonType']
-
-        row_df['player_id'] = i['playerId']
-        row_df['uniform_number'] = i['uniformNumber']
-        row_df['uniform_number_display'] = str(i['uniformNumberDisplay'])
+        row_df['season'] = get_au_volleyball_season(i['seasonId'])
+        row_df['seasonId'] = i['seasonId']
+        row_df['weekNumber'] = 0
+        row_df['gameNumber'] = 0
+        row_df['seasonType'] = ""
+
+        row_df['playerId'] = i['playerId']
+        row_df['uniformNumber'] = i['uniformNumber']
+        row_df['uniformNumberDisplay'] = str(i['uniformNumberDisplay'])
         
-        row_df['primary_position_lk'] = i['primaryPositionLk']
-        row_df['secondary_position_lk'] = i['secondaryPositionLk']
+        row_df['primaryPositionLk'] = i['primaryPositionLk']
+        row_df['secondaryPositionLk'] = i['secondaryPositionLk']
         row_df['first_name'] = str(i['firstName']).replace('\u2019','\'')
         row_df['last_name'] = str(i['lastName']).replace('\u2019','\'')
         row_df['full_name'] = f"{i['firstName']} {i['lastName']}".replace('\u2019','\'')
 
         ##############################################################################################################################
-        ## Game Stats
+        ## Player/Team stats
         ##############################################################################################################################
-        
-        row_df['G'] = i['stats'][0]['gamesPlayed']
-        row_df['MIN'] = i['stats'][0]['minutesPlayed']
+        row_df['player_id'] = i['stats'][0]['playerId']
+        row_df['first_name'] = i['stats'][0]['firstName']
+        row_df['last_name'] = i['stats'][0]['lastName']
+        row_df['uniform_number'] = i['stats'][0]['uniformNumber']
+        row_df['uniform_number_display'] = str(i['stats'][0]['uniformNumberDisplay'])
+        row_df['primary_position_lk'] = i['stats'][0]['primaryPositionLk']
+        row_df['secondary_position_lk'] = i['stats'][0]['secondaryPositionLk']
+        row_df['team_id'] = i['stats'][0]['teamId']
+        row_df['sets_played'] = i['stats'][0]['setsPlayed']
+        row_df['player_id'] = i['stats'][0]['playerId']
+        row_df['kills'] = i['stats'][0]['kills']
+        row_df['kills_per_set'] = i['stats'][0]['killsPerSet']
+        row_df['attack_errors'] = i['stats'][0]['attackErrors']
+        row_df['attack_attempts'] = i['stats'][0]['attackAttempts']
+        row_df['attack_percentage'] = i['stats'][0]['attackPercentage']
+        row_df['assists'] = i['stats'][0]['assists']
+        row_df['assists_per_set'] = i['stats'][0]['assistsPerSet']
+        row_df['setting_errors'] = i['stats'][0]['settingErrors']
+        row_df['service_errors'] = i['stats'][0]['serviceErrors']
+        row_df['service_aces'] = i['stats'][0]['serviceAces']
+        row_df['service_aces_per_set'] = i['stats'][0]['serviceAcesPerSet']
+        row_df['total_reception_attempts'] = i['stats'][0]['totalReceptionAttempts']
+        row_df['reception_errors'] = i['stats'][0]['receptionErrors']
+        row_df['positive_reception_pct'] = i['stats'][0]['positiveReceptionPct']
+        row_df['digs'] = i['stats'][0]['digs']
+        row_df['digs_per_set'] = i['stats'][0]['digsPerSet']
+        row_df['blocks'] = i['stats'][0]['blocks']
+        row_df['blocks_per_set'] = i['stats'][0]['blocksPerSet']
+        row_df['au_total_points'] = i['stats'][0]['auTotalPoints']
+        row_df['week_number'] = i['stats'][0]['weekNumber']
+        row_df['game_number'] = i['stats'][0]['gameNumber']
+        row_df['season_type'] = i['stats'][0]['seasonType']
 
-        row_df['FGM'] = i['stats'][0]['fieldGoalsMade']
-        row_df['FGA'] = i['stats'][0]['fieldGoalsAttempted']
-        row_df['FG%'] = row_df['FGM'] /row_df['FGA']
-        row_df['FG%'] = row_df['FG%'].round(3)
-
-        row_df['3PM'] = i['stats'][0]['made3Pointers']
-        row_df['3PA'] = i['stats'][0]['attempted3Pointers']
-        row_df['3P%'] = row_df['3PM'] /row_df['3PA']
-        row_df['3P%'] = row_df['3P%'].round(3)
-
-        row_df['2PM'] = i['stats'][0]['made2Pointers']
-        row_df['2PA'] = i['stats'][0]['missed2Pointers'] + i['stats'][0]['made2Pointers']
-        row_df['2P%'] = row_df['2PM'] /row_df['2PA']
-        row_df['2P%'] = row_df['2P%'].round(3)
-
-        row_df['FTM'] = i['stats'][0]['madeFreeThrows']
-        row_df['FTA'] = i['stats'][0]['freeThrowsAttempted']
-        row_df['FT%'] = row_df['FTM'] / row_df['FTA']
-        row_df['FT%'] = row_df['FT%'].round(3)
-
-        row_df['ORB'] = i['stats'][0]['offensiveRebounds']
-        row_df['DRB'] = i['stats'][0]['defensiveRebounds']
-        row_df['TRB'] = i['stats'][0]['rebounds']
-
-        row_df['AST'] = i['stats'][0]['assists']
-        row_df['STL'] = i['stats'][0]['steals']
-        row_df['BLK'] = i['stats'][0]['blocks']
-
-        row_df['TOV'] = i['stats'][0]['turnovers']
-        row_df['PTS'] = i['stats'][0]['points']
-
-        row_df['AU_PTS'] = i['stats'][0]['auTotalPoints']
-
-        row_df['eFG%'] = (row_df['FGM'] + (0.5 * row_df['3PM'])) / row_df['FGA']
-        row_df['eFG%'] = row_df['eFG%'].round(3)
-
-        row_df['TS%'] = row_df['PTS'] / (2 * ((row_df['FGA']) + (0.44 * row_df['FTA'])))
-        row_df['TS%'] = row_df['TS%'].round(3)
-        row_df['shootingFoulsCommitted'] = i['stats'][0]['shootingFoulsCommitted']
-        row_df['shootingFoulsDrawn'] = i['stats'][0]['shootingFoulsDrawn']
-        row_df['personalFoulsCommitted'] = i['stats'][0]['personalFoulsCommitted']
-        row_df['personalFoulsDrawn'] = i['stats'][0]['personalFoulsDrawn']
-        row_df['offensiveFoulsCommitted'] = i['stats'][0]['offensiveFoulsCommitted']
-        row_df['offensiveFoulsDrawn'] = i['stats'][0]['offensiveFoulsDrawn']
-        row_df['doubleDoubles'] = i['stats'][0]['doubleDoubles']
-        row_df['tripleDoubles'] = i['stats'][0]['tripleDoubles']
 
-        row_df['GmSc'] = row_df['PTS'] + (0.4 * row_df['FGM']) + (0.7 * row_df['ORB']) + (0.3 * row_df['DRB']) + row_df['STL'] + (0.7 * row_df['AST']) + (0.7 * row_df['BLK']) * (0.7 * row_df['FGA']) - (0.4 * (row_df['FTA'] - row_df['FTM'])) - (0.4 * row_df['personalFoulsCommitted']) - row_df['TOV']
-        
         ##############################################################################################################################
         ## Save the data to the correct DataFrame
         ##############################################################################################################################
 
         if i['type'] == "Team":
             team_stats_df = pd.concat([team_stats_df,row_df],ignore_index=True)
         else:
             player_stats_df = pd.concat([player_stats_df,row_df],ignore_index=True)
 
+        row_df['type'] = i['type']
+        row_df['teamId'] = i['teamId']
+
+        if i['homeTeamFlg'] == True:
+            row_df['homeTeamFlg'] = 1
+        else:
+            row_df['homeTeamFlg'] = 0
+
         del row_df
 
     ##############################################################################################################################
     ## Once we're done, return the correct dataframe.
     ##############################################################################################################################
     
     if get_player_and_team_stats == True:
@@ -233,108 +215,95 @@
     elif get_team_stats == True:        
         del player_stats_df
         return team_stats_df
     else:
         del team_stats_df
         return player_stats_df
 
-def get_au_basketball_pbp(season:int,game_id:int,return_participation_data=False):
+def get_au_volleyball_pbp(season_id:int,game_id:int,return_participation_data=False) -> pd.DataFrame():
     """
-    Retrieves the play-by-play (PBP) data for an Atheltes Unlimited (AU) basketball game.
+    Retrieves the play-by-play (PBP) data for an Atheltes Unlimited (AU) volleyball game.
 
     Parameters
     ----------
-    `season` (int, mandatory):
-        The AU basketball season you want a game from.
+    `season_id` (int, mandatory):
+        The AU volleyball season ID you want a game from.
     
     `game_id` (int, mandatory):
-        The AU basketball game ID you want PBP data from.
+        The AU volleyball game ID you want PBP data from.
     
     `return_participation_data` (bool, optional) = `False`:
         Optional argument. 
-        If set to `True`, `get_au_basketball_pbp()` will return a secondary pandas DataFrame
-        containing roster information for this AU basketball game.
+        If set to `True`, `get_au_volleyball_pbp()` will return a secondary pandas DataFrame
+        containing roster information for this AU volleyball game.
 
     Returns
     ----------
-    A pandas DataFrame containing PBP data for a given AU game ID within a given AU season.
+    A pandas DataFrame containing PBP data for a given AU game ID within a given AU season ID.
     If `return_participation_data` is set to `True`, an additional pandas DataFrame containing roster data for this game will be returned as well.
     """
 
-    season_id = get_au_basketball_season_id(season)
+    # season_id = get_au_volleyball_season_id(season)
+    season = get_au_volleyball_season(season_id)
 
     headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
     game_pbp_df = pd.DataFrame()
     roster_df = pd.DataFrame()
     row_df = pd.DataFrame()
         
     if game_id < 1:
         raise ValueError('`game_id` cannot be less than 0.')
     
     key = int(time.time()) # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
-    url = f"https://auprosports.com/proxy.php?request=/api/play-by-play/basketball/v1/event/{season_id}/game/{game_id}?k={key}"
+    url = f"https://auprosports.com/proxy.php?request=/api/play-by-play/volleyball/v1/event/{season_id}/game/{game_id}?k={key}"
 
     response = requests.get(url,headers=headers)
     raise_html_status_code(response.status_code)
     
-    del headers, key
 
     json_data = json.loads(response.text)
-    time.sleep(0.5)
 
+    del headers, key
+    #print(json_data)
     for i in tqdm(json_data['data'][0]['plays']):
         row_df = pd.DataFrame({'season':season,'game_id':game_id},index=[0])
+
         row_df['game_number'] = i['gameNumber']
+        row_df['game_id'] = i['gameId']
         row_df['play_seq_num'] = i['playSeqno']
-        row_df['narrative'] = i['narrative']
+        row_df['narrative_formatted'] = i['narrativeFormatted']
+        row_df['start_time'] = i['startTime']
+        row_df['end_time'] = i['endTime']
+        row_df['set_number'] = i['setNumber']
+        row_df['set_status_lk'] = i['setStatusLk']
+        row_df['rally_number'] = i['rallyNumber']
+        row_df['play_code'] = i['playCode']
+        row_df['play_text'] = i['playText']
+        row_df['player_id'] = i['playerId']
+        row_df['serve_ace'] = i['serveAce']
+        row_df['serve_error'] = i['serveError']
+        row_df['serve_continue'] = i['serveContinue']
+        row_df['attack_kill'] = i['attackKill']
+        row_df['attack_error'] = i['attackError']
+        row_df['attack_continue'] = i['attackContinue']
+        row_df['pass_good'] = i['passGood']
+        row_df['pass_error'] = i['passError']
+        row_df['pass_continue'] = i['passContinue']
+        row_df['dig_dig'] = i['digDig']
+        row_df['dig_continue'] = i['digContinue']
+        row_df['block_continue'] = i['blockContinue']
+        row_df['block_stuff'] = i['blockStuff']
+        row_df['set_assist'] = i['setAssist']
+        row_df['set_error'] = i['setError']
+        row_df['set_continue'] = i['setContinue']
         row_df['home_team_id'] = i['homeTeamId']
         row_df['home_team_score'] = i['homeTeamScore']
         row_df['away_team_id'] = i['awayTeamId']
-        row_df['away_team_score'] = i['awayTeamScore']
-        row_df['is_a_play'] = i['isAPlay']
-        row_df['generates_point_audit_flag'] = i['generatesPointAuditFlg']
-        row_df['has_error'] = i['hasError']
-        row_df['player_id'] = i['playerId']
-        row_df['team_id'] = i['teamId']
-        row_df['action'] = i['action']
-        row_df['type'] = i['type']
-        row_df['quarter'] = i['quarter']
-        row_df['clock'] = i['clock']
-        row_df['assist'] = i['assist']
-        row_df['steal'] = i['steal']
-        row_df['block'] = i['block']
-        row_df['turnover'] = i['turnover']
-        row_df['jumper'] = i['jumper']
-        row_df['dunk'] = i['dunk']
-        row_df['tip_in'] = i['tipIn']
-        row_df['timeout'] = i['timeout']
-        row_df['in_the_paint'] = i['inThePaint']
-        row_df['on_fast_break'] = i['onFastBreak']
-        row_df['missed_three_pointer'] = i['missedThreePointer']
-        row_df['made_three_pointer'] = i['madeThreePointer']
-        row_df['missed_two_pointer'] = i['missedTwoPointer']
-        row_df['made_two_pointer'] = i['madeTwoPointer']
-        row_df['missed_free_throw'] = i['missedFreeThrow']
-        row_df['made_free_throw'] = i['madeFreeThrow']
-        row_df['offensive_rebound'] = i['offensiveRebound']
-        row_df['defensive_rebound'] = i['defensiveRebound']
-        row_df['shooting_foul_committed'] = i['shootingFoulCommitted']
-        row_df['shooting_foul_drawn'] = i['shootingFoulDrawn']
-        row_df['shooting_foul_drawn_by_player_id'] = i['shootingFoulDrawnByPlayerId']
-        row_df['personal_foul_committed'] = i['personalFoulCommitted']
-        row_df['personal_foul_drawn'] = i['personalFoulDrawn']
-        row_df['personal_foul_drawn_by_player_id'] = i['personalFoulDrawnByPlayerId']
-        row_df['offensive_foul_committed'] = i['offensiveFoulCommitted']
-        row_df['offensive_foul_drawn'] = i['offensiveFoulDrawn']
-        row_df['offensive_foul_drawn_by_player_id'] = i['offensiveFoulDrawnByPlayerId']
-        row_df['other_foul_committed'] = i['otherFoulCommitted']
-        row_df['other_foul_drawn'] = i['otherFoulDrawn']
-        row_df['other_foul_drawn_by_player_id'] = i['otherFoulDrawnByPlayerId']
-        row_df['scoring_play'] = i['scoringPlay']
-
+        row_df['away_team_Score'] = i['awayTeamScore']
+        row_df['scoring_team_id'] = i['scoringTeamId']
 
         game_pbp_df = pd.concat([game_pbp_df,row_df])
         del row_df
     
     if return_participation_data == True:
         
         for i in json_data['data'][0]['competitors']:
@@ -385,135 +354,135 @@
 
 ############################################################################################################################################################################################################################################################
 ##
 ## Season Functions
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_basketball_season_pbp(season:int) -> pd.DataFrame():
+def get_au_volleyball_season_pbp(season:int) -> pd.DataFrame():
     """
-    Given an Atheltes Unlimited (AU) basketball season, get and parse all play-by-play (PBP) data for an AU basketball season.
+    Given an Atheltes Unlimited (AU) volleyball season, get and parse all play-by-play (PBP) data for an AU volleyball season.
     
     Parameters
     ----------
     `season` (int, mandatory):
-        The AU basketball season you want PBP data from.
+        The AU volleyball season you want PBP data from.
 
     Returns
     ----------
     A pandas DataFrame containing PBP data from a AU season.
 
     """
     season_pbp_df = pd.DataFrame()
-    seasonId = get_au_basketball_season_id(season)
-    url = "https://auprosports.com/proxy.php?request=api/seasons/basketball/v1"
+    season_id = get_au_volleyball_season_id(season)
+    url = "https://auprosports.com/proxy.php?request=api/seasons/volleyball/v1"
     headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"}
 
     response = requests.get(url,headers=headers)
     sport_json_data = json.loads(response.text)
     
-    for i in tqdm(sport_json_data['data']):
+    for i in sport_json_data['data']:
         #print(i)
-        if i['seasonId'] == seasonId:
-            len_game_ids = len(i['gameIds'])
+        if i['seasonId'] == season_id:
+            # len_game_ids = len(i['gameIds'])
 
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game ID {j} in {season}.')
                 # try:
-                #     game_df = get_basketball_game_stats(season,j)
+                #     game_df = get_volleyball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_basketball_pbp(season,j)
+                game_df = get_au_volleyball_pbp(season_id,j)
 
                 season_pbp_df = pd.concat([season_pbp_df,game_df],ignore_index=True)
                 del game_df
 
     return season_pbp_df
 
-def get_au_basketball_season_player_box(season:int) -> pd.DataFrame():
+def get_au_volleyball_season_player_box(season:int) -> pd.DataFrame():
     """
-    Given an Atheltes Unlimited (AU) basketball season, get and parse all box-score game stats for an AU basketball season.
+    Given an Atheltes Unlimited (AU) volleyball season, get and parse all box-score game stats for an AU volleyball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
-        The AU basketball season you want player box scores from.
+        The AU volleyball season you want player box scores from.
 
     Returns
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
-    seasonId = get_au_basketball_season_id(season)
-    url = "https://auprosports.com/proxy.php?request=api/seasons/basketball/v1"
+    season_id = get_au_volleyball_season_id(season)
+    url = "https://auprosports.com/proxy.php?request=api/seasons/volleyball/v1"
     headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
     response = requests.get(url,headers=headers)
     sport_json_data = json.loads(response.text)
     
     for i in sport_json_data['data']:
         #print(i)
-        if i['seasonId'] == seasonId:
+        if i['seasonId'] == season_id:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1,len_game_ids+1)):
-                # print(f'\nOn game ID {j} for the {season}.')
+                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
                 # try:
-                #     game_df = get_basketball_game_stats(season,j)
+                #     game_df = get_volleyball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_basketball_game_stats(season,j)
+                game_df = get_au_volleyball_game_stats(season_id,j)
 
                 season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
                 del game_df
 
     return season_stats_df
 
-def get_au_basketball_season_team_box(season:int) -> pd.DataFrame():
+def get_au_volleyball_season_team_box(season:int) -> pd.DataFrame():
     """
-    Given an Atheltes Unlimited (AU) basketball season, get and parse all box-score game stats for an AU basketball season.
+    Given an Atheltes Unlimited (AU) volleyball season, get and parse all box-score game stats for an AU volleyball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
-        The AU basketball season you want player box scores from.
+        The AU volleyball season you want player box scores from.
 
     Returns
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
-    seasonId = get_au_basketball_season_id(season)
-    url = "https://auprosports.com/proxy.php?request=api/seasons/basketball/v1"
+    season_id = get_au_volleyball_season_id(season)
+    url = "https://auprosports.com/proxy.php?request=api/seasons/volleyball/v1"
     headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
     response = requests.get(url,headers=headers)
     sport_json_data = json.loads(response.text)
     
-    for i in tqdm(sport_json_data['data']):
+    for i in sport_json_data['data']:
         #print(i)
-        if i['seasonId'] == seasonId:
+        if i['seasonId'] == season_id:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1,len_game_ids+1)):
-                # print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
                 # try:
-                #     game_df = get_basketball_game_stats(season,j)
+                #     game_df = get_volleyball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_basketball_game_stats(season,j,get_team_stats=True)
+                game_df = get_au_volleyball_game_stats(season_id,j,get_team_stats=True)
 
                 season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
                 del game_df
 
     return season_stats_df
```

### Comparing `athletes_unlimited_py-0.0.2/athetes_unlimited_py/lacrosse.py` & `athletes_unlimited_py-0.0.3/athetes_unlimited_py/lacrosse.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.2/athetes_unlimited_py/softball.py` & `athletes_unlimited_py-0.0.3/athetes_unlimited_py/softball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.2/athetes_unlimited_py/utils.py` & `athletes_unlimited_py-0.0.3/athetes_unlimited_py/utils.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.2/athletes_unlimited_py.egg-info/PKG-INFO` & `athletes_unlimited_py-0.0.3/athletes_unlimited_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes-unlimited-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.2/pyproject.toml` & `athletes_unlimited_py-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","pyarrow","pandas","tqdm","requests","lxml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "athletes_unlimited_py"
-version = "0.0.2"
+version = "0.0.3"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 authors = [
     {name = "Joseph Armstrong", email="armstrongjoseph08@gmail.com"}
 ]
```

