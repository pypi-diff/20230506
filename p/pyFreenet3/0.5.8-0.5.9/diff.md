# Comparing `tmp/pyFreenet3-0.5.8.tar.gz` & `tmp/pyFreenet3-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFreenet3-0.5.8.tar", last modified: Sat Apr  1 09:11:48 2023, max compression
+gzip compressed data, was "pyFreenet3-0.5.9.tar", last modified: Sat May  6 16:26:29 2023, max compression
```

## Comparing `pyFreenet3-0.5.8.tar` & `pyFreenet3-0.5.9.tar`

### file list

```diff
@@ -1,116 +1,124 @@
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/
--rw-r--r--   0 arne      (1000) users      (998)     3548 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/PKG-INFO
--rw-r--r--   0 arne      (1000) users      (998)     2276 2022-10-16 08:49:47.312056 pyFreenet3-0.5.8/README
--rwxr-xr-x   0 arne      (1000) users      (998)    92053 2023-01-09 15:53:30.647619 pyFreenet3-0.5.8/babcom_cli
--rwxr-xr-x   0 arne      (1000) users      (998)     3660 2019-09-23 19:31:28.509958 pyFreenet3-0.5.8/copyweb
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/fcp3/
--rw-r--r--   0 arne      (1000) users      (998)     1069 2019-09-23 20:41:59.857776 pyFreenet3-0.5.8/fcp3/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)     1565 2019-09-23 20:41:59.857776 pyFreenet3-0.5.8/fcp3/arguments.py
--rw-r--r--   0 arne      (1000) users      (998)    14319 2019-09-23 20:41:59.857776 pyFreenet3-0.5.8/fcp3/fproxyproxy.py
--rw-r--r--   0 arne      (1000) users      (998)    61714 2019-09-30 08:28:53.570626 pyFreenet3-0.5.8/fcp3/freenetfs.py
--rw-r--r--   0 arne      (1000) users      (998)     1618 2019-09-23 20:41:59.849776 pyFreenet3-0.5.8/fcp3/genkey.py
--rw-r--r--   0 arne      (1000) users      (998)     3809 2019-09-23 20:41:59.849776 pyFreenet3-0.5.8/fcp3/get.py
--rw-r--r--   0 arne      (1000) users      (998)     1754 2019-09-23 20:41:59.849776 pyFreenet3-0.5.8/fcp3/invertkey.py
--rw-r--r--   0 arne      (1000) users      (998)    13073 2019-09-30 08:28:58.842639 pyFreenet3-0.5.8/fcp3/names.py
--rw-r--r--   0 arne      (1000) users      (998)   117265 2023-04-01 09:08:20.631675 pyFreenet3-0.5.8/fcp3/node.py
--rw-r--r--   0 arne      (1000) users      (998)     8805 2019-09-23 20:41:59.837776 pyFreenet3-0.5.8/fcp3/pseudopythonparser.py
--rw-r--r--   0 arne      (1000) users      (998)     9101 2019-09-23 20:41:59.837776 pyFreenet3-0.5.8/fcp3/put.py
--rw-r--r--   0 arne      (1000) users      (998)     4005 2019-09-23 20:41:59.837776 pyFreenet3-0.5.8/fcp3/redirect.py
--rw-r--r--   0 arne      (1000) users      (998)    64207 2023-04-01 08:48:38.478449 pyFreenet3-0.5.8/fcp3/sitemgr.py
--rw-r--r--   0 arne      (1000) users      (998)    11102 2023-01-26 22:51:39.869134 pyFreenet3-0.5.8/fcp3/upload.py
--rw-r--r--   0 arne      (1000) users      (998)    19419 2019-09-23 20:41:59.833776 pyFreenet3-0.5.8/fcp3/xmlobject.py
--rw-r--r--   0 arne      (1000) users      (998)     6914 2019-09-23 20:41:59.833776 pyFreenet3-0.5.8/fcp3/xmlrpc.py
--rwxr-xr-x   0 arne      (1000) users      (998)       61 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fcpgenkey
--rwxr-xr-x   0 arne      (1000) users      (998)       57 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fcpget
--rwxr-xr-x   0 arne      (1000) users      (998)     1407 2021-12-14 10:40:52.926160 pyFreenet3-0.5.8/fcpgetdir
--rwxr-xr-x   0 arne      (1000) users      (998)       64 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fcpinvertkey
--rwxr-xr-x   0 arne      (1000) users      (998)       60 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fcpnames
--rwxr-xr-x   0 arne      (1000) users      (998)       58 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fcpput
--rwxr-xr-x   0 arne      (1000) users      (998)      865 2021-12-14 04:25:54.287295 pyFreenet3-0.5.8/fcpputdir
--rwxr-xr-x   0 arne      (1000) users      (998)       63 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fcpredirect
--rwxr-xr-x   0 arne      (1000) users      (998)       61 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fcpupload
--rwxr-xr-x   0 arne      (1000) users      (998)       66 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/fproxyproxy
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet3/
--rw-r--r--   0 arne      (1000) users      (998)       42 2019-09-23 20:41:59.000000 pyFreenet3-0.5.8/freenet3/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)    22370 2019-09-23 20:41:59.000000 pyFreenet3-0.5.8/freenet3/appdirs.py
--rw-r--r--   0 arne      (1000) users      (998)     9187 2023-01-09 15:06:51.563984 pyFreenet3-0.5.8/freenet3/spawn.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/
--rw-r--r--   0 arne      (1000) users      (998)       87 2019-09-23 20:41:59.697775 pyFreenet3-0.5.8/freenet_passlib_170/__init__.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/_setup/
--rw-r--r--   0 arne      (1000) users      (998)       76 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/_setup/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)     3109 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/_setup/docdist.py
--rw-r--r--   0 arne      (1000) users      (998)     2079 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/_setup/stamp.py
--rw-r--r--   0 arne      (1000) users      (998)    46485 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/apache.py
--rw-r--r--   0 arne      (1000) users      (998)     6973 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/apps.py
--rw-r--r--   0 arne      (1000) users      (998)   113740 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/context.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/crypto/
--rw-r--r--   0 arne      (1000) users      (998)       96 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/__init__.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/
--rw-r--r--   0 arne      (1000) users      (998)     6498 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)     6224 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/_gen_files.py
--rw-r--r--   0 arne      (1000) users      (998)    20414 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/base.py
--rw-r--r--   0 arne      (1000) users      (998)    37177 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/unrolled.py
--rw-r--r--   0 arne      (1000) users      (998)     6941 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/_md4.py
--rw-r--r--   0 arne      (1000) users      (998)    51938 2019-09-23 20:41:59.701775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/des.py
--rw-r--r--   0 arne      (1000) users      (998)    30957 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/digest.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/
--rw-r--r--   0 arne      (1000) users      (998)     6781 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)     8970 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/_builtin.py
--rw-r--r--   0 arne      (1000) users      (998)     4707 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/_gen_files.py
--rw-r--r--   0 arne      (1000) users      (998)     5731 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/_salsa.py
--rw-r--r--   0 arne      (1000) users      (998)    11612 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/exc.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/ext/
--rw-r--r--   0 arne      (1000) users      (998)        1 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/ext/__init__.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/ext/django/
--rw-r--r--   0 arne      (1000) users      (998)      240 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/ext/django/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)     1350 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/ext/django/models.py
--rw-r--r--   0 arne      (1000) users      (998)    47852 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/ext/django/utils.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/handlers/
--rw-r--r--   0 arne      (1000) users      (998)       98 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)    32125 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/argon2.py
--rw-r--r--   0 arne      (1000) users      (998)    42498 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/bcrypt.py
--rw-r--r--   0 arne      (1000) users      (998)    11505 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/cisco.py
--rw-r--r--   0 arne      (1000) users      (998)    22482 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/des_crypt.py
--rw-r--r--   0 arne      (1000) users      (998)     5512 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/digests.py
--rw-r--r--   0 arne      (1000) users      (998)    20267 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/django.py
--rw-r--r--   0 arne      (1000) users      (998)     7883 2019-09-23 20:41:59.705775 pyFreenet3-0.5.8/freenet_passlib_170/handlers/fshp.py
--rw-r--r--   0 arne      (1000) users      (998)    10289 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/ldap_digests.py
--rw-r--r--   0 arne      (1000) users      (998)    13802 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/md5_crypt.py
--rw-r--r--   0 arne      (1000) users      (998)    10188 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/misc.py
--rw-r--r--   0 arne      (1000) users      (998)     8578 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/mssql.py
--rw-r--r--   0 arne      (1000) users      (998)     4880 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/mysql.py
--rw-r--r--   0 arne      (1000) users      (998)     6787 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/oracle.py
--rw-r--r--   0 arne      (1000) users      (998)    19202 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/pbkdf2.py
--rw-r--r--   0 arne      (1000) users      (998)     4857 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/phpass.py
--rw-r--r--   0 arne      (1000) users      (998)     2334 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/postgres.py
--rw-r--r--   0 arne      (1000) users      (998)     1214 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/roundup.py
--rw-r--r--   0 arne      (1000) users      (998)    22659 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/scram.py
--rw-r--r--   0 arne      (1000) users      (998)    14278 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/scrypt.py
--rw-r--r--   0 arne      (1000) users      (998)     5920 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/sha1_crypt.py
--rw-r--r--   0 arne      (1000) users      (998)    21292 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/sha2_crypt.py
--rw-r--r--   0 arne      (1000) users      (998)    14017 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/sun_md5_crypt.py
--rw-r--r--   0 arne      (1000) users      (998)    12564 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/handlers/windows.py
--rw-r--r--   0 arne      (1000) users      (998)     4034 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/hash.py
--rw-r--r--   0 arne      (1000) users      (998)     3362 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/hosts.py
--rw-r--r--   0 arne      (1000) users      (998)    12922 2019-09-23 20:41:59.709776 pyFreenet3-0.5.8/freenet_passlib_170/ifc.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/passlib-misc/
--rw-r--r--   0 arne      (1000) users      (998)     6288 2019-09-23 20:41:59.725776 pyFreenet3-0.5.8/freenet_passlib_170/passlib-misc/setup.py
--rw-r--r--   0 arne      (1000) users      (998)    28376 2019-09-23 20:41:59.725776 pyFreenet3-0.5.8/freenet_passlib_170/pwd.py
--rw-r--r--   0 arne      (1000) users      (998)    21150 2019-09-23 20:41:59.725776 pyFreenet3-0.5.8/freenet_passlib_170/registry.py
--rw-r--r--   0 arne      (1000) users      (998)    72626 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/totp.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/utils/
--rw-r--r--   0 arne      (1000) users      (998)    36793 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)    31482 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/binary.py
-drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-04-01 09:11:48.075676 pyFreenet3-0.5.8/freenet_passlib_170/utils/compat/
--rw-r--r--   0 arne      (1000) users      (998)    13503 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/compat/__init__.py
--rw-r--r--   0 arne      (1000) users      (998)     8392 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/compat/_ordered_dict.py
--rw-r--r--   0 arne      (1000) users      (998)     7675 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/decor.py
--rw-r--r--   0 arne      (1000) users      (998)     2283 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/des.py
--rw-r--r--   0 arne      (1000) users      (998)   104189 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/handlers.py
--rw-r--r--   0 arne      (1000) users      (998)     1278 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/md4.py
--rw-r--r--   0 arne      (1000) users      (998)     6976 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/utils/pbkdf2.py
--rw-r--r--   0 arne      (1000) users      (998)     2687 2019-09-23 20:41:59.737776 pyFreenet3-0.5.8/freenet_passlib_170/win32.py
--rwxr-xr-x   0 arne      (1000) users      (998)    18189 2023-03-29 08:16:20.331209 pyFreenet3-0.5.8/freesitemgr
--rwxr-xr-x   0 arne      (1000) users      (998)     3320 2019-09-23 19:31:28.517957 pyFreenet3-0.5.8/pyNodeConfig
--rw-r--r--   0 arne      (1000) users      (998)       59 2021-04-02 09:53:44.858436 pyFreenet3-0.5.8/setup.cfg
--rwxr-xr-x   0 arne      (1000) users      (998)     2987 2023-04-01 09:09:19.730535 pyFreenet3-0.5.8/setup.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/
+-rw-r--r--   0 arne      (1000) users      (998)      208 2019-09-23 19:31:28.000000 pyFreenet3-0.5.9/AUTHORS
+-rw-r--r--   0 arne      (1000) users      (998)      395 2022-11-04 20:16:05.000000 pyFreenet3-0.5.9/COPYING
+-rw-r--r--   0 arne      (1000) users      (998)     1097 2019-09-23 19:31:28.000000 pyFreenet3-0.5.9/LICENSE_appdirs.txt
+-rw-r--r--   0 arne      (1000) users      (998)     3066 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/PKG-INFO
+-rw-r--r--   0 arne      (1000) users      (998)     2276 2022-10-16 08:49:47.000000 pyFreenet3-0.5.9/README
+-rwxr-xr-x   0 arne      (1000) users      (998)    92053 2023-01-09 15:53:30.000000 pyFreenet3-0.5.9/babcom_cli
+-rwxr-xr-x   0 arne      (1000) users      (998)     3660 2019-09-23 19:31:28.000000 pyFreenet3-0.5.9/copyweb
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/fcp3/
+-rw-r--r--   0 arne      (1000) users      (998)     1069 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)     1565 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/arguments.py
+-rw-r--r--   0 arne      (1000) users      (998)    14319 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/fproxyproxy.py
+-rw-r--r--   0 arne      (1000) users      (998)    61714 2019-09-30 08:28:53.000000 pyFreenet3-0.5.9/fcp3/freenetfs.py
+-rw-r--r--   0 arne      (1000) users      (998)     1618 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/genkey.py
+-rw-r--r--   0 arne      (1000) users      (998)     3809 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/get.py
+-rw-r--r--   0 arne      (1000) users      (998)     1754 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/invertkey.py
+-rw-r--r--   0 arne      (1000) users      (998)    13073 2019-09-30 08:28:58.000000 pyFreenet3-0.5.9/fcp3/names.py
+-rw-r--r--   0 arne      (1000) users      (998)   117265 2023-05-06 16:20:30.000000 pyFreenet3-0.5.9/fcp3/node.py
+-rw-r--r--   0 arne      (1000) users      (998)     8805 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/pseudopythonparser.py
+-rw-r--r--   0 arne      (1000) users      (998)     9101 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/put.py
+-rw-r--r--   0 arne      (1000) users      (998)     4005 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/redirect.py
+-rw-r--r--   0 arne      (1000) users      (998)    64666 2023-05-06 12:08:09.000000 pyFreenet3-0.5.9/fcp3/sitemgr.py
+-rw-r--r--   0 arne      (1000) users      (998)    11102 2023-01-26 22:51:39.000000 pyFreenet3-0.5.9/fcp3/upload.py
+-rw-r--r--   0 arne      (1000) users      (998)    19419 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/xmlobject.py
+-rw-r--r--   0 arne      (1000) users      (998)     6914 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcp3/xmlrpc.py
+-rwxr-xr-x   0 arne      (1000) users      (998)       61 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcpgenkey
+-rwxr-xr-x   0 arne      (1000) users      (998)       57 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcpget
+-rwxr-xr-x   0 arne      (1000) users      (998)     1407 2021-12-14 10:40:52.000000 pyFreenet3-0.5.9/fcpgetdir
+-rwxr-xr-x   0 arne      (1000) users      (998)       64 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcpinvertkey
+-rwxr-xr-x   0 arne      (1000) users      (998)       60 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcpnames
+-rwxr-xr-x   0 arne      (1000) users      (998)       58 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcpput
+-rwxr-xr-x   0 arne      (1000) users      (998)      865 2021-12-14 04:25:54.000000 pyFreenet3-0.5.9/fcpputdir
+-rwxr-xr-x   0 arne      (1000) users      (998)       63 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcpredirect
+-rwxr-xr-x   0 arne      (1000) users      (998)       61 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fcpupload
+-rwxr-xr-x   0 arne      (1000) users      (998)       66 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/fproxyproxy
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/freenet3/
+-rw-r--r--   0 arne      (1000) users      (998)       42 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet3/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)    22370 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet3/appdirs.py
+-rw-r--r--   0 arne      (1000) users      (998)     9187 2023-01-09 15:06:51.000000 pyFreenet3-0.5.9/freenet3/spawn.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/freenet_passlib_170/
+-rw-r--r--   0 arne      (1000) users      (998)       87 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/__init__.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/freenet_passlib_170/_setup/
+-rw-r--r--   0 arne      (1000) users      (998)       76 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/_setup/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)     3109 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/_setup/docdist.py
+-rw-r--r--   0 arne      (1000) users      (998)     2079 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/_setup/stamp.py
+-rw-r--r--   0 arne      (1000) users      (998)    46485 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/apache.py
+-rw-r--r--   0 arne      (1000) users      (998)     6973 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/apps.py
+-rw-r--r--   0 arne      (1000) users      (998)   113740 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/context.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/freenet_passlib_170/crypto/
+-rw-r--r--   0 arne      (1000) users      (998)       96 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/__init__.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/
+-rw-r--r--   0 arne      (1000) users      (998)     6498 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)     6224 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/_gen_files.py
+-rw-r--r--   0 arne      (1000) users      (998)    20414 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/base.py
+-rw-r--r--   0 arne      (1000) users      (998)    37177 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/unrolled.py
+-rw-r--r--   0 arne      (1000) users      (998)     6941 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/_md4.py
+-rw-r--r--   0 arne      (1000) users      (998)    51938 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/des.py
+-rw-r--r--   0 arne      (1000) users      (998)    30957 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/digest.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/
+-rw-r--r--   0 arne      (1000) users      (998)     6781 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)     8970 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/_builtin.py
+-rw-r--r--   0 arne      (1000) users      (998)     4707 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/_gen_files.py
+-rw-r--r--   0 arne      (1000) users      (998)     5731 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/_salsa.py
+-rw-r--r--   0 arne      (1000) users      (998)    11612 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/exc.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.683771 pyFreenet3-0.5.9/freenet_passlib_170/ext/
+-rw-r--r--   0 arne      (1000) users      (998)        1 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/ext/__init__.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/freenet_passlib_170/ext/django/
+-rw-r--r--   0 arne      (1000) users      (998)      240 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/ext/django/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)     1350 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/ext/django/models.py
+-rw-r--r--   0 arne      (1000) users      (998)    47852 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/ext/django/utils.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/freenet_passlib_170/handlers/
+-rw-r--r--   0 arne      (1000) users      (998)       98 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)    32125 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/argon2.py
+-rw-r--r--   0 arne      (1000) users      (998)    42498 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/bcrypt.py
+-rw-r--r--   0 arne      (1000) users      (998)    11505 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/cisco.py
+-rw-r--r--   0 arne      (1000) users      (998)    22482 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/des_crypt.py
+-rw-r--r--   0 arne      (1000) users      (998)     5512 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/digests.py
+-rw-r--r--   0 arne      (1000) users      (998)    20267 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/django.py
+-rw-r--r--   0 arne      (1000) users      (998)     7883 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/fshp.py
+-rw-r--r--   0 arne      (1000) users      (998)    10289 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/ldap_digests.py
+-rw-r--r--   0 arne      (1000) users      (998)    13802 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/md5_crypt.py
+-rw-r--r--   0 arne      (1000) users      (998)    10188 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/misc.py
+-rw-r--r--   0 arne      (1000) users      (998)     8578 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/mssql.py
+-rw-r--r--   0 arne      (1000) users      (998)     4880 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/mysql.py
+-rw-r--r--   0 arne      (1000) users      (998)     6787 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/oracle.py
+-rw-r--r--   0 arne      (1000) users      (998)    19202 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/pbkdf2.py
+-rw-r--r--   0 arne      (1000) users      (998)     4857 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/phpass.py
+-rw-r--r--   0 arne      (1000) users      (998)     2334 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/postgres.py
+-rw-r--r--   0 arne      (1000) users      (998)     1214 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/roundup.py
+-rw-r--r--   0 arne      (1000) users      (998)    22659 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/scram.py
+-rw-r--r--   0 arne      (1000) users      (998)    14278 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/scrypt.py
+-rw-r--r--   0 arne      (1000) users      (998)     5920 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/sha1_crypt.py
+-rw-r--r--   0 arne      (1000) users      (998)    21292 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/sha2_crypt.py
+-rw-r--r--   0 arne      (1000) users      (998)    14017 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/sun_md5_crypt.py
+-rw-r--r--   0 arne      (1000) users      (998)    12564 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/handlers/windows.py
+-rw-r--r--   0 arne      (1000) users      (998)     4034 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/hash.py
+-rw-r--r--   0 arne      (1000) users      (998)     3362 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/hosts.py
+-rw-r--r--   0 arne      (1000) users      (998)    12922 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/ifc.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/freenet_passlib_170/passlib-misc/
+-rw-r--r--   0 arne      (1000) users      (998)     6288 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/passlib-misc/setup.py
+-rw-r--r--   0 arne      (1000) users      (998)    28376 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/pwd.py
+-rw-r--r--   0 arne      (1000) users      (998)    21150 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/registry.py
+-rw-r--r--   0 arne      (1000) users      (998)    72626 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/totp.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/freenet_passlib_170/utils/
+-rw-r--r--   0 arne      (1000) users      (998)    36793 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)    31482 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/binary.py
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/freenet_passlib_170/utils/compat/
+-rw-r--r--   0 arne      (1000) users      (998)    13503 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/compat/__init__.py
+-rw-r--r--   0 arne      (1000) users      (998)     8392 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/compat/_ordered_dict.py
+-rw-r--r--   0 arne      (1000) users      (998)     7675 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/decor.py
+-rw-r--r--   0 arne      (1000) users      (998)     2283 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/des.py
+-rw-r--r--   0 arne      (1000) users      (998)   104189 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/handlers.py
+-rw-r--r--   0 arne      (1000) users      (998)     1278 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/md4.py
+-rw-r--r--   0 arne      (1000) users      (998)     6976 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/utils/pbkdf2.py
+-rw-r--r--   0 arne      (1000) users      (998)     2687 2019-09-23 20:41:59.000000 pyFreenet3-0.5.9/freenet_passlib_170/win32.py
+-rwxr-xr-x   0 arne      (1000) users      (998)    18189 2023-03-29 08:16:20.000000 pyFreenet3-0.5.9/freesitemgr
+drwxr-xr-x   0 arne      (1000) users      (998)        0 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/pyFreenet3.egg-info/
+-rw-r--r--   0 arne      (1000) users      (998)     3066 2023-05-06 16:26:29.000000 pyFreenet3-0.5.9/pyFreenet3.egg-info/PKG-INFO
+-rw-r--r--   0 arne      (1000) users      (998)     3157 2023-05-06 16:26:29.000000 pyFreenet3-0.5.9/pyFreenet3.egg-info/SOURCES.txt
+-rw-r--r--   0 arne      (1000) users      (998)        1 2023-05-06 16:26:29.000000 pyFreenet3-0.5.9/pyFreenet3.egg-info/dependency_links.txt
+-rw-r--r--   0 arne      (1000) users      (998)       34 2023-05-06 16:26:29.000000 pyFreenet3-0.5.9/pyFreenet3.egg-info/top_level.txt
+-rwxr-xr-x   0 arne      (1000) users      (998)     3320 2019-09-23 19:31:28.000000 pyFreenet3-0.5.9/pyNodeConfig
+-rw-r--r--   0 arne      (1000) users      (998)       76 2023-05-06 16:26:29.687770 pyFreenet3-0.5.9/setup.cfg
+-rwxr-xr-x   0 arne      (1000) users      (998)     2987 2023-05-06 16:20:14.000000 pyFreenet3-0.5.9/setup.py
```

### Comparing `pyFreenet3-0.5.8/PKG-INFO` & `pyFreenet3-0.5.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,82 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyFreenet3
-Version: 0.5.8
+Version: 0.5.9
 Summary: Freenet Client Protocol Helper
 Home-page: http://127.0.0.1:8888/USK@~osOPnNLdMLVrYVNTahLufdwOuMhhC4GkpIHulnSm04,bwAmjkK-BZZnj-bujBQehwgGqUM1AUFhzTW4hcDGXQ0,AQACAAE/infocalypse_and_pyFreenet/5/
 Author: Arne Babenhauserheide
 Author-email: arne_bab@web.de
