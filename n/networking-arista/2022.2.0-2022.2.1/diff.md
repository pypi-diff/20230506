# Comparing `tmp/networking_arista-2022.2.0.tar.gz` & `tmp/networking_arista-2022.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networking_arista-2022.2.0.tar", last modified: Thu Feb  2 19:43:32 2023, max compression
+gzip compressed data, was "networking_arista-2022.2.1.tar", last modified: Fri May  5 23:18:59 2023, max compression
```

## Comparing `networking_arista-2022.2.0.tar` & `networking_arista-2022.2.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.198367 networking_arista-2022.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2023-02-02 19:43:31.000000 networking_arista-2022.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13103 2023-02-02 19:43:31.000000 networking_arista-2022.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2023-02-02 19:43:32.198367 networking_arista-2022.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.174366 networking_arista-2022.2.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3834 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.166366 networking_arista-2022.2.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.174366 networking_arista-2022.2.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2465 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.174366 networking_arista-2022.2.0/dockerfiles/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/dockerfiles/README
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.174366 networking_arista-2022.2.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5954 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/etc/ml2_conf_arista.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6570 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/etc/policy.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.174366 networking_arista-2022.2.0/networking_arista/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1365 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.178366 networking_arista-2022.2.0/networking_arista/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5949 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/common/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11071 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2227 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23632 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/common/db_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2168 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.178366 networking_arista-2022.2.0/networking_arista/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.178366 networking_arista-2022.2.0/networking_arista/db/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.182366 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3518 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.182366 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/296b4e0236e0_initial_db_version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/CONTRACT_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/EXPAND_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.166366 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/liberty/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.182366 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/liberty/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/liberty/contract/47036dc8697a_initial_db_version_contract.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.182366 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/liberty/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/liberty/expand/1c6993ce7db0_initial_db_version_expand.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.166366 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.182366 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/contract/39c2eeb67116_drop_aristaprovisionednets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/contract/941bad5630c1_drop_aristaprovisionedvms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/contract/dc7bf9c1ab4d_drop_aristaprovisionedtenants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.182366 networking_arista-2022.2.0/networking_arista/l3Plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/l3Plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31700 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/l3Plugin/arista_l3_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18189 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/l3Plugin/l3_arista.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.186366 networking_arista-2022.2.0/networking_arista/ml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24396 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/arista_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10975 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/arista_sync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7178 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/arista_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17821 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/mechanism_arista.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.186366 networking_arista-2022.2.0/networking_arista/ml2/rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/rpc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13615 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/rpc/arista_eapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7800 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/rpc/arista_json.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/rpc/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.186366 networking_arista-2022.2.0/networking_arista/ml2/security_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/security_groups/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6040 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/security_groups/arista_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/security_groups/security_group_sync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21025 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/security_groups/switch_helper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.186366 networking_arista-2022.2.0/networking_arista/ml2/type_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/type_drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7139 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/type_drivers/driver_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3882 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/ml2/type_drivers/type_arista_vlan.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.190367 networking_arista-2022.2.0/networking_arista/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/test_networking_arista.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.190367 networking_arista-2022.2.0/networking_arista/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.190367 networking_arista-2022.2.0/networking_arista/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9099 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/common/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14620 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/common/test_db_lib.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.190367 networking_arista-2022.2.0/networking_arista/tests/unit/l3Plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/l3Plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60414 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/l3Plugin/test_arista_l3_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.194367 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/mechanism_fabric.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4120 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/mechanism_ha_simulator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24570 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/ml2_test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.194367 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/rpc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8328 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/rpc/test_arista_eapi_rpc_wrapper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7266 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/rpc/test_arista_json_rpc_wrapper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.194367 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3195 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/sg_test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25554 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/test_arista_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20755 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/test_security_group_sync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58601 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/test_arista_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/test_arista_sync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    66347 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/test_mechanism_arista.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.194367 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/type_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/type_drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7874 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/ml2/type_drivers/test_arista_type_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34505 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/networking_arista/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-02 19:43:32.178366 networking_arista-2022.2.0/networking_arista.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2023-02-02 19:43:32.000000 networking_arista-2022.2.0/networking_arista.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2023-02-02 19:43:32.198367 networking_arista-2022.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2023-02-02 19:43:09.000000 networking_arista-2022.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.042289 networking_arista-2022.2.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13182 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2023-05-05 23:18:59.042289 networking_arista-2022.2.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.022289 networking_arista-2022.2.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3834 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.014289 networking_arista-2022.2.1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.022289 networking_arista-2022.2.1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2465 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.022289 networking_arista-2022.2.1/dockerfiles/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/dockerfiles/README
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.022289 networking_arista-2022.2.1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5954 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/etc/ml2_conf_arista.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6570 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/etc/policy.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.026289 networking_arista-2022.2.1/networking_arista/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1365 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.026289 networking_arista-2022.2.1/networking_arista/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5949 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/common/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11071 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2227 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23772 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/common/db_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2204 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.030289 networking_arista-2022.2.1/networking_arista/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.030289 networking_arista-2022.2.1/networking_arista/db/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.030289 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3518 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.030289 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/296b4e0236e0_initial_db_version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/CONTRACT_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/EXPAND_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.018289 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/liberty/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.030289 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/liberty/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/liberty/contract/47036dc8697a_initial_db_version_contract.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.030289 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/liberty/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/liberty/expand/1c6993ce7db0_initial_db_version_expand.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.018289 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.030289 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/contract/39c2eeb67116_drop_aristaprovisionednets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/contract/941bad5630c1_drop_aristaprovisionedvms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/contract/dc7bf9c1ab4d_drop_aristaprovisionedtenants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.034289 networking_arista-2022.2.1/networking_arista/l3Plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/l3Plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31700 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/l3Plugin/arista_l3_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18189 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/l3Plugin/l3_arista.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.034289 networking_arista-2022.2.1/networking_arista/ml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23971 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/arista_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10975 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/arista_sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7178 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/arista_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17890 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/mechanism_arista.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.034289 networking_arista-2022.2.1/networking_arista/ml2/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13615 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/rpc/arista_eapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7800 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/rpc/arista_json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/rpc/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.034289 networking_arista-2022.2.1/networking_arista/ml2/security_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/security_groups/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6040 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/security_groups/arista_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/security_groups/security_group_sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21025 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/security_groups/switch_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.034289 networking_arista-2022.2.1/networking_arista/ml2/type_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/type_drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7139 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/type_drivers/driver_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3882 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/ml2/type_drivers/type_arista_vlan.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.038289 networking_arista-2022.2.1/networking_arista/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/test_networking_arista.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.038289 networking_arista-2022.2.1/networking_arista/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.038289 networking_arista-2022.2.1/networking_arista/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9099 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/common/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14620 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/common/test_db_lib.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.038289 networking_arista-2022.2.1/networking_arista/tests/unit/l3Plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/l3Plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60414 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/l3Plugin/test_arista_l3_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.038289 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/mechanism_fabric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4120 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/mechanism_ha_simulator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24874 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/ml2_test_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.042289 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/rpc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8328 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/rpc/test_arista_eapi_rpc_wrapper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7266 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/rpc/test_arista_json_rpc_wrapper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.042289 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3195 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/sg_test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25554 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/test_arista_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20755 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/test_security_group_sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58679 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/test_arista_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/test_arista_sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70128 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/test_mechanism_arista.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.042289 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/type_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/type_drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7874 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/ml2/type_drivers/test_arista_type_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34505 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/networking_arista/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-05 23:18:59.026289 networking_arista-2022.2.1/networking_arista.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/networking_arista.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4628 2023-05-05 23:18:59.000000 networking_arista-2022.2.1/networking_arista.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/networking_arista.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/networking_arista.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/networking_arista.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/networking_arista.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/networking_arista.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2023-05-05 23:18:58.000000 networking_arista-2022.2.1/networking_arista.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2023-05-05 23:18:59.046289 networking_arista-2022.2.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2023-05-05 23:18:17.000000 networking_arista-2022.2.1/tox.ini
```

### Comparing `networking_arista-2022.2.0/AUTHORS` & `networking_arista-2022.2.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/CONTRIBUTING.rst` & `networking_arista-2022.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/ChangeLog` & `networking_arista-2022.2.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+2022.2.1
+--------
+
+* Add support for provisioning L2 connectivity for L3 GW ports
+
 2022.2.0
 --------
 
 * Use context manager from neutron-lib accessing VlanAllocation
 * Revert "Check for missing port bindings each sync period"
 * Ensure queries are executed in reader sessions
 * Don't send sync complete on sync failure after switchover
