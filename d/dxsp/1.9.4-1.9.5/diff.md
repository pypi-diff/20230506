# Comparing `tmp/dxsp-1.9.4.tar.gz` & `tmp/dxsp-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.9.4.tar", max compression
+gzip compressed data, was "dxsp-1.9.5.tar", max compression
```

## Comparing `dxsp-1.9.4.tar` & `dxsp-1.9.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-06 05:22:37.420173 dxsp-1.9.4/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-06 05:22:37.420173 dxsp-1.9.4/README.md
--rw-r--r--   0        0        0       38 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-06 05:22:38.060159 dxsp-1.9.4/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/config.py
--rw-r--r--   0        0        0      556 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28346 2023-05-06 05:22:37.424172 dxsp-1.9.4/dxsp/main.py
--rw-r--r--   0        0        0     1787 2023-05-06 05:22:38.060159 dxsp-1.9.4/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 09:36:45.530501 dxsp-1.9.5/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-06 09:36:45.530501 dxsp-1.9.5/README.md
+-rw-r--r--   0        0        0       38 2023-05-06 09:36:45.530501 dxsp-1.9.5/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-06 09:36:46.310510 dxsp-1.9.5/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-06 09:36:45.530501 dxsp-1.9.5/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-06 09:36:45.530501 dxsp-1.9.5/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-06 09:36:45.530501 dxsp-1.9.5/dxsp/config.py
+-rw-r--r--   0        0        0      581 2023-05-06 09:36:45.530501 dxsp-1.9.5/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    27786 2023-05-06 09:36:45.534501 dxsp-1.9.5/dxsp/main.py
+-rw-r--r--   0        0        0     1787 2023-05-06 09:36:46.310510 dxsp-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.5/PKG-INFO
```

### Comparing `dxsp-1.9.4/LICENSE` & `dxsp-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.4/README.md` & `dxsp-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.4/dxsp/assets/blockchains.py` & `dxsp-1.9.5/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.4/dxsp/default_settings.toml` & `dxsp-1.9.5/dxsp/default_settings.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #📝tokenlist
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 #📝trading token setup
 trading_quote_ccy = "USDT"
+trading_risk_amount = 10
 stablecoins = ["USDC", "USDT"]
 
 #📝apollo API
 apollo_spot_api_key = ""
 apollo_spot_api_secret = ""
 
 apollo_future_api_key = ""
```

### Comparing `dxsp-1.9.4/dxsp/main.py` & `dxsp-1.9.5/dxsp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,15 @@
                  wallet_address: str | None = None,
                  private_key: str | None = None,
                  block_explorer_api: str | None = None,
                  block_explorer_url: str | None = None,
                  rpc: str | None = None,
                  w3: Web3 | None = None,
                  protocol_type: str | None = None,
-                 dex_exchange: str | None = None,
-                 dex_router: str | None = None,
+                 router_contract_addr: str | None = None,
                  amount_trading_option: int = 1,
                  ):
         """build a web3 object for swap"""
         self.logger = logging.getLogger(__name__)
         self.logger.info("DexSwap version: %s", __version__)
         self.logger.info("Initializing DexSwap for %s on %s",
                          wallet_address, chain_id)
@@ -84,28 +83,17 @@
         else:
             base_url = blockchain["1inch"]
 
         self.dex_url = f"{base_url}"
         self.logger.debug("self.dex_url %s", self.dex_url)
         self.logger.debug("self.protocol_type %s", self.protocol_type)
 
-        self.dex_exchange = dex_exchange
-        self.logger.debug("self.dex_exchange %s", self.dex_exchange)
-
-        self.dex_router = dex_router
-        if self.dex_router is None:
-            if (
-                self.dex_exchange is None
-                or self.dex_exchange != blockchain["uniswap_v3"]
-            ):
-                self.router_contract_addr = blockchain["uniswap_v2"]
-            else:
-                self.router_contract_addr = blockchain["uniswap_v3"]
-        else:
-            self.router_contract_addr = self.dex_router
+        self.router_contract_addr = router_contract_addr
+        if self.router_contract_addr is None:
+            self.router_contract_addr = blockchain["uniswap_v2"]
 
         self.name = "TBD"
         self.logger.debug("self.name %s", self.name)
 
         self.trading_quote_ccy = settings.trading_quote_ccy
         self.logger.debug("self.trading_quote_ccy %s", self.trading_quote_ccy)
 
@@ -176,34 +164,33 @@
             self.logger.error("get_quote %s", e)
             return
 
     async def execute_order(self, order_params):
         """execute swap function"""
         action = order_params.get('action')
         instrument = order_params.get('instrument')
-        # stop_loss = order_params.get('stop_loss', 1000)
-        # take_profit = order_params.get('take_profit', 1000)
         quantity = order_params.get('quantity', 1)
         try:
