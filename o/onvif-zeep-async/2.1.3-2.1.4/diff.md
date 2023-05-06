# Comparing `tmp/onvif-zeep-async-2.1.3.tar.gz` & `tmp/onvif-zeep-async-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-2.1.3.tar", last modified: Sat May  6 21:13:50 2023, max compression
+gzip compressed data, was "onvif-zeep-async-2.1.4.tar", last modified: Sat May  6 21:24:12 2023, max compression
```

## Comparing `onvif-zeep-async-2.1.3.tar` & `onvif-zeep-async-2.1.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:13:50.499552 onvif-zeep-async-2.1.3/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.3/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.3/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 21:13:50.499601 onvif-zeep-async-2.1.3/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:13:50.491352 onvif-zeep-async-2.1.3/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:13:50.491938 onvif-zeep-async-2.1.3/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    29161 2023-05-06 21:13:27.000000 onvif-zeep-async-2.1.3/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 21:13:35.000000 onvif-zeep-async-2.1.3/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:13:50.498544 onvif-zeep-async-2.1.3/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.1.3/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:13:50.499354 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 21:13:50.000000 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-06 21:13:50.000000 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-06 21:13:50.000000 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-06 21:13:50.000000 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-06 21:13:50.000000 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 21:13:50.000000 onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-06 21:13:50.499833 onvif-zeep-async-2.1.3/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:13:50.499458 onvif-zeep-async-2.1.3/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.3/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.893273 onvif-zeep-async-2.1.4/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.4/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.4/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 21:24:12.893325 onvif-zeep-async-2.1.4/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.886771 onvif-zeep-async-2.1.4/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.887355 onvif-zeep-async-2.1.4/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    28963 2023-05-06 21:23:49.000000 onvif-zeep-async-2.1.4/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 21:23:52.000000 onvif-zeep-async-2.1.4/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.892233 onvif-zeep-async-2.1.4/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.1.4/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.893061 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-06 21:24:12.893556 onvif-zeep-async-2.1.4/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.893172 onvif-zeep-async-2.1.4/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/tests/test.py
```

### Comparing `onvif-zeep-async-2.1.3/.gitignore` & `onvif-zeep-async-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/.pre-commit-config.yaml` & `onvif-zeep-async-2.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/LICENSE` & `onvif-zeep-async-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/Makefile` & `onvif-zeep-async-2.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/PKG-INFO` & `onvif-zeep-async-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.1.3
+Version: 2.1.4
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-2.1.3/README.rst` & `onvif-zeep-async-2.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/examples/events.py` & `onvif-zeep-async-2.1.4/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/examples/rotate_image.py` & `onvif-zeep-async-2.1.4/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/examples/streaming.py` & `onvif-zeep-async-2.1.4/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/__init__.py` & `onvif-zeep-async-2.1.4/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/client.py` & `onvif-zeep-async-2.1.4/onvif/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,18 +406,19 @@
         # Create subscription manager
         # 5.2.3 BASIC NOTIFICATION INTERFACE - NOTIFY
         # Call SetSynchronizationPoint to generate a notification message
         # to ensure the webhooks are working.
         #
         # If this fails this is OK as it just means we will switch
         # to webhook later when the first notification is received.
-        # WSAs enabled per
-        # https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        #
+        # WSAs not enabled on this service per
+        # https://github.com/home-assistant/core/issues/92308
         service = await self._device.create_onvif_service(
-            "pullpoint", port_type="NotificationConsumer", enable_wsa=True
+            "pullpoint", port_type="NotificationConsumer"
         )
         self._operation = service.document.bindings[service.binding_name].get(
             "PullMessages"
         )
         self._service = service
         return await self._device.create_subscription_service("NotificationConsumer")
 
@@ -723,18 +724,18 @@
     async def create_deviceio_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("deviceio")
 
     async def create_events_service(self) -> ONVIFService:
         """Service creation helper.
 
-        WSAs enabled per
-        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        WSAs not enabled on this service per
+        https://github.com/home-assistant/core/issues/92308
         """
-        return await self.create_onvif_service("events", enable_wsa=True)
+        return await self.create_onvif_service("events")
 
     async def create_analytics_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("analytics")
 
     async def create_recording_service(self) -> ONVIFService:
         """Service creation helper."""
@@ -747,32 +748,31 @@
     async def create_replay_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("replay")
 
     async def create_pullpoint_service(self) -> ONVIFService:
         """Service creation helper.
 
-        WSAs enabled per
-        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        WSAs not enabled on this service per
+        https://github.com/home-assistant/core/issues/92308
         """
         return await self.create_onvif_service(
             "pullpoint",
             port_type="PullPointSubscription",
             read_timeout=_PULLPOINT_TIMEOUT,
             write_timeout=_PULLPOINT_TIMEOUT,
-            enable_wsa=True,
         )
 
     async def create_notification_service(self) -> ONVIFService:
         """Service creation helper.
 
-        WSAs enabled per
-        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        WSAs not enabled on this service per
+        https://github.com/home-assistant/core/issues/92308
         """
-        return await self.create_onvif_service("notification", enable_wsa=True)
+        return await self.create_onvif_service("notification")
 
     async def create_subscription_service(
         self, port_type: Optional[str] = None
     ) -> ONVIFService:
         """Service creation helper.
 
         WSAs enabled per
```

### Comparing `onvif-zeep-async-2.1.3/onvif/definition.py` & `onvif-zeep-async-2.1.4/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/exceptions.py` & `onvif-zeep-async-2.1.4/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/.events.wsdl.swn` & `onvif-zeep-async-2.1.4/onvif/wsdl/.events.wsdl.swn`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/addressing` & `onvif-zeep-async-2.1.4/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/display.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/envelope` & `onvif-zeep-async-2.1.4/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/events.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/media.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/search.wsdl` & `onvif-zeep-async-2.1.4/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/types.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/xml.xsd` & `onvif-zeep-async-2.1.4/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif/wsdl/xmlmime` & `onvif-zeep-async-2.1.4/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.1.3
+Version: 2.1.4
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-2.1.3/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/pylintrc` & `onvif-zeep-async-2.1.4/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/setup.py` & `onvif-zeep-async-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.3/tests/test.py` & `onvif-zeep-async-2.1.4/tests/test.py`

 * *Files identical despite different names*

