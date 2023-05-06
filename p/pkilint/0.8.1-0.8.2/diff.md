# Comparing `tmp/pkilint-0.8.1.tar.gz` & `tmp/pkilint-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkilint-0.8.1.tar", last modified: Wed May  3 13:12:28 2023, max compression
+gzip compressed data, was "pkilint-0.8.2.tar", last modified: Sat May  6 04:55:15 2023, max compression
```

## Comparing `pkilint-0.8.1.tar` & `pkilint-0.8.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 13:12:10.000000 pkilint-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-05-03 13:12:28.503013 pkilint-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-05-03 13:12:10.000000 pkilint-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 13:12:10.000000 pkilint-0.8.1/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint/adobe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/adobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/adobe/adobe_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint/adobe/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/adobe/asn1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/convert_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_cabf_serverauth_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_pkix_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/cabf_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/servercert/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/servercert/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/asn1/ev_guidelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/servercert/servercert_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/cabf/smime/
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/cabf/smime/smime_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/etsi/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/etsi/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/asn1/en_319_412_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/etsi/asn1/ts_119_495.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/iso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/iso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/iso/lei.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/itu/x520_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/msft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/msft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/msft/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/msft/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/msft/msft_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.499013 pkilint-0.8.1/pkilint/pkix/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/pkilint/pkix/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/certificate/certificate_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/pkilint/pkix/crl/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/crl_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/crl_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/crl/crl_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/general_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/pkilint/pkix/ocsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_basic_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/pkix/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-03 13:12:10.000000 pkilint-0.8.1/pkilint/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.495013 pkilint-0.8.1/pkilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:12:28.000000 pkilint-0.8.1/pkilint.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-03 13:12:28.503013 pkilint-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 13:12:10.000000 pkilint-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/tests/integration_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/integration_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/integration_certificate/test_cabf_smime_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:28.503013 pkilint-0.8.1/tests/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/itu/test_bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/itu/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-03 13:12:10.000000 pkilint-0.8.1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-06 04:55:05.000000 pkilint-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-06 04:55:15.417621 pkilint-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-06 04:55:05.000000 pkilint-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 04:55:05.000000 pkilint-0.8.2/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.409622 pkilint-0.8.2/pkilint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/adobe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/adobe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/adobe/adobe_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/adobe/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/adobe/asn1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/convert_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_cabf_serverauth_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_pkix_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/servercert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/servercert/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/asn1/ev_guidelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/smime/
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/etsi/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/etsi/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/asn1/en_319_412_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/asn1/ts_119_495.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/iso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/iso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/iso/lei.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/x520_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/msft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/msft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/msft/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/msft/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/msft/msft_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/crl_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/crl_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/crl_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/ocsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_basic_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-06 04:55:15.421622 pkilint-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 04:55:05.000000 pkilint-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/tests/integration_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/integration_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/integration_certificate/test_cabf_smime_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/tests/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/itu/test_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/itu/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/util.py
```

### Comparing `pkilint-0.8.1/LICENSE` & `pkilint-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/PKG-INFO` & `pkilint-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.1
+Version: 0.8.2
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -46,14 +46,20 @@
 
 3. Use pipx to install pkilint:
 
     `pipx install pkilint`
 
 Once installed, the bundled command line applications (listed below) and the API will be available on your machine.
 
+### Upgrading
+
+When a new version of pkilint is released, run the following command to upgrade your installation:
+
+   `pipx upgrade pkilint`
+
 ## Usage
 
 In addition to the API, several command line tools are bundled with pkilint. Upon termination of execution, each linter
 will return the number of reported findings as the process exit code.
 
 The list of command line linters bundled with pkilint:
```

### Comparing `pkilint-0.8.1/README.md` & `pkilint-0.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
 3. Use pipx to install pkilint:
 
     `pipx install pkilint`
 
 Once installed, the bundled command line applications (listed below) and the API will be available on your machine.
 
+### Upgrading
+
+When a new version of pkilint is released, run the following command to upgrade your installation:
+
+   `pipx upgrade pkilint`
+
 ## Usage
 
 In addition to the API, several command line tools are bundled with pkilint. Upon termination of execution, each linter
 will return the number of reported findings as the process exit code.
 
 The list of command line linters bundled with pkilint:
```

### Comparing `pkilint-0.8.1/pkilint/adobe/adobe_validator.py` & `pkilint-0.8.2/pkilint/adobe/adobe_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/adobe/asn1/__init__.py` & `pkilint-0.8.2/pkilint/adobe/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/bin/convert_cert.py` & `pkilint-0.8.2/pkilint/bin/convert_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/bin/lint_cabf_serverauth_cert.py` & `pkilint-0.8.2/pkilint/bin/lint_cabf_serverauth_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/bin/lint_cabf_smime_cert.py` & `pkilint-0.8.2/pkilint/bin/lint_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/bin/lint_crl.py` & `pkilint-0.8.2/pkilint/bin/lint_crl.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
     crl_type = crl.CertificateRevocationListType[args.type]
 
     validity_additional_validators = []
     doc_additional_validators = []
 
     if args.profile == 'BR':
         doc_additional_validators.append(
-            servercert_crl.create_reason_code_validator(crl_type)
+            cabf_crl.create_reason_code_validator(crl_type)
         )
 
         validity_additional_validators.append(
-            servercert_crl.create_validity_period_validator(crl_type)
+            cabf_crl.create_validity_period_validator(crl_type)
         )
 
     doc_validator = crl.create_pkix_crl_validator_container(
         [
             pkix.create_attribute_decoder(name.ATTRIBUTE_TYPE_MAPPINGS),
             pkix.create_extension_decoder(extension.EXTENSION_MAPPINGS),
         ],
```

### Comparing `pkilint-0.8.1/pkilint/bin/lint_ocsp_response.py` & `pkilint-0.8.2/pkilint/bin/lint_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/bin/lint_pkix_cert.py` & `pkilint-0.8.2/pkilint/bin/lint_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/bin/lint_pkix_signer_signee_cert_chain.py` & `pkilint-0.8.2/pkilint/bin/lint_pkix_signer_signee_cert_chain.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/__init__.py` & `pkilint-0.8.2/pkilint/cabf/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/cabf_constants.py` & `pkilint-0.8.2/pkilint/cabf/cabf_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/cabf_crl.py` & `pkilint-0.8.2/pkilint/cabf/cabf_crl.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 
 def create_validity_period_validator(
         crl_type: crl.CertificateRevocationListType
 ):
     if crl_type == crl.CertificateRevocationListType.CRL:
         max_validity_days = 10
-        finding = 'br.crl_invalid_validity_period'
+        finding = 'cabf.crl_invalid_validity_period'
     else:
         max_validity_days = 365  # TODO: handle leap years?
-        finding = 'br.arl_invalid_validity_period'
+        finding = 'cabf.arl_invalid_validity_period'
 
     thresholds = [
         (
             operator.le,
             timedelta(days=max_validity_days),
             validation.ValidationFinding(
                 validation.ValidationFindingSeverity.ERROR,
```

### Comparing `pkilint-0.8.1/pkilint/cabf/cabf_extension.py` & `pkilint-0.8.2/pkilint/cabf/cabf_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/cabf_key.py` & `pkilint-0.8.2/pkilint/cabf/cabf_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/cabf_name.py` & `pkilint-0.8.2/pkilint/cabf/cabf_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/servercert/__init__.py` & `pkilint-0.8.2/pkilint/cabf/servercert/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/servercert/asn1/ev_guidelines.py` & `pkilint-0.8.2/pkilint/cabf/servercert/asn1/ev_guidelines.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/servercert/servercert_extension.py` & `pkilint-0.8.2/pkilint/cabf/servercert/servercert_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/servercert/servercert_key.py` & `pkilint-0.8.2/pkilint/cabf/servercert/servercert_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/servercert/servercert_name.py` & `pkilint-0.8.2/pkilint/cabf/servercert/servercert_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/smime/__init__.py` & `pkilint-0.8.2/pkilint/cabf/smime/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/smime/smime_constants.py` & `pkilint-0.8.2/pkilint/cabf/smime/smime_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/smime/smime_extension.py` & `pkilint-0.8.2/pkilint/cabf/smime/smime_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/smime/smime_key.py` & `pkilint-0.8.2/pkilint/cabf/smime/smime_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/cabf/smime/smime_name.py` & `pkilint-0.8.2/pkilint/cabf/smime/smime_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/document.py` & `pkilint-0.8.2/pkilint/document.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/etsi/__init__.py` & `pkilint-0.8.2/pkilint/etsi/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/etsi/asn1/en_319_412_5.py` & `pkilint-0.8.2/pkilint/etsi/asn1/en_319_412_5.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/etsi/asn1/ts_119_495.py` & `pkilint-0.8.2/pkilint/etsi/asn1/ts_119_495.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/iso/lei.py` & `pkilint-0.8.2/pkilint/iso/lei.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/itu/bitstring.py` & `pkilint-0.8.2/pkilint/itu/bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/itu/string.py` & `pkilint-0.8.2/pkilint/itu/string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/itu/x520_name.py` & `pkilint-0.8.2/pkilint/itu/x520_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/loader.py` & `pkilint-0.8.2/pkilint/loader.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/msft/msft_name.py` & `pkilint-0.8.2/pkilint/msft/msft_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/__init__.py` & `pkilint-0.8.2/pkilint/pkix/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/algorithm.py` & `pkilint-0.8.2/pkilint/pkix/algorithm.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/certificate/__init__.py` & `pkilint-0.8.2/pkilint/pkix/certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/certificate/certificate_extension.py` & `pkilint-0.8.2/pkilint/pkix/certificate/certificate_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/certificate/certificate_key.py` & `pkilint-0.8.2/pkilint/pkix/certificate/certificate_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/certificate/certificate_name.py` & `pkilint-0.8.2/pkilint/pkix/certificate/certificate_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/certificate/certificate_validator.py` & `pkilint-0.8.2/pkilint/pkix/certificate/certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/certificate/certificate_validity.py` & `pkilint-0.8.2/pkilint/pkix/certificate/certificate_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/crl/__init__.py` & `pkilint-0.8.2/pkilint/pkix/crl/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/crl/crl_extension.py` & `pkilint-0.8.2/pkilint/pkix/crl/crl_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/crl/crl_validator.py` & `pkilint-0.8.2/pkilint/pkix/crl/crl_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/crl/crl_validity.py` & `pkilint-0.8.2/pkilint/pkix/crl/crl_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/extension.py` & `pkilint-0.8.2/pkilint/pkix/extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/general_name.py` & `pkilint-0.8.2/pkilint/pkix/general_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/name.py` & `pkilint-0.8.2/pkilint/pkix/name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/ocsp/__init__.py` & `pkilint-0.8.2/pkilint/pkix/ocsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_basic_response.py` & `pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_basic_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_response.py` & `pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/ocsp/ocsp_validity.py` & `pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/pkix/time.py` & `pkilint-0.8.2/pkilint/pkix/time.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/report.py` & `pkilint-0.8.2/pkilint/report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/util.py` & `pkilint-0.8.2/pkilint/util.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint/validation.py` & `pkilint-0.8.2/pkilint/validation.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/pkilint.egg-info/PKG-INFO` & `pkilint-0.8.2/pkilint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.1
+Version: 0.8.2
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -46,14 +46,20 @@
 
 3. Use pipx to install pkilint:
 
     `pipx install pkilint`
 
 Once installed, the bundled command line applications (listed below) and the API will be available on your machine.
 
+### Upgrading
+
+When a new version of pkilint is released, run the following command to upgrade your installation:
+
+   `pipx upgrade pkilint`
+
 ## Usage
 
 In addition to the API, several command line tools are bundled with pkilint. Upon termination of execution, each linter
 will return the number of reported findings as the process exit code.
 
 The list of command line linters bundled with pkilint:
```

### Comparing `pkilint-0.8.1/pkilint.egg-info/SOURCES.txt` & `pkilint-0.8.2/pkilint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/setup.cfg` & `pkilint-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/tests/integration_certificate/__init__.py` & `pkilint-0.8.2/tests/integration_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/tests/integration_certificate/test_cabf_smime_cert.py` & `pkilint-0.8.2/tests/integration_certificate/test_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/tests/itu/test_bitstring.py` & `pkilint-0.8.2/tests/itu/test_bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/tests/itu/test_string.py` & `pkilint-0.8.2/tests/itu/test_string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.1/tests/util.py` & `pkilint-0.8.2/tests/util.py`

 * *Files identical despite different names*