@@ -270,16 +275,16 @@
 * Check that shared networks are VLAN networks before in Arista ML2
 * Fixed typos in arista\_l3\_driver.py
 * Fix error handling to handle invalid URL, response
 * Enabling creation of unattached ports
 * Ensuring that the response contains 'errors' key
 * Use requests library instead of jsonrpclib
 
-2015.2.0
---------
+2015.2
+------
 
 * Adding database migration scripts
 * Use auth\_uri in when set
 * Adding support for multiple EOS instances
 * Supporting neutron HA
 * Using 'INTERNAL-TENANT-ID' as the network owner
 * Fixed HA router network cleanup
```

### Comparing `networking_arista-2022.2.0/LICENSE` & `networking_arista-2022.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/PKG-INFO` & `networking_arista-2022.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: networking_arista
-Version: 2022.2.0
+Version: 2022.2.1
 Summary: Arista Networking drivers
 Home-page: https://opendev.org/x/networking-arista/
 Author: Arista Networks
 Author-email: openstack-dev@arista.com
 License: UNKNOWN
 Description: ===============================
         networking-arista
```

### Comparing `networking_arista-2022.2.0/devstack/plugin.sh` & `networking_arista-2022.2.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/doc/source/conf.py` & `networking_arista-2022.2.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/doc/source/index.rst` & `networking_arista-2022.2.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/etc/ml2_conf_arista.ini` & `networking_arista-2022.2.1/etc/ml2_conf_arista.ini`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/etc/policy.json` & `networking_arista-2022.2.1/etc/policy.json`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/__init__.py` & `networking_arista-2022.2.1/networking_arista/__init__.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/_i18n.py` & `networking_arista-2022.2.1/networking_arista/_i18n.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/common/api.py` & `networking_arista-2022.2.1/networking_arista/common/api.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/common/config.py` & `networking_arista-2022.2.1/networking_arista/common/config.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/common/constants.py` & `networking_arista-2022.2.1/networking_arista/common/constants.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/common/db_lib.py` & `networking_arista-2022.2.1/networking_arista/common/db_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,16 @@
                          instance_id=instance_id)
 
 
 def get_router_instances(instance_id=None):
     """Returns filtered list of routers that may be relevant on CVX"""
     return get_instances(device_owners=[n_const.DEVICE_OWNER_DVR_INTERFACE,
                                         n_const.DEVICE_OWNER_ROUTER_HA_INTF,
-                                        n_const.DEVICE_OWNER_ROUTER_INTF],
+                                        n_const.DEVICE_OWNER_ROUTER_INTF,
+                                        n_const.DEVICE_OWNER_ROUTER_GW],
                          instance_id=instance_id)
 
 
 def get_vm_instances(instance_id=None):
     """Returns filtered list of vms that may be relevant on CVX"""
     return get_instances(device_owners=[n_const.DEVICE_OWNER_COMPUTE_PREFIX],
                          vnic_type=portbindings.VNIC_NORMAL,
@@ -310,15 +311,16 @@
                      port_id=port_id)
 
 
 def get_router_ports(port_id=None):
     """Returns filtered list of routers that may be relevant on CVX"""
     return get_ports(device_owners=[n_const.DEVICE_OWNER_DVR_INTERFACE,
                                     n_const.DEVICE_OWNER_ROUTER_HA_INTF,
-                                    n_const.DEVICE_OWNER_ROUTER_INTF],
+                                    n_const.DEVICE_OWNER_ROUTER_INTF,
+                                    n_const.DEVICE_OWNER_ROUTER_GW],
                      port_id=port_id)
 
 
 def get_vm_ports(port_id=None):
     """Returns filtered list of vms that may be relevant on CVX"""
     return get_ports(device_owners=[n_const.DEVICE_OWNER_COMPUTE_PREFIX,
                                     t_const.TRUNK_SUBPORT_OWNER],
```

### Comparing `networking_arista-2022.2.0/networking_arista/common/exceptions.py` & `networking_arista-2022.2.1/networking_arista/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/common/utils.py` & `networking_arista-2022.2.1/networking_arista/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 SUPPORTED_DEVICE_OWNERS = [
     n_const.DEVICE_OWNER_COMPUTE_PREFIX,
     n_const.DEVICE_OWNER_BAREMETAL_PREFIX,
     n_const.DEVICE_OWNER_DHCP,
     n_const.DEVICE_OWNER_DVR_INTERFACE,
     n_const.DEVICE_OWNER_ROUTER_HA_INTF,
     n_const.DEVICE_OWNER_ROUTER_INTF,
+    n_const.DEVICE_OWNER_ROUTER_GW,
     t_const.TRUNK_SUBPORT_OWNER]
 
 
 UNSUPPORTED_DEVICE_OWNERS = [
     n_const.DEVICE_OWNER_COMPUTE_PREFIX + 'probe']
```

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/env.py` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/script.py.mako` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/296b4e0236e0_initial_db_version.py` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/296b4e0236e0_initial_db_version.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/liberty/contract/47036dc8697a_initial_db_version_contract.py` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/liberty/contract/47036dc8697a_initial_db_version_contract.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/liberty/expand/1c6993ce7db0_initial_db_version_expand.py` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/liberty/expand/1c6993ce7db0_initial_db_version_expand.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/contract/39c2eeb67116_drop_aristaprovisionednets.py` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/contract/39c2eeb67116_drop_aristaprovisionednets.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/contract/941bad5630c1_drop_aristaprovisionedvms.py` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/contract/941bad5630c1_drop_aristaprovisionedvms.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/db/migration/alembic_migrations/versions/queens/contract/dc7bf9c1ab4d_drop_aristaprovisionedtenants.py` & `networking_arista-2022.2.1/networking_arista/db/migration/alembic_migrations/versions/queens/contract/dc7bf9c1ab4d_drop_aristaprovisionedtenants.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/l3Plugin/arista_l3_driver.py` & `networking_arista-2022.2.1/networking_arista/l3Plugin/arista_l3_driver.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/l3Plugin/l3_arista.py` & `networking_arista-2022.2.1/networking_arista/l3Plugin/l3_arista.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/arista_resources.py` & `networking_arista-2022.2.1/networking_arista/ml2/arista_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,36 +332,25 @@
                                     submodel='Port')]
     endpoint = 'region/%(region)s/dhcp'
     get_db_resources = staticmethod(db_lib.get_dhcp_instances)
 
 
 class Routers(AristaResourcesBase):
 
