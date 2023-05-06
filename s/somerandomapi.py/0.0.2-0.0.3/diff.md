# Comparing `tmp/somerandomapi.py-0.0.2.tar.gz` & `tmp/somerandomapi.py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somerandomapi.py-0.0.2.tar", last modified: Sat Mar  4 16:47:18 2023, max compression
+gzip compressed data, was "somerandomapi.py-0.0.3.tar", last modified: Sat May  6 16:38:39 2023, max compression
```

## Comparing `somerandomapi.py-0.0.2.tar` & `somerandomapi.py-0.0.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.754312 somerandomapi.py-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-03-04 16:47:18.754312 somerandomapi.py-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 16:47:18.754312 somerandomapi.py-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.742312 somerandomapi.py-0.0.2/somerandomapi/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.746312 somerandomapi.py-0.0.2/somerandomapi/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/animu.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/clients/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.746312 somerandomapi.py-0.0.2/somerandomapi/internals/
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/internals/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/internals/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.750312 somerandomapi.py-0.0.2/somerandomapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/animal_fact.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/animu_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/lyrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/namecard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/rankcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/tweet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.750312 somerandomapi.py-0.0.2/somerandomapi/models/welcome/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/welcome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/welcome/free.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/welcome/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/models/youtube_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.750312 somerandomapi.py-0.0.2/somerandomapi/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/animu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.754312 somerandomapi.py-0.0.2/somerandomapi/types/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/canvas/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/canvas/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/canvas/overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/img.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/others.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/types/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-03-04 16:47:11.000000 somerandomapi.py-0.0.2/somerandomapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:47:18.742312 somerandomapi.py-0.0.2/somerandomapi.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-03-04 16:47:18.000000 somerandomapi.py-0.0.2/somerandomapi.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-04 16:47:18.000000 somerandomapi.py-0.0.2/somerandomapi.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 16:47:18.000000 somerandomapi.py-0.0.2/somerandomapi.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-04 16:47:18.000000 somerandomapi.py-0.0.2/somerandomapi.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-04 16:47:18.000000 somerandomapi.py-0.0.2/somerandomapi.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/animu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/clients/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/internals/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/internals/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.697849 somerandomapi.py-0.0.3/somerandomapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/animal_fact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/animu_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/namecard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/rankcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/tweet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.697849 somerandomapi.py-0.0.3/somerandomapi/models/welcome/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/welcome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/welcome/free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/welcome/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/models/youtube_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.697849 somerandomapi.py-0.0.3/somerandomapi/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/animu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.701849 somerandomapi.py-0.0.3/somerandomapi/types/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/canvas/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/canvas/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/canvas/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/img.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/others.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/types/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-06 16:38:28.000000 somerandomapi.py-0.0.3/somerandomapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:38:39.693849 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 16:38:39.000000 somerandomapi.py-0.0.3/somerandomapi.py.egg-info/top_level.txt
```

### Comparing `somerandomapi.py-0.0.2/LICENSE` & `somerandomapi.py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/PKG-INFO` & `somerandomapi.py-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somerandomapi.py
-Version: 0.0.2
+Version: 0.0.3
 Summary: A maintained wrapper for the somerandomapi API.
 Author: Soheab_
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -375,15 +375,15 @@
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
 Project-URL: homepage, https://github.com/Soheab/somerandomapi.py
 Project-URL: documentation, https://somerandomapipy.readthedocs.io/
 Project-URL: repository, https://github.com/Soheab/somerandomapi.py
-Keywords: some-random-api,api,somerandomapi,random,images,fun,discord,discord.py,generation,rankcard,canvas,welcome,free,open-source,asyncio,aiohttp,async,wrapper
+Keywords: https://some-random-api.com,some-random-api,api,somerandomapi,random,images,fun,discord,discord.py,generation,rankcard,canvas,welcome,free,open-source,asyncio,aiohttp,async,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -401,14 +401,14 @@
 **Documentation**: https://somerandomapipy.readthedocs.io/ \
 **Examples**: https://github.com/Soheab/somerandomapi.py/blob/main/examples \
 **PyPI**: https://pypi.org/project/somerandomapi.py/
 
 **Installation**: `pip install somerandomapi.py`
 
 
