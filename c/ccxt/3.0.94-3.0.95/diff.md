# Comparing `tmp/ccxt-3.0.94.tar.gz` & `tmp/ccxt-3.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-3.0.94.tar", last modified: Fri May  5 16:10:46 2023, max compression
+gzip compressed data, was "dist/ccxt-3.0.95.tar", last modified: Sat May  6 00:35:33 2023, max compression
```

## Comparing `ccxt-3.0.94.tar` & `ccxt-3.0.95.tar`

### file list

```diff
@@ -1,487 +1,487 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.430756 ccxt-3.0.94/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-05-05 16:10:30.000000 ccxt-3.0.94/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-05 15:55:39.000000 ccxt-3.0.94/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-05 16:10:46.434757 ccxt-3.0.94/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-05-05 15:55:39.000000 ccxt-3.0.94/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.094733 ccxt-3.0.94/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15626 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.170738 ccxt-3.0.94/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11071 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2347 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17077 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8966 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8653 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22372 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5594 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71684 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9017 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14759 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3736 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7452 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6840 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20893 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10639 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/stex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7689 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25850 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41329 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33161 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   127668 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.318749 ccxt-3.0.94/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15429 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41553 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33307 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128282 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.322749 ccxt-3.0.94/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128268 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.330749 ccxt-3.0.94/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62726 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   374663 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35688 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46227 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69752 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111979 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38049 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   204759 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42790 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131902 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   120028 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63629 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87760 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88471 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68835 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82612 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17931 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93903 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77171 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74597 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16351 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47523 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35438 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22683 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111410 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48897 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22323 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35602 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45959 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/buda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   394329 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65248 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125230 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74293 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34414 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191811 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39252 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39813 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34679 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81496 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18912 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108492 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80021 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84440 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119560 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152866 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89266 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   221908 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69449 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62675 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117197 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69616 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   357192 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87087 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67772 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30046 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42709 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35208 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/itbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101946 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82058 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160977 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98228 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37998 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70399 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33953 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98405 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40781 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48763 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34881 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   210181 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106630 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62006 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37393 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   178258 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   265343 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22933 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   192396 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88811 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75472 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68946 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47585 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ripio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118368 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/stex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42655 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65784 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119594 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75965 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103947 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35792 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92591 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95037 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   188966 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51652 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28959 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   184533 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74326 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.334750 ccxt-3.0.94/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-05-05 16:07:38.000000 ccxt-3.0.94/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   169537 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62340 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   373477 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35482 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39008 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45973 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69312 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111509 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37741 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28316 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   203909 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42572 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131264 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119564 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63261 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87308 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88097 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68449 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82190 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17785 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93397 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76761 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74167 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16241 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47095 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35160 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22489 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   110784 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48547 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22177 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35384 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45591 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/buda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   392459 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64922 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   124586 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73787 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34208 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   190913 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38956 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39565 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34455 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81092 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18778 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   107966 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79629 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84060 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119018 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152160 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88724 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   221082 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69001 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62241 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116511 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69194 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   355886 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86605 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67332 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29810 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42437 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34960 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/itbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101404 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81756 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160363 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97782 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37750 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70007 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33717 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97857 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40473 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48461 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34639 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   209135 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106106 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61638 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37055 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   177794 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   264325 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22745 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191812 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88311 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75104 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.390754 ccxt-3.0.94/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6039 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26668 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34553 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77193 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41903 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44698 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24486 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55606 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12557 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16235 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20784 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36705 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26009 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31132 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60648 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44892 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29075 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40578 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22975 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22087 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33925 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24397 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41718 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21786 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    85533 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23052 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28068 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11059 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44317 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52058 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34128 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27781 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41886 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30234 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35657 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    59743 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22635 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/ripio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29862 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34279 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25030 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68596 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47325 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ripio.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.390754 ccxt-3.0.94/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.398754 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.398754 ccxt-3.0.94/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/keccak/keccak.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117868 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/stex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.402754 ccxt-3.0.94/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.426756 ccxt-3.0.94/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-05-05 16:07:42.000000 ccxt-3.0.94/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      922 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2110 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-05-05 16:07:41.000000 ccxt-3.0.94/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2145 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5234 2023-05-05 16:07:40.000000 ccxt-3.0.94/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1957 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5671 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22034 2023-05-05 16:07:40.000000 ccxt-3.0.94/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2025 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1327 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3392 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2983 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3526 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10987 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1226 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4935 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1850 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26500 2023-05-05 16:07:42.000000 ccxt-3.0.94/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26096 2023-05-05 16:07:42.000000 ccxt-3.0.94/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42407 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65452 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119250 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75531 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103453 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35544 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92139 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    94453 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   187865 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51368 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28777 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   183857 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74036 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.098733 ccxt-3.0.94/ccxt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11640 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8459 2023-05-05 16:10:29.000000 ccxt-3.0.94/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-05-05 16:10:46.438757 ccxt-3.0.94/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-05-05 15:55:39.000000 ccxt-3.0.94/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.817483 ccxt-3.0.95/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-05-06 00:35:18.000000 ccxt-3.0.95/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-06 00:09:53.000000 ccxt-3.0.95/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-06 00:35:33.821483 ccxt-3.0.95/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-05-06 00:09:53.000000 ccxt-3.0.95/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.665467 ccxt-3.0.95/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15626 2023-05-06 00:35:17.000000 ccxt-3.0.95/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.693470 ccxt-3.0.95/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11071 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2347 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17077 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8966 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8653 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22372 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5594 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71684 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9017 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14759 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3736 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7452 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6840 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20893 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10639 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/stex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7689 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25850 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-06 00:13:54.000000 ccxt-3.0.95/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41329 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33161 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   127668 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.741475 ccxt-3.0.95/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15429 2023-05-06 00:35:17.000000 ccxt-3.0.95/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41553 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33307 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128282 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.741475 ccxt-3.0.95/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128268 2023-05-06 00:35:17.000000 ccxt-3.0.95/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.745475 ccxt-3.0.95/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62726 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   374663 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35688 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46227 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69752 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111979 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38049 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   204759 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42790 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131902 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   120028 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63629 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87760 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88471 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68835 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82612 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17931 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93903 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77171 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74597 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16351 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47523 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35438 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22683 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111410 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48897 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22323 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35602 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45959 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/buda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   394329 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65248 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125230 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74293 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34414 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191811 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39252 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39813 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34679 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81496 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18912 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108492 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80021 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84440 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119560 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152866 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89266 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   221908 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69449 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62675 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117197 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69616 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   357192 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87087 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67772 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30046 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42709 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35208 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/itbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101946 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82058 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160977 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98228 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37998 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70399 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33953 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98405 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40781 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48763 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34881 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   210181 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106630 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62006 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37393 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   178258 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   265343 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22933 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   192396 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88811 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75472 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68946 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47585 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/ripio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118368 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/stex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42655 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65784 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119594 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75965 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103947 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35792 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92591 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95037 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   188868 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51652 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28959 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   184533 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74326 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.745475 ccxt-3.0.95/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-05-06 00:21:39.000000 ccxt-3.0.95/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   169537 2023-05-06 00:35:17.000000 ccxt-3.0.95/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62340 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   373477 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35482 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39008 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45973 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69312 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111509 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37741 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28316 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   203909 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42572 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131264 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119564 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63261 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87308 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88097 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68449 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82190 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17785 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93397 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76761 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74167 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16241 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47095 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35160 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22489 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110784 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48547 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22177 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35384 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45591 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/buda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   392459 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64922 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   124586 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73787 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34208 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   190913 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38956 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39565 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34455 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81092 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18778 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   107966 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79629 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84060 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119018 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152160 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88724 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   221082 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69001 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62241 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116511 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69194 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   355886 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86605 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67332 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29810 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42437 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34960 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/itbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101404 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81756 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160363 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97782 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37750 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70007 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33717 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97857 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40473 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48461 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34639 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   209135 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106106 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61638 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37055 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   177794 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   264325 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22745 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191812 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88311 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75104 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.789480 ccxt-3.0.95/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6039 2023-05-06 00:35:17.000000 ccxt-3.0.95/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26668 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34553 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77193 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41903 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44698 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24486 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55606 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12557 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16235 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20784 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36705 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26009 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31132 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60648 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44892 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29075 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40578 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22975 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22087 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33925 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24397 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41718 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21786 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85533 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23052 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28068 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11059 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44317 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52058 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34128 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27781 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41886 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30234 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35657 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    59743 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22635 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/ripio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29862 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34279 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25030 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/pro/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68596 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47325 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/ripio.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.789480 ccxt-3.0.95/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.789480 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.805481 ccxt-3.0.95/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/static_dependencies/keccak/keccak.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117868 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/stex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.805481 ccxt-3.0.95/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.817483 ccxt-3.0.95/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-05-06 00:21:44.000000 ccxt-3.0.95/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      922 2023-05-06 00:22:51.000000 ccxt-3.0.95/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2110 2023-05-06 00:22:51.000000 ccxt-3.0.95/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2023-05-06 00:22:51.000000 ccxt-3.0.95/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2023-05-06 00:22:51.000000 ccxt-3.0.95/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-05-06 00:21:42.000000 ccxt-3.0.95/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2145 2023-05-06 00:22:51.000000 ccxt-3.0.95/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5234 2023-05-06 00:21:41.000000 ccxt-3.0.95/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1957 2023-05-06 00:22:51.000000 ccxt-3.0.95/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5671 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22034 2023-05-06 00:21:41.000000 ccxt-3.0.95/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2025 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1327 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3392 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2983 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3526 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10987 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1226 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4935 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1850 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-06 00:22:52.000000 ccxt-3.0.95/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26500 2023-05-06 00:21:43.000000 ccxt-3.0.95/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26096 2023-05-06 00:21:43.000000 ccxt-3.0.95/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42407 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65452 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119250 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75531 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103453 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35544 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92139 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94453 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   187767 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51368 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28777 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   183857 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74036 2023-05-06 00:09:53.000000 ccxt-3.0.95/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-06 00:35:33.665467 ccxt-3.0.95/ccxt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-06 00:35:33.000000 ccxt-3.0.95/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11640 2023-05-06 00:35:33.000000 ccxt-3.0.95/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-06 00:35:33.000000 ccxt-3.0.95/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-05-06 00:35:33.000000 ccxt-3.0.95/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-05-06 00:35:33.000000 ccxt-3.0.95/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8459 2023-05-06 00:35:18.000000 ccxt-3.0.95/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-05-06 00:35:33.821483 ccxt-3.0.95/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-05-06 00:09:53.000000 ccxt-3.0.95/setup.py
```

### Comparing `ccxt-3.0.94/LICENSE.txt` & `ccxt-3.0.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/PKG-INFO` & `ccxt-3.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 3.0.94
+Version: 3.0.95
 Summary: A JavaScript / Python / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -227,21 +227,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@3.0.94/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.95/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@3.0.95/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.95/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-3.0.94/README.rst` & `ccxt-3.0.95/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/__init__.py` & `ccxt-3.0.95/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '3.0.94'
