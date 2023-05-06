# Comparing `tmp/just-jobs-1.1.0.tar.gz` & `tmp/just_jobs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just-jobs-1.1.0.tar", max compression
+gzip compressed data, was "just_jobs-2.0.0.tar", last modified: Sat May  6 03:01:22 2023, max compression
```

## Comparing `just-jobs-1.1.0.tar` & `just_jobs-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1215 2022-05-18 18:43:55.927402 just-jobs-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      804 2022-05-18 19:17:55.015713 just-jobs-1.1.0/just_jobs/__init__.py
--rw-r--r--   0        0        0       72 2022-05-18 19:18:06.296313 just-jobs-1.1.0/just_jobs/brokers/__init__.py
--rw-r--r--   0        0        0     4319 2022-05-18 18:47:39.450443 just-jobs-1.1.0/just_jobs/brokers/base.py
--rw-r--r--   0        0        0     2944 2022-05-18 21:14:42.843494 just-jobs-1.1.0/just_jobs/brokers/redis.py
--rw-r--r--   0        0        0      439 2022-05-18 19:18:56.428267 just-jobs-1.1.0/just_jobs/errors.py
--rw-r--r--   0        0        0     4320 2022-05-18 19:17:51.255265 just-jobs-1.1.0/just_jobs/manager.py
--rw-r--r--   0        0        0        0 2021-07-24 20:17:02.002842 just-jobs-1.1.0/just_jobs/py.typed
--rw-r--r--   0        0        0     1322 2021-08-27 17:59:26.309811 just-jobs-1.1.0/LICENSE
--rw-r--r--   0        0        0      743 2022-05-18 20:25:51.798628 just-jobs-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3108 2022-05-18 21:02:08.437708 just-jobs-1.1.0/README.md
--rw-r--r--   0        0        0     3912 2022-05-18 21:16:25.430055 just-jobs-1.1.0/setup.py
--rw-r--r--   0        0        0     3990 2022-05-18 21:16:25.430055 just-jobs-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1683 2023-05-06 03:00:07.988141 just_jobs-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1462 2023-05-06 02:17:56.635972 just_jobs-2.0.0/LICENSE
+-rw-r--r--   0        0        0     7262 2023-05-06 02:17:56.820059 just_jobs-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2021-07-24 20:17:02.002842 just_jobs-2.0.0/just_jobs/py.typed
+-rw-r--r--   0        0        0     1043 2023-05-06 03:01:22.722490 just_jobs-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 18:43:21.184656 just_jobs-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-06 02:17:56.436966 just_jobs-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      848 2023-05-06 01:36:07.154826 just_jobs-2.0.0/tests/test_broker.py
+-rw-r--r--   0        0        0     2197 2023-05-06 02:17:56.437970 just_jobs-2.0.0/tests/test_job.py
+-rw-r--r--   0        0        0     1436 2023-05-06 01:36:07.156496 just_jobs-2.0.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1781 2023-05-06 01:36:07.157696 just_jobs-2.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0     7766 1970-01-01 00:00:00.000000 just_jobs-2.0.0/PKG-INFO
```

### Comparing `just-jobs-1.1.0/CHANGELOG.md` & `just_jobs-2.0.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.0.0] - 2023-05-05
+
+I discovered arq, and it does a lot of the same things I was hoping just-jobs would eventually support. Rather than remake the wheel, V2 is a complete rethinking and rewrite using arq as an engine.
+
+Some internal concepts are the same though:
+
+- Redis is the default broking service.
+- You can use both sync and async jobs.
+- Sync jobs are run in an executor to prevent event loop blocking.
+- Jobs are runnable if you don't want to delay it.
+
 ## [1.1.0] - 2022-05-18
 
 ### Changed
 
 - Replaced `aioredis` with asyncio `redis-py` and `hiredis`.
 - Replaced `pdoc3` with `pdoc`.
```

### Comparing `just-jobs-1.1.0/LICENSE` & `just_jobs-2.0.0/LICENSE`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-BSD 2-Clause License
+Copyright 2023 Elias Gabriel
 
-Copyright (c) 2021, Elias Gabriel
-All rights reserved.
+Redistribution and use in source and binary forms, with or without modification, are
+permitted provided that the following conditions are met:
 
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
+1. Redistributions of source code must retain the above copyright notice, this list of
+conditions and the following disclaimer.
 
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
+2. Redistributions in binary form must reproduce the above copyright notice, this list
+of conditions and the following disclaimer in the documentation and/or other materials
+provided with the distribution.
 
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
+3. Neither the name of the copyright holder nor the names of its contributors may be
+used to endorse or promote products derived from this software without specific prior
+written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL
+THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
+STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
+THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

