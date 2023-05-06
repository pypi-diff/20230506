# Comparing `tmp/nats_nsc-0.1.1.tar.gz` & `tmp/nats_nsc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats_nsc-0.1.1.tar", last modified: Fri May  5 09:15:43 2023, max compression
+gzip compressed data, was "nats_nsc-0.2.0.tar", last modified: Sat May  6 11:42:52 2023, max compression
```

## Comparing `nats_nsc-0.1.1.tar` & `nats_nsc-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/LICENSE
--rw-r--r--   0        0        0      191 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/README.md
--rw-r--r--   0        0        0      516 2023-05-05 09:15:43.725042 nats_nsc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3460 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/src/nats_nsc/__init__.py
--rw-r--r--   0        0        0     4460 2023-05-05 09:15:21.904690 nats_nsc-0.1.1/src/nats_nsc/nsc_utils.py
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 nats_nsc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 18:34:12.009002 nats_nsc-0.2.0/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-04 19:38:27.273447 nats_nsc-0.2.0/README.md
+-rw-r--r--   0        0        0      730 2023-05-06 11:42:52.113360 nats_nsc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2770 2023-05-05 14:27:21.654699 nats_nsc-0.2.0/src/nats_nsc/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-05 14:27:03.640871 nats_nsc-0.2.0/src/nats_nsc/common.py
+-rw-r--r--   0        0        0     5933 2023-05-05 14:30:33.673820 nats_nsc-0.2.0/src/nats_nsc/nsc_utils.py
+-rw-r--r--   0        0        0       68 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/.gitignore
+-rw-r--r--   0        0        0     1073 2023-05-05 09:44:07.272634 nats_nsc-0.2.0/tests/nsc_workdir/creds/nats-nsc-testing/SYS/sys.creds
+-rw-r--r--   0        0        0      989 2023-05-05 09:44:07.275634 nats_nsc-0.2.0/tests/nsc_workdir/creds/nats-nsc-testing/nats-nsc-testing/nats-nsc-testing.creds
+-rw-r--r--   0        0        0       58 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/keys/A/BH/ABHCY75MEEWFP5UNOOU67I274H3AZXFYYLS5H52CWHOE5AAXWXJTFOPU.nk
+-rw-r--r--   0        0        0       58 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/keys/A/BP/ABPQC72WINWR73PDSIC2XWNXUD7FOVXEKRRCKVJMFP3BTL5CPDBUGXTT.nk
+-rw-r--r--   0        0        0       58 2023-05-05 09:44:07.273634 nats_nsc-0.2.0/tests/nsc_workdir/keys/A/DD/ADDMOZZDAAU5LB4UML6N2QLIVCGXLEIYZZ5TT4YJCUKQT2FQIE25BZAG.nk
+-rw-r--r--   0        0        0       71 2023-05-05 14:35:54.867681 nats_nsc-0.2.0/tests/nsc_workdir/keys/DO_NOT_USE
+-rw-r--r--   0        0        0       58 2023-05-05 09:44:07.273634 nats_nsc-0.2.0/tests/nsc_workdir/keys/O/CC/OCCPKPFZ6DBHOKSJP4HXYPJE6Q5IFXKDOBYX4OOG7AUI5N5CW4VN3IP5.nk
+-rw-r--r--   0        0        0       58 2023-05-05 09:44:07.271634 nats_nsc-0.2.0/tests/nsc_workdir/keys/U/CO/UCORDZHQ2OEOFJUPTWF7LQCD4LT76YJVUKS7NLSX4BPAHZCGUYKPHAAT.nk
+-rw-r--r--   0        0        0       58 2023-05-05 09:44:07.275634 nats_nsc-0.2.0/tests/nsc_workdir/keys/U/DZ/UDZBHCCXJREZRPMRHZFEBNF6TTOVYUMB4J36GM6UJUQUJMRC5GBZ5BLG.nk
+-rw-r--r--   0        0        0       75 2023-05-05 09:44:07.268634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/.nsc
+-rw-r--r--   0        0        0     1582 2023-05-05 09:44:07.270634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/SYS.jwt
+-rw-r--r--   0        0        0      646 2023-05-05 09:44:07.271634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/SYS/users/sys.jwt
+-rw-r--r--   0        0        0      745 2023-05-05 09:44:07.274634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      562 2023-05-05 09:44:07.275634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/accounts/nats-nsc-testing/users/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      668 2023-05-05 09:44:07.272634 nats_nsc-0.2.0/tests/nsc_workdir/nats-nsc-testing/nats-nsc-testing.jwt
+-rw-r--r--   0        0        0      175 2023-05-05 09:44:07.274634 nats_nsc-0.2.0/tests/nsc_workdir/nsc.json
+-rw-r--r--   0        0        0     1412 2023-05-05 14:32:48.745494 nats_nsc-0.2.0/tests/test_setup.py
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 nats_nsc-0.2.0/PKG-INFO
```

### Comparing `nats_nsc-0.1.1/LICENSE` & `nats_nsc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nats_nsc-0.1.1/src/nats_nsc/__init__.py` & `nats_nsc-0.2.0/src/nats_nsc/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,71 @@
-import base64
-import json
 import os
-import shutil
+import typing as ty
 import tempfile
-import typing
-from dataclasses import dataclass
-
-from nats_nsc import nsc_utils
 
+from nats_nsc import nsc_utils, common
 
 _DEFAULT_NSC_PATH = "nsc"
 
