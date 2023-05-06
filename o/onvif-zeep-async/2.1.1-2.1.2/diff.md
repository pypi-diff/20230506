# Comparing `tmp/onvif-zeep-async-2.1.1.tar.gz` & `tmp/onvif-zeep-async-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-2.1.1.tar", last modified: Fri May  5 00:25:38 2023, max compression
+gzip compressed data, was "onvif-zeep-async-2.1.2.tar", last modified: Sat May  6 18:20:48 2023, max compression
```

## Comparing `onvif-zeep-async-2.1.1.tar` & `onvif-zeep-async-2.1.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-05 00:25:38.627652 onvif-zeep-async-2.1.1/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.1/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.1/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-05 00:25:38.627723 onvif-zeep-async-2.1.1/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-05 00:25:38.618823 onvif-zeep-async-2.1.1/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-05 00:25:38.619451 onvif-zeep-async-2.1.1/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    27861 2023-05-05 00:24:59.000000 onvif-zeep-async-2.1.1/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-05 00:25:09.000000 onvif-zeep-async-2.1.1/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-05 00:25:38.626605 onvif-zeep-async-2.1.1/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.1.1/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-05 00:25:38.627418 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-05 00:25:38.000000 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-05 00:25:38.000000 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-05 00:25:38.000000 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-05 00:25:38.000000 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-05 00:25:38.000000 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-05 00:25:38.000000 onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-05 00:25:38.627962 onvif-zeep-async-2.1.1/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-05 00:25:38.627521 onvif-zeep-async-2.1.1/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.1/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 18:20:48.216812 onvif-zeep-async-2.1.2/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.2/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.2/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 18:20:48.216911 onvif-zeep-async-2.1.2/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 18:20:48.206711 onvif-zeep-async-2.1.2/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 18:20:48.207649 onvif-zeep-async-2.1.2/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    29161 2023-05-06 18:15:36.000000 onvif-zeep-async-2.1.2/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 18:15:43.000000 onvif-zeep-async-2.1.2/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 18:20:48.215277 onvif-zeep-async-2.1.2/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.1.2/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 18:20:48.216474 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 18:20:48.000000 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-06 18:20:48.000000 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-06 18:20:48.000000 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-06 18:20:48.000000 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-06 18:20:48.000000 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 18:20:48.000000 onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-06 18:20:48.217200 onvif-zeep-async-2.1.2/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 18:20:48.216657 onvif-zeep-async-2.1.2/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.2/tests/test.py
```

### Comparing `onvif-zeep-async-2.1.1/.gitignore` & `onvif-zeep-async-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/.pre-commit-config.yaml` & `onvif-zeep-async-2.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/LICENSE` & `onvif-zeep-async-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/Makefile` & `onvif-zeep-async-2.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/PKG-INFO` & `onvif-zeep-async-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.1.1
+Version: 2.1.2
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-2.1.1/README.rst` & `onvif-zeep-async-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/examples/events.py` & `onvif-zeep-async-2.1.2/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/examples/rotate_image.py` & `onvif-zeep-async-2.1.2/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/examples/streaming.py` & `onvif-zeep-async-2.1.2/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/__init__.py` & `onvif-zeep-async-2.1.2/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/client.py` & `onvif-zeep-async-2.1.2/onvif/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,14 +248,15 @@
         encrypt=True,
         no_cache=False,
         dt_diff=None,
         binding_name="",
         binding_key="",
         read_timeout: Optional[int] = None,
         write_timeout: Optional[int] = None,
+        enable_wsa: bool = False,
     ) -> None:
         if not _path_isfile(url):
             raise ONVIFError("%s doesn`t exist!" % url)
 
         self.url = url
         self.xaddr = xaddr
         self.binding_key = binding_key
@@ -292,40 +293,45 @@
         self.document: Optional[Document] = None
         self.zeep_client_authless: Optional[ZeepAsyncClient] = None
         self.ws_client_authless: Optional[AsyncServiceProxy] = None
         self.zeep_client: Optional[ZeepAsyncClient] = None
         self.ws_client: Optional[AsyncServiceProxy] = None
         self.create_type: Optional[Callable] = None
         self.loop = asyncio.get_event_loop()
+        self._enable_wsa = enable_wsa
 
     async def setup(self):
         """Setup the transport."""
         settings = _DEFAULT_SETTINGS
         binding_name = self.binding_name
         wsse = UsernameDigestTokenDtDiff(
             self.user, self.passwd, dt_diff=self.dt_diff, use_digest=self.encrypt
         )
         self.document = await self.loop.run_in_executor(
             None, _cached_document, self.url
         )