-    def set_router_host_id(device_owner, resource):
-        if device_owner == n_const.DEVICE_OWNER_ROUTER_HA_INTF:
-            return 'HA Router'
-
-        if device_owner == n_const.DEVICE_OWNER_DVR_INTERFACE:
-            return 'distributed'
-
-        if device_owner == n_const.DEVICE_OWNER_ROUTER_INTF:
-            portbinding = getattr(resource, 'PortBinding')
-            return utils.hostname(portbinding.host) if portbinding else ''
-
     def modify_blank_project_id(project_id, resource):
         if len(project_id) == 0:
             l3ha_router = getattr(resource, 'Router')
             if l3ha_router:
                 project_id = l3ha_router.project_id
         return project_id
 
     formatter = [AttributeFormatter('device_id', 'id',
                                     submodel='Port'),
                  AttributeFormatter('device_owner', 'hostId',
-                                    set_router_host_id,
+                                    lambda *args: '(see router ports)',
                                     submodel='Port'),
                  AttributeFormatter('project_id', 'tenantId',
                                     modify_blank_project_id,
                                     submodel='Port')]
     endpoint = 'region/%(region)s/router'
     get_db_resources = staticmethod(db_lib.get_router_instances)
```

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/arista_sync.py` & `networking_arista-2022.2.1/networking_arista/ml2/arista_sync.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/arista_trunk.py` & `networking_arista-2022.2.1/networking_arista/ml2/arista_trunk.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/mechanism_arista.py` & `networking_arista-2022.2.1/networking_arista/ml2/mechanism_arista.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
         if port[portbindings.VNIC_TYPE] == portbindings.VNIC_BAREMETAL:
             return a_const.BAREMETAL_RESOURCE
         owner_to_type = {
             n_const.DEVICE_OWNER_DHCP: a_const.DHCP_RESOURCE,
             n_const.DEVICE_OWNER_DVR_INTERFACE: a_const.ROUTER_RESOURCE,
             n_const.DEVICE_OWNER_ROUTER_INTF: a_const.ROUTER_RESOURCE,
             n_const.DEVICE_OWNER_ROUTER_HA_INTF: a_const.ROUTER_RESOURCE,
+            n_const.DEVICE_OWNER_ROUTER_GW: a_const.ROUTER_RESOURCE,
             trunk_consts.TRUNK_SUBPORT_OWNER: a_const.VM_RESOURCE}
         if port['device_owner'] in owner_to_type.keys():
             return owner_to_type[port['device_owner']]
         elif port['device_owner'].startswith(
                 n_const.DEVICE_OWNER_COMPUTE_PREFIX):
             return a_const.VM_RESOURCE
         return None
```

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/rpc/arista_eapi.py` & `networking_arista-2022.2.1/networking_arista/ml2/rpc/arista_eapi.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/rpc/arista_json.py` & `networking_arista-2022.2.1/networking_arista/ml2/rpc/arista_json.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/rpc/base.py` & `networking_arista-2022.2.1/networking_arista/ml2/rpc/base.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/security_groups/arista_security_groups.py` & `networking_arista-2022.2.1/networking_arista/ml2/security_groups/arista_security_groups.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/security_groups/security_group_sync.py` & `networking_arista-2022.2.1/networking_arista/ml2/security_groups/security_group_sync.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/security_groups/switch_helper.py` & `networking_arista-2022.2.1/networking_arista/ml2/security_groups/switch_helper.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/type_drivers/driver_helpers.py` & `networking_arista-2022.2.1/networking_arista/ml2/type_drivers/driver_helpers.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/ml2/type_drivers/type_arista_vlan.py` & `networking_arista-2022.2.1/networking_arista/ml2/type_drivers/type_arista_vlan.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/base.py` & `networking_arista-2022.2.1/networking_arista/tests/base.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/test_networking_arista.py` & `networking_arista-2022.2.1/networking_arista/tests/test_networking_arista.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/__init__.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/common/test_api.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/common/test_api.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/common/test_db_lib.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/common/test_db_lib.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/l3Plugin/__init__.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/l3Plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/l3Plugin/test_arista_l3_driver.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/l3Plugin/test_arista_l3_driver.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/__init__.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/__init__.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/mechanism_fabric.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/mechanism_fabric.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/mechanism_ha_simulator.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/mechanism_ha_simulator.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/ml2_test_base.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/ml2_test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from oslo_log import fixture as log_fixture
 
 import cProfile
 from eventlet import queue
 import mock
 from pstats import Stats
 
