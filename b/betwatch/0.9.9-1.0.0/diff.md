# Comparing `tmp/betwatch-0.9.9.tar.gz` & `tmp/betwatch-1.0.0.tar.gz`

## Comparing `betwatch-0.9.9.tar` & `betwatch-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-0.9.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-0.9.9/.github/dependabot.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 betwatch-0.9.9/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/__about__.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/__init__.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/client.py
--rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/client_async.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/filters.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/markets.py
--rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 betwatch-0.9.9/betwatch/types/race.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_race_prices.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_races.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/get_races_async.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 betwatch-0.9.9/examples/subscriptions.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_race.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_race_async.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_races.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 betwatch-0.9.9/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 betwatch-0.9.9/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-0.9.9/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-0.9.9/README.md
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 betwatch-0.9.9/pyproject.toml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 betwatch-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.0/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/client.py
+-rw-r--r--   0        0        0    26463 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/types/markets.py
+-rw-r--r--   0        0        0    11720 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.0/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.0/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.0/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.0/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.0/examples/get_races_async.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.0/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.0/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.0/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.0/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.0/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.0/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.0/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 betwatch-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.0/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.0/PKG-INFO
```

### Comparing `betwatch-0.9.9/.github/workflows/test.yml` & `betwatch-1.0.0/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   cancel-in-progress: true
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `betwatch-0.9.9/betwatch/client.py` & `betwatch-1.0.0/betwatch/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import atexit
 import logging
 from datetime import datetime, timedelta
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 import backoff
 import typedload
 from gql import Client
 from gql.transport.exceptions import TransportQueryError
 from gql.transport.requests import RequestsHTTPTransport
 from gql.transport.requests import log as http_logger
 from graphql import DocumentNode
 
 from betwatch.__about__ import __version__
 from betwatch.queries import (
+    MUTATION_UPDATE_USER_EVENT_DATA,
     QUERY_GET_LAST_SUCCESSFUL_PRICE_UPDATE,
     query_get_race,
     query_get_races,
 )
 from betwatch.types import Bookmaker, Race, RaceProjection
 from betwatch.types.filters import RacesFilter
+from betwatch.types.updates import SelectionData
 
 
 class BetwatchClient:
-    def __init__(self, api_key: str, transport_logging_level: int = logging.WARNING):
+    def __init__(
+        self,
+        api_key: str,
+        transport_logging_level: int = logging.WARNING,
+        host="api.betwatch.com",
+    ):
         self.api_key = api_key
         self._gql_transport = RequestsHTTPTransport(
-            url="https://api.betwatch.com/query",
+            url=f"https://{host}/query",
             headers={
                 "X-API-KEY": self.api_key,
                 "User-Agent": f"betwatch-python-{__version__}",
             },
             timeout=30,
         )
         # Create a GraphQL client using the defined transport
@@ -50,84 +57,93 @@
         self._gql_client.close_sync()
         self._gql_transport.close()
 
     def get_races_between_dates(
         self,
         date_from: Union[str, datetime],
         date_to: Union[str, datetime],
-        projection=RaceProjection(),
-        filter=RacesFilter(),
+        projection: Optional[RaceProjection] = None,
+        filter: Optional[RacesFilter] = None,
     ) -> List[Race]:
         """Get a list of races in between two dates.
 
         Args:
             date_from (Union[str, datetime]): Date to start from (inclusive)
             date_to (Union[str, datetime]): Date to end at (inclusive   )
             projection (_type_, optional): The fields to return. Defaults to RaceProjection().
             filter (_type_, optional): Filter the results. Defaults to RacesFilter().
 
         Returns:
             List[Race]: List of races that match the criteria
         """
+        # handle defaults
+        if not projection:
+            projection = RaceProjection()
+        if not filter:
+            filter = RacesFilter()
+
         if isinstance(date_from, datetime):
             date_from = date_from.strftime("%Y-%m-%d")
         if isinstance(date_to, datetime):
             date_to = date_to.strftime("%Y-%m-%d")
 
         # prefer the date_from and date_to passed into the function
         if filter.date_from and filter.date_from != date_from:
-            logging.warning(
+            logging.debug(
                 f"Overriding date_from in filter ({filter.date_from} with {date_from})"
             )
-            filter.date_from = datetime.strptime(date_from, "%Y-%m-%d")
+            filter.date_from = date_from
         if filter.date_to and filter.date_to != date_to:
-            logging.warning(
+            logging.debug(
                 f"Overriding date_to in filter ({filter.date_to} with {date_to})"
             )
-            filter.date_to = datetime.strptime(date_to, "%Y-%m-%d")
+            filter.date_to = date_to
         return self.get_races(projection, filter)
 
     def get_races(
         self,
-        projection=RaceProjection(),
-        filter=RacesFilter(),
+        projection: Optional[RaceProjection] = None,
+        filter: Optional[RacesFilter] = None,
     ) -> List[Race]:
+        # handle defaults
+        if not projection:
+            projection = RaceProjection()
+        if not filter:
+            filter = RacesFilter()
+
         try:
             logging.info(
                 f"Getting races with projection {projection} and filter {filter}"
             )
 
             done = False
             races: List[Race] = []
             # iterate until no more races are found
             while not done:
-
                 query = query_get_races(projection)
 
                 variables = filter.to_dict()
 
                 result = self._gql_client.execute(query, variable_values=variables)
 
                 if result.get("races"):
-                    logging.debug(
-                        f"Received {len(result['races'])} races - attempting to get more"
+                    logging.info(
+                        f"Received {len(result['races'])} races - attempting to get more..."
                     )
                     races.extend(typedload.load(result["races"], List[Race]))
 
                     # change the offset to the next page
                     filter.offset += filter.limit
                 else:
                     filter.offset = 0
                     logging.debug("No more races found")
                     done = True
 
             return races
-        # except (ClientError, HTTPClientError, HTTPServerError) as e:
-        #     logging.warning(f"Error reaching Betwatch API: {e}")
-        #     raise e
+
         except TransportQueryError as e:
             if e.errors:
                 for error in e.errors:
                     msg = error.get("message")
                     if msg:
                         # sometimes we can provide better feedback
                         if "limit argument" in msg:
@@ -145,35 +161,84 @@
                     else:
                         logging.error(f"{error}")
             else:
                 logging.error(f"Error querying Betwatch API: {e}")
             return []
 
     def get_race(
-        self, race_id: str, projection=RaceProjection(markets=True)
+        self, race_id: str, projection: Optional[RaceProjection] = None
     ) -> Union[Race, None]:
+        # handle defaults
+        if not projection:
+            projection = RaceProjection(markets=True)
         query = query_get_race(projection)
-        return self._get_race_by_id(race_id, query)
 
-    def get_races_today(self, projection=RaceProjection()) -> List[Race]:
+        return self._get_race_by_id(
+            race_id,
+            query,
+        )
+
+    def get_races_today(
+        self, projection: Optional[RaceProjection] = None
+    ) -> List[Race]:
         """Get all races for today."""
-        today = datetime.now().strftime("%Y-%m-%d")
-        tomorrow = (datetime.now() + timedelta(days=0)).strftime("%Y-%m-%d")
+        today = datetime.now()
+        tomorrow = datetime.now() + timedelta(days=0)
         return self.get_races_between_dates(today, tomorrow, projection)
 
     @backoff.on_exception(backoff.expo, Exception, max_time=60, max_tries=5)
-    def _get_race_by_id(self, race_id: str, query: DocumentNode) -> Union[Race, None]:
+    def _get_race_by_id(
+        self,
+        race_id: str,
+        query: DocumentNode,
+    ) -> Union[Race, None]:
         logging.info(f"Getting race (id={race_id})")
-        variables = {"id": race_id}
+
+        variables = {
+            "id": race_id,
+        }
         result = self._gql_client.execute(query, variable_values=variables)
 
         if result.get("race"):
             return typedload.load(result["race"], Race)
         return None
 
+    def update_event_data(
+        self, race_id: str, column_name: str, data: List[SelectionData]
+    ):
+        """
+        Updates event data for a given race ID.
+
+        Args:
+            race_id (str): race id to be checked
+            column_name (str): name of the column to be updated
+            data (List[SelectionData]): list of selection data to be updated
+        """
+
+        logging.info(f"Updating event data (id={race_id})")
+        selection_data = [
+            {"selectionId": d["selection_id"], "value": str(d["value"])} for d in data
+        ]
+
+        if not selection_data:
+            raise ValueError("Cannot update event data with empty selection data")
+
+        res = self._gql_client.execute(
+            MUTATION_UPDATE_USER_EVENT_DATA,
+            variable_values={
+                "input": {
+                    "eventId": race_id,
+                    "customData": [
+                        {"columnName": column_name, "selectionData": selection_data}
+                    ],
+                }
+            },
+        )
+        logging.debug(res)
+
     def get_race_last_updated_times(self, race_id: str) -> Dict[Bookmaker, datetime]:
         """Get the last time each bookmaker was checked for a price update.
            This does not mean that the price was updated, just that the bookmaker was checked.
 
         Args:
             race_id (str): race id to be checked
```

