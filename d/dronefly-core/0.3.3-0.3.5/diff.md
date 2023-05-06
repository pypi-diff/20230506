# Comparing `tmp/dronefly_core-0.3.3.tar.gz` & `tmp/dronefly_core-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.3.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.5.tar", max compression
```

## Comparing `dronefly_core-0.3.3.tar` & `dronefly_core-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0    55577 2022-05-23 14:14:52.620333 dronefly_core-0.3.3/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.3/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.3/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.3/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0      619 2023-01-29 11:28:22.518452 dronefly_core-0.3.3/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     2015 2023-02-27 18:46:48.109234 dronefly_core-0.3.3/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.3/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0       78 2022-05-23 14:14:52.620333 dronefly_core-0.3.3/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0     2183 2023-02-27 18:46:48.109234 dronefly_core-0.3.3/dronefly/core/formatters/discord.py
--rw-r--r--   0        0        0    15019 2023-02-27 18:46:48.109234 dronefly_core-0.3.3/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.3/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     2142 2023-02-10 14:20:58.613458 dronefly_core-0.3.3/dronefly/core/models/taxon.py
--rw-r--r--   0        0        0      127 2023-01-29 11:28:22.574452 dronefly_core-0.3.3/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.3/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3656 2023-02-11 09:58:55.005728 dronefly_core-0.3.3/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.3/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6332 2022-06-12 18:18:34.473328 dronefly_core-0.3.3/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.3/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.3/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0     6379 2023-02-18 14:18:27.838102 dronefly_core-0.3.3/dronefly/core/query/query.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.3/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      960 2022-05-23 16:01:58.043793 dronefly_core-0.3.3/dronefly/core/utils/decorators.py
--rw-r--r--   0        0        0      704 2023-02-27 18:43:38.733426 dronefly_core-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 dronefly_core-0.3.3/setup.py
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 dronefly_core-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.5/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.5/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.5/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.5/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.5/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     4734 2023-04-16 14:27:09.193332 dronefly_core-0.3.5/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.5/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.5/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.5/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    30581 2023-04-30 15:34:08.268856 dronefly_core-0.3.5/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.5/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.5/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.5/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.5/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3672 2023-03-06 21:18:23.821142 dronefly_core-0.3.5/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.5/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.5/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.5/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.5/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    19236 2023-04-16 13:38:29.366402 dronefly_core-0.3.5/dronefly/core/query/query.py
+-rw-r--r--   0        0        0      527 2023-04-22 12:12:03.306747 dronefly_core-0.3.5/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-06 10:34:27.666900 dronefly_core-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 dronefly_core-0.3.5/PKG-INFO
```

### Comparing `dronefly_core-0.3.3/LICENSE` & `dronefly_core-0.3.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Format: https://www.debian.org/doc/packaging-manuals/copyright-format/1.0/
 Upstream-Name: dronefly-core
 Source: https://github.com/dronefly-garden/dronefly-core
 
 Files: *
-Copyright: 2019-2022 Ben Armstrong
+Copyright: 2019-2023 Ben Armstrong
 License: AGPL-3+
 
+Files: dronefly/core/formatters/generic.py
+Copyright:
+ 2019-2023 Ben Armstrong
+ 2015-2023 Rapptz
+License: AGPL-3+, and MIT
+
 License: AGPL-3+
                     GNU AFFERO GENERAL PUBLIC LICENSE
                        Version 3, 19 November 2007
  .
  Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
@@ -1091,7 +1097,28 @@
  without limitation, in connection with any unauthorized modifications
  to any of its public licenses or any other arrangements,
  understandings, or agreements concerning use of licensed material. For
  the avoidance of doubt, this paragraph does not form part of the public
  licenses.
  .
  Creative Commons may be contacted at creativecommons.org.
