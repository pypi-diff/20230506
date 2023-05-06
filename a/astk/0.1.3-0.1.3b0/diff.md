# Comparing `tmp/astk-0.1.3.tar.gz` & `tmp/astk-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astk-0.1.3.tar", last modified: Sat May  6 07:40:53 2023, max compression
+gzip compressed data, was "astk-0.1.3b0.tar", last modified: Sat May  6 07:30:25 2023, max compression
```

## Comparing `astk-0.1.3.tar` & `astk-0.1.3b0.tar`

### file list

```diff
@@ -1,419 +1,419 @@
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.825221 astk-0.1.3/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1527 2022-11-03 01:59:44.000000 astk-0.1.3/LICENSE
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       44 2022-11-03 01:59:44.000000 astk-0.1.3/MANIFEST.in
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1034 2023-05-06 07:40:53.824221 astk-0.1.3/PKG-INFO
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      762 2023-05-05 06:43:18.000000 astk-0.1.3/README.md
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.733221 astk-0.1.3/astk/
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.736221 astk-0.1.3/astk/R/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3672 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/CoSpliceNet.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      168 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/dl_keggdata.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2968 2023-05-04 06:15:41.000000 astk-0.1.3/astk/R/enrich.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3294 2023-05-04 06:46:26.000000 astk-0.1.3/astk/R/enrichCompare.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2869 2023-04-14 02:29:46.000000 astk-0.1.3/astk/R/gsea.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1048 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/gseaPlot.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2613 2023-04-30 07:09:14.000000 astk-0.1.3/astk/R/install.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      462 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/makeTxDb.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3259 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/motifMap.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      631 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/motifPlot.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      689 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/seqLogo.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1635 2022-11-03 01:59:44.000000 astk-0.1.3/astk/R/upset.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14912 2023-05-03 02:48:27.000000 astk-0.1.3/astk/R/utils.R
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        0 2023-02-20 01:59:46.000000 astk-0.1.3/astk/__init__.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.738222 astk-0.1.3/astk/cli/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      235 2023-03-11 08:22:05.000000 astk-0.1.3/astk/cli/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      491 2023-03-26 13:53:39.000000 astk-0.1.3/astk/cli/aliases.ini
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5031 2023-03-16 14:16:18.000000 astk-0.1.3/astk/cli/as_event.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8716 2023-05-03 06:40:12.000000 astk-0.1.3/astk/cli/config.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6144 2023-05-05 07:14:52.000000 astk-0.1.3/astk/cli/draw.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3445 2023-04-30 14:54:26.000000 astk-0.1.3/astk/cli/epi.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1816 2023-03-30 12:17:52.000000 astk-0.1.3/astk/cli/experiment.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7458 2023-05-04 06:46:28.000000 astk-0.1.3/astk/cli/gsea.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9104 2023-04-30 14:36:22.000000 astk-0.1.3/astk/cli/ml.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5632 2023-02-20 01:59:46.000000 astk-0.1.3/astk/cli/motif.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      928 2022-11-03 01:59:44.000000 astk-0.1.3/astk/cli/net.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8307 2023-04-10 12:32:20.000000 astk-0.1.3/astk/cli/seqfeature.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5551 2023-04-07 06:56:36.000000 astk-0.1.3/astk/cli/suppa.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11856 2023-03-13 06:26:06.000000 astk-0.1.3/astk/cli/utils.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4617 2023-03-04 08:32:09.000000 astk-0.1.3/astk/constant.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      237 2023-03-17 02:36:37.000000 astk-0.1.3/astk/ctypes.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.730222 astk-0.1.3/astk/data/
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.741222 astk-0.1.3/astk/data/maxent/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  1595043 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/maxent/ss3_score.json
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   472299 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/maxent/ss5seq_score.json
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.731222 astk-0.1.3/astk/data/motif/
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.748221 astk-0.1.3/astk/data/motif/ATtRACT/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4459 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1251 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      634 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Bombyx_mori.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      571 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Bos_taurus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      506 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Brachypodium_distachyon.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32322 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      502 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Chaetomium_thermophilum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      921 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Cricetulus_griseus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2679 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Danio_rerio.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    47701 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6358 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Gallus_gallus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   674737 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Homo_sapiens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2388 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Leishmania_major.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1454 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29005 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Mus_musculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      738 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Naegleria_gruberi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      776 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Nematostella_vectensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1309 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Neurospora_crassa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2523 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1352 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Oryzias_latipes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1274 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1937 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Physcomitrella_patens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      716 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4695 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11158 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Rattus_norvegicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      670 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    43405 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      629 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      682 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1540 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1307 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      687 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3021 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4015 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      836 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6096 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Xenopus_laevis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4865 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2441 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ATtRACT/Zea_mays.meme
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.795221 astk-0.1.3/astk/data/motif/CISBP-RNA/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14270 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18150 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1703 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37235 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2163 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5774 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31421 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18154 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20491 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Apis_mellifera.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4315 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3679 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2438 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2211 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1664 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2175 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2101 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1188 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1216 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13085 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Bombyx_mori.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38156 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Bos_taurus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3742 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19275 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5171 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Brugia_malayi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9824 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10312 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10846 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8805 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9823 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    40543 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      637 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_albicans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_glabrata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37241 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Canis_familiaris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15084 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Capitella_teleta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37866 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1655 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21518 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9963 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9399 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2236 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2760 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      642 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15784 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Culex_pipiens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15604 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    33623 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Danio_rerio.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15219 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23518 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31954 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23747 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22774 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21646 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26626 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24185 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19664 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22874 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23799 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20806 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21658 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22709 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24840 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28911 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1218 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35839 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Equus_caballus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24489 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20944 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Felis_catus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      659 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30729 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Gallus_gallus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31435 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4280 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Glycine_max.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37787 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11728 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    46774 2022-11-21 03:15:49.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Homo_sapiens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5292 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9004 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2451 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1666 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3189 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2680 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3043 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_major.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3171 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6695 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Loa_loa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13348 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3269 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35812 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37085 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26202 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2713 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3760 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3796 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3746 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1189 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28964 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5218 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1162 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Microsporum_canis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3780 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37066 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1177 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1709 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38188 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Mus_musculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2802 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1693 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1719 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28910 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      622 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16833 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2833 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10051 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Neospora_caninum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2642 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2234 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2799 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    27878 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4841 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29248 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37518 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2733 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Oryza_indica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3242 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Oryza_sativa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31120 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1656 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1153 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2134 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22825 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38413 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16093 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      649 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1683 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1720 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2209 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3736 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1173 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1145 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      638 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      647 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      711 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3812 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4317 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3995 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2756 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1705 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1674 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2714 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Podospora_anserina.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1200 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37096 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1713 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Postia_placenta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4162 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26820 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Procavia_capensis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3739 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Prunus_persica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35919 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6506 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38860 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1616 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3749 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ricinus_communis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1914 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2310 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1217 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1644 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5826 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2215 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3271 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1702 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23198 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Sorex_araneus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3224 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20742 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2145 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10832 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29388 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Sus_scrofa.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32434 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30452 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26504 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31987 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1125 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2817 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1715 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2207 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2786 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2794 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2546 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6932 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5682 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4326 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2773 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2735 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1682 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23608 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34596 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1146 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2212 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26009 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3777 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Volvox_carteri.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5691 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30403 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34934 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3236 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Zea_mays.meme
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.811221 astk-0.1.3/astk/data/motif/ELM/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    79014 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ELM/elm_classes.tsv
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   855778 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ELM/elm_instances.tsv
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003) 11720265 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ELM/hg38_alter_exon_seq.json
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  4375026 2022-11-03 01:59:44.000000 astk-0.1.3/astk/data/motif/ELM/mm10_alter_exon_seq.json
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.817221 astk-0.1.3/astk/draw/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      123 2022-11-03 01:59:44.000000 astk-0.1.3/astk/draw/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6863 2023-05-05 07:15:54.000000 astk-0.1.3/astk/draw/_func.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.818221 astk-0.1.3/astk/epi/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      236 2023-04-30 14:39:09.000000 astk-0.1.3/astk/epi/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7159 2023-04-30 14:52:01.000000 astk-0.1.3/astk/epi/_func.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.818221 astk-0.1.3/astk/event/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      152 2023-02-27 08:00:31.000000 astk-0.1.3/astk/event/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6026 2023-03-17 02:40:47.000000 astk-0.1.3/astk/event/_cli_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3009 2023-04-07 12:22:47.000000 astk-0.1.3/astk/event/eid.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.818221 astk-0.1.3/astk/gsea/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      237 2022-11-28 11:24:56.000000 astk-0.1.3/astk/gsea/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6330 2023-05-03 13:57:59.000000 astk-0.1.3/astk/gsea/_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1537 2023-03-08 12:39:17.000000 astk-0.1.3/astk/lazy_loader.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.819222 astk-0.1.3/astk/ml/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       89 2023-03-26 13:56:20.000000 astk-0.1.3/astk/ml/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2713 2023-03-26 13:56:20.000000 astk-0.1.3/astk/ml/_chunk_permutation_importance.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2869 2023-03-26 13:56:20.000000 astk-0.1.3/astk/ml/_metric.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4506 2023-03-30 12:07:57.000000 astk-0.1.3/astk/ml/_tools.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.820222 astk-0.1.3/astk/motif/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      151 2022-11-03 01:59:44.000000 astk-0.1.3/astk/motif/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6099 2023-03-11 07:50:42.000000 astk-0.1.3/astk/motif/_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1641 2022-11-03 01:59:44.000000 astk-0.1.3/astk/motif/elm.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.820222 astk-0.1.3/astk/network/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      132 2022-11-03 01:59:44.000000 astk-0.1.3/astk/network/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2358 2022-11-03 01:59:44.000000 astk-0.1.3/astk/network/_func.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.821221 astk-0.1.3/astk/seqfeature/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      121 2022-11-03 01:59:44.000000 astk-0.1.3/astk/seqfeature/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5220 2023-04-30 07:04:25.000000 astk-0.1.3/astk/seqfeature/_compare.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3774 2023-04-10 07:31:13.000000 astk-0.1.3/astk/seqfeature/_feature.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3735 2023-03-10 02:43:17.000000 astk-0.1.3/astk/seqfeature/_splice_score.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4067 2023-04-24 12:34:54.000000 astk-0.1.3/astk/seqfeature/feature.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.822221 astk-0.1.3/astk/suppa/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31571 2023-01-22 11:43:29.000000 astk-0.1.3/astk/suppa/AS_event.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       54 2023-04-07 08:57:38.000000 astk-0.1.3/astk/suppa/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7043 2023-04-07 12:40:54.000000 astk-0.1.3/astk/suppa/_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1236 2023-02-20 01:59:46.000000 astk-0.1.3/astk/suppa/event_psi.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4413 2023-02-20 01:59:46.000000 astk-0.1.3/astk/suppa/gtf_parse.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.823222 astk-0.1.3/astk/suppa/lib/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       84 2022-11-03 01:59:44.000000 astk-0.1.3/astk/suppa/lib/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23418 2022-11-03 01:59:44.000000 astk-0.1.3/astk/suppa/lib/diff_tools.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24715 2022-11-03 01:59:44.000000 astk-0.1.3/astk/suppa/lib/event.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8048 2022-11-03 01:59:44.000000 astk-0.1.3/astk/suppa/lib/gtf_store.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    12030 2022-11-03 01:59:44.000000 astk-0.1.3/astk/suppa/lib/optics.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22325 2022-11-03 01:59:44.000000 astk-0.1.3/astk/suppa/lib/tools.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24158 2022-11-03 01:59:44.000000 astk-0.1.3/astk/suppa/lib/var_event.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.824221 astk-0.1.3/astk/utils/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      173 2022-11-03 01:59:44.000000 astk-0.1.3/astk/utils/__init__.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3711 2023-04-30 14:57:10.000000 astk-0.1.3/astk/utils/_cli_func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9589 2023-04-10 12:32:19.000000 astk-0.1.3/astk/utils/_coord.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      537 2023-02-20 01:59:46.000000 astk-0.1.3/astk/utils/_getfasta.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15326 2023-05-03 13:44:10.000000 astk-0.1.3/astk/utils/func.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4513 2023-02-28 07:54:41.000000 astk-0.1.3/astk/utils/meta_template.py
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3970 2023-02-27 07:37:24.000000 astk-0.1.3/astk/utils/select.py
-drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:40:53.734222 astk-0.1.3/astk.egg-info/
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1034 2023-05-06 07:40:53.000000 astk-0.1.3/astk.egg-info/PKG-INFO
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    17588 2023-05-06 07:40:53.000000 astk-0.1.3/astk.egg-info/SOURCES.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        1 2023-05-06 07:40:53.000000 astk-0.1.3/astk.egg-info/dependency_links.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       42 2023-05-06 07:40:53.000000 astk-0.1.3/astk.egg-info/entry_points.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      189 2023-05-06 07:40:53.000000 astk-0.1.3/astk.egg-info/requires.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        5 2023-05-06 07:40:53.000000 astk-0.1.3/astk.egg-info/top_level.txt
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       38 2023-05-06 07:40:53.825221 astk-0.1.3/setup.cfg
--rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1189 2023-05-06 07:36:47.000000 astk-0.1.3/setup.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.880193 astk-0.1.3b0/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1527 2022-11-03 01:59:44.000000 astk-0.1.3b0/LICENSE
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       44 2022-11-03 01:59:44.000000 astk-0.1.3b0/MANIFEST.in
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1036 2023-05-06 07:30:25.880193 astk-0.1.3b0/PKG-INFO
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      762 2023-05-05 06:43:18.000000 astk-0.1.3b0/README.md
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.798193 astk-0.1.3b0/astk/
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.800193 astk-0.1.3b0/astk/R/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3672 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/CoSpliceNet.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      168 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/dl_keggdata.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2968 2023-05-04 06:15:41.000000 astk-0.1.3b0/astk/R/enrich.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3294 2023-05-04 06:46:26.000000 astk-0.1.3b0/astk/R/enrichCompare.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2869 2023-04-14 02:29:46.000000 astk-0.1.3b0/astk/R/gsea.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1048 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/gseaPlot.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2613 2023-04-30 07:09:14.000000 astk-0.1.3b0/astk/R/install.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      462 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/makeTxDb.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3259 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/motifMap.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      631 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/motifPlot.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      689 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/seqLogo.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1635 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/R/upset.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14912 2023-05-03 02:48:27.000000 astk-0.1.3b0/astk/R/utils.R
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        0 2023-02-20 01:59:46.000000 astk-0.1.3b0/astk/__init__.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.803193 astk-0.1.3b0/astk/cli/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      235 2023-03-11 08:22:05.000000 astk-0.1.3b0/astk/cli/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      491 2023-03-26 13:53:39.000000 astk-0.1.3b0/astk/cli/aliases.ini
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5031 2023-03-16 14:16:18.000000 astk-0.1.3b0/astk/cli/as_event.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8716 2023-05-03 06:40:12.000000 astk-0.1.3b0/astk/cli/config.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6144 2023-05-05 07:14:52.000000 astk-0.1.3b0/astk/cli/draw.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3445 2023-04-30 14:54:26.000000 astk-0.1.3b0/astk/cli/epi.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1816 2023-03-30 12:17:52.000000 astk-0.1.3b0/astk/cli/experiment.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7458 2023-05-04 06:46:28.000000 astk-0.1.3b0/astk/cli/gsea.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9104 2023-04-30 14:36:22.000000 astk-0.1.3b0/astk/cli/ml.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5632 2023-02-20 01:59:46.000000 astk-0.1.3b0/astk/cli/motif.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      928 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/cli/net.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8307 2023-04-10 12:32:20.000000 astk-0.1.3b0/astk/cli/seqfeature.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5551 2023-04-07 06:56:36.000000 astk-0.1.3b0/astk/cli/suppa.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11856 2023-03-13 06:26:06.000000 astk-0.1.3b0/astk/cli/utils.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4617 2023-03-04 08:32:09.000000 astk-0.1.3b0/astk/constant.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      237 2023-03-17 02:36:37.000000 astk-0.1.3b0/astk/ctypes.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.795193 astk-0.1.3b0/astk/data/
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.805193 astk-0.1.3b0/astk/data/maxent/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  1595043 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/maxent/ss3_score.json
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   472299 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/maxent/ss5seq_score.json
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.795193 astk-0.1.3b0/astk/data/motif/
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.812193 astk-0.1.3b0/astk/data/motif/ATtRACT/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4459 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1251 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      634 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Bombyx_mori.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      571 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Bos_taurus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      506 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Brachypodium_distachyon.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32322 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      502 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Chaetomium_thermophilum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      921 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Cricetulus_griseus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2679 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Danio_rerio.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    47701 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6358 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Gallus_gallus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   674737 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Homo_sapiens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2388 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Leishmania_major.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1454 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29005 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Mus_musculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      738 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Naegleria_gruberi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      776 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Nematostella_vectensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1309 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Neurospora_crassa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2523 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1352 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Oryzias_latipes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1274 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1937 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Physcomitrella_patens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      716 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4695 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11158 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Rattus_norvegicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      670 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    43405 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      629 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      682 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1540 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1307 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      687 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3021 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4015 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      836 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6096 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Xenopus_laevis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4865 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2441 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ATtRACT/Zea_mays.meme
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.856193 astk-0.1.3b0/astk/data/motif/CISBP-RNA/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    14270 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18150 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1703 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37235 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2163 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5774 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31421 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    18154 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20491 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Apis_mellifera.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4315 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3679 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2438 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2211 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1664 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2175 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2101 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1188 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1216 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13085 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Bombyx_mori.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38156 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Bos_taurus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3742 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19275 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5171 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Brugia_malayi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9824 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10312 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10846 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8805 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9823 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    40543 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      637 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_albicans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_glabrata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37241 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Canis_familiaris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15084 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Capitella_teleta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1143 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37866 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1157 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1655 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21518 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9963 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9399 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1172 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2236 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2718 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2760 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      642 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15784 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Culex_pipiens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15604 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    33623 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Danio_rerio.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15219 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23518 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31954 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23747 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22774 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21646 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26626 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24185 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    19664 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22874 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23799 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20806 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    21658 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22709 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24840 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28911 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1218 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35839 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Equus_caballus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24489 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20944 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Felis_catus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      659 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30729 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Gallus_gallus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31435 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4280 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Glycine_max.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37787 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    11728 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    46774 2022-11-21 03:15:49.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Homo_sapiens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5292 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9004 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2451 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1666 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3189 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2680 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3043 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_major.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3171 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6695 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Loa_loa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    13348 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3269 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35812 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37085 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26202 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2713 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3760 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3796 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3746 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1189 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28964 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5218 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1162 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Microsporum_canis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3780 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37066 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1177 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1709 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38188 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mus_musculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2802 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1693 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1719 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    28910 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      622 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16833 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2833 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10051 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neospora_caninum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2642 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2234 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2799 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    27878 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4841 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29248 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37518 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2733 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryza_indica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3242 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryza_sativa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31120 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1656 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1153 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2134 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22825 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38413 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    16093 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2171 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      649 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1683 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1720 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2209 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3736 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1173 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1145 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      638 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      647 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      711 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3812 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4317 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3995 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3791 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2756 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1705 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1674 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2714 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Podospora_anserina.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1200 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    37096 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4245 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1713 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Postia_placenta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4162 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26820 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Procavia_capensis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3739 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Prunus_persica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    35919 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6506 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    38860 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1616 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3749 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ricinus_communis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1914 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2310 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1217 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2464 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1644 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3721 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5826 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2215 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1152 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      639 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3271 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1702 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23198 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sorex_araneus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3224 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    20742 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2145 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    10832 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    29388 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sus_scrofa.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    32434 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30452 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26504 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31987 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1125 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      643 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2817 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1715 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2207 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2786 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2794 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2546 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1661 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1658 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6932 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5682 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4326 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2773 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2735 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1682 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23608 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34596 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2167 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1146 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1149 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2212 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    26009 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3777 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      660 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Volvox_carteri.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5691 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    30403 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    34934 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      645 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3236 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Zea_mays.meme
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2461 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.869193 astk-0.1.3b0/astk/data/motif/ELM/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    79014 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ELM/elm_classes.tsv
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)   855778 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ELM/elm_instances.tsv
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003) 11720265 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ELM/hg38_alter_exon_seq.json
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)  4375026 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/data/motif/ELM/mm10_alter_exon_seq.json
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.873193 astk-0.1.3b0/astk/draw/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      123 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/draw/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6863 2023-05-05 07:15:54.000000 astk-0.1.3b0/astk/draw/_func.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.874193 astk-0.1.3b0/astk/epi/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      236 2023-04-30 14:39:09.000000 astk-0.1.3b0/astk/epi/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7159 2023-04-30 14:52:01.000000 astk-0.1.3b0/astk/epi/_func.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.874193 astk-0.1.3b0/astk/event/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      152 2023-02-27 08:00:31.000000 astk-0.1.3b0/astk/event/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6026 2023-03-17 02:40:47.000000 astk-0.1.3b0/astk/event/_cli_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3009 2023-04-07 12:22:47.000000 astk-0.1.3b0/astk/event/eid.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.874193 astk-0.1.3b0/astk/gsea/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      237 2022-11-28 11:24:56.000000 astk-0.1.3b0/astk/gsea/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6330 2023-05-03 13:57:59.000000 astk-0.1.3b0/astk/gsea/_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1537 2023-03-08 12:39:17.000000 astk-0.1.3b0/astk/lazy_loader.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.875193 astk-0.1.3b0/astk/ml/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       89 2023-03-26 13:56:20.000000 astk-0.1.3b0/astk/ml/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2713 2023-03-26 13:56:20.000000 astk-0.1.3b0/astk/ml/_chunk_permutation_importance.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2869 2023-03-26 13:56:20.000000 astk-0.1.3b0/astk/ml/_metric.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4506 2023-03-30 12:07:57.000000 astk-0.1.3b0/astk/ml/_tools.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.875193 astk-0.1.3b0/astk/motif/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      151 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/motif/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     6099 2023-03-11 07:50:42.000000 astk-0.1.3b0/astk/motif/_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1641 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/motif/elm.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.876193 astk-0.1.3b0/astk/network/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      132 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/network/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     2358 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/network/_func.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.877193 astk-0.1.3b0/astk/seqfeature/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      121 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/seqfeature/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     5220 2023-04-30 07:04:25.000000 astk-0.1.3b0/astk/seqfeature/_compare.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3774 2023-04-10 07:31:13.000000 astk-0.1.3b0/astk/seqfeature/_feature.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3735 2023-03-10 02:43:17.000000 astk-0.1.3b0/astk/seqfeature/_splice_score.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4067 2023-04-24 12:34:54.000000 astk-0.1.3b0/astk/seqfeature/feature.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.877193 astk-0.1.3b0/astk/suppa/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    31571 2023-01-22 11:43:29.000000 astk-0.1.3b0/astk/suppa/AS_event.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       54 2023-04-07 08:57:38.000000 astk-0.1.3b0/astk/suppa/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     7043 2023-04-07 12:40:54.000000 astk-0.1.3b0/astk/suppa/_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1236 2023-02-20 01:59:46.000000 astk-0.1.3b0/astk/suppa/event_psi.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4413 2023-02-20 01:59:46.000000 astk-0.1.3b0/astk/suppa/gtf_parse.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.878193 astk-0.1.3b0/astk/suppa/lib/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       84 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/suppa/lib/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    23418 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/suppa/lib/diff_tools.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24715 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/suppa/lib/event.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     8048 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/suppa/lib/gtf_store.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    12030 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/suppa/lib/optics.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    22325 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/suppa/lib/tools.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    24158 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/suppa/lib/var_event.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.880193 astk-0.1.3b0/astk/utils/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      173 2022-11-03 01:59:44.000000 astk-0.1.3b0/astk/utils/__init__.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3711 2023-04-30 14:57:10.000000 astk-0.1.3b0/astk/utils/_cli_func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     9589 2023-04-10 12:32:19.000000 astk-0.1.3b0/astk/utils/_coord.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      537 2023-02-20 01:59:46.000000 astk-0.1.3b0/astk/utils/_getfasta.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    15326 2023-05-03 13:44:10.000000 astk-0.1.3b0/astk/utils/func.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     4513 2023-02-28 07:54:41.000000 astk-0.1.3b0/astk/utils/meta_template.py
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     3970 2023-02-27 07:37:24.000000 astk-0.1.3b0/astk/utils/select.py
+drwxrwxr-x   0 huangsh   (1003) huangsh   (1003)        0 2023-05-06 07:30:25.799193 astk-0.1.3b0/astk.egg-info/
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1036 2023-05-06 07:30:25.000000 astk-0.1.3b0/astk.egg-info/PKG-INFO
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)    17588 2023-05-06 07:30:25.000000 astk-0.1.3b0/astk.egg-info/SOURCES.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        1 2023-05-06 07:30:25.000000 astk-0.1.3b0/astk.egg-info/dependency_links.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       42 2023-05-06 07:30:25.000000 astk-0.1.3b0/astk.egg-info/entry_points.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)      189 2023-05-06 07:30:25.000000 astk-0.1.3b0/astk.egg-info/requires.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)        5 2023-05-06 07:30:25.000000 astk-0.1.3b0/astk.egg-info/top_level.txt
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)       38 2023-05-06 07:30:25.880193 astk-0.1.3b0/setup.cfg
+-rw-rw-r--   0 huangsh   (1003) huangsh   (1003)     1190 2023-05-06 07:30:18.000000 astk-0.1.3b0/setup.py
```

### Comparing `astk-0.1.3/LICENSE` & `astk-0.1.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/PKG-INFO` & `astk-0.1.3b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astk
-Version: 0.1.3
+Version: 0.1.3b0
 Summary: A comprehensive toolkit for alternative splicing analysis
 Home-page: https://github.com/huang-sh/astk/
 Author: huangsh
 Author-email: hsh-me@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `astk-0.1.3/README.md` & `astk-0.1.3b0/README.md`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/CoSpliceNet.R` & `astk-0.1.3b0/astk/R/CoSpliceNet.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/enrich.R` & `astk-0.1.3b0/astk/R/enrich.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/enrichCompare.R` & `astk-0.1.3b0/astk/R/enrichCompare.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/gsea.R` & `astk-0.1.3b0/astk/R/gsea.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/gseaPlot.R` & `astk-0.1.3b0/astk/R/gseaPlot.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/install.R` & `astk-0.1.3b0/astk/R/install.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/motifMap.R` & `astk-0.1.3b0/astk/R/motifMap.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/motifPlot.R` & `astk-0.1.3b0/astk/R/motifPlot.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/seqLogo.R` & `astk-0.1.3b0/astk/R/seqLogo.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/upset.R` & `astk-0.1.3b0/astk/R/upset.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/R/utils.R` & `astk-0.1.3b0/astk/R/utils.R`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/as_event.py` & `astk-0.1.3b0/astk/cli/as_event.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/config.py` & `astk-0.1.3b0/astk/cli/config.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/draw.py` & `astk-0.1.3b0/astk/cli/draw.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/epi.py` & `astk-0.1.3b0/astk/cli/epi.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/experiment.py` & `astk-0.1.3b0/astk/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/gsea.py` & `astk-0.1.3b0/astk/cli/gsea.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/ml.py` & `astk-0.1.3b0/astk/cli/ml.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/motif.py` & `astk-0.1.3b0/astk/cli/motif.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/net.py` & `astk-0.1.3b0/astk/cli/net.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/seqfeature.py` & `astk-0.1.3b0/astk/cli/seqfeature.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/suppa.py` & `astk-0.1.3b0/astk/cli/suppa.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/cli/utils.py` & `astk-0.1.3b0/astk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/constant.py` & `astk-0.1.3b0/astk/constant.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/maxent/ss3_score.json` & `astk-0.1.3b0/astk/data/maxent/ss3_score.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/maxent/ss5seq_score.json` & `astk-0.1.3b0/astk/data/maxent/ss5seq_score.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Arabidopsis_thaliana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Aspergillus_nidulans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Bombyx_mori.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Bombyx_mori.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Bos_taurus.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Bos_taurus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Caenorhabditis_elegans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Cricetulus_griseus.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Cricetulus_griseus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Danio_rerio.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Danio_rerio.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Drosophila_melanogaster.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Gallus_gallus.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Gallus_gallus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Homo_sapiens.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Homo_sapiens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Leishmania_major.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Leishmania_major.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Mesocricetus_auratus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Mus_musculus.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Mus_musculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Naegleria_gruberi.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Naegleria_gruberi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Nematostella_vectensis.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Nematostella_vectensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Neurospora_crassa.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Neurospora_crassa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Oryctolagus_cuniculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Oryzias_latipes.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Oryzias_latipes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Ostreococcus_tauri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Physcomitrella_patens.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Physcomitrella_patens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Phytophthora_ramorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Plasmodium_falciparum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Rattus_norvegicus.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Rattus_norvegicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Rhizopus_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Saccharomyces_cerevisiae_s288c.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Schistosoma_mansoni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Spodoptera_frugiperda.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Tetraodon_nigroviridis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Thalassiosira_pseudonana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Trichomonas_vaginalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Trypanosoma_brucei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Vanderwaltozyma_polyspora.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Xenopus_laevis.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Xenopus_laevis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Xenopus_tropicalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ATtRACT/Zea_mays.meme` & `astk-0.1.3b0/astk/data/motif/ATtRACT/Zea_mays.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Acyrtosiphon_pisum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aedes_aegypti.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Agaricus_bisporus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ailuropoda_melanoleuca.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Allomyces_macrogynus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Alternaria_brassicicola.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Amphimedon_queenslandica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Anolis_carolinensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Anopheles_gambiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Apis_mellifera.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Apis_mellifera.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Arabidopsis_lyrata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Arabidopsis_thaliana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Arthroderma_benhamiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ashbya_gossypii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_carbonarius.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_clavatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_flavus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_fumigatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_nidulans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_niger.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aspergillus_terreus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Aureococcus_anophagefferens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Batrachochytrium_dendrobatidis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Blastomyces_dermatitidis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Bombyx_mori.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Bombyx_mori.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Bos_taurus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Bos_taurus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Botrytis_cinerea.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Brachypodium_distachyon.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Branchiostoma_floridae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Brugia_malayi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Brugia_malayi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_brenneri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_briggsae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_elegans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_japonica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Caenorhabditis_remanei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Callithrix_jacchus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_albicans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_albicans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_dubliniensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_glabrata.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_glabrata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_guilliermondii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_lusitaniae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_parapsilosis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Candida_tropicalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Canis_familiaris.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Canis_familiaris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cannabis_sativa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Capitella_teleta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Capitella_teleta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Capsaspora_owczarzaki.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cavia_porcellus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chaetomium_globosum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chlamydomonas_reinhardtii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chlorella_NC64A.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Chlorella_vulgaris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Choloepus_hoffmanni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ciona_intestinalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ciona_savignyi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coccidioides_immitis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coccidioides_posadasii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coccomyxa_C_169.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cochliobolus_heterostrophus_C5.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Colletotrichum_graminicola.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Coprinopsis_cinerea.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cryphonectria_parasitica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cryptosporidium_hominis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cryptosporidium_parvum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Cucumis_sativus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Culex_pipiens.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Culex_pipiens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Culex_quinquefasciatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Danio_rerio.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Danio_rerio.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Daphnia_pulex.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dasypus_novemcinctus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Debaryomyces_hansenii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dictyostelium_discoideum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dictyostelium_purpureum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Dipodomys_ordii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_ananassae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_erecta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_grimshawi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_melanogaster.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_mojavensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_persimilis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_pseudoobscura.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_sechellia.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_simulans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_virilis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_willistoni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Drosophila_yakuba.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Echinops_telfairi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Emiliania_huxleyi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Equus_caballus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Equus_caballus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Erinaceus_europaeus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Felis_catus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Felis_catus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fragilariopsis_cylindrus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fusarium_graminearum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fusarium_oxysporum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Fusarium_verticillioides.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Gallus_gallus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Gallus_gallus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Gasterosteus_aculeatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Glycine_max.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Glycine_max.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Gorilla_gorilla.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Helobdella_robusta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Heterobasidion_annosum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Histoplasma_capsulatum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Homo_sapiens.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Homo_sapiens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Hydra_magnipapillata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ixodes_scapularis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Kluyveromyces_lactis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Kluyveromyces_thermotolerans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Kluyveromyces_waltii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Laccaria_bicolor.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lachancea_kluyveri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_braziliensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_infantum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_major.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_major.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Leishmania_mexicana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Loa_loa.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Loa_loa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lodderomyces_elongisporus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lottia_gigantea.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Lotus_japonicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Loxodonta_africana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Macaca_mulatta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Macropus_eugenii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Magnaporthe_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Malassezia_globosa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Malus_x_domestica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Manihot_esculenta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Medicago_truncatula.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Melampsora_laricis_populina.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Meleagris_gallopavo.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Meloidogyne_incognita.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Microcebus_murinus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Micromonas_pusilla.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Microsporum_canis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Microsporum_canis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Microsporum_gypseum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mimulus_guttatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Monodelphis_domestica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Monosiga_brevicollis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mucor_circinelloides.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Mus_musculus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mus_musculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Myceliophthora_thermophila.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mycosphaerella_fijiensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Mycosphaerella_graminicola.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Myotis_lucifugus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Naegleria_gruberi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Nasonia_vitripennis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Nectria_haematococca.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Nematostella_vectensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neosartorya_fischeri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Neospora_caninum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neospora_caninum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neurospora_crassa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neurospora_discreta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Neurospora_tetrasperma.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ochotona_princeps.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oikopleura_dioica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ornithorhynchus_anatinus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryctolagus_cuniculus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Oryza_indica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryza_indica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Oryza_sativa.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryza_sativa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Oryzias_latipes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ostreococcus_RCC809.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ostreococcus_lucimarinus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ostreococcus_tauri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Otolemur_garnettii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pan_troglodytes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Paracoccidioides_brasiliensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pediculus_humanus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Penicillium_chrysogenum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Penicillium_marneffei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phaeodactylum_tricornutum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phaeosphaeria_nodorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phanerochaete_chrysosporium.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phoenix_dactylifera.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phycomyces_blakesleeanus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Physcomitrella_patens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_capsici.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_infestans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_ramorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Phytophthora_sojae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pichia_pastoris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pichia_stipitis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_berghei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_chabaudi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_falciparum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_knowlesi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_vivax.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Plasmodium_yoelii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pleurotus_ostreatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pneumocystis_carinii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Podospora_anserina.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Podospora_anserina.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Polysphondylium_pallidum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pongo_pygmaeus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Populus_trichocarpa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Postia_placenta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Postia_placenta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pristionchus_pacificus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Procavia_capensis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Procavia_capensis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Prunus_persica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Prunus_persica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pteropus_vampyrus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Pyrenophora_tritici_repentis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/RNAcompete_CONSTRUCTS.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Rattus_norvegicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Rhizopus_oryzae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ricinus_communis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ricinus_communis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_bayanus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_castellii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_cerevisiae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_kudriavzevii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_mikatae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saccharomyces_paradoxus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Salpingoeca_rosetta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Saprolegnia_parasitica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schistosoma_japonicum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schistosoma_mansoni.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizophyllum_commune.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_cryophilus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_japonicus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_octosporus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Schizosaccharomyces_pombe.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sclerotinia_sclerotiorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Selaginella_moellendorfii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Serpula_lacrymans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Sorex_araneus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sorex_araneus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sorghum_bicolor.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Spermophilus_tridecemlineatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Spizellomyces_punctatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sporobolomyces_roseus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Stagonospora_nodorum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Strongylocentrotus_purpuratus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Sus_scrofa.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Sus_scrofa.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Taeniopygia_guttata.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Takifugu_rubripes.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tarsius_syrichta.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tetraodon_nigroviridis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Thalassiosira_pseudonana.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Thecamonas_trahens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Thielavia_terrestris.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Toxoplasma_gondii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tremella_mesenterica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tribolium_castaneum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoderma_atroviride.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoderma_reesei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoderma_virens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichomonas_vaginalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_equinum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_rubrum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_tonsurans.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichophyton_verrucosum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trichoplax_adhaerens.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_brucei.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_congolense.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_cruzi.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Trypanosoma_vivax.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tuber_melanosporum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tupaia_belangeri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Tursiops_truncatus.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Uncinocarpus_reesii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Ustilago_maydis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Vanderwaltozyma_polyspora.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Verticillium_albo_atrum.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Verticillium_dahliae.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Vicugna_pacos.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Vitis_vinifera.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Volvox_carteri.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Volvox_carteri.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Wuchereria_bancrofti.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Xenopus_laevis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Xenopus_tropicalis.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Yarrowia_lipolytica.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Zea_mays.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Zea_mays.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme` & `astk-0.1.3b0/astk/data/motif/CISBP-RNA/Zygosaccharomyces_rouxii.meme`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ELM/elm_classes.tsv` & `astk-0.1.3b0/astk/data/motif/ELM/elm_classes.tsv`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ELM/elm_instances.tsv` & `astk-0.1.3b0/astk/data/motif/ELM/elm_instances.tsv`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ELM/hg38_alter_exon_seq.json` & `astk-0.1.3b0/astk/data/motif/ELM/hg38_alter_exon_seq.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/data/motif/ELM/mm10_alter_exon_seq.json` & `astk-0.1.3b0/astk/data/motif/ELM/mm10_alter_exon_seq.json`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/draw/_func.py` & `astk-0.1.3b0/astk/draw/_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/epi/_func.py` & `astk-0.1.3b0/astk/epi/_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/event/_cli_func.py` & `astk-0.1.3b0/astk/event/_cli_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/event/eid.py` & `astk-0.1.3b0/astk/event/eid.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/gsea/_func.py` & `astk-0.1.3b0/astk/gsea/_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/lazy_loader.py` & `astk-0.1.3b0/astk/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/ml/_chunk_permutation_importance.py` & `astk-0.1.3b0/astk/ml/_chunk_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/ml/_metric.py` & `astk-0.1.3b0/astk/ml/_metric.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/ml/_tools.py` & `astk-0.1.3b0/astk/ml/_tools.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/motif/_func.py` & `astk-0.1.3b0/astk/motif/_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/motif/elm.py` & `astk-0.1.3b0/astk/motif/elm.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/network/_func.py` & `astk-0.1.3b0/astk/network/_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/seqfeature/_compare.py` & `astk-0.1.3b0/astk/seqfeature/_compare.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/seqfeature/_feature.py` & `astk-0.1.3b0/astk/seqfeature/_feature.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/seqfeature/_splice_score.py` & `astk-0.1.3b0/astk/seqfeature/_splice_score.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/seqfeature/feature.py` & `astk-0.1.3b0/astk/seqfeature/feature.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/AS_event.py` & `astk-0.1.3b0/astk/suppa/AS_event.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/_func.py` & `astk-0.1.3b0/astk/suppa/_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/event_psi.py` & `astk-0.1.3b0/astk/suppa/event_psi.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/gtf_parse.py` & `astk-0.1.3b0/astk/suppa/gtf_parse.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/lib/diff_tools.py` & `astk-0.1.3b0/astk/suppa/lib/diff_tools.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/lib/event.py` & `astk-0.1.3b0/astk/suppa/lib/event.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/lib/gtf_store.py` & `astk-0.1.3b0/astk/suppa/lib/gtf_store.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/lib/optics.py` & `astk-0.1.3b0/astk/suppa/lib/optics.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/lib/tools.py` & `astk-0.1.3b0/astk/suppa/lib/tools.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/suppa/lib/var_event.py` & `astk-0.1.3b0/astk/suppa/lib/var_event.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/utils/_cli_func.py` & `astk-0.1.3b0/astk/utils/_cli_func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/utils/_coord.py` & `astk-0.1.3b0/astk/utils/_coord.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/utils/_getfasta.py` & `astk-0.1.3b0/astk/utils/_getfasta.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/utils/func.py` & `astk-0.1.3b0/astk/utils/func.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/utils/meta_template.py` & `astk-0.1.3b0/astk/utils/meta_template.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk/utils/select.py` & `astk-0.1.3b0/astk/utils/select.py`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/astk.egg-info/PKG-INFO` & `astk-0.1.3b0/astk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astk
-Version: 0.1.3
+Version: 0.1.3b0
 Summary: A comprehensive toolkit for alternative splicing analysis
 Home-page: https://github.com/huang-sh/astk/
 Author: huangsh
 Author-email: hsh-me@outlook.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `astk-0.1.3/astk.egg-info/SOURCES.txt` & `astk-0.1.3b0/astk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astk-0.1.3/setup.py` & `astk-0.1.3b0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 
 setup(
     name="astk",
-    version="0.1.3",
+    version="0.1.3b",
     url='https://github.com/huang-sh/astk/',
     author='huangsh',
     author_email='hsh-me@outlook.com',
     packages=find_packages(), 
     description="A comprehensive toolkit for alternative splicing analysis",
     long_description=description,
     long_description_content_type="text/markdown",
```

