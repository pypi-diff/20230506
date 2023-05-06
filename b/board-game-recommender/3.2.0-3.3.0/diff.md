# Comparing `tmp/board-game-recommender-3.2.0.tar.gz` & `tmp/board-game-recommender-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "board-game-recommender-3.2.0.tar", last modified: Wed Apr 12 18:48:02 2023, max compression
+gzip compressed data, was "board-game-recommender-3.3.0.tar", last modified: Sat May  6 19:41:30 2023, max compression
```

## Comparing `board-game-recommender-3.2.0.tar` & `board-game-recommender-3.3.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-04-12 18:48:02.374303 board-game-recommender-3.2.0/
--rw-r--r--   0 markus     (501) staff       (20)     1072 2020-09-18 05:15:08.000000 board-game-recommender-3.2.0/LICENSE
--rw-r--r--   0 markus     (501) staff       (20)       26 2021-11-28 20:14:53.000000 board-game-recommender-3.2.0/MANIFEST.in
--rw-r--r--   0 markus     (501) staff       (20)     4047 2023-04-12 18:48:02.373755 board-game-recommender-3.2.0/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)     2704 2021-05-19 13:26:08.000000 board-game-recommender-3.2.0/README.md
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-04-12 18:48:02.370539 board-game-recommender-3.2.0/board_game_recommender/
--rw-r--r--   0 markus     (501) staff       (20)      429 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/__init__.py
--rw-r--r--   0 markus     (501) staff       (20)     5079 2023-04-11 10:26:21.000000 board-game-recommender-3.2.0/board_game_recommender/__main__.py
--rw-r--r--   0 markus     (501) staff       (20)       78 2023-04-12 18:47:34.000000 board-game-recommender-3.2.0/board_game_recommender/__version__.py
--rw-r--r--   0 markus     (501) staff       (20)     1846 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/base.py
--rw-r--r--   0 markus     (501) staff       (20)     9358 2023-04-12 18:45:41.000000 board-game-recommender-3.2.0/board_game_recommender/light.py
--rw-r--r--   0 markus     (501) staff       (20)     4766 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/rankings.py
--rw-r--r--   0 markus     (501) staff       (20)    31608 2023-04-11 10:26:21.000000 board-game-recommender-3.2.0/board_game_recommender/recommend.py
--rw-r--r--   0 markus     (501) staff       (20)     2099 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/trust.py
--rw-r--r--   0 markus     (501) staff       (20)     3767 2023-04-11 10:26:21.000000 board-game-recommender-3.2.0/board_game_recommender/utils.py
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-04-12 18:48:02.373036 board-game-recommender-3.2.0/board_game_recommender.egg-info/
--rw-r--r--   0 markus     (501) staff       (20)     4047 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)      573 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/SOURCES.txt
--rw-r--r--   0 markus     (501) staff       (20)        1 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/dependency_links.txt
--rw-r--r--   0 markus     (501) staff       (20)       65 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/requires.txt
--rw-r--r--   0 markus     (501) staff       (20)       23 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/top_level.txt
--rw-r--r--   0 markus     (501) staff       (20)       38 2023-04-12 18:48:02.374440 board-game-recommender-3.2.0/setup.cfg
--rwxr-xr-x   0 markus     (501) staff       (20)     4947 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/setup.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-06 19:41:30.912780 board-game-recommender-3.3.0/
+-rw-r--r--   0 markus     (501) staff       (20)     1072 2020-09-18 05:15:08.000000 board-game-recommender-3.3.0/LICENSE
+-rw-r--r--   0 markus     (501) staff       (20)       26 2021-11-28 20:14:53.000000 board-game-recommender-3.3.0/MANIFEST.in
+-rw-r--r--   0 markus     (501) staff       (20)     4074 2023-05-06 19:41:30.912400 board-game-recommender-3.3.0/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)     2704 2021-05-19 13:26:08.000000 board-game-recommender-3.3.0/README.md
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-06 19:41:30.909205 board-game-recommender-3.3.0/board_game_recommender/
+-rw-r--r--   0 markus     (501) staff       (20)      429 2023-04-11 10:14:59.000000 board-game-recommender-3.3.0/board_game_recommender/__init__.py
+-rw-r--r--   0 markus     (501) staff       (20)     5544 2023-05-01 18:48:43.000000 board-game-recommender-3.3.0/board_game_recommender/__main__.py
+-rw-r--r--   0 markus     (501) staff       (20)       78 2023-05-06 19:40:57.000000 board-game-recommender-3.3.0/board_game_recommender/__version__.py
+-rw-r--r--   0 markus     (501) staff       (20)     2124 2023-04-30 20:00:56.000000 board-game-recommender-3.3.0/board_game_recommender/base.py
+-rw-r--r--   0 markus     (501) staff       (20)     7041 2023-05-02 19:45:34.000000 board-game-recommender-3.3.0/board_game_recommender/baseline.py
+-rw-r--r--   0 markus     (501) staff       (20)     3043 2023-05-06 19:40:40.000000 board-game-recommender-3.3.0/board_game_recommender/evaluation.py
+-rw-r--r--   0 markus     (501) staff       (20)     9584 2023-05-01 20:18:49.000000 board-game-recommender-3.3.0/board_game_recommender/hyperparameter.py
+-rw-r--r--   0 markus     (501) staff       (20)    10190 2023-05-06 19:40:40.000000 board-game-recommender-3.3.0/board_game_recommender/light.py
+-rw-r--r--   0 markus     (501) staff       (20)     4766 2023-04-11 10:14:59.000000 board-game-recommender-3.3.0/board_game_recommender/rankings.py
+-rw-r--r--   0 markus     (501) staff       (20)    33402 2023-05-02 19:47:04.000000 board-game-recommender-3.3.0/board_game_recommender/recommend.py
+-rw-r--r--   0 markus     (501) staff       (20)     2099 2023-04-11 10:14:59.000000 board-game-recommender-3.3.0/board_game_recommender/trust.py
+-rw-r--r--   0 markus     (501) staff       (20)     3767 2023-04-30 20:37:05.000000 board-game-recommender-3.3.0/board_game_recommender/utils.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-06 19:41:30.911793 board-game-recommender-3.3.0/board_game_recommender.egg-info/
+-rw-r--r--   0 markus     (501) staff       (20)     4074 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)      686 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/SOURCES.txt
+-rw-r--r--   0 markus     (501) staff       (20)        1 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/dependency_links.txt
+-rw-r--r--   0 markus     (501) staff       (20)       99 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/requires.txt
+-rw-r--r--   0 markus     (501) staff       (20)       23 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/top_level.txt
+-rw-r--r--   0 markus     (501) staff       (20)       38 2023-05-06 19:41:30.912912 board-game-recommender-3.3.0/setup.cfg
+-rwxr-xr-x   0 markus     (501) staff       (20)     4993 2023-04-30 20:00:56.000000 board-game-recommender-3.3.0/setup.py
```

### Comparing `board-game-recommender-3.2.0/LICENSE` & `board-game-recommender-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.2.0/PKG-INFO` & `board-game-recommender-3.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-recommender
-Version: 3.2.0
+Version: 3.3.0
 Summary: Board games recommender engine
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-recommender/blob/master/README.md
 Project-URL: Funding, https://paypal.me/mschepke
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0,<3.9.0
 Description-Content-Type: text/markdown