-@dataclass
-class Operator():
-    name: str
-    jwt_path: str
-    pub_key: str
-    jwt_payload: typing.Dict[str, typing.Any]
-
-@dataclass
-class Account():
-    name: str
-    jwt_path: str
-    pub_key: str
-    has_priv_key: bool
-
-class Credential():
-    def __init__(self, payload:str) -> None:
-        self._payload = payload
-    
-    @property
-    def payload(self) -> str:
-        return self._payload
-    
-    @property
-    def jwt(self) -> str:
-        payload_splitted = self._payload.split('\n')
-        jwt_line_start = payload_splitted.index('-----BEGIN NATS ACCOUNT JWT-----')
-        jwt_line_end = payload_splitted.index('-----END NATS ACCOUNT JWT-----')
-        return '\n'.join(payload_splitted[jwt_line_start+1:jwt_line_end])
-
-    @property
-    def nkey(self) -> str:
-        payload_splitted = self._payload.split('\n')
-        nkey_line_start = payload_splitted.index('-----BEGIN USER NKEY SEED-----')
-        nkey_line_end = payload_splitted.index('-----END USER NKEY SEED-----')
-        return '\n'.join(payload_splitted[nkey_line_start+1:nkey_line_end])
 
 class Context():
     '''Base context for nsc-py, including working directory and nsc binary path.'''
 
-    def __init__(self, nsc_path: typing.Optional[str] = None):
-        self._nsc_path = nsc_path or _DEFAULT_NSC_PATH
-        if not nsc_utils.verify_binary(self._nsc_path):
+    @classmethod
+    async def async_factory(cls, nsc_path: ty.Optional[str] = None) -> 'Context':
+        '''Create a context asynchronously.'''
+
+        _nsc_path = nsc_path or _DEFAULT_NSC_PATH
+        if not await nsc_utils.verify_binary(_nsc_path):
             if nsc_path is None:
                 raise ValueError("nsc binary not found in PATH")
             else:
-                raise ValueError(f"Invalid nsc binary path: {self._nsc_path}")
-        self.work_dir = tempfile.mkdtemp(prefix='nsc-py-')
+                raise ValueError(f"Invalid nsc binary path: {_nsc_path}")
+        work_dir = tempfile.TemporaryDirectory(prefix='nsc-py-')
+        ctx = cls(work_dir, _nsc_path)
+        return ctx
+
+    def __init__(self, work_dir: tempfile.TemporaryDirectory, nsc_path: str):
+        self._nsc_path = nsc_path
+        self.work_dir = work_dir
         self.operators = {}
         self.accounts = {}
 
-    @classmethod
-    def _decode_jwt_payload(cls, jwt: str) -> dict:
-        '''Decode JWT payload.'''
-        try:
-            return json.loads(base64.b64decode(jwt.split('.')[1]))
-        except Exception:
-            raise ValueError("Invalid JWT")
-    
-    def add_operator(self, jwt: str) -> Operator:
-        payload = self._decode_jwt_payload(jwt)
+    async def add_operator(self, jwt_token: str) -> common.Operator:
+        payload = common.decode_jwt_payload(jwt_token)
         if payload['nats']['type'] != 'operator':
             raise ValueError("Invalid JWT type")
-        nsc_utils.load_operator(self._nsc_path, self.work_dir, jwt)
+        await nsc_utils.load_operator(self._nsc_path, self.work_dir.name, jwt_token)
         op_name = payload['name']
-        operator = Operator(
+        operator = common.Operator(
             name=op_name,
-            jwt_path=os.path.join(self.work_dir, f"{op_name}/{op_name}.jwt"),
+            jwt_path=os.path.join(self.work_dir.name, f"{op_name}/{op_name}.jwt"),
             pub_key=payload['sub'],
             jwt_payload=payload
         )
         self.operators[op_name] = operator
         return operator
 
-    def add_account(self, jwt: str, priv_key: str) -> Account:
-        payload = self._decode_jwt_payload(jwt)
+    async def add_account(self, jwt_token: str, operator: common.Operator,
+                          priv_key: ty.Optional[str] = None) -> common.Account:
+        payload = common.decode_jwt_payload(jwt_token)
         if payload['nats']['type'] != 'account':
             raise ValueError("Invalid JWT type")
         if priv_key is not None:
-            nsc_utils.load_key(self._nsc_path, self.work_dir, priv_key)
+            await nsc_utils.load_key(self._nsc_path, self.work_dir.name, priv_key)
         acc_name = payload['name']
-        nsc_utils.load_account(self.work_dir, jwt, acc_name)
-        account = Account(
+        await nsc_utils.load_account(self.work_dir.name, jwt_token, operator, acc_name)
+        account = common.Account(
             name=acc_name,
-            jwt_path=os.path.join(self.work_dir, f"accounts/{acc_name}/{acc_name}.jwt"),
+            operator_name=operator.name,
+            jwt_path=os.path.join(self.work_dir.name, f"accounts/{acc_name}/{acc_name}.jwt"),
             pub_key=payload['sub'],
             has_priv_key=priv_key is not None
         )
         self.accounts[acc_name] = account
         return account
 
+    async def create_user(self, user_name: str, account: common.Account) -> common.Credential:
+        return await nsc_utils.create_user(self._nsc_path, self.work_dir.name, user_name, account)
 
     def __del__(self):
-        shutil.rmtree(self.work_dir, ignore_errors=True)
+        self.work_dir.cleanup()
```