-            asset_out_symbol = self.trading_quote_ccy if action == "BUY" else instrument
-            asset_in_symbol = instrument if action == "BUY" else self.trading_quote_ccy
-            asset_out_contract = await self.get_token_contract(asset_out_symbol)
+            asset_out_symbol = (self.trading_quote_ccy if
+                                action == "BUY" else instrument)
+            asset_in_symbol = (instrument if action == "BUY"
+                               else self.trading_quote_ccy)
+            asset_out_contract = await self.get_token_contract(
+                asset_out_symbol)
             try:
                 asset_out_decimals = asset_out_contract.functions.decimals().call()
             except Exception as e:
                 self.logger.error("execute_order decimals: %s", e)
                 asset_out_decimals = 18
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
-            # if amount_trading_option == 2:
-            #     # SELL all token in case of sell order for example
-            #     asset_out_amount = (asset_out_balance)/(10 ** asset_out_decimals)
-            # else:
-            #     # buy or sell %p percentage DEFAULT OPTION
-            asset_out_amount = ((asset_out_balance)/
-                                (10 ** asset_out_decimals))*(float(quantity)/100)
+            #  buy or sell %p percentage DEFAULT OPTION is 10%
+            asset_out_amount = ((asset_out_balance) /
+                                (settings.trading_risk_amount
+                                ** asset_out_decimals)
+                                )*(float(quantity)/100)
 
             order = await self.get_swap(
                     asset_out_symbol,
                     asset_in_symbol,
                     asset_out_amount
                     )
             if order:
@@ -218,15 +205,15 @@
                 asset_out_symbol: str,
                 asset_in_symbol: str,
                 amount: int,
                 slippage_tolerance_percentage=2
                 ):
         """main swap function"""
 
-        self.logger.debug("get_swap %s %s %s", asset_out_symbol, asset_in_symbol, amount)
+        self.logger.debug("get_swap")
         try:
             # ASSET OUT
             asset_out_address = await self.search_contract(asset_out_symbol)
             asset_out_contract = await self.get_token_contract(asset_out_symbol)
             self.logger.debug("asset_out_address %s %s", asset_out_address,asset_out_symbol)
             if asset_out_contract is None:
                 raise ValueError(f"Non contract identified for {asset_out_symbol}")
@@ -325,18 +312,18 @@
             trade['id'] = order_receipt['transactionHash']
             trade['timestamp'] = order_block['timestamp']
             trade['instrument'] = asset_out_symbol
             trade['contract'] = asset_out_address
             trade['amount'] = order_amount
             trade['fee'] = order_receipt['gasUsed']
             trade['price'] = "TBD"
-            trade['confirmation'] = f"➕ Size: {trade['amount']}\n\
-                                ⚫️ Entry: {trade['price']}\n\
-                                ℹ️ {trade['id']}\n\
-                                🗓️ {trade['timestamp']}"
+            trade['confirmation'] += f"➕ Size: {round(trade['amount'],4)}\n"
+            trade['confirmation'] += f"⚫️ Entry: {round(trade['price'],4)}\n"
+            trade['confirmation'] += f"ℹ️ {trade['id']}\n"
+            trade['confirmation'] += f"🗓️ {trade['datetime']}"
             self.logger.info("trade %s", trade)
             return trade
         except Exception as e:
             self.logger.error("get_confirmation %s", e)
             return
 
     async def get_block_explorer_status(self, txHash):
@@ -431,15 +418,14 @@
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s", e)
             return
 
-
 # ###UTILS
     async def get_approve(
                         self,
                         asset_out_address: str,
                         amount=None
                     ):
         self.logger.debug("get_approve %s", asset_out_address)
@@ -486,15 +472,15 @@
                 order_params = {
                             'from': self.wallet_address,
                             'gas': await self.get_gas(order),
                             'gasPrice': await self.get_gasPrice(order),
                             'nonce': self.w3.eth.get_transaction_count(
                                 self.wallet_address),
                             }
-                order = order.build_transaction(order)
+                order = order.build_transaction(order_params)
             elif self.protocol_type in ["1inch","1inch_limit"]:
                 order = order['tx']
                 order['gas'] = await self.get_gas(order)
                 order['nonce'] = self.w3.eth.get_transaction_count(
                     self.wallet_address)
                 order['value'] = int(order['value'])
                 order['gasPrice'] = await self.get_gasPrice(order)
@@ -541,17 +527,17 @@
                     "address": addr,
                     "apikey": self.block_explorer_api
                     }
                 # Create a dictionary of headers
                 headers = {"User-Agent": "Mozilla/5.0"}
                 # Make a GET request to the block explorer URL
                 resp = await self._get(
-                                       url = self.block_explorer_url,
-                                       params = params,
-                                       headers = headers
+                                       url=self.block_explorer_url,
+                                       params=params,
+                                       headers=headers
                                        )
                 # If the response status is 1, log the ABI
                 if resp['status']=="1":
                     self.logger.debug("ABI found %s", resp)
                     abi = resp["result"]
                     return abi
                 # If no ABI is identified, log a warning
@@ -591,15 +577,17 @@
             self.logger.error("get_token_balance %s: %s", token, e)
             return 0
 
     async def get_quote_ccy_balance(
                                 self
                             ):
         try:
-            trading_quote_ccy_balance = await self.get_token_balance(self.trading_quote_ccy)
+            trading_quote_ccy_balance = await self.get_token_balance(
+                self.trading_quote_ccy
+                )
             return trading_quote_ccy_balance
 
         except Exception as e:
             self.logger.error("get_basecoin_balance %s: %s", e)
             return 0
 
     async def get_stablecoin_balance(
```

### Comparing `dxsp-1.9.4/pyproject.toml` & `dxsp-1.9.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.9.4"
+version = "1.9.5"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.9.4/PKG-INFO` & `dxsp-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.9.4
+Version: 1.9.5
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