+from neutron_lib.api.definitions import l3 as l3_const
 from neutron_lib.api.definitions import portbindings
 from neutron_lib import constants as n_const
 import neutron_lib.context
 from neutron_lib.plugins import constants as p_const
 from neutron_lib.plugins import directory
 from neutron_lib.services.trunk import constants as trunk_const
 from oslo_config import cfg
@@ -421,22 +422,26 @@
     def _register_l3_agent(self, host):
         return helpers.register_l3_agent(host=host)
 
     def setUp(self):
         super(L3HARouterTestFramework, self).setUp()
         self.l3_plugin = directory.get_plugin(p_const.L3)
         self.l3_rpc_cb = l3_rpc.L3RpcCallback()
+        self.ext_net = None
 
-    def create_router(self, ha=False):
-        router = self.l3_plugin.create_router(
-            self.context, {'router': {'name': 'router',
-                                      'admin_state_up': True,
-                                      'tenant_id': self._tenant_id,
-                                      'ha': ha,
-                                      'distributed': False}})
+    def create_router(self, ha=False, ext_net=None):
+        router_dict = {'router': {'name': 'router',
+                                  'admin_state_up': True,
+                                  'tenant_id': self._tenant_id,
+                                  'ha': ha,
+                                  'distributed': False}}
+        if ext_net:
+            router_dict['router'][l3_const.EXTERNAL_GW_INFO] = {'network_id':
+                                                                ext_net['id']}
+        router = self.l3_plugin.create_router(self.context, router_dict)
         self.l3_plugin.schedule_router(self.context, router['id'])
         for host in self.l3_agents:
             self.sync_routers(router['id'], host['host'])
         return router
 
     def sync_routers(self, router_id, host):
         """Call to L3 Agent plugin sync_routers
@@ -499,26 +504,26 @@
         common_utils.wait_until_true(resource_created)
 
     def assertLegacyRouterCreated(self, router, host):
         endpoint = self._get_endpoint('router')
 
         def resource_created():
             cvx_data = list(self.cvx.endpoint_data[endpoint].values())
-            expected_data = {'hostId': host,
+            expected_data = {'hostId': '(see router ports)',
                              'tenantId': router['project_id'],
                              'id': router['id']}
             return cvx_data and cvx_data[0] == expected_data
         common_utils.wait_until_true(resource_created)
 
     def assertL3HARouterCreated(self, router):
         endpoint = self._get_endpoint('router')
 
         def resource_created():
             cvx_data = list(self.cvx.endpoint_data[endpoint].values())
-            expected_data = {'hostId': 'HA Router',
+            expected_data = {'hostId': '(see router ports)',
                              'tenantId': router['project_id'],
                              'id': router['id']}
             return cvx_data and cvx_data[0] == expected_data
         common_utils.wait_until_true(resource_created)
 
     def assertL3HAPortCreated(self, router, port_id):
         endpoint = self._get_endpoint('router_port')
```

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/rpc/test_arista_eapi_rpc_wrapper.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/rpc/test_arista_eapi_rpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/rpc/test_arista_json_rpc_wrapper.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/rpc/test_arista_json_rpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/sg_test_base.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/sg_test_base.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/test_arista_security_groups.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/test_arista_security_groups.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/security_groups/test_security_group_sync.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/security_groups/test_security_group_sync.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/test_arista_resources.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/test_arista_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,50 +576,50 @@
 
     def test_routers_scenario(self):
         id_base = n_const.DEVICE_OWNER_DVR_INTERFACE + 'normal'
         ha_id_base = n_const.DEVICE_OWNER_ROUTER_HA_INTF + 'normal'
         legacy_id_base = n_const.DEVICE_OWNER_ROUTER_INTF + 'normal'
         expect_created = {'%s1' % id_base:
                           {'tenantId': 't1',
-                           'hostId': 'distributed',
+                           'hostId': '(see router ports)',
                            'id': '%s1' % id_base},
                           '%s2' % id_base:
                           {'tenantId': 't2',
-                           'hostId': 'distributed',
+                           'hostId': '(see router ports)',
                            'id': '%s2' % id_base},
                           '%s' % ha_id_base:
                           {'tenantId': 'ha-router-project',
-                           'hostId': 'HA Router',
+                           'hostId': '(see router ports)',
                            'id': '%s' % ha_id_base},
                           '%s1' % legacy_id_base:
                           {'tenantId': 't1',
-                           'hostId': 'host1',
+                           'hostId': '(see router ports)',
                            'id': '%s1' % legacy_id_base},
                           '%s2' % legacy_id_base:
                           {'tenantId': 't2',
-                           'hostId': 'host2',
+                           'hostId': '(see router ports)',
                            'id': '%s2' % legacy_id_base}}
         self.run_scenario(expect_created)
 
     def test_routers_managed_physnets_scenario(self):
         cfg.CONF.set_override('managed_physnets', 'switch1', 'ml2_arista')
         id_base = n_const.DEVICE_OWNER_DVR_INTERFACE + 'normal'
         legacy_id_base = n_const.DEVICE_OWNER_ROUTER_INTF + 'normal'
         ha_id_base = n_const.DEVICE_OWNER_ROUTER_HA_INTF + 'normal'
         expect_created = {'%s2' % id_base:
                           {'tenantId': 't2',
-                           'hostId': 'distributed',
+                           'hostId': '(see router ports)',
                            'id': '%s2' % id_base},
                           '%s2' % legacy_id_base:
                           {'id': '%s2' % legacy_id_base,
                            'tenantId': 't2',
-                           'hostId': 'host2'},
+                           'hostId': '(see router ports)'},
                           '%s' % ha_id_base:
                           {'tenantId': 'ha-router-project',
-                           'hostId': 'HA Router',
+                           'hostId': '(see router ports)',
                            'id': '%s' % ha_id_base}}
         self.run_scenario(expect_created)
 
 
 class AristaVmTest(AristaInstancesTestBase):
     """Test cases for creation & deletion of arista vms"""
```

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/test_arista_sync.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/test_arista_sync.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/test_mechanism_arista.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/test_mechanism_arista.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import mock
 
 from neutron.tests.common import helpers
+from neutron_lib.api.definitions import external_net as extnet_const
 from neutron_lib import constants as n_const
 from oslo_config import cfg
 
 from networking_arista.tests.unit.ml2 import ml2_test_base
 
 from neutron_lib.api.definitions import portbindings
 
@@ -1321,60 +1322,81 @@
         self.delete_port(port_2['id'])
         self.assertTenantDeleted(port_tenant)
 
 
 class BasicL3HARouterTests(object):
 
     def test_create_delete_router(self):
-        ha_router_ports = []
-        router = self.create_router(ha=True)
+        router_ports = []
+        ext_net = None
+        if self.ext_net:
+            ext_net, ext_net_ctx = self.create_network(self.ext_net)
+        router = self.create_router(ha=True, ext_net=ext_net)
         for l3_agent in self.l3_agents:
             port = self.update_routers_states(router['id'], l3_agent)
-            ha_router_ports.append(port)
+            router_ports.append(port)
         ha_network_id = self.get_ha_network(router)
-        ha_segments = self.get_network_segments(ha_network_id)
+        segments = self.get_network_segments(ha_network_id)
+        if self.ext_net:
+            segments.extend(self.get_network_segments(ext_net['id']))
+            router_ports.append(self.plugin.get_port(self.context,
+                                                     router['gw_port_id']))
         self.assertTenantCreated(router['project_id'])
         self.assertL3HANetworkCreated(router, ha_network_id)
         self.assertRouterCreated(router['id'])
         self.assertL3HARouterCreated(router)
-        for port in ha_router_ports:
-            self.assertL3HAPortCreated(router, port['id'])
+        for port in router_ports:
+            if port['device_owner'] != n_const.DEVICE_OWNER_ROUTER_GW:
+                self.assertL3HAPortCreated(router, port['id'])
+            else:
+                self.assertRouterPortCreated(port['id'])
             self.assertPortBindingCreated((port['id'],
                                            port[portbindings.HOST_ID]))
-        self.assertSegmentsCreated(ha_segments)
+        self.assertSegmentsCreated(segments)
 
         # Delete the router
         self.delete_router(router['id'])
-        self.assertRouterPortsDeleted([p['id'] for p in ha_router_ports])
+        if self.ext_net:
+            self.delete_network(ext_net['id'])
+        self.assertRouterPortsDeleted([p['id'] for p in router_ports])
         self.assertRouterDeleted(router['id'])
-        self.assertSegmentsDeleted(ha_segments)
+        self.assertSegmentsDeleted(segments)
         self.assertNetworkDeleted(ha_network_id)
         self.assertTenantDeleted(router['project_id'])
-        for port in ha_router_ports:
+        for port in router_ports:
             self.assertPortBindingDeleted((port['id'],
                                            port[portbindings.HOST_ID]))
 
 
 class BasicRouterTests(object):
+
     def test_create_delete_router(self):
-        router = self.create_router()
         net_list = []
         port_list = []
         segment_list = []
+        ext_net = None
+        if self.ext_net:
+            ext_net, ext_net_ctx = self.create_network(self.ext_net)
+        router = self.create_router(ext_net=ext_net)
         for net in self.net_dict:
             network, net_ctx = self.create_network(net)
             net_list.append((network, net_ctx))
         self.assertTenantCreated(router['project_id'])
         for net, net_ctx in net_list:
             interface_info = {'subnet_id': net_ctx.current['subnets'][0]}
             intf = self.add_router_interface(router, interface_info)
             self.sync_routers(router['id'], self.l3_agent1['host'])
             port = self.get_legacy_router_port(intf['port_id'])
             self.assertNotEqual(len(port), 0)
             port_list.append(port)
+        if self.ext_net:
+            net_list.append((ext_net, ext_net_ctx))
+            port = self.get_legacy_router_port(router['gw_port_id'])
+            self.assertNotEqual(len(port), 0)
+            port_list.append(port)
         self.assertLegacyRouterCreated(router, self.l3_agent1['host'])
         for network, _ in net_list:
             self.assertNetworkCreated(network['id'])
             segment_list.extend(self.get_network_segments(network['id']))
         self.assertEqual(len(segment_list), self.total_segments)
         self.assertSegmentsCreated(segment_list)
         for port in port_list:
@@ -1392,19 +1414,31 @@
         self.assertPortBindingDeleted((intf['port_id'],
                                        port[portbindings.HOST_ID]))
 
         # Remove second router interface
         network, net_ctx = net_list[1]
         interface_info = {'subnet_id': net_ctx.current['subnets'][0]}
         intf = self.remove_router_interface(router, interface_info)
-        self.assertRouterDeleted(router['id'])
+        # If there's still an external gateway port, the router will
+        # still exist on CVX. Otherwise, it will be deleted
+        if not self.ext_net:
+            self.assertRouterDeleted(router['id'])
+        else:
+            self.assertRouterCreated(router['id'])
         self.assertRouterPortDeleted(intf['port_id'])
         self.assertPortBindingDeleted((intf['port_id'],
                                        port[portbindings.HOST_ID]))
 
+        # Delete router to delete external gateway port
+        self.delete_router(router['id'])
+        self.assertRouterDeleted(router['id'])
+        self.assertRouterPortDeleted(router['gw_port_id'])
+        self.assertPortBindingDeleted((router['gw_port_id'],
+                                       port[portbindings.HOST_ID]))
+
         for network, _ in net_list:
             self.delete_network(network['id'])
             self.assertNetworkDeleted(network['id'])
         self.assertSegmentsDeleted(segment_list)
 
 
 class BasicL3HARouterTestCases(ml2_test_base.L3HARouterTestFramework,
@@ -1479,7 +1513,51 @@
         self.net_dict = [{'network': {'name': 'hpb_net-%d' % r,
                                       'tenant_id': self._tenant_id,
                                       'admin_state_up': True,
                                       'shared': False}}
                          for r in range(1, 3)]
         self.total_segments = 4
         self.l3_agents = [self.l3_agent1]
+
+
+class RouterGatewayTestCases(ml2_test_base.L3HARouterTestFramework,
+                             BasicRouterTests):
+    def setUp(self):
+        cfg.CONF.set_override('tenant_network_types', 'vlan', 'ml2')
+        super(RouterGatewayTestCases, self).setUp()
+        self.l3_agent1 = self._register_l3_agent(host=self.host1)
+        self.ext_net = {'network': {'name': 'ext_net',
+                                    'tenant_id': self._tenant_id,
+                                    'admin_state_up': True,
+                                    'shared': False,
+                                    'provider:physical_network': self.physnet,
+                                    'provider:network_type': 'vlan',
+                                    extnet_const.EXTERNAL: True}}
+        self.net_dict = [
+            {'network': {'name': 'net-%d' % r,
+                         'tenant_id': self._tenant_id,
+                         'admin_state_up': True,
+                         'shared': False,
+                         'provider:physical_network': self.physnet,
+                         'provider:network_type': 'vlan'}}
+            for r in range(1, 3)]
+        self.total_segments = 3
+        self.l3_agents = [self.l3_agent1]
+
+
+class RouterGatewayL3HARouterTestCases(ml2_test_base.L3HARouterTestFramework,
+                                       BasicL3HARouterTests):
+
+    def setUp(self):
+        cfg.CONF.set_override('tenant_network_types', 'vlan', 'ml2')
+        super(RouterGatewayL3HARouterTestCases, self).setUp()
+        cfg.CONF.set_override('max_l3_agents_per_router', 2)
+        self.l3_agent1 = self._register_l3_agent(host=self.host1)
+        self.l3_agent2 = self._register_l3_agent(host=self.host2)
+        self.l3_agents = [self.l3_agent1, self.l3_agent2]
+        self.ext_net = {'network': {'name': 'ext_net',
+                                    'tenant_id': self._tenant_id,
+                                    'admin_state_up': True,
+                                    'shared': False,
+                                    'provider:physical_network': self.physnet,
+                                    'provider:network_type': 'vlan',
+                                    extnet_const.EXTERNAL: True}}
```

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/ml2/type_drivers/test_arista_type_driver.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/ml2/type_drivers/test_arista_type_driver.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista/tests/unit/utils.py` & `networking_arista-2022.2.1/networking_arista/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista.egg-info/PKG-INFO` & `networking_arista-2022.2.1/networking_arista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: networking-arista
-Version: 2022.2.0
+Version: 2022.2.1
 Summary: Arista Networking drivers
 Home-page: https://opendev.org/x/networking-arista/
 Author: Arista Networks
 Author-email: openstack-dev@arista.com
 License: UNKNOWN
 Description: ===============================
         networking-arista
```

### Comparing `networking_arista-2022.2.0/networking_arista.egg-info/SOURCES.txt` & `networking_arista-2022.2.1/networking_arista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/networking_arista.egg-info/entry_points.txt` & `networking_arista-2022.2.1/networking_arista.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/requirements.txt` & `networking_arista-2022.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/setup.cfg` & `networking_arista-2022.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/setup.py` & `networking_arista-2022.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `networking_arista-2022.2.0/tox.ini` & `networking_arista-2022.2.1/tox.ini`

 * *Files identical despite different names*

