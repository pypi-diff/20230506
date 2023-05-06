# Comparing `tmp/bavest-1.0.0.tar.gz` & `tmp/bavest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bavest-1.0.0.tar", max compression
+gzip compressed data, was "bavest-1.0.1.tar", max compression
```

## Comparing `bavest-1.0.0.tar` & `bavest-1.0.1.tar`

### file list

```diff
@@ -1,95 +1,96 @@
--rw-r--r--   0        0        0     1990 2023-03-10 13:44:18.599466 bavest-1.0.0/README.md
--rw-r--r--   0        0        0       43 2023-03-10 12:31:10.112932 bavest-1.0.0/bavest/__init__.py
--rw-r--r--   0        0        0      225 2023-03-08 07:04:13.724210 bavest-1.0.0/bavest/api.py
--rw-r--r--   0        0        0     1538 2023-03-10 12:30:06.906035 bavest-1.0.0/bavest/errors.py
--rw-r--r--   0        0        0        1 2023-03-10 12:24:33.406285 bavest-1.0.0/bavest/finance/__init__.py
--rw-r--r--   0        0        0       29 2023-03-10 12:24:33.406372 bavest-1.0.0/bavest/finance/client/__init__.py
--rw-r--r--   0        0        0    30628 2023-03-10 12:24:33.406570 bavest-1.0.0/bavest/finance/client/bavest_client.py
--rw-r--r--   0        0        0     2147 2023-03-10 12:27:50.932882 bavest-1.0.0/bavest/finance/client/urls.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.725302 bavest-1.0.0/bavest/finance/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.725525 bavest-1.0.0/bavest/finance/models/v0/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.725766 bavest-1.0.0/bavest/finance/models/v0/candle/__init__.py
--rw-r--r--   0        0        0      496 2023-03-10 12:24:33.406706 bavest-1.0.0/bavest/finance/models/v0/candle/candle.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.725963 bavest-1.0.0/bavest/finance/models/v0/etf/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.726060 bavest-1.0.0/bavest/finance/models/v0/etf/country/__init__.py
--rw-r--r--   0        0        0      423 2023-03-10 12:24:33.406827 bavest-1.0.0/bavest/finance/models/v0/etf/country/country.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.726270 bavest-1.0.0/bavest/finance/models/v0/etf/holding/__init__.py
--rw-r--r--   0        0        0      493 2023-03-10 12:27:50.957336 bavest-1.0.0/bavest/finance/models/v0/etf/holding/holding.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.726487 bavest-1.0.0/bavest/finance/models/v0/etf/profile/__init__.py
--rw-r--r--   0        0        0      648 2023-03-10 12:24:33.407030 bavest-1.0.0/bavest/finance/models/v0/etf/profile/profile.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.726686 bavest-1.0.0/bavest/finance/models/v0/etf/sector/__init__.py
--rw-r--r--   0        0        0      425 2023-03-10 12:27:50.949013 bavest-1.0.0/bavest/finance/models/v0/etf/sector/sector.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.726890 bavest-1.0.0/bavest/finance/models/v0/forex/__init__.py
--rw-r--r--   0        0        0      539 2023-03-10 12:24:33.407239 bavest-1.0.0/bavest/finance/models/v0/forex/forex.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.727091 bavest-1.0.0/bavest/finance/models/v0/market/__init__.py
--rw-r--r--   0        0        0      513 2023-03-10 12:24:33.407354 bavest-1.0.0/bavest/finance/models/v0/market/news.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.727594 bavest-1.0.0/bavest/finance/models/v0/portfolio/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.727715 bavest-1.0.0/bavest/finance/models/v0/portfolio/allocation/__init__.py
--rw-r--r--   0        0        0      442 2023-03-10 12:27:50.942153 bavest-1.0.0/bavest/finance/models/v0/portfolio/allocation/allocation.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.727932 bavest-1.0.0/bavest/finance/models/v0/portfolio/chart/__init__.py
--rw-r--r--   0        0        0      534 2023-03-10 12:24:33.407576 bavest-1.0.0/bavest/finance/models/v0/portfolio/chart/chart.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.728135 bavest-1.0.0/bavest/finance/models/v0/portfolio/metric/__init__.py
--rw-r--r--   0        0        0      644 2023-03-10 12:24:33.407684 bavest-1.0.0/bavest/finance/models/v0/portfolio/metric/metric.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.728332 bavest-1.0.0/bavest/finance/models/v0/portfolio/price/__init__.py
--rw-r--r--   0        0        0      368 2023-03-10 12:24:33.407788 bavest-1.0.0/bavest/finance/models/v0/portfolio/price/price.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.728517 bavest-1.0.0/bavest/finance/models/v0/portfolio/region/__init__.py
--rw-r--r--   0        0        0      422 2023-03-10 12:24:33.407888 bavest-1.0.0/bavest/finance/models/v0/portfolio/region/region.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.728714 bavest-1.0.0/bavest/finance/models/v0/portfolio/sector/__init__.py
--rw-r--r--   0        0        0      419 2023-03-10 12:24:33.407987 bavest-1.0.0/bavest/finance/models/v0/portfolio/sector/sector.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.728872 bavest-1.0.0/bavest/finance/models/v0/portfolio/stats/__init__.py
--rw-r--r--   0        0        0     2145 2023-03-10 12:24:33.408155 bavest-1.0.0/bavest/finance/models/v0/portfolio/stats/stats.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.729174 bavest-1.0.0/bavest/finance/models/v0/quote/__init__.py
--rw-r--r--   0        0        0      867 2023-03-10 12:24:33.408262 bavest-1.0.0/bavest/finance/models/v0/quote/quote.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.729560 bavest-1.0.0/bavest/finance/models/v0/screener/__init__.py
--rw-r--r--   0        0        0      441 2023-03-10 12:24:33.408393 bavest-1.0.0/bavest/finance/models/v0/screener/screener.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.729797 bavest-1.0.0/bavest/finance/models/v0/search/__init__.py
--rw-r--r--   0        0        0      583 2023-03-10 12:24:33.408498 bavest-1.0.0/bavest/finance/models/v0/search/search.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.729969 bavest-1.0.0/bavest/finance/models/v0/sentiment/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.730055 bavest-1.0.0/bavest/finance/models/v0/sentiment/sentiment/__init__.py
--rw-r--r--   0        0        0      381 2023-03-10 12:27:50.945741 bavest-1.0.0/bavest/finance/models/v0/sentiment/sentiment/sentiment.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.730232 bavest-1.0.0/bavest/finance/models/v0/sentiment/social_sentiment/__init__.py
--rw-r--r--   0        0        0      528 2023-03-10 12:27:50.952174 bavest-1.0.0/bavest/finance/models/v0/sentiment/social_sentiment/social_sentiment.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.730403 bavest-1.0.0/bavest/finance/models/v0/status/__init__.py
--rw-r--r--   0        0        0      280 2023-03-10 12:24:33.408824 bavest-1.0.0/bavest/finance/models/v0/status/status.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.730553 bavest-1.0.0/bavest/finance/models/v0/stock/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.730646 bavest-1.0.0/bavest/finance/models/v0/stock/analyst_estimates/__init__.py
--rw-r--r--   0        0        0      856 2023-03-10 12:27:50.954478 bavest-1.0.0/bavest/finance/models/v0/stock/analyst_estimates/analyst_estimates.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.730911 bavest-1.0.0/bavest/finance/models/v0/stock/calendar/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.731001 bavest-1.0.0/bavest/finance/models/v0/stock/calendar/earnings/__init__.py
--rw-r--r--   0        0        0      534 2023-03-10 12:24:33.409249 bavest-1.0.0/bavest/finance/models/v0/stock/calendar/earnings/earnings.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.731176 bavest-1.0.0/bavest/finance/models/v0/stock/calendar/economics/__init__.py
--rw-r--r--   0        0        0      557 2023-03-10 12:27:50.960077 bavest-1.0.0/bavest/finance/models/v0/stock/calendar/economics/economics.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.731351 bavest-1.0.0/bavest/finance/models/v0/stock/calendar/ipo/__init__.py
--rw-r--r--   0        0        0      509 2023-03-10 12:24:33.409509 bavest-1.0.0/bavest/finance/models/v0/stock/calendar/ipo/ipo.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.731564 bavest-1.0.0/bavest/finance/models/v0/stock/candle/__init__.py
--rw-r--r--   0        0        0      483 2023-03-10 12:27:50.939448 bavest-1.0.0/bavest/finance/models/v0/stock/candle/candle.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.731783 bavest-1.0.0/bavest/finance/models/v0/stock/dividend/__init__.py
--rw-r--r--   0        0        0      468 2023-03-10 12:27:50.917762 bavest-1.0.0/bavest/finance/models/v0/stock/dividend/dividend.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.731993 bavest-1.0.0/bavest/finance/models/v0/stock/earnings_transcript/__init__.py
--rw-r--r--   0        0        0      432 2023-03-10 12:24:33.409824 bavest-1.0.0/bavest/finance/models/v0/stock/earnings_transcript/earnings_transcript.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.732461 bavest-1.0.0/bavest/finance/models/v0/stock/esg/__init__.py
--rw-r--r--   0        0        0     1474 2023-03-10 12:24:33.409982 bavest-1.0.0/bavest/finance/models/v0/stock/esg/esg.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.732766 bavest-1.0.0/bavest/finance/models/v0/stock/financials/__init__.py
--rw-r--r--   0        0        0     1515 2023-03-10 12:24:33.410098 bavest-1.0.0/bavest/finance/models/v0/stock/financials/financials.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.732974 bavest-1.0.0/bavest/finance/models/v0/stock/fundamentals/__init__.py
--rw-r--r--   0        0        0     1453 2023-03-10 12:24:33.410216 bavest-1.0.0/bavest/finance/models/v0/stock/fundamentals/fundamentals.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.733176 bavest-1.0.0/bavest/finance/models/v0/stock/ipo/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.733290 bavest-1.0.0/bavest/finance/models/v0/stock/ipo/prospectus/__init__.py
--rw-r--r--   0        0        0      708 2023-03-10 12:24:33.410333 bavest-1.0.0/bavest/finance/models/v0/stock/ipo/prospectus/prospectus.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.733507 bavest-1.0.0/bavest/finance/models/v0/stock/metric/__init__.py
--rw-r--r--   0        0        0     4031 2023-03-10 12:24:33.410445 bavest-1.0.0/bavest/finance/models/v0/stock/metric/metric.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.733684 bavest-1.0.0/bavest/finance/models/v0/stock/news/__init__.py
--rw-r--r--   0        0        0      435 2023-03-10 12:24:33.410554 bavest-1.0.0/bavest/finance/models/v0/stock/news/news.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.733849 bavest-1.0.0/bavest/finance/models/v0/stock/peers/__init__.py
--rw-r--r--   0        0        0      294 2023-03-10 12:24:33.410659 bavest-1.0.0/bavest/finance/models/v0/stock/peers/peers.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.734227 bavest-1.0.0/bavest/finance/models/v0/stock/profile/__init__.py
--rw-r--r--   0        0        0      851 2023-03-10 12:24:33.410771 bavest-1.0.0/bavest/finance/models/v0/stock/profile/profile.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.734424 bavest-1.0.0/bavest/finance/models/v0/stock/split/__init__.py
--rw-r--r--   0        0        0      416 2023-03-10 12:24:33.410879 bavest-1.0.0/bavest/finance/models/v0/stock/split/split.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.734589 bavest-1.0.0/bavest/finance/models/v0/widget/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.734672 bavest-1.0.0/bavest/finance/models/v0/widget/stock/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 07:04:13.734755 bavest-1.0.0/bavest/finance/models/v0/widget/stock/peers/__init__.py
--rw-r--r--   0        0        0      444 2023-03-10 12:24:33.410990 bavest-1.0.0/bavest/finance/models/v0/widget/stock/peers/peers.py
--rw-r--r--   0        0        0      377 2023-03-10 12:37:06.084603 bavest-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4632 1970-01-01 00:00:00.000000 bavest-1.0.0/setup.py
--rw-r--r--   0        0        0     2452 1970-01-01 00:00:00.000000 bavest-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-06 08:52:51.785265 bavest-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     3056 2023-05-06 09:04:28.174020 bavest-1.0.1/README.md
+-rw-r--r--   0        0        0       43 2023-05-06 08:52:51.785474 bavest-1.0.1/bavest/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-06 08:52:51.785556 bavest-1.0.1/bavest/api.py
+-rw-r--r--   0        0        0     1538 2023-05-06 08:52:51.785638 bavest-1.0.1/bavest/errors.py
+-rw-r--r--   0        0        0        1 2023-05-06 08:52:51.785753 bavest-1.0.1/bavest/finance/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-06 08:52:51.785866 bavest-1.0.1/bavest/finance/client/__init__.py
+-rw-r--r--   0        0        0    30629 2023-05-06 08:54:01.842957 bavest-1.0.1/bavest/finance/client/bavest_client.py
+-rw-r--r--   0        0        0     2149 2023-05-06 08:52:51.786112 bavest-1.0.1/bavest/finance/client/urls.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.786198 bavest-1.0.1/bavest/finance/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.786312 bavest-1.0.1/bavest/finance/models/v0/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.786423 bavest-1.0.1/bavest/finance/models/v0/candle/__init__.py
+-rw-r--r--   0        0        0      496 2023-05-06 08:52:51.786529 bavest-1.0.1/bavest/finance/models/v0/candle/candle.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.786615 bavest-1.0.1/bavest/finance/models/v0/etf/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.786728 bavest-1.0.1/bavest/finance/models/v0/etf/country/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-06 08:52:51.786834 bavest-1.0.1/bavest/finance/models/v0/etf/country/country.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.786916 bavest-1.0.1/bavest/finance/models/v0/etf/holding/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-06 08:52:51.787024 bavest-1.0.1/bavest/finance/models/v0/etf/holding/holding.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.787109 bavest-1.0.1/bavest/finance/models/v0/etf/profile/__init__.py
+-rw-r--r--   0        0        0      648 2023-05-06 08:52:51.787216 bavest-1.0.1/bavest/finance/models/v0/etf/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.787309 bavest-1.0.1/bavest/finance/models/v0/etf/sector/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-06 08:52:51.787430 bavest-1.0.1/bavest/finance/models/v0/etf/sector/sector.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.787521 bavest-1.0.1/bavest/finance/models/v0/forex/__init__.py
+-rw-r--r--   0        0        0      539 2023-05-06 08:52:51.787626 bavest-1.0.1/bavest/finance/models/v0/forex/forex.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.787717 bavest-1.0.1/bavest/finance/models/v0/market/__init__.py
+-rw-r--r--   0        0        0      513 2023-05-06 08:52:51.787829 bavest-1.0.1/bavest/finance/models/v0/market/news.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.787921 bavest-1.0.1/bavest/finance/models/v0/portfolio/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.788037 bavest-1.0.1/bavest/finance/models/v0/portfolio/allocation/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-06 08:52:51.788147 bavest-1.0.1/bavest/finance/models/v0/portfolio/allocation/allocation.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.788231 bavest-1.0.1/bavest/finance/models/v0/portfolio/chart/__init__.py
+-rw-r--r--   0        0        0      534 2023-05-06 08:52:51.788353 bavest-1.0.1/bavest/finance/models/v0/portfolio/chart/chart.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.788444 bavest-1.0.1/bavest/finance/models/v0/portfolio/metric/__init__.py
+-rw-r--r--   0        0        0      644 2023-05-06 08:52:51.788576 bavest-1.0.1/bavest/finance/models/v0/portfolio/metric/metric.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.788661 bavest-1.0.1/bavest/finance/models/v0/portfolio/price/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-06 08:52:51.788784 bavest-1.0.1/bavest/finance/models/v0/portfolio/price/price.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.788878 bavest-1.0.1/bavest/finance/models/v0/portfolio/region/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-06 08:52:51.788983 bavest-1.0.1/bavest/finance/models/v0/portfolio/region/region.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.789080 bavest-1.0.1/bavest/finance/models/v0/portfolio/sector/__init__.py
+-rw-r--r--   0        0        0      419 2023-05-06 08:52:51.789183 bavest-1.0.1/bavest/finance/models/v0/portfolio/sector/sector.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.789272 bavest-1.0.1/bavest/finance/models/v0/portfolio/stats/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-06 08:52:51.789384 bavest-1.0.1/bavest/finance/models/v0/portfolio/stats/stats.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.789464 bavest-1.0.1/bavest/finance/models/v0/quote/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-06 08:52:51.789550 bavest-1.0.1/bavest/finance/models/v0/quote/quote.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.789622 bavest-1.0.1/bavest/finance/models/v0/screener/__init__.py
+-rw-r--r--   0        0        0      441 2023-05-06 08:52:51.789710 bavest-1.0.1/bavest/finance/models/v0/screener/screener.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.789783 bavest-1.0.1/bavest/finance/models/v0/search/__init__.py
+-rw-r--r--   0        0        0      583 2023-05-06 08:52:51.789878 bavest-1.0.1/bavest/finance/models/v0/search/search.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.789953 bavest-1.0.1/bavest/finance/models/v0/sentiment/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.790042 bavest-1.0.1/bavest/finance/models/v0/sentiment/sentiment/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-06 08:52:51.790134 bavest-1.0.1/bavest/finance/models/v0/sentiment/sentiment/sentiment.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.790210 bavest-1.0.1/bavest/finance/models/v0/sentiment/social_sentiment/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-06 08:52:51.790304 bavest-1.0.1/bavest/finance/models/v0/sentiment/social_sentiment/social_sentiment.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.790379 bavest-1.0.1/bavest/finance/models/v0/status/__init__.py
+-rw-r--r--   0        0        0      280 2023-05-06 08:52:51.790469 bavest-1.0.1/bavest/finance/models/v0/status/status.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.790538 bavest-1.0.1/bavest/finance/models/v0/stock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.790629 bavest-1.0.1/bavest/finance/models/v0/stock/analyst_estimates/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-06 08:52:51.790729 bavest-1.0.1/bavest/finance/models/v0/stock/analyst_estimates/analyst_estimates.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.790805 bavest-1.0.1/bavest/finance/models/v0/stock/calendar/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.790899 bavest-1.0.1/bavest/finance/models/v0/stock/calendar/earnings/__init__.py
+-rw-r--r--   0        0        0      534 2023-05-06 08:52:51.790991 bavest-1.0.1/bavest/finance/models/v0/stock/calendar/earnings/earnings.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.791070 bavest-1.0.1/bavest/finance/models/v0/stock/calendar/economics/__init__.py
+-rw-r--r--   0        0        0      558 2023-05-06 08:52:51.791161 bavest-1.0.1/bavest/finance/models/v0/stock/calendar/economics/economics.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.791247 bavest-1.0.1/bavest/finance/models/v0/stock/calendar/ipo/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-06 08:52:51.791341 bavest-1.0.1/bavest/finance/models/v0/stock/calendar/ipo/ipo.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.791419 bavest-1.0.1/bavest/finance/models/v0/stock/candle/__init__.py
+-rw-r--r--   0        0        0      484 2023-05-06 08:52:51.791532 bavest-1.0.1/bavest/finance/models/v0/stock/candle/candle.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.791609 bavest-1.0.1/bavest/finance/models/v0/stock/dividend/__init__.py
+-rw-r--r--   0        0        0      469 2023-05-06 08:52:51.791724 bavest-1.0.1/bavest/finance/models/v0/stock/dividend/dividend.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.791808 bavest-1.0.1/bavest/finance/models/v0/stock/earnings_transcript/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-06 08:52:51.791900 bavest-1.0.1/bavest/finance/models/v0/stock/earnings_transcript/earnings_transcript.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.791973 bavest-1.0.1/bavest/finance/models/v0/stock/esg/__init__.py
+-rw-r--r--   0        0        0     1474 2023-05-06 08:52:51.792077 bavest-1.0.1/bavest/finance/models/v0/stock/esg/esg.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.792165 bavest-1.0.1/bavest/finance/models/v0/stock/financials/__init__.py
+-rw-r--r--   0        0        0     1515 2023-05-06 08:52:51.792268 bavest-1.0.1/bavest/finance/models/v0/stock/financials/financials.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.792347 bavest-1.0.1/bavest/finance/models/v0/stock/fundamentals/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-06 08:52:51.792440 bavest-1.0.1/bavest/finance/models/v0/stock/fundamentals/fundamentals.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.792509 bavest-1.0.1/bavest/finance/models/v0/stock/ipo/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.792611 bavest-1.0.1/bavest/finance/models/v0/stock/ipo/prospectus/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-06 08:52:51.792704 bavest-1.0.1/bavest/finance/models/v0/stock/ipo/prospectus/prospectus.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.792775 bavest-1.0.1/bavest/finance/models/v0/stock/metric/__init__.py
+-rw-r--r--   0        0        0     4031 2023-05-06 08:52:51.792861 bavest-1.0.1/bavest/finance/models/v0/stock/metric/metric.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.792930 bavest-1.0.1/bavest/finance/models/v0/stock/news/__init__.py
+-rw-r--r--   0        0        0      435 2023-05-06 08:52:51.793013 bavest-1.0.1/bavest/finance/models/v0/stock/news/news.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.793098 bavest-1.0.1/bavest/finance/models/v0/stock/peers/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-06 08:52:51.793190 bavest-1.0.1/bavest/finance/models/v0/stock/peers/peers.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.793273 bavest-1.0.1/bavest/finance/models/v0/stock/profile/__init__.py
+-rw-r--r--   0        0        0      851 2023-05-06 08:52:51.793377 bavest-1.0.1/bavest/finance/models/v0/stock/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.793467 bavest-1.0.1/bavest/finance/models/v0/stock/split/__init__.py
+-rw-r--r--   0        0        0      416 2023-05-06 08:52:51.793570 bavest-1.0.1/bavest/finance/models/v0/stock/split/split.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.793653 bavest-1.0.1/bavest/finance/models/v0/widget/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.793744 bavest-1.0.1/bavest/finance/models/v0/widget/stock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 08:52:51.793835 bavest-1.0.1/bavest/finance/models/v0/widget/stock/peers/__init__.py
+-rw-r--r--   0        0        0      444 2023-05-06 08:52:51.793917 bavest-1.0.1/bavest/finance/models/v0/widget/stock/peers/peers.py
+-rw-r--r--   0        0        0      377 2023-05-06 08:54:01.875598 bavest-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5727 1970-01-01 00:00:00.000000 bavest-1.0.1/setup.py
+-rw-r--r--   0        0        0     3518 1970-01-01 00:00:00.000000 bavest-1.0.1/PKG-INFO
```

### Comparing `bavest-1.0.0/README.md` & `bavest-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 <p align="center">
-  <img wsymbolth="300" alt="posthoglogo" src="https://i.imgur.com/z4ZPmGN.png">
+  <img  src="https://www.bavest.co/images/api-home.png">
 </p>
 
