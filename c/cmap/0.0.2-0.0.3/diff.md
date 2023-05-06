# Comparing `tmp/cmap-0.0.2.tar.gz` & `tmp/cmap-0.0.3.tar.gz`

## Comparing `cmap-0.0.2.tar` & `cmap-0.0.3.tar`

### file list

```diff
@@ -1,196 +1,197 @@
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/__init__.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/_catalog.py
--rw-r--r--   0        0        0    20363 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/_color.py
--rw-r--r--   0        0        0    45461 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/_colormap.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/_external.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/_png.py
--rw-r--r--   0        0        0    16254 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/__init__.py
--rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/bids/__init__.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/bids/record.json
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/chrisluts/record.json
--rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cividis/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cividis/record.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmap/record.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/__init__.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/algae.py
--rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/amp.py
--rw-r--r--   0        0        0    22339 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/balance.py
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/curl.py
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/deep.py
--rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/delta.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/dense.py
--rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/diff.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/haline.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/ice.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/matter.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/oxy.py
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/phase.py
--rw-r--r--   0        0        0    17189 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/rain.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/record.json
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/solar.py
--rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/speed.py
--rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/tarn.py
--rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/tempo.py
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/thermal.py
--rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/topo.py
--rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cmocean/turbid.py
--rw-r--r--   0        0        0    39760 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorbrewer/__init__.py
--rw-r--r--   0        0        0    45183 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorbrewer/record.json
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C1.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C10.py
--rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C11.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C2.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C3.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C4.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C5.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C6.py
--rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C7.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C8.py
--rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_C9.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBC1.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBC2.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBD1.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBD2.py
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBL1.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBL2.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBL3.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBL4.py
--rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBTC1.py
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBTC2.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBTD1.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL1.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL2.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL3.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL4.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D1.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D10.py
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D11.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D12.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D13.py
--rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D1A.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D2.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D3.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D4.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D5.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D6.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D7.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D8.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_D9.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_I1.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_I2.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_I3.py
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L1.py
--rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L10.py
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L11.py
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L12.py
--rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L13.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L14.py
--rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L15.py
--rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L16.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L17.py
--rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L18.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L19.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L2.py
--rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L20.py
--rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L3.py
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L4.py
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L5.py
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L6.py
--rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L7.py
--rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L8.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_L9.py
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_R1.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_R2.py
--rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_R3.py
--rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/CET_R4.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/__init__.py
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/colorcet/record.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/__init__.py
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/acton.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/bam.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/bamO.py
--rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/bamako.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/batlow.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/batlowK.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/batlowW.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/berlin.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/bilbao.py
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/broc.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/brocO.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/buda.py
--rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/bukavu.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/cork.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/corkO.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/davos.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/devon.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/fes.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/grayC.py
--rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/hawaii.py
--rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/imola.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/lajolla.py
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/lapaz.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/lisbon.py
--rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/nuuk.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/oleron.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/oslo.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/record.json
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/roma.py
--rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/romaO.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/tofino.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/tokyo.py
--rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/turku.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/vanimo.py
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/vik.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/crameri/vikO.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cubehelix/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/cubehelix/record.json
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/glasbey/__init__.py
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/glasbey/_glasbey.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/glasbey/_grids.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/glasbey/_internals.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/glasbey/prebuilt.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/glasbey/record.json
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/gnuplot/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/gnuplot/record.json
--rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/google/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/google/record.json
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/imagej/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/imagej/record.json
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/matlab/__init__.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/matlab/record.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/matplotlib/_CMRmap.py
--rw-r--r--   0        0        0    45909 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/matplotlib/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/matplotlib/_coolwarm.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/matplotlib/_wistia.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/matplotlib/record.json
--rw-r--r--   0        0        0    64086 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/seaborn/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/seaborn/record.json
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/tableau/__init__.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/tableau/record.json
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/vispy/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/vispy/record.json
--rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/yorick/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmap-0.0.2/src/cmap/data/yorick/record.json
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_catalog.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_color.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_colormap.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_data.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_glasbey.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_model_fields.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_third_party.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 cmap-0.0.2/tests/test_utils.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cmap-0.0.2/.gitignore
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 cmap-0.0.2/README.md
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cmap-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_CMOCEAN
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_COLORBREWER
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_COLORCET
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_CRAMERI
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_CVIDIS
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_GLASBEY
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_WISTIA
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 cmap-0.0.2/LICENSE/LICENSE_YORICK
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 cmap-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/__init__.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/_catalog.py
+-rw-r--r--   0        0        0    20363 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/_color.py
+-rw-r--r--   0        0        0    45461 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/_colormap.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/_external.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/_png.py
+-rw-r--r--   0        0        0    16254 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/__init__.py
+-rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/bids/__init__.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/bids/record.json
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/chrisluts/record.json
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cividis/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cividis/record.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmap/record.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/__init__.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/algae.py
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/amp.py
+-rw-r--r--   0        0        0    22339 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/balance.py
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/curl.py
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/deep.py
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/delta.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/dense.py
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/diff.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/haline.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/ice.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/matter.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/oxy.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/phase.py
+-rw-r--r--   0        0        0    17189 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/rain.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/record.json
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/solar.py
+-rw-r--r--   0        0        0    17281 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/speed.py
+-rw-r--r--   0        0        0    21589 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/tarn.py
+-rw-r--r--   0        0        0    17165 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/tempo.py
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/thermal.py
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/topo.py
+-rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cmocean/turbid.py
+-rw-r--r--   0        0        0    39760 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorbrewer/__init__.py
+-rw-r--r--   0        0        0    45183 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorbrewer/record.json
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C1.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C10.py
+-rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C11.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C2.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C4.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C5.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C6.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C7.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C8.py
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_C9.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBC1.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBC2.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBD1.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBD2.py
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBL1.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBL3.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBL4.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBTC1.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBTC2.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBTD1.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL1.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL2.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL3.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL4.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D1.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D10.py
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D11.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D12.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D13.py
+-rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D1A.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D2.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D3.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D4.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D5.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D6.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D7.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D8.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_D9.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_I1.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_I2.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_I3.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L1.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L10.py
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L11.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L12.py
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L13.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L14.py
+-rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L15.py
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L16.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L17.py
+-rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L18.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L19.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L2.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L20.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L3.py
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L4.py
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L5.py
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L6.py
+-rw-r--r--   0        0        0     9072 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L7.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L8.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_L9.py
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_R1.py
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_R2.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_R3.py
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/CET_R4.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/__init__.py
+-rw-r--r--   0        0        0    19688 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/colorcet/record.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/__init__.py
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/acton.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/bam.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/bamO.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/bamako.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/batlow.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/batlowK.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/batlowW.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/berlin.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/bilbao.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/broc.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/brocO.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/buda.py
+-rw-r--r--   0        0        0     9215 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/bukavu.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/cork.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/corkO.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/davos.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/devon.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/fes.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/grayC.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/hawaii.py
+-rw-r--r--   0        0        0     9227 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/imola.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/lajolla.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/lapaz.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/lisbon.py
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/nuuk.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/oleron.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/oslo.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/record.json
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/roma.py
+-rw-r--r--   0        0        0     9217 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/romaO.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/tofino.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/tokyo.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/turku.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/vanimo.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/vik.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/crameri/vikO.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cubehelix/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/cubehelix/record.json
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/glasbey/__init__.py
+-rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/glasbey/_glasbey.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/glasbey/_grids.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/glasbey/_internals.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/glasbey/prebuilt.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/glasbey/record.json
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/gnuplot/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/gnuplot/record.json
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/google/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/google/record.json
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/imagej/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/imagej/record.json
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/matlab/__init__.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/matlab/record.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/matplotlib/_CMRmap.py
+-rw-r--r--   0        0        0    45909 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/matplotlib/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/matplotlib/_coolwarm.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/matplotlib/_wistia.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/matplotlib/record.json
+-rw-r--r--   0        0        0    64086 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/seaborn/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/seaborn/record.json
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/tableau/__init__.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/tableau/record.json
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/vispy/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/vispy/record.json
+-rw-r--r--   0        0        0     7649 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/yorick/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 cmap-0.0.3/src/cmap/data/yorick/record.json
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_catalog.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_color.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_colormap.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_data.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_glasbey.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_model_fields.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_third_party.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 cmap-0.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cmap-0.0.3/.gitignore
+-rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 cmap-0.0.3/README.md
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 cmap-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_CMOCEAN
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_COLORBREWER
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_COLORCET
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_CRAMERI
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_CVIDIS
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_GLASBEY
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_WISTIA
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 cmap-0.0.3/LICENSE/LICENSE_YORICK
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 cmap-0.0.3/PKG-INFO
```