-License: UNKNOWN
-Description: README file for pyFreenet3
-        
-        PyFreenet3 is a suite of command-line freenet applications, as well as a
-        powerful Python library, for Freenet.
-        
-        Contribute at https://github.com/freenet/pyFreenet
-        
-        
-        Install via::
-        
-          $ pip3 install --upgrade --user pyFreenet3
-          (this requires python3 and python3-setuptools and python3-distutils installed)
-        
-        To just upload a file into Freenet (currently only on GNU/Linux), install a Java JRE or JDK and then use::
-        
-          $ fcpupload --spawn <file>`
-        
-        It starts a Freenet node, uploads the file and returns the key to access the file via Freenet.
-        
-        
-        If you need a library for Python 2, please use pyFreenet.
-        
-        
-        This pyFreenet3 release includes:
-        
-         - command-line freenet client applications, which will get installed as
-           executable commands in your PATH, including:
-        
-             - freesitemgr - a simple yet flexible freesite management utility
-             - fcpnames - utility for managing the new 'name service' layer
-             - fproxyproxy - an experimental http proxy that sits on top of
-               fproxy, and translates human-friendly site names transparently
-             - fcpget - a single key fetcher
-             - fcpput - a single key inserter
-             - fcpupload - fcpput with more convenient defaults
-             - fcpgenkey - a keypair generator
-             - fcpinvertkey - generate new SSK/USK keypairs
-             - fcpredirect - insert a redirect from one 'key' to another 'key'.
-             - copyweb - download a page from a website with all resources.
-        
-         - python package 'fcp3' and 'freenet3', containing classes for interacting with freenet.
-        
-         - an XML-RPC server for freenet access, which can be run standalone, or
-           easily integrated into an existing website
-        
-        To get good API documentation, run::
-        
-          $ epydoc -n "pyFreenet API manual" -o html fcp
-        
-        When you install this package (refer INSTALL), you should 
-        end up with a command 'freesitemgr' on your PATH.
-        
-        'freesitemgr' is a console-based freesite insertion utility
-        which keeps your freesite configs and status in a single
-        config file (~/.freesitemgr, unless you specify otherwise).
-        
-        Just use 'freesitemgr add FOLDER' to upload a website into Freenet.
-        
-        Invoke 'freesitemgr -h' (or if on windows, 'freesitemgr.py -h')
-        and read the options.
-        
-        release a new version::
-        
-          python3 setup.py sdist; python3 -m twine upload dist/pyFreenet3-0.5.5.tar.gz 
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE_appdirs.txt
+License-File: COPYING
+License-File: AUTHORS
+
+README file for pyFreenet3
+
+PyFreenet3 is a suite of command-line freenet applications, as well as a
+powerful Python library, for Freenet.
+
+Contribute at https://github.com/freenet/pyFreenet
+
+
+Install via::
+
+  $ pip3 install --upgrade --user pyFreenet3
+  (this requires python3 and python3-setuptools and python3-distutils installed)
+
+To just upload a file into Freenet (currently only on GNU/Linux), install a Java JRE or JDK and then use::
+
+  $ fcpupload --spawn <file>`
+
+It starts a Freenet node, uploads the file and returns the key to access the file via Freenet.
+
+
+If you need a library for Python 2, please use pyFreenet.
+
+
+This pyFreenet3 release includes:
+
+ - command-line freenet client applications, which will get installed as
+   executable commands in your PATH, including:
+
+     - freesitemgr - a simple yet flexible freesite management utility
+     - fcpnames - utility for managing the new 'name service' layer
+     - fproxyproxy - an experimental http proxy that sits on top of
+       fproxy, and translates human-friendly site names transparently
+     - fcpget - a single key fetcher
+     - fcpput - a single key inserter
+     - fcpupload - fcpput with more convenient defaults
+     - fcpgenkey - a keypair generator
+     - fcpinvertkey - generate new SSK/USK keypairs
+     - fcpredirect - insert a redirect from one 'key' to another 'key'.
+     - copyweb - download a page from a website with all resources.
+
+ - python package 'fcp3' and 'freenet3', containing classes for interacting with freenet.
+
+ - an XML-RPC server for freenet access, which can be run standalone, or
+   easily integrated into an existing website
+
+To get good API documentation, run::
+
+  $ epydoc -n "pyFreenet API manual" -o html fcp
+
+When you install this package (refer INSTALL), you should 
+end up with a command 'freesitemgr' on your PATH.
+
+'freesitemgr' is a console-based freesite insertion utility
+which keeps your freesite configs and status in a single
+config file (~/.freesitemgr, unless you specify otherwise).
+
+Just use 'freesitemgr add FOLDER' to upload a website into Freenet.
+
+Invoke 'freesitemgr -h' (or if on windows, 'freesitemgr.py -h')
+and read the options.
+
+release a new version::
+
+  python3 setup.py sdist; python3 -m twine upload dist/pyFreenet3-0.5.5.tar.gz
```

### Comparing `pyFreenet3-0.5.8/README` & `pyFreenet3-0.5.9/README`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/babcom_cli` & `pyFreenet3-0.5.9/babcom_cli`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/copyweb` & `pyFreenet3-0.5.9/copyweb`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/__init__.py` & `pyFreenet3-0.5.9/fcp3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/arguments.py` & `pyFreenet3-0.5.9/fcp3/arguments.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/fproxyproxy.py` & `pyFreenet3-0.5.9/fcp3/fproxyproxy.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/freenetfs.py` & `pyFreenet3-0.5.9/fcp3/freenetfs.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/genkey.py` & `pyFreenet3-0.5.9/fcp3/genkey.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/get.py` & `pyFreenet3-0.5.9/fcp3/get.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/invertkey.py` & `pyFreenet3-0.5.9/fcp3/invertkey.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/names.py` & `pyFreenet3-0.5.9/fcp3/names.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/node.py` & `pyFreenet3-0.5.9/fcp3/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 00000b80: 0a23 2070 6565 7220 6e6f 7465 2074 7970  .# peer note typ
 00000b90: 6573 0a50 4545 525f 4e4f 5445 5f50 5249  es.PEER_NOTE_PRI
 00000ba0: 5641 5445 5f44 4152 4b4e 4554 5f43 4f4d  VATE_DARKNET_COM
 00000bb0: 4d45 4e54 203d 2031 0a0a 6465 6661 756c  MENT = 1..defaul
 00000bc0: 7456 6572 626f 7369 7479 203d 2045 5252  tVerbosity = ERR
 00000bd0: 4f52 0a0a 4f4e 455f 5945 4152 203d 2038  OR..ONE_YEAR = 8
 00000be0: 3634 3030 202a 2033 3635 0a0a 6663 7056  6400 * 365..fcpV
-00000bf0: 6572 7369 6f6e 203d 2022 302e 332e 3422  ersion = "0.3.4"
+00000bf0: 6572 7369 6f6e 203d 2022 302e 352e 3922  ersion = "0.5.9"
 00000c00: 0a0a 0a63 6c61 7373 2046 4350 4e6f 6465  ...class FCPNode
 00000c10: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
 00000c20: 7072 6573 656e 7473 2061 6e20 696e 7465  presents an inte
 00000c30: 7266 6163 6520 746f 2061 2066 7265 656e  rface to a freen
 00000c40: 6574 206e 6f64 6520 7669 6120 6974 7320  et node via its 
 00000c50: 4643 5020 706f 7274 2c0a 2020 2020 616e  FCP port,.    an
 00000c60: 6420 6578 706f 7365 7320 7072 696d 6974  d exposes primit
```