-# Bavest Finance SDK
+# Bavest Python SDK
+
+<img wsymbolth=300 src="https://img.shields.io/badge/license-MIT-brightgreen" > <img wsymbolth=300 src="https://img.shields.io/badge/tests-passing-brightgreen" > <img src="https://img.shields.io/github/issues/Bavest/python-sdk"> <img src="https://img.shields.io/pypi/pyversions/bavest"> <img src="https://img.shields.io/pypi/wheel/bavest">
 
 **The Bavest Finance SDK is an open-source library to create finance products in weeks. Bavest offers:**
 
-* Financial api with 99.999% uptime
+* Financial api with 99.95% uptime
 * Easy to integrate and use
 * Free for open-source projects
 
-## Get started for free
-
-### Personal API key
+## Get API key
 
-First, you need to create an account on [Bavest](https://www.dashboard.bavest.com).
+First, you need to create a [Bavest](https://www.dashboard.bavest.com) account.
 After registration, you will find your api key in the dashboard.
 
-### Open-Source projects
+### Free API key for Open-Source projects
 
-If you are working on an open-source project, you can use the SDK for free.
-Just send us an email to `support@bavest.co` with the following information:
+First, use the [TypeForm](https://e0nemwrtihz.typeform.com/to/xT8KfS0I) to provide all required information.
+After, you will receive an API key via E-Mail.
 
-* Your GitHub username
-* The name of your project
-* The link to your project on GitHub
-* A description of your project
+### Template
+````python
+import os
+import dateutil
+from bavest import BavestRESTClient, Resolution
+from datetime import datetime
+import dateutil.relativedelta as relativedelta
+
+BAVEST_API_KEY = os.environ.get('BAVEST_API_KEY')
+client = BavestRESTClient(BAVEST_API_KEY)
+
+if __name__ == "__main__":
+    to = datetime.now()
+    frm = to + dateutil.relativedelta.relativedelta(days=-2)
+    to = to + dateutil.relativedelta.relativedelta(days=-1)
+    resolution = Resolution.DAILY
+    candles = client.candles("AAPL", frm, to, resolution)
+````
 
 ### Install the package
 
-First install the python package:
+First install the python package using [pip](https://pypi.org/project/bavest):
 
  ```python 
 pip install bavest 
  ```
+ 
+ 
+### Documentation
+See [here](https://docs.bavest.co/) for more information. 
 
 ### Usage
 
 1. Now, use the package in your project:
 
  ```python 
 from bavest import BavestRESTClient
@@ -76,7 +94,16 @@
 transactionItem = TransactionItem("MSFT", 2, frm).get()
 transactionList = [transactionItem]
 
 portfolioRegion = client.portfolio.region(transactionList)
 portfolioStats = client.portfolio.stats(frm, to, resolution, transactionList, "USD")
 portfolioChart = client.portfolio.chart(frm, to, resolution, transactionList)
  ```
+ 
+# :octocat: Credits
+1. William Todt <william.todt@bavest.co> - Maintainer
+2. Hisham Parveez <hisham.parveez@bavest.co> - Maintainer
+
+# Contact
+Please open a Github issue or send us an email at `support@bavest.co`.
+ 
+
```

### Comparing `bavest-1.0.0/bavest/errors.py` & `bavest-1.0.1/bavest/errors.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/client/bavest_client.py` & `bavest-1.0.1/bavest/finance/client/bavest_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -756,15 +756,15 @@
         :return:
         """
         try:
             frm_time = datetime.timestamp(frm_date)
             to_time = datetime.timestamp(to_date)
             body = {"symbol": symbol, "from": frm_time, "to": to_time, "resolution": resolution.name,
                     "currency": currency}
-            self.response = api.post(urls.quote_url, self.headers, body)
+            self.response = api.post(urls.candle_url, self.headers, body)
             content = check_response(json.loads(self.response.content))
             return content
         except requests.exceptions.Timeout:
             print("Timeout Error")
         except requests.exceptions.TooManyRedirects:
             print("Exceeded redirects:Bad URL, please try different URL")
```

### Comparing `bavest-1.0.0/bavest/finance/client/urls.py` & `bavest-1.0.1/bavest/finance/client/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,7 +31,9 @@
 etf_Profile = "https://api.bavest.co/v0/etf/profile"
 etf_holding = "https://api.bavest.co/v0/etf/holdings"
 etf_sector = "https://api.bavest.co/v0/etf/sector"
 etf_country = "https://api.bavest.co/v0/etf/country"
 search = "https://api.bavest.co/v0/search"
 api_status = "https://api.bavest.co/v0/status"
 forex = "https://api.bavest.co/v0/fx/quote"
+
+
```

### Comparing `bavest-1.0.0/bavest/finance/models/v0/etf/profile/profile.py` & `bavest-1.0.1/bavest/finance/models/v0/etf/profile/profile.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/forex/forex.py` & `bavest-1.0.1/bavest/finance/models/v0/forex/forex.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/market/news.py` & `bavest-1.0.1/bavest/finance/models/v0/market/news.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/portfolio/chart/chart.py` & `bavest-1.0.1/bavest/finance/models/v0/portfolio/chart/chart.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/portfolio/metric/metric.py` & `bavest-1.0.1/bavest/finance/models/v0/portfolio/metric/metric.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/portfolio/stats/stats.py` & `bavest-1.0.1/bavest/finance/models/v0/portfolio/stats/stats.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/quote/quote.py` & `bavest-1.0.1/bavest/finance/models/v0/quote/quote.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/search/search.py` & `bavest-1.0.1/bavest/finance/models/v0/search/search.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/sentiment/social_sentiment/social_sentiment.py` & `bavest-1.0.1/bavest/finance/models/v0/sentiment/social_sentiment/social_sentiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 
 def fromjson(json_response):
     if json_response is not None:
         user = SocialSentiment(**json_response)
     else:
         return {"error": 404, "body": "Bavest api error"}
     return user
+
```

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/analyst_estimates/analyst_estimates.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/analyst_estimates/analyst_estimates.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,7 +29,8 @@
 
 def fromjson(json_response):
     if json_response is not None:
         user = AnalystEstimates(**json_response)
     else:
         return {"error": 404, "body": "Bavest api error"}
     return user
+
```

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/calendar/earnings/earnings.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/calendar/earnings/earnings.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/calendar/economics/economics.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/calendar/economics/economics.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,7 +21,8 @@
 
 def fromjson(json_response):
     if json_response is not None:
         user = EconomicCalendar(**json_response)
     else:
         return {"error": 404, "body": "Bavest api error"}
     return user
+
```

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/esg/esg.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/esg/esg.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/financials/financials.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/financials/financials.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/fundamentals/fundamentals.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/fundamentals/fundamentals.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/ipo/prospectus/prospectus.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/ipo/prospectus/prospectus.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/metric/metric.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/metric/metric.py`

 * *Files identical despite different names*

### Comparing `bavest-1.0.0/bavest/finance/models/v0/stock/profile/profile.py` & `bavest-1.0.1/bavest/finance/models/v0/stock/profile/profile.py`

 * *Files identical despite different names*