### Comparing `cmap-0.0.2/src/cmap/_color.py` & `cmap-0.0.3/src/cmap/_color.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/_colormap.py` & `cmap-0.0.3/src/cmap/_colormap.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/_external.py` & `cmap-0.0.3/src/cmap/_external.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,11 +161,11 @@
 
     # TODO: this is a side-effect
     console = get_console()
     color_cell = Text("")
     if cm.interpolation == "nearest":
         width = len(cm.color_stops)
     else:
-        width or (console.width - 12)
+        width = width or (console.width - 12)
     for color in cm.iter_colors(width):
         color_cell += Text(" ", style=Style(bgcolor=color.hex[:7]))
     console.print(color_cell)
```

### Comparing `cmap-0.0.2/src/cmap/_png.py` & `cmap-0.0.3/src/cmap/_png.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/_util.py` & `cmap-0.0.3/src/cmap/_util.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/bids/__init__.py` & `cmap-0.0.3/src/cmap/data/bids/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/bids/record.json` & `cmap-0.0.3/src/cmap/data/bids/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/chrisluts/record.json` & `cmap-0.0.3/src/cmap/data/chrisluts/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cividis/__init__.py` & `cmap-0.0.3/src/cmap/data/cividis/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cividis/record.json` & `cmap-0.0.3/src/cmap/data/cividis/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmap/record.json` & `cmap-0.0.3/src/cmap/data/cmap/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/algae.py` & `cmap-0.0.3/src/cmap/data/cmocean/algae.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/amp.py` & `cmap-0.0.3/src/cmap/data/cmocean/amp.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/balance.py` & `cmap-0.0.3/src/cmap/data/cmocean/balance.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/curl.py` & `cmap-0.0.3/src/cmap/data/cmocean/curl.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/deep.py` & `cmap-0.0.3/src/cmap/data/cmocean/deep.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/delta.py` & `cmap-0.0.3/src/cmap/data/cmocean/delta.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/dense.py` & `cmap-0.0.3/src/cmap/data/cmocean/dense.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/diff.py` & `cmap-0.0.3/src/cmap/data/cmocean/diff.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/haline.py` & `cmap-0.0.3/src/cmap/data/cmocean/haline.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/ice.py` & `cmap-0.0.3/src/cmap/data/cmocean/ice.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/matter.py` & `cmap-0.0.3/src/cmap/data/cmocean/matter.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/oxy.py` & `cmap-0.0.3/src/cmap/data/cmocean/oxy.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/phase.py` & `cmap-0.0.3/src/cmap/data/cmocean/phase.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/rain.py` & `cmap-0.0.3/src/cmap/data/cmocean/rain.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/record.json` & `cmap-0.0.3/src/cmap/data/cmocean/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/solar.py` & `cmap-0.0.3/src/cmap/data/cmocean/solar.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/speed.py` & `cmap-0.0.3/src/cmap/data/cmocean/speed.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/tarn.py` & `cmap-0.0.3/src/cmap/data/cmocean/tarn.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/tempo.py` & `cmap-0.0.3/src/cmap/data/cmocean/tempo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/thermal.py` & `cmap-0.0.3/src/cmap/data/cmocean/thermal.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/topo.py` & `cmap-0.0.3/src/cmap/data/cmocean/topo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cmocean/turbid.py` & `cmap-0.0.3/src/cmap/data/cmocean/turbid.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorbrewer/__init__.py` & `cmap-0.0.3/src/cmap/data/colorbrewer/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorbrewer/record.json` & `cmap-0.0.3/src/cmap/data/colorbrewer/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C10.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C11.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C3.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C4.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C5.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C6.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C7.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C8.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_C9.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_C9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBC1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBC1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBC2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBC2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBD1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBD1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBD2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBD2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBL1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBL1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBL2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBL2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBL3.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBL3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBL4.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBL4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBTC1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBTC1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBTC2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBTC2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBTD1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBTD1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL3.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_CBTL4.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_CBTL4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D10.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D11.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D12.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D12.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D13.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D13.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D1A.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D1A.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D3.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D4.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D5.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D6.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D7.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D8.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_D9.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_D9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_I1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_I1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_I2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_I2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_I3.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_I3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L10.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L10.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L11.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L11.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L12.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L12.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L13.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L13.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L14.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L14.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L15.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L15.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L16.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L16.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L17.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L17.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L18.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L18.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L19.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L19.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L20.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L20.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L3.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L4.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L5.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L5.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L6.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L6.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L7.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L7.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L8.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L8.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_L9.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_L9.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_R1.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_R1.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_R2.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_R2.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_R3.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_R3.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/CET_R4.py` & `cmap-0.0.3/src/cmap/data/colorcet/CET_R4.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/colorcet/__init__.py` & `cmap-0.0.3/src/cmap/data/colorcet/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/acton.py` & `cmap-0.0.3/src/cmap/data/crameri/acton.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/bam.py` & `cmap-0.0.3/src/cmap/data/crameri/bam.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/bamO.py` & `cmap-0.0.3/src/cmap/data/crameri/bamO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/bamako.py` & `cmap-0.0.3/src/cmap/data/crameri/bamako.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/batlow.py` & `cmap-0.0.3/src/cmap/data/crameri/batlow.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/batlowK.py` & `cmap-0.0.3/src/cmap/data/crameri/batlowK.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/batlowW.py` & `cmap-0.0.3/src/cmap/data/crameri/batlowW.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/berlin.py` & `cmap-0.0.3/src/cmap/data/crameri/berlin.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/bilbao.py` & `cmap-0.0.3/src/cmap/data/crameri/bilbao.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/broc.py` & `cmap-0.0.3/src/cmap/data/crameri/broc.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/brocO.py` & `cmap-0.0.3/src/cmap/data/crameri/brocO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/buda.py` & `cmap-0.0.3/src/cmap/data/crameri/buda.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/bukavu.py` & `cmap-0.0.3/src/cmap/data/crameri/bukavu.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/cork.py` & `cmap-0.0.3/src/cmap/data/crameri/cork.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/corkO.py` & `cmap-0.0.3/src/cmap/data/crameri/corkO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/davos.py` & `cmap-0.0.3/src/cmap/data/crameri/davos.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/devon.py` & `cmap-0.0.3/src/cmap/data/crameri/devon.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/fes.py` & `cmap-0.0.3/src/cmap/data/crameri/fes.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/grayC.py` & `cmap-0.0.3/src/cmap/data/crameri/grayC.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/hawaii.py` & `cmap-0.0.3/src/cmap/data/crameri/hawaii.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/imola.py` & `cmap-0.0.3/src/cmap/data/crameri/imola.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/lajolla.py` & `cmap-0.0.3/src/cmap/data/crameri/lajolla.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/lapaz.py` & `cmap-0.0.3/src/cmap/data/crameri/lapaz.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/lisbon.py` & `cmap-0.0.3/src/cmap/data/crameri/lisbon.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/nuuk.py` & `cmap-0.0.3/src/cmap/data/crameri/nuuk.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/oleron.py` & `cmap-0.0.3/src/cmap/data/crameri/oleron.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/oslo.py` & `cmap-0.0.3/src/cmap/data/crameri/oslo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/record.json` & `cmap-0.0.3/src/cmap/data/crameri/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/roma.py` & `cmap-0.0.3/src/cmap/data/crameri/roma.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/romaO.py` & `cmap-0.0.3/src/cmap/data/crameri/romaO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/tofino.py` & `cmap-0.0.3/src/cmap/data/crameri/tofino.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/tokyo.py` & `cmap-0.0.3/src/cmap/data/crameri/tokyo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/turku.py` & `cmap-0.0.3/src/cmap/data/crameri/turku.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/vanimo.py` & `cmap-0.0.3/src/cmap/data/crameri/vanimo.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/vik.py` & `cmap-0.0.3/src/cmap/data/crameri/vik.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/crameri/vikO.py` & `cmap-0.0.3/src/cmap/data/crameri/vikO.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/cubehelix/__init__.py` & `cmap-0.0.3/src/cmap/data/cubehelix/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/glasbey/__init__.py` & `cmap-0.0.3/src/cmap/data/glasbey/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/glasbey/_glasbey.py` & `cmap-0.0.3/src/cmap/data/glasbey/_glasbey.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/glasbey/_grids.py` & `cmap-0.0.3/src/cmap/data/glasbey/_grids.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/glasbey/_internals.py` & `cmap-0.0.3/src/cmap/data/glasbey/_internals.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/glasbey/prebuilt.py` & `cmap-0.0.3/src/cmap/data/glasbey/prebuilt.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/gnuplot/__init__.py` & `cmap-0.0.3/src/cmap/data/gnuplot/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/gnuplot/record.json` & `cmap-0.0.3/src/cmap/data/gnuplot/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/google/__init__.py` & `cmap-0.0.3/src/cmap/data/google/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/google/record.json` & `cmap-0.0.3/src/cmap/data/google/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/imagej/__init__.py` & `cmap-0.0.3/src/cmap/data/imagej/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/imagej/record.json` & `cmap-0.0.3/src/cmap/data/imagej/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/matlab/__init__.py` & `cmap-0.0.3/src/cmap/data/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/matlab/record.json` & `cmap-0.0.3/src/cmap/data/matlab/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/matplotlib/_CMRmap.py` & `cmap-0.0.3/src/cmap/data/matplotlib/_CMRmap.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/matplotlib/__init__.py` & `cmap-0.0.3/src/cmap/data/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/matplotlib/_coolwarm.py` & `cmap-0.0.3/src/cmap/data/matplotlib/_coolwarm.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/matplotlib/_wistia.py` & `cmap-0.0.3/src/cmap/data/matplotlib/_wistia.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/matplotlib/record.json` & `cmap-0.0.3/src/cmap/data/matplotlib/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/seaborn/__init__.py` & `cmap-0.0.3/src/cmap/data/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/seaborn/record.json` & `cmap-0.0.3/src/cmap/data/seaborn/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/tableau/__init__.py` & `cmap-0.0.3/src/cmap/data/tableau/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/tableau/record.json` & `cmap-0.0.3/src/cmap/data/tableau/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/vispy/__init__.py` & `cmap-0.0.3/src/cmap/data/vispy/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/vispy/record.json` & `cmap-0.0.3/src/cmap/data/vispy/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/yorick/__init__.py` & `cmap-0.0.3/src/cmap/data/yorick/__init__.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/src/cmap/data/yorick/record.json` & `cmap-0.0.3/src/cmap/data/yorick/record.json`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/tests/test_catalog.py` & `cmap-0.0.3/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/tests/test_color.py` & `cmap-0.0.3/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/tests/test_colormap.py` & `cmap-0.0.3/tests/test_colormap.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,11 +170,19 @@
 @pytest.fixture(params=(True, False))
 def with_or_without_PIL(request, monkeypatch):
     if not request.param:
         monkeypatch.setitem(sys.modules, "PIL", None)
     return request.param
 
 
+def test_cmap_info() -> None:
+    cm = Colormap("viridis")
+    assert cm.info
+    assert cm.info.qualified_name == "bids:viridis"
+    assert "matplotlib:viridis" in cm.info.aliases
+    assert "viridis" in cm.info.aliases
+
+
 def test_repr_notebook(with_or_without_PIL) -> None:
     cm = Colormap("viridis")
     assert "viridis" in cm._repr_html_()
     assert isinstance(cm._repr_png_(), bytes)
```