+
+License: MIT
+ The MIT License (MIT)
+ .
+ Copyright (c) 2015-present Rapptz
+ .
+ Permission is hereby granted, free of charge, to any person obtaining a
+ copy of this software and associated documentation files (the "Software"),
+ to deal in the Software without restriction, including without limitation
+ the rights to use, copy, modify, merge, publish, distribute, sublicense,
+ and/or sell copies of the Software, and to permit persons to whom the
+ Software is furnished to do so, subject to the following conditions:
+ The above copyright notice and this permission notice shall be included in
+ all copies or substantial portions of the Software.
+ THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+ OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+ FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+ AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+ LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+ FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+ DEALINGS IN THE SOFTWARE.
```

### Comparing `dronefly_core-0.3.3/README.md` & `dronefly_core-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.3/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.5/dronefly/core/parsers/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     # excluded in order to match only actual unknowns (Bacteria, Archaea, & Viruses):
     "unknown": {"opt": ["iconic_taxa=unknown", "without_taxon_id=67333,151817,131236"]},
     "waspsonly": {"of": "apocrita", "opt": ["without_taxon_id=47336,630955"]},
     "mothsonly": {"of": "lepidoptera", "opt": ["without_taxon_id=47224"]},
     "herps": {"opt": ["taxon_ids=20978,26036"]},
     "lichenish": {
         "opt": [
-            "taxon_ids=152028,942664,791197,54743,152030,175541,127378,117881,117869",
-            "without_taxon_id=352459",
+            "taxon_ids=152028,54743,152030,175541,127378,117881,117869,175246",
+            "without_taxon_id=372831,1040687,1040689,352459",
         ]
     },
     "nonflowering": {
         "of": "plantae",
         "opt": ["without_taxon_id=47125"],
     },
     "nonvascular": {
```

### Comparing `dronefly_core-0.3.3/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.5/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.3/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.5/dronefly/core/parsers/unixlike.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import re
 from typing import Optional
 
 import shlex
 import dateparser
 
-from dronefly.core.models.taxon import RANK_EQUIVALENTS
+from dronefly.core.constants import RANK_EQUIVALENTS
 from dronefly.core.query.query import Query, TaxonQuery
 from dronefly.core.parsers.constants import ARGPARSE_ARGS
 from dronefly.core.parsers.url import PAT_TAXON_LINK
 
 
 class NoExitParser(argparse.ArgumentParser):
     """Handle default error as RuntimeError, not sys.exit.
```

### Comparing `dronefly_core-0.3.3/dronefly/core/parsers/url.py` & `dronefly_core-0.3.5/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.3/pyproject.toml` & `dronefly_core-0.3.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 exclude_dirs = ["tests"]
 
 [tool.flake8]
 max-line-length = 100
 
 [tool.poetry]
 name = "dronefly-core"
-version = "0.3.3"
+version = "0.3.5"
 description = "Core dronefly components"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
 	{ include = "dronefly/core" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-pyinaturalist = ">=0.18,<0.19"
+pyinaturalist = ">=0.18,<0.20"
 dateparser = "^1.1.1"
 inflect = "^5.3.0"
 rich = ">=10.9,<14"
 attrs = ">=21.2"
+html2markdown = "^0.1.7"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 pytest-mock = "^3.10.0"
 pylint = "^2.10.2"
 pytest-asyncio = "^0.20.3"
```

### Comparing `dronefly_core-0.3.3/PKG-INFO` & `dronefly_core-0.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.3
+Version: 0.3.5
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=21.2)
 Requires-Dist: dateparser (>=1.1.1,<2.0.0)
+Requires-Dist: html2markdown (>=0.1.7,<0.2.0)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
-Requires-Dist: pyinaturalist (>=0.18,<0.19)
+Requires-Dist: pyinaturalist (>=0.18,<0.20)
 Requires-Dist: rich (>=10.9,<14)
 Description-Content-Type: text/markdown
 
 # Dronefly core
 
 This is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)
 Discord bot's core components. We're not yet making version guarantees until
```

