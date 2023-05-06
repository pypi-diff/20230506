# Comparing `tmp/cardano-nft-vending-machine-0.6.4.tar.gz` & `tmp/cardano-nft-vending-machine-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-lgs6mp_f/cardano-nft-vending-machine-0.6.4.tar", last modified: Mon May  1 02:24:38 2023, max compression
+gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-ghk_ag8n/cardano-nft-vending-machine-0.7.0.tar", last modified: Sat May  6 17:50:48 2023, max compression
```

## Comparing `cardano-nft-vending-machine-0.6.4.tar` & `cardano-nft-vending-machine-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.446302 cardano-nft-vending-machine-0.6.4/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.6.4/LICENSE
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-05-01 02:24:38.446012 cardano-nft-vending-machine-0.6.4/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12558 2023-04-01 01:43:17.000000 cardano-nft-vending-machine-0.6.4/README.md
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-01 02:23:43.000000 cardano-nft-vending-machine-0.6.4/pyproject.toml
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-01 02:24:38.446392 cardano-nft-vending-machine-0.6.4/setup.cfg
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.439061 cardano-nft-vending-machine-0.6.4/src/
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.440181 cardano-nft-vending-machine-0.6.4/src/cardano/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.4/src/cardano/__init__.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.442036 cardano-nft-vending-machine-0.6.4/src/cardano/wt/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4987 2023-02-15 06:22:29.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/blockfrost.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.442619 cardano-nft-vending-machine-0.6.4/src/cardano/wt/bonuses/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/bonuses/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/bonuses/bogo.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2803 2023-05-01 02:21:29.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/cardano_cli.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5560 2023-05-01 02:21:29.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/mint.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     9769 2023-05-01 02:22:50.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/nft_vending_machine.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/utxo.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.444042 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/asset_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/filesystem.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/no_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/wallet_whitelist.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-01 02:24:38.445574 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      772 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/requires.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-01 02:24:38.000000 cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/top_level.txt
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.674536 cardano-nft-vending-machine-0.7.0/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.7.0/LICENSE
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-06 17:50:48.674041 cardano-nft-vending-machine-0.7.0/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12474 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/README.md
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-05-05 03:11:27.000000 cardano-nft-vending-machine-0.7.0/pyproject.toml
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-05-06 17:50:48.674697 cardano-nft-vending-machine-0.7.0/setup.cfg
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.660414 cardano-nft-vending-machine-0.7.0/src/
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.662286 cardano-nft-vending-machine-0.7.0/src/cardano/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.0/src/cardano/__init__.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.665296 cardano-nft-vending-machine-0.7.0/src/cardano/wt/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5054 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/blockfrost.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.666368 cardano-nft-vending-machine-0.7.0/src/cardano/wt/bonuses/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/bonuses/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/bonuses/bogo.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     3931 2023-05-06 03:37:44.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/cardano_cli.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5604 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/mint.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       40 2023-05-05 03:06:45.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/network.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11029 2023-05-06 03:12:13.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/nft_vending_machine.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/utxo.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.670117 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/asset_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/filesystem.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/no_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/wallet_whitelist.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-05-06 17:50:48.673272 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13134 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      798 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/requires.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-05-06 17:50:48.000000 cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/top_level.txt
```

### Comparing `cardano-nft-vending-machine-0.6.4/LICENSE` & `cardano-nft-vending-machine-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.4/PKG-INFO` & `cardano-nft-vending-machine-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.6.4
+Version: 0.7.0
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -44,16 +44,16 @@
 This project contains Library bindings that can be installed using the standard [wheel](https://pypi.org/project/wheel/) mechanism.  See the [script quickstart section](#cardano_vending_machinepy) for how to run from CLI.
 ### Library Usage
 The library consists of several Python objects representing the mint process.  The sample below shows how one could run an infinite CNFT vending machine on mainnet for a 10₳ mint (gross of fees and rebates) with their NFT:
 
     # There are several sample whitelist implementations in cardano.wt.whitelist or you can implement your own
     whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/directory')
 
-    # The Mint object below represents your Mint policy and specifies price, and developer fee in Lovelace (both can be 0)
-    mint = Mint('<POLICY_ID>', 10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
+    # The Mint object below represents your Mint and specifies price, and developer fee in Lovelace (both can be 0)
+    mint = Mint(10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
 
     # Blockfrost is used in the code to validate where the UTXO sent to the payment address came from
     blockfrost_api = BlockfrostApi('<BLOCKFROST_PROJ_ID>', mainnet=True)
 
     # CardanoCli is a wrapper around the cardano-cli command (used as a utility without any interaction with the network)
     cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json')
 
@@ -72,15 +72,14 @@
         python3 main.py [validate | run] \
                 --payment-addr <PAYMENT_ADDR> \
                 --payment-sign-key /FULL/PATH/TO/payment.skey \
                 --profit-addr <PROFIT_ADDR> \
                 [--mint-price <PRICE_LOVELACE> | --free-mint] \
                 --mint-script /FULL/PATH/TO/policy.script \
                 --mint-sign-key /FULL/PATH/TO/policy.skey \
-                --mint-policy $(cat /FULL/PATH/TO/policyID) \
                 --blockfrost-project <BLOCKFROST_PROJECT_ID> \
                 --metadata-dir metadata/ \
                 --output-dir output/ \
                 --single-vend-max <MAX_SINGLE_VEND> \
                 [--vend-randomly] \
                 [--no-whitelist | \
                   [--single-use-asset-whitelist <WHITELIST_DIR> \
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.4 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.0 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
@@ -28,19 +28,19 @@
 pypi.org/project/wheel/) mechanism. See the [script quickstart section]
 (#cardano_vending_machinepy) for how to run from CLI. ### Library Usage The
 library consists of several Python objects representing the mint process. The
 sample below shows how one could run an infinite CNFT vending machine on
 mainnet for a 10â³ mint (gross of fees and rebates) with their NFT: # There
 are several sample whitelist implementations in cardano.wt.whitelist or you can
 implement your own whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/
-directory') # The Mint object below represents your Mint policy and specifies
-price, and developer fee in Lovelace (both can be 0) mint = Mint('', 10000000,
-1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/
-script', '/path/to/mint.skey', whitelist) # Blockfrost is used in the code to
-validate where the UTXO sent to the payment address came from blockfrost_api =
+directory') # The Mint object below represents your Mint and specifies price,
+and developer fee in Lovelace (both can be 0) mint = Mint(10000000, 1000000,
+'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/
+path/to/mint.skey', whitelist) # Blockfrost is used in the code to validate
+where the UTXO sent to the payment address came from blockfrost_api =
 BlockfrostApi('', mainnet=True) # CardanoCli is a wrapper around the cardano-
 cli command (used as a utility without any interaction with the network)
 cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json') #
 NftVendingMachine vends NFTs and needs to be called repeatedly (with a 25-vend
 max) so long as the mint period is open nft_vending_machine = NftVendingMachine
 ('addr_payment', '/path/to/payment.skey', 'addr_profit', 25, mint,
 blockfrost_api, cardano_cli, mainnet=True) # The following simple loop carries
@@ -49,61 +49,61 @@
 nft_vending_machine.vend('/path/to/output/dir', 'locking_subdir_name',
 'metadata_subdir_name', already_completed) time.sleep(WAIT_TIMEOUT) ###
 ``main.py`` There is a sample vending machine script that is included in the
 ``src/`` directory to show how to invoke the library components. Use ``-h`` to
 see detailed help or use a command like below: python3 main.py [validate | run]
 \ --payment-addr  \ --payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-
 addr  \ [--mint-price  | --free-mint] \ --mint-script /FULL/PATH/TO/
-policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --mint-policy $(cat
-/FULL/PATH/TO/policyID) \ --blockfrost-project  \ --metadata-dir metadata/ \ --
-output-dir output/ \ --single-vend-max  \ [--vend-randomly] \ [--no-whitelist |
-\ [--single-use-asset-whitelist  \ | --unlimited-asset-whitelist  \ | --wallet-
-whitelist  ] \ [--dev-fee dev_fee --dev-addr dev_addr] \ [--bogo threshold
-additional] \ [--mainnet] ## Installation This package is available from [PyPI]
-(https://pypi.org/) and can be installed using ``pip3``. Python <3.8 is
-currently unsupported at this time. pip3 install cardano-nft-vending-machine
-### Scripts In the `scripts/` directory there are several scripts that can be
-used to help operationalize the vending machine. #### initialize_whitelist.py
-This file should be used exactly once to initialize an asset-based whitelist
-for an existing NFT policy with *ALL* of the assets that are currently minted.
-Note that the `CONSUMED_DIR` folder is created but left empty so that the
-vending machine (e.g., started with `main.py`) can use it during running.
-usage: initialize_whitelist.py [-h] asset --blockfrost-project
-BLOCKFROST_PROJECT --consumed-dir CONSUMED_DIR [--mainnet] --policy-id
-POLICY_ID [--preview] --whitelist-dir WHITELIST_DIR Initialize an asset-based
-whitelist for an existing NFT policy optional arguments: -h, --help show this
-help message and exit --blockfrost-project BLOCKFROST_PROJECT Blockfrost
-project ID to use for retrieving chain data --consumed-dir CONSUMED_DIR Local
-folder where consumed whitelist files will go after processing (MUST NOT YET
-EXIST) --mainnet Run the initializer against mainnet assets (default is False
-[preprod]) --policy-id POLICY_ID Policy ID of the assets to be whitelisted --
-preview Run the initializer against preview assets (default is False [preprod])
---whitelist-dir WHITELIST_DIR Local folder where whitelist files are stored
-(MUST NOT YET EXIST) --num-mints-per-wl NUMBER How many whitelist spots are
-available for each asset on the whitelist #### upload_wl_usage.py This file
-should be run continuously during a whitelist mint to upload changes in the
-assets used for consumption by external parties. Note that if there are any
-performance issues (e.g., IOPS throughput) with the local vending machine
-filesystem it is recommended you not use this file. It is kept separate from
-the main vending machine operation to avoid any synchronization or performance
-issues as it is not critical. usage: upload_wl_usage.py [-h] --old-wl-file
-OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
-CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
-assets have been recently used in the vending machine optional arguments: -h, -
--help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
-of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
-store the new used whitelist information if any changes (can be same as --old-
-wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
-files have gone after processing by vending machine --whitelist-dir
-WHITELIST_DIR Local folder where unused whitelist files are stored to be
-processed by vending machine --credentials CREDENTIALS JSON-formatted
-application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
-uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
-documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
-the source code. A mirror of ``master`` is hosted on [Github Pages](https://
+policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --blockfrost-
+project  \ --metadata-dir metadata/ \ --output-dir output/ \ --single-vend-max
+\ [--vend-randomly] \ [--no-whitelist | \ [--single-use-asset-whitelist  \ | --
+unlimited-asset-whitelist  \ | --wallet-whitelist  ] \ [--dev-fee dev_fee --
+dev-addr dev_addr] \ [--bogo threshold additional] \ [--mainnet] ##
+Installation This package is available from [PyPI](https://pypi.org/) and can
+be installed using ``pip3``. Python <3.8 is currently unsupported at this time.
+pip3 install cardano-nft-vending-machine ### Scripts In the `scripts/
+` directory there are several scripts that can be used to help operationalize
+the vending machine. #### initialize_whitelist.py This file should be used
+exactly once to initialize an asset-based whitelist for an existing NFT policy
+with *ALL* of the assets that are currently minted. Note that the
+`CONSUMED_DIR` folder is created but left empty so that the vending machine
+(e.g., started with `main.py`) can use it during running. usage:
+initialize_whitelist.py [-h] asset --blockfrost-project BLOCKFROST_PROJECT --
+consumed-dir CONSUMED_DIR [--mainnet] --policy-id POLICY_ID [--preview] --
+whitelist-dir WHITELIST_DIR Initialize an asset-based whitelist for an existing
+NFT policy optional arguments: -h, --help show this help message and exit --
+blockfrost-project BLOCKFROST_PROJECT Blockfrost project ID to use for
+retrieving chain data --consumed-dir CONSUMED_DIR Local folder where consumed
+whitelist files will go after processing (MUST NOT YET EXIST) --mainnet Run the
+initializer against mainnet assets (default is False [preprod]) --policy-id
+POLICY_ID Policy ID of the assets to be whitelisted --preview Run the
+initializer against preview assets (default is False [preprod]) --whitelist-dir
+WHITELIST_DIR Local folder where whitelist files are stored (MUST NOT YET
+EXIST) --num-mints-per-wl NUMBER How many whitelist spots are available for
+each asset on the whitelist #### upload_wl_usage.py This file should be run
+continuously during a whitelist mint to upload changes in the assets used for
+consumption by external parties. Note that if there are any performance issues
+(e.g., IOPS throughput) with the local vending machine filesystem it is
+recommended you not use this file. It is kept separate from the main vending
+machine operation to avoid any synchronization or performance issues as it is
+not critical. usage: upload_wl_usage.py [-h] --old-wl-file OLD_WL_FILE --out-
+file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials CREDENTIALS] [--
+upload-method UPLOAD_METHOD] Determine if a set of whitelist assets have been
+recently used in the vending machine optional arguments: -h, --help show this
+help message and exit --old-wl-file OLD_WL_FILE Most recent run of this program
+that was uploaded to cloud storage --out-file OUT_FILE Where to store the new
+used whitelist information if any changes (can be same as --old-wl-file) --
+whitelist-dir WHITELIST_DIR Local folder where consumed whitelist files have
+gone after processing by vending machine --whitelist-dir WHITELIST_DIR Local
+folder where unused whitelist files are stored to be processed by vending
+machine --credentials CREDENTIALS JSON-formatted application-specific
+credentials --upload-method UPLOAD_METHOD Mechanism for uploading changes in
+whitelist files (e.g., CloudFlare) ## APIs All API documentation is auto-
+generated from ``pydoc3``-formatted multi-line strings in the source code. A
+mirror of ``master`` is hosted on [Github Pages](https://
 thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
 Building this project creates a ``.whl`` file for uploading to [PyPI]() or
 installing locally on a server. All output is, by default, stored to ``dist/``.
 To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
```

### Comparing `cardano-nft-vending-machine-0.6.4/README.md` & `cardano-nft-vending-machine-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 This project contains Library bindings that can be installed using the standard [wheel](https://pypi.org/project/wheel/) mechanism.  See the [script quickstart section](#cardano_vending_machinepy) for how to run from CLI.
 ### Library Usage
 The library consists of several Python objects representing the mint process.  The sample below shows how one could run an infinite CNFT vending machine on mainnet for a 10₳ mint (gross of fees and rebates) with their NFT:
 
     # There are several sample whitelist implementations in cardano.wt.whitelist or you can implement your own
     whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/directory')
 
-    # The Mint object below represents your Mint policy and specifies price, and developer fee in Lovelace (both can be 0)
-    mint = Mint('<POLICY_ID>', 10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
+    # The Mint object below represents your Mint and specifies price, and developer fee in Lovelace (both can be 0)
+    mint = Mint(10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
 
     # Blockfrost is used in the code to validate where the UTXO sent to the payment address came from
     blockfrost_api = BlockfrostApi('<BLOCKFROST_PROJ_ID>', mainnet=True)
 
     # CardanoCli is a wrapper around the cardano-cli command (used as a utility without any interaction with the network)
     cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json')
 
@@ -57,15 +57,14 @@
         python3 main.py [validate | run] \
                 --payment-addr <PAYMENT_ADDR> \
                 --payment-sign-key /FULL/PATH/TO/payment.skey \
                 --profit-addr <PROFIT_ADDR> \
                 [--mint-price <PRICE_LOVELACE> | --free-mint] \
                 --mint-script /FULL/PATH/TO/policy.script \
                 --mint-sign-key /FULL/PATH/TO/policy.skey \
-                --mint-policy $(cat /FULL/PATH/TO/policyID) \
                 --blockfrost-project <BLOCKFROST_PROJECT_ID> \
                 --metadata-dir metadata/ \
                 --output-dir output/ \
                 --single-vend-max <MAX_SINGLE_VEND> \
                 [--vend-randomly] \
                 [--no-whitelist | \
                   [--single-use-asset-whitelist <WHITELIST_DIR> \
```

#### html2text {}

```diff
@@ -19,19 +19,19 @@
 pypi.org/project/wheel/) mechanism. See the [script quickstart section]
 (#cardano_vending_machinepy) for how to run from CLI. ### Library Usage The
 library consists of several Python objects representing the mint process. The
 sample below shows how one could run an infinite CNFT vending machine on
 mainnet for a 10â³ mint (gross of fees and rebates) with their NFT: # There
 are several sample whitelist implementations in cardano.wt.whitelist or you can
 implement your own whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/
-directory') # The Mint object below represents your Mint policy and specifies
-price, and developer fee in Lovelace (both can be 0) mint = Mint('', 10000000,
-1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/
-script', '/path/to/mint.skey', whitelist) # Blockfrost is used in the code to
-validate where the UTXO sent to the payment address came from blockfrost_api =
+directory') # The Mint object below represents your Mint and specifies price,
+and developer fee in Lovelace (both can be 0) mint = Mint(10000000, 1000000,
+'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/
+path/to/mint.skey', whitelist) # Blockfrost is used in the code to validate
+where the UTXO sent to the payment address came from blockfrost_api =
 BlockfrostApi('', mainnet=True) # CardanoCli is a wrapper around the cardano-
 cli command (used as a utility without any interaction with the network)
 cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json') #
 NftVendingMachine vends NFTs and needs to be called repeatedly (with a 25-vend
 max) so long as the mint period is open nft_vending_machine = NftVendingMachine
 ('addr_payment', '/path/to/payment.skey', 'addr_profit', 25, mint,
 blockfrost_api, cardano_cli, mainnet=True) # The following simple loop carries
@@ -40,61 +40,61 @@
 nft_vending_machine.vend('/path/to/output/dir', 'locking_subdir_name',
 'metadata_subdir_name', already_completed) time.sleep(WAIT_TIMEOUT) ###
 ``main.py`` There is a sample vending machine script that is included in the
 ``src/`` directory to show how to invoke the library components. Use ``-h`` to
 see detailed help or use a command like below: python3 main.py [validate | run]
 \ --payment-addr  \ --payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-
 addr  \ [--mint-price  | --free-mint] \ --mint-script /FULL/PATH/TO/
-policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --mint-policy $(cat
-/FULL/PATH/TO/policyID) \ --blockfrost-project  \ --metadata-dir metadata/ \ --
-output-dir output/ \ --single-vend-max  \ [--vend-randomly] \ [--no-whitelist |
-\ [--single-use-asset-whitelist  \ | --unlimited-asset-whitelist  \ | --wallet-
-whitelist  ] \ [--dev-fee dev_fee --dev-addr dev_addr] \ [--bogo threshold
-additional] \ [--mainnet] ## Installation This package is available from [PyPI]
-(https://pypi.org/) and can be installed using ``pip3``. Python <3.8 is
-currently unsupported at this time. pip3 install cardano-nft-vending-machine
-### Scripts In the `scripts/` directory there are several scripts that can be
-used to help operationalize the vending machine. #### initialize_whitelist.py
-This file should be used exactly once to initialize an asset-based whitelist
-for an existing NFT policy with *ALL* of the assets that are currently minted.
-Note that the `CONSUMED_DIR` folder is created but left empty so that the
-vending machine (e.g., started with `main.py`) can use it during running.
-usage: initialize_whitelist.py [-h] asset --blockfrost-project
-BLOCKFROST_PROJECT --consumed-dir CONSUMED_DIR [--mainnet] --policy-id
-POLICY_ID [--preview] --whitelist-dir WHITELIST_DIR Initialize an asset-based
-whitelist for an existing NFT policy optional arguments: -h, --help show this
-help message and exit --blockfrost-project BLOCKFROST_PROJECT Blockfrost
-project ID to use for retrieving chain data --consumed-dir CONSUMED_DIR Local
-folder where consumed whitelist files will go after processing (MUST NOT YET
-EXIST) --mainnet Run the initializer against mainnet assets (default is False
-[preprod]) --policy-id POLICY_ID Policy ID of the assets to be whitelisted --
-preview Run the initializer against preview assets (default is False [preprod])
---whitelist-dir WHITELIST_DIR Local folder where whitelist files are stored
-(MUST NOT YET EXIST) --num-mints-per-wl NUMBER How many whitelist spots are
-available for each asset on the whitelist #### upload_wl_usage.py This file
-should be run continuously during a whitelist mint to upload changes in the
-assets used for consumption by external parties. Note that if there are any
-performance issues (e.g., IOPS throughput) with the local vending machine
-filesystem it is recommended you not use this file. It is kept separate from
-the main vending machine operation to avoid any synchronization or performance
-issues as it is not critical. usage: upload_wl_usage.py [-h] --old-wl-file
-OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
-CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
-assets have been recently used in the vending machine optional arguments: -h, -
--help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
-of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
-store the new used whitelist information if any changes (can be same as --old-
-wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
-files have gone after processing by vending machine --whitelist-dir
-WHITELIST_DIR Local folder where unused whitelist files are stored to be
-processed by vending machine --credentials CREDENTIALS JSON-formatted
-application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
-uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
-documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
-the source code. A mirror of ``master`` is hosted on [Github Pages](https://
+policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --blockfrost-
+project  \ --metadata-dir metadata/ \ --output-dir output/ \ --single-vend-max
+\ [--vend-randomly] \ [--no-whitelist | \ [--single-use-asset-whitelist  \ | --
+unlimited-asset-whitelist  \ | --wallet-whitelist  ] \ [--dev-fee dev_fee --
+dev-addr dev_addr] \ [--bogo threshold additional] \ [--mainnet] ##
+Installation This package is available from [PyPI](https://pypi.org/) and can
+be installed using ``pip3``. Python <3.8 is currently unsupported at this time.
+pip3 install cardano-nft-vending-machine ### Scripts In the `scripts/
+` directory there are several scripts that can be used to help operationalize
+the vending machine. #### initialize_whitelist.py This file should be used
+exactly once to initialize an asset-based whitelist for an existing NFT policy
+with *ALL* of the assets that are currently minted. Note that the
+`CONSUMED_DIR` folder is created but left empty so that the vending machine
+(e.g., started with `main.py`) can use it during running. usage:
+initialize_whitelist.py [-h] asset --blockfrost-project BLOCKFROST_PROJECT --
+consumed-dir CONSUMED_DIR [--mainnet] --policy-id POLICY_ID [--preview] --
+whitelist-dir WHITELIST_DIR Initialize an asset-based whitelist for an existing
+NFT policy optional arguments: -h, --help show this help message and exit --
+blockfrost-project BLOCKFROST_PROJECT Blockfrost project ID to use for
+retrieving chain data --consumed-dir CONSUMED_DIR Local folder where consumed
+whitelist files will go after processing (MUST NOT YET EXIST) --mainnet Run the
+initializer against mainnet assets (default is False [preprod]) --policy-id
+POLICY_ID Policy ID of the assets to be whitelisted --preview Run the
+initializer against preview assets (default is False [preprod]) --whitelist-dir
+WHITELIST_DIR Local folder where whitelist files are stored (MUST NOT YET
+EXIST) --num-mints-per-wl NUMBER How many whitelist spots are available for
+each asset on the whitelist #### upload_wl_usage.py This file should be run
+continuously during a whitelist mint to upload changes in the assets used for
+consumption by external parties. Note that if there are any performance issues
+(e.g., IOPS throughput) with the local vending machine filesystem it is
+recommended you not use this file. It is kept separate from the main vending
+machine operation to avoid any synchronization or performance issues as it is
+not critical. usage: upload_wl_usage.py [-h] --old-wl-file OLD_WL_FILE --out-
+file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials CREDENTIALS] [--
+upload-method UPLOAD_METHOD] Determine if a set of whitelist assets have been
+recently used in the vending machine optional arguments: -h, --help show this
+help message and exit --old-wl-file OLD_WL_FILE Most recent run of this program
+that was uploaded to cloud storage --out-file OUT_FILE Where to store the new
+used whitelist information if any changes (can be same as --old-wl-file) --
+whitelist-dir WHITELIST_DIR Local folder where consumed whitelist files have
+gone after processing by vending machine --whitelist-dir WHITELIST_DIR Local
+folder where unused whitelist files are stored to be processed by vending
+machine --credentials CREDENTIALS JSON-formatted application-specific
+credentials --upload-method UPLOAD_METHOD Mechanism for uploading changes in
+whitelist files (e.g., CloudFlare) ## APIs All API documentation is auto-
+generated from ``pydoc3``-formatted multi-line strings in the source code. A
+mirror of ``master`` is hosted on [Github Pages](https://
 thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
 Building this project creates a ``.whl`` file for uploading to [PyPI]() or
 installing locally on a server. All output is, by default, stored to ``dist/``.
 To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
```

### Comparing `cardano-nft-vending-machine-0.6.4/pyproject.toml` & `cardano-nft-vending-machine-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.3.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardano-nft-vending-machine"
-version = "0.6.4"
+version = "0.7.0"
 
 description = "Library to perform NFT mints automatically on the Cardano blockchain"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/blockfrost.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/blockfrost.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 import requests
 import time
 
 from http import HTTPStatus
 
+from cardano.wt import network
 from cardano.wt.utxo import Utxo
 
 """
 Repreentation of the Blockfrost web API used in retrieving metadata about txn i/o on the chain.
 """
 class BlockfrostApi(object):
 
-    PREPROD_MAGIC = '1'
-    PREVIEW_MAGIC = '2'
+    PREPROD_MAGIC = network.PREPROD_MAGIC
+    PREVIEW_MAGIC = network.PREVIEW_MAGIC
 
     _API_CALLS_PER_SEC = 10
     _APPLICATION_JSON = 'application/json'
     _BACKOFF_SEC = 10
     _MAX_GET_RETRIES = 9
     _MAX_POST_RETRIES = 2
     _UTXO_LIST_LIMIT = 100
```

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/cardano_cli.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/cardano_cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import os
 import subprocess
+import tempfile
 
 from deprecated import deprecated
 
+from cardano.wt import network
 from cardano.wt.utxo import Utxo
 
 """
 cardano-cli *nix script representation in Python
 """
 class CardanoCli(object):
 
@@ -21,29 +23,37 @@
         print(cmd)
         cli_cmd = subprocess.Popen(cmd,  shell=True, text=True, stdout=subprocess.PIPE)
         (out, err) = cli_cmd.communicate()
         print(f'[STDOUT] {out}')
         print(f'[STDERR] {err}')
         return out
 
-    def named_asset_str(nft_policy, nft_names):
-        return '+'.join(['.'.join([f"1 {nft_policy}", nft_name]) for nft_name in nft_names])
+    def named_assets_str(nft_policy_map):
+        named_assets = []
+        for policy in nft_policy_map:
+            for nft_name in nft_policy_map[policy]:
+                hex_name = nft_name.encode('UTF-8').hex()
+                named_assets.append(f"{policy}.{hex_name}")
+        return '+'.join([f"1 {named_asset}" for named_asset in named_assets])
 
     def build_raw_txn(self, output_dir, txn_id, tx_in_args, tx_out_args, fee, metadata_json_file, addl_args, era='--alonzo-era'):
         raw_build_file = os.path.join(output_dir, CardanoCli.TXN_DIR, f"txn_{txn_id}.raw.build")
         metadata_file_args = f"--metadata-json-file {metadata_json_file}" if metadata_json_file else ''
         self.__run_script(
             f'transaction build-raw --fee {fee} {era} {" ".join(tx_out_args)} {" ".join(tx_in_args)} \
                 {metadata_file_args} --out-file {raw_build_file} {" ".join(addl_args)}'
         )
         return raw_build_file
 
-    def build_raw_mint_txn(self, output_dir, txn_id, tx_in_args, tx_out_args, fee, metadata_json_file, mint, nft_names):
-        named_asset_str = CardanoCli.named_asset_str(mint.policy, nft_names)
-        mint_args = [f"--mint=\"{named_asset_str}\"", f"--minting-script-file {mint.script}"] if nft_names else []
+    def build_raw_mint_txn(self, output_dir, txn_id, tx_in_args, tx_out_args, fee, metadata_json_file, mint, nft_policy_map, scripts_map):
+        mint_args = []
+        if nft_policy_map:
+            named_asset_str = CardanoCli.named_assets_str(nft_policy_map)
+            mint_args.append(f"--mint=\"{named_asset_str}\"")
+            mint_args.extend([f"--minting-script-file {scripts_map[script]}" for script in scripts_map if script in nft_policy_map])
         if mint.initial_slot:
             mint_args.append(f"--invalid-before {mint.initial_slot}")
         if mint.expiration_slot:
             mint_args.append(f"--invalid-hereafter {mint.expiration_slot}")
         return self.build_raw_txn(output_dir, txn_id, tx_in_args, tx_out_args, fee, metadata_json_file, mint_args)
 
     def calculate_min_fee(self, raw_build_file, tx_in_count, tx_out_count, witness_count):
@@ -56,7 +66,21 @@
     def sign_txn(self, signing_files, build_file):
         signed_file = f"{build_file}.signed"
         signing_key_args = ' '.join([f"--signing-key-file {signing_file}" for signing_file in signing_files])
         self.__run_script(
             f'transaction sign {signing_key_args} --tx-body-file {build_file} --out-file {signed_file}'
         )
         return signed_file
+
+    def build_addr(self, payment_sign_key, mainnet=False):
+        with tempfile.NamedTemporaryFile() as verification_file:
+            self.__run_script(
+                f"key verification-key --signing-key-file {payment_sign_key} --verification-key-file {verification_file.name}"
+            )
+            network_flag = "--mainnet" if mainnet else f"--testnet-magic {network.PREPROD_MAGIC}"
+            address = self.__run_script(
+                f"address build --payment-verification-key-file {verification_file.name} {network_flag}"
+            )
+            return address.strip()
+
+    def policy_id(self, script_file):
+        return self.__run_script(f"transaction policyid --script-file {script_file}").strip()
```

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/mint.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/mint.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,46 +37,50 @@
             script_json = json.load(script_file)
         if 'scripts' in script_json:
             for validator in script_json['scripts']:
                 if validator['type'] == validation:
                     return validator[key]
         return None
 
-    def __init__(self, policy, price, dev_fee, dev_addr, nfts_dir, script, sign_key, whitelist, bogo=None):
-        self.policy = policy
+    def __init__(self, price, dev_fee, dev_addr, nfts_dir, scripts, sign_keys, whitelist, bogo=None):
         self.price = price
         self.dev_fee = dev_fee
         self.dev_addr = dev_addr
         self.nfts_dir = nfts_dir
-        self.script = script
-        self.sign_key = sign_key
+        self.scripts = scripts
+        self.sign_keys = sign_keys
         self.whitelist = whitelist
         self.bogo = bogo
 
-        self.initial_slot = Mint.__read_validator('after', 'slot', script)
-        self.expiration_slot = Mint.__read_validator('before', 'slot', script)
+        after_slots = list(filter(None, [Mint.__read_validator('after', 'slot', script) for script in self.scripts]))
+        self.initial_slot = min(after_slots) if after_slots else None
+        before_slots = list(filter(None, [Mint.__read_validator('before', 'slot', script) for script in self.scripts]))
+        self.expiration_slot = max(before_slots) if before_slots else None
 
     def validate(self):
         if self.dev_fee and self.dev_fee < Utxo.MIN_UTXO_VALUE:
             raise ValueError(f"Thank you for offering to pay your dev {self.dev_fee} but the minUTxO on Cardano is {Utxo.MIN_UTXO_VALUE} lovelace")
         if self.dev_fee and not self.dev_addr:
             raise ValueError(f"Thank you for offering to pay your dev {self.dev_fee} but you did not provide a dev address")
         if self.price and self.price < Mint._MIN_PRICE:
             raise ValueError(f"Minimum mint price is {Mint._MIN_PRICE}, you entered {self.price}")
         validated_names = []
         for filename in os.listdir(self.nfts_dir):
             with open(os.path.join(self.nfts_dir, filename), 'r') as file:
                 print(f"Validating '{filename}'")
-                validated_nft = self.__validated_nft(json.load(file), validated_names, filename)
-                validated_names.append(validated_nft)
+                validated_nfts = self.__validated_nft(json.load(file), validated_names, filename)
+                validated_names.extend(validated_nfts)
         self.validated_names = validated_names
-        if not os.path.exists(self.script):
-            raise ValueError(f"Minting script file '{self.script}' not found on filesystem")
-        if not os.path.exists(self.sign_key):
-            raise ValueError(f"Signing key file '{self.sign_key}' not found on filesystem")
+        for script in self.scripts:
+            if not os.path.exists(script):
+                raise ValueError(f"Minting script file '{script}' not found on filesystem")
+        for sign_key in self.sign_keys:
+            if not os.path.exists(sign_key):
+                raise ValueError(f"Signing key file '{sign_key}' not found on filesystem")
+        self.policies = list(set([nft_name.split('.')[0] for nft_name in self.validated_names]))
         print(f"Validating whitelist of type {self.whitelist.__class__}")
         self.whitelist.validate()
 
     def __validate_str_lengths(self, metadata):
         if type(metadata) is dict:
             for key, value in metadata.items():
                 self.__validate_str_lengths(value)
@@ -90,24 +94,23 @@
         if len(nft.keys()) != 1:
             raise ValueError(f"Incorrect # of keys ({len(nft.keys())}) found in file '{filename}'")
         if not Mint._METADATA_KEY in nft:
             raise ValueError(f"Missing top-level metadata key ({Mint._METADATA_KEY}) in file '{filename}'")
         nft_policy_obj = nft[Mint._METADATA_KEY]
         if len(nft_policy_obj.keys()) == 0:
             raise ValueError(f"No policy keys found in file '{filename}'")
-        if len(nft_policy_obj.keys()) > 2:
-            raise ValueError(f"Too many policy keys ({len(nft_policy_obj.keys())}) found in file '{filename}'")
-        if len(nft_policy_obj.keys()) == 2 and not 'version' in nft_policy_obj.keys():
-            raise ValueError(f"Found 2 keys but 1 is not 'version' (file '{filename}') [see CIP-0025]")
-        policy = sorted(list(nft_policy_obj.keys()))[0]
-        if len(policy) != Mint._POLICY_LEN:
-            raise ValueError(f"Incorrect looking policy {policy} in file '{filename}'")
-        if policy != self.policy:
-            raise ValueError(f"Encountered asset with policy {policy} different from vending machine start value {self.policy}")
-        asset_obj = nft_policy_obj[policy]
-        if len(asset_obj.keys()) != 1:
-            raise ValueError(f"Incorrect # of assets ({len(asset_obj.keys())}) found in file '{filename}'")
-        asset_name = list(asset_obj.keys())[0]
-        if asset_name in existing:
-            raise ValueError(f"Found duplicate asset name '{asset_name}' in file '{filename}'")
-        self.__validate_str_lengths(asset_obj)
-        return asset_name
+        asset_names = []
+        for policy in nft_policy_obj:
+            if policy == 'version':
+                continue
+            if len(policy) != Mint._POLICY_LEN:
+                raise ValueError(f"Incorrect looking policy {policy} in file '{filename}'")
+            asset_obj = nft_policy_obj[policy]
+            if len(asset_obj.keys()) == 0:
+                raise ValueError(f"Need at least 1 asset for policy '{policy}' in file '{filename}'")
+            asset_name = list(asset_obj.keys())[0]
+            full_name = f"{policy}.{asset_name}"
+            if full_name in existing:
+                raise ValueError(f"Found duplicate asset name '{full_name}' in file '{filename}'")
+            self.__validate_str_lengths(asset_obj)
+            asset_names.append(full_name)
+        return asset_names
```

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/nft_vending_machine.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/nft_vending_machine.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,48 +29,53 @@
         self.payment_sign_key = payment_sign_key
         self.profit_addr = profit_addr
         self.vend_randomly = vend_randomly
         self.single_vend_max = single_vend_max
         self.mint = mint
         self.blockfrost_api = blockfrost_api
         self.cardano_cli = cardano_cli
+        self.mainnet = mainnet
         self.__is_validated = False
 
-    def __get_tx_out_args(self, input_addr, change, nft_names, total_profit, total_dev_fee):
-        user_tokens = filter(None, [input_addr, str(change), CardanoCli.named_asset_str(self.mint.policy, nft_names)])
+    def __get_tx_out_args(self, input_addr, change, nft_policy_map, total_profit, total_dev_fee):
+        user_tokens = filter(None, [input_addr, str(change), CardanoCli.named_assets_str(nft_policy_map)])
         user_output = f"--tx-out \"{'+'.join(user_tokens)}\""
         profit_output = f"--tx-out \"{self.profit_addr}+{total_profit}\"" if total_profit else ''
         dev_output = f"--tx-out \"{self.mint.dev_addr}+{total_dev_fee}\"" if total_dev_fee else ''
         return [user_output, profit_output, dev_output]
 
-    def __generate_nft_names_from(self, metadata_file):
+    def __get_policy_name_map(self, metadata_file):
+        nft_names = {}
         with open(metadata_file, 'r') as metadata_filehandle:
-            policy_json = json.load(metadata_filehandle)['721'][self.mint.policy]
-            names = policy_json.keys()
-            return [name.encode('UTF-8').hex() for name in names]
-
-    def __get_nft_names_from(self, metadata_file):
-        with open(metadata_file, 'r') as metadata_filehandle:
-            policy_json = json.load(metadata_filehandle)['721'][self.mint.policy]
-            return policy_json.keys()
+            cip25_metadata = json.load(metadata_filehandle)['721']
+            for policy in cip25_metadata:
+                if policy == 'version':
+                    continue
+                nft_names[policy] = list(cip25_metadata[policy].keys())
+        return nft_names
 
     def __lock_and_merge(self, available_mints, num_mints, output_dir, locked_subdir, metadata_subdir, txn_id):
         combined_nft_metadata = {}
         for i in range(num_mints):
             mint_metadata_filename = available_mints.pop(0)
             mint_metadata_orig = os.path.join(self.mint.nfts_dir, mint_metadata_filename)
             with open(mint_metadata_orig, 'r') as mint_metadata_handle:
                 mint_metadata = json.load(mint_metadata_handle)
-                for nft_name, nft_metadata in mint_metadata['721'][self.mint.policy].items():
-                    combined_nft_metadata[nft_name] = nft_metadata
+                for policy in mint_metadata['721']:
+                    if policy == 'version':
+                        continue
+                    for nft_name, nft_metadata in mint_metadata['721'][policy].items():
+                        if not policy in combined_nft_metadata:
+                            combined_nft_metadata[policy] = {}
+                        combined_nft_metadata[policy][nft_name] = nft_metadata
             mint_metadata_locked = os.path.join(output_dir, locked_subdir, mint_metadata_filename)
             shutil.move(mint_metadata_orig, mint_metadata_locked)
         combined_output_path = os.path.join(output_dir, metadata_subdir, f"{txn_id}.json")
         with open(combined_output_path, 'w') as combined_metadata_handle:
-            json.dump({'721': { self.mint.policy : combined_nft_metadata }}, combined_metadata_handle)
+            json.dump({'721': combined_nft_metadata }, combined_metadata_handle)
         return combined_output_path
 
     def __do_vend(self, mint_req, output_dir, locked_subdir, metadata_subdir):
         available_mints = sorted(os.listdir(self.mint.nfts_dir))
         if not available_mints:
             print("WARNING: Metadata directory is empty, please restock the vending machine...")
         elif self.vend_randomly:
@@ -112,44 +117,45 @@
             bonuses = self.mint.bogo.determine_bonuses(num_mints_requested)
             print(f"Bonus of {bonuses} NFTs determined based on {num_mints_requested}")
             num_mints = min(self.single_vend_max, len(available_mints), (num_mints + bonuses))
 
         print(f"Beginning to mint {num_mints} NFTs to send to address {input_addr}")
         txn_id = int(time.time())
         nft_metadata_file = self.__lock_and_merge(available_mints, num_mints, output_dir, locked_subdir, metadata_subdir, txn_id)
-        nft_names = self.__generate_nft_names_from(nft_metadata_file)
+        nft_policy_map = self.__get_policy_name_map(nft_metadata_file)
 
-        total_name_chars = sum([len(name) for name in self.__get_nft_names_from(nft_metadata_file)])
-        user_rebate = Mint.RebateCalculator.calculate_rebate_for(NftVendingMachine.__SINGLE_POLICY, num_mints, total_name_chars) if self.mint.price else 0
+        all_names = [name for name_lst in nft_policy_map.values() for name in name_lst]
+        total_name_chars = sum([len(name) for name in all_names])
+        user_rebate = Mint.RebateCalculator.calculate_rebate_for(len(nft_policy_map.keys()), len(all_names), total_name_chars) if self.mint.price else 0
         dev_fee = num_mints * self.mint.dev_fee
         net_profit = gross_profit - dev_fee - user_rebate
         print(f"Minimum rebate to user is {user_rebate}, net profit to vault is {net_profit}")
 
         tx_ins = [f"--tx-in {mint_req.hash}#{mint_req.ix}"]
-        tx_outs = self.__get_tx_out_args(input_addr, user_rebate + change, nft_names, net_profit, dev_fee)
-        mint_build_tmp = self.cardano_cli.build_raw_mint_txn(output_dir, txn_id, tx_ins, tx_outs, 0, nft_metadata_file, self.mint, nft_names)
+        tx_outs = self.__get_tx_out_args(input_addr, user_rebate + change, nft_policy_map, net_profit, dev_fee)
+        mint_build_tmp = self.cardano_cli.build_raw_mint_txn(output_dir, txn_id, tx_ins, tx_outs, 0, nft_metadata_file, self.mint, nft_policy_map, self.script_map)
 
         tx_in_count = len(tx_ins)
         tx_out_count = len([tx_out for tx_out in tx_outs if tx_out])
         signers = [self.payment_sign_key]
         if num_mints:
-            signers.append(self.mint.sign_key)
+            signers.extend(self.mint.sign_keys)
         fee = self.cardano_cli.calculate_min_fee(mint_build_tmp, tx_in_count, tx_out_count, len(signers))
 
         if net_profit:
             net_profit = net_profit - fee
         else:
             change = change - fee
 
         final_change = user_rebate + change
         if (final_change and (final_change < Utxo.MIN_UTXO_VALUE)) or (net_profit and (net_profit < Utxo.MIN_UTXO_VALUE)):
             raise BadUtxoError(mint_req, f"UTxO left change of {change}, and net_profit of {net_profit}, causing a minUTxO error")
 
-        tx_outs = self.__get_tx_out_args(input_addr, final_change, nft_names, net_profit, dev_fee)
-        mint_build = self.cardano_cli.build_raw_mint_txn(output_dir, txn_id, tx_ins, tx_outs, fee, nft_metadata_file, self.mint, nft_names)
+        tx_outs = self.__get_tx_out_args(input_addr, final_change, nft_policy_map, net_profit, dev_fee)
+        mint_build = self.cardano_cli.build_raw_mint_txn(output_dir, txn_id, tx_ins, tx_outs, fee, nft_metadata_file, self.mint, nft_policy_map, self.script_map)
         mint_signed = self.cardano_cli.sign_txn(signers, mint_build)
         self.mint.whitelist.consume(wl_resources, num_mints)
         self.blockfrost_api.submit_txn(mint_signed)
 
     def vend(self, output_dir, locked_subdir, metadata_subdir, exclusions):
         if not self.__is_validated:
             raise ValueError('Attempting to vend from non-validated vending machine')
@@ -163,22 +169,39 @@
                 print(traceback.format_exc())
             except Exception as e:
                 print(f"WARNING: Uncaught exception for {mint_req}, added to exclusions (RETRY WILL NOT BE ATTEMPTED)")
                 print(traceback.format_exc())
                 time.sleep(NftVendingMachine.__ERROR_WAIT)
 
     def validate(self):
+        self.mint.validate()
         if self.payment_addr == self.profit_addr:
             raise ValueError(f"Payment address and profit address ({self.payment_addr}) cannot be the same!")
-        self.mint.validate()
         self.max_rebate = self.__max_rebate_for(self.mint.validated_names)
         if self.mint.price and self.mint.price < (self.max_rebate + self.mint.dev_fee + Utxo.MIN_UTXO_VALUE):
             raise ValueError(f"Price of {self.mint.price} with dev fee of {self.mint.dev_fee} could lead to a minUTxO error due to rebates")
+        if not os.path.exists(self.payment_sign_key):
+            raise ValueError(f"Payment signing key file '{self.payment_sign_key}' not found on filesystem")
+        expected_payment_addr = self.cardano_cli.build_addr(self.payment_sign_key, self.mainnet)
+        if not expected_payment_addr == self.payment_addr:
+            raise ValueError(f"Could not match {self.payment_addr} to signature at '{self.payment_sign_key}' (expected {expected_payment_addr})")
+        self.script_map = {}
+        for policy in self.mint.policies:
+            self.script_map[policy] = self.__validate_script_file(policy)
+            if not self.script_map[policy]:
+                raise ValueError(f"No matching script file found for policy {policy}")
         self.__is_validated = True
 
+    def __validate_script_file(self, policy):
+        for script in self.mint.scripts:
+            if self.cardano_cli.policy_id(script) == policy:
+                return script
+        return None
+
     def __max_rebate_for(self, nft_names):
-        max_len = 0 if not nft_names else max([len(nft_name) for nft_name in nft_names])
+        max_len = 0 if not nft_names else max([len(nft_name.split('.')[1]) for nft_name in nft_names])
+        all_policies = [nft_name.split('.')[0] for nft_name in nft_names]
         return Mint.RebateCalculator.calculate_rebate_for(
-            NftVendingMachine.__SINGLE_POLICY,
+            len(set(all_policies)),
             self.single_vend_max,
             max_len * self.single_vend_max
         )
```

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/utxo.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/utxo.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/asset_whitelist.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/asset_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/filesystem.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/filesystem.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/no_whitelist.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/no_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano/wt/whitelist/wallet_whitelist.py` & `cardano-nft-vending-machine-0.7.0/src/cardano/wt/whitelist/wallet_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/PKG-INFO` & `cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.6.4
+Version: 0.7.0
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -44,16 +44,16 @@
 This project contains Library bindings that can be installed using the standard [wheel](https://pypi.org/project/wheel/) mechanism.  See the [script quickstart section](#cardano_vending_machinepy) for how to run from CLI.
 ### Library Usage
 The library consists of several Python objects representing the mint process.  The sample below shows how one could run an infinite CNFT vending machine on mainnet for a 10₳ mint (gross of fees and rebates) with their NFT:
 
     # There are several sample whitelist implementations in cardano.wt.whitelist or you can implement your own
     whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/directory')
 
-    # The Mint object below represents your Mint policy and specifies price, and developer fee in Lovelace (both can be 0)
-    mint = Mint('<POLICY_ID>', 10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
+    # The Mint object below represents your Mint and specifies price, and developer fee in Lovelace (both can be 0)
+    mint = Mint(10000000, 1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/path/to/mint.skey', whitelist)
 
     # Blockfrost is used in the code to validate where the UTXO sent to the payment address came from
     blockfrost_api = BlockfrostApi('<BLOCKFROST_PROJ_ID>', mainnet=True)
 
     # CardanoCli is a wrapper around the cardano-cli command (used as a utility without any interaction with the network)
     cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json')
 
@@ -72,15 +72,14 @@
         python3 main.py [validate | run] \
                 --payment-addr <PAYMENT_ADDR> \
                 --payment-sign-key /FULL/PATH/TO/payment.skey \
                 --profit-addr <PROFIT_ADDR> \
                 [--mint-price <PRICE_LOVELACE> | --free-mint] \
                 --mint-script /FULL/PATH/TO/policy.script \
                 --mint-sign-key /FULL/PATH/TO/policy.skey \
-                --mint-policy $(cat /FULL/PATH/TO/policyID) \
                 --blockfrost-project <BLOCKFROST_PROJECT_ID> \
                 --metadata-dir metadata/ \
                 --output-dir output/ \
                 --single-vend-max <MAX_SINGLE_VEND> \
                 [--vend-randomly] \
                 [--no-whitelist | \
                   [--single-use-asset-whitelist <WHITELIST_DIR> \
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.4 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.7.0 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
@@ -28,19 +28,19 @@
 pypi.org/project/wheel/) mechanism. See the [script quickstart section]
 (#cardano_vending_machinepy) for how to run from CLI. ### Library Usage The
 library consists of several Python objects representing the mint process. The
 sample below shows how one could run an infinite CNFT vending machine on
 mainnet for a 10â³ mint (gross of fees and rebates) with their NFT: # There
 are several sample whitelist implementations in cardano.wt.whitelist or you can
 implement your own whitelist = SingleUseWhitelist('/path/to/whitelisted/assets/
-directory') # The Mint object below represents your Mint policy and specifies
-price, and developer fee in Lovelace (both can be 0) mint = Mint('', 10000000,
-1000000, 'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/
-script', '/path/to/mint.skey', whitelist) # Blockfrost is used in the code to
-validate where the UTXO sent to the payment address came from blockfrost_api =
+directory') # The Mint object below represents your Mint and specifies price,
+and developer fee in Lovelace (both can be 0) mint = Mint(10000000, 1000000,
+'addr1_developer', '/path/to/nft/json/metadata', '/path/to/mint/script', '/
+path/to/mint.skey', whitelist) # Blockfrost is used in the code to validate
+where the UTXO sent to the payment address came from blockfrost_api =
 BlockfrostApi('', mainnet=True) # CardanoCli is a wrapper around the cardano-
 cli command (used as a utility without any interaction with the network)
 cardano_cli = CardanoCli(protocol_params='/path/to/protocol.json') #
 NftVendingMachine vends NFTs and needs to be called repeatedly (with a 25-vend
 max) so long as the mint period is open nft_vending_machine = NftVendingMachine
 ('addr_payment', '/path/to/payment.skey', 'addr_profit', 25, mint,
 blockfrost_api, cardano_cli, mainnet=True) # The following simple loop carries
@@ -49,61 +49,61 @@
 nft_vending_machine.vend('/path/to/output/dir', 'locking_subdir_name',
 'metadata_subdir_name', already_completed) time.sleep(WAIT_TIMEOUT) ###
 ``main.py`` There is a sample vending machine script that is included in the
 ``src/`` directory to show how to invoke the library components. Use ``-h`` to
 see detailed help or use a command like below: python3 main.py [validate | run]
 \ --payment-addr  \ --payment-sign-key /FULL/PATH/TO/payment.skey \ --profit-
 addr  \ [--mint-price  | --free-mint] \ --mint-script /FULL/PATH/TO/
-policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --mint-policy $(cat
-/FULL/PATH/TO/policyID) \ --blockfrost-project  \ --metadata-dir metadata/ \ --
-output-dir output/ \ --single-vend-max  \ [--vend-randomly] \ [--no-whitelist |
-\ [--single-use-asset-whitelist  \ | --unlimited-asset-whitelist  \ | --wallet-
-whitelist  ] \ [--dev-fee dev_fee --dev-addr dev_addr] \ [--bogo threshold
-additional] \ [--mainnet] ## Installation This package is available from [PyPI]
-(https://pypi.org/) and can be installed using ``pip3``. Python <3.8 is
-currently unsupported at this time. pip3 install cardano-nft-vending-machine
-### Scripts In the `scripts/` directory there are several scripts that can be
-used to help operationalize the vending machine. #### initialize_whitelist.py
-This file should be used exactly once to initialize an asset-based whitelist
-for an existing NFT policy with *ALL* of the assets that are currently minted.
-Note that the `CONSUMED_DIR` folder is created but left empty so that the
-vending machine (e.g., started with `main.py`) can use it during running.
-usage: initialize_whitelist.py [-h] asset --blockfrost-project
-BLOCKFROST_PROJECT --consumed-dir CONSUMED_DIR [--mainnet] --policy-id
-POLICY_ID [--preview] --whitelist-dir WHITELIST_DIR Initialize an asset-based
-whitelist for an existing NFT policy optional arguments: -h, --help show this
-help message and exit --blockfrost-project BLOCKFROST_PROJECT Blockfrost
-project ID to use for retrieving chain data --consumed-dir CONSUMED_DIR Local
-folder where consumed whitelist files will go after processing (MUST NOT YET
-EXIST) --mainnet Run the initializer against mainnet assets (default is False
-[preprod]) --policy-id POLICY_ID Policy ID of the assets to be whitelisted --
-preview Run the initializer against preview assets (default is False [preprod])
---whitelist-dir WHITELIST_DIR Local folder where whitelist files are stored
-(MUST NOT YET EXIST) --num-mints-per-wl NUMBER How many whitelist spots are
-available for each asset on the whitelist #### upload_wl_usage.py This file
-should be run continuously during a whitelist mint to upload changes in the
-assets used for consumption by external parties. Note that if there are any
-performance issues (e.g., IOPS throughput) with the local vending machine
-filesystem it is recommended you not use this file. It is kept separate from
-the main vending machine operation to avoid any synchronization or performance
-issues as it is not critical. usage: upload_wl_usage.py [-h] --old-wl-file
-OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
-CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
-assets have been recently used in the vending machine optional arguments: -h, -
--help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
-of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
-store the new used whitelist information if any changes (can be same as --old-
-wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
-files have gone after processing by vending machine --whitelist-dir
-WHITELIST_DIR Local folder where unused whitelist files are stored to be
-processed by vending machine --credentials CREDENTIALS JSON-formatted
-application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
-uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
-documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
-the source code. A mirror of ``master`` is hosted on [Github Pages](https://
+policy.script \ --mint-sign-key /FULL/PATH/TO/policy.skey \ --blockfrost-
+project  \ --metadata-dir metadata/ \ --output-dir output/ \ --single-vend-max
+\ [--vend-randomly] \ [--no-whitelist | \ [--single-use-asset-whitelist  \ | --
+unlimited-asset-whitelist  \ | --wallet-whitelist  ] \ [--dev-fee dev_fee --
+dev-addr dev_addr] \ [--bogo threshold additional] \ [--mainnet] ##
+Installation This package is available from [PyPI](https://pypi.org/) and can
+be installed using ``pip3``. Python <3.8 is currently unsupported at this time.
+pip3 install cardano-nft-vending-machine ### Scripts In the `scripts/
+` directory there are several scripts that can be used to help operationalize
+the vending machine. #### initialize_whitelist.py This file should be used
+exactly once to initialize an asset-based whitelist for an existing NFT policy
+with *ALL* of the assets that are currently minted. Note that the
+`CONSUMED_DIR` folder is created but left empty so that the vending machine
+(e.g., started with `main.py`) can use it during running. usage:
+initialize_whitelist.py [-h] asset --blockfrost-project BLOCKFROST_PROJECT --
+consumed-dir CONSUMED_DIR [--mainnet] --policy-id POLICY_ID [--preview] --
+whitelist-dir WHITELIST_DIR Initialize an asset-based whitelist for an existing
+NFT policy optional arguments: -h, --help show this help message and exit --
+blockfrost-project BLOCKFROST_PROJECT Blockfrost project ID to use for
+retrieving chain data --consumed-dir CONSUMED_DIR Local folder where consumed
+whitelist files will go after processing (MUST NOT YET EXIST) --mainnet Run the
+initializer against mainnet assets (default is False [preprod]) --policy-id
+POLICY_ID Policy ID of the assets to be whitelisted --preview Run the
+initializer against preview assets (default is False [preprod]) --whitelist-dir
+WHITELIST_DIR Local folder where whitelist files are stored (MUST NOT YET
+EXIST) --num-mints-per-wl NUMBER How many whitelist spots are available for
+each asset on the whitelist #### upload_wl_usage.py This file should be run
+continuously during a whitelist mint to upload changes in the assets used for
+consumption by external parties. Note that if there are any performance issues
+(e.g., IOPS throughput) with the local vending machine filesystem it is
+recommended you not use this file. It is kept separate from the main vending
+machine operation to avoid any synchronization or performance issues as it is
+not critical. usage: upload_wl_usage.py [-h] --old-wl-file OLD_WL_FILE --out-
+file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials CREDENTIALS] [--
+upload-method UPLOAD_METHOD] Determine if a set of whitelist assets have been
+recently used in the vending machine optional arguments: -h, --help show this
+help message and exit --old-wl-file OLD_WL_FILE Most recent run of this program
+that was uploaded to cloud storage --out-file OUT_FILE Where to store the new
+used whitelist information if any changes (can be same as --old-wl-file) --
+whitelist-dir WHITELIST_DIR Local folder where consumed whitelist files have
+gone after processing by vending machine --whitelist-dir WHITELIST_DIR Local
+folder where unused whitelist files are stored to be processed by vending
+machine --credentials CREDENTIALS JSON-formatted application-specific
+credentials --upload-method UPLOAD_METHOD Mechanism for uploading changes in
+whitelist files (e.g., CloudFlare) ## APIs All API documentation is auto-
+generated from ``pydoc3``-formatted multi-line strings in the source code. A
+mirror of ``master`` is hosted on [Github Pages](https://
 thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
 Building this project creates a ``.whl`` file for uploading to [PyPI]() or
 installing locally on a server. All output is, by default, stored to ``dist/``.
 To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
```

### Comparing `cardano-nft-vending-machine-0.6.4/src/cardano_nft_vending_machine.egg-info/SOURCES.txt` & `cardano-nft-vending-machine-0.7.0/src/cardano_nft_vending_machine.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 src/cardano/__init__.py
 src/cardano/wt/__init__.py
 src/cardano/wt/blockfrost.py
 src/cardano/wt/cardano_cli.py
 src/cardano/wt/mint.py
+src/cardano/wt/network.py
 src/cardano/wt/nft_vending_machine.py
 src/cardano/wt/utxo.py
 src/cardano/wt/bonuses/__init__.py
 src/cardano/wt/bonuses/bogo.py
 src/cardano/wt/whitelist/__init__.py
 src/cardano/wt/whitelist/asset_whitelist.py
 src/cardano/wt/whitelist/filesystem.py
```

