# Comparing `tmp/dxsp-1.9.6.tar.gz` & `tmp/dxsp-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.9.6.tar", max compression
+gzip compressed data, was "dxsp-1.9.7.tar", max compression
```

## Comparing `dxsp-1.9.6.tar` & `dxsp-1.9.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-06 09:46:03.738133 dxsp-1.9.6/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-06 09:46:03.738133 dxsp-1.9.6/README.md
--rw-r--r--   0        0        0       38 2023-05-06 09:46:03.738133 dxsp-1.9.6/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-06 09:46:04.410149 dxsp-1.9.6/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-06 09:46:03.742133 dxsp-1.9.6/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-06 09:46:03.742133 dxsp-1.9.6/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-06 09:46:03.742133 dxsp-1.9.6/dxsp/config.py
--rw-r--r--   0        0        0      581 2023-05-06 09:46:03.742133 dxsp-1.9.6/dxsp/default_settings.toml
--rw-r--r--   0        0        0    27786 2023-05-06 09:46:03.742133 dxsp-1.9.6/dxsp/main.py
--rw-r--r--   0        0        0     1787 2023-05-06 09:46:04.406149 dxsp-1.9.6/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 10:54:44.842896 dxsp-1.9.7/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-06 10:54:44.842896 dxsp-1.9.7/README.md
+-rw-r--r--   0        0        0       38 2023-05-06 10:54:44.842896 dxsp-1.9.7/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-06 10:54:45.778937 dxsp-1.9.7/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-06 10:54:44.842896 dxsp-1.9.7/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-06 10:54:44.842896 dxsp-1.9.7/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-06 10:54:44.842896 dxsp-1.9.7/dxsp/config.py
+-rw-r--r--   0        0        0      581 2023-05-06 10:54:44.842896 dxsp-1.9.7/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28222 2023-05-06 10:54:44.842896 dxsp-1.9.7/dxsp/main.py
+-rw-r--r--   0        0        0     1787 2023-05-06 10:54:45.778937 dxsp-1.9.7/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.7/PKG-INFO
```

### Comparing `dxsp-1.9.6/LICENSE` & `dxsp-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.6/README.md` & `dxsp-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.6/dxsp/assets/blockchains.py` & `dxsp-1.9.7/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.6/dxsp/default_settings.toml` & `dxsp-1.9.7/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.6/dxsp/main.py` & `dxsp-1.9.7/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
                  private_key: str | None = None,
                  block_explorer_api: str | None = None,
                  block_explorer_url: str | None = None,
                  rpc: str | None = None,
                  w3: Web3 | None = None,
                  protocol_type: str | None = None,
                  router_contract_addr: str | None = None,
-                 amount_trading_option: int = 1,
                  ):
         """build a web3 object for swap"""
         self.logger = logging.getLogger(__name__)
         self.logger.info("DexSwap version: %s", __version__)
         self.logger.info("Initializing DexSwap for %s on %s",
                          wallet_address, chain_id)
 
@@ -93,17 +92,14 @@
 
         self.name = "TBD"
         self.logger.debug("self.name %s", self.name)
 
         self.trading_quote_ccy = settings.trading_quote_ccy
         self.logger.debug("self.trading_quote_ccy %s", self.trading_quote_ccy)
 
-        self.amount_trading_option = amount_trading_option
-        self.logger.debug("trading_option %s", self.amount_trading_option)
-
         try:
             self.gecko_api = CoinGeckoAPI()
             assetplatform = self.gecko_api.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
                            == int(self.chain_id)]
             self.gecko_platform = output_dict[0]['id']
             self.logger.debug("self.gecko_platform %s", self.gecko_platform)
@@ -143,23 +139,30 @@
         # asset_out_contract = await self.get_token_contract(asset_out_symbol)
         # asset_out_decimals = asset_out_contract.functions.decimals().call()
         # self.logger.debug(f"asset_out_decimals {asset_out_decimals}")
         try:
             if self.protocol_type == "1inch":
                 asset_out_amount = self.w3.to_wei(1, 'ether')
                 self.logger.debug("asset_out_amount %s", asset_out_amount)