+Provides-Extra: evaluation
 Provides-Extra: full
 Provides-Extra: light
 Provides-Extra: trust
 License-File: LICENSE
 
 
 # 🎲 Board Game Recommender 👍
```

### Comparing `board-game-recommender-3.2.0/README.md` & `board-game-recommender-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.2.0/board_game_recommender/__main__.py` & `board-game-recommender-3.3.0/board_game_recommender/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,47 +13,75 @@
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 
 def _parse_args():
     parser = argparse.ArgumentParser(description="train board game recommender model")
     parser.add_argument("users", nargs="*", help="users to be recommended games")
     parser.add_argument(
-        "--bga", "-b", action="store_true", help="use Board Game Atlas data"
+        "--bga",
+        "-b",
+        action="store_true",
+        help="use Board Game Atlas data",
     )
     parser.add_argument("--model", "-m", help="model directory")
     parser.add_argument("--train", "-t", action="store_true", help="train a new model")
     parser.add_argument(
-        "--similarity", "-s", action="store_true", help="train a new similarity model"
+        "--num-factors",
+        "-n",
+        type=int,
+        default=32,
+        help="number of latent factors",
+    )
+    parser.add_argument(
+        "--similarity",
+        "-s",
+        action="store_true",
+        help="train a new similarity model",
     )
     parser.add_argument("--games-file", "-G", help="games file")
     parser.add_argument("--ratings-file", "-R", help="ratings file")
     parser.add_argument(
         "--side-data-columns",
         "-S",
         nargs="+",
         help="game features to use in recommender model",
     )
     parser.add_argument(
-        "--num-rec", "-n", type=int, default=10, help="number of games to recommend"
+        "--num-rec",
+        "-r",
+        type=int,
+        default=10,
+        help="number of games to recommend",
     )
     parser.add_argument(
         "--max-iterations",
         "-M",
         type=int,
         default=100,
         help="maximal number of training steps",
     )
     parser.add_argument(
-        "--diversity", "-d", type=float, default=0, help="diversity in recommendations"
+        "--diversity",
+        "-d",
+        type=float,
+        default=0,
+        help="diversity in recommendations",
     )
     parser.add_argument(
-        "--cooperative", "-c", action="store_true", help="recommend cooperative games"
+        "--cooperative",
+        "-c",
+        action="store_true",
+        help="recommend cooperative games",
     )
     parser.add_argument(
-        "--games", "-g", type=int, nargs="+", help="restrict to these games"
+        "--games",
+        "-g",
+        type=int,
+        nargs="+",
+        help="restrict to these games",
     )
     parser.add_argument("--players", "-p", type=int, help="player count")
     parser.add_argument("--complexity", "-C", type=float, nargs="+", help="complexity")
     parser.add_argument("--time", "-T", type=float, help="max playing time")
     parser.add_argument("--worst", "-w", action="store_true", help="show worst games")
     parser.add_argument(
         "--verbose",
@@ -77,27 +105,35 @@
 
     LOGGER.info(args)
 
     if args.bga:
         model_cls = BGARecommender
         model_dir = args.model or os.path.join(BASE_DIR, ".bga")
         games_file = args.games_file or os.path.join(
-            BASE_DIR, "results", "bga_GameItem.jl"
+            BASE_DIR,
+            "results",
+            "bga_GameItem.jl",
         )
         ratings_file = args.ratings_file or os.path.join(
-            BASE_DIR, "results", "bga_RatingItem.jl"
+            BASE_DIR,
+            "results",
+            "bga_RatingItem.jl",
         )
     else:
         model_cls = BGGRecommender
         model_dir = args.model or os.path.join(BASE_DIR, ".bgg")
         games_file = args.games_file or os.path.join(
-            BASE_DIR, "results", "bgg_GameItem.jl"
+            BASE_DIR,
+            "results",
+            "bgg_GameItem.jl",
         )
         ratings_file = args.ratings_file or os.path.join(
-            BASE_DIR, "results", "bgg_RatingItem.jl"
+            BASE_DIR,
+            "results",
+            "bgg_RatingItem.jl",
         )
 
     games_filters = {}
 
     if args.cooperative:
         games_filters["cooperative"] = True
 
@@ -118,14 +154,15 @@
 
     if args.train:
         recommender = model_cls.train_from_files(
             games_file=games_file,
             ratings_file=ratings_file,
             side_data_columns=args.side_data_columns,
             similarity_model=args.similarity,
+            num_factors=args.num_factors,
             max_iterations=args.max_iterations,
             verbose=bool(args.verbose),
         )
         recommender.save(model_dir)
     else:
         recommender = model_cls.load(model_dir)
```

### Comparing `board-game-recommender-3.2.0/board_game_recommender/base.py` & `board-game-recommender-3.3.0/board_game_recommender/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Abstract base recommender class."""
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, AbstractSet, Generic, Iterable, TypeVar, Union
 
+import numpy as np
+
 GameKeyType = TypeVar("GameKeyType")
 UserKeyType = TypeVar("UserKeyType")
 
 if TYPE_CHECKING:
     import pandas
     import turicreate
 
@@ -46,14 +48,22 @@
         self: "BaseGamesRecommender",
         users: Iterable[UserKeyType],
         **kwargs,
     ) -> DataFrame:
         """Recommend games for given users."""
 
     @abstractmethod
+    def recommend_as_numpy(
+        self: "BaseGamesRecommender",
+        users: Iterable[UserKeyType],
+        games: Iterable[GameKeyType],
+    ) -> np.ndarray:
+        """Recommend games for given users and games as a numpy array."""
+
+    @abstractmethod
     def recommend_similar(
         self: "BaseGamesRecommender",
         games: Iterable[GameKeyType],
         **kwargs,
     ) -> DataFrame:
         """Recommend games similar to the given ones."""
```

### Comparing `board-game-recommender-3.2.0/board_game_recommender/light.py` & `board-game-recommender-3.3.0/board_game_recommender/light.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, FrozenSet, Iterable, List, Optional, Type, Union
 
 import numpy as np
 import pandas as pd
 
 from board_game_recommender.base import BaseGamesRecommender
+from board_game_recommender.baseline import dataframe_from_scores
 
 LOGGER = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     import turicreate
 
 RecommenderModel = Union[
@@ -22,20 +23,20 @@
 
 
 @dataclass(frozen=True)
 class CollaborativeFilteringData:
     """Labels, vectors and matrices for linear collaborative filtering models."""
 
     intercept: float
-    users_labels: np.ndarray
-    users_linear_terms: np.ndarray
-    users_factors: np.ndarray
-    items_labels: np.ndarray
-    items_linear_terms: np.ndarray
-    items_factors: np.ndarray
+    users_labels: np.ndarray  # (num_users,)
+    users_linear_terms: np.ndarray  # (num_users,)
+    users_factors: np.ndarray  # (num_users, num_factors)
+    items_labels: np.ndarray  # (num_items,)
+    items_linear_terms: np.ndarray  # (num_items,)
+    items_factors: np.ndarray  # (num_factors, num_items)
 
     def to_npz(self: "CollaborativeFilteringData", file_path: Union[Path, str]) -> None:
         """Save data into an .npz file."""
 
         file_path = Path(file_path).resolve()
         LOGGER.info("Saving data as .npz to <%s>", file_path)
         with file_path.open(mode="wb") as file:
@@ -137,45 +138,67 @@
         self._known_users = frozenset(self.users_labels)
         return self._known_users
 
     @property
     def num_users(self: "LightGamesRecommender") -> int:
         return len(self.users_labels)
 
+    def _recommendation_scores(
+        self: "LightGamesRecommender",
+        users: Optional[List[str]] = None,
+        games: Optional[List[int]] = None,
+    ) -> np.ndarray:
+        """Calculate recommendations scores for certain users and games."""
+
+        if users:
+            user_ids = np.array([self.users_indexes[user] for user in users])
+            user_factors = self.users_factors[user_ids]
+            users_linear_terms = self.users_linear_terms[user_ids].reshape(-1, 1)
+        else:
+            user_factors = self.users_factors
+            users_linear_terms = self.users_linear_terms.reshape(-1, 1)
+
+        if games:
+            # TODO Unknown games will cause a key error. Instead, use the user's
+            # average predicted rating (user + global bias) for unknown games. (#57)
+            game_ids = np.array([self.items_indexes[game] for game in games])
+            items_factors = self.items_factors[:, game_ids]
+            items_linear_terms = self.items_linear_terms[game_ids].reshape(1, -1)
+        else:
+            items_factors = self.items_factors
+            items_linear_terms = self.items_linear_terms.reshape(1, -1)
+
+        return (
+            user_factors @ items_factors  # (num_users, num_items)
+            + users_linear_terms  # (num_users, 1)
+            + items_linear_terms  # (1, num_items)
+            + self.intercept  # (1,)
+        )
+
     def recommend(
         self: "LightGamesRecommender",
         users: Iterable[str],
         **kwargs,
     ) -> pd.DataFrame:
         """Calculate recommendations for certain users."""
 
         users = list(users)
-        user_ids = np.array([self.users_indexes[user] for user in users])
-
-        scores = (
-            self.users_factors[user_ids] @ self.items_factors
-            + self.users_linear_terms[user_ids].reshape(len(user_ids), 1)
-            + self.items_linear_terms
-            + self.intercept
-        )
-
-        result = pd.DataFrame(
-            index=self.items_labels,
-            columns=pd.MultiIndex.from_product([users, ["score"]]),
-            data=scores.T,
-        )
-        result[pd.MultiIndex.from_product([users, ["rank"]])] = result.rank(
-            method="min",
-            ascending=False,
-        ).astype(int)
+        scores = self._recommendation_scores(users=users)
+        return dataframe_from_scores(users, self.items_labels, scores)
 
-        if len(users) == 1:
-            result.sort_values((users[0], "rank"), inplace=True)
+    def recommend_as_numpy(
+        self: "LightGamesRecommender",
+        users: Iterable[str],
+        games: Iterable[int],
+    ) -> np.ndarray:
+        """Calculate recommendations for certain users and games as a numpy array."""
 
-        return result[pd.MultiIndex.from_product([users, ["score", "rank"]])]
+        users = list(users)
+        games = list(games)
+        return self._recommendation_scores(users=users, games=games)
 
     def recommend_similar(
         self: "LightGamesRecommender",
         games: Iterable[int],
         **kwargs,
     ) -> pd.DataFrame:
         """
@@ -202,29 +225,15 @@
         """Find games similar to the given games based on cosine similarity of latent factors."""
 
         games = list(games)
         game_ids = np.array([self.items_indexes[game] for game in games])
         game_factors = self.items_factors[:, game_ids]
 
         scores = cosine_similarity(game_factors, self.items_factors)
-
-        result = pd.DataFrame(
-            index=self.items_labels,
-            columns=pd.MultiIndex.from_product([games, ["score"]]),
-            data=scores.T,
-        )
-        result[pd.MultiIndex.from_product([games, ["rank"]])] = result.rank(
-            method="min",
-            ascending=False,
-        ).astype(int)
-
-        if len(games) == 1:
-            result.sort_values((games[0], "rank"), inplace=True)
-
-        return result[pd.MultiIndex.from_product([games, ["score", "rank"]])]
+        return dataframe_from_scores(games, self.items_labels, scores)
 
 
 def cosine_similarity(matrix_1: np.ndarray, matrix_2: np.ndarray) -> np.ndarray:
     """
     Calculates the cosine similarity between two matrices.
 
     The input matrices need to be of shape (m,n) and (m,l); the result shape will be (n,l).
```

### Comparing `board-game-recommender-3.2.0/board_game_recommender/rankings.py` & `board-game-recommender-3.3.0/board_game_recommender/rankings.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.2.0/board_game_recommender/recommend.py` & `board-game-recommender-3.3.0/board_game_recommender/recommend.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import sys
 import tempfile
 
 # from datetime import date
 from typing import Any, Dict, FrozenSet, Iterable, Optional, Tuple, Type
 
+import numpy as np
 import turicreate as tc
 from pytility import arg_to_iter, clear_list
 
 from board_game_recommender.base import BaseGamesRecommender, GameKeyType, UserKeyType
 from board_game_recommender.utils import (
     condense_csv,
     filter_sframe,
@@ -55,30 +56,34 @@
         tdata[tar] = tdata[tar].apply(
             lambda x: [i for i in map(_convert, x or ()) if i is not None],
             dtype=list,
             skip_na=True,
         )
 
         tdata = tdata.stack(
-            column_name=tar, new_column_name=tar, new_column_type=tdt, drop_na=True
+            column_name=tar,
+            new_column_name=tar,
+            new_column_type=tdt,
+            drop_na=True,
         )
 
         if not tdata:
             continue
 
         graph = graph.add_edges(edges=tdata, src_field=item_id, dst_field=tar)
 
         del tdata, _convert
 
     if not graph.edges:
         return tc.SArray(dtype=list)
 
     components_model = tc.connected_components.create(graph)
     clusters = components_model.component_id.groupby(
-        "component_id", {"cluster": tc.aggregate.CONCAT("__id")}
+        "component_id",
+        {"cluster": tc.aggregate.CONCAT("__id")},
     )["cluster"]
 
     return clusters.filter(lambda x: x is not None and len(x) > 1)
 
 
 class GamesRecommender(BaseGamesRecommender):
     """games recommender"""
@@ -273,22 +278,24 @@
         exclude_compilations=True,
     ):
         if exclude_known and self.ratings:
             for user in users:
                 if not user:
                     continue
                 rated = self.ratings.filter_by([user], self.user_id_field)[
-                    self.id_field, self.user_id_field
+                    self.id_field,
+                    self.user_id_field,
                 ]
                 exclude = rated.copy() if exclude is None else exclude.append(rated)
                 del rated
 
         if exclude_clusters and exclude:
             grouped = exclude.groupby(
-                self.user_id_field, {"game_ids": tc.aggregate.CONCAT(self.id_field)}
+                self.user_id_field,
+                {"game_ids": tc.aggregate.CONCAT(self.id_field)},
             )
             for user, game_ids in zip(grouped[self.user_id_field], grouped["game_ids"]):
                 game_ids = frozenset(game_ids)
                 if not user or not game_ids:
                     continue
                 game_ids = {
                     linked
@@ -296,28 +303,32 @@
                     for linked in self.cluster(game_id)
                     if linked not in game_ids
                 }
                 clusters = tc.SFrame(
                     {
                         self.id_field: tc.SArray(list(game_ids), dtype=self.id_type),
                         self.user_id_field: tc.SArray.from_const(
-                            user, len(game_ids), self.user_id_type
+                            user,
+                            len(game_ids),
+                            self.user_id_type,
                         ),
                     }
                 )
                 exclude = exclude.append(clusters)
                 del clusters
             del grouped
 
         # pylint: disable=len-as-condition
         if exclude_compilations and len(self.compilations):
             comp = tc.SFrame({self.id_field: self.compilations})
             for user in users:
                 comp[self.user_id_field] = tc.SArray.from_const(
-                    user, len(self.compilations), self.user_id_type
+                    user,
+                    len(self.compilations),
+                    self.user_id_type,
                 )
                 exclude = comp.copy() if exclude is None else exclude.append(comp)
             del comp
 
         return exclude
 
     def _post_process_games(
@@ -340,15 +351,14 @@
             games["stars"] = [
                 star_rating(score=score, buckets=buckets, low=1.0, high=5.0)
                 for score in games["score"]
             ]
 
         return games.sort(sort_by, ascending=ascending)[columns]
 
-    # pylint: disable=no-self-use
     def process_user_id(self: "GamesRecommender", user_id):
         """process user ID"""
         return user_id or None
 
     def recommend(
         self: "GamesRecommender",
         users: Iterable[UserKeyType],
@@ -424,14 +434,53 @@
             sort_by=[self.user_id_field, "rank"]
             if self.user_id_field in columns
             else "rank",
             star_percentiles=star_percentiles,
             ascending=ascending,
         )
 
+    def recommend_as_numpy(
+        self: "GamesRecommender",
+        users: Iterable[str],
+        games: Iterable[int],
+    ) -> np.ndarray:
+        """Calculate recommendations for certain users and games as a numpy array."""
+
+        users = list(users)
+        users_sf = tc.SFrame(
+            {
+                self.user_id_field: users,
+                "sort_users": range(len(users)),
+            }
+        )
+
+        games = list(games)
+        games_sf = tc.SFrame(
+            {
+                self.id_field: games,
+                "sort_games": range(len(games)),
+            }
+        )
+
+        recommendations = self.model.recommend(
+            users=users,
+            items=games,
+            exclude_known=False,
+            k=len(games),
+        )
+
+        assert len(recommendations) == len(users) * len(games)
+
+        result = (
+            recommendations.join(users_sf)
+            .join(games_sf)
+            .sort(["sort_users", "sort_games"])
+        )
+        return result["score"].to_numpy().reshape(len(users), len(games))
+
     def recommend_similar(
         self: "GamesRecommender",
         games: Iterable[GameKeyType],
         *,
         items=None,
         games_filters=None,
         threshold=0.001,
@@ -450,27 +499,31 @@
         columns = list(arg_to_iter(columns)) or ["rank", "name", self.id_field, "score"]
 
         model = self.similarity_model or self.model
 
         self.logger.debug("recommending games similar to %s using %s", games, model)
 
         recommendations = model.recommend_from_interactions(
-            observed_items=games, items=items, **kwargs
+            observed_items=games,
+            items=items,
+            **kwargs,
         )
 
         recommendations = (
             recommendations[recommendations["score"] >= threshold]
             if threshold
             else recommendations
         )
 
         del games, items, model
 
         return self._post_process_games(
-            games=recommendations, columns=columns, join_on=self.id_field
+            games=recommendations,
+            columns=columns,
+            join_on=self.id_field,
         )
 
     def similar_games(
         self: "GamesRecommender",
         games: Iterable[GameKeyType],
         *,
         num_games=10,
@@ -666,16 +719,18 @@
         )
 
     @classmethod
     def train(
         cls,
         games,
         ratings,
+        *,
         side_data_columns=None,
         similarity_model=False,
+        num_factors=32,
         max_iterations=100,
         verbose=False,
         defaults=True,
         **filters,
     ):
         """train recommender from data"""
 
@@ -689,26 +744,32 @@
         all_games = games
         games = filter_sframe(games[columns].dropna(), **filters)
 
         side_data_columns = list(arg_to_iter(side_data_columns))
         if cls.id_field not in side_data_columns:
             side_data_columns.append(cls.id_field)
         if len(side_data_columns) > 1:
-            LOGGER.info("using game side features: %r", side_data_columns)
+            cls.logger.info("using game side features: %r", side_data_columns)
             item_data = all_games[side_data_columns].dropna()
         else:
             item_data = None
 
         ratings_filtered = ratings.filter_by(games[cls.id_field], cls.id_field)
 
+        cls.logger.info(
+            "Using %d latent factors in collaborative filtering",
+            num_factors,
+        )
+
         model = tc.ranking_factorization_recommender.create(
             observation_data=ratings_filtered,
             user_id=cls.user_id_field,
             item_id=cls.id_field,
             target=cls.rating_id_field,
+            num_factors=num_factors,
             item_data=item_data,
             max_iterations=max_iterations,
             verbose=verbose,
         )
 
         sim_model = (
             tc.item_similarity_recommender.create(
@@ -720,46 +781,53 @@
                 verbose=verbose,
             )
             if similarity_model
             else None
         )
 
         return cls(
-            model=model, similarity_model=sim_model, games=all_games, ratings=ratings
+            model=model,
+            similarity_model=sim_model,
+            games=all_games,
+            ratings=ratings,
         )
 
     @classmethod
     def load_games_csv(cls, games_csv, columns=None):
         """load games from CSV"""
 
         columns = cls.columns_games if columns is None else columns
         _, csv_cond = tempfile.mkstemp(text=True)
         num_games = condense_csv(games_csv, csv_cond, columns.keys())
 
         cls.logger.info("condensed %d games into <%s>", num_games, csv_cond)
 
         games = tc.SFrame.read_csv(
-            csv_cond, column_type_hints=columns, usecols=columns.keys()
+            csv_cond,
+            column_type_hints=columns,
+            usecols=columns.keys(),
         )
 
         try:
             os.remove(csv_cond)
         except Exception as exc:
             cls.logger.exception(exc)
 
         if cls.compilation_field in columns:
             # pylint: disable=unexpected-keyword-arg
             games[cls.compilation_field] = games[cls.compilation_field].apply(
-                bool, skip_na=False
+                bool,
+                skip_na=False,
             )
 
         if cls.cooperative_field in columns:
             # pylint: disable=unexpected-keyword-arg
             games[cls.cooperative_field] = games[cls.cooperative_field].apply(
-                bool, skip_na=False
+                bool,
+                skip_na=False,
             )
 
         return games
 
     @classmethod
     def load_games_json(cls, games_json, columns=None, orient="lines"):
         """load games from JSON"""
@@ -772,20 +840,22 @@
         for col in columns:
             if col not in games.column_names():
                 games[col] = None
 
         if cls.compilation_field in games.column_names():
             # pylint: disable=unexpected-keyword-arg
             games[cls.compilation_field] = games[cls.compilation_field].apply(
-                bool, skip_na=False
+                bool,
+                skip_na=False,
             )
 
         if cls.cooperative_field in games.column_names():
             games[cls.cooperative_field] = games[cls.cooperative_field].apply(
-                bool, skip_na=False
+                bool,
+                skip_na=False,
             )
 
         return games
 
     # pylint: disable=unused-argument
     @classmethod
     def process_ratings(cls, ratings, **kwargs):
@@ -794,15 +864,17 @@
 
     @classmethod
     def load_ratings_csv(cls, ratings_csv, columns=None, **kwargs):
         """load ratings from CSV"""
 
         columns = cls.columns_ratings if columns is None else columns
         ratings = tc.SFrame.read_csv(
-            ratings_csv, column_type_hints=columns, usecols=columns.keys()
+            ratings_csv,
+            column_type_hints=columns,
+            usecols=columns.keys(),
         ).dropna()
 
         return cls.process_ratings(ratings, **kwargs)
 
     @classmethod
     def load_ratings_json(cls, ratings_json, columns=None, orient="lines", **kwargs):
         """load ratings from JSON"""
@@ -818,46 +890,53 @@
         cls,
         games_file,
         ratings_file,
         games_columns=None,
         ratings_columns=None,
         side_data_columns=None,
         similarity_model=False,
+        num_factors=32,
         max_iterations=100,
         verbose=False,
         defaults=True,
         **filters,
     ):
         """load data from JSON or CSV and train recommender"""
 
         games_format = format_from_path(games_file)
         if games_format == "csv":
             games = cls.load_games_csv(games_csv=games_file, columns=games_columns)
         else:
             orient = "records" if games_format == "json" else "lines"
             games = cls.load_games_json(
-                games_json=games_file, columns=games_columns, orient=orient
+                games_json=games_file,
+                columns=games_columns,
+                orient=orient,
             )
 
         ratings_format = format_from_path(ratings_file)
         if ratings_format == "csv":
             ratings = cls.load_ratings_csv(
-                ratings_csv=ratings_file, columns=ratings_columns
+                ratings_csv=ratings_file,
+                columns=ratings_columns,
             )
         else:
             orient = "records" if ratings_format == "json" else "lines"
             ratings = cls.load_ratings_json(
-                ratings_json=ratings_file, columns=ratings_columns, orient=orient
+                ratings_json=ratings_file,
+                columns=ratings_columns,
+                orient=orient,
             )
 
         return cls.train(
             games=games,
             ratings=ratings,
             side_data_columns=side_data_columns,
             similarity_model=similarity_model,
+            num_factors=num_factors,
             max_iterations=max_iterations,
             verbose=verbose,
             defaults=defaults,
             **filters,
         )
 
     def __str__(self):
@@ -937,15 +1016,16 @@
                 dtype=cls.user_id_type,
                 skip_na=True,
             )
 
         if kwargs.get("dedupe") and cls.rating_id_field in ratings.column_names():
             ratings = ratings.unstack(cls.rating_id_field, "ratings")
             ratings[cls.rating_id_field] = ratings["ratings"].apply(
-                lambda x: x[-1], dtype=float
+                lambda x: x[-1],
+                dtype=float,
             )
             del ratings["ratings"]
 
         return ratings
 
 
 class BGARecommender(GamesRecommender):
```

### Comparing `board-game-recommender-3.2.0/board_game_recommender/trust.py` & `board-game-recommender-3.3.0/board_game_recommender/trust.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.2.0/board_game_recommender/utils.py` & `board-game-recommender-3.3.0/board_game_recommender/utils.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.2.0/board_game_recommender.egg-info/PKG-INFO` & `board-game-recommender-3.3.0/board_game_recommender.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-recommender
-Version: 3.2.0
+Version: 3.3.0
 Summary: Board games recommender engine
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-recommender/blob/master/README.md
 Project-URL: Funding, https://paypal.me/mschepke
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0,<3.9.0
 Description-Content-Type: text/markdown
+Provides-Extra: evaluation
 Provides-Extra: full
 Provides-Extra: light
 Provides-Extra: trust
 License-File: LICENSE
 
 
 # 🎲 Board Game Recommender 👍
```

### Comparing `board-game-recommender-3.2.0/board_game_recommender.egg-info/SOURCES.txt` & `board-game-recommender-3.3.0/board_game_recommender.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 MANIFEST.in
 README.md
 setup.py
 board_game_recommender/__init__.py
 board_game_recommender/__main__.py
 board_game_recommender/__version__.py
 board_game_recommender/base.py
+board_game_recommender/baseline.py
+board_game_recommender/evaluation.py
+board_game_recommender/hyperparameter.py
 board_game_recommender/light.py
 board_game_recommender/rankings.py
 board_game_recommender/recommend.py
 board_game_recommender/trust.py
 board_game_recommender/utils.py
 board_game_recommender.egg-info/PKG-INFO
 board_game_recommender.egg-info/SOURCES.txt
```

### Comparing `board-game-recommender-3.2.0/setup.py` & `board-game-recommender-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,21 @@
 URL_TWITTER = "https://twitter.com/recommend_games"
 EMAIL = "markus@recommend.games"
 AUTHOR = "Markus Shepherd"
 REQUIRES_PYTHON = ">=3.7.0,<3.9.0"
 VERSION = None  # will be read from __version__.py
 
 # What packages are required for this module to be executed?
-REQUIRED = ()
+REQUIRED = ("numpy",)
 
 # What packages are optional?
 EXTRAS = {
+    "evaluation": ("polars", "scikit-learn"),
     "full": ("pytility", "turicreate"),
-    "light": ("numpy", "pandas"),
+    "light": ("pandas",),
     "trust": ("scipy",),
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

