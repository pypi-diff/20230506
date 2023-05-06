# Comparing `tmp/avnet-scotty-2023.4.tar.gz` & `tmp/avnet-scotty-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avnet-scotty-2023.4.tar", last modified: Fri Apr 28 08:20:55 2023, max compression
+gzip compressed data, was "avnet-scotty-2023.4.1.tar", last modified: Sat May  6 11:07:01 2023, max compression
```

## Comparing `avnet-scotty-2023.4.tar` & `avnet-scotty-2023.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/
--rw-r--r--   0 root         (0) root         (0)    32879 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    18391 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18093 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/avnet_scotty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18391 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/bumper/
--rw-r--r--   0 root         (0) root         (0)      110 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/bumper/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4006 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/bumper/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     6703 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scotty
--rwxr-xr-x   0 root         (0) root         (0)     1580 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scotty-runqemu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      811 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scripts/vm_bundle.sh
--rw-r--r--   0 root         (0) root         (0)     1137 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scripts/vm_create.sh.template
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/
+-rw-r--r--   0 root         (0) root         (0)    32879 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    18967 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18667 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/avnet_scotty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18967 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/bumper/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/bumper/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4006 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/bumper/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6698 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scotty
+-rwxr-xr-x   0 root         (0) root         (0)     1580 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scotty-runqemu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      811 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scripts/vm_bundle.sh
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scripts/vm_create.sh.template
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/setup.py
```

### Comparing `avnet-scotty-2023.4/LICENSE` & `avnet-scotty-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4/PKG-INFO` & `avnet-scotty-2023.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.4
+Version: 2023.4.1
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -65,14 +65,29 @@
 
 .. note:: Remove the following paragraph once the BSP is open-sourced.
 
 To allow ``scotty`` to download the associated docker image, you will need to run
 a docker login command, as documented on
 `<https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry#authenticating-to-the-container-registry>`_
 
+Running scotty on a different docker image
+------------------------------------------
+
+By default scotty will use the corresponding version of the `scotty docker image <https://github.com/orgs/avnet-embedded/packages/container/package/scotty>`_.
+To use a different docker image run::
+
+  $ SCOTTY_DOCKER_IMAGE=<image> scotty ...
+
+e.g. to use the latest development version::
+
+  $ SCOTTY_DOCKER_IMAGE="ghcr.io/avnet-embedded/simplecore-tools:kirkstone" scotty ...
+
+to use a different release::
+
+  $ SCOTTY_DOCKER_IMAGE="ghcr.io/avnet-embedded/scotty:<release tag>" scotty ...
 
 Scotty subcommands
 ------------------
 
 Several commands are supported by Scotty, with different goals:
   - ``update``: download or update the Yocto sources. Will be triggered
     implicitly with default parameters if no sources are found.
```

### Comparing `avnet-scotty-2023.4/README.rst` & `avnet-scotty-2023.4.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,29 @@
 
 .. note:: Remove the following paragraph once the BSP is open-sourced.
 
 To allow ``scotty`` to download the associated docker image, you will need to run
 a docker login command, as documented on
 `<https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry#authenticating-to-the-container-registry>`_
 
+Running scotty on a different docker image
+------------------------------------------
+
+By default scotty will use the corresponding version of the `scotty docker image <https://github.com/orgs/avnet-embedded/packages/container/package/scotty>`_.
+To use a different docker image run::
+
+  $ SCOTTY_DOCKER_IMAGE=<image> scotty ...
+
+e.g. to use the latest development version::
+
+  $ SCOTTY_DOCKER_IMAGE="ghcr.io/avnet-embedded/simplecore-tools:kirkstone" scotty ...
+
+to use a different release::
+
+  $ SCOTTY_DOCKER_IMAGE="ghcr.io/avnet-embedded/scotty:<release tag>" scotty ...
 
 Scotty subcommands
 ------------------
 
 Several commands are supported by Scotty, with different goals:
   - ``update``: download or update the Yocto sources. Will be triggered
     implicitly with default parameters if no sources are found.
```

### Comparing `avnet-scotty-2023.4/avnet_scotty.egg-info/PKG-INFO` & `avnet-scotty-2023.4.1/avnet_scotty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.4
+Version: 2023.4.1
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -65,14 +65,29 @@
 
 .. note:: Remove the following paragraph once the BSP is open-sourced.
 
 To allow ``scotty`` to download the associated docker image, you will need to run
 a docker login command, as documented on
 `<https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry#authenticating-to-the-container-registry>`_
 
+Running scotty on a different docker image
+------------------------------------------
+
+By default scotty will use the corresponding version of the `scotty docker image <https://github.com/orgs/avnet-embedded/packages/container/package/scotty>`_.
+To use a different docker image run::
+
+  $ SCOTTY_DOCKER_IMAGE=<image> scotty ...
+
+e.g. to use the latest development version::
+
+  $ SCOTTY_DOCKER_IMAGE="ghcr.io/avnet-embedded/simplecore-tools:kirkstone" scotty ...
+
+to use a different release::
+
+  $ SCOTTY_DOCKER_IMAGE="ghcr.io/avnet-embedded/scotty:<release tag>" scotty ...
 
 Scotty subcommands
 ------------------
 
 Several commands are supported by Scotty, with different goals:
   - ``update``: download or update the Yocto sources. Will be triggered
     implicitly with default parameters if no sources are found.
```

### Comparing `avnet-scotty-2023.4/bumper/__main__.py` & `avnet-scotty-2023.4.1/bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4/scotty` & `avnet-scotty-2023.4.1/scotty`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 	TERM \
 	UBOOT_ENV_VARS \
 	"
 # SCOTTY_FEATURES_LAYERS REPO_URL SCOTTY_MACHINE_DIR BUILDDIR
 declare -r scotty_whitelist=${SCOTTY_WHITELIST:-${scotty_whitelist_default}}
 
 if [ "${SCOTTY_DOCKER_IMAGE:-1}" == "1" ]; then
-    declare -r docker_default_image="ghcr.io/avnet-embedded/simplecore-tools:2023.4"
+    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:kirkstone"
 else
     declare -r docker_default_image="${SCOTTY_DOCKER_IMAGE}"
 fi
 
-export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.4"
+export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.4.1"
 export SCOTTY_DEFAULT_MANIFEST_NAME="default-release.xml"
 
 debug() {
 	if [ "${SCOTTY_DEBUG:-0}" == "1" ]; then
 		echo -e "\033[1;38m${*}\033[0m"
 	fi
 }
```

### Comparing `avnet-scotty-2023.4/scotty-runqemu` & `avnet-scotty-2023.4.1/scotty-runqemu`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4/scripts/vm_bundle.sh` & `avnet-scotty-2023.4.1/scripts/vm_bundle.sh`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4/scripts/vm_create.sh.template` & `avnet-scotty-2023.4.1/scripts/vm_create.sh.template`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4/setup.py` & `avnet-scotty-2023.4.1/setup.py`

 * *Files identical despite different names*