-                quote_url = f"{self.dex_url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
+                quote_url = (self.dex_url
+                             + "/quote?fromTokenAddress="
+                             + asset_in_address
+                             + "&toTokenAddress="
+                             + asset_out_address
+                             + "&amount="
+                             + asset_out_amount)
                 quote = await self._get(quote_url)
                 self.logger.debug("quote %s", quote)
                 raw_quote = quote['toTokenAmount']
                 self.logger.debug("raw_quote %s", raw_quote)
                 asset_quote_decimals = quote['fromToken']['decimals']
                 self.logger.debug("asset_quote_decimals %s",
                                   asset_quote_decimals)
-                quote_readable = self.w3.from_wei(int(raw_quote), 'wei') / (10 ** asset_quote_decimals)
+                quote_readable = (self.w3.from_wei(int(raw_quote), 'wei') /
+                                  (10 ** asset_quote_decimals))
                 self.logger.debug("quote_readable %s", quote_readable)
                 return round(quote_readable, 2)
             if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 return
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
@@ -173,15 +176,16 @@
             asset_out_symbol = (self.trading_quote_ccy if
                                 action == "BUY" else instrument)
             asset_in_symbol = (instrument if action == "BUY"
                                else self.trading_quote_ccy)
             asset_out_contract = await self.get_token_contract(
                 asset_out_symbol)
             try:
-                asset_out_decimals = asset_out_contract.functions.decimals().call()
+                asset_out_decimals = (
+                    asset_out_contract.functions.decimals().call())
             except Exception as e:
                 self.logger.error("execute_order decimals: %s", e)
                 asset_out_decimals = 18
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
             #  buy or sell %p percentage DEFAULT OPTION is 10%
             asset_out_amount = ((asset_out_balance) /
                                 (settings.trading_risk_amount
@@ -208,86 +212,100 @@
                 slippage_tolerance_percentage=2
                 ):
         """main swap function"""
 
         self.logger.debug("get_swap")
         try:
             # ASSET OUT
-            asset_out_address = await self.search_contract(asset_out_symbol)
-            asset_out_contract = await self.get_token_contract(asset_out_symbol)
-            self.logger.debug("asset_out_address %s %s", asset_out_address,asset_out_symbol)
+            asset_out_address = await self.search_contract(
+                asset_out_symbol)
+            asset_out_contract = await self.get_token_contract(
+                asset_out_symbol)
             if asset_out_contract is None:
-                raise ValueError(f"Non contract identified for {asset_out_symbol}")
+                raise ValueError("No contract identified")
             asset_out_decimals = asset_out_contract.functions.decimals().call()
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
-            self.logger.debug("asset_out_balance %s",asset_out_balance)
+            self.logger.debug("asset_out_balance %s", asset_out_balance)
             if asset_out_balance == 0:
                 self.logger.warning("No Money")
-                raise ValueError(f"Non contract identified for {asset_out_symbol}")
+                raise ValueError("Non contract identified")
                 return
             # ASSETS IN
             asset_in_address = await self.search_contract(asset_in_symbol)
             self.logger.debug("asset_in_address %s", asset_in_address)
             if asset_in_address is None:
                 return
 
             # AMOUNT
             asset_out_decimals = asset_out_contract.functions.decimals().call()
             self.logger.debug("asset_out_decimals %s", asset_out_decimals)
             asset_out_amount = amount * 10 ** asset_out_decimals
             # defaulted to 2% slippage if not given
-            slippage = slippage_tolerance_percentage  
+            slippage = slippage_tolerance_percentage
             self.logger.debug("slippage %s", slippage)
-            asset_out_amount_converted = self.w3.to_wei(asset_out_amount,'ether')
+            asset_out_amount_converted = self.w3.to_wei(
+                asset_out_amount, 'ether')
 
-            order_amount = int((asset_out_amount_converted *(slippage/100)))
-            self.logger.debug("order_amount %s",order_amount)
+            order_amount = int((asset_out_amount_converted * (slippage/100)))
+            self.logger.debug("order_amount %s", order_amount)
 
             # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             await self.get_approve(asset_out_address)
 
             # 1INCH
             if self.protocol_type in ["1inch"]:
-                swap_url = f"{self.dex_url}/swap?fromTokenAddress={asset_out_address}&toTokenAddress={asset_in_address}&amount={order_amount}&fromAddress={self.wallet_address}&slippage={slippage}"
+                swap_url = (self.dex_url
+                            + "/swap?fromTokenAddress="
+                            + asset_out_address
+                            + "&toTokenAddress="
+                            + asset_in_address
+                            + "&amount="
+                            + order_amount
+                            + "&fromAddress="
+                            + self.wallet_address
+                            + "&slippage="
+                            + slippage
+                            )
                 swap_order = await self._get(swap_url)
                 swap_order_status = swap_order['statusCode']
                 if swap_order_status != 200:
                     return
             # UNISWAP V2
             if self.protocol_type in ["uniswap_v2"]:
                 order_path_dex = [asset_out_address, asset_in_address]
                 router_abi = await self.get_abi(self.router_contract_addr)
                 router = self.w3.eth.contract(
-                                  self.w3.to_checksum_address(self.router_contract_addr),
+                                  self.w3.to_checksum_address(
+                                    self.router_contract_addr),
                                   router_abi)
                 deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
                 order_min_amount = int(router.functions.getAmountsOut(
                                         order_amount,
                                         order_path_dex).call()[1])
                 swap_order = router.functions.swapExactTokensForTokens(
-                                                                                order_amount, 
-                                                                                order_min_amount,
-                                                                                order_path_dex,
-                                                                                self.wallet_address,
-                                                                                deadline)
+                                order_amount,
+                                order_min_amount,
+                                order_path_dex,
+                                self.wallet_address,
+                                deadline)
             # 1INCH LIMIT
             if self.protocol_type in ["1inch_limit"]:
                 return
 
             # UNISWAP V3
             if self.protocol_type in ['uniswap_v3']:
                 return
             if swap_order:
                 self.logger.debug("swap_order %s", swap_order)
                 signed_order = await self.get_sign(swap_order)
                 order_hash = str(self.w3.to_hex(signed_order))
                 order_hash_details = self.w3.wait_for_transaction_receipt(
-                                            order_hash,
-                                            timeout=120,
-                                            poll_latency=0.1)
+                                        order_hash,
+                                        timeout=120,
+                                        poll_latency=0.1)
                 if order_hash_details['status'] == "1":
                     await self.get_confirmation(
                         order_hash,
                         order_hash_details,
                         asset_out_symbol,
                         asset_out_address,
                         order_amount,)
@@ -301,57 +319,69 @@
                                asset_out_symbol,
                                asset_out_address,
                                order_amount,
                                ):
         """ trade confirmation function"""
         self.logger.debug("get_confirmation")
         try:
-            order_blockNumber = order_hash_details['blockNumber']
-            order_receipt = self.w3.eth.get_transaction_receipt(order_hash)
-            order_block = self.w3.eth.get_block(order_blockNumber)
+            trade_blockNumber = order_hash_details['blockNumber']
+            trade_receipt = self.w3.eth.get_transaction_receipt(order_hash)
+            trade_block = self.w3.eth.get_block(trade_blockNumber)
             trade = {}
-            trade['id'] = order_receipt['transactionHash']
-            trade['timestamp'] = order_block['timestamp']
+            trade['id'] = trade_receipt['transactionHash']
+            trade['timestamp'] = trade_block['timestamp']
             trade['instrument'] = asset_out_symbol
             trade['contract'] = asset_out_address
             trade['amount'] = order_amount
-            trade['fee'] = order_receipt['gasUsed']
+            trade['fee'] = trade_receipt['gasUsed']
             trade['price'] = "TBD"
             trade['confirmation'] += f"➕ Size: {round(trade['amount'],4)}\n"
             trade['confirmation'] += f"⚫️ Entry: {round(trade['price'],4)}\n"
             trade['confirmation'] += f"ℹ️ {trade['id']}\n"
             trade['confirmation'] += f"🗓️ {trade['datetime']}"
             self.logger.info("trade %s", trade)
             return trade
         except Exception as e:
             self.logger.error("get_confirmation %s", e)
             return
 
     async def get_block_explorer_status(self, txHash):
         self.logger.debug("get_block_explorer_status %s", txHash)