-**API**: https://somerandomapi.com/ \
+**API**: https://some-random-api.ml/ \
 **API Discord**: https://discord.gg/tTUMWFd
 
 **Library Discord**: https://discord.gg/yCzcfju
 
 
 **License**: MLP-2.0
```

### Comparing `somerandomapi.py-0.0.2/pyproject.toml` & `somerandomapi.py-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 name = "somerandomapi.py"
 description = "A maintained wrapper for the somerandomapi API."
 authors = [
     {name = "Soheab_"},
 ]
 requires-python = ">=3.9"
 keywords = [
+    "https://some-random-api.com",
     "some-random-api",
     "api",
     "somerandomapi",
     "random",
     "images",
     "fun",
     "discord",
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/__init__.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/animal.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/animal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union
 
+from .. import utils
 from ..enums import Animal as AnimalEnum, FactAnimal as AnimalFactsEnum, ImgAnimal as AnimalImgEnum
 from ..internals.endpoints import Animal as AnimalEndpoint, Facts as AnimalFactsEndpoint, Img as AnimalImgEndpoint
 from ..models.animal_fact import AnimalImageFact
 
 
 if TYPE_CHECKING:
     from ..internals.http import HTTPClient
@@ -45,15 +46,15 @@
         if not isinstance(animal, AnimalEnum):
             valid_animals = list(map(str, list(AnimalEnum)))
             if animal not in valid_animals:
                 raise ValueError(
                     f"'animal' must be an instance of `Animal` or one of {', '.join(valid_animals)}, not {animal!r}"
                 )
 
-            _animal = AnimalEnum(animal.upper())
+            _animal = AnimalEnum(animal.lower())
 
         _endpoint: AnimalEndpoint = AnimalEndpoint.from_enum(_animal)
         response = await self.__http.request(_endpoint)
         return AnimalImageFact(**response)
 
     async def get_image(self, animal: Union[AnimalImgEnum, ImgAnimalsLiterals]) -> str:
         """Get a random image of an animal.
@@ -73,15 +74,15 @@
         if not isinstance(animal, AnimalImgEnum):
             valid_animals = list(map(str, list(AnimalImgEnum)))
             if animal not in valid_animals:
                 raise ValueError(
                     f"'animal' must be an instance of `ImgAnimal` or one of {', '.join(valid_animals)}, not {animal!r}"
                 )
 
-            _animal = AnimalImgEnum(animal.upper())
+            _animal = AnimalImgEnum(animal.lower())
 
         _endpoint: AnimalImgEndpoint = AnimalImgEndpoint.from_enum(_animal)
         response = await self.__http.request(_endpoint)
         return response["link"]
 
     async def get_fact(self, animal: Union[AnimalFactsEnum, FactsAnimalsLiterals]) -> str:
         """Get a random fact about an animal.
@@ -101,12 +102,12 @@
         if not isinstance(animal, AnimalFactsEnum):
             valid_animals = list(map(str, list(AnimalFactsEnum)))
             if animal not in valid_animals:
                 raise ValueError(
                     f"'animal' must be an instance of `FactAnimal` or one of {', '.join(valid_animals)}, not {animal!r}"
                 )
 
-            _animal = AnimalFactsEnum(animal.upper())
+            _animal = AnimalFactsEnum(animal.lower())
 
         _endpoint: AnimalFactsEndpoint = AnimalFactsEndpoint.from_enum(_animal)
         response = await self.__http.request(_endpoint)
         return response["fact"]
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/animu.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/animu.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/canvas.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from .. import utils as _utils
 from ..enums import CanvasBorder, CanvasCrop, CanvasFilter, CanvasOverlay
 from ..internals.endpoints import (
     CanvasFilter as CanvasFilterEndpoint,
     CanvasMisc as CanvasMiscEndpoint,
     CanvasOverlay as CanvasOverlayEndpoint,
-)
+    )
 from ..models.image import Image
 from ..models.namecard import GenshinNamecard
 from ..models.tweet import Tweet
 from ..models.youtube_comment import YoutubeComment
 
 
 if TYPE_CHECKING:
