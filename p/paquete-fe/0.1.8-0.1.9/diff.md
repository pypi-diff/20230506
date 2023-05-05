# Comparing `tmp/paquete-fe-0.1.8.tar.gz` & `tmp/paquete_fe-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paquete-fe-0.1.8.tar", last modified: Fri May  5 23:34:01 2023, max compression
+gzip compressed data, was "paquete_fe-0.1.9.tar", max compression
```

## Comparing `paquete-fe-0.1.8.tar` & `paquete_fe-0.1.9.tar`

### file list

```diff
@@ -1,88 +1,67 @@
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/
--rw-r--r--   0 aortiz     (501) staff       (20)      472 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/PKG-INFO
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:17:07.000000 paquete-fe-0.1.8/paquetefe/__init__.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/set/
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:38.000000 paquete-fe-0.1.8/paquetefe/set/__init__.py
--rw-r--r--   0 aortiz     (501) staff       (20)     1712 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/cert_manager.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/
--rw-r--r--   0 aortiz     (501) staff       (20)     2141 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-ruc.wsdl
--rw-r--r--   0 aortiz     (501) staff       (20)    20224 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/Evento_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      379 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/siRecepEvento_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    43942 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-ruc.wsdl.xsd1.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:44.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/__init__.py
--rw-r--r--   0 aortiz     (501) staff       (20)    27146 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/Evento_Types_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    10293 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/xmldsig-core-schema.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    45782 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-lote.wsdl.xsd1.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)     2106 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/evento.wsdl
--rw-r--r--   0 aortiz     (501) staff       (20)     8116 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/evento.wsdl.xsd2.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)     2185 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-lote.wsdl
--rw-r--r--   0 aortiz     (501) staff       (20)    38647 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/evento.wsdl.xsd1.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)     3242 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/wsdl/WS_SiConsRUC_v141.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)     7772 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/set/set_service.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/de_classes/
--rw-r--r--   0 aortiz     (501) staff       (20)     3459 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/gen_xml.py
--rw-r--r--   0 aortiz     (501) staff       (20)     9243 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/estructura_nodos_xml.csv
--rw-r--r--   0 aortiz     (501) staff       (20)   383102 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/referencia_geografica.csv
--rw-r--r--   0 aortiz     (501) staff       (20)      635 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/test_validate_xsd_eventos.py
--rw-r--r--   0 aortiz     (501) staff       (20)     4656 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/geography_reference.py
--rw-r--r--   0 aortiz     (501) staff       (20)     4236 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/countries_iso3166.csv
--rw-r--r--   0 aortiz     (501) staff       (20)     1219 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/globals.py
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/__init__.py
--rw-r--r--   0 aortiz     (501) staff       (20)   119783 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/mysql_db_admin.py
--rw-r--r--   0 aortiz     (501) staff       (20)    16673 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/vistas.py
--rw-r--r--   0 aortiz     (501) staff       (20)     3456 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/validate.py
--rw-r--r--   0 aortiz     (501) staff       (20)     1933 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_provider.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/
--rw-r--r--   0 aortiz     (501) staff       (20)    20329 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/Evento_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      416 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/siRecepEvento_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    79525 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/DE_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      411 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/siRecepEventoReceptor_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      394 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/siRecepDE_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:54.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/__init__.py
--rw-r--r--   0 aortiz     (501) staff       (20)    27583 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/Evento_Types_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      409 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/siRecepEventoEmisor_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    29554 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/utils.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/
--rw-r--r--   0 aortiz     (501) staff       (20)    20195 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Evento_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      297 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/siRecepEvento_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    64382 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/DE_Types_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    79192 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/DE_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      364 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/siRecepEventoReceptor_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      222 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/siRecepDE_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:51.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/__init__.py
--rw-r--r--   0 aortiz     (501) staff       (20)    27537 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Evento_Types_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    14927 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Unidades_Medida_v141.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    10190 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/xmldsig-core-schema.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    55709 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Monedas_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)      362 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/siRecepEventoEmisor_v150.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)    52000 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Paises_v100.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)     5965 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Departamentos_v141.xsd
--rw-r--r--   0 aortiz     (501) staff       (20)     2444 2023-05-05 21:23:32.000000 paquete-fe-0.1.8/paquetefe/de_classes/process_mysql.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/factury/
--rw-r--r--   0 aortiz     (501) staff       (20)    18695 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/factury/factury_service_client.py
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:56.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/factury/__init__.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/cima/
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/cima/__init__.py
--rw-r--r--   0 aortiz     (501) staff       (20)    19121 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/cima/cima_service_client.py
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:47.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/__init__.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/code100/
--rw-r--r--   0 aortiz     (501) staff       (20)        0 2023-05-05 21:38:57.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/code100/__init__.py
--rw-r--r--   0 aortiz     (501) staff       (20)    18596 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/code100/code100_service_client.py
--rw-r--r--   0 aortiz     (501) staff       (20)     2105 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/validaciones.txt
--rw-r--r--   0 aortiz     (501) staff       (20)       23 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/settings.py
--rw-r--r--   0 aortiz     (501) staff       (20)     2174 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/eventos.py
--rw-r--r--   0 aortiz     (501) staff       (20)     4326 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/xml_namespace_local.xml
--rw-r--r--   0 aortiz     (501) staff       (20)     8633 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/paquetefe/de_classes/currency_iso_4217_table.csv
--rw-r--r--   0 aortiz     (501) staff       (20)      463 2023-05-05 23:33:55.000000 paquete-fe-0.1.8/pyproject.toml
--rw-r--r--   0 aortiz     (501) staff       (20)       52 2023-05-05 23:33:50.000000 paquete-fe-0.1.8/MANIFEST.in
--rw-r--r--   0 aortiz     (501) staff       (20)       14 2023-05-05 16:51:58.000000 paquete-fe-0.1.8/README.md
--rw-r--r--   0 aortiz     (501) staff       (20)      701 2023-05-05 23:30:45.000000 paquete-fe-0.1.8/setup.py
-drwxr-xr-x   0 aortiz     (501) staff       (20)        0 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquete_fe.egg-info/
--rw-r--r--   0 aortiz     (501) staff       (20)      472 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquete_fe.egg-info/PKG-INFO
--rw-r--r--   0 aortiz     (501) staff       (20)     3156 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquete_fe.egg-info/SOURCES.txt
--rw-r--r--   0 aortiz     (501) staff       (20)       45 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquete_fe.egg-info/requires.txt
--rw-r--r--   0 aortiz     (501) staff       (20)       10 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquete_fe.egg-info/top_level.txt
--rw-r--r--   0 aortiz     (501) staff       (20)        1 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/paquete_fe.egg-info/dependency_links.txt
--rw-r--r--   0 aortiz     (501) staff       (20)       38 2023-05-05 23:34:01.000000 paquete-fe-0.1.8/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-05 21:17:07.508253 paquete_fe-0.1.9/paquetefe/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:51:58.124674 paquete_fe-0.1.9/paquetefe/de_classes/__init__.py
+-rw-r--r--   0        0        0     4236 2023-05-05 16:51:58.124859 paquete_fe-0.1.9/paquetefe/de_classes/countries_iso3166.csv
+-rw-r--r--   0        0        0     8633 2023-05-05 16:51:58.125046 paquete_fe-0.1.9/paquetefe/de_classes/currency_iso_4217_table.csv
+-rw-r--r--   0        0        0     9243 2023-05-05 16:51:58.125214 paquete_fe-0.1.9/paquetefe/de_classes/estructura_nodos_xml.csv
+-rw-r--r--   0        0        0     2174 2023-05-05 16:51:58.125398 paquete_fe-0.1.9/paquetefe/de_classes/eventos.py
+-rw-r--r--   0        0        0     3459 2023-05-05 16:51:58.125664 paquete_fe-0.1.9/paquetefe/de_classes/gen_xml.py
+-rw-r--r--   0        0        0     4656 2023-05-05 16:51:58.125815 paquete_fe-0.1.9/paquetefe/de_classes/geography_reference.py
+-rw-r--r--   0        0        0     1219 2023-05-05 16:51:58.125991 paquete_fe-0.1.9/paquetefe/de_classes/globals.py
+-rw-r--r--   0        0        0   119783 2023-05-05 16:51:58.126894 paquete_fe-0.1.9/paquetefe/de_classes/mysql_db_admin.py
+-rw-r--r--   0        0        0     2444 2023-05-05 21:23:32.704523 paquete_fe-0.1.9/paquetefe/de_classes/process_mysql.py
+-rw-r--r--   0        0        0   383102 2023-05-05 16:51:58.128654 paquete_fe-0.1.9/paquetefe/de_classes/referencia_geografica.csv
+-rw-r--r--   0        0        0       23 2023-05-05 16:51:58.128812 paquete_fe-0.1.9/paquetefe/de_classes/settings.py
+-rw-r--r--   0        0        0     1933 2023-05-05 16:51:58.128947 paquete_fe-0.1.9/paquetefe/de_classes/signature_provider.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:47.988535 paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:58.595775 paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/cima/__init__.py
+-rw-r--r--   0        0        0    19121 2023-05-05 16:51:58.129294 paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/cima/cima_service_client.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:57.659360 paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/code100/__init__.py
+-rw-r--r--   0        0        0    18596 2023-05-05 16:51:58.129642 paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/code100/code100_service_client.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:56.220223 paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/factury/__init__.py
+-rw-r--r--   0        0        0    18695 2023-05-05 16:51:58.129953 paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/factury/factury_service_client.py
+-rw-r--r--   0        0        0      635 2023-05-05 16:51:58.130135 paquete_fe-0.1.9/paquetefe/de_classes/test_validate_xsd_eventos.py
+-rw-r--r--   0        0        0    29554 2023-05-05 16:51:58.130379 paquete_fe-0.1.9/paquetefe/de_classes/utils.py
+-rw-r--r--   0        0        0     2105 2023-05-05 16:51:58.130569 paquete_fe-0.1.9/paquetefe/de_classes/validaciones.txt
+-rw-r--r--   0        0        0     3456 2023-05-05 16:51:58.130718 paquete_fe-0.1.9/paquetefe/de_classes/validate.py
+-rw-r--r--   0        0        0    16673 2023-05-05 16:51:58.130952 paquete_fe-0.1.9/paquetefe/de_classes/vistas.py
+-rw-r--r--   0        0        0     4326 2023-05-05 16:51:58.131140 paquete_fe-0.1.9/paquetefe/de_classes/xml_namespace_local.xml
+-rw-r--r--   0        0        0    64382 2023-05-05 16:51:58.131761 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/DE_Types_v150.xsd
+-rw-r--r--   0        0        0    79192 2023-05-05 16:51:58.132339 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/DE_v150.xsd
+-rw-r--r--   0        0        0     5965 2023-05-05 16:51:58.132545 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Departamentos_v141.xsd
+-rw-r--r--   0        0        0    27537 2023-05-05 16:51:58.132782 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Evento_Types_v150.xsd
+-rw-r--r--   0        0        0    20195 2023-05-05 16:51:58.133020 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Evento_v150.xsd
+-rw-r--r--   0        0        0    55709 2023-05-05 16:51:58.133338 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Monedas_v150.xsd
+-rw-r--r--   0        0        0    52000 2023-05-05 16:51:58.133751 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Paises_v100.xsd
+-rw-r--r--   0        0        0    14927 2023-05-05 16:51:58.134007 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Unidades_Medida_v141.xsd
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:51.069174 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/__init__.py
+-rw-r--r--   0        0        0      222 2023-05-05 16:51:58.134343 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/siRecepDE_v150.xsd
+-rw-r--r--   0        0        0      362 2023-05-05 16:51:58.134593 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/siRecepEventoEmisor_v150.xsd
+-rw-r--r--   0        0        0      364 2023-05-05 16:51:58.134827 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/siRecepEventoReceptor_v150.xsd
+-rw-r--r--   0        0        0      297 2023-05-05 16:51:58.135043 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/siRecepEvento_v150.xsd
+-rw-r--r--   0        0        0    10190 2023-05-05 16:51:58.135325 paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/xmldsig-core-schema.xsd
+-rw-r--r--   0        0        0    79525 2023-05-05 16:51:58.135848 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/DE_v150.xsd
+-rw-r--r--   0        0        0    27583 2023-05-05 16:51:58.136143 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/Evento_Types_v150.xsd
+-rw-r--r--   0        0        0    20329 2023-05-05 16:51:58.136450 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/Evento_v150.xsd
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:54.028346 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/__init__.py
+-rw-r--r--   0        0        0      394 2023-05-05 16:51:58.136682 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/siRecepDE_v150.xsd
+-rw-r--r--   0        0        0      409 2023-05-05 16:51:58.136888 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/siRecepEventoEmisor_v150.xsd
+-rw-r--r--   0        0        0      411 2023-05-05 16:51:58.137132 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/siRecepEventoReceptor_v150.xsd
+-rw-r--r--   0        0        0      416 2023-05-05 16:51:58.137321 paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/siRecepEvento_v150.xsd
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:38.859927 paquete_fe-0.1.9/paquetefe/set/__init__.py
+-rw-r--r--   0        0        0     1712 2023-05-05 16:51:58.137851 paquete_fe-0.1.9/paquetefe/set/cert_manager.py
+-rw-r--r--   0        0        0     7772 2023-05-05 16:51:58.138132 paquete_fe-0.1.9/paquetefe/set/set_service.py
+-rw-r--r--   0        0        0    27146 2023-05-05 16:51:58.138504 paquete_fe-0.1.9/paquetefe/set/wsdl/Evento_Types_v150.xsd
+-rw-r--r--   0        0        0    20224 2023-05-05 16:51:58.138787 paquete_fe-0.1.9/paquetefe/set/wsdl/Evento_v150.xsd
+-rw-r--r--   0        0        0     3242 2023-05-05 16:51:58.139020 paquete_fe-0.1.9/paquetefe/set/wsdl/WS_SiConsRUC_v141.xsd
+-rw-r--r--   0        0        0        0 2023-05-05 21:38:44.998720 paquete_fe-0.1.9/paquetefe/set/wsdl/__init__.py
+-rw-r--r--   0        0        0     2185 2023-05-05 16:51:58.139255 paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-lote.wsdl
+-rw-r--r--   0        0        0    45782 2023-05-05 16:51:58.139751 paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-lote.wsdl.xsd1.xsd
+-rw-r--r--   0        0        0     2141 2023-05-05 16:51:58.140124 paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-ruc.wsdl
+-rw-r--r--   0        0        0    43942 2023-05-05 16:51:58.140659 paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-ruc.wsdl.xsd1.xsd
+-rw-r--r--   0        0        0     2106 2023-05-05 16:51:58.140898 paquete_fe-0.1.9/paquetefe/set/wsdl/evento.wsdl
+-rw-r--r--   0        0        0    38647 2023-05-05 16:51:58.141291 paquete_fe-0.1.9/paquetefe/set/wsdl/evento.wsdl.xsd1.xsd
+-rw-r--r--   0        0        0     8116 2023-05-05 16:51:58.141656 paquete_fe-0.1.9/paquetefe/set/wsdl/evento.wsdl.xsd2.xsd
+-rw-r--r--   0        0        0      379 2023-05-05 16:51:58.141962 paquete_fe-0.1.9/paquetefe/set/wsdl/siRecepEvento_v150.xsd
+-rw-r--r--   0        0        0    10293 2023-05-05 16:51:58.142230 paquete_fe-0.1.9/paquetefe/set/wsdl/xmldsig-core-schema.xsd
+-rw-r--r--   0        0        0      463 2023-05-05 23:37:09.465493 paquete_fe-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 paquete_fe-0.1.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `paquete-fe-0.1.8/paquetefe/set/cert_manager.py` & `paquete_fe-0.1.9/paquetefe/set/cert_manager.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-ruc.wsdl` & `paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-ruc.wsdl`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/Evento_v150.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/Evento_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-ruc.wsdl.xsd1.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-ruc.wsdl.xsd1.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/Evento_Types_v150.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/Evento_Types_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/xmldsig-core-schema.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-lote.wsdl.xsd1.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-lote.wsdl.xsd1.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/evento.wsdl` & `paquete_fe-0.1.9/paquetefe/set/wsdl/evento.wsdl`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/evento.wsdl.xsd2.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/evento.wsdl.xsd2.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/consulta-lote.wsdl` & `paquete_fe-0.1.9/paquetefe/set/wsdl/consulta-lote.wsdl`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/evento.wsdl.xsd1.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/evento.wsdl.xsd1.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/wsdl/WS_SiConsRUC_v141.xsd` & `paquete_fe-0.1.9/paquetefe/set/wsdl/WS_SiConsRUC_v141.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/set/set_service.py` & `paquete_fe-0.1.9/paquetefe/set/set_service.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/gen_xml.py` & `paquete_fe-0.1.9/paquetefe/de_classes/gen_xml.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/estructura_nodos_xml.csv` & `paquete_fe-0.1.9/paquetefe/de_classes/estructura_nodos_xml.csv`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/referencia_geografica.csv` & `paquete_fe-0.1.9/paquetefe/de_classes/referencia_geografica.csv`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/test_validate_xsd_eventos.py` & `paquete_fe-0.1.9/paquetefe/de_classes/test_validate_xsd_eventos.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/geography_reference.py` & `paquete_fe-0.1.9/paquetefe/de_classes/geography_reference.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/countries_iso3166.csv` & `paquete_fe-0.1.9/paquetefe/de_classes/countries_iso3166.csv`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/globals.py` & `paquete_fe-0.1.9/paquetefe/de_classes/globals.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/mysql_db_admin.py` & `paquete_fe-0.1.9/paquetefe/de_classes/mysql_db_admin.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/vistas.py` & `paquete_fe-0.1.9/paquetefe/de_classes/vistas.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/validate.py` & `paquete_fe-0.1.9/paquetefe/de_classes/validate.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/signature_provider.py` & `paquete_fe-0.1.9/paquetefe/de_classes/signature_provider.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/Evento_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/Evento_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/DE_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/DE_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_sifen/Evento_Types_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_sifen/Evento_Types_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/utils.py` & `paquete_fe-0.1.9/paquetefe/de_classes/utils.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Evento_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Evento_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/DE_Types_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/DE_Types_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/DE_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/DE_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Evento_Types_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Evento_Types_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Unidades_Medida_v141.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Unidades_Medida_v141.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/xmldsig-core-schema.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Monedas_v150.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Monedas_v150.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Paises_v100.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Paises_v100.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xsd_files/Departamentos_v141.xsd` & `paquete_fe-0.1.9/paquetefe/de_classes/xsd_files/Departamentos_v141.xsd`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/process_mysql.py` & `paquete_fe-0.1.9/paquetefe/de_classes/process_mysql.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/factury/factury_service_client.py` & `paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/factury/factury_service_client.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/cima/cima_service_client.py` & `paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/cima/cima_service_client.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/signature_providers/code100/code100_service_client.py` & `paquete_fe-0.1.9/paquetefe/de_classes/signature_providers/code100/code100_service_client.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/validaciones.txt` & `paquete_fe-0.1.9/paquetefe/de_classes/validaciones.txt`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/eventos.py` & `paquete_fe-0.1.9/paquetefe/de_classes/eventos.py`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/xml_namespace_local.xml` & `paquete_fe-0.1.9/paquetefe/de_classes/xml_namespace_local.xml`

 * *Files identical despite different names*

### Comparing `paquete-fe-0.1.8/paquetefe/de_classes/currency_iso_4217_table.csv` & `paquete_fe-0.1.9/paquetefe/de_classes/currency_iso_4217_table.csv`

 * *Files identical despite different names*