-        checkTransactionSuccessURL = f"{self.block_explorer_url}?module=transaction&action=gettxreceiptstatus&txhash={txHash}&apikey={self.block_explorer_api}"
+        checkTransactionSuccessURL = (
+            self.block_explorer_url
+            + "?module=transaction&action=gettxreceiptstatus&txhash="
+            + txHash
+            + "&apikey="
+            + self.block_explorer_api)
         checkTransactionRequest = self._get(checkTransactionSuccessURL)
         return checkTransactionRequest['status']
 
 # ###CONTRACT SEARCH
     async def search_contract(
                             self,
                             token
                             ):
         """search a contract function"""
         self.logger.debug("search_contract")
 
         try:
-            token_contract = await self.get_contract_address(settings.TOKEN_PERSONAL_LIST,token)
+            token_contract = await self.get_contract_address(
+                settings.TOKEN_PERSONAL_LIST,
+                token)
             if token_contract is None:
-                token_contract = await self.get_contract_address(settings.TOKEN_TESTNET_LIST,token)
+                token_contract = await self.get_contract_address(
+                    settings.TOKEN_TESTNET_LIST,
+                    token)
                 if token_contract is None:
-                    token_contract = await self.get_contract_address(settings.TOKEN_MAINNET_LIST,token)
+                    token_contract = await self.get_contract_address(
+                        settings.TOKEN_MAINNET_LIST,
+                        token)
                     if token_contract is None:
-                        token_contract = await self.search_gecko_contract(token)
+                        token_contract = await self.search_gecko_contract(
+                            token)
             if token_contract is not None:
                 self.logger.info("token_contract found %s", token_contract)
                 return self.w3.to_checksum_address(token_contract)
             self.logger.info("no contract found for %s", token)
         except Exception as e:
             self.logger.error("search_contract %s", e)
             return
@@ -390,23 +420,23 @@
             return
 
     async def get_contract_address(
                             self,
                             token_list_url,
                             symbol
                         ):
