# Comparing `tmp/nats_nsc-0.2.0.tar.gz` & `tmp/nats_nsc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_nsc-0.2.0.tar", last modified: Sat May  6 11:42:52 2023, max compression
+gzip compressed data, was "nats_nsc-0.2.1.tar", last modified: Sat May  6 16:14:08 2023, max compression
```

## Comparing `nats_nsc-0.2.0.tar` & `nats_nsc-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-05-04 18:34:12.009002 nats_nsc-0.2.0/LICENSE
--rw-r--r--   0        0        0      191 2023-05-04 19:38:27.273447 nats_nsc-0.2.0/README.md
--rw-r--r--   0        0        0      730 2023-05-06 11:42:52.113360 nats_nsc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2770 2023-05-05 14:27:21.654699 nats_nsc-0.2.0/src/nats_nsc/__init__.py
--rw-r--r--   0        0        0     1708 2023-05-05 14:27:03.640871 nats_nsc-0.2.0/src/nats_nsc/common.py
--rw-r--r--   0        0        0     5933 2023-05-05 14:30:33.673820 nats_nsc-0.2.0/src/nats_nsc/nsc_utils.py
--rw-r--r--   0        0        0       68 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/.gitignore
--rw-r--r--   0        0        0     1073 2023-05-05 09:44:07.272634 nats_nsc-0.2.0/tests/nsc_workdir/creds/nats-nsc-testing/SYS/sys.creds
--rw-r--r--   0        0        0      989 2023-05-05 09:44:07.275634 nats_nsc-0.2.0/tests/nsc_workdir/creds/nats-nsc-testing/nats-nsc-testing/nats-nsc-testing.creds
--rw-r--r--   0        0        0       58 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/keys/A/BH/ABHCY75MEEWFP5UNOOU67I274H3AZXFYYLS5H52CWHOE5AAXWXJTFOPU.nk
--rw-r--r--   0        0        0       58 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/keys/A/BP/ABPQC72WINWR73PDSIC2XWNXUD7FOVXEKRRCKVJMFP3BTL5CPDBUGXTT.nk
--rw-r--r--   0        0        0       58 2023-05-05 09:44:07.273634 nats_nsc-0.2.0/tests/nsc_workdir/keys/A/DD/ADDMOZZDAAU5LB4UML6N2QLIVCGXLEIYZZ5TT4YJCUKQT2FQIE25BZAG.nk
--rw-r--r--   0        0        0       71 2023-05-05 14:35:54.867681 nats_nsc-0.2.0/tests/nsc_workdir/keys/DO_NOT_USE
--rw-r--r--   0        0        0       58 2023-05-05 09:44:07.273634 nats_nsc-0.2.0/tests/nsc_workdir/keys/O/CC/OCCPKPFZ6DBHOKSJP4HXYPJE6Q5IFXKDOBYX4OOG7AUI5N5CW4VN3IP5.nk
--rw-r--r--   0        0        0       58 2023-05-05 09:44:07.271634 nats_nsc-0.2.0/tests/nsc_workdir/keys/U/CO/UCORDZHQ2OEOFJUPTWF7LQCD4LT76YJVUKS7NLSX4BPAHZCGUYKPHAAT.nk
--rw-r--r--   0        0        0       58 2023-05-05 09:44:07.275634 nats_nsc-0.2.0/tests/nsc_workdir/keys/U/DZ/UDZBHCCXJREZRPMRHZFEBNF6TTOVYUMB4J36GM6UJUQUJMRC5GBZ5BLG.nk
--rw-r--r--   0        0        0       75 2023-05-05 09:44:07.268634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/.nsc
--rw-r--r--   0        0        0     1582 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
--rw-r--r--   0        0        0      646 2023-05-05 09:44:07.271634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
--rw-r--r--   0        0        0      745 2023-05-05 09:44:07.274634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      562 2023-05-05 09:44:07.275634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      668 2023-05-05 09:44:07.272634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
--rw-r--r--   0        0        0      175 2023-05-05 09:44:07.274634 nats_nsc-0.2.0/tests/nsc_workdir/nsc.json
--rw-r--r--   0        0        0     1412 2023-05-05 14:32:48.745494 nats_nsc-0.2.0/tests/test_setup.py
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 nats_nsc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/README.md
+-rw-r--r--   0        0        0      730 2023-05-06 16:14:08.531966 nats_nsc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4489 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/src/nats_nsc/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/src/nats_nsc/common.py
+-rw-r--r--   0        0        0     6008 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/src/nats_nsc/nsc_utils.py
+-rw-r--r--   0        0        0       68 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/.gitignore
+-rw-r--r--   0        0        0       71 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/keys/DO_NOT_USE
+-rw-r--r--   0        0        0       75 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/.nsc
+-rw-r--r--   0        0        0     1582 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
+-rw-r--r--   0        0        0      646 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
+-rw-r--r--   0        0        0      745 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      562 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      668 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      175 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/nsc_workdir/nsc.json
+-rw-r--r--   0        0        0     1412 2023-05-06 16:13:42.942248 nats_nsc-0.2.1/tests/test_setup.py
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 nats_nsc-0.2.1/PKG-INFO
```

### Comparing `nats_nsc-0.2.0/LICENSE` & `nats_nsc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.0/pyproject.toml` & `nats_nsc-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [tool.pytest.ini_options]
 pythonpath = [
     "src/",
 ]
 
 [project]
 name = "nats-nsc"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python wrapper for nsc, nats credential manager"
 authors = [
     { name = "Mikołaj Nowak", email = "12396461+m3nowak@users.noreply.github.com" },
 ]
 dependencies = [
     "pyJWT~=2.6.0",
     "aiofiles~=23.1.0",
```

### Comparing `nats_nsc-0.2.0/src/nats_nsc/common.py` & `nats_nsc-0.2.1/src/nats_nsc/common.py`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.0/src/nats_nsc/nsc_utils.py` & `nats_nsc-0.2.1/src/nats_nsc/nsc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,29 +68,31 @@
     '''Convert timedelta to precise nats duration string.'''
     return f"{td.days*24*60 + td.seconds}s{td.microseconds//1000}ms"
 
 
 async def create_user(nsc_path: str, nsc_work_dir: str,
                       user_name: str, account: common.Account,
                       allow_pub: ty.Optional[ty.List[str]] = None,
-                      allow_pub_response: int = 1,
+                      allow_pub_response: ty.Optional[int] = None,
                       allow_pubsub: ty.Optional[ty.List[str]] = None,
                       allow_sub: ty.Optional[ty.List[str]] = None,
                       bearer: bool = False,
                       deny_pub: ty.Optional[ty.List[str]] = None,
                       deny_pubsub: ty.Optional[ty.List[str]] = None,
                       deny_sub: ty.Optional[ty.List[str]] = None,
                       expiry: ty.Optional[timedelta] = None,
                       response_ttl: ty.Optional[timedelta] = None,
                       source_networks: ty.Optional[ty.List[str]] = None,
                       start: ty.Optional[timedelta] = None,
                       tag: ty.Optional[ty.List[str]] = None) -> common.Credential:
     '''Create user.'''
     args = [nsc_path, "-H", nsc_work_dir, 'add', 'user', '-a', shlex.quote(account.name), '-n', shlex.quote(
-        user_name), f'--allow-pub-response={allow_pub_response}']
+        user_name)]
+    if allow_pub_response is not None:
+        args.append(f'--allow-pub-response={allow_pub_response}')
     if allow_pub is not None:
         args += ['--allow-pub', shlex.quote(','.join(allow_pub))]
     if allow_pubsub is not None:
         args += ['--allow-pubsub', shlex.quote(','.join(allow_pubsub))]
     if allow_sub is not None:
         args += ['--allow-sub', shlex.quote(','.join(allow_sub))]
     if bearer:
```

### Comparing `nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt` & `nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt` & `nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt` & `nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt` & `nats_nsc-0.2.1/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.2.0/tests/test_setup.py` & `nats_nsc-0.2.1/tests/test_setup.py`

 * *Files identical despite different names*

