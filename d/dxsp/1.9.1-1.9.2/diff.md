# Comparing `tmp/dxsp-1.9.1.tar.gz` & `tmp/dxsp-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.9.1.tar", max compression
+gzip compressed data, was "dxsp-1.9.2.tar", max compression
```

## Comparing `dxsp-1.9.1.tar` & `dxsp-1.9.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-05 18:51:36.092758 dxsp-1.9.1/LICENSE
--rw-r--r--   0        0        0     3215 2023-05-05 18:51:36.092758 dxsp-1.9.1/README.md
--rw-r--r--   0        0        0       38 2023-05-05 18:51:36.092758 dxsp-1.9.1/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-05 18:51:36.780769 dxsp-1.9.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-05 18:51:36.092758 dxsp-1.9.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-05 18:51:36.092758 dxsp-1.9.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-05 18:51:36.092758 dxsp-1.9.1/dxsp/config.py
--rw-r--r--   0        0        0      556 2023-05-05 18:51:36.092758 dxsp-1.9.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28346 2023-05-05 18:51:36.092758 dxsp-1.9.1/dxsp/main.py
--rw-r--r--   0        0        0     1787 2023-05-05 18:51:36.780769 dxsp-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 dxsp-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 04:33:25.279697 dxsp-1.9.2/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-06 04:33:25.279697 dxsp-1.9.2/README.md
+-rw-r--r--   0        0        0       38 2023-05-06 04:33:25.279697 dxsp-1.9.2/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-06 04:33:26.023700 dxsp-1.9.2/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-06 04:33:25.279697 dxsp-1.9.2/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-06 04:33:25.279697 dxsp-1.9.2/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-06 04:33:25.279697 dxsp-1.9.2/dxsp/config.py
+-rw-r--r--   0        0        0      556 2023-05-06 04:33:25.279697 dxsp-1.9.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28346 2023-05-06 04:33:25.279697 dxsp-1.9.2/dxsp/main.py
+-rw-r--r--   0        0        0     1787 2023-05-06 04:33:26.023700 dxsp-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.2/PKG-INFO
```

### Comparing `dxsp-1.9.1/LICENSE` & `dxsp-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.1/README.md` & `dxsp-1.9.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # DXSP (DeX SwaP)
 
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) ![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
+|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
 
 
 Key features:
 
 - 24 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
 - 2 swap protocol type supported:
```

### Comparing `dxsp-1.9.1/dxsp/assets/blockchains.py` & `dxsp-1.9.2/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.1/dxsp/default_settings.toml` & `dxsp-1.9.2/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.1/dxsp/main.py` & `dxsp-1.9.2/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.1/pyproject.toml` & `dxsp-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.9.1"
+version = "1.9.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.9.1/PKG-INFO` & `dxsp-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.9.1
+Version: 1.9.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
 
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) ![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
+|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
 
 
 Key features:
 
 - 24 blockchains mainnet and testnet supported with default block explorer, RPC, Router (uniswap and pancakeswap) and protocol url (1inch and 0x). Other blockchains can be supported via function attributes
 - 2 swap protocol type supported:
```