@@ -66,22 +66,23 @@
         _enum = CanvasFilter
         if not isinstance(filter, _enum):
             raise TypeError(f"Expected CanvasFilter, got {filter.__class__.__name__}")
 
         # because these require different parameters, we need to check and deny them here
         if filter in (_enum.BRIGHTNESS, _enum.COLOR, _enum.THRESHOLD):
             raise ValueError(
-                f"Filter {filter} cannot be used with this method. Use `filter_{filter.name.lower()}` instead."
+                f"Filter {filter} cannot be used with this method. Use `.filter_{filter.name.lower()}()` instead."
             )
 
-        _endpoint_cls = (
-            CanvasFilterEndpoint if filter not in (_enum.BLUR, _enum.JPG, _enum.PIXELATE) else CanvasMiscEndpoint
-        )
 
-        _endpoint = _endpoint_cls.from_enum(filter)
+        if filter in (_enum.BLUR, _enum.JPG, _enum.PIXELATE):
+            _endpoint = CanvasMiscEndpoint.from_enum(filter)
+        else:
+            _endpoint = CanvasFilterEndpoint.from_enum(filter)
+
         return await self.__http.request(_endpoint, avatar=avatar_url)
 
     async def filter_brightness(self, avatar_url: str, brightness: Optional[int] = None) -> Image:
         """Apply a brightness filter to an image.
 
         Parameters
         ----------
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/chatbot.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/chatbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         This is used for the ratelimit handling.
         As of writing:
         - 1: 15 requests per 60 seconds
         - 2: 30 requests per 60 seconds
         - 3: 60 requests per 60 seconds
 
     _handle_ratelimit: :class:`bool`
-        https://some-random-api.ml/docs/welcome/ratelimits#chatbot
+        https://some-random-api.com/docs/welcome/ratelimits#chatbot
         Whether to handle the ratelimit automatically. This is subject to change and should not be relied on.
         If this is set to ``True``, you must provide either a client or a key and a key_tier.
     """
 
     _endpoint = ChatbotEndpoints.CHATBOT
     __request: _ChatbotRequestMethod
     # __ratelimit: Ratelimit
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/client.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/client.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/pokemon.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/clients/premium.py` & `somerandomapi.py-0.0.3/somerandomapi/clients/premium.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/enums.py` & `somerandomapi.py-0.0.3/somerandomapi/enums.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/errors.py` & `somerandomapi.py-0.0.3/somerandomapi/errors.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/internals/endpoints.py` & `somerandomapi.py-0.0.3/somerandomapi/internals/endpoints.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Optional, TYPE_CHECKING
+from typing import Any, Callable, Literal, Optional, TYPE_CHECKING
 from urllib.parse import quote_plus, urlencode
 
-from ..enums import BaseEnum
+from .. import enums
 
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from ..internals.http import APIKey
     from ..types.http import ValidPaths
@@ -20,25 +20,25 @@
 _TIER_ERROR_PARAMETER = (
     "Missing required key tier level for {param} param for the {path} endpoint. "
     "Expected a tier {tier} or above key. "
     "Either pass such key when calling the method, set it in the Client constructor or don't pass the parameter."
 )
 
 
-class BaseEndpoint(BaseEnum):
+class BaseEndpoint(enums.BaseEnum):
     @classmethod
     def ratelimit(cls) -> tuple[int, int]:
         raise NotImplementedError
 
     @classmethod
     def base(cls) -> ValidPaths:
         raise NotImplementedError
 
     @classmethod