### Comparing `pyFreenet3-0.5.8/fcp3/pseudopythonparser.py` & `pyFreenet3-0.5.9/fcp3/pseudopythonparser.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/put.py` & `pyFreenet3-0.5.9/fcp3/put.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/redirect.py` & `pyFreenet3-0.5.9/fcp3/redirect.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/sitemgr.py` & `pyFreenet3-0.5.9/fcp3/sitemgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 #@+others
 #@+node:imports
 import sys, os, os.path, io, threading, traceback, pprint, time, stat, json
 
 import fcp3 as fcp
-from fcp3 import CRITICAL, ERROR, INFO, DETAIL, DEBUG, NOISY
+from fcp3 import CRITICAL, ERROR, INFO, DETAIL, DEBUG #, NOISY
 from fcp3.node import hashFile
 
 #@-node:imports
 #@+node:globals
 defaultBaseDir = os.path.join(os.path.expanduser('~'), ".freesitemgr")
 
 maxretries = -1
@@ -653,15 +653,18 @@
                     w("# " + comment + "\n")
                 for name, value in list(kw.items()):
                     w(name + " = ")
                     # json fails at True, False, None
                     if value is True or value is False or value is None:
                         pp.pprint(value)
                     else:
-                        w(js.encode(value).lstrip())
+                        try:
+                            w(js.encode(value).lstrip())
+                        except TypeError:
+                            pass
                         w("\n")
                 if comment:
                     w("\n")
                 w(tail)
                 f.flush()
     
             w("# freesitemgr state file for freesite '%s'\n" % self.name)