-        """Given a token symbol and json format url address tokenlist, 
+        """Given a token symbol and json format url address tokenlist,
         get token address"""
         self.logger.debug("get_contract_address %s %s", token_list_url, symbol)
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and
-                    keyval['chainId'] == self.chain_id):
+                   keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
             return
 
     async def get_token_contract(
                                 self,
@@ -426,43 +456,55 @@
     async def get_approve(
                         self,
                         asset_out_address: str,
                         amount=None
                     ):
         self.logger.debug("get_approve %s", asset_out_address)
         if self.protocol_type in ["1inch", "1inch_limit"]:
-            approval_check_URL = f"{self.dex_url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
+            approval_check_URL = (
+                self.dex_url
+                + "/approve/allowance?tokenAddress="
+                + asset_out_address
+                + "&walletAddress="
+                + self.wallet_address)
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check == 0):
-                approval_URL = f"{self.dex_url}/approve/transaction?tokenAddress={asset_out_address}"
+                approval_URL = (
+                    self.dex_url
+                    + "/approve/transaction?tokenAddress="
+                    + asset_out_address)
                 approval_response = await self._get(approval_URL)
         elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
             asset_out_abi = await self.get_abi(asset_out_address)
             asset_out_contract = self.w3.eth.contract(
                                  asset_out_address,
                                  asset_out_abi)
             approval_check = asset_out_contract.functions.allowance(
                              self.w3.to_checksum_address(self.wallet_address),
-                             self.w3.to_checksum_address(self.router_contract_addr)
+                             self.w3.to_checksum_address(
+                                self.router_contract_addr)
                              ).call()
             if (approval_check == 0):
                 approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
                 asset_out_abi = await self.get_abi(asset_out_address)
                 asset_out_contract = self.w3.eth.contract(
                                      asset_out_address,
                                      asset_out_abi)
                 approval_TX = asset_out_contract.functions.approve(
-                                self.w3.to_checksum_address(self.router_contract_addr),
+                                self.w3.to_checksum_address(
+                                    self.router_contract_addr),
                                 approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
-                approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(
-                                           approval_txHash,
-                                           timeout=120,
-                                           poll_latency=0.1)
+                approval_txHash_complete = (
+                    self.w3.eth.wait_for_transaction_receipt(
+                        approval_txHash,
+                        timeout=120,
+                        poll_latency=0.1))
+                return approval_txHash_complete
 
     async def get_sign(
                     self,
                     order
                 ):
         self.logger.debug("get_sign %s", order)
         try:
@@ -473,15 +515,15 @@
                             'from': self.wallet_address,
                             'gas': await self.get_gas(order),
                             'gasPrice': await self.get_gasPrice(order),
                             'nonce': self.w3.eth.get_transaction_count(
                                 self.wallet_address),
                             }
                 order = order.build_transaction(order_params)
-            elif self.protocol_type in ["1inch","1inch_limit"]:
+            elif self.protocol_type in ["1inch", "1inch_limit"]:
                 order = order['tx']
                 order['gas'] = await self.get_gas(order)
                 order['nonce'] = self.w3.eth.get_transaction_count(
                     self.wallet_address)
                 order['value'] = int(order['value'])
                 order['gasPrice'] = await self.get_gasPrice(order)
             signed = self.w3.eth.account.sign_transaction(
@@ -532,20 +574,20 @@
                 # Make a GET request to the block explorer URL
                 resp = await self._get(
                                        url=self.block_explorer_url,
                                        params=params,
                                        headers=headers
                                        )
                 # If the response status is 1, log the ABI
-                if resp['status']=="1":
+                if resp['status'] == "1":
                     self.logger.debug("ABI found %s", resp)
                     abi = resp["result"]
                     return abi
                 # If no ABI is identified, log a warning
-                self.logger.warning("No ABI identified for contract %s on chain %s",addr,self.chain_id)
+                self.logger.warning("No ABI identified")
             except Exception as e:
                 # Log an error
                 self.logger.error("error get_abi %s", e)
                 return
         else:
             # If no block_explorer_api is set, log a warning
             self.logger.warning("No block_explorer_api. Option B needed TBD")
@@ -561,21 +603,23 @@
         try:
             token_address = await self.search_contract(token)
             if token_address is None:
                 raise ValueError(f"Token address not found for {token}")
             token_abi = await self.get_abi(token_address)
             if token_abi is None:
                 raise ValueError(f"ABI not found for {token_address}")
-            token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
+            token_contract = self.w3.eth.contract(
+                token_address,
+                token_abi)
             token_balance = 0
             try:
-                token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
+                token_balance = token_contract.functions.balanceOf(
+                    self.wallet_address).call()
             except ValueError as e:
-                self.logger.warning("Invalid address %s for token %s: %s", self.wallet_address, token, e)
-            # (ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
+                self.logger.warning("Invalid address: %s", e)
             return 0 if token_balance <= 0 else token_balance
         except Exception as e:
             self.logger.error("get_token_balance %s: %s", token, e)
             return 0
 
     async def get_quote_ccy_balance(
                                 self
@@ -605,15 +649,15 @@
             self.logger.error("get_stablecoin_balance error: %s", e)
             return 0
 
     async def get_account_balance(
                             self
                         ):
         try:
-            return self.w3.eth.get_balance(self.wallet_address)
+            return self.w3.eth.get_balance(str(self.wallet_address))
         except Exception as e:
             self.logger.error("get_account_balance error: %s", e)
             return "balance error"
             # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_position(
                                     self
```

### Comparing `dxsp-1.9.6/pyproject.toml` & `dxsp-1.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.9.6"
+version = "1.9.7"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.9.6/PKG-INFO` & `dxsp-1.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.9.6
+Version: 1.9.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