### Comparing `betwatch-0.9.9/betwatch/client_async.py` & `betwatch-1.0.0/betwatch/client_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import atexit
 import logging
 from datetime import datetime, timedelta
 from time import monotonic
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import backoff
 import typedload
 from aiohttp.client_exceptions import ClientError
 from aiohttp.web_exceptions import HTTPClientError, HTTPServerError
 from gql import Client
 from gql.client import AsyncClientSession, ReconnectingAsyncClientSession
@@ -17,14 +17,15 @@
 from gql.transport.websockets import WebsocketsTransport
 from gql.transport.websockets import log as websockets_logger
 from graphql import DocumentNode
 from typedload.exceptions import TypedloadException
 
 from betwatch.__about__ import __version__
 from betwatch.queries import (
+    MUTATION_UPDATE_USER_EVENT_DATA,
     QUERY_GET_LAST_SUCCESSFUL_PRICE_UPDATE,
     SUBSCRIPTION_BETFAIR_UPDATES,
     SUBSCRIPTION_RACES_UPDATES,
     query_get_race,
     query_get_races,
     subscription_race_price_updates,
 )
@@ -34,20 +35,33 @@
     BookmakerMarket,
     Race,
     RaceProjection,
     RaceUpdate,
     SubscriptionUpdate,
 )
 from betwatch.types.filters import RacesFilter
+from betwatch.types.updates import SelectionData
 
 
 class BetwatchAsyncClient:
-    def __init__(self, api_key: str, transport_logging_level: int = logging.WARNING):
+    def __init__(
+        self,
+        api_key: str,
+        transport_logging_level: int = logging.WARNING,
+        host="api.betwatch.com",
+    ):
         self.api_key = api_key
 
+        self._gql_sub_transport: WebsocketsTransport
+        self._gql_transport: AIOHTTPTransport
+        self._gql_sub_client: Client
+        self._gql_client: Client
+
+        self._host = host
+
         self.connect()
 
         self._http_session: Union[
             None, ReconnectingAsyncClientSession, AsyncClientSession
         ] = None
 
         # flag to indicate if we have entered the context manager
@@ -65,31 +79,31 @@
         self._session_lock = asyncio.Lock()
 
         self._subscription_queue: asyncio.Queue[SubscriptionUpdate] = asyncio.Queue()
         self._subscriptions_betfair: Dict[str, asyncio.Task] = {}
         self._subscriptions_prices: Dict[str, asyncio.Task] = {}
         self._subscriptions_updates: Dict[Tuple[str, str], asyncio.Task] = {}
 