@@ -774,14 +777,24 @@
                 self.log(
                     ERROR,
                     "insert:%s: checking if a new insert is needed" % self.name)
     
         # compare our representation to what's on disk
         self.scan()
         
+        # ------------------------------------------------
+        # check which files should be part of the manifest
+        # we have to do this after creating the index and 
+        # sitemap, because we have to know the size of the 
+        # index and the sitemap. This will lead to some 
+        # temporary errors in the sitemap. They will 
+        # disappear at the next insert.
+        
+        self.markManifestFiles()
+
         # bail if site is already up to date
         if not self.needToUpdate:
             log(ERROR, "insert:%s: No update required" % self.name)
             return
 
         # bail if --no-insert was given
         if self.noInsert:
@@ -792,32 +805,22 @@
     
         # not currently updating, so anything on the queue is crap
         self.clearNodeQueue()
     
         # ------------------------------------------------
         # may need to auto-generate an index.html
         self.createIndexAndSitemapIfNeeded()
-    
-        # ------------------------------------------------
-        # check which files should be part of the manifest
-        # we have to do this after creating the index and 
-        # sitemap, because we have to know the size of the 
-        # index and the sitemap. This will lead to some 
-        # temporary errors in the sitemap. They will 
-        # disappear at the next insert.
-        
-        self.markManifestFiles()
         
         # ------------------------------------------------
         # select which files to insert, and get their CHKs
     
         # get records of files to insert    
         # TODO: Check whether the CHK top block is retrievable
         filesToInsert = [r for r in self.files if (r['state'] in ('changed', 'waiting') 
-                                          and not r['target'] == 'manifest')]
+                                          and not r.get('target', 'separate') == 'manifest')]
         # sort by size: smallest first, so that the node queue is
         # cleared more quickly.
         filesToInsert.sort(key=lambda x: x['sizebytes'])
         
         # compute CHKs for all these files, synchronously, and at the same time,
         # submit the inserts, asynchronously
         chkCounter = 0