-    def from_enum(cls, enum: BaseEnum) -> Self:
+    def from_enum(cls, enum: enums.BaseEnum) -> Self:
         try:
             val = enum.value.replace("-", "_").upper()
             return getattr(cls, val)
         except AttributeError:
             raise AttributeError("No endpoint found for this enum") from None
 
 
@@ -156,32 +156,62 @@
 EndpointWithAvatarParam: Callable[[str], Endpoint] = lambda path: Endpoint(
     path,
     avatar=Parameter(extra="use png or jpg"),
 )
 
 
 class Animu(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[None]) -> None:
+            ...
+
     @classmethod
     def base(cls):
         return "animu/"
 
     FACE_PALM = Endpoint("face-palm")
     HUG = Endpoint("hug")
     PAT = Endpoint("pat")
     QUOTE = Endpoint("quote")
     WINK = Endpoint("wink")
 
 
 class BaseCanvas(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[None]) -> None:
+            ...
+
     @classmethod
     def base(cls):
         return "canvas/"
 
 
 class CanvasFilter(BaseCanvas):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(
+            cls,
+            enum: Literal[
+                enums.CanvasFilter.BLURPLE,
+                enums.CanvasFilter.BLURPLE_2,
+                enums.CanvasFilter.BRIGHTNESS,
+                enums.CanvasFilter.COLOR,
+                enums.CanvasFilter.BLUE,
+                enums.CanvasFilter.GREEN,
+                enums.CanvasFilter.RED,
+                enums.CanvasFilter.SEPIA,
+                enums.CanvasFilter.GREYSCALE,
+                enums.CanvasFilter.INVERT,
+                enums.CanvasFilter.INVERT_GREYSCALE,
+                enums.CanvasFilter.THRESHOLD,
+        ]) -> Self:
+            ...
+
     @classmethod
     def base(cls):
         return super().base() + "filter/"
 
     BLUE = EndpointWithAvatarParam("blue")
     BLURPLE = EndpointWithAvatarParam("blurple")
     BLURPLE_2 = EndpointWithAvatarParam("blurple2")
@@ -205,14 +235,19 @@
         "threshold",
         avatar=Parameter(extra="use png or jpg"),
         threshold=Parameter(required=False, extra="threshold value from 1-255"),
     )
 
 
 class CanvasMisc(BaseCanvas):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[enums.CanvasFilter.BLUR, enums.CanvasFilter.JPG, enums.CanvasFilter.PIXELATE]) -> Self:
+            ...
+
     @classmethod
     def base(cls):
         return super().base() + "misc/"
 
     BISEXUAL_BORDER = EndpointWithAvatarParam("bisexual")
     BLUR = EndpointWithAvatarParam("blur")
     CIRCLE_CROP = EndpointWithAvatarParam("circle")
@@ -264,42 +299,57 @@
         username=Parameter(extra="max 25 characters"),
         avatar=Parameter(extra="use png or jpg"),
         comment=Parameter(extra="max 1000 characters"),
     )
 
 
 class CanvasOverlay(BaseCanvas):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: enums.CanvasOverlay) -> Self:
+            ...
+
     @classmethod
     def base(cls):
         return super().base() + "overlay/"
 
     COMRADE = EndpointWithAvatarParam("comrade")
     GAY = EndpointWithAvatarParam("gay")
     GLASS = EndpointWithAvatarParam("glass")
     JAIL = EndpointWithAvatarParam("jail")
     PASSED = EndpointWithAvatarParam("passed")
     TRIGGERED = EndpointWithAvatarParam("triggered")
     WASTED = EndpointWithAvatarParam("wasted")
 
 
 class Facts(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: enums.FactAnimal) -> Self:
+            ...
+
     @classmethod
     def base(cls):
         return "facts/"
 
     # can't subclass BaseAnimals
     BIRD = Endpoint("bird")
     CAT = Endpoint("cat")
     DOG = Endpoint("dog")
     FOX = Endpoint("fox")
     KOALA = Endpoint("koala")
     PANDA = Endpoint("panda")
 
 
 class Animal(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: enums.Animal) -> Self:
+            ...
+
     @classmethod
     def base(cls):
         return "animal/"
 
     # can't subclass BaseAnimals
     BIRD = Endpoint("bird")
     CAT = Endpoint("cat")
@@ -310,14 +360,19 @@
 
     KANGAROO = Endpoint("kangaroo")
     RACCOON = Endpoint("raccoon")
     RED_PANDA = Endpoint("red_panda")
 
 
 class Img(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: enums.ImgAnimal) -> Self:
+            ...
+
     @classmethod
     def base(cls):
         return "img/"
 
     # can't subclass BaseAnimals
     BIRD = Endpoint("bird")
     CAT = Endpoint("cat")
@@ -327,14 +382,19 @@
     PANDA = Endpoint("panda")
 
     PIKACHU = Endpoint("pikachu")
     WHALE = Endpoint("whale")
 
 
 class Others(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[None]) -> None:
+            ...
+
     @classmethod
     def base(cls):
         return "others/"
 
     BASE64 = Endpoint(
         "base64",
         encode=Parameter(extra="Text to encode into base64", required=False),
@@ -348,25 +408,35 @@
     BOTTOKEN = Endpoint("bottoken", id=Parameter(extra="ID of the discord bot"))
     DICTIONARY = Endpoint("dictionary", word=Parameter(extra="Word to lookup"))
     JOKE = Endpoint("joke")
     LYRICS = Endpoint("lyrics", title=Parameter(extra="Title of song to search"))
 
 
 class Pokemon(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[None]) -> None:
+            ...
+
     @classmethod
     def base(cls):
         return "pokemon/"
 
     ABILITIES = Endpoint("abilities", ability=Parameter(extra="Ability name or id of a pokemon ability"))
     ITEMS = Endpoint("items", item=Parameter(extra="Item name or id of a pokemon item"))
     MOVES = Endpoint("moves", move=Parameter(extra="Pokemon move name or id of a pokemon move"))
     POKEDEX = Endpoint("pokedex", pokemon=Parameter(extra="Pokemon name"))
 
 
 class Premium(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[None]) -> None:
+            ...
+
     @classmethod
     def base(cls):
         return "premium/"
 
     AMONGUS = Endpoint(
         "amongus",
         avatar=Parameter(extra="use png or jpg"),
@@ -408,14 +478,19 @@
         font=Parameter(
             required=False, extra="Choose a custom font from our predetermined list, use a number from 1-10"
         ),
     )
 
 
 class Chatbot(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[None]) -> None:
+            ...
+
     @classmethod
     def base(cls):
         return ""
 
     CHATBOT = Endpoint(
         "chatbot",
         message=Parameter(extra="Message that will be sent to the chatbot"),
@@ -423,14 +498,19 @@
             key_tier=1,
             is_key_parameter=True,
         ),  # assuming tier 1 is the minimum
     )
 
 
 class WelcomeImages(BaseEndpoint):