-        self._monitor_task: asyncio.Task | None = None
+        self._monitor_task: Union[asyncio.Task, None] = None
         self._last_reconnect: float = monotonic()
 
     def connect(self):
         logging.debug("connecting to client sessions")
         self._gql_sub_transport = WebsocketsTransport(
-            url="wss://api.betwatch.com/sub",
+            url=f"wss://{self._host}/sub",
             headers={
                 "X-API-KEY": self.api_key,
                 "User-Agent": f"betwatch-sdk-python-{__version__}",
             },
             init_payload={"apiKey": self.api_key},
             pong_timeout=60,
             ping_interval=5,
         )
         self._gql_transport = AIOHTTPTransport(
-            url="https://api.betwatch.com/query",
+            url=f"https://{self._host}/query",
             headers={
                 "X-API-KEY": self.api_key,
                 "User-Agent": f"betwatch-sdk-python-{__version__}",
             },
         )
         # Create a GraphQL client using the defined transport
         self._gql_sub_client = Client(
@@ -164,66 +178,84 @@
         """Setup the HTTP session."""
         async with self._session_lock:
             if not self._http_session:
                 self._http_session = await self._gql_client.connect_async()
         return self._http_session
 
     async def get_races_today(
-        self, projection=RaceProjection(), filter=RacesFilter()
+        self,
+        projection: Optional[RaceProjection] = None,
+        filter: Optional[RacesFilter] = None,
     ) -> List[Race]:
         """Get all races for today."""
+        # set defaults
+        if not projection:
+            projection = RaceProjection()
+        if not filter:
+            filter = RacesFilter()
+
         today = datetime.today().strftime("%Y-%m-%d")
         tomorrow = (datetime.today() + timedelta(days=0)).strftime("%Y-%m-%d")
-        return await self.get_races_between_dates(today, tomorrow, projection, filter)
+        return await self.get_races_between_dates(
+            today, tomorrow, projection=projection, filter=filter
+        )
 
     async def get_races_between_dates(
         self,
         date_from: Union[str, datetime],
         date_to: Union[str, datetime],
-        projection=RaceProjection(),
-        filter=RacesFilter(),
+        projection: Optional[RaceProjection] = None,
+        filter: Optional[RacesFilter] = None,
     ) -> List[Race]:
         """Get a list of races in between two dates.
 
         Args:
             date_from (Union[str, datetime]): Date to start from (inclusive)
             date_to (Union[str, datetime]): Date to end at (inclusive   )
             projection (_type_, optional): The fields to return. Defaults to RaceProjection().
             filter (_type_, optional): The filter to apply. Defaults to RacesFilter().
 
         Returns:
             List[Race]: List of races that match the criteria
         """
+        # set defaults
+        if not projection:
+            projection = RaceProjection()
+        if not filter:
+            filter = RacesFilter()
+
         if isinstance(date_from, datetime):
             date_from = date_from.strftime("%Y-%m-%d")
         if isinstance(date_to, datetime):
             date_to = date_to.strftime("%Y-%m-%d")
 
         # prefer the date_from and date_to passed into the function
         if filter.date_from and filter.date_from != date_from:
-            logging.warning(
+            logging.debug(
                 f"Overriding date_from in filter ({filter.date_from} with {date_from})"
             )
-            filter.date_from = datetime.strptime(date_from, "%Y-%m-%d")
+            filter.date_from = date_from
         if filter.date_to and filter.date_to != date_to:
-            logging.warning(
+            logging.debug(
                 f"Overriding date_to in filter ({filter.date_to} with {date_to})"
             )
-            filter.date_to = datetime.strptime(date_to, "%Y-%m-%d")
+            filter.date_to = date_to
         return await self.get_races(projection, filter)
 
-    async def query_races(self, projection=RaceProjection(), filter=RacesFilter()):
-        pass
-
     @backoff.on_exception(backoff.expo, (ClientError, HTTPClientError, HTTPServerError))
     async def get_races(
         self,
-        projection=RaceProjection(),
-        filter=RacesFilter(),
+        projection: Optional[RaceProjection] = None,
+        filter: Optional[RacesFilter] = None,
     ) -> List[Race]:
+        # set defaults
+        if not projection:
+            projection = RaceProjection()
+        if not filter:
+            filter = RacesFilter()
         try:
             logging.info(
                 f"Getting races with projection {projection} and filter {filter}"
             )
 
             done = False
             races: List[Race] = []
@@ -234,16 +266,16 @@
                 query = query_get_races(projection)
 
                 variables = filter.to_dict()
 
                 result = await session.execute(query, variable_values=variables)
 
                 if result.get("races"):
-                    logging.debug(
-                        f"Received {len(result['races'])} races - attempting to get more"
+                    logging.info(
+                        f"Received {len(result['races'])} races - attempting to get more..."
                     )
                     races.extend(typedload.load(result["races"], List[Race]))
 
                     # change the offset to the next page
                     filter.offset += filter.limit
                 else:
                     filter.offset = 0
@@ -278,25 +310,28 @@
                     else:
                         logging.error(f"{error}")
             else:
                 logging.error(f"Error querying Betwatch API: {e}")
             return []
 
     async def get_race(
-        self, race_id: str, projection=RaceProjection(markets=True)
+        self, race_id: str, projection: Optional[RaceProjection] = None
     ) -> Union[Race, None]:
         """Get all details of a specific race by id.
 
         Args:
             race_id (str): The id of a race. This can be obtained from the `get_races` method.
             projection (RaceProjection, optional): The fields to return. Defaults to RaceProjection(markets=True).
 
         Returns:
             Union[Race, None]: The race object or None if the race is not found.
         """
+        # set defaults
+        if not projection:
+            projection = RaceProjection(markets=True)
         query = query_get_race(projection)
         return await self._get_race_by_id(race_id, query)
 
     async def _monitor(self):
         """Monitor the subscription tasks and restart them if they fail"""
         logging.debug("Starting subscription monitor")
         while True:
@@ -309,19 +344,24 @@
                 ]:
                     for key, task in d.items():
                         if task.done():
                             # check for errors
                             try:
                                 err = task.exception()
                                 if err:
-                                    logging.error(f"Error in subscription task: {err}")
+                                    logging.warning(f"Subscription task closed: {err}")
+                                    # reset the connection
+                                    if self._websocket_session:
+                                        await self.disconnect()
                             except asyncio.InvalidStateError:
                                 pass
 
-                            logging.info(f"Restarting subscription task for {key}")
+                            logging.warning(
+                                f"Retrying subscription task for {key if key else 'all races'}"
+                            )
 
                             # replace the task in the dict with a new one
                             if d == self._subscriptions_prices:
                                 d[key] = asyncio.create_task(
                                     self._subscribe_bookmaker_updates(key)
                                 )
                             elif d == self._subscriptions_updates:
@@ -335,15 +375,15 @@
 
                             # update last reconnect
                             self._last_reconnect = monotonic()
             except asyncio.CancelledError:
                 logging.debug("Subscription monitor cancelled")
                 return
             except Exception as e:
-                logging.error(f"Error in subscription monitor: {e}")
+                logging.debug(f"Error in subscription monitor: {e}")
                 raise e
 
     async def listen(self):
         """Subscribe to any updates from your subscriptions"""
         if (
             len(self._subscriptions_prices) < 1
             and len(self._subscriptions_betfair) < 1
@@ -401,46 +441,53 @@
         logging.info(
             f"Unsubscribed from {race_id if race_id else 'all races'} bookmaker updates"
         )
 
     async def subscribe_bookmaker_updates(
         self,
         race_id: str,
-        projection=RaceProjection(markets=True),
+        projection: Optional[RaceProjection] = None,
     ):
+        # set defaults
+        if not projection:
+            projection = RaceProjection(markets=True)
+
         if race_id in self._subscriptions_prices:
             logging.info(
                 f"Already subscribed to {race_id if race_id else 'all races'} bookmaker updates"
             )
             return
 
         # make sure the total subscriptions is less than 10
         if len(self._subscriptions_prices) >= 10:
             raise Exception(
                 "Cannot subscribe to more than 10 races at one time. Use an empty race_id to subscribe to all races in one subscription"
             )
-            return
 
         self._subscriptions_prices[race_id] = asyncio.create_task(
             self._subscribe_bookmaker_updates(race_id, projection)
         )
 
     async def _subscribe_bookmaker_updates(
         self,
         race_id: str,
-        projection=RaceProjection(markets=True),
+        projection: Optional[RaceProjection] = None,
     ):
         """Subscribe to price updates for a specific race.
 
         Args:
             race_id (str): The id of a specific race. This can be obtained from the `get_races` method.
 
         Yields:
             List[BookmakerMarket]: A list of bookmaker markets with updated prices.
         """
+        # set defaults
+        if not projection:
+            projection = RaceProjection(markets=True)
+
         try:
             session = await self._setup_websocket_session()
 
             query = subscription_race_price_updates(projection)
             variables = {"id": race_id}
 
             logging.info(
@@ -454,18 +501,20 @@
                         bookmaker_markets=typedload.load(
                             result["priceUpdates"], List[BookmakerMarket]
                         ),
                     )
 
                     self._subscription_queue.put_nowait(update)
         except TransportError as e:
-            logging.error(f"Error subscribing to bookmaker updates: {e}")
+            logging.debug(f"Error subscribing to bookmaker updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_bookmaker_updates(race_id)
             return
+        except Exception as e:
+            logging.error(f"Error subscribing to bookmaker updates: {e}")
 
     async def unsubscribe_betfair_updates(self, race_id: str):
         if race_id not in self._subscriptions_betfair:
             logging.info(
                 f"Not subscribed to {race_id if race_id else 'all races'} betfair updates"
             )
             return
@@ -522,15 +571,15 @@
                         betfair_markets=typedload.load(
                             result["betfairUpdates"], List[BetfairMarket]
                         ),
                     )
                     self._subscription_queue.put_nowait(update)
 
         except TransportError as e:
-            logging.error(f"Error subscribing to betfair updates: {e}")
+            logging.debug(f"Error subscribing to betfair updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_betfair_updates(race_id)
             return
 
     async def unsubscribe_race_updates(self, date_from: str, date_to: str):
         if (date_from, date_to) not in self._subscriptions_updates:
             logging.info(f"Not subscribed to races updates for {date_from} - {date_to}")
@@ -573,27 +622,63 @@
             logging.error(f"Error subscribing to race updates: {e}")
         except asyncio.CancelledError:
             await self.unsubscribe_race_updates(date_from, date_to)
             return
 
     @backoff.on_exception(backoff.expo, Exception, max_time=60, max_tries=5)
     async def _get_race_by_id(
-        self, race_id: str, query: DocumentNode
+        self,
+        race_id: str,
+        query: DocumentNode,
     ) -> Union[Race, None]:
         logging.info(f"Getting race (id={race_id})")
         session = await self._setup_http_session()
-
-        variables = {"id": race_id}
+        variables = {
+            "id": race_id,
+        }
 
         result = await session.execute(query, variable_values=variables)
 
         if result.get("race"):
             return typedload.load(result["race"], Race)
         return None
 
+    async def update_event_data(
+        self, race_id: str, column_name: str, data: List[SelectionData]
+    ):
+        """
+        Updates event data for a given race ID.
+
+        Args:
+            race_id (str): race id to be checked
+            column_name (str): name of the column to be updated
+            data (List[SelectionData]): list of selection data to be updated
+        """
+
+        logging.info(f"Updating event data (id={race_id})")
+        selection_data = [
+            {"selectionId": d["selection_id"], "value": str(d["value"])} for d in data
+        ]
+
+        if not selection_data:
+            raise ValueError("Cannot update event data with empty selection data")
+
+        res = await self._gql_client.execute_async(
+            MUTATION_UPDATE_USER_EVENT_DATA,
+            variable_values={
+                "input": {
+                    "eventId": race_id,
+                    "customData": [
+                        {"columnName": column_name, "selectionData": selection_data}
+                    ],
+                }
+            },
+        )
+        logging.debug(res)
+
     async def get_race_last_updated_times(
         self, race_id: str
     ) -> Dict[Bookmaker, datetime]:
         """Get the last time each bookmaker was checked for a price update.
            This does not mean that the price was updated, just that the bookmaker was checked.
 
         Args:
```

### Comparing `betwatch-0.9.9/betwatch/queries.py` & `betwatch-1.0.0/betwatch/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from gql import gql
 from graphql import DocumentNode
 
 from betwatch.types import RaceProjection
 
 
-def get_race_query(projection=RaceProjection()) -> str:
+def get_race_query(projection: RaceProjection) -> str:
     """Get a GQL query based on a projection."""
+
     bookmakers = (
         "["
-        + ",".join(['"' + bookmaker.value + '"' for bookmaker in projection.bookmakers])
+        + ",".join(['"' + str(bookmaker) + '"' for bookmaker in projection.bookmakers])
         + "]"
     )
 
+    if projection.flucs and projection.bookmakers:
+        bookmakers_with_flucs = bookmakers
+        bookmakers = '[""]'
+    else:
+        bookmakers_with_flucs = "[]"
+
     runners_gql = (
         "runners { id betfairId name number scratchedTime barrier trainerName riderName "
         + (
             "betfairMarkets { id sp marketName marketId totalMatched marketTotalMatched lastPriceTraded back { price size lastUpdated } lay { price size lastUpdated } } "
             if projection.betfair
             else ""
         )
         + (
             (
                 "bookmakerMarkets(bookmakers: "
                 + bookmakers
+                + ", bookmakersWithFlucs: "
+                + bookmakers_with_flucs
                 + ") { id bookmaker "
                 + "fixedWin { price lastUpdated "
                 + ("flucs { price lastUpdated } " if projection.flucs else "")
                 + "} "
                 + (
                     "fixedPlace { price lastUpdated "
                     + ("flucs { price lastUpdated } " if projection.flucs else "")
@@ -175,7 +184,24 @@
                 bookmaker
                 lastSuccessfulPriceUpdate
             }
         }
     }
     """
 )
+
+MUTATION_UPDATE_USER_EVENT_DATA = gql(
+    """
+    mutation UpdateUserEventData($input: UpdateUserEventDataInput!) {
+        updateUserEventData(input: $input) {
+            eventId
+            data {
+                columnName
+                selectionData {
+                    selectionId
+                    value
+                }
+            }
+        }
+    }
+    """
+)
```

### Comparing `betwatch-0.9.9/betwatch/types/bookmakers.py` & `betwatch-1.0.0/betwatch/types/bookmakers.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,10 +77,13 @@
     PICKLEBET = "Picklebet"
     BETGALAXY = "Betgalaxy"
     DIAMONDBET = "Diamondbet"
     BITWINNING = "Bitwinning"
     COMBET = "Combet"
     BETM = "BetM"
     ULTRABET = "Ultrabet"
+    THUNDERBET = "Thunderbet"
+    ESKANDERBET = "EskanderBet"
+    SPORTCHAMPS = "SportChamps"
 
     def __str__(self):
         return self.value
```

### Comparing `betwatch-0.9.9/betwatch/types/filters.py` & `betwatch-1.0.0/betwatch/types/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,70 @@
 from datetime import datetime
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 
 from betwatch.types.bookmakers import Bookmaker
 from betwatch.types.race import MeetingType
 
 
+def get_australian_states() -> List[str]:
+    """Return a list of Australian states."""
+    return [
+        "ACT",
+        "NSW",
+        "NT",
+        "QLD",
+        "SA",
+        "TAS",
+        "VIC",
+        "WA",
+    ]
+
+
 class RacesFilter:
     def __init__(
         self,
         limit: int = 100,
         offset: int = 0,
-        types: List[Union[MeetingType, str]] = [],
-        tracks: List[str] = [],
-        locations: List[str] = [],
-        has_bookmakers: List[Bookmaker] = [],
-        has_runners: List[str] = [],
-        has_trainers: List[str] = [],
-        has_riders: List[str] = [],
-        date_from: datetime = datetime.now(),
-        date_to: datetime = datetime.now(),
+        types: Optional[List[Union[MeetingType, str]]] = None,
+        tracks: Optional[List[str]] = None,
+        locations: Optional[Union[List[str], Literal["Australia"]]] = None,
+        has_bookmakers: Optional[List[Bookmaker]] = None,
+        has_runners: Optional[List[str]] = None,
+        has_trainers: Optional[List[str]] = None,
+        has_riders: Optional[List[str]] = None,
+        date_from: Optional[Union[datetime, str]] = None,
+        date_to: Optional[Union[datetime, str]] = None,
     ) -> None:
         self.limit = limit
         self.offset = offset
-        self.types = types
-        self.tracks = tracks
-        self.locations = locations
-        self.has_bookmakers = has_bookmakers
-        self.has_runners = has_runners
-        self.has_trainers = has_trainers
-        self.has_riders = has_riders
+        self.types = types if types else []
+        self.tracks = tracks if tracks else []
+
+        # if locations is a string, convert to a list
+        # this is to simplify filtering for Australian races
+        if isinstance(locations, str):
+            if locations == "Australia":
+                locations = get_australian_states()
+
+        self.locations = locations if locations else []
+        self.has_bookmakers = has_bookmakers if has_bookmakers else []
+        self.has_runners = has_runners if has_runners else []
+        self.has_trainers = has_trainers if has_trainers else []
+        self.has_riders = has_riders if has_riders else []
+
+        # parse the dates to strings
+        if not date_from:
+            date_from = datetime.now()
+        if not date_to:
+            date_to = datetime.now()
+        if isinstance(date_from, datetime):
+            date_from = date_from.strftime("%Y-%m-%d")
+        if isinstance(date_to, datetime):
+            date_to = date_to.strftime("%Y-%m-%d")
+
         self.date_from = date_from
         self.date_to = date_to
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict."""
         return {
             "limit": self.limit,
@@ -40,34 +72,38 @@
             "types": [t.value if isinstance(t, MeetingType) else t for t in self.types],
             "tracks": self.tracks,
             "locations": self.locations,
             "hasBookmakers": [bookmaker.value for bookmaker in self.has_bookmakers],
             "hasRunners": self.has_runners,
             "hasTrainers": self.has_trainers,
             "hasRiders": self.has_riders,
-            "dateFrom": self.date_from.strftime("%Y-%m-%d"),
-            "dateTo": self.date_to.strftime("%Y-%m-%d"),
+            "dateFrom": self.date_from.strftime("%Y-%m-%d")
+            if isinstance(self.date_from, datetime)
+            else self.date_from,
+            "dateTo": self.date_to.strftime("%Y-%m-%d")
+            if isinstance(self.date_to, datetime)
+            else self.date_to,
         }
 
     def __str__(self) -> str:
-        return f"RacesFilter({('limit='+str(self.limit)+' ') if self.limit else ''}{'offset='+str(self.offset)+' ' if self.offset else ''}{'types=' + ','.join([t.value if isinstance(t, MeetingType) else t for t in self.types])} {'tracks='+str(self.tracks)} {'locations='+str(self.locations)} {'has_bookmakers='+str([b.value for b in self.has_bookmakers])+' ' if self.has_bookmakers else ''}{'has_runners='+str(self.has_runners)+' ' if self.has_runners else ''}{'has_trainers='+str(self.has_trainers)+' ' if self.has_trainers else ''}{'has_riders='+str(self.has_riders)+' ' if self.has_riders else ''}{'date_from='+self.date_from.strftime('%Y-%m-%d')+' ' if self.date_from else ''}{'date_to='+self.date_to.strftime('%Y-%m-%d') if self.date_to else ''})"
+        return f"RacesFilter({('limit='+str(self.limit)+' ') if self.limit else ''}{'offset='+str(self.offset)+' ' if self.offset else ''}{'types=' + ','.join([t.value if isinstance(t, MeetingType) else t for t in self.types])} {'tracks='+str(self.tracks)} {'locations='+str(self.locations)} {'has_bookmakers='+str([b.value for b in self.has_bookmakers])+' ' if self.has_bookmakers else ''}{'has_runners='+str(self.has_runners)+' ' if self.has_runners else ''}{'has_trainers='+str(self.has_trainers)+' ' if self.has_trainers else ''}{'has_riders='+str(self.has_riders)+' ' if self.has_riders else ''}{'date_from='+self.date_from+' ' if self.date_from else ''}{'date_to='+self.date_to if self.date_to else ''})"
 
 
 class RaceProjection:
     def __init__(
         self,
         markets=False,
         place_markets=False,
         flucs=False,
         links=False,
         betfair=False,
-        bookmakers: List[Bookmaker] = [],
+        bookmakers: Optional[List[Union[Bookmaker, str]]] = None,
     ) -> None:
         self.markets = markets
         self.place_markets = place_markets
         self.links = links
         self.flucs = flucs
         self.betfair = betfair
-        self.bookmakers = bookmakers
+        self.bookmakers = bookmakers if bookmakers else []
 
     def __str__(self) -> str:
         return f"RaceProjection({'markets ' if self.markets else ''}{' place_markets' if self.place_markets else ''}{' links' if self.links else ''}{' flucs' if self.flucs else ''}{' betfair' if self.betfair else ''}{' bookmakers' if self.bookmakers else ''})"
```

### Comparing `betwatch-0.9.9/betwatch/types/race.py` & `betwatch-1.0.0/betwatch/types/race.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
-from typing import List, Optional
+from typing import List, Literal, Optional, Union
 
 import dateutil.parser
 
 from betwatch.types.markets import (
     BetfairMarket,
     Bookmaker,
     BookmakerMarket,
@@ -96,15 +96,21 @@
     def __post_init__(self):
         self.scratched_time = (
             dateutil.parser.isoparse(self._scratched_time)
             if self._scratched_time
             else None
         )
 
-    def get_bookmaker_market(self, bookmaker: Bookmaker) -> Optional[BookmakerMarket]:
+    def get_bookmaker_market(
+        self, bookmaker: Union[Bookmaker, str]
+    ) -> Optional[BookmakerMarket]:
+        # try to get bookmaker if passed as string
+        if isinstance(bookmaker, str):
+            bookmaker = Bookmaker(bookmaker)
+
         if not self.bookmaker_markets:
             return None
         for market in self.bookmaker_markets:
             if market.bookmaker == bookmaker:
                 return market
         return None
 
@@ -122,19 +128,23 @@
         for market in self.betfair_markets:
             if market.market_name == "place":
                 return market
         return None
 
     def get_bookmaker_markets_by_price(
         self,
-        bookmakers: List[Bookmaker] = [bookmaker for bookmaker in Bookmaker],
+        bookmakers: Optional[List[Bookmaker]] = None,
         price_type: MarketPriceType = MarketPriceType.FIXED_WIN,
         max_length: Optional[int] = None,
     ) -> List[BookmakerMarket]:
         """Sorts the bookmaker markets for a runner with the given price type by price"""
+        # handle defaults
+        if not bookmakers:
+            bookmakers = [bookmaker for bookmaker in Bookmaker]
+
         if not self.bookmaker_markets:
             return []
         best_markets: List[BookmakerMarket] = []
         best_prices: List[Price] = []
         for market in self.bookmaker_markets:
             if market.bookmaker in bookmakers:
                 price = market.get_price(price_type)
@@ -160,54 +170,82 @@
 
         if max_length:
             return best_markets[:max_length]
         return best_markets
 
     def get_highest_bookmaker_market(
         self,
-        bookmakers: List[Bookmaker] = [bookmaker for bookmaker in Bookmaker],
+        bookmakers: Optional[List[Bookmaker]] = None,
         market_type: MarketPriceType = MarketPriceType.FIXED_WIN,
     ) -> Optional[BookmakerMarket]:
         """Returns the best bookmaker market for a runner with the given market type"""
+        # handle defaults
+        if not bookmakers:
+            bookmakers = [bookmaker for bookmaker in Bookmaker]
+
         best_markets = self.get_bookmaker_markets_by_price(
             bookmakers=bookmakers, price_type=market_type, max_length=1
         )
         if best_markets:
             return best_markets[0]
         return None
 
     def get_lowest_bookmaker_market(
         self,
-        bookmakers: List[Bookmaker] = [bookmaker for bookmaker in Bookmaker],
-        market_type: MarketPriceType = MarketPriceType.FIXED_WIN,
+        bookmakers: Optional[List[Bookmaker]] = None,
+        market_type: Union[
+            Literal["FIXED_WIN", "FIXED_PLACE"], MarketPriceType
+        ] = MarketPriceType.FIXED_WIN,
     ) -> Optional[BookmakerMarket]:
         """Returns the worst bookmaker market for a runner with the given market type"""
+        # handle defaults
+        if not bookmakers:
+            bookmakers = [bookmaker for bookmaker in Bookmaker]
+
+        # parse market type
+        if isinstance(market_type, str):
+            market_type = MarketPriceType(market_type)
+
         best_markets = self.get_bookmaker_markets_by_price(
             bookmakers=bookmakers, price_type=market_type
         )
         if best_markets:
             return best_markets[-1]
         return None
 
 
 @dataclass
 class RaceLink:
-    bookmaker: Optional[Bookmaker] = None
+    _bookmaker: Union[Bookmaker, str] = field(metadata={"name": "bookmaker"})
     nav_link: Optional[str] = field(metadata={"name": "navLink"}, default=None)
     _last_successful_price_update: Optional[str] = field(
         metadata={"name": "lastSuccessfulPriceUpdate"}, default=None
     )
 
     def __post_init__(self):
         self.last_successful_price_update = (
             dateutil.parser.isoparse(self._last_successful_price_update)
             if self._last_successful_price_update
             else None
         )
 
+    @property
+    def bookmaker(self) -> Bookmaker:
+        try:
+            if isinstance(self._bookmaker, str):
+                return Bookmaker(self._bookmaker)
+            return self._bookmaker
+        except ValueError as e:
+            if isinstance(self._bookmaker, str):
+                # try to find enum value by name (case insensitive)
+                for bm in Bookmaker:
+                    if bm.value.lower() == self._bookmaker.lower():
+                        return bm
+            raise e
+
 
 @dataclass
 class RaceUpdate:
     """Only the fields that are returned in the RacesUpdated query"""
 
     id: str
     status: RaceStatus
@@ -254,41 +292,49 @@
         #     dateutil.parser.isoparse(self._updated_at) if self._updated_at else None
         # )
         # self.created_at = (
         #     dateutil.parser.isoparse(self._created_at) if self._created_at else None
         # )
 
     def __str__(self) -> str:
-
         # format start_time in local timezone
         st = (
             self.start_time.astimezone().strftime(" [%d/%m/%Y %H:%M]")
             if self.start_time
             else ""
         )
 
         if self.meeting is None:
             return f"R{self.number} [{st}]"
         return f"({self.meeting.type}) {self.meeting.track} R{self.number}{st}"
 
-    def get_bookmaker_link(self, bookmaker: Bookmaker) -> Optional[RaceLink]:
+    def get_bookmaker_link(
+        self, bookmaker: Union[Bookmaker, str]
+    ) -> Optional[RaceLink]:
         """Returns the link for the given bookmaker"""
+        # parse bookmaker if string
+        if isinstance(bookmaker, str):
+            bookmaker = Bookmaker(bookmaker)
+
         if not self.links:
             return None
         for link in self.links:
             if link.bookmaker == bookmaker:
                 return link
         return None
 
     def get_runners_by_price(
         self,
         market_type: MarketPriceType,
-        bookmakers: List[Bookmaker] = [bookmaker for bookmaker in Bookmaker],
+        bookmakers: Optional[List[Bookmaker]] = None,
     ) -> List[Runner]:
         """Sorts the runners by the given market types best price"""
+        # handle defaults
+        if not bookmakers:
+            bookmakers = [bookmaker for bookmaker in Bookmaker]
         if not self.runners:
             return []
         best_runners: List[Runner] = []
         best_prices: List[Price] = []
         for runner in self.runners:
             market = runner.get_highest_bookmaker_market(
                 market_type=market_type, bookmakers=bookmakers
```

### Comparing `betwatch-0.9.9/examples/get_race_prices.py` & `betwatch-1.0.0/examples/get_races.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 import logging
 import os
 from datetime import datetime, timedelta
 
-from dotenv import load_dotenv
-
 import betwatch
-from betwatch.types import Bookmaker, MeetingType, RaceProjection, RacesFilter
+from betwatch.types import (
+    MeetingType,
+    RaceProjection,
+    RacesFilter,
+)
 
 
 def main():
     api_key = os.getenv("API_KEY")
     if not api_key:
         raise Exception("API_KEY not set in .env file")
 
     client = betwatch.connect(api_key=api_key)
 
     # define the projection of the returned data
     # we can filter out for certain bookmakers as well as define whether we want market data or flucs
     projection = RaceProjection(
         markets=True,
-        flucs=False,
-        bookmakers=[Bookmaker.SPORTSBET, Bookmaker.BLUEBET, Bookmaker.NEDS],
+        place_markets=False,
+        flucs=True,
+        links=False,
+        betfair=False,
+        # bookmakers=[Bookmaker.SPORTSBET, Bookmaker.BLUEBET],
     )
 
     # define the filter for the query
     # here we can filter by date, type of meeting, and various other parameters
     races_filter = RacesFilter(
-        date_from=datetime.now() - timedelta(days=7),
+        limit=10,
+        date_from=datetime.now() - timedelta(days=2),
         date_to=datetime.now() + timedelta(days=2),
-        types=[MeetingType.THOROUGHBRED],
-        limit=100,
-        has_riders=["bowman", "mccoy"],  # filter on any race containing these riders
+        types=[MeetingType.THOROUGHBRED],  # filter on a race type
+        locations="Australia",  # filter on a location (this could be a list of states or countries too)
     )
 
     races = client.get_races(projection, races_filter)
 
-    print(f"Found {len(races)} races matching the query")
-
-    if len(races) < 1:
-        print("No races found")
-        return
-    print(f"Observing race {races[0]}")
-
-    if not races[0].runners:
-        print("No runners found")
-        return
-
-    # we only requested sportsbet and bluebet data in the projection
-    for runner in races[0].runners:
-        print(f"Runner: {runner.number}. {runner.name}")
-        print(f"Best Price: {runner.get_highest_bookmaker_market()}")
-        print(f"Lowest Price: {runner.get_lowest_bookmaker_market()}")
-        print(f"Sportsbet Price: {runner.get_bookmaker_market(Bookmaker.SPORTSBET)}")
-
-        # get all the bookmaker markets sorted by price
-        markets_sorted_by_price = runner.get_bookmaker_markets_by_price()
-        print(f"Markets sorted by price: {markets_sorted_by_price}")
+    logging.info(f"Found {len(races)} races matching the query")
+    for race in races:
+        logging.info(race)
+        if race.runners:
+            for runner in race.runners:
+                print(runner)
+                if not runner.bookmaker_markets:
+                    print("No bookmaker markets for this runner")
+                    continue
+                for market in runner.bookmaker_markets:
+                    print(market)
+                    if market.fixed_win:
+                        print(f"Fixed Win Price: {market.fixed_win.price}")
+                        if market.fixed_win.flucs:
+                            for fluc in market.fixed_win.flucs:
+                                print(fluc)
 
 
 if __name__ == "__main__":
     # setup logging
     logging.basicConfig(
-        level=logging.INFO,
+        level=logging.DEBUG if os.getenv("DEBUG") else logging.INFO,
         format="%(asctime)s [%(levelname)s]: %(message)s",
         handlers=[logging.StreamHandler()],
         datefmt="%Y-%m-%d %H:%M:%S",
     )
-    load_dotenv()
     main()
```

### Comparing `betwatch-0.9.9/examples/get_races.py` & `betwatch-1.0.0/examples/get_races_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+import asyncio
 import logging
 import os
 from datetime import datetime, timedelta
 
-from dotenv import load_dotenv
-
 import betwatch
 from betwatch.types import MeetingType, RaceProjection, RacesFilter
 from betwatch.types.bookmakers import Bookmaker
 
 
-def main():
+async def main():
     api_key = os.getenv("API_KEY")
     if not api_key:
         raise Exception("API_KEY not set in .env file")
 
-    client = betwatch.connect(api_key=api_key)
+    client = betwatch.connect_async(api_key=api_key)
 
     # define the projection of the returned data
     # we can filter out for certain bookmakers as well as define whether we want market data or flucs
     projection = RaceProjection(
         markets=True, flucs=True, bookmakers=[Bookmaker.SPORTSBET, Bookmaker.BLUEBET]
     )
 
@@ -27,24 +26,21 @@
     races_filter = RacesFilter(
         date_from=datetime.now() - timedelta(days=7),
         date_to=datetime.now() + timedelta(days=2),
         types=[MeetingType.THOROUGHBRED],  # filter on a race type
         has_riders=["bowman", "mccoy"],  # filter on any race containing these riders
     )
 
-    races = client.get_races(projection, races_filter)
+    races = await client.get_races(projection, races_filter)
 
-    logging.info(f"Found {len(races)} races matching the query")
-    for race in races:
-        logging.info(race)
+    print(f"Found {len(races)} races matching the query")
 
 
 if __name__ == "__main__":
     # setup logging
     logging.basicConfig(
-        level=logging.INFO,
+        level=logging.DEBUG if os.getenv("DEBUG") else logging.INFO,
         format="%(asctime)s [%(levelname)s]: %(message)s",
         handlers=[logging.StreamHandler()],
         datefmt="%Y-%m-%d %H:%M:%S",
     )
-    load_dotenv()
-    main()
+    asyncio.run(main())
```

### Comparing `betwatch-0.9.9/examples/subscriptions.py` & `betwatch-1.0.0/examples/subscriptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import asyncio
 import logging
 import os
 from datetime import datetime, timedelta
 
-from dotenv import load_dotenv
-
 import betwatch
 
 
 async def main():
     api_key = os.getenv("API_KEY")
     if not api_key:
         raise Exception("API_KEY not set in .env file")
 
-    client = await betwatch.connect_async(api_key)
+    client = betwatch.connect_async(api_key)
 
     # use a context handler to automatically close the connection gracefully
     async with client:
         # get today in YYYY-MM-DD format
         today = datetime.today()
         tomorrow = datetime.today() + timedelta(days=1)
 
@@ -46,14 +44,13 @@
                 # has updated race info (e.g. status, updated start tiem)
                 pass
 
 
 if __name__ == "__main__":
     # setup logging
     logging.basicConfig(
-        level=logging.INFO,
+        level=logging.DEBUG if os.getenv("DEBUG") else logging.INFO,
         format="%(asctime)s [%(levelname)s]: %(message)s",
         handlers=[logging.StreamHandler()],
         datefmt="%Y-%m-%d %H:%M:%S",
     )
-    load_dotenv()
     asyncio.run(main())
```

### Comparing `betwatch-0.9.9/tests/test_get_race.py` & `betwatch-1.0.0/tests/test_get_race.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 
-from dotenv import load_dotenv
-
 import betwatch
 from betwatch.types import RaceProjection, RaceStatus
 
 
 def get_race(race_id: str):
-    load_dotenv()
     api_key = os.getenv("API_KEY")
     if not api_key:
         raise Exception("API_KEY not set in .env file")
 
     client = betwatch.connect(api_key=api_key)
 
     projection = RaceProjection(markets=True, flucs=True, links=True, betfair=True)
```

### Comparing `betwatch-0.9.9/tests/test_get_races.py` & `betwatch-1.0.0/tests/test_get_races.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import os
 
-from dotenv import load_dotenv
-
 import betwatch
 
 
 def get_races():
-    load_dotenv()
     api_key = os.getenv("API_KEY")
     if not api_key:
         raise Exception("API_KEY not set in .env file")
 
     client = betwatch.connect(api_key=api_key)
 
     races_from = "2022-12-21"
```

### Comparing `betwatch-0.9.9/tests/test_get_races_async.py` & `betwatch-1.0.0/tests/test_get_races_async.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 
 import pytest
-from dotenv import load_dotenv
 
 import betwatch
 
 
 async def get_races():
-    load_dotenv()
     api_key = os.getenv("API_KEY")
     if not api_key:
         raise Exception("API_KEY not set in .env file")
 
-    client = await betwatch.connect_async(api_key=api_key)
+    client = betwatch.connect_async(api_key=api_key)
 
     races_from = "2022-12-21"
     races_to = "2022-12-22"
 
     races = await client.get_races_between_dates(races_from, races_to)
 
     return races
```

### Comparing `betwatch-0.9.9/.gitignore` & `betwatch-1.0.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.rtx.toml
+.envrc
 frames.json
 playground/
 .vscode
 .ruff_cache
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `betwatch-0.9.9/LICENSE.txt` & `betwatch-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.9/README.md` & `betwatch-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-0.9.9/pyproject.toml` & `betwatch-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,77 +2,77 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "betwatch"
 description = 'A Python package for interacting with the Betwatch.com API'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
-keywords = []
+keywords = ["betwatch", "betting", "sports", "api", "sdk"]
 authors = [{ name = "Jamie Watts", email = "jamie@betwatch.com" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "gql[aiohttp,websockets,requests]==3.5.0b3",
-    "typedload==2.21",
+    "typedload==2.22",
     "aiohttp==3.8.3",
     "python-dateutil==2.8.2",
+    "urllib3>=1.26,<2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/betwatch/betwatch-sdk-python#readme"
 Issues = "https://github.com/betwatch/betwatch-sdk-python/issues"
 Source = "https://github.com/betwatch/betwatch-sdk-python"
 "Betwatch.com" = "https://betwatch.com"
 
 [tool.hatch.version]
 path = "betwatch/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
+    "ruff",
     "pytest",
     "pytest-cov",
     "python-dotenv",
     "pytest-asyncio",
     "black",
     "pre-commit",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=betwatch --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = ["betwatch/__about__.py"]
 
 [tool.coverage.report]
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.ruff]
+
 # Enable Pyflakes and pycodestyle rules.
-select = ["E", "F"]
+select = ["E", "F", "B"]
 
 # Never enforce `E501` (line length violations).
 ignore = ["E501"]
 
-# Always autofix, but never try to fix `F401` (unused imports).
 fix = true
-unfixable = ["F401"]
 
 # Ignore `E402` (import violations) in all `__init__.py` files
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "E402"]
```

### Comparing `betwatch-0.9.9/PKG-INFO` & `betwatch-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 0.9.9
+Version: 1.0.0
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
+Keywords: api,betting,betwatch,sdk,sports
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: aiohttp==3.8.3
 Requires-Dist: gql[aiohttp,requests,websockets]==3.5.0b3
 Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: typedload==2.21
+Requires-Dist: typedload==2.22
+Requires-Dist: urllib3<2,>=1.26
 Description-Content-Type: text/markdown
 
 # Betwatch Python SDK
 
 [![PyPI - Version](https://img.shields.io/pypi/v/betwatch.svg)](https://pypi.org/project/betwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/betwatch.svg)](https://pypi.org/project/betwatch)
```