+__version__ = '3.0.95'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-3.0.94/ccxt/abstract/ace.py` & `ccxt-3.0.95/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/alpaca.py` & `ccxt-3.0.95/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/ascendex.py` & `ccxt-3.0.95/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bequant.py` & `ccxt-3.0.95/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bigone.py` & `ccxt-3.0.95/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/binance.py` & `ccxt-3.0.95/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/binancecoinm.py` & `ccxt-3.0.95/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/binanceus.py` & `ccxt-3.0.95/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/binanceusdm.py` & `ccxt-3.0.95/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bit2c.py` & `ccxt-3.0.95/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitbank.py` & `ccxt-3.0.95/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitbay.py` & `ccxt-3.0.95/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitbns.py` & `ccxt-3.0.95/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitcoincom.py` & `ccxt-3.0.95/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitfinex.py` & `ccxt-3.0.95/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitfinex2.py` & `ccxt-3.0.95/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitflyer.py` & `ccxt-3.0.95/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitforex.py` & `ccxt-3.0.95/ccxt/abstract/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitget.py` & `ccxt-3.0.95/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bithumb.py` & `ccxt-3.0.95/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitmart.py` & `ccxt-3.0.95/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitmex.py` & `ccxt-3.0.95/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitopro.py` & `ccxt-3.0.95/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitpanda.py` & `ccxt-3.0.95/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitrue.py` & `ccxt-3.0.95/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitso.py` & `ccxt-3.0.95/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitstamp.py` & `ccxt-3.0.95/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitstamp1.py` & `ccxt-3.0.95/ccxt/abstract/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bittrex.py` & `ccxt-3.0.95/ccxt/abstract/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bitvavo.py` & `ccxt-3.0.95/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bkex.py` & `ccxt-3.0.95/ccxt/abstract/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bl3p.py` & `ccxt-3.0.95/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/blockchaincom.py` & `ccxt-3.0.95/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/btcalpha.py` & `ccxt-3.0.95/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/btcbox.py` & `ccxt-3.0.95/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/btcex.py` & `ccxt-3.0.95/ccxt/abstract/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/btcmarkets.py` & `ccxt-3.0.95/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/btctradeua.py` & `ccxt-3.0.95/ccxt/abstract/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/btcturk.py` & `ccxt-3.0.95/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/bybit.py` & `ccxt-3.0.95/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/cex.py` & `ccxt-3.0.95/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinbase.py` & `ccxt-3.0.95/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinbaseprime.py` & `ccxt-3.0.95/ccxt/abstract/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinbasepro.py` & `ccxt-3.0.95/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coincheck.py` & `ccxt-3.0.95/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinex.py` & `ccxt-3.0.95/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinfalcon.py` & `ccxt-3.0.95/ccxt/abstract/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinmate.py` & `ccxt-3.0.95/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinone.py` & `ccxt-3.0.95/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinsph.py` & `ccxt-3.0.95/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/coinspot.py` & `ccxt-3.0.95/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/cryptocom.py` & `ccxt-3.0.95/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/currencycom.py` & `ccxt-3.0.95/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/delta.py` & `ccxt-3.0.95/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/deribit.py` & `ccxt-3.0.95/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/digifinex.py` & `ccxt-3.0.95/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/exmo.py` & `ccxt-3.0.95/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/fmfwio.py` & `ccxt-3.0.95/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/gate.py` & `ccxt-3.0.95/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/gateio.py` & `ccxt-3.0.95/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/gemini.py` & `ccxt-3.0.95/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/hitbtc.py` & `ccxt-3.0.95/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/hitbtc3.py` & `ccxt-3.0.95/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/hollaex.py` & `ccxt-3.0.95/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/huobi.py` & `ccxt-3.0.95/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/huobijp.py` & `ccxt-3.0.95/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/huobipro.py` & `ccxt-3.0.95/ccxt/abstract/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/idex.py` & `ccxt-3.0.95/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/independentreserve.py` & `ccxt-3.0.95/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/indodax.py` & `ccxt-3.0.95/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/kraken.py` & `ccxt-3.0.95/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/krakenfutures.py` & `ccxt-3.0.95/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/kucoin.py` & `ccxt-3.0.95/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/kucoinfutures.py` & `ccxt-3.0.95/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/kuna.py` & `ccxt-3.0.95/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/latoken.py` & `ccxt-3.0.95/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/lbank.py` & `ccxt-3.0.95/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/lbank2.py` & `ccxt-3.0.95/ccxt/abstract/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/luno.py` & `ccxt-3.0.95/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/lykke.py` & `ccxt-3.0.95/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/mercado.py` & `ccxt-3.0.95/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/mexc.py` & `ccxt-3.0.95/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/mexc3.py` & `ccxt-3.0.95/ccxt/abstract/mexc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/ndax.py` & `ccxt-3.0.95/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/novadax.py` & `ccxt-3.0.95/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/oceanex.py` & `ccxt-3.0.95/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/okcoin.py` & `ccxt-3.0.95/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/okex.py` & `ccxt-3.0.95/ccxt/abstract/okex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/okex5.py` & `ccxt-3.0.95/ccxt/abstract/okex5.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/okx.py` & `ccxt-3.0.95/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/paymium.py` & `ccxt-3.0.95/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/phemex.py` & `ccxt-3.0.95/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/poloniex.py` & `ccxt-3.0.95/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/poloniexfutures.py` & `ccxt-3.0.95/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/probit.py` & `ccxt-3.0.95/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/stex.py` & `ccxt-3.0.95/ccxt/abstract/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/tidex.py` & `ccxt-3.0.95/ccxt/abstract/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/timex.py` & `ccxt-3.0.95/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/tokocrypto.py` & `ccxt-3.0.95/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/upbit.py` & `ccxt-3.0.95/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/wavesexchange.py` & `ccxt-3.0.95/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/wazirx.py` & `ccxt-3.0.95/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/whitebit.py` & `ccxt-3.0.95/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/woo.py` & `ccxt-3.0.95/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/xt.py` & `ccxt-3.0.95/ccxt/abstract/xt.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/yobit.py` & `ccxt-3.0.95/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/zaif.py` & `ccxt-3.0.95/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/abstract/zonda.py` & `ccxt-3.0.95/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/ace.py` & `ccxt-3.0.95/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/alpaca.py` & `ccxt-3.0.95/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/ascendex.py` & `ccxt-3.0.95/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/__init__.py` & `ccxt-3.0.95/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.0.94'
+__version__ = '3.0.95'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-3.0.94/ccxt/async_support/ace.py` & `ccxt-3.0.95/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/alpaca.py` & `ccxt-3.0.95/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/ascendex.py` & `ccxt-3.0.95/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/exchange.py` & `ccxt-3.0.95/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.0.94'
+__version__ = '3.0.95'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-3.0.94/ccxt/async_support/base/throttler.py` & `ccxt-3.0.95/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/__init__.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/cache.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/client.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/fast_client.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/functions.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/order_book.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-3.0.95/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bequant.py` & `ccxt-3.0.95/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bigone.py` & `ccxt-3.0.95/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/binance.py` & `ccxt-3.0.95/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/binancecoinm.py` & `ccxt-3.0.95/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/binanceus.py` & `ccxt-3.0.95/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/binanceusdm.py` & `ccxt-3.0.95/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bit2c.py` & `ccxt-3.0.95/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitbank.py` & `ccxt-3.0.95/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitbns.py` & `ccxt-3.0.95/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitfinex.py` & `ccxt-3.0.95/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitfinex2.py` & `ccxt-3.0.95/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitflyer.py` & `ccxt-3.0.95/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitforex.py` & `ccxt-3.0.95/ccxt/async_support/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitget.py` & `ccxt-3.0.95/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bithumb.py` & `ccxt-3.0.95/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitmart.py` & `ccxt-3.0.95/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitmex.py` & `ccxt-3.0.95/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitopro.py` & `ccxt-3.0.95/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitpanda.py` & `ccxt-3.0.95/ccxt/async_support/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitrue.py` & `ccxt-3.0.95/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitso.py` & `ccxt-3.0.95/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitstamp.py` & `ccxt-3.0.95/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitstamp1.py` & `ccxt-3.0.95/ccxt/async_support/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bittrex.py` & `ccxt-3.0.95/ccxt/async_support/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bitvavo.py` & `ccxt-3.0.95/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bkex.py` & `ccxt-3.0.95/ccxt/async_support/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bl3p.py` & `ccxt-3.0.95/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/blockchaincom.py` & `ccxt-3.0.95/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/btcalpha.py` & `ccxt-3.0.95/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/btcbox.py` & `ccxt-3.0.95/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/btcex.py` & `ccxt-3.0.95/ccxt/async_support/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/btcmarkets.py` & `ccxt-3.0.95/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/btctradeua.py` & `ccxt-3.0.95/ccxt/async_support/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/btcturk.py` & `ccxt-3.0.95/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/buda.py` & `ccxt-3.0.95/ccxt/async_support/buda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/bybit.py` & `ccxt-3.0.95/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/cex.py` & `ccxt-3.0.95/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinbase.py` & `ccxt-3.0.95/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinbaseprime.py` & `ccxt-3.0.95/ccxt/async_support/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinbasepro.py` & `ccxt-3.0.95/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coincheck.py` & `ccxt-3.0.95/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinex.py` & `ccxt-3.0.95/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinfalcon.py` & `ccxt-3.0.95/ccxt/async_support/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinmate.py` & `ccxt-3.0.95/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinone.py` & `ccxt-3.0.95/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinsph.py` & `ccxt-3.0.95/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/coinspot.py` & `ccxt-3.0.95/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/cryptocom.py` & `ccxt-3.0.95/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/currencycom.py` & `ccxt-3.0.95/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/delta.py` & `ccxt-3.0.95/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/deribit.py` & `ccxt-3.0.95/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/digifinex.py` & `ccxt-3.0.95/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/exmo.py` & `ccxt-3.0.95/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/flowbtc.py` & `ccxt-3.0.95/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/fmfwio.py` & `ccxt-3.0.95/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/gate.py` & `ccxt-3.0.95/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/gemini.py` & `ccxt-3.0.95/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/hitbtc.py` & `ccxt-3.0.95/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/hitbtc3.py` & `ccxt-3.0.95/ccxt/async_support/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/hollaex.py` & `ccxt-3.0.95/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/huobi.py` & `ccxt-3.0.95/ccxt/async_support/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/huobijp.py` & `ccxt-3.0.95/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/huobipro.py` & `ccxt-3.0.95/ccxt/async_support/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/idex.py` & `ccxt-3.0.95/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/independentreserve.py` & `ccxt-3.0.95/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/indodax.py` & `ccxt-3.0.95/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/itbit.py` & `ccxt-3.0.95/ccxt/async_support/itbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/kraken.py` & `ccxt-3.0.95/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/krakenfutures.py` & `ccxt-3.0.95/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/kucoin.py` & `ccxt-3.0.95/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/kucoinfutures.py` & `ccxt-3.0.95/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/kuna.py` & `ccxt-3.0.95/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/latoken.py` & `ccxt-3.0.95/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/lbank.py` & `ccxt-3.0.95/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/lbank2.py` & `ccxt-3.0.95/ccxt/async_support/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/luno.py` & `ccxt-3.0.95/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/lykke.py` & `ccxt-3.0.95/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/mercado.py` & `ccxt-3.0.95/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/mexc.py` & `ccxt-3.0.95/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/ndax.py` & `ccxt-3.0.95/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/novadax.py` & `ccxt-3.0.95/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/oceanex.py` & `ccxt-3.0.95/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/okcoin.py` & `ccxt-3.0.95/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/okx.py` & `ccxt-3.0.95/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/paymium.py` & `ccxt-3.0.95/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/phemex.py` & `ccxt-3.0.95/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/poloniex.py` & `ccxt-3.0.95/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/poloniexfutures.py` & `ccxt-3.0.95/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/probit.py` & `ccxt-3.0.95/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/ripio.py` & `ccxt-3.0.95/ccxt/async_support/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/stex.py` & `ccxt-3.0.95/ccxt/async_support/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/tidex.py` & `ccxt-3.0.95/ccxt/async_support/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/timex.py` & `ccxt-3.0.95/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/tokocrypto.py` & `ccxt-3.0.95/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/upbit.py` & `ccxt-3.0.95/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/wavesexchange.py` & `ccxt-3.0.95/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/wazirx.py` & `ccxt-3.0.95/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/whitebit.py` & `ccxt-3.0.95/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/woo.py` & `ccxt-3.0.95/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/xt.py` & `ccxt-3.0.95/ccxt/async_support/xt.py`

 * *Files 0% similar despite different names*

```diff
@@ -2110,19 +2110,19 @@
         subType = None
         response = None
         type, params = self.handle_market_type_and_params('fetchOrder', market, params)
         subType, params = self.handle_sub_type_and_params('fetchOrder', market, params)
         stop = self.safe_value(params, 'stop')
         stopLossTakeProfit = self.safe_value(params, 'stopLossTakeProfit')
         if stop:
-            request['entrustId'] = self.convert_to_big_int(id)
+            request['entrustId'] = id
         elif stopLossTakeProfit:
-            request['profitId'] = self.convert_to_big_int(id)
+            request['profitId'] = id
         else:
-            request['orderId'] = self.convert_to_big_int(id)
+            request['orderId'] = id
         if stop:
             params = self.omit(params, 'stop')
             if subType == 'inverse':
                 response = await self.privateInverseGetFutureTradeV1EntrustPlanDetail(self.extend(request, params))
             else:
                 response = await self.privateLinearGetFutureTradeV1EntrustPlanDetail(self.extend(request, params))
         elif stopLossTakeProfit:
@@ -2739,19 +2739,19 @@
         subType = None
         response = None
         type, params = self.handle_market_type_and_params('cancelOrder', market, params)
         subType, params = self.handle_sub_type_and_params('cancelOrder', market, params)
         stop = self.safe_value(params, 'stop')
         stopLossTakeProfit = self.safe_value(params, 'stopLossTakeProfit')
         if stop:
-            request['entrustId'] = self.convert_to_big_int(id)
+            request['entrustId'] = id
         elif stopLossTakeProfit:
-            request['profitId'] = self.convert_to_big_int(id)
+            request['profitId'] = id
         else:
-            request['orderId'] = self.convert_to_big_int(id)
+            request['orderId'] = id
         if stop:
             params = self.omit(params, 'stop')
             if subType == 'inverse':
                 response = await self.privateInversePostFutureTradeV1EntrustCancelPlan(self.extend(request, params))
             else:
                 response = await self.privateLinearPostFutureTradeV1EntrustCancelPlan(self.extend(request, params))
         elif stopLossTakeProfit:
@@ -4178,27 +4178,27 @@
             body = params
             if (payload == '/v4/order') or (payload == '/future/trade/v1/order/create') or (payload == '/future/trade/v1/entrust/create-plan') or (payload == '/future/trade/v1/entrust/create-profit') or (payload == '/future/trade/v1/order/create-batch'):
                 body['clientMedia'] = 'CCXT'
             isUndefinedBody = ((method == 'GET') or (path == 'order/{orderId}'))
             body = None if isUndefinedBody else self.json(body)
             payloadString = None
             if endpoint == 'spot':
-                payloadString = 'xt-validate-algorithms=HmacSHA256&xt-validate-appkey=' + self.apiKey + '&xt-validate-recvwindow=' + recvWindow + '&xt-validate-timestamp=' + timestamp
+                payloadString = 'xt-validate-algorithms=HmacSHA256&xt-validate-appkey=' + self.apiKey + '&xt-validate-recvwindow=' + recvWindow + '&xt-validate-t' + 'imestamp=' + timestamp
                 if isUndefinedBody:
                     if urlencoded:
                         url += '?' + urlencoded
                         payloadString += '#' + method + '#' + payload + '#' + urlencoded
                     else:
                         payloadString += '#' + method + '#' + payload
                 else:
                     payloadString += '#' + method + '#' + payload + '#' + body
                 headers['xt-validate-algorithms'] = 'HmacSHA256'
                 headers['xt-validate-recvwindow'] = recvWindow
             else:
-                payloadString = 'xt-validate-appkey=' + self.apiKey + '&xt-validate-timestamp=' + timestamp
+                payloadString = 'xt-validate-appkey=' + self.apiKey + '&xt-validate-t' + 'imestamp=' + timestamp  # we can't glue timestamp, breaks in php
                 if method == 'GET':
                     if urlencoded:
                         url += '?' + urlencoded
                         payloadString += '#' + payload + '#' + urlencoded
                     else:
                         payloadString += '#' + payload
                 else:
```

### Comparing `ccxt-3.0.94/ccxt/async_support/yobit.py` & `ccxt-3.0.95/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/zaif.py` & `ccxt-3.0.95/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/zb.py` & `ccxt-3.0.95/ccxt/async_support/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/async_support/zonda.py` & `ccxt-3.0.95/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/base/__init__.py` & `ccxt-3.0.95/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/base/decimal_to_precision.py` & `ccxt-3.0.95/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/base/errors.py` & `ccxt-3.0.95/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/base/exchange.py` & `ccxt-3.0.95/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.0.94'
+__version__ = '3.0.95'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
```

### Comparing `ccxt-3.0.94/ccxt/base/precise.py` & `ccxt-3.0.95/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/base/types.py` & `ccxt-3.0.95/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bequant.py` & `ccxt-3.0.95/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bigone.py` & `ccxt-3.0.95/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/binance.py` & `ccxt-3.0.95/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/binancecoinm.py` & `ccxt-3.0.95/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/binanceus.py` & `ccxt-3.0.95/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/binanceusdm.py` & `ccxt-3.0.95/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bit2c.py` & `ccxt-3.0.95/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitbank.py` & `ccxt-3.0.95/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitbns.py` & `ccxt-3.0.95/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitfinex.py` & `ccxt-3.0.95/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitfinex2.py` & `ccxt-3.0.95/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitflyer.py` & `ccxt-3.0.95/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitforex.py` & `ccxt-3.0.95/ccxt/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitget.py` & `ccxt-3.0.95/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bithumb.py` & `ccxt-3.0.95/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitmart.py` & `ccxt-3.0.95/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitmex.py` & `ccxt-3.0.95/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitopro.py` & `ccxt-3.0.95/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitpanda.py` & `ccxt-3.0.95/ccxt/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitrue.py` & `ccxt-3.0.95/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitso.py` & `ccxt-3.0.95/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitstamp.py` & `ccxt-3.0.95/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitstamp1.py` & `ccxt-3.0.95/ccxt/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bittrex.py` & `ccxt-3.0.95/ccxt/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bitvavo.py` & `ccxt-3.0.95/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bkex.py` & `ccxt-3.0.95/ccxt/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bl3p.py` & `ccxt-3.0.95/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/blockchaincom.py` & `ccxt-3.0.95/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/btcalpha.py` & `ccxt-3.0.95/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/btcbox.py` & `ccxt-3.0.95/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/btcex.py` & `ccxt-3.0.95/ccxt/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/btcmarkets.py` & `ccxt-3.0.95/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/btctradeua.py` & `ccxt-3.0.95/ccxt/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/btcturk.py` & `ccxt-3.0.95/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/buda.py` & `ccxt-3.0.95/ccxt/buda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/bybit.py` & `ccxt-3.0.95/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/cex.py` & `ccxt-3.0.95/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinbase.py` & `ccxt-3.0.95/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinbaseprime.py` & `ccxt-3.0.95/ccxt/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinbasepro.py` & `ccxt-3.0.95/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coincheck.py` & `ccxt-3.0.95/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinex.py` & `ccxt-3.0.95/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinfalcon.py` & `ccxt-3.0.95/ccxt/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinmate.py` & `ccxt-3.0.95/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinone.py` & `ccxt-3.0.95/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinsph.py` & `ccxt-3.0.95/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/coinspot.py` & `ccxt-3.0.95/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/cryptocom.py` & `ccxt-3.0.95/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/currencycom.py` & `ccxt-3.0.95/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/delta.py` & `ccxt-3.0.95/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/deribit.py` & `ccxt-3.0.95/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/digifinex.py` & `ccxt-3.0.95/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/exmo.py` & `ccxt-3.0.95/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/flowbtc.py` & `ccxt-3.0.95/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/fmfwio.py` & `ccxt-3.0.95/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/gate.py` & `ccxt-3.0.95/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/gemini.py` & `ccxt-3.0.95/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/hitbtc.py` & `ccxt-3.0.95/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/hitbtc3.py` & `ccxt-3.0.95/ccxt/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/hollaex.py` & `ccxt-3.0.95/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/huobi.py` & `ccxt-3.0.95/ccxt/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/huobijp.py` & `ccxt-3.0.95/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/huobipro.py` & `ccxt-3.0.95/ccxt/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/idex.py` & `ccxt-3.0.95/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/independentreserve.py` & `ccxt-3.0.95/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/indodax.py` & `ccxt-3.0.95/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/itbit.py` & `ccxt-3.0.95/ccxt/itbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/kraken.py` & `ccxt-3.0.95/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/krakenfutures.py` & `ccxt-3.0.95/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/kucoin.py` & `ccxt-3.0.95/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/kucoinfutures.py` & `ccxt-3.0.95/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/kuna.py` & `ccxt-3.0.95/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/latoken.py` & `ccxt-3.0.95/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/lbank.py` & `ccxt-3.0.95/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/lbank2.py` & `ccxt-3.0.95/ccxt/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/luno.py` & `ccxt-3.0.95/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/lykke.py` & `ccxt-3.0.95/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/mercado.py` & `ccxt-3.0.95/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/mexc.py` & `ccxt-3.0.95/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/ndax.py` & `ccxt-3.0.95/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/novadax.py` & `ccxt-3.0.95/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/oceanex.py` & `ccxt-3.0.95/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/okcoin.py` & `ccxt-3.0.95/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/okx.py` & `ccxt-3.0.95/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/paymium.py` & `ccxt-3.0.95/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/phemex.py` & `ccxt-3.0.95/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/poloniex.py` & `ccxt-3.0.95/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/poloniexfutures.py` & `ccxt-3.0.95/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/__init__.py` & `ccxt-3.0.95/ccxt/pro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '3.0.94'
+__version__ = '3.0.95'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-3.0.94/ccxt/pro/alpaca.py` & `ccxt-3.0.95/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/ascendex.py` & `ccxt-3.0.95/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bequant.py` & `ccxt-3.0.95/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/binance.py` & `ccxt-3.0.95/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/binancecoinm.py` & `ccxt-3.0.95/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/binanceus.py` & `ccxt-3.0.95/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/binanceusdm.py` & `ccxt-3.0.95/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitcoincom.py` & `ccxt-3.0.95/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitfinex.py` & `ccxt-3.0.95/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitfinex2.py` & `ccxt-3.0.95/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitget.py` & `ccxt-3.0.95/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitmart.py` & `ccxt-3.0.95/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitmex.py` & `ccxt-3.0.95/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitopro.py` & `ccxt-3.0.95/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitrue.py` & `ccxt-3.0.95/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitstamp.py` & `ccxt-3.0.95/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bittrex.py` & `ccxt-3.0.95/ccxt/pro/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bitvavo.py` & `ccxt-3.0.95/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/btcex.py` & `ccxt-3.0.95/ccxt/pro/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/bybit.py` & `ccxt-3.0.95/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/cex.py` & `ccxt-3.0.95/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/coinbaseprime.py` & `ccxt-3.0.95/ccxt/pro/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/coinbasepro.py` & `ccxt-3.0.95/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/coinex.py` & `ccxt-3.0.95/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/cryptocom.py` & `ccxt-3.0.95/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/currencycom.py` & `ccxt-3.0.95/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/deribit.py` & `ccxt-3.0.95/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/exmo.py` & `ccxt-3.0.95/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/gate.py` & `ccxt-3.0.95/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/gemini.py` & `ccxt-3.0.95/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/hitbtc.py` & `ccxt-3.0.95/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/hollaex.py` & `ccxt-3.0.95/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/huobi.py` & `ccxt-3.0.95/ccxt/pro/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/huobijp.py` & `ccxt-3.0.95/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/idex.py` & `ccxt-3.0.95/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/independentreserve.py` & `ccxt-3.0.95/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/kraken.py` & `ccxt-3.0.95/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/krakenfutures.py` & `ccxt-3.0.95/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/kucoin.py` & `ccxt-3.0.95/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/kucoinfutures.py` & `ccxt-3.0.95/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/luno.py` & `ccxt-3.0.95/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/mexc.py` & `ccxt-3.0.95/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/ndax.py` & `ccxt-3.0.95/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/okcoin.py` & `ccxt-3.0.95/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/okx.py` & `ccxt-3.0.95/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/phemex.py` & `ccxt-3.0.95/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/probit.py` & `ccxt-3.0.95/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/ripio.py` & `ccxt-3.0.95/ccxt/pro/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/upbit.py` & `ccxt-3.0.95/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/wazirx.py` & `ccxt-3.0.95/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/whitebit.py` & `ccxt-3.0.95/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/woo.py` & `ccxt-3.0.95/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/pro/zb.py` & `ccxt-3.0.95/ccxt/pro/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/probit.py` & `ccxt-3.0.95/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/ripio.py` & `ccxt-3.0.95/ccxt/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-3.0.95/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-3.0.95/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/stex.py` & `ccxt-3.0.95/ccxt/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/__init__.py` & `ccxt-3.0.95/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_account.py` & `ccxt-3.0.95/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_balance.py` & `ccxt-3.0.95/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_borrow_interest.py` & `ccxt-3.0.95/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_borrow_rate.py` & `ccxt-3.0.95/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_calculate_fee.py` & `ccxt-3.0.95/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_crypto.py` & `ccxt-3.0.95/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_currency.py` & `ccxt-3.0.95/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_datetime.py` & `ccxt-3.0.95/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-3.0.95/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_deep_extend.py` & `ccxt-3.0.95/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-3.0.95/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-3.0.95/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_funding_rate_history.py` & `ccxt-3.0.95/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_ledger_entry.py` & `ccxt-3.0.95/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_ledger_item.py` & `ccxt-3.0.95/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_leverage_tier.py` & `ccxt-3.0.95/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_margin_modification.py` & `ccxt-3.0.95/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_market.py` & `ccxt-3.0.95/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_number.py` & `ccxt-3.0.95/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_ohlcv.py` & `ccxt-3.0.95/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_open_interest.py` & `ccxt-3.0.95/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_order.py` & `ccxt-3.0.95/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_order_book.py` & `ccxt-3.0.95/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_position.py` & `ccxt-3.0.95/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_shared_methods.py` & `ccxt-3.0.95/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_status.py` & `ccxt-3.0.95/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_throttle.py` & `ccxt-3.0.95/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_ticker.py` & `ccxt-3.0.95/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_trade.py` & `ccxt-3.0.95/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_trading_fee.py` & `ccxt-3.0.95/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/base/test_transaction.py` & `ccxt-3.0.95/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/test_async.py` & `ccxt-3.0.95/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/test/test_sync.py` & `ccxt-3.0.95/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/tidex.py` & `ccxt-3.0.95/ccxt/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/timex.py` & `ccxt-3.0.95/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/tokocrypto.py` & `ccxt-3.0.95/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/upbit.py` & `ccxt-3.0.95/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/wavesexchange.py` & `ccxt-3.0.95/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/wazirx.py` & `ccxt-3.0.95/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/whitebit.py` & `ccxt-3.0.95/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/woo.py` & `ccxt-3.0.95/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/xt.py` & `ccxt-3.0.95/ccxt/xt.py`

 * *Files 0% similar despite different names*

```diff
@@ -2109,19 +2109,19 @@
         subType = None
         response = None
         type, params = self.handle_market_type_and_params('fetchOrder', market, params)
         subType, params = self.handle_sub_type_and_params('fetchOrder', market, params)
         stop = self.safe_value(params, 'stop')
         stopLossTakeProfit = self.safe_value(params, 'stopLossTakeProfit')
         if stop:
-            request['entrustId'] = self.convert_to_big_int(id)
+            request['entrustId'] = id
         elif stopLossTakeProfit:
-            request['profitId'] = self.convert_to_big_int(id)
+            request['profitId'] = id
         else:
-            request['orderId'] = self.convert_to_big_int(id)
+            request['orderId'] = id
         if stop:
             params = self.omit(params, 'stop')
             if subType == 'inverse':
                 response = self.privateInverseGetFutureTradeV1EntrustPlanDetail(self.extend(request, params))
             else:
                 response = self.privateLinearGetFutureTradeV1EntrustPlanDetail(self.extend(request, params))
         elif stopLossTakeProfit:
@@ -2738,19 +2738,19 @@
         subType = None
         response = None
         type, params = self.handle_market_type_and_params('cancelOrder', market, params)
         subType, params = self.handle_sub_type_and_params('cancelOrder', market, params)
         stop = self.safe_value(params, 'stop')
         stopLossTakeProfit = self.safe_value(params, 'stopLossTakeProfit')
         if stop:
-            request['entrustId'] = self.convert_to_big_int(id)
+            request['entrustId'] = id
         elif stopLossTakeProfit:
-            request['profitId'] = self.convert_to_big_int(id)
+            request['profitId'] = id
         else:
-            request['orderId'] = self.convert_to_big_int(id)
+            request['orderId'] = id
         if stop:
             params = self.omit(params, 'stop')
             if subType == 'inverse':
                 response = self.privateInversePostFutureTradeV1EntrustCancelPlan(self.extend(request, params))
             else:
                 response = self.privateLinearPostFutureTradeV1EntrustCancelPlan(self.extend(request, params))
         elif stopLossTakeProfit:
@@ -4177,27 +4177,27 @@
             body = params
             if (payload == '/v4/order') or (payload == '/future/trade/v1/order/create') or (payload == '/future/trade/v1/entrust/create-plan') or (payload == '/future/trade/v1/entrust/create-profit') or (payload == '/future/trade/v1/order/create-batch'):
                 body['clientMedia'] = 'CCXT'
             isUndefinedBody = ((method == 'GET') or (path == 'order/{orderId}'))
             body = None if isUndefinedBody else self.json(body)
             payloadString = None
             if endpoint == 'spot':
-                payloadString = 'xt-validate-algorithms=HmacSHA256&xt-validate-appkey=' + self.apiKey + '&xt-validate-recvwindow=' + recvWindow + '&xt-validate-timestamp=' + timestamp
+                payloadString = 'xt-validate-algorithms=HmacSHA256&xt-validate-appkey=' + self.apiKey + '&xt-validate-recvwindow=' + recvWindow + '&xt-validate-t' + 'imestamp=' + timestamp
                 if isUndefinedBody:
                     if urlencoded:
                         url += '?' + urlencoded
                         payloadString += '#' + method + '#' + payload + '#' + urlencoded
                     else:
                         payloadString += '#' + method + '#' + payload
                 else:
                     payloadString += '#' + method + '#' + payload + '#' + body
                 headers['xt-validate-algorithms'] = 'HmacSHA256'
                 headers['xt-validate-recvwindow'] = recvWindow
             else:
-                payloadString = 'xt-validate-appkey=' + self.apiKey + '&xt-validate-timestamp=' + timestamp
+                payloadString = 'xt-validate-appkey=' + self.apiKey + '&xt-validate-t' + 'imestamp=' + timestamp  # we can't glue timestamp, breaks in php
                 if method == 'GET':
                     if urlencoded:
                         url += '?' + urlencoded
                         payloadString += '#' + payload + '#' + urlencoded
                     else:
                         payloadString += '#' + payload
                 else:
```

### Comparing `ccxt-3.0.94/ccxt/yobit.py` & `ccxt-3.0.95/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/zaif.py` & `ccxt-3.0.95/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/zb.py` & `ccxt-3.0.95/ccxt/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt/zonda.py` & `ccxt-3.0.95/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/ccxt.egg-info/PKG-INFO` & `ccxt-3.0.95/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 3.0.94
+Version: 3.0.95
 Summary: A JavaScript / Python / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -227,21 +227,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@3.0.94/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.95/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@3.0.95/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.95/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-3.0.94/ccxt.egg-info/SOURCES.txt` & `ccxt-3.0.95/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.94/package.json` & `ccxt-3.0.95/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'3.0.95'"}*

```diff
@@ -217,9 +217,9 @@
         "update-badges": "node build/update-badges",
         "update-links": "node build/update-links",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "3.0.94"
+    "version": "3.0.95"
 }
```

### Comparing `ccxt-3.0.94/setup.py` & `ccxt-3.0.95/setup.py`

 * *Files identical despite different names*