### Comparing `cmap-0.0.2/tests/test_data.py` & `cmap-0.0.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/tests/test_glasbey.py` & `cmap-0.0.3/tests/test_glasbey.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/tests/test_model_fields.py` & `cmap-0.0.3/tests/test_model_fields.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/tests/test_third_party.py` & `cmap-0.0.3/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/tests/test_utils.py` & `cmap-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/.gitignore` & `cmap-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/README.md` & `cmap-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
 The `cmap.Colormap` object has convenience methods that allow it to be used with a number of third-party colormap objects (like
 `matplotlib`, `vispy`, `napari`, `plotly`, etc...).
 
 See [documentation](https://cmap-docs.readthedocs.io/en/latest/colormaps/#usage-with-external-visualization-libraries)
 for details.
 
-If you would like to see support added for a particular library, please open an issue or PR. 
+If you would like to see support added for a particular library, please open an issue or PR.
 
 ## Alternatives
 
 Other libraries providing colormaps:
 
 
 - [matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html)
```

### Comparing `cmap-0.0.2/pyproject.toml` & `cmap-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 # https://hatch.pypa.io/latest/config/metadata/
 [tool.hatch.version]
 source = "vcs"
 
 # https://hatch.pypa.io/latest/config/build/#file-selection
 [tool.hatch.build.targets.sdist]
-include = ["/src", "/tests"]
+include = ["/src", "/tests", "CHANGELOG.md"]
 
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
 target-version = "py38"
 fix = true
```

### Comparing `cmap-0.0.2/LICENSE/LICENSE` & `cmap-0.0.3/LICENSE/LICENSE`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/LICENSE/LICENSE_CMOCEAN` & `cmap-0.0.3/LICENSE/LICENSE_CMOCEAN`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/LICENSE/LICENSE_COLORBREWER` & `cmap-0.0.3/LICENSE/LICENSE_COLORBREWER`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/LICENSE/LICENSE_CRAMERI` & `cmap-0.0.3/LICENSE/LICENSE_CRAMERI`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/LICENSE/LICENSE_CVIDIS` & `cmap-0.0.3/LICENSE/LICENSE_CVIDIS`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/LICENSE/LICENSE_GLASBEY` & `cmap-0.0.3/LICENSE/LICENSE_GLASBEY`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/LICENSE/LICENSE_WISTIA` & `cmap-0.0.3/LICENSE/LICENSE_WISTIA`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/LICENSE/LICENSE_YORICK` & `cmap-0.0.3/LICENSE/LICENSE_YORICK`

 * *Files identical despite different names*

### Comparing `cmap-0.0.2/PKG-INFO` & `cmap-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmap
-Version: 0.0.2
+Version: 0.0.3
 Summary: Scientific colormaps for python, without dependencies
 Project-URL: Homepage, https://github.com/tlambert03/cmap
 Project-URL: Repository, https://github.com/tlambert03/cmap
 Project-URL: Bug Tracker, https://github.com/tlambert03/cmap/issues
 Project-URL: Documentation, https://cmap-docs.rtfd.io/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
@@ -161,15 +161,15 @@
 
 The `cmap.Colormap` object has convenience methods that allow it to be used with a number of third-party colormap objects (like
 `matplotlib`, `vispy`, `napari`, `plotly`, etc...).
 
 See [documentation](https://cmap-docs.readthedocs.io/en/latest/colormaps/#usage-with-external-visualization-libraries)
 for details.
 
-If you would like to see support added for a particular library, please open an issue or PR. 
+If you would like to see support added for a particular library, please open an issue or PR.
 
 ## Alternatives
 
 Other libraries providing colormaps:
 
 
 - [matplotlib](https://matplotlib.org/stable/tutorials/colors/colormaps.html)
```