+    if TYPE_CHECKING:
+        @classmethod
+        def from_enum(cls, enum: Literal[None]) -> None:
+            ...
+
     @classmethod
     def base(cls):
         return "welcome/img/"
 
     WELCOME = Endpoint(
         "",
         type=Parameter(),
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi/internals/http.py` & `somerandomapi.py-0.0.3/somerandomapi/internals/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     T = TypeVar("T")
     Response = Coroutine[Any, Any, T]
 
 
 __all__ = ()
 
 
-# source: https://github.com/Rapptz/discord.py/blob/master/discord/http.py
 async def json_or_text(response: aiohttp.ClientResponse) -> Union[dict[str, Any], str]:
     text = await response.text(encoding="utf-8")
     if response.content_type == "application/json":
         return json.loads(text)
 
     return text
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/abc.py` & `somerandomapi.py-0.0.3/somerandomapi/models/abc.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/dictionary.py` & `somerandomapi.py-0.0.3/somerandomapi/models/dictionary.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/encoding.py` & `somerandomapi.py-0.0.3/somerandomapi/models/encoding.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/image.py` & `somerandomapi.py-0.0.3/somerandomapi/models/image.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/lyrics.py` & `somerandomapi.py-0.0.3/somerandomapi/models/lyrics.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/namecard.py` & `somerandomapi.py-0.0.3/somerandomapi/models/namecard.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/pokemon.py` & `somerandomapi.py-0.0.3/somerandomapi/models/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/rankcard.py` & `somerandomapi.py-0.0.3/somerandomapi/models/rankcard.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/rgb.py` & `somerandomapi.py-0.0.3/somerandomapi/models/rgb.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/tweet.py` & `somerandomapi.py-0.0.3/somerandomapi/models/tweet.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/welcome/free.py` & `somerandomapi.py-0.0.3/somerandomapi/models/welcome/free.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/welcome/premium.py` & `somerandomapi.py-0.0.3/somerandomapi/models/welcome/premium.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/models/youtube_comment.py` & `somerandomapi.py-0.0.3/somerandomapi/models/youtube_comment.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/types/pokemon.py` & `somerandomapi.py-0.0.3/somerandomapi/types/pokemon.py`

 * *Files identical despite different names*

### Comparing `somerandomapi.py-0.0.2/somerandomapi/utils.py` & `somerandomapi.py-0.0.3/somerandomapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,21 @@
 
 
 def _try_enum(enum: Type[EnumT], input: Any) -> Optional[EnumT]:
     if not input:
         return None
 
     try:
-        return enum[input]
+        return enum[input.upper()] # name
     except KeyError:
         try:
-            return enum(input)
+            return enum(input.lower()) # value
         except ValueError:
             return None
 
-    return None
-
-
 def _gen_colour(numbers: Optional[int] = None) -> str:
     random_number = numbers or random.randint(0, 16777215)
     hex_number = str(hex(random_number))
     return hex_number[2:]
 
 
 def _check_colour_value(hex_input: Optional[Union[str, int]], param_name: Optional[str] = None) -> str:
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi.py.egg-info/PKG-INFO` & `somerandomapi.py-0.0.3/somerandomapi.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somerandomapi.py
-Version: 0.0.2
+Version: 0.0.3
 Summary: A maintained wrapper for the somerandomapi API.
 Author: Soheab_
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -375,15 +375,15 @@
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
 Project-URL: homepage, https://github.com/Soheab/somerandomapi.py
 Project-URL: documentation, https://somerandomapipy.readthedocs.io/
 Project-URL: repository, https://github.com/Soheab/somerandomapi.py
-Keywords: some-random-api,api,somerandomapi,random,images,fun,discord,discord.py,generation,rankcard,canvas,welcome,free,open-source,asyncio,aiohttp,async,wrapper
+Keywords: https://some-random-api.com,some-random-api,api,somerandomapi,random,images,fun,discord,discord.py,generation,rankcard,canvas,welcome,free,open-source,asyncio,aiohttp,async,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -401,14 +401,14 @@
 **Documentation**: https://somerandomapipy.readthedocs.io/ \
 **Examples**: https://github.com/Soheab/somerandomapi.py/blob/main/examples \
 **PyPI**: https://pypi.org/project/somerandomapi.py/
 
 **Installation**: `pip install somerandomapi.py`
 
 
-**API**: https://somerandomapi.com/ \
+**API**: https://some-random-api.ml/ \
 **API Discord**: https://discord.gg/tTUMWFd
 
 **Library Discord**: https://discord.gg/yCzcfju
 
 
 **License**: MLP-2.0
```

### Comparing `somerandomapi.py-0.0.2/somerandomapi.py.egg-info/SOURCES.txt` & `somerandomapi.py-0.0.3/somerandomapi.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