@@ -1496,14 +1499,20 @@
             if rec['sizebytes'] + totalsize <= maxsize + redirectSize:
                 rec['target'] = 'manifest'
                 totalsize += rec['sizebytes']
                 maxsize += redirectSize # no redirect needed for this file
                 # remember this
                 fileNamesInManifest.add(rec['name'])
             else:
+                if rec.get('target', 'separate') == 'manifest':
+                    # if files moved out of the manifest, they have to be uploaded again
+                    if not rec['uri']:
+                        rec['state'] = 'changed'
+                        self.needToUpdate = True
+                        self.needToSave = True
                 rec['target'] = 'separate'
         # now add more small files to the manifest until less than
         # maxNumberSeparateFiles remain separate.
         separateRecBySize = [i for i in recBySize
                              if not i['name'] in fileNamesInManifest]
         numSeparate = len(separateRecBySize)
         filesToAdd = max(0, numSeparate - self.sitemgr.maxNumberSeparateFiles)
```

### Comparing `pyFreenet3-0.5.8/fcp3/upload.py` & `pyFreenet3-0.5.9/fcp3/upload.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/xmlobject.py` & `pyFreenet3-0.5.9/fcp3/xmlobject.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcp3/xmlrpc.py` & `pyFreenet3-0.5.9/fcp3/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcpgetdir` & `pyFreenet3-0.5.9/fcpgetdir`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/fcpputdir` & `pyFreenet3-0.5.9/fcpputdir`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet3/appdirs.py` & `pyFreenet3-0.5.9/freenet3/appdirs.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet3/spawn.py` & `pyFreenet3-0.5.9/freenet3/spawn.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/_setup/docdist.py` & `pyFreenet3-0.5.9/freenet_passlib_170/_setup/docdist.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/_setup/stamp.py` & `pyFreenet3-0.5.9/freenet_passlib_170/_setup/stamp.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/apache.py` & `pyFreenet3-0.5.9/freenet_passlib_170/apache.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/apps.py` & `pyFreenet3-0.5.9/freenet_passlib_170/apps.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/context.py` & `pyFreenet3-0.5.9/freenet_passlib_170/context.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/__init__.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/_gen_files.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/_gen_files.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/base.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/base.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/_blowfish/unrolled.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/_blowfish/unrolled.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/_md4.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/_md4.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/des.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/des.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/digest.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/digest.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/__init__.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/_builtin.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/_builtin.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/_gen_files.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/_gen_files.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/crypto/scrypt/_salsa.py` & `pyFreenet3-0.5.9/freenet_passlib_170/crypto/scrypt/_salsa.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/exc.py` & `pyFreenet3-0.5.9/freenet_passlib_170/exc.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/ext/django/models.py` & `pyFreenet3-0.5.9/freenet_passlib_170/ext/django/models.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/ext/django/utils.py` & `pyFreenet3-0.5.9/freenet_passlib_170/ext/django/utils.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/argon2.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/argon2.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/bcrypt.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/bcrypt.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/cisco.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/cisco.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/des_crypt.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/des_crypt.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/digests.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/digests.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/django.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/django.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/fshp.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/fshp.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/ldap_digests.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/ldap_digests.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/md5_crypt.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/md5_crypt.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/misc.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/mssql.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/mssql.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/mysql.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/mysql.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/oracle.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/oracle.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/pbkdf2.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/phpass.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/phpass.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/postgres.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/postgres.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/roundup.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/roundup.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/scram.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/scram.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/scrypt.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/scrypt.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/sha1_crypt.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/sha1_crypt.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/sha2_crypt.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/sha2_crypt.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/sun_md5_crypt.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/sun_md5_crypt.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/handlers/windows.py` & `pyFreenet3-0.5.9/freenet_passlib_170/handlers/windows.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/hash.py` & `pyFreenet3-0.5.9/freenet_passlib_170/hash.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/hosts.py` & `pyFreenet3-0.5.9/freenet_passlib_170/hosts.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/ifc.py` & `pyFreenet3-0.5.9/freenet_passlib_170/ifc.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/passlib-misc/setup.py` & `pyFreenet3-0.5.9/freenet_passlib_170/passlib-misc/setup.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/pwd.py` & `pyFreenet3-0.5.9/freenet_passlib_170/pwd.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/registry.py` & `pyFreenet3-0.5.9/freenet_passlib_170/registry.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/totp.py` & `pyFreenet3-0.5.9/freenet_passlib_170/totp.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/__init__.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/binary.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/binary.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/compat/__init__.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/compat/_ordered_dict.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/compat/_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/decor.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/decor.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/des.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/des.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/handlers.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/md4.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/md4.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/utils/pbkdf2.py` & `pyFreenet3-0.5.9/freenet_passlib_170/utils/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freenet_passlib_170/win32.py` & `pyFreenet3-0.5.9/freenet_passlib_170/win32.py`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/freesitemgr` & `pyFreenet3-0.5.9/freesitemgr`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/pyNodeConfig` & `pyFreenet3-0.5.9/pyNodeConfig`

 * *Files identical despite different names*

### Comparing `pyFreenet3-0.5.8/setup.py` & `pyFreenet3-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             else:
                 print(e)
         if not doze:
             os.system("cp " + man_dir + "/*.1 " + man_target_dir)
 
 
 setup(name="pyFreenet3",
-      version="0.5.8",
+      version="0.5.9",
       description="Freenet Client Protocol Helper",
       author="Arne Babenhauserheide",
       author_email="arne_bab@web.de",
       url="http://127.0.0.1:8888/USK@~osOPnNLdMLVrYVNTahLufdwOuMhhC4GkpIHulnSm04,bwAmjkK-BZZnj-bujBQehwgGqUM1AUFhzTW4hcDGXQ0,AQACAAE/infocalypse_and_pyFreenet/5/",
       packages = ['fcp3', 'freenet3', 'freenet_passlib_170'] + [
           'freenet_passlib_170' + "." + i
           for i in "crypto ext ext.django handlers passlib-misc _setup".split() +
```