+        # Some cameras never return a response to GetCapabilities if WS-Addressing is enabled
+        # but some cameras require WS-Addressing to be enabled for PullPoint or events to work
+        # so we have a flag to enable/disable it which can be changed per service.
+        plugins = [WsAddressingPlugin()] if self._enable_wsa else []
         self.zeep_client_authless = ZeepAsyncClient(
             wsdl=self.document,
             transport=self.transport,
             settings=settings,
-            plugins=[WsAddressingPlugin()],
+            plugins=plugins,
         )
         self.ws_client_authless = self.zeep_client_authless.create_service(
             binding_name, self.xaddr
         )
         self.zeep_client = ZeepAsyncClient(
             wsdl=self.document,
             wsse=wsse,
             transport=self.transport,
             settings=settings,
-            plugins=[WsAddressingPlugin()],
+            plugins=plugins,
         )
         self.ws_client = self.zeep_client.create_service(binding_name, self.xaddr)
         namespace = binding_name[binding_name.find("{") + 1 : binding_name.find("}")]
         available_ns = self.zeep_client.namespaces
         active_ns = (
             list(available_ns.keys())[list(available_ns.values()).index(namespace)]
             or "ns0"
@@ -400,16 +406,18 @@
         # Create subscription manager
         # 5.2.3 BASIC NOTIFICATION INTERFACE - NOTIFY
         # Call SetSynchronizationPoint to generate a notification message
         # to ensure the webhooks are working.
         #
         # If this fails this is OK as it just means we will switch
         # to webhook later when the first notification is received.
+        # WSAs enabled per
+        # https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
         service = await self._device.create_onvif_service(
-            "pullpoint", port_type="NotificationConsumer"
+            "pullpoint", port_type="NotificationConsumer", enable_wsa=True
         )
         self._operation = service.document.bindings[service.binding_name].get(
             "PullMessages"
         )
         self._service = service
         return await self._device.create_subscription_service("NotificationConsumer")
 
@@ -645,14 +653,15 @@
 
     async def create_onvif_service(
         self,
         name: str,
         port_type: Optional[str] = None,
         read_timeout: Optional[int] = None,
         write_timeout: Optional[int] = None,
+        enable_wsa: bool = False,
     ) -> ONVIFService:
         """Create ONVIF service client"""
         name = name.lower()
         # Don't re-create bindings if the xaddr remains the same.
         # The xaddr can change when a new PullPointSubscription is created.
         binding_key = (name, port_type)
 
@@ -683,14 +692,15 @@
             self.encrypt,
             no_cache=self.no_cache,
             dt_diff=self.dt_diff,
             binding_name=binding_name,
             binding_key=binding_key,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
+            enable_wsa=enable_wsa,
         )
         await service.setup()
 
         self.services[binding_key] = service
 
         return service
 
@@ -711,16 +721,20 @@
         return await self.create_onvif_service("imaging")
 
     async def create_deviceio_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("deviceio")
 
     async def create_events_service(self) -> ONVIFService:
-        """Service creation helper."""
-        return await self.create_onvif_service("events")
+        """Service creation helper.
+
+        WSAs enabled per
+        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        """
+        return await self.create_onvif_service("events", enable_wsa=True)
 
     async def create_analytics_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("analytics")
 
     async def create_recording_service(self) -> ONVIFService:
         """Service creation helper."""
@@ -731,28 +745,43 @@
         return await self.create_onvif_service("search")
 
     async def create_replay_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("replay")
 
     async def create_pullpoint_service(self) -> ONVIFService:
-        """Service creation helper."""
+        """Service creation helper.
+
+        WSAs enabled per
+        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        """
         return await self.create_onvif_service(
             "pullpoint",
             port_type="PullPointSubscription",
             read_timeout=_PULLPOINT_TIMEOUT,
             write_timeout=_PULLPOINT_TIMEOUT,
+            enable_wsa=True,
         )
 
     async def create_notification_service(self) -> ONVIFService:
-        """Service creation helper."""
-        return await self.create_onvif_service("notification")
+        """Service creation helper.
+
+        WSAs enabled per
+        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        """
+        return await self.create_onvif_service("notification", enable_wsa=True)
 
     async def create_subscription_service(
         self, port_type: Optional[str] = None
     ) -> ONVIFService:
-        """Service creation helper."""
-        return await self.create_onvif_service("subscription", port_type=port_type)
+        """Service creation helper.
+
+        WSAs enabled per
+        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
+        """
+        return await self.create_onvif_service(
+            "subscription", port_type=port_type, enable_wsa=True
+        )
 
     async def create_receiver_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("receiver")
```

### Comparing `onvif-zeep-async-2.1.1/onvif/definition.py` & `onvif-zeep-async-2.1.2/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/exceptions.py` & `onvif-zeep-async-2.1.2/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/.events.wsdl.swn` & `onvif-zeep-async-2.1.2/onvif/wsdl/.events.wsdl.swn`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/addressing` & `onvif-zeep-async-2.1.2/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/display.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/envelope` & `onvif-zeep-async-2.1.2/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/events.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/media.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/search.wsdl` & `onvif-zeep-async-2.1.2/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/types.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/xml.xsd` & `onvif-zeep-async-2.1.2/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif/wsdl/xmlmime` & `onvif-zeep-async-2.1.2/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.1.1
+Version: 2.1.2
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-2.1.1/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-2.1.2/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/pylintrc` & `onvif-zeep-async-2.1.2/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/setup.py` & `onvif-zeep-async-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.1/tests/test.py` & `onvif-zeep-async-2.1.2/tests/test.py`

 * *Files identical despite different names*

